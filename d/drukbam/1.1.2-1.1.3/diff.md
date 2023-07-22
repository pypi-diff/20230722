# Comparing `tmp/DrukBam-1.1.2.tar.gz` & `tmp/drukbam-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DrukBam-1.1.2.tar", max compression
+gzip compressed data, was "drukbam-1.1.3.tar", max compression
```

## Comparing `DrukBam-1.1.2.tar` & `drukbam-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    15495 2021-10-03 19:57:22.049386 DrukBam-1.1.2/DrukBam/MapPlot.py
--rw-r--r--   0        0        0    15658 2021-10-04 20:01:22.101340 DrukBam-1.1.2/DrukBam/PlotCalc.py
--rw-r--r--   0        0        0       36 2021-09-05 09:39:09.274450 DrukBam-1.1.2/DrukBam/__init__.py
--rw-r--r--   0        0        0     6326 2021-09-26 10:39:40.724305 DrukBam-1.1.2/DrukBam/__main__.py
--rw-r--r--   0        0        0    10929 2021-09-25 10:36:45.911285 DrukBam-1.1.2/DrukBam/bamCalc.py
--rw-r--r--   0        0        0      403 2021-10-04 19:55:17.583471 DrukBam-1.1.2/DrukBam/classic.ini
--rw-r--r--   0        0        0      799 2021-09-05 09:39:09.275450 DrukBam-1.1.2/DrukBam/setup.py
--rw-r--r--   0        0        0     2183 2021-09-25 16:08:52.511471 DrukBam-1.1.2/DrukBam/vcfParse.py
--rw-r--r--   0        0        0      646 2021-10-04 20:07:20.144651 DrukBam-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      877 2021-10-04 20:07:45.260711 DrukBam-1.1.2/setup.py
--rw-r--r--   0        0        0      633 2021-10-04 20:07:45.261009 DrukBam-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    15495 2023-07-22 10:22:08.767745 drukbam-1.1.3/DrukBam/MapPlot.py
+-rw-r--r--   0        0        0    15779 2023-07-22 10:30:31.051968 drukbam-1.1.3/DrukBam/PlotCalc.py
+-rw-r--r--   0        0        0       36 2023-07-22 10:22:08.768745 drukbam-1.1.3/DrukBam/__init__.py
+-rw-r--r--   0        0        0     6326 2023-07-22 10:22:08.768745 drukbam-1.1.3/DrukBam/__main__.py
+-rw-r--r--   0        0        0    10929 2023-07-22 10:22:08.769745 drukbam-1.1.3/DrukBam/bamCalc.py
+-rw-r--r--   0        0        0      388 2023-07-22 10:22:08.769745 drukbam-1.1.3/DrukBam/classic.ini
+-rw-r--r--   0        0        0      799 2023-07-22 10:22:08.769745 drukbam-1.1.3/DrukBam/setup.py
+-rw-r--r--   0        0        0     2183 2023-07-22 10:22:08.769745 drukbam-1.1.3/DrukBam/vcfParse.py
+-rw-r--r--   0        0        0      646 2023-07-22 10:34:23.806286 drukbam-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 drukbam-1.1.3/PKG-INFO
```

### Comparing `DrukBam-1.1.2/DrukBam/MapPlot.py` & `drukbam-1.1.3/DrukBam/MapPlot.py`

 * *Files identical despite different names*

### Comparing `DrukBam-1.1.2/DrukBam/PlotCalc.py` & `drukbam-1.1.3/DrukBam/PlotCalc.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,15 +183,14 @@
         rangeEnd=end-diffEnd
         x=size
         if rangeEnd==end:
             x=0
         sizeChunks=list(range(rangeStart,rangeEnd+x,size))
         chunks=[start]+sizeChunks+[end]
         if type(vcfPos)==int:
-            print('here')
             chunks=chunks+[vcfPos]
             chunks.sort()
         return chunks
 
 
 
     def AxSet(self,ax,start,end,chunk=False,direction='all',vcf=False):
@@ -281,22 +280,25 @@
                     fastaChunk=str(fa.fetch(self.chrom,s,e)).upper()
             e=e+1
             s=s+1
             if y>self.maxHeight:
                 ax.plot((s,e),(self.maxHeight+1,self.maxHeight+1),color=self.colorDict['max coverage'],alpha=0.1)
                 continue
 
-            chunk_cigarstring=self.CigChunker(cig)
+            chunk_cigarstring_orig=self.CigChunker(cig)
             query_alignment_sequence=qS
-            chunkL=len(chunk_cigarstring)
-            chunk_cigarstringS=[x for x in chunk_cigarstring if x =='S' or x =='H']
-            chunk_cigarstring=[x for x in chunk_cigarstring if x !='S' and x !='H']
+            chunkL=len(chunk_cigarstring_orig)
+            chunk_cigarstringS=[x for x in chunk_cigarstring_orig if x =='S' or x =='H']
+            chunk_cigarstring=[x for x in chunk_cigarstring_orig if x !='S' and x !='H'  and x!='D']
 
             ipos=[x for x,y in enumerate(chunk_cigarstring) if y=='I']
             ipos=self.listConsec(ipos)
+            
+            chunk_cigarstring=[x for x in chunk_cigarstring_orig if x !='S' and x !='H']
+            
             chunk_cigarstring=[x for x in chunk_cigarstring if x !='I']
             iposCounter=0
 
             for i in ipos:
                 query_alignment_sequence="".join([x for _,x in enumerate(query_alignment_sequence) if _+iposCounter not in i])
                 iposCounter=iposCounter+len(i)
```

### Comparing `DrukBam-1.1.2/DrukBam/__main__.py` & `drukbam-1.1.3/DrukBam/__main__.py`

 * *Files identical despite different names*

### Comparing `DrukBam-1.1.2/DrukBam/bamCalc.py` & `drukbam-1.1.3/DrukBam/bamCalc.py`

 * *Files identical despite different names*

### Comparing `DrukBam-1.1.2/DrukBam/setup.py` & `drukbam-1.1.3/DrukBam/setup.py`

 * *Files identical despite different names*

### Comparing `DrukBam-1.1.2/DrukBam/vcfParse.py` & `drukbam-1.1.3/DrukBam/vcfParse.py`

 * *Files identical despite different names*

### Comparing `DrukBam-1.1.2/pyproject.toml` & `drukbam-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "DrukBam"
 homepage = "https://github.com/StephanHolgerD/DrukBam"
-version = "1.1.2"
+version = "1.1.3"
 description = "Comandline plotting of sort,indexed bam files"
 authors = ["Stephan Holger Drukewitz"]
 license = "MIT"
 packages = [
     {include = "DrukBam"}
 ]
```

### Comparing `DrukBam-1.1.2/PKG-INFO` & `drukbam-1.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: drukbam
-Version: 1.1.2
+Version: 1.1.3
 Summary: Comandline plotting of sort,indexed bam files
 Home-page: https://github.com/StephanHolgerD/DrukBam
 License: MIT
 Author: Stephan Holger Drukewitz
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cython (>=0.29,<0.30)
 Requires-Dist: matplotlib (>=3.4.2,<4.0.0)
 Requires-Dist: pandas (>=1.2.4,<2.0.0)
 Requires-Dist: pysam (>=0.16.0,<0.17.0)
 Requires-Dist: tqdm (>=4.61.1,<5.0.0)
```

