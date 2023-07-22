# Comparing `tmp/pyntweb-0.2.6.tar.gz` & `tmp/pyntweb-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntweb-0.2.6.tar", last modified: Fri Jul 21 20:04:03 2023, max compression
+gzip compressed data, was "pyntweb-0.2.7.tar", last modified: Sat Jul 22 13:07:25 2023, max compression
```

## Comparing `pyntweb-0.2.6.tar` & `pyntweb-0.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 20:04:03.616702 pyntweb-0.2.6/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    35149 2023-07-21 15:15:13.000000 pyntweb-0.2.6/LICENSE
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-21 20:04:03.613369 pyntweb-0.2.6/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      550 2023-07-21 15:15:13.000000 pyntweb-0.2.6/README.md
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 20:04:03.600036 pyntweb-0.2.6/ntcss/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.6/ntcss/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.6/ntcss/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 15:15:13.000000 pyntweb-0.2.6/ntcss/ntml_parser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.6/ntcss/ntmlc.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.6/ntcss/tran.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 20:04:03.603369 pyntweb-0.2.6/ntml/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.6/ntml/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.6/ntml/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2561 2023-07-21 15:15:13.000000 pyntweb-0.2.6/ntml/errors.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5550 2023-07-21 19:53:43.000000 pyntweb-0.2.6/ntml/ntml_parser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.6/ntml/ntmlc.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13738 2023-07-21 20:03:45.000000 pyntweb-0.2.6/ntml/tran.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 20:04:03.603369 pyntweb-0.2.6/pyntweb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-21 20:04:03.000000 pyntweb-0.2.6/pyntweb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      500 2023-07-21 20:04:03.000000 pyntweb-0.2.6/pyntweb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 20:04:03.000000 pyntweb-0.2.6/pyntweb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:18:26.000000 pyntweb-0.2.6/pyntweb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       18 2023-07-21 20:04:03.000000 pyntweb-0.2.6/pyntweb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       20 2023-07-21 20:04:03.000000 pyntweb-0.2.6/pyntweb.egg-info/top_level.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      784 2023-07-21 20:03:54.000000 pyntweb-0.2.6/pyproject.toml
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-21 20:04:03.616702 pyntweb-0.2.6/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      869 2023-07-21 20:03:58.000000 pyntweb-0.2.6/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-21 20:04:03.613369 pyntweb-0.2.6/webfalco/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      228 2023-07-21 15:15:13.000000 pyntweb-0.2.6/webfalco/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.6/webfalco/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5524 2023-07-21 15:15:13.000000 pyntweb-0.2.6/webfalco/lrparser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.6/webfalco/tran.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.6/webfalco/webfalcoc.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.449930 pyntweb-0.2.7/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    35149 2023-07-21 15:15:13.000000 pyntweb-0.2.7/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-22 13:07:25.449930 pyntweb-0.2.7/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      550 2023-07-21 15:15:13.000000 pyntweb-0.2.7/README.md
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.446597 pyntweb-0.2.7/ntcss/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/ntml_parser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/ntmlc.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/tran.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.446597 pyntweb-0.2.7/ntml/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntml/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntml/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2561 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntml/errors.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5550 2023-07-22 13:06:51.000000 pyntweb-0.2.7/ntml/ntml_parser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntml/ntmlc.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13738 2023-07-21 20:03:45.000000 pyntweb-0.2.7/ntml/tran.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.446597 pyntweb-0.2.7/pyntweb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      500 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:18:26.000000 pyntweb-0.2.7/pyntweb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       18 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       20 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/top_level.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      784 2023-07-22 13:07:17.000000 pyntweb-0.2.7/pyproject.toml
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-22 13:07:25.449930 pyntweb-0.2.7/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      869 2023-07-22 13:07:14.000000 pyntweb-0.2.7/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.449930 pyntweb-0.2.7/webfalco/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      228 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5524 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/lrparser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/tran.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/webfalcoc.py
```

### Comparing `pyntweb-0.2.6/LICENSE` & `pyntweb-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.6/PKG-INFO` & `pyntweb-0.2.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,19 @@
-Metadata-Version: 2.1
-Name: pyntweb
-Version: 0.2.6
-Summary: NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом кодеПосесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi
-Author-email: talismanchet@vk.com
-License: GNU GPL 3.0
-License-File: LICENSE
+"""
+setup.py
+"""
+
+from setuptools import setup
+
+setup(name='pyntweb',
+      version='0.2.7',
+      description='''
+NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: 
+HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же 
+традиционные языки нативно поддерживаются в самом коде
+
+Посесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi'''.replace("\n", ""),
+      packages=['ntml', 'webfalco', 'ntcss'],
+      license='GNU GPL 3.0',
+      install_requires=['parglare', 'colorama'],
+      author_email='talismanchet@vk.com',
+      zip_safe=False)
```

### Comparing `pyntweb-0.2.6/README.md` & `pyntweb-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.6/ntcss/ntml_parser.py` & `pyntweb-0.2.7/ntcss/ntml_parser.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.6/ntcss/tran.py` & `pyntweb-0.2.7/ntcss/tran.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.6/ntml/errors.py` & `pyntweb-0.2.7/ntml/errors.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.6/ntml/ntml_parser.py` & `pyntweb-0.2.7/ntml/ntml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     Simport: Timport "(" Tname "," Tstr ")" Tstr;
 
     Stitle: Ttitle Tstr;
 
     Stag: Ttagname Sprops? Sbody? | Tscript Sprops Tbody?;
 
-        Sprops: "(" ( (Sassign ( "," Sassign )*)? (Tat Tstr+)? ) ")";
+        Sprops: "(" ( (Sassign ( "," Sassign )*)? (Tat Tstr)* ) ")";
 
             Sassign: Tname "=" Sexpr;
 
                 Sexpr: "(" Sexpr ")"
                      | Sexpr "**" Sexpr
                      | Sexpr "*" Sexpr
                      | Sexpr "/" Sexpr
@@ -50,15 +50,15 @@
 Tcomment: /\/\*.*\*\//;
 Tdoctype: "doctype";
 Tntml: /ntml/;
 Timport: "import";
 Ttitle: "title";
 Tscript: /script\b\s*(?=\()/;
 Ttagname: /(?!script)\b[A-Za-zА-Яа-яЁё_]\w*\b\s*(?=(\(|\{))/;
-Tname: /\b[A-Za-zА-Яа-яЁё_]\w*\b(?!(\(|\{))/;
+Tname: /\b[A-Za-zА-Яа-яЁё_-]\w*\b(?!(\(|\{))/;
 Tint: /0[xX](?:_?[0-9a-fA-F])+|0[bB](?:_?[01])+|0[oO](?:_?[0-7])+|(?:0(?:_?0)*|[1-9](?:_?\d)*)/;
 Tverfloat: /\d\.\d+(\.\d+)?/;
 Tfloat: /\d(?:_?\d)*\.(?:\d(?:_?\d)*)?/;
 Tescape: /\[.{1,4}\]/;
 Tat: "@";
 Tbody: /\#\{[^\}\\]*(?:\[.[^\}\\]\]*)*\}/;
 Tany: /(\+|\;|\/|\/|\*|\`|\’|\:|\d|\?|\&|\~|\'|\"SUPPRESS_NEWLINW
```

### Comparing `pyntweb-0.2.6/ntml/tran.py` & `pyntweb-0.2.7/ntml/tran.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.6/pyntweb.egg-info/PKG-INFO` & `pyntweb-0.2.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Metadata-Version: 2.1
 Name: pyntweb
-Version: 0.2.6
+Version: 0.2.7
 Summary: NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом кодеПосесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi
 Author-email: talismanchet@vk.com
 License: GNU GPL 3.0
 License-File: LICENSE
```

### Comparing `pyntweb-0.2.6/pyproject.toml` & `pyntweb-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyntweb"
-version = "0.2.6"
+version = "0.2.7"
 description = "NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом коде."
 authors = ["Talisman Chet <talismanchet@vk.com>"]
 license = "GNU GPL 3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyntweb-0.2.6/webfalco/lrparser.py` & `pyntweb-0.2.7/webfalco/lrparser.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.6/webfalco/tran.py` & `pyntweb-0.2.7/webfalco/tran.py`

 * *Files identical despite different names*

