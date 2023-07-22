# Comparing `tmp/snpio-1.0.1.1.tar.gz` & `tmp/snpio-1.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snpio-1.0.1.1.tar", last modified: Sat Jul 22 18:41:19 2023, max compression
+gzip compressed data, was "snpio-1.0.1.2.tar", last modified: Sat Jul 22 18:42:46 2023, max compression
```

## Comparing `snpio-1.0.1.1.tar` & `snpio-1.0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:41:18.544128 snpio-1.0.1.1/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35149 2023-04-12 14:52:30.000000 snpio-1.0.1.1/LICENSE
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16152 2023-07-22 18:41:18.537128 snpio-1.0.1.1/PKG-INFO
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13083 2023-07-22 17:50:20.000000 snpio-1.0.1.1/README.md
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1709 2023-07-22 18:40:59.000000 snpio-1.0.1.1/pyproject.toml
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)       38 2023-07-22 18:41:18.545128 snpio-1.0.1.1/setup.cfg
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2075 2023-07-22 18:41:05.000000 snpio-1.0.1.1/setup.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:41:17.529148 snpio-1.0.1.1/snpio/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      152 2023-07-21 17:59:43.000000 snpio-1.0.1.1/snpio/__init__.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:41:17.769140 snpio-1.0.1.1/snpio/filtering/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-21 17:58:22.000000 snpio-1.0.1.1/snpio/filtering/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    55612 2023-07-22 16:45:38.000000 snpio-1.0.1.1/snpio/filtering/nremover2.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:41:17.866139 snpio-1.0.1.1/snpio/plotting/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-21 17:58:27.000000 snpio-1.0.1.1/snpio/plotting/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    76795 2023-07-22 16:46:45.000000 snpio-1.0.1.1/snpio/plotting/plotting.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:41:18.023137 snpio-1.0.1.1/snpio/popgenstats/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-06-02 16:36:49.000000 snpio-1.0.1.1/snpio/popgenstats/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    26425 2023-07-22 16:45:52.000000 snpio-1.0.1.1/snpio/popgenstats/pop_gen_statistics.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:41:18.235134 snpio-1.0.1.1/snpio/read_input/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-21 17:57:45.000000 snpio-1.0.1.1/snpio/read_input/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)   122873 2023-07-22 16:46:35.000000 snpio-1.0.1.1/snpio/read_input/genotype_data.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11793 2023-07-22 16:46:41.000000 snpio-1.0.1.1/snpio/read_input/popmap_file.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:41:18.380130 snpio-1.0.1.1/snpio/utils/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2022-06-18 03:33:16.000000 snpio-1.0.1.1/snpio/utils/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    23949 2023-06-26 19:20:02.000000 snpio-1.0.1.1/snpio/utils/misc.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    22414 2023-07-08 04:15:25.000000 snpio-1.0.1.1/snpio/utils/sequence_tools.py
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:41:17.722142 snpio-1.0.1.1/snpio.egg-info/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16152 2023-07-22 18:41:16.000000 snpio-1.0.1.1/snpio.egg-info/PKG-INFO
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      723 2023-07-22 18:41:16.000000 snpio-1.0.1.1/snpio.egg-info/SOURCES.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        1 2023-07-22 18:41:16.000000 snpio-1.0.1.1/snpio.egg-info/dependency_links.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)       45 2023-07-22 18:41:16.000000 snpio-1.0.1.1/snpio.egg-info/entry_points.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      222 2023-07-22 18:41:16.000000 snpio-1.0.1.1/snpio.egg-info/requires.txt
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)       12 2023-07-22 18:41:16.000000 snpio-1.0.1.1/snpio.egg-info/top_level.txt
-drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:41:18.510128 snpio-1.0.1.1/tests/
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-06-21 16:48:56.000000 snpio-1.0.1.1/tests/__init__.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1389 2023-06-23 03:09:10.000000 snpio-1.0.1.1/tests/benchmarking.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      498 2023-06-23 04:46:01.000000 snpio-1.0.1.1/tests/filter_packages.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      538 2023-06-23 03:21:16.000000 snpio-1.0.1.1/tests/get_docstrings.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      462 2023-06-23 04:39:50.000000 snpio-1.0.1.1/tests/get_pkg_resources.py
--rwxrwxrwx   0 btm002    (1000) btm002    (1000)      883 2023-06-23 04:34:30.000000 snpio-1.0.1.1/tests/modulefinder.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:42:45.767860 snpio-1.0.1.2/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    35149 2023-04-12 14:52:30.000000 snpio-1.0.1.2/LICENSE
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16152 2023-07-22 18:42:45.764859 snpio-1.0.1.2/PKG-INFO
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    13083 2023-07-22 17:50:20.000000 snpio-1.0.1.2/README.md
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1709 2023-07-22 18:42:37.000000 snpio-1.0.1.2/pyproject.toml
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)       38 2023-07-22 18:42:45.769859 snpio-1.0.1.2/setup.cfg
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     2073 2023-07-22 18:42:23.000000 snpio-1.0.1.2/setup.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:42:45.073870 snpio-1.0.1.2/snpio/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      152 2023-07-21 17:59:43.000000 snpio-1.0.1.2/snpio/__init__.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:42:45.298868 snpio-1.0.1.2/snpio/filtering/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-21 17:58:22.000000 snpio-1.0.1.2/snpio/filtering/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    55612 2023-07-22 16:45:38.000000 snpio-1.0.1.2/snpio/filtering/nremover2.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:42:45.357868 snpio-1.0.1.2/snpio/plotting/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-21 17:58:27.000000 snpio-1.0.1.2/snpio/plotting/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    76795 2023-07-22 16:46:45.000000 snpio-1.0.1.2/snpio/plotting/plotting.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:42:45.411864 snpio-1.0.1.2/snpio/popgenstats/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-06-02 16:36:49.000000 snpio-1.0.1.2/snpio/popgenstats/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    26425 2023-07-22 16:45:52.000000 snpio-1.0.1.2/snpio/popgenstats/pop_gen_statistics.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:42:45.482864 snpio-1.0.1.2/snpio/read_input/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-21 17:57:45.000000 snpio-1.0.1.2/snpio/read_input/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)   122873 2023-07-22 16:46:35.000000 snpio-1.0.1.2/snpio/read_input/genotype_data.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    11793 2023-07-22 16:46:41.000000 snpio-1.0.1.2/snpio/read_input/popmap_file.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:42:45.559862 snpio-1.0.1.2/snpio/utils/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2022-06-18 03:33:16.000000 snpio-1.0.1.2/snpio/utils/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    23949 2023-06-26 19:20:02.000000 snpio-1.0.1.2/snpio/utils/misc.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    22414 2023-07-08 04:15:25.000000 snpio-1.0.1.2/snpio/utils/sequence_tools.py
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:42:45.245868 snpio-1.0.1.2/snpio.egg-info/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)    16152 2023-07-22 18:42:43.000000 snpio-1.0.1.2/snpio.egg-info/PKG-INFO
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      723 2023-07-22 18:42:44.000000 snpio-1.0.1.2/snpio.egg-info/SOURCES.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        1 2023-07-22 18:42:43.000000 snpio-1.0.1.2/snpio.egg-info/dependency_links.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)       45 2023-07-22 18:42:43.000000 snpio-1.0.1.2/snpio.egg-info/entry_points.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      229 2023-07-22 18:42:43.000000 snpio-1.0.1.2/snpio.egg-info/requires.txt
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)       12 2023-07-22 18:42:43.000000 snpio-1.0.1.2/snpio.egg-info/top_level.txt
+drwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-07-22 18:42:45.735862 snpio-1.0.1.2/tests/
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)        0 2023-06-21 16:48:56.000000 snpio-1.0.1.2/tests/__init__.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)     1389 2023-06-23 03:09:10.000000 snpio-1.0.1.2/tests/benchmarking.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      498 2023-06-23 04:46:01.000000 snpio-1.0.1.2/tests/filter_packages.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      538 2023-06-23 03:21:16.000000 snpio-1.0.1.2/tests/get_docstrings.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      462 2023-06-23 04:39:50.000000 snpio-1.0.1.2/tests/get_pkg_resources.py
+-rwxrwxrwx   0 btm002    (1000) btm002    (1000)      883 2023-06-23 04:34:30.000000 snpio-1.0.1.2/tests/modulefinder.py
```

### Comparing `snpio-1.0.1.1/LICENSE` & `snpio-1.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/PKG-INFO` & `snpio-1.0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snpio
-Version: 1.0.1.1
+Version: 1.0.1.2
 Summary: Reads and writes VCF, PHYLIP, and STRUCTURE files and performs data filtering on the alignment.
 Home-page: https://github.com/btmartin721/SNPio
 Author: Bradley T. Martin and Tyler K. Chafin
 Author-email: evobio721@gmail.com
 License: GPL3
 Project-URL: Source Code, https://github.com/btmartin721/SNPio
 Project-URL: Bug Tracker, https://github.com/btmartin721/SNPio/issues
```

### Comparing `snpio-1.0.1.1/README.md` & `snpio-1.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/pyproject.toml` & `snpio-1.0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SNPio"
-version = "1.0.1.1"
+version = "1.0.1.2"
 authors = [
     { name="Bradley T. Martin", email="evobio721@gmail.com" }, 
     { name="Tyler K. Chafin", email="tylerkchafin@gmail.com" } 
 ]
 description = "Reads and writes VCF, PHYLIP, and STRUCTURE files and performs data filtering on the alignment."
 keywords=[
         "genomics",
```

### Comparing `snpio-1.0.1.1/setup.py` & `snpio-1.0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="snpio",
-    version="1.0.1.1",
+    version="1.0.1.2",
     url="https://github.com/btmartin721/SNPio",
     author="Bradley T. Martin and Tyler K. Chafin",
     author_email="evobio721@gmail.com",
     description="Reads and writes VCF, PHYLIP, and STRUCTURE files and performs data filtering on the alignment.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="GPL3",
@@ -35,15 +35,15 @@
         "kneed",
         "matplotlib",
         "numpy",
         "pandas",
         "panel",
         "plotly",
         "requests",
-        # "cyvcf2",
+        "cyvcf2",
         "scikit-learn",
         "scipy",
         "seaborn",
         "toytree",
         "kaleido",
         "psutil",
     ],
```

### Comparing `snpio-1.0.1.1/snpio/filtering/nremover2.py` & `snpio-1.0.1.2/snpio/filtering/nremover2.py`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/snpio/plotting/plotting.py` & `snpio-1.0.1.2/snpio/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/snpio/popgenstats/pop_gen_statistics.py` & `snpio-1.0.1.2/snpio/popgenstats/pop_gen_statistics.py`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/snpio/read_input/genotype_data.py` & `snpio-1.0.1.2/snpio/read_input/genotype_data.py`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/snpio/read_input/popmap_file.py` & `snpio-1.0.1.2/snpio/read_input/popmap_file.py`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/snpio/utils/misc.py` & `snpio-1.0.1.2/snpio/utils/misc.py`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/snpio/utils/sequence_tools.py` & `snpio-1.0.1.2/snpio/utils/sequence_tools.py`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/snpio.egg-info/PKG-INFO` & `snpio-1.0.1.2/snpio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snpio
-Version: 1.0.1.1
+Version: 1.0.1.2
 Summary: Reads and writes VCF, PHYLIP, and STRUCTURE files and performs data filtering on the alignment.
 Home-page: https://github.com/btmartin721/SNPio
 Author: Bradley T. Martin and Tyler K. Chafin
 Author-email: evobio721@gmail.com
 License: GPL3
 Project-URL: Source Code, https://github.com/btmartin721/SNPio
 Project-URL: Bug Tracker, https://github.com/btmartin721/SNPio/issues
```

### Comparing `snpio-1.0.1.1/snpio.egg-info/SOURCES.txt` & `snpio-1.0.1.2/snpio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/tests/benchmarking.py` & `snpio-1.0.1.2/tests/benchmarking.py`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/tests/get_docstrings.py` & `snpio-1.0.1.2/tests/get_docstrings.py`

 * *Files identical despite different names*

### Comparing `snpio-1.0.1.1/tests/modulefinder.py` & `snpio-1.0.1.2/tests/modulefinder.py`

 * *Files identical despite different names*

