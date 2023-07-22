# Comparing `tmp/proces-0.1.4.tar.gz` & `tmp/proces-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proces-0.1.4.tar", last modified: Thu Mar 16 14:43:06 2023, max compression
+gzip compressed data, was "proces-0.1.5.tar", last modified: Sat Jul 22 11:27:27 2023, max compression
```

## Comparing `proces-0.1.4.tar` & `proces-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 ailln      (501) staff       (20)        0 2023-03-16 14:43:06.522066 proces-0.1.4/
--rw-r--r--   0 ailln      (501) staff       (20)     1062 2021-11-03 17:50:35.000000 proces-0.1.4/LICENSE
--rw-r--r--   0 ailln      (501) staff       (20)      150 2023-03-16 14:33:19.000000 proces-0.1.4/MANIFEST.in
--rw-r--r--   0 ailln      (501) staff       (20)     2929 2023-03-16 14:43:06.521941 proces-0.1.4/PKG-INFO
--rw-r--r--   0 ailln      (501) staff       (20)     2355 2023-03-16 14:41:23.000000 proces-0.1.4/README.md
-drwxr-xr-x   0 ailln      (501) staff       (20)        0 2023-03-16 14:43:06.521169 proces-0.1.4/proces/
--rw-r--r--   0 ailln      (501) staff       (20)      674 2023-03-16 02:38:38.000000 proces-0.1.4/proces/__init__.py
--rw-r--r--   0 ailln      (501) staff       (20)    57579 2022-11-02 17:47:52.000000 proces-0.1.4/proces/conf.py
--rw-r--r--   0 ailln      (501) staff       (20)     3417 2023-03-16 02:15:35.000000 proces-0.1.4/proces/preprocess.py
--rw-r--r--   0 ailln      (501) staff       (20)     4762 2023-03-16 02:36:28.000000 proces-0.1.4/proces/preprocess_test.py
-drwxr-xr-x   0 ailln      (501) staff       (20)        0 2023-03-16 14:43:06.521768 proces-0.1.4/proces.egg-info/
--rw-r--r--   0 ailln      (501) staff       (20)     2929 2023-03-16 14:43:06.000000 proces-0.1.4/proces.egg-info/PKG-INFO
--rw-r--r--   0 ailln      (501) staff       (20)      264 2023-03-16 14:43:06.000000 proces-0.1.4/proces.egg-info/SOURCES.txt
--rw-r--r--   0 ailln      (501) staff       (20)        1 2023-03-16 14:43:06.000000 proces-0.1.4/proces.egg-info/dependency_links.txt
--rw-r--r--   0 ailln      (501) staff       (20)        7 2023-03-16 14:43:06.000000 proces-0.1.4/proces.egg-info/top_level.txt
--rw-r--r--   0 ailln      (501) staff       (20)        1 2021-11-03 17:53:28.000000 proces-0.1.4/proces.egg-info/zip-safe
--rw-r--r--   0 ailln      (501) staff       (20)       38 2023-03-16 14:43:06.522122 proces-0.1.4/setup.cfg
--rw-r--r--   0 ailln      (501) staff       (20)     1638 2023-03-16 14:34:45.000000 proces-0.1.4/setup.py
+drwxr-xr-x   0 ailln      (501) staff       (20)        0 2023-07-22 11:27:27.274837 proces-0.1.5/
+-rw-r--r--   0 ailln      (501) staff       (20)     1062 2021-11-03 17:50:35.000000 proces-0.1.5/LICENSE
+-rw-r--r--   0 ailln      (501) staff       (20)      150 2023-03-16 14:33:19.000000 proces-0.1.5/MANIFEST.in
+-rw-r--r--   0 ailln      (501) staff       (20)     2979 2023-07-22 11:27:27.274595 proces-0.1.5/PKG-INFO
+-rw-r--r--   0 ailln      (501) staff       (20)     2355 2023-03-16 14:41:23.000000 proces-0.1.5/README.md
+drwxr-xr-x   0 ailln      (501) staff       (20)        0 2023-07-22 11:27:27.273335 proces-0.1.5/proces/
+-rw-r--r--   0 ailln      (501) staff       (20)      777 2023-07-14 08:54:37.000000 proces-0.1.5/proces/__init__.py
+-rw-r--r--   0 ailln      (501) staff       (20)    57579 2022-11-02 17:47:52.000000 proces-0.1.5/proces/conf.py
+drwxr-xr-x   0 ailln      (501) staff       (20)        0 2023-07-22 11:27:27.274040 proces-0.1.5/proces/data/
+-rw-r--r--   0 ailln      (501) staff       (20)     7083 2023-07-14 09:46:28.000000 proces-0.1.5/proces/data/province_city.yaml
+-rw-r--r--   0 ailln      (501) staff       (20)      619 2023-07-22 11:17:43.000000 proces-0.1.5/proces/masking.py
+-rw-r--r--   0 ailln      (501) staff       (20)     3156 2023-07-22 11:24:05.000000 proces-0.1.5/proces/masking_test.py
+-rw-r--r--   0 ailln      (501) staff       (20)     3416 2023-07-22 11:01:31.000000 proces-0.1.5/proces/preprocess.py
+-rw-r--r--   0 ailln      (501) staff       (20)     4762 2023-03-16 02:36:28.000000 proces-0.1.5/proces/preprocess_test.py
+drwxr-xr-x   0 ailln      (501) staff       (20)        0 2023-07-22 11:27:27.274390 proces-0.1.5/proces/util/
+-rw-r--r--   0 ailln      (501) staff       (20)        0 2023-07-22 11:05:48.000000 proces-0.1.5/proces/util/__init__.py
+-rw-r--r--   0 ailln      (501) staff       (20)      352 2023-07-18 01:38:11.000000 proces-0.1.5/proces/util/conf.py
+-rw-r--r--   0 ailln      (501) staff       (20)     2723 2023-07-22 11:23:02.000000 proces-0.1.5/proces/util/data.py
+drwxr-xr-x   0 ailln      (501) staff       (20)        0 2023-07-22 11:27:27.273927 proces-0.1.5/proces.egg-info/
+-rw-r--r--   0 ailln      (501) staff       (20)     2979 2023-07-22 11:27:27.000000 proces-0.1.5/proces.egg-info/PKG-INFO
+-rw-r--r--   0 ailln      (501) staff       (20)      400 2023-07-22 11:27:27.000000 proces-0.1.5/proces.egg-info/SOURCES.txt
+-rw-r--r--   0 ailln      (501) staff       (20)        1 2023-07-22 11:27:27.000000 proces-0.1.5/proces.egg-info/dependency_links.txt
+-rw-r--r--   0 ailln      (501) staff       (20)       26 2023-07-22 11:27:27.000000 proces-0.1.5/proces.egg-info/top_level.txt
+-rw-r--r--   0 ailln      (501) staff       (20)        1 2021-11-03 17:53:28.000000 proces-0.1.5/proces.egg-info/zip-safe
+-rw-r--r--   0 ailln      (501) staff       (20)       38 2023-07-22 11:27:27.274885 proces-0.1.5/setup.cfg
+-rw-r--r--   0 ailln      (501) staff       (20)     1718 2023-07-22 11:04:21.000000 proces-0.1.5/setup.py
```

### Comparing `proces-0.1.4/LICENSE` & `proces-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proces-0.1.4/PKG-INFO` & `proces-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: proces
-Version: 0.1.4
+Version: 0.1.5
 Summary: text preprocess.
 Home-page: https://github.com/Ailln/proces
 Author: Ailln
 Author-email: kinggreenhall@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Proces
```

### Comparing `proces-0.1.4/README.md` & `proces-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `proces-0.1.4/proces/__init__.py` & `proces-0.1.5/proces/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 from .preprocess import filter_unusual_characters
 from .preprocess import handle_blank_character
 from .preprocess import uppercase_to_lowercase
 from .preprocess import traditional_to_simplified
 from .preprocess import full_angle_to_half_angle
 from .preprocess import handle_substitute
 from .preprocess import preprocess
-
-__version__ = "0.1.4"
+from .masking import mask_phone
+from .masking import mask_address
 
 filter_ = filter_unusual_characters
 
+__version__ = "0.1.5"
+
 __all__ = [
     "get_all_pipelines",
     "filter_unusual_characters", "filter_",
     "handle_blank_character",
     "uppercase_to_lowercase",
     "traditional_to_simplified",
     "full_angle_to_half_angle",
     "handle_substitute",
     "preprocess",
+    "mask_phone",
+    "mask_address"
 ]
```

### Comparing `proces-0.1.4/proces/conf.py` & `proces-0.1.5/proces/conf.py`

 * *Files identical despite different names*

### Comparing `proces-0.1.4/proces/preprocess.py` & `proces-0.1.5/proces/preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import re
+from re import sub
 from typing import Union, Optional
 
 from .conf import T2S_DICT
 
 ALL_PIPELINES = [
     "filter_unusual_characters",
     "handle_blank_character",
@@ -23,25 +23,25 @@
 
     Attributes:
         text: input text
     """
     chinese = r"\u4E00-\u9FA5"
     punctuation = r"!\"#$%&\'()*+,\-./:;<=>?@\\\[\]^_`{|}~¥·—‘’“”…、。〈〉《》「」『』【】！（），：；？｜～"
 
-    return re.sub(fr"[^\w\s{chinese}{punctuation}]+", "", text)
+    return sub(fr"[^\w\s{chinese}{punctuation}]+", "", text)
 
 
 def handle_blank_character(text: str, repl: Optional[str] = "") -> str:
     """处理空白字符，默认替换成空字符
 
     Attributes:
         text: input text
         repl: replace text
     """
-    return re.sub(r"\s+", repl, text)
+    return sub(r"\s+", repl, text)
 
 
 def uppercase_to_lowercase(text: str) -> str:
     """大写转小写
 
     Attributes:
         text: input text
@@ -82,23 +82,23 @@
     """替换一些字符
 
     Attributes:
         text: input text
         ptn: re pattern
         repl: replace text
     """
-    return re.sub(ptn, repl, text)
+    return sub(ptn, repl, text)
 
 
 def preprocess(data: Union[str, list], pipelines: Optional[list] = None, params: Optional[dict] = None) \
         -> Union[str, list]:
     """文本预处理
 
     Attributes:
-        data: input data.
+        data: input data
         pipelines: default is
             ["handle_blank_character",
             "uppercase_to_lowercase",
             "traditional_to_simplified",
             "full_angle_to_half_angle"]
         params: function parameters
     """
```

### Comparing `proces-0.1.4/proces/preprocess_test.py` & `proces-0.1.5/proces/preprocess_test.py`

 * *Files identical despite different names*

### Comparing `proces-0.1.4/proces.egg-info/PKG-INFO` & `proces-0.1.5/proces.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: proces
-Version: 0.1.4
+Version: 0.1.5
 Summary: text preprocess.
 Home-page: https://github.com/Ailln/proces
 Author: Ailln
 Author-email: kinggreenhall@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Proces
```

### Comparing `proces-0.1.4/setup.py` & `proces-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import os
 import sys
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 
 NAME = "proces"
 AUTHOR = "Ailln"
 EMAIL = "kinggreenhall@gmail.com"
 URL = "https://github.com/Ailln/proces"
 LICENSE = "MIT License"
 DESCRIPTION = "text preprocess."
 
 if sys.version_info < (3, 6, 0):
-    raise RuntimeError(f"{NAME} requires Python >=3.6.0, but yours is {sys.version}!")
+    raise RuntimeError(f"{NAME} requires Python >= 3.6.0, but yours is {sys.version}!")
 
 __version__ = "0.0.0"
 try:
     lib_py = os.path.join(NAME, "__init__.py")
     with open(lib_py, "r", encoding="utf8") as f_v:
         v_line = ""
         for line in f_v.readlines():
             if line.startswith("__version__"):
                 v_line = line.strip()
                 break
-        exec(v_line)  # get __version__ from __init__.py
+        # get __version__ from __init__.py
+        exec(v_line)
 except FileNotFoundError as e:
     raise e
 
-
 if __name__ == "__main__":
     setup(
         name=NAME,
         version=__version__,
         author=AUTHOR,
         author_email=EMAIL,
         url=URL,
         license=LICENSE,
         description=DESCRIPTION,
-        packages=find_packages(),
+        packages=find_namespace_packages(),
+        long_description=open("./README.md", "r", encoding="utf-8").read(),
+        long_description_content_type="text/markdown",
         include_package_data=True,
         install_reqires=[],
         setup_requires=["setuptools>=67.6.0"],
-        long_description=open("./README.md", "r", encoding="utf-8").read(),
-        long_description_content_type='text/markdown',
         zip_safe=True,
         classifiers=[
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
             f"License :: OSI Approved :: {LICENSE}",
             "Operating System :: OS Independent",
         ],
         python_requires=">=3.6"
     )
```

