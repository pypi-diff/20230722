# Comparing `tmp/dunderlab-djangoship-0.1a11.tar.gz` & `tmp/dunderlab-djangoship-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dunderlab-djangoship-0.1a11.tar", last modified: Fri Jul 21 23:12:23 2023, max compression
+gzip compressed data, was "dunderlab-djangoship-0.1a3.tar", last modified: Thu Mar 30 04:56:26 2023, max compression
```

## Comparing `dunderlab-djangoship-0.1a11.tar` & `dunderlab-djangoship-0.1a3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-21 23:12:23.990543 dunderlab-djangoship-0.1a11/
--rw-r--r--   0 yeison    (1000) users      (984)      632 2023-07-21 23:12:23.990543 dunderlab-djangoship-0.1a11/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)       13 2023-03-18 04:47:06.000000 dunderlab-djangoship-0.1a11/README.md
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-21 23:12:23.990543 dunderlab-djangoship-0.1a11/cmd/
--rw-r--r--   0 yeison    (1000) users      (984)     1861 2023-05-07 17:57:35.000000 dunderlab-djangoship-0.1a11/cmd/djangoship
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-21 23:12:23.990543 dunderlab-djangoship-0.1a11/dunderlab/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-21 23:12:23.990543 dunderlab-djangoship-0.1a11/dunderlab/djangoship/
--rw-r--r--   0 yeison    (1000) users      (984)        2 2023-03-18 04:48:23.000000 dunderlab-djangoship-0.1a11/dunderlab/djangoship/__init__.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-21 23:12:23.990543 dunderlab-djangoship-0.1a11/dunderlab_djangoship.egg-info/
--rw-r--r--   0 yeison    (1000) users      (984)      632 2023-07-21 23:12:23.000000 dunderlab-djangoship-0.1a11/dunderlab_djangoship.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)      242 2023-07-21 23:12:23.000000 dunderlab-djangoship-0.1a11/dunderlab_djangoship.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) users      (984)        1 2023-07-21 23:12:23.000000 dunderlab-djangoship-0.1a11/dunderlab_djangoship.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) users      (984)       10 2023-07-21 23:12:23.000000 dunderlab-djangoship-0.1a11/dunderlab_djangoship.egg-info/top_level.txt
--rw-r--r--   0 yeison    (1000) users      (984)       38 2023-07-21 23:12:23.990543 dunderlab-djangoship-0.1a11/setup.cfg
--rw-r--r--   0 yeison    (1000) users      (984)     1076 2023-04-22 20:07:40.000000 dunderlab-djangoship-0.1a11/setup.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-30 04:56:26.085305 dunderlab-djangoship-0.1a3/
+-rw-r--r--   0 yeison    (1000) users      (984)      631 2023-03-30 04:56:26.081971 dunderlab-djangoship-0.1a3/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)       13 2023-03-18 04:47:06.000000 dunderlab-djangoship-0.1a3/README.md
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-30 04:56:26.081971 dunderlab-djangoship-0.1a3/cmd/
+-rw-r--r--   0 yeison    (1000) users      (984)     1078 2023-03-30 04:54:20.000000 dunderlab-djangoship-0.1a3/cmd/djangoship
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-30 04:56:26.081971 dunderlab-djangoship-0.1a3/dunderlab/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-30 04:56:26.081971 dunderlab-djangoship-0.1a3/dunderlab/djangoship/
+-rw-r--r--   0 yeison    (1000) users      (984)        2 2023-03-18 04:48:23.000000 dunderlab-djangoship-0.1a3/dunderlab/djangoship/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-03-30 04:56:26.081971 dunderlab-djangoship-0.1a3/dunderlab_djangoship.egg-info/
+-rw-r--r--   0 yeison    (1000) users      (984)      631 2023-03-30 04:56:25.000000 dunderlab-djangoship-0.1a3/dunderlab_djangoship.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)      242 2023-03-30 04:56:26.000000 dunderlab-djangoship-0.1a3/dunderlab_djangoship.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) users      (984)        1 2023-03-30 04:56:25.000000 dunderlab-djangoship-0.1a3/dunderlab_djangoship.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       10 2023-03-30 04:56:25.000000 dunderlab-djangoship-0.1a3/dunderlab_djangoship.egg-info/top_level.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       38 2023-03-30 04:56:26.085305 dunderlab-djangoship-0.1a3/setup.cfg
+-rw-r--r--   0 yeison    (1000) users      (984)     1075 2023-03-30 04:56:16.000000 dunderlab-djangoship-0.1a3/setup.py
```

### Comparing `dunderlab-djangoship-0.1a11/PKG-INFO` & `dunderlab-djangoship-0.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunderlab-djangoship
-Version: 0.1a11
+Version: 0.1a3
 Summary: DjangoShip
 Download-URL: https://github.com/dunderlab/python-dunderlab.djangoship
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: BSD-2-Clause
```

### Comparing `dunderlab-djangoship-0.1a11/dunderlab_djangoship.egg-info/PKG-INFO` & `dunderlab-djangoship-0.1a3/dunderlab_djangoship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunderlab-djangoship
-Version: 0.1a11
+Version: 0.1a3
 Summary: DjangoShip
 Download-URL: https://github.com/dunderlab/python-dunderlab.djangoship
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: BSD-2-Clause
```

### Comparing `dunderlab-djangoship-0.1a11/setup.py` & `dunderlab-djangoship-0.1a3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 setup(
     name='dunderlab-djangoship',
-    version='0.1a11',
+    version='0.1a3',
     packages=['dunderlab.djangoship'],
     author='Yeison Cardona',
     author_email='yencardonaal@unal.edu.co',
     maintainer='Yeison Cardona',
     maintainer_email='yencardonaal@unal.edu.co',
     download_url='https://github.com/dunderlab/python-dunderlab.djangoship',
     install_requires=[
```

