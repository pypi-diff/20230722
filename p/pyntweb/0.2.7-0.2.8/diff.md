# Comparing `tmp/pyntweb-0.2.7.tar.gz` & `tmp/pyntweb-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntweb-0.2.7.tar", last modified: Sat Jul 22 13:07:25 2023, max compression
+gzip compressed data, was "pyntweb-0.2.8.tar", last modified: Sat Jul 22 13:20:08 2023, max compression
```

## Comparing `pyntweb-0.2.7.tar` & `pyntweb-0.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.449930 pyntweb-0.2.7/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    35149 2023-07-21 15:15:13.000000 pyntweb-0.2.7/LICENSE
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-22 13:07:25.449930 pyntweb-0.2.7/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      550 2023-07-21 15:15:13.000000 pyntweb-0.2.7/README.md
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.446597 pyntweb-0.2.7/ntcss/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/ntml_parser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/ntmlc.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntcss/tran.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.446597 pyntweb-0.2.7/ntml/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntml/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntml/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2561 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntml/errors.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5550 2023-07-22 13:06:51.000000 pyntweb-0.2.7/ntml/ntml_parser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.7/ntml/ntmlc.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13738 2023-07-21 20:03:45.000000 pyntweb-0.2.7/ntml/tran.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.446597 pyntweb-0.2.7/pyntweb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      500 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:18:26.000000 pyntweb-0.2.7/pyntweb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       18 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       20 2023-07-22 13:07:25.000000 pyntweb-0.2.7/pyntweb.egg-info/top_level.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      784 2023-07-22 13:07:17.000000 pyntweb-0.2.7/pyproject.toml
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-22 13:07:25.449930 pyntweb-0.2.7/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      869 2023-07-22 13:07:14.000000 pyntweb-0.2.7/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:07:25.449930 pyntweb-0.2.7/webfalco/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      228 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/const.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5524 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/lrparser.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/tran.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.7/webfalco/webfalcoc.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:20:08.955130 pyntweb-0.2.8/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    35149 2023-07-21 15:15:13.000000 pyntweb-0.2.8/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-22 13:20:08.955130 pyntweb-0.2.8/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      550 2023-07-21 15:15:13.000000 pyntweb-0.2.8/README.md
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:20:08.951797 pyntweb-0.2.8/ntcss/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.8/ntcss/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.8/ntcss/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5462 2023-07-21 15:15:13.000000 pyntweb-0.2.8/ntcss/ntml_parser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.8/ntcss/ntmlc.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.8/ntcss/tran.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:20:08.951797 pyntweb-0.2.8/ntml/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      208 2023-07-21 15:15:13.000000 pyntweb-0.2.8/ntml/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.8/ntml/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2561 2023-07-21 15:15:13.000000 pyntweb-0.2.8/ntml/errors.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5670 2023-07-22 13:19:37.000000 pyntweb-0.2.8/ntml/ntml_parser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.8/ntml/ntmlc.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13738 2023-07-21 20:03:45.000000 pyntweb-0.2.8/ntml/tran.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:20:08.955130 pyntweb-0.2.8/pyntweb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      677 2023-07-22 13:20:08.000000 pyntweb-0.2.8/pyntweb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      500 2023-07-22 13:20:08.000000 pyntweb-0.2.8/pyntweb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-22 13:20:08.000000 pyntweb-0.2.8/pyntweb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-21 15:18:26.000000 pyntweb-0.2.8/pyntweb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       18 2023-07-22 13:20:08.000000 pyntweb-0.2.8/pyntweb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       20 2023-07-22 13:20:08.000000 pyntweb-0.2.8/pyntweb.egg-info/top_level.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      784 2023-07-22 13:20:05.000000 pyntweb-0.2.8/pyproject.toml
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-22 13:20:08.955130 pyntweb-0.2.8/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      869 2023-07-22 13:20:03.000000 pyntweb-0.2.8/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-22 13:20:08.955130 pyntweb-0.2.8/webfalco/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      228 2023-07-21 15:15:13.000000 pyntweb-0.2.8/webfalco/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       24 2023-07-21 15:15:13.000000 pyntweb-0.2.8/webfalco/const.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5524 2023-07-21 15:15:13.000000 pyntweb-0.2.8/webfalco/lrparser.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    13667 2023-07-21 15:15:13.000000 pyntweb-0.2.8/webfalco/tran.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      467 2023-07-21 15:15:13.000000 pyntweb-0.2.8/webfalco/webfalcoc.py
```

### Comparing `pyntweb-0.2.7/LICENSE` & `pyntweb-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.7/PKG-INFO` & `pyntweb-0.2.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Metadata-Version: 2.1
 Name: pyntweb
-Version: 0.2.7
+Version: 0.2.8
 Summary: NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом кодеПосесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi
 Author-email: talismanchet@vk.com
 License: GNU GPL 3.0
 License-File: LICENSE
```

### Comparing `pyntweb-0.2.7/README.md` & `pyntweb-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.7/ntcss/ntml_parser.py` & `pyntweb-0.2.8/ntcss/ntml_parser.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.7/ntcss/tran.py` & `pyntweb-0.2.8/ntcss/tran.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.7/ntml/errors.py` & `pyntweb-0.2.8/ntml/errors.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.7/ntml/ntml_parser.py` & `pyntweb-0.2.8/ntml/ntml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
                      | Sexpr "*" Sexpr
                      | Sexpr "/" Sexpr
                      | Sexpr "+" Sexpr
                      | Sexpr "-" Sexpr
                      | "-" Sexpr
                      | Tstr
                      | Tfloat
-                     | Tint;
+                     | Tint
+                     | Tbool;
 
         Sbody: "{" ( Stag | Tcomment | Tname | Tescape | Tany | Tat )* "}";
 
 terminals
 
 Tstr: /"[^"\\]*(?:\\.[^"\\]*)*"/;
 Tcomment: /\/\*.*\*\//;
@@ -54,14 +55,15 @@
 Ttitle: "title";
 Tscript: /script\b\s*(?=\()/;
 Ttagname: /(?!script)\b[A-Za-zА-Яа-яЁё_]\w*\b\s*(?=(\(|\{))/;
 Tname: /\b[A-Za-zА-Яа-яЁё_-]\w*\b(?!(\(|\{))/;
 Tint: /0[xX](?:_?[0-9a-fA-F])+|0[bB](?:_?[01])+|0[oO](?:_?[0-7])+|(?:0(?:_?0)*|[1-9](?:_?\d)*)/;
 Tverfloat: /\d\.\d+(\.\d+)?/;
 Tfloat: /\d(?:_?\d)*\.(?:\d(?:_?\d)*)?/;
+Tbool: /(true|false)/;
 Tescape: /\[.{1,4}\]/;
 Tat: "@";
 Tbody: /\#\{[^\}\\]*(?:\[.[^\}\\]\]*)*\}/;
 Tany: /(\+|\;|\/|\/|\*|\`|\’|\:|\d|\?|\&|\~|\'|\"SUPPRESS_NEWLINW
 |\!|\-|\,|\.|\)|\]|<|>||\"|\=|\!|\@|\#|\||\$|\%|\^|\&|\*|\:|\/(?!\*)|\d|\b|\w(?!(\(|\{)))+/;
 
 """.replace("SUPPRESS_NEWLINE\n", "")
@@ -128,24 +130,27 @@
         return {}
 
     n = flat(n[1:][:-1])
     ret = {}
     marks = []
     ptr = 0
 
-    while ptr < len(n) and n[ptr] != "@":
-        if n[ptr]:
-            ret[n[ptr]] = n[ptr+2]
-            ptr += 4
-        else:
-            ptr += 1
+    
     try:
-        if n[ptr] == "@":
-            for i in n[ptr+1:]:
-                marks.append(eval(i))
+        while ptr < len(n):
+            if n[ptr] != "@":
+                if n[ptr]:
+                    ret[n[ptr]] = n[ptr+2]
+                    ptr += 4
+                else:
+                    ptr += 1
+            elif n[ptr] == "@":
+                marks.append(eval(n[ptr+1]))
+                ptr += 2
+
     except IndexError:
         pass
     
     return ret, marks
 
 
 def unescape(raw):
```

### Comparing `pyntweb-0.2.7/ntml/tran.py` & `pyntweb-0.2.8/ntml/tran.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.7/pyntweb.egg-info/PKG-INFO` & `pyntweb-0.2.8/pyntweb.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Metadata-Version: 2.1
 Name: pyntweb
-Version: 0.2.7
+Version: 0.2.8
 Summary: NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом кодеПосесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi
 Author-email: talismanchet@vk.com
 License: GNU GPL 3.0
 License-File: LICENSE
```

### Comparing `pyntweb-0.2.7/pyproject.toml` & `pyntweb-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyntweb"
-version = "0.2.7"
+version = "0.2.8"
 description = "NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же традиционные языки нативно поддерживаются в самом коде."
 authors = ["Talisman Chet <talismanchet@vk.com>"]
 license = "GNU GPL 3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyntweb-0.2.7/setup.py` & `pyntweb-0.2.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 setup.py
 """
 
 from setuptools import setup
 
 setup(name='pyntweb',
-      version='0.2.7',
+      version='0.2.8',
       description='''
 NTWeb - это экосистема компиляторов, которая планирует прийти на замену существующим в web стандартам: 
 HTML, CSS, JS. На данный момент код на её языках переводится в традиционные языки web, так же 
 традиционные языки нативно поддерживаются в самом коде
 
 Посесите оффициальную группу проекта: https://t.me/+ft6pYhYcqtk3NDdi'''.replace("\n", ""),
       packages=['ntml', 'webfalco', 'ntcss'],
```

### Comparing `pyntweb-0.2.7/webfalco/lrparser.py` & `pyntweb-0.2.8/webfalco/lrparser.py`

 * *Files identical despite different names*

### Comparing `pyntweb-0.2.7/webfalco/tran.py` & `pyntweb-0.2.8/webfalco/tran.py`

 * *Files identical despite different names*

