# Comparing `tmp/FicImageScript-1.0.2.tar.gz` & `tmp/FicImageScript-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FicImageScript-1.0.2.tar", last modified: Fri May 12 16:34:55 2023, max compression
+gzip compressed data, was "FicImageScript-2.0.0.tar", last modified: Sat Jul 22 10:33:59 2023, max compression
```

## Comparing `FicImageScript-1.0.2.tar` & `FicImageScript-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-12 16:34:55.014353 FicImageScript-1.0.2/
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-12 16:34:55.002352 FicImageScript-1.0.2/FicImage/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       22 2023-05-12 16:34:10.000000 FicImageScript-1.0.2/FicImage/__init__.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5514 2023-05-08 22:25:50.000000 FicImageScript-1.0.2/FicImage/image.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     4648 2023-05-12 15:10:31.000000 FicImageScript-1.0.2/FicImage/main.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     2265 2023-05-12 13:41:09.000000 FicImageScript-1.0.2/FicImage/utils.py
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-12 16:34:55.010353 FicImageScript-1.0.2/FicImageScript.egg-info/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     6811 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      361 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/SOURCES.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/dependency_links.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/entry_points.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/requires.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/top_level.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImageScript-1.0.2/LICENSE
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     6811 2023-05-12 16:34:55.010353 FicImageScript-1.0.2/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     6087 2023-05-12 15:54:55.000000 FicImageScript-1.0.2/PYPI_README.rst
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5698 2023-05-08 23:07:54.000000 FicImageScript-1.0.2/README.md
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      955 2023-05-12 16:11:28.000000 FicImageScript-1.0.2/pyproject.toml
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-12 16:34:55.014353 FicImageScript-1.0.2/setup.cfg
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1252 2023-05-12 16:34:10.000000 FicImageScript-1.0.2/setup.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1000)        0 2023-07-22 10:33:59.170045 FicImageScript-2.0.0/
+drwxrwxr-x   0 nonso     (1000) nonso     (1000)        0 2023-07-22 10:33:59.170045 FicImageScript-2.0.0/FicImage/
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)        0 2023-07-22 10:31:02.000000 FicImageScript-2.0.0/FicImage/__init__.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)     5514 2023-07-22 10:31:02.000000 FicImageScript-2.0.0/FicImage/image.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)     7464 2023-07-22 10:31:02.000000 FicImageScript-2.0.0/FicImage/main.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)     2404 2023-07-22 10:31:02.000000 FicImageScript-2.0.0/FicImage/utils.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1000)        0 2023-07-22 10:33:59.170045 FicImageScript-2.0.0/FicImageScript.egg-info/
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)     8445 2023-07-22 10:33:59.000000 FicImageScript-2.0.0/FicImageScript.egg-info/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)      361 2023-07-22 10:33:59.000000 FicImageScript-2.0.0/FicImageScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)        1 2023-07-22 10:33:59.000000 FicImageScript-2.0.0/FicImageScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)       48 2023-07-22 10:33:59.000000 FicImageScript-2.0.0/FicImageScript.egg-info/entry_points.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)      182 2023-07-22 10:33:59.000000 FicImageScript-2.0.0/FicImageScript.egg-info/requires.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)        9 2023-07-22 10:33:59.000000 FicImageScript-2.0.0/FicImageScript.egg-info/top_level.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)     1075 2023-07-22 10:31:02.000000 FicImageScript-2.0.0/LICENSE
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)     8445 2023-07-22 10:33:59.170045 FicImageScript-2.0.0/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)     6399 2023-07-22 10:31:18.000000 FicImageScript-2.0.0/PYPI_README.rst
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)     5929 2023-07-22 10:31:02.000000 FicImageScript-2.0.0/README.md
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)      934 2023-07-22 10:33:42.000000 FicImageScript-2.0.0/pyproject.toml
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)       38 2023-07-22 10:33:59.170045 FicImageScript-2.0.0/setup.cfg
+-rw-rw-r--   0 nonso     (1000) nonso     (1000)     1252 2023-07-22 10:31:02.000000 FicImageScript-2.0.0/setup.py
```

### Comparing `FicImageScript-1.0.2/FicImage/image.py` & `FicImageScript-2.0.0/FicImage/image.py`

 * *Files identical despite different names*

### Comparing `FicImageScript-1.0.2/FicImage/utils.py` & `FicImageScript-2.0.0/FicImage/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,16 +38,18 @@
 def load_config_json(ficimage_path: str) -> dict:
 	"""
 	Loads ficimage.json. Calls `sys.exit` if there's a JSONDecodeError.
 	:param ficimage_path: The path to ficimage.json.
 	:return: A dict containing the data stored inside ficimage.json
 	"""
 	try:
-		with open(os.path.join(ficimage_path, "../ficimage.json"), 'r') as f:
+		with open(os.path.join(ficimage_path, "ficimage.json"), 'r') as f:
 			return json.load(f)
+	except FileNotFoundError:
+		sys.exit(f"[Loading Config JSON]: File not found. Are you sure there's a ficimage.json file in {ficimage_path}")
 	except json.decoder.JSONDecodeError:
 		sys.exit("[Loading Config JSON]: Invalid JSON in Config File")
 
 
 def default_ficimage_settings() -> dict:
 	"""
 	Returns a dict containing the default config settings for ficimage.
```

### Comparing `FicImageScript-1.0.2/FicImageScript.egg-info/PKG-INFO` & `FicImageScript-2.0.0/FicImageScript.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,39 @@
 Metadata-Version: 2.1
 Name: FicImageScript
-Version: 1.0.2
+Version: 2.0.0
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
-Author-email: jemenichinonso11@gmail.com
+Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Emmanuel C. Jemeni
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/Jemeni11/FicImage
 Project-URL: Bug Tracker, https://github.com/Jemeni11/FicImage/issues
-Keywords: fanfiction fichub ficimage image download epub
+Keywords: fanfiction,fichub,ficimage,image
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -29,36 +52,40 @@
 ----------
 
 Installation with PIP
 ~~~~~~~~~~~~~~~~~~~~~
 
 1. Install FicImage using ``pip install FicImageScript``.
 2. After installation, run the program using
-   ``ficimage path/to/epub -c path/to/ficimage/json`` where
+   ``ficimage -p path/to/epub -c path/to/ficimage/json`` where
    ``path/to/epub`` is the path to the **FicHub epub** you want to add
    images to and ``path/to/ficimage/json`` is the path to a file called
    **ficimage.json** . ficimage.json lets you configure FicImage. See
    more `in the configuration section below <#configuration>`__.
 
 .. code:: shell
 
    (virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
-   usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
+    usage: main.py [-h] [-p PATH_TO_EPUB] [-c CONFIG_FILE_PATH] [-d] [-v] [-r RECURSIVE]
 
-   Update a FicHub epub file with images.
+    Update a FicHub epub file with images.
 
-   positional arguments:
-     path_to_epub          The path to the FicHub epub file.
-
-   optional arguments:
-     -h, --help            show this help message and exit
-     -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
-                           The path to the ficimage.json file.
-     -d, --debug           Enable debug mode.
+    options:
+      -h, --help            show this help message and exit
+      -p PATH_TO_EPUB, --path_to_epub PATH_TO_EPUB
+                            The path to the FicHub epub file.
+      -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
+                            The path to the ficimage.json file.
+      -d, --debug           Enable debug mode.
+      -v, --version         Prints out the current version and quits
+      -r RECURSIVE, --recursive RECURSIVE
+                            This will update all files in the directory path given and its subdirectories
 
+..              
+                            
 Image Support
 ~~~~~~~~~~~~~
 
 `FicHub <https://fichub.net/>`__ creates EPUB 3.3 files, which means
 that FicImage only save images in the following file format:
 
 - JPEG
```

### Comparing `FicImageScript-1.0.2/LICENSE` & `FicImageScript-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FicImageScript-1.0.2/PKG-INFO` & `FicImageScript-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,39 @@
 Metadata-Version: 2.1
 Name: FicImageScript
-Version: 1.0.2
+Version: 2.0.0
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
-Author-email: jemenichinonso11@gmail.com
+Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Emmanuel C. Jemeni
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/Jemeni11/FicImage
 Project-URL: Bug Tracker, https://github.com/Jemeni11/FicImage/issues
-Keywords: fanfiction fichub ficimage image download epub
+Keywords: fanfiction,fichub,ficimage,image
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -29,36 +52,40 @@
 ----------
 
 Installation with PIP
 ~~~~~~~~~~~~~~~~~~~~~
 
 1. Install FicImage using ``pip install FicImageScript``.
 2. After installation, run the program using
-   ``ficimage path/to/epub -c path/to/ficimage/json`` where
+   ``ficimage -p path/to/epub -c path/to/ficimage/json`` where
    ``path/to/epub`` is the path to the **FicHub epub** you want to add
    images to and ``path/to/ficimage/json`` is the path to a file called
    **ficimage.json** . ficimage.json lets you configure FicImage. See
    more `in the configuration section below <#configuration>`__.
 
 .. code:: shell
 
    (virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
-   usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
+    usage: main.py [-h] [-p PATH_TO_EPUB] [-c CONFIG_FILE_PATH] [-d] [-v] [-r RECURSIVE]
 
-   Update a FicHub epub file with images.
+    Update a FicHub epub file with images.
 
-   positional arguments:
-     path_to_epub          The path to the FicHub epub file.
-
-   optional arguments:
-     -h, --help            show this help message and exit
-     -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
-                           The path to the ficimage.json file.
-     -d, --debug           Enable debug mode.
+    options:
+      -h, --help            show this help message and exit
+      -p PATH_TO_EPUB, --path_to_epub PATH_TO_EPUB
+                            The path to the FicHub epub file.
+      -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
+                            The path to the ficimage.json file.
+      -d, --debug           Enable debug mode.
+      -v, --version         Prints out the current version and quits
+      -r RECURSIVE, --recursive RECURSIVE
+                            This will update all files in the directory path given and its subdirectories
 
+..              
+                            
 Image Support
 ~~~~~~~~~~~~~
 
 `FicHub <https://fichub.net/>`__ creates EPUB 3.3 files, which means
 that FicImage only save images in the following file format:
 
 - JPEG
```

### Comparing `FicImageScript-1.0.2/PYPI_README.rst` & `FicImageScript-2.0.0/PYPI_README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,36 +11,40 @@
 ----------
 
 Installation with PIP
 ~~~~~~~~~~~~~~~~~~~~~
 
 1. Install FicImage using ``pip install FicImageScript``.
 2. After installation, run the program using
-   ``ficimage path/to/epub -c path/to/ficimage/json`` where
+   ``ficimage -p path/to/epub -c path/to/ficimage/json`` where
    ``path/to/epub`` is the path to the **FicHub epub** you want to add
    images to and ``path/to/ficimage/json`` is the path to a file called
    **ficimage.json** . ficimage.json lets you configure FicImage. See
    more `in the configuration section below <#configuration>`__.
 
 .. code:: shell
 
    (virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
-   usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
+    usage: main.py [-h] [-p PATH_TO_EPUB] [-c CONFIG_FILE_PATH] [-d] [-v] [-r RECURSIVE]
 
-   Update a FicHub epub file with images.
+    Update a FicHub epub file with images.
 
-   positional arguments:
-     path_to_epub          The path to the FicHub epub file.
-
-   optional arguments:
-     -h, --help            show this help message and exit
-     -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
-                           The path to the ficimage.json file.
-     -d, --debug           Enable debug mode.
+    options:
+      -h, --help            show this help message and exit
+      -p PATH_TO_EPUB, --path_to_epub PATH_TO_EPUB
+                            The path to the FicHub epub file.
+      -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
+                            The path to the ficimage.json file.
+      -d, --debug           Enable debug mode.
+      -v, --version         Prints out the current version and quits
+      -r RECURSIVE, --recursive RECURSIVE
+                            This will update all files in the directory path given and its subdirectories
 
+..              
+                            
 Image Support
 ~~~~~~~~~~~~~
 
 `FicHub <https://fichub.net/>`__ creates EPUB 3.3 files, which means
 that FicImage only save images in the following file format:
 
 - JPEG
```

### Comparing `FicImageScript-1.0.2/README.md` & `FicImageScript-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 ## Introduction
 FicImage is an application designed to enhance the reading experience of FicHub epubs. With FicImage, users can easily add missing images to their FicHub epubs, bringing the stories to life with vibrant visuals. This user-friendly tool allows readers to fully immerse themselves in their favorite fan fiction stories and enjoy them in a whole new way.
 
 ## How to Use
 
 ### Installation with PIP
 1. Install FicImage using `pip install FicImageScript`.
-2.  After installation, run the program using `ficimage path/to/epub -c path/to/ficimage/json` 
+2.  After installation, run the program using `ficimage -p path/to/epub -c path/to/ficimage/json` 
 where `path/to/epub` is the path to the **FicHub epub** you want to add 
 images to and `path/to/ficimage/json` is the path to a file called **ficimage.json** . 
 ficimage.json lets you configure FicImage. See more [below](#configuration).
 
 
 ```shell
 (virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
-usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
+usage: main.py [-h] [-p PATH_TO_EPUB] [-c CONFIG_FILE_PATH] [-d] [-v] [-r RECURSIVE]
 
 Update a FicHub epub file with images.
 
-positional arguments:
-  path_to_epub          The path to the FicHub epub file.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
-                        The path to the ficimage.json file.
-  -d, --debug           Enable debug mode.
-
+options:
+  -h, --help                  Show this help message and exit.
+  -p PATH_TO_EPUB,            The path to the FicHub epub file.
+  --path_to_epub PATH_TO_EPUB
+  -c CONFIG_FILE_PATH,        The path to the ficimage.json file.
+  --config_file_path CONFIG_FILE_PATH
+  -d, --debug                 Enable debug mode.
+  -v, --version               Prints out the current version and quits.
+  -r RECURSIVE,               This will update all files in the directory path given and its subdirectories.
+  --recursive RECURSIVE
 ```
 
 ### Image Support
 
 [FicHub](https://fichub.net/) creates EPUB 3.3 files, which means that FicImage only save images 
 in the following file format:
 - JPEG
```

### Comparing `FicImageScript-1.0.2/pyproject.toml` & `FicImageScript-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#[project]
-#name = "FicImageScript"
-#version = "1.0.1"
-#authors = [
-#  { name="Emmanuel C. Jemeni", email="jemenichinonso11@gmail.com" }
-#]
-#description = "FicImage is an application designed to enhance the reading experience of FicHub epubs."
-#readme = "PYPI_README.rst"
-#requires-python = ">=3.6"
-#license = {file = "LICENSE"}
-#keywords = ["fanfiction", "fichub", "ficimage", "image"]
-#classifiers = [
-#    "Development Status :: 5 - Production/Stable",
-#    "Programming Language :: Python :: 3",
-#    "License :: OSI Approved :: MIT License",
-#    "Operating System :: OS Independent",
-#    "Topic :: Internet :: WWW/HTTP",
-#]
-#
-#[project.urls]
-#"Homepage" = "https://github.com/Jemeni11/FicImage"
-#"Bug Tracker" = "https://github.com/Jemeni11/FicImage/issues"
+[project]
+name = "FicImageScript"
+version = "2.0.0"
+authors = [
+  { name="Emmanuel C. Jemeni", email="jemenichinonso11@gmail.com" }
+]
+description = "FicImage is an application designed to enhance the reading experience of FicHub epubs."
+readme = "PYPI_README.rst"
+requires-python = ">=3.6"
+license = {file = "LICENSE"}
+keywords = ["fanfiction", "fichub", "ficimage", "image"]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Topic :: Internet :: WWW/HTTP",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/Jemeni11/FicImage"
+"Bug Tracker" = "https://github.com/Jemeni11/FicImage/issues"
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
-requires = ["setuptools>=43.0.0", "wheel"]
+requires = ["setuptools>=43.0.0", "wheel"]
```

### Comparing `FicImageScript-1.0.2/setup.py` & `FicImageScript-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("PYPI_README.rst", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="FicImageScript",
-	version="1.0.2",
+	version="2.0.0",
 	author="Emmanuel C. Jemeni",
 	author_email="jemenichinonso11@gmail.com",
 	description="FicImage is an application designed to enhance the reading experience of FicHub epubs.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://github.com/Jemeni11/FicImage",
 	project_urls={
```

