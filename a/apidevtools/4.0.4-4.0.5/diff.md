# Comparing `tmp/apidevtools-4.0.4.tar.gz` & `tmp/apidevtools-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-4.0.4.tar", last modified: Fri Jul  7 19:58:12 2023, max compression
+gzip compressed data, was "apidevtools-4.0.5.tar", last modified: Sat Jul 22 17:23:30 2023, max compression
```

## Comparing `apidevtools-4.0.4.tar` & `apidevtools-4.0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.143501 apidevtools-4.0.4/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-4.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3546 2023-07-07 19:58:12.143501 apidevtools-4.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-4.0.4/README.md
--rw-rw-rw-   0        0        0     2185 2023-07-07 19:57:48.000000 apidevtools-4.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 19:58:12.144502 apidevtools-4.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.100501 apidevtools-4.0.4/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-4.0.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.103501 apidevtools-4.0.4/src/apidevtools/
--rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-4.0.4/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-4.0.4/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.112503 apidevtools-4.0.4/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-4.0.4/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-4.0.4/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-4.0.4/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-4.0.4/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.118502 apidevtools-4.0.4/src/apidevtools/orm/
--rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-4.0.4/src/apidevtools/orm/__init__.py
--rw-rw-rw-   0        0        0     4930 2023-06-30 20:05:23.000000 apidevtools-4.0.4/src/apidevtools/orm/mysql.py
--rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-4.0.4/src/apidevtools/orm/postgresql.py
--rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-4.0.4/src/apidevtools/orm/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.121501 apidevtools-4.0.4/src/apidevtools/orm/types/
--rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-4.0.4/src/apidevtools/orm/types/__init__.py
--rw-rw-rw-   0        0        0     2571 2023-06-30 19:57:03.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_connector.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.128502 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/
--rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/__init__.py
--rw-rw-rw-   0        0        0     2587 2023-06-30 20:00:49.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/_operation.py
--rw-rw-rw-   0        0        0      506 2023-06-30 11:21:27.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/delete.py
--rw-rw-rw-   0        0        0     1180 2023-06-30 11:32:44.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/insert.py
--rw-rw-rw-   0        0        0      336 2023-06-30 11:21:27.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/select.py
--rw-rw-rw-   0        0        0      974 2023-06-30 18:05:45.000000 apidevtools-4.0.4/src/apidevtools/orm/types/_operations/update.py
--rw-rw-rw-   0        0        0      522 2023-06-30 17:03:13.000000 apidevtools-4.0.4/src/apidevtools/orm/types/types.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.131501 apidevtools-4.0.4/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-4.0.4/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-4.0.4/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-4.0.4/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.134501 apidevtools-4.0.4/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.139501 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2074 2023-07-07 19:47:04.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.142501 apidevtools-4.0.4/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-4.0.4/src/apidevtools/simpleorm/types/schema.py
--rw-rw-rw-   0        0        0     1120 2023-06-30 14:42:33.000000 apidevtools-4.0.4/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 19:58:12.108501 apidevtools-4.0.4/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3546 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1582 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-07 19:58:12.000000 apidevtools-4.0.4/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:30.033345 apidevtools-4.0.5/
+-rw-rw-rw-   0        0        0     1093 2023-07-22 14:54:54.000000 apidevtools-4.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3546 2023-07-22 17:23:30.032344 apidevtools-4.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-07-22 14:54:54.000000 apidevtools-4.0.5/README.md
+-rw-rw-rw-   0        0        0     2185 2023-07-22 17:19:59.000000 apidevtools-4.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 17:23:30.033345 apidevtools-4.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:29.861345 apidevtools-4.0.5/src/
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:29.873344 apidevtools-4.0.5/src/apidevtools/
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:29.895344 apidevtools-4.0.5/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-07-22 17:19:59.000000 apidevtools-4.0.5/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1180 2023-07-22 17:14:59.000000 apidevtools-4.0.5/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:29.903344 apidevtools-4.0.5/src/apidevtools/orm/
+-rw-rw-rw-   0        0        0       65 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/orm/__init__.py
+-rw-rw-rw-   0        0        0     4900 2023-07-22 17:01:48.000000 apidevtools-4.0.5/src/apidevtools/orm/mysql.py
+-rw-rw-rw-   0        0        0     4598 2023-07-22 17:00:21.000000 apidevtools-4.0.5/src/apidevtools/orm/postgresql.py
+-rw-rw-rw-   0        0        0     3482 2023-07-22 17:00:37.000000 apidevtools-4.0.5/src/apidevtools/orm/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:29.911345 apidevtools-4.0.5/src/apidevtools/orm/types/
+-rw-rw-rw-   0        0        0      157 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/orm/types/__init__.py
+-rw-rw-rw-   0        0        0     2441 2023-07-22 16:59:40.000000 apidevtools-4.0.5/src/apidevtools/orm/types/_connector.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:29.943344 apidevtools-4.0.5/src/apidevtools/orm/types/_operations/
+-rw-rw-rw-   0        0        0      154 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/orm/types/_operations/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-22 16:59:33.000000 apidevtools-4.0.5/src/apidevtools/orm/types/_operations/_operation.py
+-rw-rw-rw-   0        0        0      506 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/orm/types/_operations/delete.py
+-rw-rw-rw-   0        0        0     1180 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/orm/types/_operations/insert.py
+-rw-rw-rw-   0        0        0      336 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/orm/types/_operations/select.py
+-rw-rw-rw-   0        0        0      974 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/orm/types/_operations/update.py
+-rw-rw-rw-   0        0        0      534 2023-07-22 17:19:59.000000 apidevtools-4.0.5/src/apidevtools/orm/types/types.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:29.957344 apidevtools-4.0.5/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:29.977344 apidevtools-4.0.5/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:30.012343 apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3317 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4781 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4434 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3384 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6732 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2074 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:30.031344 apidevtools-4.0.5/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-07-22 14:54:54.000000 apidevtools-4.0.5/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     2291 2023-07-22 17:14:55.000000 apidevtools-4.0.5/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 17:23:29.892345 apidevtools-4.0.5/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3546 2023-07-22 17:23:29.000000 apidevtools-4.0.5/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1582 2023-07-22 17:23:29.000000 apidevtools-4.0.5/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 17:23:29.000000 apidevtools-4.0.5/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-07-22 17:23:29.000000 apidevtools-4.0.5/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-22 17:23:29.000000 apidevtools-4.0.5/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-4.0.4/LICENSE.txt` & `apidevtools-4.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/PKG-INFO` & `apidevtools-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 4.0.4
+Version: 4.0.5
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-4.0.4/README.md` & `apidevtools-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/pyproject.toml` & `apidevtools-4.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 maintainers = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 description = "All in one tools for API development."
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `apidevtools-4.0.4/src/apidevtools/logman.py` & `apidevtools-4.0.5/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-4.0.5/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/media/imgproc.py` & `apidevtools-4.0.5/src/apidevtools/media/imgproc.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from PIL import ImageDraw as _ImageDraw, ImageFont as _ImageFont
 import numpy as _np
 
 
 def convert(image: bytes | io.BytesIO | PIL.Image.Image) -> PIL.Image.Image:
     """
     Create PIL.Image.Image from bytes or io.BytesIO.
-    Also accepts PIL.Image.Image to simplify usage in and Image classes.
     :param image:
     :return:
     """
     if not isinstance(image, PIL.Image.Image):
         if isinstance(image, Image):
             image = image.bytesio
         elif isinstance(image, bytes):
@@ -41,33 +40,33 @@
     async def url(self) -> str | None:
         from . import telegraph
 
         return await telegraph.upload(self.bytesio)
 
 
 def generate(
-        text: str = Image.text, size: int = 512, fonttf=None,
+        text: str = Image.text, size: int = 512, ttf=None,
         bg_color: tuple[int, int, int] = (0, 0, 0), font_color: tuple[int, int, int] = (255, 255, 255)
 ) -> Image:
     """
     Generate image from apidevtools.image.Image. Supposed to be used as for instance: user
     By default has "N/A" white text on the black background.
     :param text:
     :param size:
-    :param fonttf:
+    :param ttf:
     :param bg_color:
     :param font_color:
     :return:
     """
-    if not fonttf:
+    if not ttf:
         from os import path
 
-        fonttf = path.join(path.dirname(__file__), 'ARIALNB.TTF')
+        ttf = path.join(path.dirname(__file__), 'ARIALNB.TTF')
 
-    font = _ImageFont.truetype(font=fonttf, size=int(size * 0.6))
+    font = _ImageFont.truetype(font=ttf, size=int(size * 0.6))
     img = PIL.Image.new(mode='RGB', size=(size, size), color=bg_color)
     draw = _ImageDraw.Draw(img)
     _, _, width, height = draw.textbbox((0, 0), text, font=font)
     draw.text(xy=((size - width) / 2, (size - height) / 3), text=text, font=font, fill=font_color)
     return Image(img, text)
```

### Comparing `apidevtools-4.0.4/src/apidevtools/media/telegraph.py` & `apidevtools-4.0.5/src/apidevtools/media/telegraph.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import io
 
 import ujson as _json
 
 
 async def upload(file: io.BytesIO, mime: str = 'image/png') -> str | None:
     """
-    Upload media to telegra.ph
+    Upload media to telegra.ph.
     :param file:
     :param mime:
     :return:
     """
     data = _aiohttp.FormData(dict(name='file', value=file.read(), content_type=mime, filename=f"file.{mime.split('/')[1]}"))
     with _contextlib.suppress(_aiohttp.ClientError):
         async with _aiohttp.ClientSession(
@@ -22,14 +22,14 @@
                 sources = await response.json()
                 if not (isinstance(sources, dict) and sources.get('error')):
                     return f"https://telegra.ph{sources[-1]['src']}"
 
 
 async def download(url: str) -> bytes | None:
     """
-    Download media from any source
+    Download media.
     :param url:
     :return:
     """
     async with _aiohttp.ClientSession() as session:
         async with session.get(url) as response:
             return await response.read()
```

### Comparing `apidevtools-4.0.4/src/apidevtools/orm/mysql.py` & `apidevtools-4.0.5/src/apidevtools/orm/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Any, Optional, AsyncGenerator, Callable, Awaitable, Dict
-from functools import cache
 import aiomysql
 
 from .types import Connector, RecordType, Record, Insert, Select, Update, Delete, Query, Schema, Operation
 from .. import logman
 
 
 class MySQL(Connector, Insert, Select, Update, Delete):
@@ -11,15 +10,15 @@
 
     def __init__(self, database: str,
                  host: str = 'localhost', port: int | str = 3306,
                  user: str = 'root', password: str | None = None,
                  logger: logman.Logger = logman.logger):
         self.database: str = database
         self.host: str = host
-        self.port: str | int = port
+        self.port: int = int(port)
         self.user: str = user
         self.password: str | None = password
 
         self.logger: logman.Logger = logger
         self.pool: aiomysql.Pool | None = None
 
     async def create_pool(self) -> bool:
```

### Comparing `apidevtools-4.0.4/src/apidevtools/orm/postgresql.py` & `apidevtools-4.0.5/src/apidevtools/orm/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Any, Optional, AsyncGenerator, Callable, Awaitable
-from functools import cache
 import asyncpg
 
-from .types import Connector, RecordType, Record, Insert, Select, Update, Delete, Schema, Query, Operation
+from .types import Connector, RecordType, Record, Insert, Select, Update, Delete, Schema, Query
 from .. import logman
 
 
 class PostgreSQL(Connector, Insert, Select, Update, Delete):
     _placeholder_count: int = 0
 
     def __init__(self, database: str,
@@ -98,7 +97,12 @@
 
         return to_dict if type is dict else to_schema
 
     @property
     def _placeholder(self):
         self._placeholder_count += 1
         return f'${self._placeholder_count}'
+
+    async def _parameters(self, query: Query, args: tuple[Any, ...], type: RecordType) \
+            -> tuple[str, list[Any, ...], type, Callable[[Any, RecordType], Awaitable[Record]]]:
+        self._placeholder_count = 0
+        return await super()._parameters(query, args, type)
```

### Comparing `apidevtools-4.0.4/src/apidevtools/orm/sqlite.py` & `apidevtools-4.0.5/src/apidevtools/orm/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Any, Optional, AsyncGenerator, Callable, Awaitable
-from functools import cache
 import aiosqlite
 
 from .types import Connector, RecordType, Record, Insert, Select, Update, Delete, Query, Schema
 from .. import logman
 
 
 class SQLite(Connector, Insert, Select, Update, Delete):
```

### Comparing `apidevtools-4.0.4/src/apidevtools/orm/types/_connector.py` & `apidevtools-4.0.5/src/apidevtools/orm/types/_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from contextlib import suppress
-from typing import Any, Optional, AsyncGenerator, Callable, Awaitable, Dict
+from typing import Any, Optional, AsyncGenerator, Callable, Awaitable
 from abc import abstractmethod
 from copy import copy
 
 from .types import RecordType, Record
 from ._operations import Operation
 from ._operations import Query
 
@@ -63,11 +62,9 @@
             -> tuple[str, list[Any, ...], type, Callable[[Any, RecordType], Awaitable[Record]]]:
         if isinstance(query, Operation):
             commands = {self._mapping[key]: self._commands[key] for key, value in self._commands.items()}  # noqa
             query = f"{' '.join([commands[key] for key in sorted(commands.keys())])};"  # noqa
             args = copy(self._args)  # noqa
         self._commands.clear()  # noqa
         self._args.clear()  # noqa
-        self._type = Dict[str, Any]
-        with suppress(AttributeError):
-            self._placeholder_count = 0
+        self._type = dict
         return query, args, type, self._unwrapper(type)
```

### Comparing `apidevtools-4.0.4/src/apidevtools/orm/types/_operations/_operation.py` & `apidevtools-4.0.5/src/apidevtools/orm/types/_operations/_operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Dict
+from typing import Any, Optional
 
 from ..types import RecordType, Record
 
 
 class Operation:
     _mapping: dict[str, int] = {
         'insert': 1, 'select': 1, 'update': 1, 'delete': 1, 'replace': 1,
@@ -13,15 +13,15 @@
         'order': 6,
         'limit': 7,
         'offset': 8,
         'returning': 9,
     }
     _commands: dict[str, str] = {}
     _args: list = []
-    _type: type = Dict[str, Any]
+    _type: type = dict
 
     def fr0m(self, table: str) -> 'Operation':
         c = self._constraint_wrapper  # noqa
         self._commands['from'] = f"FROM {c}{table}{c}"
         return self
 
     # =/LIKE AND/OR
@@ -45,27 +45,27 @@
 
     def offset(self, value: int) -> 'Operation':
         p = self._placeholder  # noqa
         self._args.append(value)
         self._commands['offset'] = f"OFFSET {p}"
         return self
 
-    def returning(self, *columns: str, type: RecordType = Dict[str, Any], auto: bool = False) -> 'Operation':
+    def returning(self, *columns: str, type: RecordType = dict, auto: bool = False) -> 'Operation':
         self._type = type
         if columns:
             self._commands['returning'] = f"RETURNING {', '.join(columns)}"
         if auto and not self._commands.get('returning'):
-            if any([stmt in self._commands.keys() for stmt in ['insert', 'update', 'delete']]):
+            if any(stmt in self._commands.keys() for stmt in ['insert', 'update', 'delete']):
                 self.returning('*')
         return self
 
-    async def all(self, type: RecordType = Dict[str, Any]) -> list[Record]:
+    async def all(self, type: RecordType = dict) -> list[Record]:
         return await self.fetchall(self.returning(auto=True), self._args, type)  # noqa
 
-    async def one(self, type: RecordType = Dict[str, Any]) -> Optional[Record]:
+    async def one(self, type: RecordType = dict) -> Optional[Record]:
         return await self.fetchone(self.returning(auto=True), self._args, type)  # noqa
 
     async def exec(self) -> bool:
         return await self.execute(self, self._args)  # noqa
 
 
 Query: type = type[str, Operation]
```

### Comparing `apidevtools-4.0.4/src/apidevtools/orm/types/_operations/insert.py` & `apidevtools-4.0.5/src/apidevtools/orm/types/_operations/insert.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/orm/types/_operations/update.py` & `apidevtools-4.0.5/src/apidevtools/orm/types/_operations/update.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/orm/types/types.py` & `apidevtools-4.0.5/src/apidevtools/orm/types/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     async def into_db(self) -> 'Schema':
         return self
 
     async def from_db(self) -> 'Schema':
         return self
 
 
-Record = Dict[str, Any] | Schema
-RecordType = type[Record]
+Record: type = Dict[str, Any] | Schema
+RecordType: type = type[Record]
```

### Comparing `apidevtools-4.0.4/src/apidevtools/security/encryptor.py` & `apidevtools-4.0.5/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/security/hasher.py` & `apidevtools-4.0.5/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-4.0.5/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/simpleorm/orm.py` & `apidevtools-4.0.5/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/simpleorm/redis.py` & `apidevtools-4.0.5/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/simpleorm/types/records.py` & `apidevtools-4.0.5/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-4.0.5/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.4/src/apidevtools/utils.py` & `apidevtools-4.0.5/src/apidevtools/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,75 @@
-from typing import Any
+from typing import Awaitable, Any, Callable
+from functools import cache, wraps as _wraps
 import ast as _ast
 import datetime
 
 
 INF: int = 2147483647
 LIMIT: int = 100
 
 
+class _CachedAwaitable:
+    """
+    Allows to make a coroutine reawaitable.
+    """
+    _ResultUnset: str = 'CachedAwaitableResultUnset'
+
+    def __init__(self, awaitable: Awaitable):
+        self.awaitable: Awaitable = awaitable
+        self.result: Any = _CachedAwaitable._ResultUnset
+
+    def __await__(self) -> Any:
+        if self.result == _CachedAwaitable._ResultUnset:
+            self.result = yield from self.awaitable.__await__()
+        return self.result
+
+
+def reawaitable(func: Callable, /):
+    """
+    Makes a coroutine reawaitable.
+    :param func:
+    :return:
+    """
+    @_wraps(func)
+    def wrapper(*args, **kwargs):
+        return _CachedAwaitable(func(*args, **kwargs))
+    return wrapper
+
+
+def aiocache(func: Callable, /):
+    """
+    `functools.cache` for coroutines.
+    :param func:
+    :return:
+    """
+    return cache(reawaitable(func))
+
+
 def now_tz_aware() -> datetime.datetime:
+    """
+    `datetime.now()` with timezone info.
+    :return:
+    """
     return datetime.datetime.now(datetime.timezone.utc)
 
 
 def now_tz_naive() -> datetime.datetime:
+    """
+    `datetime.now()` without timezone info.
+    :return:
+    """
     dt = datetime.datetime.now()
     dt.replace(tzinfo=None)
     return dt
 
 
 def evaluate(value: bytes, convert: bool = True) -> Any:
     """
-    normal ast.literal_eval with a fix of known error together wit adaptation to the apidevtools package
+    Normal `ast.literal_eval` with a fix of known error together wit adaptation to the apidevtools package.
     :param value:
     :param convert:
     :return:
     """
     if not convert:
         return value
     try:
@@ -32,14 +78,14 @@
         return _ast.literal_eval(f'\'{value.decode()}\'')
     except SyntaxError:
         return value.decode()
     except AttributeError:
         return None
 
 
-def is_dict(dict_t: type[dict[Any, Any]]) -> bool:
+def is_dict(type: type[dict[Any, Any]], /) -> bool:
     """
-    compares `dict[Any, Any]` with `dict`, normally done using `is`, but does not work for subscripted types
-    :param dict_t:
-    :return:
+    Compares `dict[Any, Any]` with `dict`, normally done using `is`, but does not work for subscripted types.
+    :param type:
+    :return: True if `dict` type passed, otherwise False.
     """
-    return dict_t.__name__ == 'dict'
+    return type.__name__ == 'dict'
```

### Comparing `apidevtools-4.0.4/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-4.0.5/src/apidevtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 4.0.4
+Version: 4.0.5
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-4.0.4/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-4.0.5/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

