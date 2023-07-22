# Comparing `tmp/hchacha-1.0.4.tar.gz` & `tmp/hchacha-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hchacha-1.0.4.tar", max compression
+gzip compressed data, was "hchacha-1.0.5.tar", max compression
```

## Comparing `hchacha-1.0.4.tar` & `hchacha-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-02-09 14:04:58.020837 hchacha-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0     3398 2023-07-22 17:27:45.975379 hchacha-1.0.4/README.md
--rw-r--r--   0        0        0      900 2023-07-22 17:31:20.737379 hchacha-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       47 2023-02-06 02:52:38.085523 hchacha-1.0.4/src/hchacha/__init__.py
--rw-r--r--   0        0        0     1321 2023-07-22 17:24:41.717959 hchacha-1.0.4/src/hchacha/data/GRCh37.tsv.gz
--rw-r--r--   0        0        0    11620 2023-07-22 17:24:44.853835 hchacha-1.0.4/src/hchacha/data/GRCh38.tsv.gz
--rwxr-xr-x   0        0        0     7342 2023-07-22 17:30:11.461788 hchacha-1.0.4/src/hchacha/hchacha.py
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 hchacha-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-02-09 14:04:58.020837 hchacha-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     3398 2023-07-22 17:27:45.975379 hchacha-1.0.5/README.md
+-rw-r--r--   0        0        0      900 2023-07-22 18:35:20.842171 hchacha-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-02-06 02:52:38.085523 hchacha-1.0.5/src/hchacha/__init__.py
+-rw-r--r--   0        0        0     1899 2023-07-22 18:31:43.646212 hchacha-1.0.5/src/hchacha/data/GRCh37.tsv.gz
+-rw-r--r--   0        0        0    13611 2023-07-22 18:31:46.602558 hchacha-1.0.5/src/hchacha/data/GRCh38.tsv.gz
+-rwxr-xr-x   0        0        0     7342 2023-07-22 17:30:11.461788 hchacha-1.0.5/src/hchacha/hchacha.py
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 hchacha-1.0.5/PKG-INFO
```

### Comparing `hchacha-1.0.4/LICENSE.txt` & `hchacha-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hchacha-1.0.4/README.md` & `hchacha-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hchacha-1.0.4/pyproject.toml` & `hchacha-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hchacha"
-version = "1.0.4"
+version = "1.0.5"
 description = "Human CHromosome Accession CHAnge - Convert between different human chromosome naming systems (of the same assembly/version)"
 authors = ["Bradford Powell <bpow@drpowell.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://bitbucket.org/bpow/hchacha"
 homepage = "https://bitbucket.org/bpow/hchacha"
 keywords = [ "genetics", "bam", "sam", "vcf", "variants", "bed", "fasta", "genome", "exome"]
```

### Comparing `hchacha-1.0.4/src/hchacha/hchacha.py` & `hchacha-1.0.5/src/hchacha/hchacha.py`

 * *Files identical despite different names*

### Comparing `hchacha-1.0.4/PKG-INFO` & `hchacha-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hchacha
-Version: 1.0.4
+Version: 1.0.5
 Summary: Human CHromosome Accession CHAnge - Convert between different human chromosome naming systems (of the same assembly/version)
 Home-page: https://bitbucket.org/bpow/hchacha
 License: MIT
 Keywords: genetics,bam,sam,vcf,variants,bed,fasta,genome,exome
 Author: Bradford Powell
 Author-email: bpow@drpowell.org
 Requires-Python: >=3.7,<4.0
```

