# Comparing `tmp/pygleif-4.0.6.tar.gz` & `tmp/pygleif-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygleif-4.0.6.tar", last modified: Wed Jun 29 12:10:04 2022, max compression
+gzip compressed data, was "pygleif-5.0.0.tar", last modified: Sat Jul 22 20:20:00 2023, max compression
```

## Comparing `pygleif-4.0.6.tar` & `pygleif-5.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 12:10:04.343218 pygleif-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-06-29 12:09:55.000000 pygleif-4.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-06-29 12:10:04.343218 pygleif-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-06-29 12:09:55.000000 pygleif-4.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 12:10:04.339218 pygleif-4.0.6/pygleif/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-29 12:09:55.000000 pygleif-4.0.6/pygleif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 12:10:04.343218 pygleif-4.0.6/pygleif/api/
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-06-29 12:09:55.000000 pygleif-4.0.6/pygleif/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2022-06-29 12:09:55.000000 pygleif-4.0.6/pygleif/api/data.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-06-29 12:09:55.000000 pygleif-4.0.6/pygleif/api/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-06-29 12:09:55.000000 pygleif-4.0.6/pygleif/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-06-29 12:09:55.000000 pygleif-4.0.6/pygleif/error.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-06-29 12:09:55.000000 pygleif-4.0.6/pygleif/gleif.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-06-29 12:09:55.000000 pygleif-4.0.6/pygleif/search.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-06-29 12:09:55.000000 pygleif-4.0.6/pygleif/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 12:10:04.339218 pygleif-4.0.6/pygleif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-06-29 12:10:04.000000 pygleif-4.0.6/pygleif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-06-29 12:10:04.000000 pygleif-4.0.6/pygleif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 12:10:04.000000 pygleif-4.0.6/pygleif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-29 12:10:04.000000 pygleif-4.0.6/pygleif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-06-29 12:09:55.000000 pygleif-4.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-06-29 12:10:04.343218 pygleif-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-06-29 12:09:55.000000 pygleif-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:20:00.936710 pygleif-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-22 20:19:45.000000 pygleif-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-22 20:20:00.936710 pygleif-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-22 20:19:45.000000 pygleif-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:20:00.936710 pygleif-5.0.0/pygleif/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-22 20:19:45.000000 pygleif-5.0.0/pygleif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:20:00.936710 pygleif-5.0.0/pygleif/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-22 20:19:45.000000 pygleif-5.0.0/pygleif/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-22 20:19:45.000000 pygleif-5.0.0/pygleif/api/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-22 20:19:45.000000 pygleif-5.0.0/pygleif/api/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-22 20:19:45.000000 pygleif-5.0.0/pygleif/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-22 20:19:45.000000 pygleif-5.0.0/pygleif/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-22 20:19:45.000000 pygleif-5.0.0/pygleif/gleif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-22 20:19:45.000000 pygleif-5.0.0/pygleif/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-22 20:19:45.000000 pygleif-5.0.0/pygleif/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:20:00.936710 pygleif-5.0.0/pygleif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-22 20:20:00.000000 pygleif-5.0.0/pygleif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-22 20:20:00.000000 pygleif-5.0.0/pygleif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:20:00.000000 pygleif-5.0.0/pygleif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-22 20:20:00.000000 pygleif-5.0.0/pygleif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-22 20:19:45.000000 pygleif-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-22 20:20:00.936710 pygleif-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-22 20:19:45.000000 pygleif-5.0.0/setup.py
```

### Comparing `pygleif-4.0.6/LICENSE` & `pygleif-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygleif-4.0.6/PKG-INFO` & `pygleif-5.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 Metadata-Version: 2.1
 Name: pygleif
-Version: 4.0.6
-Summary: UNKNOWN
+Version: 5.0.0
 Home-page: https://github.com/ggravlingen/pygleif
+Download-URL: https://github.com/ggravlingen/pygleif/archive/5.0.0.zip
 Author: ggravlingen
 Author-email: no@email.com
 License: MIT
-Download-URL: https://github.com/ggravlingen/pygleif/archive/4.0.6.zip
 Keywords: lei-code lei api gleif leicode
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Financial and Insurance Industry
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/pygleif.svg)](https://badge.fury.io/py/pygleif)
 
 This library queries the API of GLEIF.org to return data about a specific entity company. The result is typed using `Pydantic` It is also possible to search for organisation id to find LEI codes and also to get child notes for a specific LEI code.
-
-
```

### Comparing `pygleif-4.0.6/pygleif/api/data.py` & `pygleif-5.0.0/pygleif/api/data.py`

 * *Files identical despite different names*

### Comparing `pygleif-4.0.6/pygleif/api/meta.py` & `pygleif-5.0.0/pygleif/api/meta.py`

 * *Files identical despite different names*

### Comparing `pygleif-4.0.6/pygleif/const.py` & `pygleif-5.0.0/pygleif/const.py`

 * *Files identical despite different names*

### Comparing `pygleif-4.0.6/pygleif/search.py` & `pygleif-5.0.0/pygleif/search.py`

 * *Files identical despite different names*

### Comparing `pygleif-4.0.6/pygleif.egg-info/PKG-INFO` & `pygleif-5.0.0/pygleif.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 Metadata-Version: 2.1
 Name: pygleif
-Version: 4.0.6
-Summary: UNKNOWN
+Version: 5.0.0
 Home-page: https://github.com/ggravlingen/pygleif
+Download-URL: https://github.com/ggravlingen/pygleif/archive/5.0.0.zip
 Author: ggravlingen
 Author-email: no@email.com
 License: MIT
-Download-URL: https://github.com/ggravlingen/pygleif/archive/4.0.6.zip
 Keywords: lei-code lei api gleif leicode
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Financial and Insurance Industry
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/pygleif.svg)](https://badge.fury.io/py/pygleif)
 
 This library queries the API of GLEIF.org to return data about a specific entity company. The result is typed using `Pydantic` It is also possible to search for organisation id to find LEI codes and also to get child notes for a specific LEI code.
-
-
```

### Comparing `pygleif-4.0.6/pyproject.toml` & `pygleif-5.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.black]
-target-version = ["py38", "py39", "py310"]
+target-version = ["py310"]
 
 [tool.isort]
 # https://github.com/PyCQA/isort/wiki/isort-Settings
 profile = "black"
 # will group `import x` and `from x import` of the same module.
 force_sort_within_sections = true
 known_first_party = [
@@ -12,16 +12,15 @@
 ]
 forced_separate = [
     "tests",
 ]
 combine_as_imports = true
 
 [tool.pylint.MASTER]
-py-version = "3.8"
-
+py-version = "3.10"
 
 [tool.pylint.BASIC]
 class-const-naming-style = "any"
 
 [tool.pylint."MESSAGES CONTROL"]
```

### Comparing `pygleif-4.0.6/setup.py` & `pygleif-5.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 DOWNLOAD_URL = f"{GITHUB_URL}/archive/{VERSION}.zip"
 
 PACKAGES = find_packages(exclude=["tests", "tests.*"])
 
 setup(
     name="pygleif",
     packages=PACKAGES,
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     version=VERSION,
     long_description=LONG_DESCRIPTION,
     author='ggravlingen',
     author_email="no@email.com",
     long_description_content_type="text/markdown",
     url=GITHUB_URL,
     include_package_data=True,
     license="MIT",
     keywords='lei-code lei api gleif leicode',
     download_url=DOWNLOAD_URL,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Intended Audience :: Financial and Insurance Industry",
     ],
 )
```

