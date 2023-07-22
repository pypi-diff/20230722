# Comparing `tmp/aksharify-0.1.3.tar.gz` & `tmp/aksharify-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-0.1.3.tar", max compression
+gzip compressed data, was "aksharify-0.1.4.tar", max compression
```

## Comparing `aksharify-0.1.3.tar` & `aksharify-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.3/LICENSE.md
--rw-r--r--   0        0        0      674 2023-07-22 06:28:21.212558 aksharify-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.3/README.md
--rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.3/src/aksharify/__init__.py
--rw-r--r--   0        0        0     3515 2023-07-22 06:27:52.686603 aksharify-0.1.3/src/aksharify/aksharify.py
--rw-r--r--   0        0        0     5274 2023-07-20 14:19:37.279133 aksharify-0.1.3/src/aksharify/distributions.py
--rw-r--r--   0        0        0     1556 2023-07-18 11:04:22.323563 aksharify-0.1.3/src/aksharify/image.py
--rw-r--r--   0        0        0     4711 2023-07-18 04:15:13.427078 aksharify-0.1.3/src/aksharify/outputs.py
--rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 aksharify-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      674 2023-07-22 07:25:07.132234 aksharify-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.4/README.md
+-rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.4/src/aksharify/__init__.py
+-rw-r--r--   0        0        0     3529 2023-07-22 07:23:50.694034 aksharify-0.1.4/src/aksharify/aksharify.py
+-rw-r--r--   0        0        0     5274 2023-07-20 14:19:37.279133 aksharify-0.1.4/src/aksharify/distributions.py
+-rw-r--r--   0        0        0     1556 2023-07-18 11:04:22.323563 aksharify-0.1.4/src/aksharify/image.py
+-rw-r--r--   0        0        0     4711 2023-07-18 04:15:13.427078 aksharify-0.1.4/src/aksharify/outputs.py
+-rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 aksharify-0.1.4/PKG-INFO
```

### Comparing `aksharify-0.1.3/LICENSE.md` & `aksharify-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.3/pyproject.toml` & `aksharify-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aksharify"
-version = "0.1.3"
+version = "0.1.4"
 description = "Ascii Art + Emoji Art python Package"
 authors = ["Prime Patel <primespatel@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aksharify", from = "src"}]
 license = "MIT"
 homepage = "https://primepatel.github.io/aksharify/"
 repository = "https://github.com/primepatel/aksharify"
```

### Comparing `aksharify-0.1.3/README.md` & `aksharify-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.3/src/aksharify/aksharify.py` & `aksharify-0.1.4/src/aksharify/aksharify.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,22 +33,23 @@
         if x<self.image.w and y<self.image.h:
             self.matrix[y][x] = char
         else:
             raise IndexError
 
     def replace_chars(self, chars:str, x:int, y:int) -> None:
         x, y = abs(x), abs(y)
-        if x>self.image.w or y>self.image.h:
+        w, h = self.image.bwimg.shape[1], self.image.bwimg.shape[0]
+        if x>w or y>h:
             raise IndexError
-        if self.image.w - x >= len(chars):
+        if w - x >= len(chars):
             for i in range(x, x + len(chars)):
                 self.replace_char(chars[i-x], i, y)
         else:
-            self.replace_chars(chars[:self.image.w-x], x, y)
-            self.replace_chars(chars[self.image.w-x:], 0, y+1)
+            self.replace_chars(chars[:w-x], x, y)
+            self.replace_chars(chars[w-x:], 0, y+1)
 
     def txt_output(self, fname:str) -> None:
         text = ""
         for line_no in range(self.image.bwimg.shape[0]):
             text += "".join(self.matrix[line_no]) + "\n"
         with open(fname + ".txt", "w") as file:
             file.write(text)
```

### Comparing `aksharify-0.1.3/src/aksharify/distributions.py` & `aksharify-0.1.4/src/aksharify/distributions.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.3/src/aksharify/image.py` & `aksharify-0.1.4/src/aksharify/image.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.3/src/aksharify/outputs.py` & `aksharify-0.1.4/src/aksharify/outputs.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.3/PKG-INFO` & `aksharify-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ascii Art + Emoji Art python Package
 Home-page: https://primepatel.github.io/aksharify/
 License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
```

