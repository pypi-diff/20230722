# Comparing `tmp/interpres-0.3.3b1.tar.gz` & `tmp/interpres-0.3.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpres-0.3.3b1.tar", last modified: Sat Jul 22 00:35:05 2023, max compression
+gzip compressed data, was "interpres-0.3.3b2.tar", last modified: Sat Jul 22 00:41:46 2023, max compression
```

## Comparing `interpres-0.3.3b1.tar` & `interpres-0.3.3b2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 00:35:05.792326 interpres-0.3.3b1/
--rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.3b1/LICENSE
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 00:35:05.792326 interpres-0.3.3b1/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.3b1/README.md
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 00:35:05.792326 interpres-0.3.3b1/interpres.egg-info/
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 00:35:05.000000 interpres-0.3.3b1/interpres.egg-info/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 00:35:05.000000 interpres-0.3.3b1/interpres.egg-info/SOURCES.txt
--rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 00:35:05.000000 interpres-0.3.3b1/interpres.egg-info/dependency_links.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 00:35:05.000000 interpres-0.3.3b1/interpres.egg-info/entry_points.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 00:35:05.000000 interpres-0.3.3b1/interpres.egg-info/requires.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 00:35:05.000000 interpres-0.3.3b1/interpres.egg-info/top_level.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.3b1/pyproject.toml
--rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 00:35:05.792326 interpres-0.3.3b1/setup.cfg
--rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:32:10.000000 interpres-0.3.3b1/setup.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 00:35:05.792326 interpres-0.3.3b1/translator/
--rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 00:32:10.000000 interpres-0.3.3b1/translator/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.3b1/translator/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.3b1/translator/language.py
--rw-r--r--   0 waser     (1000) waser     (1000)    29033 2023-03-14 11:40:43.000000 interpres-0.3.3b1/translator/main.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1950 2023-03-13 15:42:00.000000 interpres-0.3.3b1/translator/translate.py
--rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.3b1/translator/utils.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 00:41:46.374499 interpres-0.3.3b2/
+-rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.3b2/LICENSE
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 00:41:46.374499 interpres-0.3.3b2/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.3b2/README.md
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 00:41:46.371165 interpres-0.3.3b2/interpres.egg-info/
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 00:41:46.000000 interpres-0.3.3b2/interpres.egg-info/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 00:41:46.000000 interpres-0.3.3b2/interpres.egg-info/SOURCES.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 00:41:46.000000 interpres-0.3.3b2/interpres.egg-info/dependency_links.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 00:41:46.000000 interpres-0.3.3b2/interpres.egg-info/entry_points.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 00:41:46.000000 interpres-0.3.3b2/interpres.egg-info/requires.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 00:41:46.000000 interpres-0.3.3b2/interpres.egg-info/top_level.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.3b2/pyproject.toml
+-rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 00:41:46.374499 interpres-0.3.3b2/setup.cfg
+-rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:39:23.000000 interpres-0.3.3b2/setup.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 00:41:46.374499 interpres-0.3.3b2/translator/
+-rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 00:39:36.000000 interpres-0.3.3b2/translator/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.3b2/translator/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.3b2/translator/language.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    29033 2023-03-14 11:40:43.000000 interpres-0.3.3b2/translator/main.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1950 2023-03-13 15:42:00.000000 interpres-0.3.3b2/translator/translate.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.3b2/translator/utils.py
```

### Comparing `interpres-0.3.3b1/LICENSE` & `interpres-0.3.3b2/LICENSE`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b1/PKG-INFO` & `interpres-0.3.3b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.3b1
+Version: 0.3.3b2
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.3b1/README.md` & `interpres-0.3.3b2/README.md`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b1/interpres.egg-info/PKG-INFO` & `interpres-0.3.3b2/interpres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.3b1
+Version: 0.3.3b2
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.3b1/pyproject.toml` & `interpres-0.3.3b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b1/setup.py` & `interpres-0.3.3b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     url='https://github.com/wasertech/Translator',
     description='Translate from one language to another.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages('.'),
     python_requires='>=3.8,<3.12',
     install_requires = [
-        'transformers~=4.25.1',
+        'transformers~=4.31.0',
         'langcodes~=3.3.0',
-        'datasets~=2.10.1',
+        'datasets~=2.13.1',
         'halo~=0.0.31',
         'psutil~=5.9.4',
         'shutils~=0.1.0',
         'accelerate~=0.17.0',
         'questionary~=1.10.0',
     ],
     entry_points={
```

### Comparing `interpres-0.3.3b1/translator/language.py` & `interpres-0.3.3b2/translator/language.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b1/translator/main.py` & `interpres-0.3.3b2/translator/main.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b1/translator/translate.py` & `interpres-0.3.3b2/translator/translate.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b1/translator/utils.py` & `interpres-0.3.3b2/translator/utils.py`

 * *Files identical despite different names*

