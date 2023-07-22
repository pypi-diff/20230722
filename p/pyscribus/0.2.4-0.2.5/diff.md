# Comparing `tmp/pyscribus-0.2.4.tar.gz` & `tmp/pyscribus-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscribus-0.2.4.tar", last modified: Thu Mar 16 17:32:39 2023, max compression
+gzip compressed data, was "pyscribus-0.2.5.tar", last modified: Sat Jul 22 20:09:30 2023, max compression
```

## Comparing `pyscribus-0.2.4.tar` & `pyscribus-0.2.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 17:32:39.470037 pyscribus-0.2.4/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    34494 2023-03-11 18:49:33.000000 pyscribus-0.2.4/LICENSE
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1342 2023-03-16 17:32:39.470037 pyscribus-0.2.4/PKG-INFO
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 17:32:39.434037 pyscribus-0.2.4/pyscribus/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      949 2023-03-16 17:27:19.000000 pyscribus-0.2.4/pyscribus/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    20868 2023-03-14 12:18:57.000000 pyscribus-0.2.4/pyscribus/colors.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 17:32:39.466037 pyscribus-0.2.4/pyscribus/common/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      930 2023-03-11 18:35:21.000000 pyscribus-0.2.4/pyscribus/common/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2632 2023-03-13 21:40:30.000000 pyscribus-0.2.4/pyscribus/common/math.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    13822 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/common/xml.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35340 2023-03-14 13:31:46.000000 pyscribus-0.2.4/pyscribus/dimensions.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    59347 2023-03-14 12:18:04.000000 pyscribus-0.2.4/pyscribus/document.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3648 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/exceptions.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 17:32:39.466037 pyscribus-0.2.4/pyscribus/extra/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      971 2023-03-11 18:35:21.000000 pyscribus-0.2.4/pyscribus/extra/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    14384 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/extra/wireframe.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 17:32:39.470037 pyscribus-0.2.4/pyscribus/headless/
--rwxrw-r--   0 etienne   (1000) etienne   (1000)     3506 2023-03-14 17:34:42.000000 pyscribus-0.2.4/pyscribus/headless/__init__.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 17:32:39.470037 pyscribus-0.2.4/pyscribus/headless/scripts/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-03-14 14:45:18.000000 pyscribus-0.2.4/pyscribus/headless/scripts/__init__.py
--rwxrw-r--   0 etienne   (1000) etienne   (1000)     1192 2023-03-14 17:29:00.000000 pyscribus-0.2.4/pyscribus/headless/scripts/topdf.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5178 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/itemattribute.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5591 2023-03-14 12:11:25.000000 pyscribus-0.2.4/pyscribus/layers.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1715 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/logs.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    10896 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/marks.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     8644 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/notes.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)   101244 2023-03-14 12:22:44.000000 pyscribus-0.2.4/pyscribus/pageobjects.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35269 2023-03-14 12:14:49.000000 pyscribus-0.2.4/pyscribus/pages.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 17:32:39.470037 pyscribus-0.2.4/pyscribus/papers/
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)      942 2023-03-11 18:35:23.000000 pyscribus-0.2.4/pyscribus/papers/__init__.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3783 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/papers/afnor.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2216 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/papers/ansi.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3259 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/papers/iso216.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1738 2023-03-11 18:35:23.000000 pyscribus-0.2.4/pyscribus/papers/iso217.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2347 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/papers/iso269.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1615 2023-03-12 15:40:15.000000 pyscribus-0.2.4/pyscribus/papers/newspaper.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5605 2023-03-14 12:19:26.000000 pyscribus-0.2.4/pyscribus/patterns.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    18730 2023-03-14 12:45:12.000000 pyscribus-0.2.4/pyscribus/printing.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     9827 2023-03-12 15:40:16.000000 pyscribus-0.2.4/pyscribus/sla.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    45290 2023-03-12 15:40:16.000000 pyscribus-0.2.4/pyscribus/stories.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)    57372 2023-03-14 12:26:14.000000 pyscribus-0.2.4/pyscribus/styles.py
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     7565 2023-03-12 15:40:16.000000 pyscribus-0.2.4/pyscribus/toc.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-03-16 17:32:39.434037 pyscribus-0.2.4/pyscribus.egg-info/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1342 2023-03-16 17:32:38.000000 pyscribus-0.2.4/pyscribus.egg-info/PKG-INFO
--rw-rw-r--   0 etienne   (1000) etienne   (1000)      990 2023-03-16 17:32:38.000000 pyscribus-0.2.4/pyscribus.egg-info/SOURCES.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-03-16 17:32:38.000000 pyscribus-0.2.4/pyscribus.egg-info/dependency_links.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       14 2023-03-16 17:32:38.000000 pyscribus-0.2.4/pyscribus.egg-info/requires.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       10 2023-03-16 17:32:38.000000 pyscribus-0.2.4/pyscribus.egg-info/top_level.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       38 2023-03-16 17:32:39.470037 pyscribus-0.2.4/setup.cfg
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1292 2023-03-16 17:27:12.000000 pyscribus-0.2.4/setup.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.166119 pyscribus-0.2.5/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    34494 2023-03-11 18:49:33.000000 pyscribus-0.2.5/LICENSE
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1519 2023-07-22 20:09:30.166119 pyscribus-0.2.5/PKG-INFO
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.158119 pyscribus-0.2.5/pyscribus/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      949 2023-07-22 20:02:37.000000 pyscribus-0.2.5/pyscribus/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    20868 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/colors.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/common/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      930 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/common/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2632 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/common/math.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    13845 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/common/xml.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35340 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/dimensions.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    61630 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/document.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3648 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/exceptions.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/extra/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      971 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/extra/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    14384 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/extra/wireframe.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/headless/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3506 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/headless/__init__.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/headless/scripts/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/headless/scripts/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1192 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/headless/scripts/topdf.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5178 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/itemattribute.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5591 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/layers.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1715 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/logs.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    10991 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/marks.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     8644 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/notes.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)   108431 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/pageobjects.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    35269 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/pages.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus/papers/
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)      942 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/__init__.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3783 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/afnor.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2216 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/ansi.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     3259 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/iso216.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1738 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/iso217.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     2347 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/iso269.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1615 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/papers/newspaper.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     5605 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/patterns.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    24054 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/printing.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     9877 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/sla.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    45306 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/stories.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)    59441 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/styles.py
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     7565 2023-07-22 19:47:56.000000 pyscribus-0.2.5/pyscribus/toc.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-22 20:09:30.162119 pyscribus-0.2.5/pyscribus.egg-info/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1519 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/PKG-INFO
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      990 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/SOURCES.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/dependency_links.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       14 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/requires.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       10 2023-07-22 20:09:30.000000 pyscribus-0.2.5/pyscribus.egg-info/top_level.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       38 2023-07-22 20:09:30.166119 pyscribus-0.2.5/setup.cfg
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)     1292 2023-07-22 20:02:37.000000 pyscribus-0.2.5/setup.py
```

### Comparing `pyscribus-0.2.4/LICENSE` & `pyscribus-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/__init__.py` & `pyscribus-0.2.5/pyscribus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,10 +20,10 @@
 """
 PyScribus
 """
 
 from pyscribus.sla import SLA
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-0.2.4/pyscribus/colors.py` & `pyscribus-0.2.5/pyscribus/colors.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/common/__init__.py` & `pyscribus-0.2.5/pyscribus/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/common/math.py` & `pyscribus-0.2.5/pyscribus/common/math.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/common/xml.py` & `pyscribus-0.2.5/pyscribus/common/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     "lower-roman": "Type_i_ii_iii",
     "upper-roman": "Type_I_II_III",
     "lower-latin": "Type_a_b_c",
     "upper-latin": "Type_A_B_C",
     "alpha-ar": "Type_Alphabet_ar",
     "abjad-ar": "Type_Abjad_ar",
     "hebrew": "Type_Hebrew",
+    # ASTERIX EST LA !
     "asterix": "Type_asterix",
     "cjk": "Type_CJK",
 }
 
 alignment = {
     "left": "0",
     "center": "1",
```

### Comparing `pyscribus-0.2.4/pyscribus/dimensions.py` & `pyscribus-0.2.5/pyscribus/dimensions.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/document.py` & `pyscribus-0.2.5/pyscribus/document.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 
 # Imports ===============================================================#
 
 # To avoid Sphinx complaints from methods annotations referencing same class
 from __future__ import annotations
 
-from typing import Union, NoReturn
+from typing import Union, NoReturn, Optional, Any, List
 
 import lxml
 import lxml.etree as ET
 
 import pyscribus.exceptions as exceptions
 
 from pyscribus.common.xml import *
@@ -50,15 +50,21 @@
 
 # Variables globales ====================================================#
 
 __author__ = "Etienne Nadji <etnadji@eml.cc>"
 
 BoolOrElement = Union[bool, ET.Element]
 
-AppendableToDocument = Union[pageobjects.PageObject, pages.PageAbstract, layers.Layer, pscolors.Color, styles.StyleAbstract]
+AppendableToDocument = Union[
+    pageobjects.PageObject,
+    pages.PageAbstract,
+    layers.Layer,
+    pscolors.Color,
+    styles.StyleAbstract,
+]
 
 # Classes ===============================================================#
 
 
 class Document(PyScribusElement):
     """
     SLA Document (DOCUMENT) in SLA file.
@@ -246,15 +252,15 @@
 
         self.autoframes = {
             # Number of Columns in automatic Textframes
             # AUTOSPALTEN = "1"
             "columns": 1,
             # Distance between Columns in automatic Textframes
             # ABSTSPALTEN = "11"
-            "colgap": dimensions.Dim(11, unit="pt")
+            "colgap": dimensions.Dim(11, unit="pt"),
         }
 
         # ----------------------------------------------
 
         # FIXME Not documented -------------------------
         # PRESET="0"
 
@@ -269,15 +275,15 @@
             "size": pages.xml_size["A4"],
             # (optional) Which PageSet to use
             # This value is the index of page set used. And it is NOT optional.
             # So by default,
             # 0 is Single page, 1 is Facing pages, 2 is 3-Fold, 3 is 4-Fold
             # BOOK = "0"
             # TODO : Link this value to pages sets in Document object
-            "set": 0
+            "set": 0,
         }
 
         # (optional) First page number in the Doc
         FIRSTNUM = "1"
 
         # (optional) Measurement unit for the Doc
         # 0 = Points 1 = Millimeters 2 = Inches 3 = Picas
@@ -580,15 +586,15 @@
         """
 
         self.page_sets = []
 
         for default in ["Single Page", "Facing Pages", "3-Fold", "4-Fold"]:
             ps = pages.PageSet()
 
-            if (success := ps.fromdefault(default)) :
+            if (success := ps.fromdefault(default)):
                 self.page_sets.append(ps)
 
     def _default_colors(self) -> NoReturn:
         """
         Set default colors.
         """
 
@@ -648,15 +654,15 @@
 
     def _default_character_styles(self) -> NoReturn:
         self.styles["character"].append(
             styles.CharacterStyle(self, default=True)
         )
         self.styles["character"][-1].is_default = True
 
-    def fromdefault(self, default: str="all") -> NoReturn:
+    def fromdefault(self, default: str = "all") -> NoReturn:
         """
         Set default settings from a default list
 
         :param default: Set of default settings or list of default features
             to set.
         :type default: str,list
 
@@ -743,36 +749,50 @@
     # =======================================================================
 
     def fromxml(self, xml: ET.Element) -> bool:
         # --- DOCUMENT attributes ----------------------------------------
 
         # TODO DOCUMENT many attribs…
 
+        for border in ["LEFT", "RIGHT", "TOP", "BOTTM"]:
+            if (border_side := xml.get(f"BORDER{border}")) is not None:
+                self.borders[border.lower()].value = float(border_side)
+
         # Pages settings
 
+        if (pagenumber := xml.get("ANZPAGES")) is not None:
+            self.page_number = int(pagenumber)
+
         if (att_value := xml.get("orientation")) is not None:
             if int(att_value):
                 self.doc_pages["orientation"] = pages.Orientation.LANDSCAPE
             else:
                 self.doc_pages["orientation"] = pages.Orientation.PORTRAIT
 
         if (att_value := xml.get("PAGESIZE")) is not None:
             for att, human in pages.xml_size.items():
                 if att_value == att:
                     self.doc_pages["size"] = pages.xml_size[att_value]
                     break
 
+        for page_dim in ["WIDTH", "HEIGHT"]:
+            if (pgdim := xml.get(f"PAGE{page_dim}")) is not None:
+                self.dims[page_dim.lower()].value = float(pgdim)
+
         if (att_value := xml.get("BOOK")) is not None:
             self.doc_pages["set"] = int(att_value)
 
         # Metadatas
 
         for att, key in Document.metadata_xml.items():
-            if (v := xml.get(att)) is not None:
-                self.metadata[key] = v
+            if (meta_value := xml.get(att)) is not None:
+                self.metadata[key] = meta_value
+
+        if (keywords := xml.get("KEYWORDS")) is not None:
+            self.metadata["keywords"] = keywords.split("; ")
 
         # Auto text frames
 
         for att, human in Document.autoframes_xml.items():
             if (att_value := xml.get(att)) is not None:
                 if human == "colums":
                     self.autoframes[human] = int(att_value)
@@ -797,509 +817,521 @@
 
         for att_name, ui_name in Document.ui_show_xml.items():
             if (att := xml.get(att_name)) is not None:
                 self.ui_show[ui_name] = num_to_bool(att)
 
         # ICC color profiles
 
-        for case in [
+        for att_name, icc_key in [
             ["DPIn", "rgb_images"],
             ["DPInCMYK", "cmyk_images"],
             ["DPIn2", "rgb_colors"],
             ["DPIn3", "cmyk_colors"],
             ["DPPr", "printer"],
         ]:
-            att_name, icc_key = case
-
             if (att := xml.get(att_name)) is not None:
                 self.icc_profiles[icc_key] = att
 
-        # Calligraphic pen
+        # Calligraphic pen -----------------------------------------------
 
-        for case in [
+        for att_base, key in [
             ["Angle", "angle"],
             ["LineColorShade", "line_shade"],
             ["FillColorShade", "fill_shade"],
         ]:
-            att_name = "calligraphicPen{}".format(case[0])
+            att_name = f"calligraphicPen{att_base}"
 
             if (att := xml.get(att_name)) is not None:
-                self.calligraphicpen[case[1]].value = int(att)
+                self.calligraphicpen[key].value = int(att)
 
-        for case in [["LineWidth", "line_width"], ["Width", "width"]]:
-            att_name = "calligraphicPen{}".format(case[0])
+        for att_base, key in [["LineWidth", "line_width"], ["Width", "width"]]:
+            att_name = f"calligraphicPen{att_base}"
 
             if (att := xml.get(att_name)) is not None:
-                self.calligraphicpen[case[1]].value = float(att)
+                self.calligraphicpen[key].value = float(att)
 
-        for case in [
+        for att_base, key in [
             ["LineColor", "line_color"],
             ["FillColor", "fill_color"],
             ["PenStyle", "style"],
         ]:
 
-            att_name = "calligraphicPen{}".format(case[0])
+            att_name = f"calligraphicPen{att_base}"
 
             if (att := xml.get(att_name)) is not None:
-                self.calligraphicpen[case[1]] = att
+                self.calligraphicpen[key] = att
 
         # --- DOCUMENT childs --------------------------------------------
 
         for child in xml:
 
-            if child.tag == "CheckProfile":
-                p = Profile()
-
-                if (success := p.fromxml(child)) :
-                    self.profiles.append(p)
-
-            if child.tag == "Gradient":
-                gr = pscolors.Gradient()
-
-                if (success := gr.fromxml(child)) :
-                    self.gradients.append(gr)
+            self.__fromxml_item(child, "CheckProfile", Profile, self.profiles)
 
-            if child.tag == "COLOR":
-                c = pscolors.Color()
-
-                if (success := c.fromxml(child)) :
-                    self.colors.append(c)
+            self.__fromxml_item(
+                child, "Gradient", pscolors.Gradient, self.gradients
+            )
 
-            if child.tag == "Pattern":
-                patt = patterns.Pattern()
+            self.__fromxml_item(child, "COLOR", pscolors.Color, self.colors)
 
-                if (success := patt.fromxml(child)) :
-                    self.patterns.append(patt)
+            self.__fromxml_item(
+                child, "Pattern", patterns.Pattern, self.patterns
+            )
 
             # TODO FIXME hyphen
 
-            if child.tag in ["STYLE", "CHARSTYLE"]:
-
-                if child.tag == "STYLE":
-                    key, xstyle = "paragraph", styles.ParagraphStyle(self)
-
-                if child.tag == "CHARSTYLE":
-                    key, xstyle = "character", styles.CharacterStyle(self)
-
-                if (success := xstyle.fromxml(child)) :
-                    self.styles[key].append(xstyle)
-
-            if child.tag == "TableStyle":
-                tstyle = styles.TableStyle(self)
-
-                if (success := tstyle.fromxml(child)) :
-                    self.styles["table"].append(tstyle)
-
-            if child.tag == "CellStyle":
-                cstyle = styles.CellStyle(self)
-
-                if (success := cstyle.fromxml(child)) :
-                    self.styles["cell"].append(cstyle)
-
-            if child.tag == "LAYERS":
-                lobj = layers.Layer()
-
-                if (success := lobj.fromxml(child)) :
-                    self.layers.append(lobj)
+            self.__fromxml_item(
+                child, "STYLE", styles.ParagraphStyle, self.styles["paragraph"],
+                True
+            )
 
-            if child.tag == "Printer":
+            self.__fromxml_item(
+                child, "CHARSTYLE", styles.CharacterStyle,
+                self.styles["character"], True
+            )
 
-                ps = printing.PrinterSettings()
+            self.__fromxml_item(
+                child, "TableStyle", styles.TableStyle, self.styles["table"],
+                True
+            )
 
-                if (success := ps.fromxml(child)) :
-                    self.printer_settings.append(ps)
+            self.__fromxml_item(
+                child, "CellStyle", styles.CellStyle, self.styles["cell"], True
+            )
 
-            if child.tag == "PDF":
+            self.__fromxml_item(
+                child, "LAYERS", layers.Layer, self.layers, True
+            )
 
-                pds = printing.PDFSettings()
+            self.__fromxml_item(
+                child, "Printer", printing.PrinterSettings,
+                self.printer_settings
+            )
 
-                if (success := pds.fromxml(child)) :
-                    self.pdf_settings.append(pds)
+            self.__fromxml_item(
+                child, "PDF", printing.PDFSettings, self.pdf_settings
+            )
 
             if child.tag == "DocItemAttributes":
 
                 for attribute in child:
-                    da = itemattribute.DocumentAttribute()
-
-                    if (success := da.fromxml(attribute)) :
-                        self.attributes.append(da)
-
-            if child.tag == "TablesOfContents":
-
-                for sub in child:
+                    doc_att_item = itemattribute.DocumentAttribute()
 
-                    if sub.tag == "TableOfContents":
-                        toc_settings = toc.TOC()
+                    if (success := doc_att_item.fromxml(attribute)):
+                        self.attributes.append(doc_att_item)
 
-                        if (success := toc_settings.fromxml(sub)) :
-                            self.tocs.append(toc_settings)
-
-            if child.tag == "Marks":
-
-                for sub in child:
-
-                    if sub.tag == "Mark":
-                        mx = marks.DocumentMark()
-
-                        if (success := mx.fromxml(sub)) :
-                            self.marks.append(mx)
-
-            if child.tag == "NotesStyles":
-
-                for sub in child:
+            self.__fromxml_section(
+                child,
+                "TablesOfContents",
+                "TableOfContents",
+                toc.TOC,
+                self.tocs,
+            )
 
-                    if sub.tag == "notesStyle":
-                        s = styles.NoteStyle()
+            self.__fromxml_section(
+                child,
+                "Marks",
+                "Mark",
+                marks.DocumentMark,
+                self.marks,
+            )
 
-                        if (success := s.fromxml(sub)) :
-                            self.styles["note"].append(s)
+            self.__fromxml_section(
+                child,
+                "NotesStyles",
+                "notesStyle",
+                styles.NoteStyle,
+                self.styles["note"],
+            )
 
             if child.tag == "NotesFrames":
 
                 for sub in child:
 
                     if sub.tag == "FOOTNOTEFRAME":
-                        nf = notes.NoteFrame()
-
-                        if (success := nf.fromxml(sub)) :
-                            self.notes_frames.append(nf)
-
-            if child.tag == "Notes":
-
-                for sub in child:
+                        note_frame = notes.NoteFrame()
 
-                    if sub.tag == "Note":
-                        nc = notes.Note()
-                        nc.doc_parent = self
+                        if (success := note_frame.fromxml(sub)):
+                            self.notes_frames.append(note_frame)
 
-                        if (success := nc.fromxml(sub)) :
-                            self.notes.append(nc)
+            self.__fromxml_section(
+                child,
+                "Notes",
+                "Note",
+                notes.Note,
+                self.notes,
+                True
+            )
 
             if child.tag == "PageSets":
 
                 for page_set in child:
-                    ps = pages.PageSet()
-
-                    if (success := ps.fromxml(page_set)) :
-                        self.page_sets.append(ps)
-
-            if child.tag == "Sections":
-
-                for sub in child:
-
-                    if sub.tag == "Section":
-                        sec = toc.Section()
+                    page_set_item = pages.PageSet()
 
-                        if (success := sec.fromxml(sub)) :
-                            self.sections.append(sec)
+                    if (success := page_set_item.fromxml(page_set)):
+                        self.page_sets.append(page_set_item)
 
-            if child.tag == "MASTERPAGE":
-                m = pages.MasterPage()
+            self.__fromxml_section(
+                child,
+                "Sections",
+                "Section",
+                toc.Section,
+                self.sections,
+            )
 
-                if (success := m.fromxml(child)) :
-                    self.master_pages.append(m)
+            self.__fromxml_item(
+                child, "MASTERPAGE", pages.MasterPage, self.master_pages, False
+            )
 
             if child.tag == "PAGE":
-                p = pages.Page()
+                page_item = pages.Page()
 
-                p.sla_parent = self.sla_parent
-                p.doc_parent = self
+                page_item.sla_parent = self.sla_parent
+                page_item.doc_parent = self
 
-                if (success := p.fromxml(child)) :
-                    self.pages.append(p)
+                if (success := page_item.fromxml(child)):
+                    self.pages.append(page_item)
 
             if child.tag == "PAGEOBJECT":
                 ptype = child.get("PTYPE")
 
-                if ptype is not None:
+                if ptype is None:
+                    continue
 
-                    try:
-                        po = pageobjects.new_from_type(
+                try:
+                    p_object = pageobjects.new_from_type(
                             ptype, self.sla_parent, self
-                        )
+                    )
 
-                        if (success := po.fromxml(child)) :
-                            self.page_objects.append(po)
+                    if (success := p_object.fromxml(child)):
+                        self.page_objects.append(p_object)
 
-                    except ValueError:
-                        pass
+                except ValueError:
+                    pass
 
         # ----------------------------------------------------------------
 
         return True
 
     def toxml(self, optional: bool = True) -> ET.Element:
         xml = ET.Element("DOCUMENT")
 
-        # --- DOCUMENT attributes ----------------------------------------
+        # === DOCUMENT attributes ========================================
 
-        # TODO DOCUMENT many attribs…
+        # Pages settings -------------------------------------------------
 
-        # Pages settings
+        xml.attrib["ANZPAGES"] = str(self.page_number)
 
         xml.attrib["ORIENTATION"] = str(int(self.doc_pages["orientation"]))
 
         for att, human in pages.xml_size.items():
             if human == self.doc_pages["size"]:
                 xml.attrib["PAGESIZE"] = att
                 break
 
         xml.attrib["BOOK"] = str(self.doc_pages["set"])
 
-        # Auto text frames
+        # Auto text frames -----------------------------------------------
 
         for att, human in Document.autoframes_xml.items():
 
             if human == "columns":
                 xml.attrib[att] = str(self.autoframes[human])
 
             if human == "colgap":
                 xml.attrib[att] = self.autoframes[human].toxmlstr(True)
 
-        # Bleed settings
+        # Bleed settings -------------------------------------------------
 
         for att, human in Document.bleed_xml.items():
             xml.attrib[att] = str(self.bleed[human])
 
-        xml.attrib["ANZPAGES"] = str(self.page_number)
-
-        # Dimensions
+        # Dimensions -----------------------------------------------------
 
         xml.attrib["PAGEWIDTH"] = self.dims["width"].toxmlstr()
         xml.attrib["PAGEHEIGHT"] = self.dims["height"].toxmlstr()
 
-        # Borders
+        # Borders --------------------------------------------------------
 
-        for b in self.borders.keys():
-            att = "BORDER{}".format(b.upper())
-            xml.attrib[att] = self.borders[b].toxmlstr()
+        for border_side, border_value in self.borders.items():
+            att = "BORDER{}".format(border_side.upper())
+            xml.attrib[att] = border_value.toxmlstr()
 
-        # Metadatas
+        # Metadatas ------------------------------------------------------
 
         for att, key in Document.metadata_xml.items():
             xml.attrib[att] = self.metadata[key]
 
         xml.attrib["KEYWORDS"] = "; ".join(self.metadata["keywords"])
 
-        # UI snapping
-
-        for k, v in self.ui_snapping.items():
-            att = "SnapTo{}".format(k.capitalize())
+        # UI snapping ----------------------------------------------------
 
-            xml.attrib[att] = bool_to_num(v)
+        for att_base, snap_value in self.ui_snapping.items():
+            att = "SnapTo{}".format(att_base.capitalize())
+            xml.attrib[att] = bool_to_num(snap_value)
 
-        # UI show
+        # UI show --------------------------------------------------------
 
         for att_name, ui_name in Document.ui_show_xml.items():
             xml.attrib[att_name] = bool_to_num(self.ui_show[ui_name])
 
-        # ICC profiles
+        # ICC profiles ---------------------------------------------------
 
         for key_out, key_in in [
             ["DPIn", "rgb_images"],
             ["DPInCMYK", "cmyk_images"],
             ["DPIn2", "rgb_colors"],
             ["DPIn3", "cmyk_colors"],
             ["DPPr", "printer"],
         ]:
             xml.attrib[key_out] = self.icc_profiles[key_in]
 
-        # Calligraphic pen
-        # -------------------------------------------------
+        # Calligraphic pen -----------------------------------------------
 
         for key_out_suffix, key_in, as_string in [
             ["Angle", "angle", True],
             ["LineWidth", "line_width", True],
             ["LineColorShade", "line_shade", True],
             ["LineColor", "line_color", False],
             ["Width", "width", True],
             ["Style", "style", False],
             ["FillColor", "fill_color", False],
             ["FillColorShade", "fill_shade", True],
         ]:
 
-            att_name = "calligraphicPen{}".format(key_out_suffix)
+            att_name = f"calligraphicPen{key_out_suffix}"
             att_value = self.calligraphicpen[key_in]
 
             if as_string:
                 att_value = att_value.toxmlstr()
 
             if key_out_suffix == "Style":
                 att_value = str(att_value)
 
             xml.attrib[att_name] = att_value
 
-        # --- DOCUMENT childs --------------------------------------------
+        # === DOCUMENT childs ============================================
 
-        # Checking profiles -------------------------------
+        # Checking profiles ----------------------------------------------
 
         for profile in self.profiles:
-            px = profile.toxml()
-
-            if not isinstance(px, bool):
-                xml.append(px)
-
-        # Colors ------------------------------------------
-
-        for color in self.colors:
-            cx = color.toxml()
-            xml.append(cx)
+            profile_xml = profile.toxml()
 
-        # TODO hyphen
+            if not isinstance(profile_xml, bool):
+                xml.append(profile_xml)
 
-        # Styles ------------------------------------------
+        # ----------------------------------------------------------------
 
-        for pstyle in self.styles["paragraph"]:
-            pstylex = pstyle.toxml()
-            xml.append(pstylex)
+        # Colors
+        xml = self.__toxml_items(xml, self.colors)
 
-        for cstyle in self.styles["character"]:
-            cstylex = cstyle.toxml()
-            xml.append(cstylex)
+        # TODO FIXME hyphen
 
-        for tstyle in self.styles["table"]:
-            tstylex = tstyle.toxml()
-            xml.append(tstylex)
+        # Styles ---------------------------------------------------------
 
-        for cstyle in self.styles["cell"]:
-            cstylex = cstyle.toxml()
-            xml.append(cstylex)
+        for style_type in ["paragraph", "character", "table", "cell"]:
 
-        # Layers ------------------------------------------
+            for style_item in self.styles[style_type]:
+                item_xml = style_item.toxml()
+                xml.append(item_xml)
 
-        for layer in self.layers:
-            layerx = layer.toxml()
-            xml.append(layerx)
+        # ----------------------------------------------------------------
 
-        # Printer settings --------------------------------
+        # Layers
+        xml = self.__toxml_items(xml, self.layers)
 
-        for ps in self.printer_settings:
-            px = ps.toxml()
-            xml.append(px)
+        # Printer settings
+        xml = self.__toxml_items(xml, self.printer_settings)
 
-        # PDF settings ------------------------------------
+        # PDF settings
+        xml = self.__toxml_items(xml, self.pdf_settings)
 
-        for pds in self.pdf_settings:
-            px = pds.toxml()
-            xml.append(px)
+        # Document attributes
+        xml = self.__toxml_section(xml, "DocItemAttributes", self.attributes)
 
-        # Document attributes -----------------------------
+        # Tables of contents
+        xml = self.__toxml_section(xml, "TablesOfContents", self.tocs)
 
-        doca = ET.Element("DocItemAttributes")
+        # Marks
+        if self.marks:
+            xml = self.__toxml_section(xml, "Marks", self.marks)
 
-        for attribute in self.attributes:
-            ax = attribute.toxml()
-            doca.append(ax)
+        # Notes : styles, frames, content --------------------------------
 
-        xml.append(doca)
+        # Notes styles
+        xml = self.__toxml_section(xml, "NotesStyles", self.styles["note"])
 
-        # Tables of contents ------------------------------
+        # Notes frames
+        if self.notes_frames:
+            xml = self.__toxml_section(xml, "NotesFrames", self.notes_frames)
 
-        tocx = ET.Element("TablesOfContents")
+        # Notes content
 
-        for tocobj in self.tocs:
-            tx = tocobj.toxml()
-            tocx.append(tx)
+        if self.notes:
+            nx = ET.Element("Notes")
 
-        xml.append(tocx)
+            for note in self.notes:
+                # n = note.toxml()
+                # nx.append(n)
+                pass
 
-        # Marks -------------------------------------------
+            xml.append(nx)
 
-        if self.marks:
+        # ----------------------------------------------------------------
 
-            marksx = ET.Element("Marks")
+        # Page sets
+        xml = self.__toxml_section(xml, "PageSets", self.page_sets)
+        # Sections
+        xml = self.__toxml_section(xml, "Sections", self.sections)
 
-            for m in self.marks:
-                mx = m.toxml()
-                marksx.append(mx)
+        # Pages (master, regular) ----------------------------------------
 
-            xml.append(marksx)
+        # Master pages
+        xml = self.__toxml_items(xml, self.master_pages)
+        # Pages
+        xml = self.__toxml_items(xml, self.pages)
 
-        # Notes : styles, frames, notes content -----------
+        # Pages objects --------------------------------------------------
 
-        # Notes styles -------------------------------
+        xml = self.__toxml_items(xml, self.page_objects)
 
-        nsx = ET.Element("NotesStyles")
+        # ----------------------------------------------------------------
 
-        for note_style in self.styles["note"]:
-            nx = note_style.toxml()
-            nsx.append(nx)
+        return xml
 
-        xml.append(nsx)
+    def __fromxml_item(
+        self,
+        xml: ET.Element,
+        item_tag: str,
+        object_class,
+        attribute,
+        parent: bool = False
+    ):
+        if xml.tag != item_tag:
+            return
 
-        # Notes frames -------------------------------
+        if parent:
+            item_object = object_class(self)
+        else:
+            item_object = object_class()
 
-        if self.notes_frames:
+        if (success := item_object.fromxml(xml)):
+            attribute.append(item_object)
 
-            nfx = ET.Element("NotesFrames")
+    def __fromxml_section(
+        self,
+        xml,
+        section_tag: str,
+        item_tag: str,
+        object_class,
+        attribute,
+        parent: bool = False
+    ):
+        if xml.tag != section_tag:
+            return
 
-            for note_frame in self.notes_frames:
-                n = note_frame.toxml()
-                nfx.append(n)
+        for element in xml:
 
-            xml.append(nfx)
+            if element.tag != item_tag:
+                continue
 
-        # Notes content ------------------------------
+            if parent:
+                item_object = object_class(self)
+            else:
+                item_object = object_class()
 
-        if self.notes:
+            if (success := item_object.fromxml(element)):
+                attribute.append(item_object)
 
-            nx = ET.Element("Notes")
+    def __toxml_items(self, xml: ET.Element, items: list) -> ET.Element:
+        """
+        Add children nodes from `toxml()` methods of items to node `xml`.
 
-            for note in self.notes:
-                # n = note.toxml()
-                # nx.append(n)
-                pass
+        :type xml: ET.Element
+        :type items: list
+        :rtype: ET.Element
+        """
 
-            xml.append(nx)
+        for item in items:
+            item_xml = item.toxml()
+            xml.append(item_xml)
 
-        # Page sets ---------------------------------------
+        return xml
 
-        pssx = ET.Element("PageSets")
+    def __toxml_section(
+        self,
+        xml: ET.Element,
+        section_tag: str,
+        section_items: list
+    ) -> ET.Element:
+        """
+        Add a node with tag `section_tag` containing the XML representation
+        of `sections_items` (accessed through `toxml()` methods) as children,
+        to node `xml`.
+
+        :type xml: ET.Element
+        :type section_tag: str
+        :type section_items: list
+        :rtype: ET.Element
+        """
+
+        section = ET.Element(section_tag)
+
+        for item in section_items:
+            item_xml = item.toxml()
+            section.append(item_xml)
 
-        for page_set in self.page_sets:
-            px = page_set.toxml()
-            pssx.append(px)
+        xml.append(section)
 
-        xml.append(pssx)
+        return xml
 
-        # Sections ----------------------------------------
+    # =======================================================================
 
-        secx = ET.Element("Sections")
+    def style(
+        self,
+        name: Optional[str] = None,
+        style_type: Optional[str] = None,
+        default: bool = False,
+    ) -> Union[List[styles.StyleAbstract], styles.StyleAbstract]:
 
-        for section in self.sections:
-            sx = section.toxml()
-            secx.append(sx)
+        result = []
+        style_types = list(self.styles.keys())
 
-        xml.append(secx)
+        if style_type is not None:
+            if style_type in style_types:
+                style_types = [style_type]
 
-        # Master pages ------------------------------------
+        for type_key in style_types:
 
-        for master in self.master_pages:
-            mx = master.toxml()
-            xml.append(mx)
+            for style in self.styles[type_key]:
 
-        # Pages -------------------------------------------
+                if name is None and style_type is not None:
 
-        for page in self.pages:
-            p = page.toxml()
-            xml.append(p)
+                    # Returns only default style of type X
+                    if default and style.is_default:
+                        return style
 
-        # Pages objects -----------------------------------
+                    # Returns all types of type X
+                    result.append(style)
+                    continue
 
-        for po in self.page_objects:
-            px = po.toxml()
-            xml.append(px)
+                # Request for default style not satisfactory
+                if default and not style.is_default:
+                    continue
 
-        # ----------------------------------------------------------------
+                # Request for style name not satisfactory
+                if name != style.name:
+                    continue
 
-        return xml
+                result.append(style)
 
-    # =======================================================================
+        return result
 
-    def pageobjects(self, object_type=False, templatable: bool = False) -> list:
+    def pageobjects(
+        self, object_type=False, templatable: bool = False
+    ) -> list:
         """
         Return document page objets.
 
         :type object_type: string,bool
         :param object_type: Page object type to filter, or do not filter at
             all. See pageobjects.po_type_classes for valid values.
         :type templatable: bool
@@ -1707,38 +1739,54 @@
         .. sealso: set_checks()
         """
         self.set_checks(checks, value)
 
     # PyScribus standard methods -------------------------------
 
     def toxml(self) -> BoolOrElement:
-        if self.checks:
-            xml = ET.Element("CheckProfile")
-            xml.attrib["Name"] = self.name
-            xml.attrib["autoCheck"] = bool_to_num(self.checks["auto"])
-
-            for check in self.checks.keys():
-                if check != "auto":
-                    xml.attrib["check{}".format(check)] = bool_to_num(
-                        self.checks[check]
-                    )
+        if not self.checks:
+            return False
 
-            for ignore in self.ignores.keys():
-                xml.attrib["ignore{}".format(ignore)] = bool_to_num(
-                    self.ignores[ignore]
-                )
-
-            for res in self.resolution.keys():
-                xml.attrib["{}Resolution".format(res)] = self.resolution[
-                    res
-                ].toxmlstr()
+        xml = ET.Element("CheckProfile")
+        xml.attrib["Name"] = self.name
 
-            return xml
+        xml.attrib["ignoreErrors"] = bool_to_num(self.ignores["Errors"])
 
-        return False
+        xml.attrib["autoCheck"] = bool_to_num(self.checks["auto"])
+
+        for check in [
+            "Glyphs",
+            "Orphans",
+            "Overflow",
+            "Pictures",
+            "PartFilledImageFrames",
+            "Resolution",
+            "Transparency",
+        ]:
+            xml.attrib[f"check{check}"] = bool_to_num(self.checks[check])
+
+        for res in self.resolution.keys():
+            xml.attrib[f"{res}Resolution"] = self.resolution[res].toxmlstr()
+
+        for check in ["Annotations", "RasterPDF", "ForGIF"]:
+            xml.attrib[f"check{check}"] = bool_to_num(self.checks[check])
+
+        xml.attrib["ignoreOffLayers"] = bool_to_num(self.ignores["OffLayers"])
+
+        for check in [
+            "NotCMYKOrSpot",
+            "DeviceColorsAndOutputIntent",
+            "FontNotEmbedded",
+            "FontIsOpenType",
+            "AppliedMasterDifferentSide",
+            "EmptyTextFrames",
+        ]:
+            xml.attrib[f"check{check}"] = bool_to_num(self.checks[check])
+
+        return xml
 
     def fromxml(self, xml: ET.Element) -> bool:
         name = xml.get("Name")
 
         if name is not None:
             self.name = name
 
@@ -1764,16 +1812,15 @@
 
             if value is not None:
                 self.resolution[res].value = int(value)
 
         return True
 
     def fromdefault(self, name: str) -> bool:
-        """
-        """
+        """ """
 
         if name not in self.pyscribus_defaults:
             return False
 
         self.name = name
 
         if name in [
@@ -1983,8 +2030,9 @@
                     "checkFontNotEmbedded",
                     "checkFontIsOpenType",
                 ]
             )
 
         return True
 
+
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-0.2.4/pyscribus/exceptions.py` & `pyscribus-0.2.5/pyscribus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/extra/__init__.py` & `pyscribus-0.2.5/pyscribus/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/extra/wireframe.py` & `pyscribus-0.2.5/pyscribus/extra/wireframe.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/headless/__init__.py` & `pyscribus-0.2.5/pyscribus/headless/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/headless/scripts/topdf.py` & `pyscribus-0.2.5/pyscribus/headless/scripts/topdf.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/itemattribute.py` & `pyscribus-0.2.5/pyscribus/itemattribute.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/layers.py` & `pyscribus-0.2.5/pyscribus/layers.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/logs.py` & `pyscribus-0.2.5/pyscribus/logs.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/marks.py` & `pyscribus-0.2.5/pyscribus/marks.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     .. seealso:: :class:`pyscribus.stories.StoryNoteMark`
     """
 
     def __init__(
         self,
         mark_type: MarkType,
         label: str = "",
-        features: Optional[str] = False,
+        features: Optional[dict] = False,
     ):
         super().__init__()
 
         self.features = {
             "inherit": False,
             "superscript": False,
         }
@@ -296,24 +296,32 @@
 
 
 class StoryNoteMark(StoryMarkAbstract):
     """
     Mark (MARK) for a (foot|end)note in Scribus stories.
     """
 
-    def __init__(self, label: str = "", features: Optional[str] = False):
+    def __init__(
+        self,
+        label: str = "",
+        features: Optional[dict] = False,
+        default: bool = False
+    ):
         StoryMarkAbstract.__init__(self, "note", label, features)
 
+        if default:
+            self.fromdefault()
+
     def fromdefault(self) -> NoReturn:
         self.set_features("inherit superscript")
 
     def __repr__(self):
         return "NOTEMARK|{}|{}".format(
             self.label,
-            [k for k, v in self.features.items() if self.features[k]],
+            [k for k in self.features if bool(k)],
         )
 
 
 class StoryVariableMark(StoryMarkAbstract):
     """
     Variable text mark
     """
```

### Comparing `pyscribus-0.2.4/pyscribus/notes.py` & `pyscribus-0.2.5/pyscribus/notes.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/pageobjects.py` & `pyscribus-0.2.5/pyscribus/pageobjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,21 @@
     line_join_xml = {"miter": "0", "bevel": "64", "round": "128"}
 
     image_scaling_type_xml = {
         "free": "0",
         "frame": "1",
     }
 
+    text_flow_xml = {
+        None: False,
+        "1": "shape",
+        "2": "rectangle",
+        "3": "outline"
+    }
+
     shape_type_xml = {
         "rectangle": "0",
         "ellipse": "1",
         "rounded-rectangle": "2",
         "free": "3",
     }
 
@@ -134,14 +141,16 @@
         # --- Page object shape and boxes ----------------------------
 
         self.box = dimensions.DimBox()
         self.rotated_box = dimensions.DimBox()
         self.rotated = False
         self.shape = {"type": None, "edited": None}
 
+        self.opacity = dimensions.Dim(float(1), unit="pcdecim")
+
         # Image frame in image object defined there because Scribus
         # does it.
 
         self.image_box = dimensions.LocalDimBox()
         self.image_rotated_box = dimensions.DimBox()
 
         self.image_scale = {
@@ -182,14 +191,15 @@
             "endcap": None,
         }
 
         # --- Page object paths --------------------------------------
 
         self.path = None
         self.copath = None
+        self.path_options = {}
 
         # --- --------------------------------------------------------
 
         if ptype and ptype in po_type_xml.keys():
             self.ptype = ptype
         else:
             self.ptype = None
@@ -383,29 +393,28 @@
         # --- Layer of the page object -------------------------------
 
         if (layer := xml.get("LAYER")) is not None:
 
             try:
                 layer = int(layer)
 
-                if self.doc_parent:
+                if self.doc_parent and self.doc_parent.layers:
 
-                    if self.doc_parent.layers:
+                    layer_found = False
 
-                        layer_found = False
+                    for doc_layer in self.doc_parent.layers:
+                        if layer != doc_layer.level:
+                            continue
 
-                        for doc_layer in self.doc_parent.layers:
-
-                            if layer == doc_layer.level:
-                                self.layer = layer
-                                layer_found = True
-                                break
+                        self.layer = layer
+                        layer_found = True
+                        break
 
-                        if not layer_found:
-                            raise exceptions.UnknownLayer(layer)
+                    if not layer_found:
+                        raise exceptions.UnknownLayer(layer)
 
             except TypeError:
                 raise exceptions.InsaneSLAValue(
                     "PageObject @LAYER value should be an integer."
                 )
 
         # --- Type specific attributes -------------------------------
@@ -528,14 +537,45 @@
         # --- Symbol attributes --------------------------------------
 
         if self.ptype == "symbol":
 
             if (pattern := xml.get("pattern")) is not None:
                 self.pattern = pattern
 
+        # --- Flow ---------------------------------------------------
+
+        if self.ptype in ["polyline", "polygon", "text"]:
+            # No text flow applied = no attribute TEXTFLOWMODE
+            text_flow_mode = xml.get("TEXTFLOWMODE")
+
+            try:
+                self.text_flow = PageObject.text_flow_xml[text_flow_mode]
+            except KeyError:
+                self.text_flow = PageObject.text_flow_xml[None]
+
+        # --- Text on path : show path -------------------------------
+
+        if self.ptype in ["textonpath", "text"]:
+            self.path_options["text_on_path"] = {
+                "show": False,
+                "offset": dimensions.Dim(0)
+            }
+
+            if (showtextpath := xml.get("PLTSHOW")) is not None:
+                self.path_options["text_on_path"]["show"] = xmlc.num_to_bool(showtextpath)
+
+            # BASEOF : Offset for the text from its path for text on a path
+            if (textpathoffset := xml.get("BASEOF")) is not None:
+                self.path_options["text_on_path"]["offset"].value = float(textpathoffset)
+
+        # --- Opacity of the object ----------------------------------
+
+        if (opacity := xml.get("TransValue")) is not None:
+            self.opacity.value = float(opacity)
+
         # --- Page objects specific children -------------------------
         # Moved in TableObject
         # Moved in TableObject
         # Moved in TableObject
         # NOTE No childs in image object
 
         # FIXME This records undocumented attributes -----------------
@@ -603,14 +643,19 @@
 
         # Page object type
         xml.attrib["PTYPE"] = str(po_type_xml[self.ptype])
 
         # Layer
         xml.attrib["LAYER"] = str(self.layer)
 
+        # --- Opacity of the object ----------------------------------
+
+        if self.opacity.value <= float(1):
+            xml.attrib["TransValue"] = self.opacity.toxmlstr(True)
+
         # ------------------------------------------------------------
 
         if self.shape["type"] is None:
             # If the shape type is not defined, we assume the frame has
             # a rectangular shape, as it is the most common
             xml.attrib["FRTYPE"] = PageObject.shape_type_xml["rectangle"]
         else:
@@ -697,17 +742,38 @@
         #      (if the item doesn't exists, Scribus crashes), or -1
 
         if self.linked["previous"] is None:
             xml.attrib["BACKITEM"] = "-1"
         else:
             xml.attrib["BACKITEM"] = self.linked["previous"]
 
+        # --- Flow ---------------------------------------------------
+
+        if self.ptype in ["polyline", "polygon", "text"]:
+
+            if self.text_flow:
+                # No text flow applied = no attribute TEXTFLOWMODE
+
+                for code, human in PageObject.text_flow_xml.items():
+                    if self.text_flow != human:
+                        continue
+                    xml.attrib["TEXTFLOWMODE"] = str(code)
+
+        # --- Text on path : show path -------------------------------
+
+        if self.ptype in ["textonpath", "text"]:
+            xml.attrib["PLTSHOW"] = xmlc.bool_to_num(
+                self.path_options["text_on_path"]["show"]
+            )
+
+            xml.attrib["BASEOF"] = self.path_options["text_on_path"]["offset"].toxmlstr(True)
+
         # FIXME This exports undocumented attributes ----------
 
-        if self.ptype not in ["table", "group", "text"]:
+        if self.ptype not in ["table", "group", "text", "image"]:
 
             try:
                 xml, undoc_attribs = xmlc.all_undocumented_to_xml(
                     xml,
                     self.undocumented,
                     True,
                     self.ptype + " '{}'".format(self.name.strip()),
@@ -816,14 +882,15 @@
 
         self.rows = 0
         self.columns = 0
 
         self.cells = []
 
         self.style = None
+        self.data_style = None
 
         self.fill = {"color": "None", "shade": None}
 
         self.borders = {
             "left": None,
             "right": None,
             "top": None,
@@ -1245,14 +1312,19 @@
         xml = PageObject.toxml(self)
 
         if not isinstance(xml, ET._Element):
             return False
 
         # --- Attributes ---------------------------------------------
 
+        if self.style is None:
+            xml.attrib["TableStyle"] = ""
+        else:
+            xml.attrib["TableStyle"] = self.style
+
         self._update_rowcols_count()
 
         # Number of rows and columns ----------------------------
 
         if self.rows > 0:
             xml.attrib["Rows"] = str(self.rows)
         else:
@@ -1312,18 +1384,18 @@
 
         # --- Children -----------------------------------------------
 
         # TableData attributes
 
         tabdata = ET.Element("TableData")
 
-        if self.style is None:
+        if self.data_style is None:
             tabdata.attrib["Style"] = ""
         else:
-            tabdata.attrib["Style"] = self.style
+            tabdata.attrib["Style"] = self.data_style
 
         tabdata.attrib["FillColor"] = self.fill["color"]
 
         if self.fill["shade"] is None:
             tabdata.attrib["FillShade"] = "100"
         else:
             tabdata.attrib["FillShade"] = self.fill["shade"].toxmlstr(True)
@@ -1349,14 +1421,17 @@
         succeed = PageObject.fromxml(self, xml)
 
         if not succeed:
             return False
 
         # --- Attributes ---------------------------------------------
 
+        if (tstyle := xml.get("TableStyle")) is not None:
+            self.style = tstyle
+
         # Number of rows and columns
 
         if (rows := xml.get("Rows")) is not None:
             self.rows = int(rows)
 
         if (cols := xml.get("Columns")) is not None:
             self.columns = int(cols)
@@ -1405,16 +1480,16 @@
 
         border_tags = [i for i in pstyles.TableBorder.sides_xml.values()]
 
         for element in xml:
 
             if element.tag == "TableData":
 
-                if (style := element.get("Style")) is not None:
-                    self.style = style
+                if (dstyle := element.get("Style")) is not None:
+                    self.data_style = dstyle
 
                 if (fill_color := element.get("FillColor")) is not None:
                     self.fill["color"] = fill_color
 
                 if (fill_shade := element.get("FillShade")) is not None:
                     self.fill["shade"] = dimensions.Dim(
                         float(fill_shade), unit="pc"
@@ -1714,16 +1789,14 @@
 
         if not succeed:
             return False
 
         # --- Attributes ---------------------------------------------
 
         # NOTE FIXME
-        # PLTSHOW |(optional) Set to 1 if the path of a Text on a path
-        #         |should be shown
         # BASEOF  |(optional) Offset for the text from its path for text
         #         |on a path
 
         # NOTE FIXME
         # Undocumented :
         #
         # textPathType
@@ -1797,15 +1870,15 @@
                     self.stories.append(story)
 
         return True
 
     def toxml(self):
         """
         :rtype: lxml.etree._Element
-        :returns: Table object as LXML element
+        :returns: Text object as LXML element
         """
 
         xml = PageObject.toxml(self)
 
         if not isinstance(xml, ET._Element):
             return False
 
@@ -1850,31 +1923,91 @@
             pass
 
         # --- Children -----------------------------------------------
 
         if self.have_stories:
 
             for story in self.stories:
-                sx = story.toxml()
-                xml.append(sx)
+                story_xml = story.toxml()
+                xml.append(story_xml)
 
         return xml
 
 
+# FIXME TODO Maybe rebase TextObject and TextOnPathObject on a common class
+# instead of copying some parts into TextOnPathObject
+
 class TextOnPathObject(PageObject):
     """
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
     :type doc_parent: pyscribus.document.Document
     :param doc_parent: SLA DOCUMENT instance
     """
 
     def __init__(self, sla_parent=False, doc_parent=False):
         PageObject.__init__(self, "textonpath", sla_parent, doc_parent)
 
+        self.stories = []
+
+    def fromxml(self, xml):
+        succeed = PageObject.fromxml(self, xml)
+
+        for element in xml:
+
+            if element.tag == "StoryText":
+                story = stories.Story()
+
+                story.sla_parent = self.sla_parent
+                story.doc_parent = self.doc_parent
+
+                if (success := story.fromxml(element)) :
+                    if not self.stories:
+                        self.have_stories = True
+
+                    self.stories.append(story)
+
+        return True
+
+    def toxml(self):
+        """
+        :rtype: lxml.etree._Element
+        :returns: TextOnPath object as LXML element
+        """
+
+        xml = PageObject.toxml(self)
+
+        if not isinstance(xml, ET._Element):
+            return False
+
+        # FIXME This exports undocumented attributes -----------------
+
+        try:
+            xml, undoc_attribs = xmlc.all_undocumented_to_xml(
+                xml,
+                self.undocumented,
+                True,
+                self.ptype + " '{}'".format(self.name.strip()),
+                logger=logs.getLogger(),
+            )
+
+        except AttributeError:
+            # NOTE If fromxml was not used
+            pass
+
+        # --- Children -----------------------------------------------
+
+        if self.have_stories:
+
+            for story in self.stories:
+                story_xml = story.toxml()
+                xml.append(story_xml)
+
+        return xml
+
 
 class ImageObject(PageObject):
     """
     Image frame object
 
     :type sla_parent: pyscribus.sla.SLA
     :param sla_parent: SLA parent instance
@@ -1900,38 +2033,141 @@
     +------------+---------------------------------+---------------+
 
     :ivar string filepath: File path of the image
     :ivar string data: Data if the incorporated image
     :ivar string data_type: Filetype of the incorporated image
     """
 
+    render_xml = {
+        "0": "perceptual",
+        "1": "rel_colorimetric",
+        "2": "saturation",
+        "3": "abs_colorimetric",
+    }
+
+    compression_method_xml = {
+        "0": "auto",
+        "1": "jpeg",
+        "2": "flate",
+        "3": "none",
+    }
+
     def __init__(self, sla_parent=False, doc_parent=False, **kwargs):
         PageObject.__init__(self, "image", sla_parent, doc_parent)
 
         # Specific attributes to this subclass ---------------------------
 
         self.data = ""  # ImageData
         self.data_type = ""
         self.filepath = ""  # PFILE
 
+        self.render_intent = ImageObject.render_xml["0"]
+
+        self.page_number = 0
+        self.is_inline = False
+
+        self.compression = {
+            "method": "auto",
+            "__method": None,
+        }
+
         # Then, quick setup ----------------------------------------------
 
         self._quick_setup(kwargs)
 
+    def toxml(self):
+        """
+        :rtype: lxml.etree._Element
+        :returns: Table object as LXML element
+        """
+
+        xml = PageObject.toxml(self)
+
+        xml.attrib["Pagenumber"] = str(self.page_number)
+
+        # Compression method ------------------------------
+
+        # @CMethod and @COMPRESSIONMETHOD follow the same syntax
+        cmethod_att = self.compression["__method"]
+
+        if cmethod_att is not None:
+
+            for code, human in ImageObject.compression_method_xml.items():
+                if human == self.compression["method"]:
+                    xml.attrib[cmethod_att] = code
+                    break
+
+        # -------------------------------------------------
+
+        for code, human in ImageObject.render_xml.items():
+            if self.render_intent == human:
+                xml.attrib["IRENDER"] = code
+
+        if self.is_inline:
+            xml.attrib["isInlineImage"] = xmlc.bool_to_num(self.is_inline)
+
+        # FIXME This exports undocumented attributes -----------------
+
+        try:
+            xml, undoc_attribs = xmlc.all_undocumented_to_xml(
+                xml,
+                self.undocumented,
+                True,
+                self.ptype + " '{}'".format(self.name.strip()),
+                logger=logs.getLogger(),
+            )
+
+        except AttributeError:
+            # NOTE If fromxml was not used
+            pass
+
+        return xml
+
     def fromxml(self, xml):
         succeed = PageObject.fromxml(self, xml)
 
         if not succeed:
             return False
 
         # --- Attributes ---------------------------------------------
 
         ipath = xml.get("PFILE")
         idata_ext = xml.get("inlineImageExt")
 
+        # Compression method ------------------------------
+
+        # @CMethod and @COMPRESSIONMETHOD follow the same syntax
+
+        cmethod = xml.get("CMethod")
+        cmethod_long = xml.get("COMPRESSIONMETHOD")
+
+        for att, value in [[cmethod_long], [cmethod]]:
+            if value is None:
+                continue
+
+            self.compression["method"] = ImageObject.compression_method_xml[value]
+            self.compression["__method"] = att
+
+        # -------------------------------------------------
+
+        if (irender := xml.get("IRENDER")) is not None:
+            for code, human in ImageObject.render_xml.items():
+                if irender == code:
+                    self.render_intent = human
+
+        if (is_inline := xml.get("isInlineImage")) is not None:
+            self.is_inline = xmlc.num_to_bool(is_inline)
+
+        if (pgnumber := xml.get("Pagenumber")) is not None:
+            try:
+                pgnumber = int(pgnumber)
+                self.page_number = pgnumber
+            except ValueError:
+                self.page_number = 0
+
         if (idata := xml.get("ImageData")) is not None:
             if idata:
                 self.data = idata
 
         if (idata_ext := xml.get("inlineImageExt")) is not None:
             if idata_ext:
                 self.data_type = idata_ext
```

### Comparing `pyscribus-0.2.4/pyscribus/pages.py` & `pyscribus-0.2.5/pyscribus/pages.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/papers/__init__.py` & `pyscribus-0.2.5/pyscribus/papers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/papers/afnor.py` & `pyscribus-0.2.5/pyscribus/papers/afnor.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/papers/ansi.py` & `pyscribus-0.2.5/pyscribus/papers/ansi.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/papers/iso216.py` & `pyscribus-0.2.5/pyscribus/papers/iso216.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/papers/iso217.py` & `pyscribus-0.2.5/pyscribus/papers/iso217.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/papers/iso269.py` & `pyscribus-0.2.5/pyscribus/papers/iso269.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/papers/newspaper.py` & `pyscribus-0.2.5/pyscribus/papers/newspaper.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/patterns.py` & `pyscribus-0.2.5/pyscribus/patterns.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus/printing.py` & `pyscribus-0.2.5/pyscribus/printing.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # Imports ===============================================================#
 
 # To avoid Sphinx complaints from methods annotations referencing same class
 from __future__ import annotations
 
 import collections
 
-from typing import NoReturn
+from typing import NoReturn, Union
 
 import lxml
 import lxml.etree as ET
 
 import pyscribus.exceptions as exceptions
 
 from pyscribus.common.xml import *
@@ -61,14 +61,15 @@
         "min": 4,
     }
 
     def __init__(self):
         super().__init__()
 
         self.lpi = []
+        self.use_lpi = False
 
         self.text_compression = True
         self.image_compression = {"method": "automatic", "quality": "max"}
 
         # ------------------------------------------------------
 
         # Flag, set to 1 when Presentation effects should be used
@@ -148,34 +149,53 @@
             "offset": dimensions.Dim(0),
             # markLength, 7.056mm but encoded in pics => roughly 20
             "length": dimensions.Dim(20),
         }
 
         # ------------------------------------------------------
 
+        # All         : -2359300
+        # None        : -2359360
+        # Only print  : -2359356
+        # Only modify : -2359352
+        # Only copy   : -2359344
+        # Only annoto : -2359328
+
         self.encryption = {
             "pass": {"owner": "", "user": ""},
             "settings": {"permissions": "-4", "encrypted": False},
         }
 
         # FIXME Documented but to organize ----------------------
 
-        # (optional) Flag, set to 1 when the informations in the LPI tags should be used
-        # for Linescreening
-        UseLpi = "0"
         # Binding for the PDF-Document 0 = Left Binding 1 = Right Binding
         Binding = "0"
-        # PDF-Version which should be generated 12 = PDF-X/3 13 = PDF-1.3 14 = PDF-1.4
-        Version = "14"
-        # Flag, set to 1 when Generate Thumbnails is checked in the PDF-Options Dialog
-        Thumbnails = "0"
-        # Flag, set to 1 when use PDF-Articles is checked in the PDF-Options Dialog
-        Articles = "0"
-        # Flag, set to 1 when include Bookmarks is checked in the PDF-Options Dialog
-        Bookmarks = "0"
+
+        # PDF version -------------------------------------------
+
+        self.version = "13"
+
+        # FIXME Documented but to organize ----------------------
+
+        self.objects = {
+            # Flag, set to 1 when Generate Thumbnails is checked in the
+            # PDF-Options Dialog
+            # Thumbnails = "0"
+            "thumbnails": False,
+            # Flag, set to 1 when include Bookmarks is checked in the
+            # PDF-Options Dialog
+            # Bookmarks = "0"
+            "bookmarks": False,
+            # Flag, set to 1 when use PDF-Articles is checked in the
+            # PDF-Options Dialog
+            # Articles = "0"
+            "articles": False,
+            # EmbedPDF="0"
+            "embedded_pdf": False,
+        }
 
         # FIXME Undocumented, managed with undocumented funs ----
 
         # ImagePr="0"
         # UseLayers="0"
         # UseSpotColors="1"
         # doMultiFile="0"
@@ -191,21 +211,88 @@
         # openAction=""
         # Intent="1"
         # Intent2="0"
         # InfoString=""
         # FontEmbedding="0"
         # Grayscale="0"
         # firstUse="1"
-        # EmbedPDF="0"
-        # MirrorH="0"
-        # MirrorV="0"
         # Clip="0"
         # rangeSel="0"
         # rangeTxt=""
-        # RotateDeg="0"
+
+        # Transformation ----------------------------------------
+
+        self.transformation = {
+            # RotateDeg="0"
+            # Four values: 0, 90, 180, 270
+            "rotation": dimensions.Dim(0, unit="deg", integer=True),
+            # MirrorH="0"
+            "mirror_h": False,
+            # MirrorV="0"
+            "mirror_v": False,
+        }
+
+    def set_version(self, version: Union[str, int, float]):
+        # We should check against Scribus version because
+        # PDF-X-3, PDF-X-4, PDF-X-1a seems not available in Scribus 1.5.
+
+        # 12 = PDF-X/3
+        # 13 = PDF-1.3 (Acrobat 4)
+        # 14 = PDF-1.4 (Acrobat 5)
+        # 15 = PDF-1.5 (Acrobat 6)
+        # 16 = PDF-1.6 (Acrobat 7)
+
+        new_version = None
+
+        if isinstance(version, float):
+
+            if int(version) in [13, 14, 15, 16]:
+                self.version = str(int(version))
+                return True
+
+            if version in [1.3, 1.4, 1.5, 1.6]:
+                new_version = str(version)
+                self.version = new_version.replace(".", "")
+                return True
+
+        if isinstance(version, int):
+
+            if version in [13, 14, 15, 16]:
+                self.version = str(version)
+                return True
+
+        if isinstance(version, str):
+
+            if version in ["1.3", "1.4", "1.5", "1.6"]:
+                new_version = version
+                self.version = new_version.replace(".", "")
+                return True
+
+            if version.startswith("acrobat-"):
+                acro_version = version.split("acrobat-")[-1]
+
+                if not acro_version:
+                    return False
+
+                try:
+                    self.version = {
+                        "4": "13",
+                        "5": "14",
+                        "6": "15",
+                        "7": "16",
+                    }[acro_version]
+                    return True
+                except KeyError:
+                    return False
+
+            if version == "X/3":
+                self.version = "12"
+                return True
+
+        return False
 
     def fromxml(self, xml: ET.Element) -> bool:
 
         if xml.tag != "PDF":
             return False
 
         # TODO
@@ -259,15 +346,70 @@
 
         for mark_tag, mark_key in [
                 ["markOffset", "offset"],
                 ["markLength", "length"]]:
             if (attrib := xml.get(mark_tag)) is not None:
                 self.marks[mark_key].value = float(attrib)
 
-        # PDF encryption settings---------------------------
+        # Version --------------------------------------------------------
+
+        version = xml.get("Version")
+
+        if version is not None:
+            self.version = version
+
+        # Objects to embed / generate ------------------------------------
+
+        embedded_pdf = xml.get("EmbedPDF")
+        thumbnails = xml.get("Thumbnails")
+        bookmarks = xml.get("Bookmarks")
+        articles = xml.get("Articles")
+
+        for att_value, human in [
+                [thumbnails, "thumbnails"], [bookmarks, "bookmarks"],
+                [articles, "articles"], [embedded_pdf, "embedded_pdf"]]:
+            if att_value is None:
+                continue
+
+            self.objects[human] = num_to_bool(att_value)
+
+        # Transformation ----------------------------------------
+
+        rotation = xml.get("RotateDeg")
+
+        if rotation is not None:
+            try:
+                rotation = int(rotation)
+
+                if rotation in [0, 90, 180, 270]:
+                    self.transformation["rotation"].value = rotation
+                else:
+                    raise exceptions.InsaneSLAValue(
+                        "PDF settings Rotation: "
+                        "Allowed values are 0, 90, 180, 270. "
+                        f"Got {rotation}."
+                    )
+            except ValueError:
+                raise exceptions.InsaneSLAValue(
+                    "PDF settings Rotation: "
+                    "Requires an integer. "
+                    f"Got {rotation}."
+                )
+
+        mirrorh = xml.get("MirrorH")
+        mirrorv = xml.get("MirrorV")
+
+        for att_value, human in [
+                [mirrorh, "mirror_h"],  [mirrorv, "mirror_v"]]:
+            if att_value is None:
+                continue
+
+            self.transformation[human] = num_to_bool(att_value)
+
+        # PDF encryption settings-----------------------------------------
 
         encrypt = xml.get("Encrypt")
         encrypt_perm = xml.get("Permissions")
 
         for pass_key, pass_tag in [["owner", "PassOwner"], ["user", "PassUser"]]:
             if (attrib := xml.get(pass_tag)) is not None:
                 self.encryption["pass"][pass_key] = attrib
@@ -276,21 +418,30 @@
             self.encryption["settings"]["encrypted"] = num_to_bool(encrypt)
 
         if encrypt_perm is not None:
             self.encryption["settings"]["permissions"] = encrypt_perm
 
         # Line per inch settings ---------------------------
 
+        # Flag, set to 1 when the informations in the LPI tags should be used
+        # for Linescreening
+        # IT IS NOT OPTIONAL
+        uselpi = xml.get("UseLpi")
+        if uselpi is not None:
+            self.use_lpi = num_to_bool(uselpi)
+
         for element in xml:
-            if element.tag == "LPI":
-                lo = LPI()
-                success = lo.fromxml(element)
+            if element.tag != "LPI":
+                continue
+
+            lpi_item = LPI()
+            success = lpi_item.fromxml(element)
 
-                if success:
-                    self.lpi.append(lo)
+            if success:
+                self.lpi.append(lpi_item)
 
         # FIXME This records undocumented attributes ----------
 
         self.undocumented = undocumented_to_python(
             xml,
             [
                 "ImagePr",
@@ -309,21 +460,17 @@
                 "openAction",
                 "Intent",
                 "Intent2",
                 "InfoString",
                 "FontEmbedding",
                 "Grayscale",
                 "firstUse",
-                "EmbedPDF",
-                "MirrorH",
-                "MirrorV",
                 "Clip",
                 "rangeSel",
                 "rangeTxt",
-                "RotateDeg",
             ],
         )
 
         return True
 
     def toxml(self) -> ET.Element:
         xml = ET.Element("PDF")
@@ -362,32 +509,52 @@
                 ["colorMarks", "colors"],
                 ["registrationMarks", "alignment"]]:
             xml.attrib[mark_tag] = bool_to_num(self.marks[mark_key])
 
         for mark_tag, mark_key in [
                 ["markOffset", "offset"],
                 ["markLength", "length"]]:
-            xml.attrib[mark_tag] = self.marks[mark_key].toxmlstr()
+            xml.attrib[mark_tag] = self.marks[mark_key].toxmlstr(True)
 
         # PDF encryption settings---------------------------
 
         xml.attrib["PassOwner"] = self.encryption["pass"]["owner"]
         xml.attrib["PassUser"] = self.encryption["pass"]["user"]
         xml.attrib["Permissions"] = self.encryption["settings"]["permissions"]
         xml.attrib["Encrypt"] = bool_to_num(
             self.encryption["settings"]["encrypted"]
         )
 
+        # Version ------------------------------------------
+
+        xml.attrib["Version"] = str(self.version)
+
+        # Objects to embed / generate ------------------------------------
+
+        for code, human in [
+                ["Thumbnails", "thumbnails"], ["Bookmarks", "bookmarks"],
+                ["Articles", "articles"], ["EmbedPDF", "embedded_pdf"]]:
+            xml.attrib[code] = bool_to_num(self.objects[human])
+
+        # Transformation ----------------------------------------
+
+        xml.attrib["RotateDeg"] = self.transformation["rotation"].toxmlstr(True)
+
+        for code, human in [["MirrorH", "mirror_h"], ["MirrorV", "mirror_v"]]:
+            xml.attrib[code] = bool_to_num(self.transformation[human])
+
         # Line per Inch children ---------------------------
 
-        for lo in self.lpi:
-            lx = lo.toxml()
+        xml.attrib["UseLpi"] = bool_to_num(self.use_lpi)
 
-            if len(lx):
-                xml.append(lx)
+        for lpi_item in self.lpi:
+            lpi_xml = lpi_item.toxml()
+
+            if lpi_xml is not None:
+                xml.append(lpi_xml)
 
         # FIXME This exports undocumented attributes ----------
 
         try:
             xml = undocumented_to_xml(xml, self.undocumented)
         except AttributeError:
             pass
@@ -463,14 +630,15 @@
                         self.spot = lpd[3]
                     else:
                         self.spot = "ellipse"
 
                     break
 
     def fromxml(self, xml: ET.Element) -> bool:
+
         if xml.tag != "LPI":
             return False
 
         if (color := xml.get("Color")) is not None:
             self.color = color
 
         if (freq := xml.get("Frequency")) is not None:
@@ -484,20 +652,23 @@
             for human, code in LPI.spot_xml.items():
                 if code == spot:
                     self.spot = human
                     break
 
         return True
 
-    def toxml(self) -> ET.Element:
+    def toxml(self) -> Union[ET.Element, None]:
         xml = ET.Element("LPI")
 
+        if not self.color:
+            return None
+
         xml.attrib["Color"] = self.color
-        xml.attrib["Frequency"] = self.frequency.toxmlstr()
-        xml.attrib["Angle"] = self.angle.toxmlstr()
+        xml.attrib["Frequency"] = self.frequency.toxmlstr(True)
+        xml.attrib["Angle"] = self.angle.toxmlstr(True)
         xml.attrib["SpotFunction"] = LPI.spot_xml[self.spot]
 
         return xml
 
 
 class PrinterSettings(PyScribusElement):
     def __init__(self):
@@ -540,14 +711,15 @@
         PDLanguage = "0"
         markLength = "7.185302734375"
         markOffset = "0"
 
         # --- Bleeds --------------------------------------------
 
         self.bleeds = collections.OrderedDict()
+
         self.bleeds["top"] = (dimensions.Dim(0),)
         self.bleeds["left"] = (dimensions.Dim(0),)
         self.bleeds["right"] = (dimensions.Dim(0),)
         self.bleeds["bottom"] = (dimensions.Dim(0),)
         self.bleeds["document"] = False
 
         # -------------------------------------------------------
@@ -571,15 +743,15 @@
 
         if (mrv := xml.get("mirrorV")) is not None:
             self.mirror_pages["vertical"] = num_to_bool(mrv)
 
         # --- Marks ---------------------------------------------
 
         for case in ["crop", "bleed", "registration", "color"]:
-            att_name = "{}Marks".format(case)
+            att_name = f"{case}Marks"
 
             if (att := xml.get(att_name)) is not None:
                 self.marks[case] = num_to_bool(att)
 
         # --- Printer bleeds ------------------------------------
 
         for case in ["top", "left", "right", "bottom"]:
@@ -607,16 +779,16 @@
                 xml.attrib[att_name] = bleed_value[0].toxmlstr()
 
         xml.attrib["mirrorH"] = bool_to_num(self.mirror_pages["horizontal"])
         xml.attrib["mirrorV"] = bool_to_num(self.mirror_pages["vertical"])
 
         xml.attrib["useDocBleeds"] = bool_to_num(self.bleeds["document"])
 
-        for k, v in self.marks.items():
-            att_name = "{}Marks".format(k)
+        for key, value in self.marks.items():
+            att_name = f"{key}Marks"
 
-            xml.attrib[att_name] = bool_to_num(v)
+            xml.attrib[att_name] = bool_to_num(value)
 
         return xml
 
 
 # vim:set shiftwidth=4 softtabstop=4 spl=en:
```

### Comparing `pyscribus-0.2.4/pyscribus/sla.py` & `pyscribus-0.2.5/pyscribus/sla.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,17 @@
 
                 try:
                     pattern = re.compile(argvalue)
                     self.templating["intext-pattern"] = pattern
 
                 except TypeError as not_re_pattern:
 
-                    raise TypeError("templating-pattern must be a re pattern string.") from not_re_pattern
+                    raise TypeError(
+                        "templating-pattern must be a re pattern string."
+                    ) from not_re_pattern
 
         if filepath:
             filepath = Path(filepath)
 
             self.parse(filepath, kwargs)
 
     def fromdefault(self) -> bool:
@@ -219,15 +221,15 @@
         """
 
         all_stories = self.document.stories()
 
         if templatable and self.templating["active"]:
             return [story for story in all_stories if story.templatable()]
 
-        return stories
+        return all_stories
 
     def pageobjects(
             self,
             object_type: StringOrBoolean=False,
             templatable: bool = False) -> list:
         """
         Return document page objets.
```

### Comparing `pyscribus-0.2.4/pyscribus/stories.py` & `pyscribus-0.2.5/pyscribus/stories.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,21 @@
 
        frag = stories.StoryFragment(
            text="Lorem ipsum", fontsize=7, fontcolor="Grey"
        )
 
     """
 
+    font_xml = [
+        ["name", "FONT"],
+        ["color", "FCOLOR"],
+        ["opacity", "FSHADE"],
+        ["size", "FONTSIZE"]
+    ]
+
     def __init__(self, **kwargs):
         super().__init__()
 
         self.text = ""
 
         # To not export to XML. This is defined by the following
         # StoryParagraphEnding in Story.sequence
@@ -371,28 +378,26 @@
         xml = ET.Element("ITEXT")
 
         have_features = len([f for f in self.features.values() if f])
 
         if have_features:
             features = []
 
-            for f, v in self.features.items():
-                if v:
-                    features.append(f)
+            for feature_name, feature_value in self.features.items():
+                if feature_value:
+                    features.append(feature_name)
 
             features = " ".join(features)
 
             xml.attrib["FEATURES"] = features
 
-        for case in zip(
-            ["name", "color", "opacity", "size"],
-            ["FONT", "FCOLOR", "FSHADE", "FONTSIZE"],
-        ):
-            if self.font[case[0]]:
-                xml.attrib[case[1]] = self.font[case[0]]
+        for human, attr_name in StoryFragment.font_xml:
+
+            if self.font[human]:
+                xml.attrib[attr_name] = self.font[human]
 
         xml.attrib["CH"] = self.text
 
         return xml
 
     def fromxml(self, xml: ET._Element) -> bool:
         if (fragtext := xml.get("CH")) is None:
@@ -401,21 +406,18 @@
         # NOTE Don't do any strip, rstrip to @CH, as it may
         # contains legitimate spaces
         self.text = fragtext
 
         if (features := xml.get("FEATURES")) is not None:
             self.set_features(features)
 
-        for case in zip(
-            ["name", "color", "opacity", "size"],
-            ["FONT", "FCOLOR", "FSHADE", "FONTSIZE"],
-        ):
+        for human, attr_name in StoryFragment.font_xml:
 
-            if (att := xml.get(case[1])) is not None:
-                self.font[case[0]] = att
+            if (att := xml.get(attr_name)) is not None:
+                self.font[human] = att
 
         # TODO Reste de l’implémentation, puis :
 
         return True
 
     def set_features(self, features: str) -> NoReturn:
         # TODO
```

### Comparing `pyscribus-0.2.4/pyscribus/styles.py` & `pyscribus-0.2.5/pyscribus/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 StringOrPath = Union[str, Path]
 BoolOrElement = Union[bool, ET.Element]
 
 LeadingMode = Literal["fixed", "automatic", "grid"]
 
 # Classes ===============================================================#
 
+
 class TextDirection(IntEnum):
     """
     Enum for (paragraph) STYLE/@DIRECTION values.
     """
 
     LTR = 0
     RTL = 1
@@ -66,15 +67,15 @@
         "document": "0",
         "section": "1",
         "story": "2",
         "page": "3",
         "form": "4",
     }
 
-    def __init__(self, default: bool=False):
+    def __init__(self, default: bool = False):
         super().__init__()
 
         if default:
             self.fromdefault()
         else:
             self.name = ""
             self.set_type("footnote")
@@ -92,15 +93,15 @@
         # if numtype.lower() in NoteStyle.keys():
         if numtype.lower() in xmlc.num_type_xml.keys():
             self.num_type = numtype.lower()
             return True
 
         return False
 
-    def set_type(self, note_type: str="footnote") -> NoReturn:
+    def set_type(self, note_type: str = "footnote") -> NoReturn:
         if note_type.lower() == "footnote":
             self.is_endnotes = False
             self.is_footnotes = True
         else:
             self.is_endnotes = True
             self.is_footnotes = False
 
@@ -263,26 +264,27 @@
                 "color": "",
                 "alignment": "left",
                 "strike": {"width": None, "offset": None},
                 "underline": {"width": None, "offset": None},
                 "shadow": {"hoffset": None, "voffset": None},
                 # NOTE There is no offset setting for outline, obviously
                 "outline": {"width": None},
+                "kerning": None,
             }
 
             # NOTE Weird, but FONTFEATURES is not the same as FEATURES
             # even if it has obviously an effect on fonts...
             self.features = {}
 
             self.lang = None
             self.shortcut = None
 
             self.background = {
                 "color": "None",
-                "shade": dimensions.Dim(100, unit="pc", integer=True)
+                "shade": dimensions.Dim(100, unit="pc", integer=True),
             }
 
         if self.style_type in ["table", "cell", "character", "paragraph"]:
             self.fill = {"color": None, "shade": None}
 
         if self.style_type in ["table", "cell"]:
             self.borders = []
@@ -295,15 +297,15 @@
             self.character_parent = ""
 
             self.space = {
                 "after": None,
                 "before": None,
             }
 
-            self.leading = {"mode": None, "value": dimensions.Dim(0)}
+            self.leading = {"mode": "fixed", "value": dimensions.Dim(0)}
 
         if default:
             self.fromdefault()
 
         if kwargs:
             self._quick_setup(kwargs)
 
@@ -356,21 +358,23 @@
 
         return False
 
     def fromdefault(self) -> bool:
         self.name = StyleAbstract.default_name[self.style_type]
 
         if self.style_type in ["paragraph", "character"]:
-            self.font = StyleAbstract.default_font
+            self.font |= StyleAbstract.default_font
 
         # TODO Le reste
 
         return True
 
-    def fromxml(self, xml: ET.Element, onlybool: bool=False) -> BoolOrElement:
+    def fromxml(
+        self, xml: ET.Element, onlybool: bool = False
+    ) -> BoolOrElement:
 
         if xml.tag != StyleAbstract.type_xml[self.style_type]:
             return False
 
         # Name -------------------------------------------------
 
         if self.style_type in ["paragraph", "table", "cell", "character"]:
@@ -392,22 +396,15 @@
 
         # Specific attributes for table ------------------------
 
         if self.style_type == "table":
             pass
 
         # Specific attributes for cell -------------------------
-
-        if self.style_type == "cell":
-
-            for case in ["left", "right", "top", "bottom"]:
-                att = xml.get("{}Padding".format(case.capitalize()))
-
-                if att is not None:
-                    self.padding[case] = att
+        # Moved in CellStyle
 
         # Common attributes to paragraphs + characters ---------
 
         if self.style_type in ["paragraph", "character"]:
 
             bshade_att = self._choose_att(StyleAbstract.bg_shade_xml)
             bcolor_att = self._choose_att(StyleAbstract.bg_color_xml)
@@ -467,14 +464,19 @@
                 )
 
             if (outline_width := xml.get("TXTOUT")) is not None:
                 self.font["outline"]["width"] = dimensions.Dim(
                     float(outline_width), unit="pcdecim"
                 )
 
+            if (kerning := xml.get("KERN")) is not None:
+                self.font["kerning"] = dimensions.Dim(
+                    float(kerning), unit="pc"
+                )
+
             # Lang ---------------------------------------------------
 
             if (lang := xml.get("LANGUAGE")) is not None:
                 if lang:
                     self.lang = lang
 
             # Parent style -------------------------------------------
@@ -542,22 +544,14 @@
             xml.attrib["DefaultStyle"] = xmlc.bool_to_num(self.is_default)
 
         # Specific attributes for table ------------------------
 
         if self.style_type == "table":
             pass
 
-        # Specific attributes for cell -------------------------
-
-        if self.style_type == "cell":
-
-            for case in ["left", "right", "top", "bottom"]:
-                att_name = "{}Padding".format(case.capitalize())
-                xml.attrib[att_name] = self.padding[case]
-
         # Common attributes to paragraphs + characters ---------
 
         if self.style_type in ["paragraph", "character"]:
 
             bshade_att = self._choose_att(StyleAbstract.bg_shade_xml)
             bcolor_att = self._choose_att(StyleAbstract.bg_color_xml)
 
@@ -611,14 +605,17 @@
                 ].toxmlstr(True)
 
             if self.font["underline"]["offset"] is not None:
                 xml.attrib["TXTULP"] = self.font["underline"][
                     "offset"
                 ].toxmlstr(True)
 
+            if self.font["kerning"] is not None:
+                xml.attrib["KERN"] = self.font["kerning"].toxmlstr(True)
+
             if self.features:
                 xml.attrib["FEATURES"] = self.features
 
             if self.lang is not None:
                 xml.attrib["LANGUAGE"] = self.lang
 
             if self.shortcut is not None:
@@ -661,15 +658,15 @@
 
         except AttributeError:
             # NOTE If fromxml was not used
             pass
 
         return xml
 
-    def fromstyle(self, style, override: bool=False):
+    def fromstyle(self, style, override: bool = False):
         """
         Set attributes according to another style.
 
         :type style: ParagraphStyle, CharacterStyle, ...
         :param style: Style to load attributes from.
         :type override: boolean
         :param override: Override attributes that differs from style
@@ -751,27 +748,44 @@
 
     glyph_scale_xml = {
         "max": "MaxGlyphExtend",
         "min": "MinGlyphShrink",
     }
 
     optical_margins_xml = {
-        "both": 14,
-        "left": 4,
-        "right": 8,
-        "none": 0,
-        "undef": None
+        "both": "14",
+        "left": "4",
+        "right": "8",
+        "none": "0",
+        "undef": None,
+    }
+
+    ol_types = {
+        "decimal": "0",
+        "decimal-ar": "1",
+        "lower-roman": "2",
+        "upper-roman": "3",
+        "lower-latin": "4",
+        "upper-latin": "5",
+        "alpha-ar": "6",
+        "abjad-ar": "7",
+        # SEUL CONTRE LES DIEUX CONTRE L'ODIEUX CESAR
+        "asterix": "8",
+        "cjk": "9",
+        "hebrew": "10",
     }
 
     def __init__(self, doc_parent, default=False, **kwargs):
         StyleAbstract.__init__(self, "paragraph", doc_parent, default)
 
         self.indentations = {"left": None, "right": None, "first-line": None}
 
-        self.listing = {"type": None, "char": None}
+        self.listing = {"type": None, "char": None, "subtype": None}
+
+        self.hyphen_following_lines = None
 
         self.glyph_scaling = {
             "min": dimensions.Dim(1.0, unit="pcscale"),
             "max": dimensions.Dim(1.0, unit="pcscale"),
         }
 
         self.initial = {
@@ -793,30 +807,44 @@
 
     def fromxml(self, xml: ET.Element) -> bool:
         is_paragraph = StyleAbstract.fromxml(self, xml, True)
 
         if not is_paragraph:
             return False
 
+        # Hyphenation ---------------------------------------------------
+
+        if (hyphen_lines := xml.get("HyphenConsecutiveLines")) is not None:
+            try:
+                hyphen_lines = int(hyphen_lines)
+
+                self.hyphen_following_lines = hyphen_lines
+            except ValueError:
+                self.hyphen_following_lines = 2
+
         # Text direction ------------------------------------------------
 
         if (text_direction := xml.get("DIRECTION")) is not None:
 
             if xmlc.num_to_bool(text_direction):
                 self.text_direction = TextDirection.RTL
             else:
                 self.text_direction = TextDirection.LTR
 
         # Optical margins -----------------------------------------------
 
-        optic_margin = xml.get("OpticalMargins")
+        if (optic_margin := xml.get("OpticalMargins")) is None:
+            self.optical_margins = "undef"
+        else:
+            for human, value in ParagraphStyle.optical_margins_xml.items():
+                if value is None or value != optic_margin:
+                    continue
 
-        for human, value in ParagraphStyle.optical_margins_xml.items():
-            if value == optic_margin:
                 self.optical_margins = human
+                break
 
         # Initial capital (aka drop capital) ----------------------------
 
         if (initial_used := xml.get("DROP")) is not None:
             self.initial["active"] = xmlc.num_to_bool(initial_used)
 
         if (initial_lines := xml.get("DROPLIN")) is not None:
@@ -868,14 +896,21 @@
                 is_ul = True
 
         if (is_numeroted := xml.get("Numeration")) is not None:
             if is_numeroted == "1":
                 self.listing["type"] = "ol"
                 is_ol = True
 
+        if (num_format := xml.get("NumerationFormat")) is not None:
+            if is_ol:
+                for human, code in ParagraphStyle.ol_types.items():
+                    if code == num_format:
+                        self.listing["subtype"] = human
+                        break
+
         if is_ol and is_ul:
             raise exceptions.InsaneSLAValue(
                 "Style {} is both bullet and numeroted list.".format(self.name)
             )
 
         if (bullet_char := xml.get("BulletStr")) is not None:
             self.listing["char"] = bullet_char
@@ -890,19 +925,22 @@
         if (leading := xml.get("LINESPMode")) is not None:
 
             for human, code in ParagraphStyle.leading_xml.items():
                 if leading == code:
                     self.leading["mode"] = human
                     break
 
-            if self.leading["mode"] == "fixed":
-                leading_value = xml.get("LINESP")
+        if (leading_value := xml.get("LINESP")) is not None:
+            # NOTE Leading value unit is pica in fixed mode, in points in
+            #      automatic mode.
+            if self.leading["mode"] == "automatic":
+                self.leading["value"].set_unit("pt")
 
-                if leading_value is not None:
-                    self.leading["value"].value = float(leading_value)
+            if self.leading["mode"] in ["fixed", "automatic"]:
+                self.leading["value"].value = float(leading_value)
 
         # Alignment -----------------------------------------------------
 
         if (alignment := xml.get("ALIGN")) is not None:
             for human, code in xmlc.alignment.items():
                 if alignment == code:
                     self.font["alignment"] = human
@@ -918,15 +956,15 @@
         # Tabs ----------------------------------------------------------
 
         for child in xml:
 
             if child.tag == "Tabs":
                 to = StyleTab()
 
-                if (success := to.fromxml(child)) :
+                if success := to.fromxml(child):
                     self.tabs.append(to)
 
         # End of parsing ------------------------------------------------
 
         self.undocumented = xmlc.all_undocumented_to_python(xml)
 
         return True
@@ -934,30 +972,41 @@
     def toxml(self) -> ET.Element:
         xml = StyleAbstract.toxml(self)
 
         # Text direction ------------------------------------------------
 
         xml.attrib["DIRECTION"] = str(int(self.text_direction))
 
+        # Hyphenation ---------------------------------------------------
+
+        if self.hyphen_following_lines is not None:
+            xml.attrib["HyphenConsecutiveLines"] = str(
+                self.hyphen_following_lines
+            )
+
         # Optical margins -----------------------------------------------
 
         if self.optical_margins is not None:
             xml.attrib["OpticalMargins"] = str(
                 ParagraphStyle.optical_margins_xml[self.optical_margins]
             )
 
         # Initial capital (aka drop capital) ----------------------------
 
         xml.attrib["DROP"] = xmlc.bool_to_num(self.initial["active"])
         xml.attrib["DROPLIN"] = str(self.initial["lines"])
 
-        xml.attrib[self.initial["__offset_att"]] = self.initial["offset"].toxmlstr()
+        xml.attrib[self.initial["__offset_att"]] = self.initial[
+            "offset"
+        ].toxmlstr()
 
         if self.initial["auto_indent"]:
-            xml.attrib["ParagraphEffectIndent"] = xmlc.bool_to_num(self.initial["auto_indent"] )
+            xml.attrib["ParagraphEffectIndent"] = xmlc.bool_to_num(
+                self.initial["auto_indent"]
+            )
 
         # Glyph scaling ---------------------------------------------
 
         for human, att in ParagraphStyle.glyph_scale_xml.items():
             if self.glyph_scaling[human].value != 1.0:
                 xml.attrib[att] = self.glyph_scaling[human].toxmlstr()
 
@@ -966,15 +1015,16 @@
         xml.attrib["ALIGN"] = xmlc.alignment[self.font["alignment"]]
 
         if self.leading["mode"] is not None:
             xml.attrib["LINESPMode"] = ParagraphStyle.leading_xml[
                 self.leading["mode"]
             ]
 
-            if self.leading["mode"] == "fixed":
+        if self.leading["mode"] in ["fixed", "automatic"]:
+            if self.leading["value"].value > 0:
                 xml.attrib["LINESP"] = self.leading["value"].toxmlstr()
 
         # Indentation -----------------------------------------------
 
         for case in [
             ["left", "INDENT"],
             ["right", "RMARGIN"],
@@ -991,16 +1041,21 @@
         if self.listing["type"] == "ol":
             att_seq = [False, True]
         elif self.listing["type"] == "ul":
             att_seq = [True, False]
         else:
             att_seq = [False, False]
 
-        for case in zip(att_seq, ["Bullet", "Numeration"]):
-            xml.attrib[case[1]] = xmlc.bool_to_num(case[0])
+        for list_val, list_att in zip(att_seq, ["Bullet", "Numeration"]):
+            xml.attrib[list_att] = xmlc.bool_to_num(list_val)
+
+        if self.listing["type"] == "ol":
+            xml.attrib["NumerationFormat"] = ParagraphStyle.ol_types[
+                self.listing["subtype"]
+            ]
 
         xml.attrib["BulletStr"] = xmlc.none_or_str(self.listing["char"])
 
         # Parent character style ------------------------------------
 
         # NOTE To not confuse with parent paragraph style which is
         # in @PARENT, and handled in StyleAbstract
@@ -1093,17 +1148,15 @@
                 self.character_parent = setting_value
 
             if setting_name == "leading":
                 if setting_value in ParagraphStyle.leading_xml:
                     self.leading["mode"] = setting_value
 
             if setting_name == "leadingValue":
-                self.leading["value"] = dimensions.Dim(
-                    float(setting_value)
-                )
+                self.leading["value"] = dimensions.Dim(float(setting_value))
 
             if setting_name == "alignment":
 
                 if setting_value.lower() in xmlc.alignment.keys():
                     self.font["alignment"] = setting_value
                 else:
                     raise ValueError(
@@ -1156,23 +1209,22 @@
     |              | the default name.           |          |
     +--------------+-----------------------------+----------+
     """
 
     scale_xml = {
         "SCALEH": "horizontal",
         "SCALEV": "vertical",
-        "BASEO": "baseline_offset"
+        "BASEO": "baseline_offset",
     }
 
     def __init__(self, doc_parent, default=False, **kwargs):
         StyleAbstract.__init__(self, "character", doc_parent, default)
         StyleAbstract._quick_setup(self, kwargs)
 
         self.font["space_width"] = dimensions.Dim(1, unit="pcdecim")
-        self.font["kerning"] = None
 
         self.hyphen_word_min = None
 
         self.scale = {
             "horizontal": 100,
             "vertical": 100,
             "baseline_offset": 0,
@@ -1219,17 +1271,14 @@
         # Font settings -------------------------------------------------
 
         if (wordtrack := xml.get("wordTrack")) is not None:
             self.font["space_width"] = dimensions.Dim(
                 float(wordtrack), unit="pcdecim"
             )
 
-        if (kerning := xml.get("KERN")) is not None:
-            self.font["kerning"] = dimensions.Dim(float(kerning), unit="pc")
-
         # Scales --------------------------------------------------------
 
         for att, human in CharacterStyle.scale_xml.items():
             if (scale_att := xml.get(att)) is not None:
                 self.scale[human] = float(scale_att)
 
         # End of parsing ------------------------------------------------
@@ -1253,17 +1302,14 @@
 
         # Font settings -------------------------------------------------
 
         if self.font["space_width"] is not None:
             if self.font["space_width"].value != 1.0:
                 xml.attrib["wordTrack"] = self.font["space_width"].toxmlstr()
 
-        if self.font["kerning"] is not None:
-            xml.attrib["KERN"] = self.font["kerning"].toxmlstr(True)
-
         # Scales --------------------------------------------------------
 
         for att, human in CharacterStyle.scale_xml.items():
             xml.attrib[att] = str(mathc.necessary_float(self.scale[human]))
 
         # ---------------------------------------------------------------
 
@@ -1296,15 +1342,15 @@
             return False
 
         for border in x:
 
             if border.tag in TableBorder.sides_xml.values():
                 tb = TableBorder()
 
-                if (success := tb.fromxml(border)) :
+                if success := tb.fromxml(border):
                     self.borders.append(tb)
 
         return True
 
     def toxml(self) -> ET.Element:
         xml = StyleAbstract.toxml(self)
 
@@ -1327,15 +1373,15 @@
     sides_xml = {
         "left": "TableBorderLeft",
         "right": "TableBorderRight",
         "top": "TableBorderTop",
         "bottom": "TableBorderBottom",
     }
 
-    def __init__(self, side: Optional[str]=False):
+    def __init__(self, side: Optional[str] = False):
         super().__init__()
 
         if side:
             if side.lower() in TableBorder.sides_xml.keys():
                 self.side = side.lower()
             else:
                 self.side = False
@@ -1379,15 +1425,15 @@
         # -------------------------------------------------
 
         for line in xml:
 
             if line.tag == "TableBorderLine":
                 lo = TableBorderLine()
 
-                if (success := lo.fromxml(line)) :
+                if success := lo.fromxml(line):
                     self.lines.append(lo)
 
         return True
 
     def toxml(self) -> ET.Element:
         xml = ET.Element(TableBorder.sides_xml[self.side])
 
@@ -1467,14 +1513,34 @@
     """
     Cell style in SLA (CellStyle)
     """
 
     def __init__(self, doc_parent, default=False, **kwargs):
         TabularStyleAbstract.__init__(self, "cell", doc_parent, default)
 
+    def fromxml(self, xml: ET.Element) -> BoolOrElement:
+        success = TabularStyleAbstract.fromxml(self, xml)
+
+        for case in ["left", "right", "top", "bottom"]:
+            att = xml.get("{}Padding".format(case.capitalize()))
+
+            if att is not None:
+                self.padding[case] = att
+
+        return True
+
+    def toxml(self) -> ET.Element:
+        xml = TabularStyleAbstract.toxml(self)
+
+        for case in ["left", "right", "top", "bottom"]:
+            att_name = "{}Padding".format(case.capitalize())
+            xml.attrib[att_name] = self.padding[case]
+
+        return xml
+
 
 class StyleTab(xmlc.PyScribusElement):
     tab_type_xml = {
         "left": "0",
         "right": "1",
         "period": "2",
         "comma": "3",
@@ -1547,15 +1613,15 @@
             self.name = name
 
         for element in xml:
 
             if element.tag == "SubLine":
                 sl = RuleStyleLine()
 
-                if (success := sl.fromxml(element)) :
+                if success := sl.fromxml(element):
                     self.lines.append(sl)
 
         return True
 
     def toxml(self) -> ET.Element:
         """"""
 
@@ -1638,16 +1704,15 @@
 
     def fromdefault(self) -> NoReturn:
         self.end = "flat"
         self.join = "pointy"
         self.opacity = dimensions.Dim(100, unit="pc")
 
     def fromxml(self, xml: ET.Element) -> bool:
-        """
-        """
+        """ """
 
         if xml.tag != "SubLine":
             return False
 
         # --- Shortcut -----------------------------------------------
 
         if (shortcut := xml.get("Shortcut")) is not None:
@@ -1692,16 +1757,15 @@
                 if code == line_join:
                     self.join = human
                     break
 
         return True
 
     def toxml(self) -> ET.Element:
-        """
-        """
+        """ """
 
         xml = ET.Element("SubLine")
 
         # --- Color and opacity --------------------------------------
 
         if self.color is not None:
             xml.attrib["Color"] = self.color
@@ -1728,15 +1792,17 @@
 
         return xml
 
 
 # Fonctions =============================================================#
 
 
-def fromSLA(filepath: StringOrPath="", slastring: str="") -> Union[dict, bool]:
+def fromSLA(
+    filepath: StringOrPath = "", slastring: str = ""
+) -> Union[dict, bool]:
     """
     Parse a SLA file / string and returns a dictionary of all styles in it.
 
     :type filepath: string
     :param filepath: SLA filepath
     :type slastring: string
     :param slastring: SLA XML string
```

### Comparing `pyscribus-0.2.4/pyscribus/toc.py` & `pyscribus-0.2.5/pyscribus/toc.py`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/pyscribus.egg-info/SOURCES.txt` & `pyscribus-0.2.5/pyscribus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscribus-0.2.4/setup.py` & `pyscribus-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:Utf-8 -*-
 
 import setuptools
 
 with open("../README.pypi.rst", "r") as fh:
     long_description = fh.read()
 
-VERSION = "0.2.4"
+VERSION = "0.2.5"
 DESCRIPTION = "Read, create and update Scribus .sla files."
 
 REQUIRED = ['lxml', 'svg.path']
 
 setuptools.setup(
     name="pyscribus",
     version=VERSION,
```

