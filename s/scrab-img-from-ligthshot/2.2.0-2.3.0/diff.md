# Comparing `tmp/scrab_img_from_ligthshot-2.2.0.tar.gz` & `tmp/scrab_img_from_ligthshot-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrab_img_from_ligthshot-2.2.0.tar", max compression
+gzip compressed data, was "scrab_img_from_ligthshot-2.3.0.tar", max compression
```

## Comparing `scrab_img_from_ligthshot-2.2.0.tar` & `scrab_img_from_ligthshot-2.3.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    10173 2023-06-07 15:41:05.465902 scrab_img_from_ligthshot-2.2.0/LICENSE
--rw-r--r--   0        0        0     2122 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/README.md
--rw-r--r--   0        0        0      640 2023-07-14 17:28:50.230603 scrab_img_from_ligthshot-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/src/silf/__init__.py
--rw-r--r--   0        0        0     1334 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/src/silf/cli.py
--rwxr-xr-x   0        0        0     2977 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/src/silf/main.py
--rw-r--r--   0        0        0     3873 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/src/silf/scrab_img_from_lightshot.py
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 scrab_img_from_ligthshot-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-07-19 10:22:06.952679 scrab_img_from_ligthshot-2.3.0/LICENSE
+-rw-r--r--   0        0        0     2186 2023-07-19 10:22:06.952679 scrab_img_from_ligthshot-2.3.0/README.md
+-rw-r--r--   0        0        0      744 2023-07-22 01:09:37.426502 scrab_img_from_ligthshot-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-07-22 01:03:38.638419 scrab_img_from_ligthshot-2.3.0/src/silf/__init__.py
+-rw-r--r--   0        0        0     1409 2023-07-22 01:03:38.638419 scrab_img_from_ligthshot-2.3.0/src/silf/cli.py
+-rw-r--r--   0        0        0     2041 2023-07-22 01:03:38.638419 scrab_img_from_ligthshot-2.3.0/src/silf/ect.py
+-rwxr-xr-x   0        0        0     1370 2023-07-22 01:03:38.638419 scrab_img_from_ligthshot-2.3.0/src/silf/main.py
+-rw-r--r--   0        0        0     5232 2023-07-22 01:03:38.638419 scrab_img_from_ligthshot-2.3.0/src/silf/scrab_img_from_lightshot.py
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 scrab_img_from_ligthshot-2.3.0/PKG-INFO
```

### Comparing `scrab_img_from_ligthshot-2.2.0/LICENSE` & `scrab_img_from_ligthshot-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrab_img_from_ligthshot-2.2.0/README.md` & `scrab_img_from_ligthshot-2.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry)
+![PyPI](https://img.shields.io/pypi/v/scrab-img-from-ligthshot)
 ![Static Badge](https://img.shields.io/badge/poetry-1.4%2B-green)
 ![Static Badge](https://img.shields.io/badge/only_linux_support-green)
 ![Static Badge](https://img.shields.io/badge/pass_tests-none-red)
 ![GitHub issues](https://img.shields.io/github/issues-raw/Transparency010101/scrab-img-from-ligthshot)
 
 
 # Scrab Img(images) From LightShot
```

### Comparing `scrab_img_from_ligthshot-2.2.0/src/silf/cli.py` & `scrab_img_from_ligthshot-2.3.0/src/silf/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This module provide only CLI interface
+"""This module provide CLI interface
 
 License:
     Copyright 2023 Transparency010101
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
@@ -15,36 +15,36 @@
     See the License for the specific language governing permissions and
     limitations under the License.
 
 Foreword:
     I'm trying to observe standards of code writing on Python(PEP8)
 
 Functions:
-    cli
+    cli: CLI interface
 """
 
 import argparse
 
 
 def cli():
     """CLI interface
 
     Returns:
         Namespace
     """
+    description = """
+    This program download images from ligthshot's site. See more in README file
+    """
     cli_parser = argparse.ArgumentParser(
-        prog="silf",
-        description="This program download images from ligthshot's site. See more in README file"
-    )
+            prog="silf",
+            description=description)
     cli_parser.add_argument(
-        "count_of_images",
-        help="Just print hello world",
-        type=int
-    )
+            "count_of_images",
+            help="Just print hello world",
+            type=int)
     cli_parser.add_argument(
-        "-D", "--delete_images",
-        action="store_false",
-        help="to don't delete images in folder",
-        default=True
-    )
+            "-D", "--delete_images",
+            action="store_false",
+            help="to don't delete images in folder",
+            default=True)
 
     return cli_parser.parse_args()
```

### Comparing `scrab_img_from_ligthshot-2.2.0/src/silf/main.py` & `scrab_img_from_ligthshot-2.3.0/src/silf/ect.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Download images from Lightshot's site
+"""This module contain necessary functions for good working, or convince
 
 License:
     Copyright 2023 Transparency010101
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
@@ -14,94 +14,55 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
 Foreword:
     I'm trying to observe standards of code writing on Python(PEP8)
 
-Usage:
-    See in README file
-
 Functions:
-    create_img_folder_if_not_exist
-    delete_all_images
-    start_downloading
-    main
+    create_img_folder_if_not_exist: Create folder img/ if it doesn't exist.
+    delete_all_images: Delete all images from folder img/
 """
 
-import time
 import os
 
-from .scrab_img_from_lightshot import ScrabImgFromLightShot
-from .cli import cli
+from .scrab_img_from_lightshot import (
+    ScrabImgFromLightShot,
+    PATH_TO_FOLDER_IMG
+)
 
 
 def create_img_folder_if_not_exist():
     """Create folder img/ if it doesn't exist.
 
     If folder img/ doesn't exist will be an error, so need to check this every
     time when program starts.
 
     Returns:
         None
     """
-    if not os.path.exists("img/"):
-        os.makedirs(os.path.dirname("img/"))
+    if not os.path.exists(PATH_TO_FOLDER_IMG):
+        os.makedirs(os.path.dirname(PATH_TO_FOLDER_IMG))
 
 
-def delete_all_images(to_delete):
+def do_delete_all_images(to_delete):
     """Delete all images from folder img/
 
     It did it for convince, to don't delete it manually. There are 2 choices to
-    delete it, or not, for convince.
+    delete it, or not, for convince. And it's option, if folder img/ contain
+    some images.
 
     Arguments:
         to_delete (bool): to delete images from folder img/
 
     Returns:
         None
     """
-    if len(os.listdir("img/")) != 0:
+    if len(os.listdir(PATH_TO_FOLDER_IMG)) != 0:
         if to_delete:
-            for folder, _, files in os.walk("img/"):
+            for folder, _, files in os.walk(PATH_TO_FOLDER_IMG):
                 for file in files:
                     os.remove(folder + file)
         elif not to_delete:
             pass
         else:
             print("Incorrect input, try again")
-
-
-def start_downloading(number_of_images, debug_mod=False):
-    """Start downloading images
-
-    Arguments:
-        number_of_images (int): number of images, that need to download
-        debug_mod (bool): turn on/off debug mod
-
-    Returns:
-        None
-    """
-    # While this code executing, sometimes errors occur and that stop program
-    # that's why code wrapped in try/except, but there is nuance, bugs that I
-    # accidentally made while developing, are not shown, so there is debug mod
-    # in function
-    while number_of_images != len(os.listdir("img/")):
-        try:
-            ScrabImgFromLightShot.download_img()
-        except Exception as error:
-            if debug_mod:
-                print("SOMETHING WENT WRONG!:")
-                print(error)
-            pass
-
-
-def main():
-    """Enter point in program"""
-    start_program_time = time.time()
-
-    cli_args = cli()
-    create_img_folder_if_not_exist()
-    delete_all_images(cli_args.delete_images)
-    start_downloading(cli_args.count_of_images)
-
-    print(f"All time: {int(time.time() - start_program_time)}")
```

### Comparing `scrab_img_from_ligthshot-2.2.0/PKG-INFO` & `scrab_img_from_ligthshot-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrab-img-from-ligthshot
-Version: 2.2.0
+Version: 2.3.0
 Summary: scrab images from ligthshot (i don't know is this legal)
 Home-page: https://github.com/Transparency010101/scrab-img-from-ligthshot
 License: Apache-2.0
 Author: ossys
 Author-email: ossys1010110@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,15 @@
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Project-URL: Repository, https://github.com/Transparency010101/scrab-img-from-ligthshot
 Description-Content-Type: text/markdown
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry)
+![PyPI](https://img.shields.io/pypi/v/scrab-img-from-ligthshot)
 ![Static Badge](https://img.shields.io/badge/poetry-1.4%2B-green)
 ![Static Badge](https://img.shields.io/badge/only_linux_support-green)
 ![Static Badge](https://img.shields.io/badge/pass_tests-none-red)
 ![GitHub issues](https://img.shields.io/github/issues-raw/Transparency010101/scrab-img-from-ligthshot)
 
 
 # Scrab Img(images) From LightShot
```

