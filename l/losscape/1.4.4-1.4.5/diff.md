# Comparing `tmp/losscape-1.4.4.tar.gz` & `tmp/losscape-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.4.4.tar", last modified: Sat Jul 22 07:57:19 2023, max compression
+gzip compressed data, was "losscape-1.4.5.tar", last modified: Sat Jul 22 09:13:33 2023, max compression
```

## Comparing `losscape-1.4.4.tar` & `losscape-1.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 07:57:19.961383 losscape-1.4.4/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 07:57:19.961383 losscape-1.4.4/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.4.4/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 07:57:19.961383 losscape-1.4.4/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.4.4/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.4.4/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.4.4/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16226 2023-07-22 07:56:43.000000 losscape-1.4.4/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.4.4/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 07:57:19.961383 losscape-1.4.4/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 07:57:19.000000 losscape-1.4.4/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-22 07:57:19.000000 losscape-1.4.4/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-22 07:57:19.000000 losscape-1.4.4/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-22 07:57:19.000000 losscape-1.4.4/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-22 07:57:19.000000 losscape-1.4.4/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-22 07:57:19.961383 losscape-1.4.4/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      588 2023-07-22 07:57:04.000000 losscape-1.4.4/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 09:13:33.168268 losscape-1.4.5/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 09:13:33.168268 losscape-1.4.5/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.4.5/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 09:13:33.168268 losscape-1.4.5/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.4.5/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.4.5/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.4.5/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16226 2023-07-22 07:56:43.000000 losscape-1.4.5/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.4.5/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 09:13:33.168268 losscape-1.4.5/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-22 09:13:33.168268 losscape-1.4.5/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      596 2023-07-22 09:13:26.000000 losscape-1.4.5/setup.py
```

### Comparing `losscape-1.4.4/PKG-INFO` & `losscape-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.4.4
+Version: 1.4.5
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.4.4/README.md` & `losscape-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `losscape-1.4.4/losscape/compute_loss.py` & `losscape-1.4.5/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.4/losscape/create_directions.py` & `losscape-1.4.5/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.4/losscape/create_landscape.py` & `losscape-1.4.5/losscape/create_landscape.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.4/losscape/train.py` & `losscape-1.4.5/losscape/train.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.4/losscape.egg-info/PKG-INFO` & `losscape-1.4.5/losscape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.4.4
+Version: 1.4.5
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.4.4/setup.py` & `losscape-1.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from pathlib import Path
 current_dir = Path(__file__).parent
 desc = (current_dir / "README.md").read_text()
 
 setup(
     name='losscape',
-    version='1.4.4',
+    version='1.4.5',
     url='https://github.com/Procuste34/losscape',
     author='Alexandre TL',
     author_email='alexandretl3434@gmail.com',
     description='Visualize easily the loss landscape of your neural networks',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),  
-    install_requires=['torch>=1.8.1', 'numpy', 'scipy', 'matplotlib'],
+    install_requires=['torch>=1.8.1', 'numpy', 'scipy', 'matplotlib', 'h5py'],
 )
```

