# Comparing `tmp/linovelib2epub-0.1.2-py3-none-any.whl.zip` & `tmp/linovelib2epub-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 37729 bytes, number of entries: 18
+Zip file size: 37728 bytes, number of entries: 18
 -rw-r--r--  2.0 fat       23 b- defN 20-Feb-02 00:00 linovelib2epub/__about__.py
 -rw-r--r--  2.0 fat       62 b- defN 20-Feb-02 00:00 linovelib2epub/__init__.py
 -rw-r--r--  2.0 fat      120 b- defN 20-Feb-02 00:00 linovelib2epub/exceptions.py
 -rw-r--r--  2.0 fat    17331 b- defN 20-Feb-02 00:00 linovelib2epub/linovel.py
--rw-r--r--  2.0 fat     2799 b- defN 20-Feb-02 00:00 linovelib2epub/logger.py
+-rw-r--r--  2.0 fat     2700 b- defN 20-Feb-02 00:00 linovelib2epub/logger.py
 -rw-r--r--  2.0 fat     3349 b- defN 20-Feb-02 00:00 linovelib2epub/models.py
 -rw-r--r--  2.0 fat     1246 b- defN 20-Feb-02 00:00 linovelib2epub/settings.py
 -rw-r--r--  2.0 fat     3522 b- defN 20-Feb-02 00:00 linovelib2epub/utils.py
 -rw-r--r--  2.0 fat      331 b- defN 20-Feb-02 00:00 linovelib2epub/spider/__init__.py
 -rw-r--r--  2.0 fat     9144 b- defN 20-Feb-02 00:00 linovelib2epub/spider/base_spider.py
 -rw-r--r--  2.0 fat    23200 b- defN 20-Feb-02 00:00 linovelib2epub/spider/linovelib_mobile_spider.py
 -rw-r--r--  2.0 fat      812 b- defN 20-Feb-02 00:00 linovelib2epub/styles/chapter.css
 -rw-r--r--  2.0 fat      295 b- defN 20-Feb-02 00:00 linovelib2epub/styles/cover.css
 -rw-r--r--  2.0 fat      368 b- defN 20-Feb-02 00:00 linovelib2epub/styles/nav.css
-?rw-r--r--  2.0 fat    11153 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.2.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 fat    35176 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat     1537 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.2.dist-info/RECORD
-18 files, 110555 bytes uncompressed, 35195 bytes compressed:  68.2%
+?rw-r--r--  2.0 fat    11231 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.3.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 fat    35176 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat     1537 b- defN 20-Feb-02 00:00 linovelib2epub-0.1.3.dist-info/RECORD
+18 files, 110534 bytes uncompressed, 35194 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: linovelib2epub/styles/cover.css
 Comment: 
 
 Filename: linovelib2epub/styles/nav.css
 Comment: 
 
-Filename: linovelib2epub-0.1.2.dist-info/METADATA
+Filename: linovelib2epub-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: linovelib2epub-0.1.2.dist-info/WHEEL
+Filename: linovelib2epub-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: linovelib2epub-0.1.2.dist-info/licenses/LICENSE
+Filename: linovelib2epub-0.1.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: linovelib2epub-0.1.2.dist-info/RECORD
+Filename: linovelib2epub-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## linovelib2epub/__about__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
```

## linovelib2epub/logger.py

```diff
@@ -1,20 +1,16 @@
-import logging
 import os
-import sys
-import traceback
 from logging import (CRITICAL, DEBUG, ERROR, INFO, WARN, WARNING, FileHandler,
-                     Formatter, StreamHandler, getLogger)
-from os import path
+                     Formatter, getLogger)
 from time import localtime, strftime
 from typing import Optional
 
 from rich.logging import RichHandler
 
-DEFAULT_LOG_FOLDER = os.path.join(os.path.dirname(os.getcwd()), 'logs')
+DEFAULT_LOG_FOLDER = os.path.join(os.getcwd(), 'logs')
 
 
 class Logger:
     LEVEL_MAP = {
         'INFO': INFO,
         'DEBUG': DEBUG,
         'WARN': WARN,
```

## Comparing `linovelib2epub-0.1.2.dist-info/METADATA` & `linovelib2epub-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linovelib2epub
-Version: 0.1.2
+Version: 0.1.3
 Summary: Craw light novel from [哔哩轻小说(linovelib)](https://w.linovelib.com/) and convert to epub.
 Project-URL: Homepage, https://github.com/wdpm/linovelib2epub
 Project-URL: Source, https://github.com/wdpm/linovelib2epub
 Project-URL: Tracker, https://github.com/wdpm/linovelib2epub/issues
 Author-email: wdpm <1137299673@qq.com>
 License-File: LICENSE
 Keywords: ebook,epub,library,light novel,哔哩轻小说
@@ -125,14 +125,18 @@
 ```
 
 ### install from pypi
 1. Install this package from pypi:
 ```
 pip install linovelib2epub
 ```
+Or update to the latest version:
+```
+pip install linovelib2epub --upgrade
+```
 2. create a python file and edit the content as follows:
 ```python
 from linovelib2epub.linovel import Linovelib2Epub
 
 # warning!: must run within __main__ module guard due to process spawn issue.
 if __name__ == '__main__':
     linovelib_epub = Linovelib2Epub(book_id=3279)
```

## Comparing `linovelib2epub-0.1.2.dist-info/licenses/LICENSE` & `linovelib2epub-0.1.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `linovelib2epub-0.1.2.dist-info/RECORD` & `linovelib2epub-0.1.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-linovelib2epub/__about__.py,sha256=TWY2HHBr7soKzDojVTmRRRQj8LWtiK2CcaOJolf0kU0,23
+linovelib2epub/__about__.py,sha256=0PD6QxIuSaaldK8FubSi9rwJiuvflX7C1EqT2hLSBjs,23
 linovelib2epub/__init__.py,sha256=8CCbmojIlWmlU7B-linDBDGXcs3FOCtsl4-Ojqvu0yU,62
 linovelib2epub/exceptions.py,sha256=lFhHpmN0tJFrNGLg4Le5TxrNzuRxsQN8atGnsJ8FMdg,120
 linovelib2epub/linovel.py,sha256=Vynuc0MGUpFsTRvQHXD-OO4iIFLddfTIeDySId4sjjY,17331
-linovelib2epub/logger.py,sha256=jJ9XRppJw_XnK7miTacLe51zdxQU4g6Ad8EyhH_GYo0,2799
+linovelib2epub/logger.py,sha256=wRGbnWyCd0vhdnquJHJ0EIYGzN183Lbp69wF6TzAcDw,2700
 linovelib2epub/models.py,sha256=roTMd2xK7edAtYhoXMZfLhHOh1SFKyiebgmyrHyc3so,3349
 linovelib2epub/settings.py,sha256=joZ6dJ0SAY_tKlnYAnrtmbs0EJCUH_x7QEt4XxGw3ts,1246
 linovelib2epub/utils.py,sha256=dD50_YpNMXg3kCyrf8UQXl4wAdO1-Y_55q9K1AcBun0,3522
 linovelib2epub/spider/__init__.py,sha256=LAW6YwlEprVWfQ60XiQGdt38MacuKRlkbfeY-kYp57I,331
 linovelib2epub/spider/base_spider.py,sha256=pUrDsTJFRKLcVKdILBHufppTYsWGLl50N5D_rBcLolA,9144
 linovelib2epub/spider/linovelib_mobile_spider.py,sha256=r4UuRkRCzXwo1ACBZI-JW_o7os5mDXrIL4YiZ1sFTUI,23200
 linovelib2epub/styles/chapter.css,sha256=Y9B1m4Az_POEmBCmTi7-VRZtZ2rKtAJiUXQgXfkhD6I,812
 linovelib2epub/styles/cover.css,sha256=XNLJieS0z6pM-N7JmzlIbPB8zHDJTlYzj8up5gRSlng,295
 linovelib2epub/styles/nav.css,sha256=lYOD7xRWIQeTFPxZb3DusjhhssYGIBICjokDjiQW-lo,368
-linovelib2epub-0.1.2.dist-info/METADATA,sha256=mhRIa0xRPKMSwwM4BAxmifTFmMZ_GRYtMKGDahl9d8s,11153
-linovelib2epub-0.1.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-linovelib2epub-0.1.2.dist-info/licenses/LICENSE,sha256=kn2aD5kGS5Dv7OCGNVznr_sf1puJqE85rLQaqVwZFG8,35176
-linovelib2epub-0.1.2.dist-info/RECORD,,
+linovelib2epub-0.1.3.dist-info/METADATA,sha256=CSkFt2xfmvLyvfkFSTU1OHxpfx-zpbhbvwerunliBsY,11231
+linovelib2epub-0.1.3.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+linovelib2epub-0.1.3.dist-info/licenses/LICENSE,sha256=kn2aD5kGS5Dv7OCGNVznr_sf1puJqE85rLQaqVwZFG8,35176
+linovelib2epub-0.1.3.dist-info/RECORD,,
```

