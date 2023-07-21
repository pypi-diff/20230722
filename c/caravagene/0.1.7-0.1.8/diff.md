# Comparing `tmp/caravagene-0.1.7.tar.gz` & `tmp/caravagene-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caravagene-0.1.7.tar", last modified: Tue May 10 23:08:27 2022, max compression
+gzip compressed data, was "caravagene-0.1.8.tar", last modified: Fri Jul 21 23:11:55 2023, max compression
```

## Comparing `caravagene-0.1.7.tar` & `caravagene-0.1.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-10 23:08:27.245549 caravagene-0.1.7/
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2022-05-10 21:25:50.000000 caravagene-0.1.7/LICENCE.txt
--rwxrwxr-x   0 peter     (1000) peter     (1000)      124 2022-05-10 21:25:50.000000 caravagene-0.1.7/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)      897 2022-05-10 23:08:27.245549 caravagene-0.1.7/PKG-INFO
--rwxrwxr-x   0 peter     (1000) peter     (1000)     4755 2022-05-10 23:08:16.000000 caravagene-0.1.7/README.rst
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-10 23:08:27.221550 caravagene-0.1.7/caravagene/
--rwxrwxr-x   0 peter     (1000) peter     (1000)      149 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    11306 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/caravagene.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-10 23:08:27.241550 caravagene-0.1.7/caravagene/symbols/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4382 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/ATG.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     1901 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/CDS.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2118 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/DNA-binding-element.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2671 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/IRES.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2158 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/ITR.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2183 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/LTR.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)      714 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/RBS.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     1930 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/RNA-stability-sequence.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2096 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/UTR.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2269 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/backbone.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     1702 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/blank.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2277 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/etc.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     3220 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/expression-cassette.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)      692 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/five-prime-overhang.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2342 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/homology-arm.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)      751 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/insulator.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     1783 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/none.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     1880 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/origin-of-replication.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2636 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/p2A.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2726 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/part-linker.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2437 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/peptide-linker.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)      721 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/promoter.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2191 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/protein-tag.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2141 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/recombinase-recognition-sequence-directed.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2449 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/recombinase-recognition-sequence.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)      663 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/restriction-enzyme-recognition-site.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2716 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/signal-peptide.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)      692 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/terminator.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)      692 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/three-prime-overhang.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)      705 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/symbols/user-defined.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)     2033 2022-05-10 21:25:50.000000 caravagene-0.1.7/caravagene/template.html
--rwxrwxr-x   0 peter     (1000) peter     (1000)       22 2022-05-10 23:08:16.000000 caravagene-0.1.7/caravagene/version.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-10 23:08:27.225550 caravagene-0.1.7/caravagene.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)      897 2022-05-10 23:08:26.000000 caravagene-0.1.7/caravagene.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     1529 2022-05-10 23:08:27.000000 caravagene-0.1.7/caravagene.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2022-05-10 23:08:26.000000 caravagene-0.1.7/caravagene.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       30 2022-05-10 23:08:26.000000 caravagene-0.1.7/caravagene.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2022-05-10 23:08:27.000000 caravagene-0.1.7/caravagene.egg-info/top_level.txt
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-10 23:08:27.245549 caravagene-0.1.7/examples/
--rw-rw-r--   0 peter     (1000) peter     (1000)      416 2022-05-10 21:25:50.000000 caravagene-0.1.7/examples/construct_jpeg.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      256 2022-05-10 21:25:50.000000 caravagene-0.1.7/examples/from_json.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      138 2022-05-10 21:25:50.000000 caravagene-0.1.7/examples/from_spreadsheet.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1024 2022-05-10 21:25:50.000000 caravagene-0.1.7/examples/multiconstruct_pdf.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-10 23:08:27.245549 caravagene-0.1.7/scripts/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1651 2022-05-10 21:25:50.000000 caravagene-0.1.7/scripts/caravagene
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2022-05-10 23:08:27.245549 caravagene-0.1.7/setup.cfg
--rwxrwxr-x   0 peter     (1000) peter     (1000)      538 2022-05-10 21:25:50.000000 caravagene-0.1.7/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 23:11:55.381463 caravagene-0.1.8/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2022-05-10 21:25:50.000000 caravagene-0.1.8/LICENCE.txt
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      124 2022-05-10 21:25:50.000000 caravagene-0.1.8/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)      897 2023-07-21 23:11:55.381463 caravagene-0.1.8/PKG-INFO
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     4755 2022-05-10 23:08:16.000000 caravagene-0.1.8/README.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 23:11:55.325464 caravagene-0.1.8/caravagene/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      149 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11398 2023-07-21 23:11:29.000000 caravagene-0.1.8/caravagene/caravagene.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 23:11:55.381463 caravagene-0.1.8/caravagene/symbols/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4382 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/ATG.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1901 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/CDS.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2118 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/DNA-binding-element.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2671 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/IRES.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2158 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/ITR.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2183 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/LTR.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      714 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/RBS.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1930 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/RNA-stability-sequence.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2096 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/UTR.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2269 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/backbone.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1702 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/blank.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2277 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/etc.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3220 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/expression-cassette.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      692 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/five-prime-overhang.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2342 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/homology-arm.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      751 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/insulator.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1783 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/none.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1880 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/origin-of-replication.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2636 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/p2A.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2726 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/part-linker.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2437 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/peptide-linker.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      721 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/promoter.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2191 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/protein-tag.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2141 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/recombinase-recognition-sequence-directed.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2449 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/recombinase-recognition-sequence.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      663 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/restriction-enzyme-recognition-site.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2716 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/signal-peptide.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      692 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/terminator.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      692 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/three-prime-overhang.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      705 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/symbols/user-defined.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2033 2022-05-10 21:25:50.000000 caravagene-0.1.8/caravagene/template.html
+-rwxrwxr-x   0 peter     (1000) peter     (1000)       22 2023-07-21 23:11:03.000000 caravagene-0.1.8/caravagene/version.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 23:11:55.325464 caravagene-0.1.8/caravagene.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      897 2023-07-21 23:11:54.000000 caravagene-0.1.8/caravagene.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1529 2023-07-21 23:11:55.000000 caravagene-0.1.8/caravagene.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-21 23:11:54.000000 caravagene-0.1.8/caravagene.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       30 2023-07-21 23:11:55.000000 caravagene-0.1.8/caravagene.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-07-21 23:11:55.000000 caravagene-0.1.8/caravagene.egg-info/top_level.txt
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 23:11:55.381463 caravagene-0.1.8/examples/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      416 2022-05-10 21:25:50.000000 caravagene-0.1.8/examples/construct_jpeg.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      256 2022-05-10 21:25:50.000000 caravagene-0.1.8/examples/from_json.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      138 2022-05-10 21:25:50.000000 caravagene-0.1.8/examples/from_spreadsheet.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1024 2022-05-10 21:25:50.000000 caravagene-0.1.8/examples/multiconstruct_pdf.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 23:11:55.381463 caravagene-0.1.8/scripts/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1651 2022-05-10 21:25:50.000000 caravagene-0.1.8/scripts/caravagene
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-21 23:11:55.381463 caravagene-0.1.8/setup.cfg
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      538 2022-05-10 21:25:50.000000 caravagene-0.1.8/setup.py
```

### Comparing `caravagene-0.1.7/LICENCE.txt` & `caravagene-0.1.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/PKG-INFO` & `caravagene-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caravagene
-Version: 0.1.7
+Version: 0.1.8
 Summary: UNKNOWN
 Author: Zulko
 License: MIT
 Keywords: SBOL DNA assembly plot
 Platform: UNKNOWN
 License-File: LICENCE.txt
```

### Comparing `caravagene-0.1.7/README.rst` & `caravagene-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/caravagene.py` & `caravagene-0.1.8/caravagene/caravagene.py`

 * *Files 5% similar despite different names*

```diff
@@ -318,14 +318,15 @@
         data as a string.
         """
         if outfile is None:
             outfile = "-"
         process = sp.Popen(
             [
                 "wkhtmltopdf",
+                "--enable-local-file-access",
                 "--quiet",
                 "--page-size",
                 self.page_size,
                 "--orientation",
                 self.orientation,
                 "-",
                 outfile,
@@ -351,14 +352,15 @@
         if outfile is None:
             outfile = "-"
         else:
             extension = os.path.splitext(outfile)[1][1:]
         process = sp.Popen(
             [
                 "wkhtmltoimage",
+                "--enable-local-file-access",
                 "--format",
                 extension,
                 "--width",
                 "%d" % self.width,
                 "--disable-smart-width",
                 "-",
                 outfile,
```

### Comparing `caravagene-0.1.7/caravagene/symbols/ATG.svg` & `caravagene-0.1.8/caravagene/symbols/ATG.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/CDS.svg` & `caravagene-0.1.8/caravagene/symbols/CDS.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/DNA-binding-element.svg` & `caravagene-0.1.8/caravagene/symbols/DNA-binding-element.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/IRES.svg` & `caravagene-0.1.8/caravagene/symbols/IRES.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/ITR.svg` & `caravagene-0.1.8/caravagene/symbols/ITR.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/LTR.svg` & `caravagene-0.1.8/caravagene/symbols/LTR.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/RBS.svg` & `caravagene-0.1.8/caravagene/symbols/RBS.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/RNA-stability-sequence.svg` & `caravagene-0.1.8/caravagene/symbols/RNA-stability-sequence.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/UTR.svg` & `caravagene-0.1.8/caravagene/symbols/UTR.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/backbone.svg` & `caravagene-0.1.8/caravagene/symbols/backbone.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/blank.svg` & `caravagene-0.1.8/caravagene/symbols/blank.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/etc.svg` & `caravagene-0.1.8/caravagene/symbols/etc.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/expression-cassette.svg` & `caravagene-0.1.8/caravagene/symbols/expression-cassette.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/five-prime-overhang.svg` & `caravagene-0.1.8/caravagene/symbols/five-prime-overhang.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/homology-arm.svg` & `caravagene-0.1.8/caravagene/symbols/homology-arm.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/insulator.svg` & `caravagene-0.1.8/caravagene/symbols/insulator.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/none.svg` & `caravagene-0.1.8/caravagene/symbols/none.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/origin-of-replication.svg` & `caravagene-0.1.8/caravagene/symbols/origin-of-replication.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/p2A.svg` & `caravagene-0.1.8/caravagene/symbols/p2A.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/part-linker.svg` & `caravagene-0.1.8/caravagene/symbols/part-linker.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/peptide-linker.svg` & `caravagene-0.1.8/caravagene/symbols/peptide-linker.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/promoter.svg` & `caravagene-0.1.8/caravagene/symbols/promoter.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/protein-tag.svg` & `caravagene-0.1.8/caravagene/symbols/protein-tag.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/recombinase-recognition-sequence-directed.svg` & `caravagene-0.1.8/caravagene/symbols/recombinase-recognition-sequence-directed.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/recombinase-recognition-sequence.svg` & `caravagene-0.1.8/caravagene/symbols/recombinase-recognition-sequence.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/restriction-enzyme-recognition-site.svg` & `caravagene-0.1.8/caravagene/symbols/restriction-enzyme-recognition-site.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/signal-peptide.svg` & `caravagene-0.1.8/caravagene/symbols/signal-peptide.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/terminator.svg` & `caravagene-0.1.8/caravagene/symbols/terminator.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/three-prime-overhang.svg` & `caravagene-0.1.8/caravagene/symbols/three-prime-overhang.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/symbols/user-defined.svg` & `caravagene-0.1.8/caravagene/symbols/user-defined.svg`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene/template.html` & `caravagene-0.1.8/caravagene/template.html`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/caravagene.egg-info/PKG-INFO` & `caravagene-0.1.8/caravagene.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caravagene
-Version: 0.1.7
+Version: 0.1.8
 Summary: UNKNOWN
 Author: Zulko
 License: MIT
 Keywords: SBOL DNA assembly plot
 Platform: UNKNOWN
 License-File: LICENCE.txt
```

### Comparing `caravagene-0.1.7/caravagene.egg-info/SOURCES.txt` & `caravagene-0.1.8/caravagene.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/examples/multiconstruct_pdf.py` & `caravagene-0.1.8/examples/multiconstruct_pdf.py`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/scripts/caravagene` & `caravagene-0.1.8/scripts/caravagene`

 * *Files identical despite different names*

### Comparing `caravagene-0.1.7/setup.py` & `caravagene-0.1.8/setup.py`

 * *Files identical despite different names*

