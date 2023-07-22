# Comparing `tmp/thelogger-0.3.4-py3-none-any.whl.zip` & `tmp/thelogger-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 15597 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      486 b- defN 23-Jul-21 04:09 thelogger/__init__.py
+Zip file size: 15606 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      514 b- defN 23-Jul-22 00:12 thelogger/__init__.py
 -rw-rw-rw-  2.0 fat     4234 b- defN 22-Feb-20 09:05 thelogger/__logger.py
 -rw-rw-rw-  2.0 fat      214 b- defN 23-Apr-27 17:46 thelogger/__ver.py
 -rw-rw-rw-  2.0 fat     1049 b- defN 23-Jun-17 05:10 thelogger/dirty_timer.py
 -rw-rw-rw-  2.0 fat     4390 b- defN 23-Jul-22 00:09 thelogger/sys_meta.py
 -rw-rw-rw-  2.0 fat      140 b- defN 22-Feb-20 09:05 thelogger/notify/__init__.py
 -rw-rw-rw-  2.0 fat     3611 b- defN 22-Feb-20 09:49 thelogger/notify/decorator.py
 -rw-rw-rw-  2.0 fat     6990 b- defN 23-Feb-28 14:35 thelogger/notify/exec_func.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-22 00:11 thelogger-0.3.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6692 b- defN 23-Jul-22 00:11 thelogger-0.3.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-22 00:11 thelogger-0.3.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-22 00:11 thelogger-0.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1041 b- defN 23-Jul-22 00:11 thelogger-0.3.4.dist-info/RECORD
-13 files, 40507 bytes uncompressed, 13867 bytes compressed:  65.8%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6692 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1041 b- defN 23-Jul-22 00:13 thelogger-0.3.5.dist-info/RECORD
+13 files, 40535 bytes uncompressed, 13876 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: thelogger/notify/decorator.py
 Comment: 
 
 Filename: thelogger/notify/exec_func.py
 Comment: 
 
-Filename: thelogger-0.3.4.dist-info/LICENSE
+Filename: thelogger-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: thelogger-0.3.4.dist-info/METADATA
+Filename: thelogger-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: thelogger-0.3.4.dist-info/WHEEL
+Filename: thelogger-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: thelogger-0.3.4.dist-info/top_level.txt
+Filename: thelogger-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: thelogger-0.3.4.dist-info/RECORD
+Filename: thelogger-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## thelogger/__init__.py

```diff
@@ -10,14 +10,15 @@
 from .__logger import logger, log, lg
 from .notify import notify
 from .dirty_timer import beg, end, timer
 from .sys_meta import (
     get_cpu_model,
     get_machine_info,
     get_resource_usage,
+    get_imported_pkg_vers,
     get_env_info,
     sys_info
     )
 
 from .__ver import __version__
 
 try:
```

## Comparing `thelogger-0.3.4.dist-info/LICENSE` & `thelogger-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `thelogger-0.3.4.dist-info/METADATA` & `thelogger-0.3.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thelogger
-Version: 0.3.4
+Version: 0.3.5
 Summary: Easy logging, timing and email notifications of code execution.
 Home-page: https://github.com/tom1919/TheLogger
 Author: Tom1919
 Author-email: py.notify1@gmail.com
 License: Apache 2.0
 Keywords: log,logging,logger,email,timimg,notification
 Platform: UNKNOWN
```

## Comparing `thelogger-0.3.4.dist-info/RECORD` & `thelogger-0.3.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-thelogger/__init__.py,sha256=dhhY16P4WEGhomsCWhVx3MWMdQBnHbydtr8V3vVC-ZE,486
+thelogger/__init__.py,sha256=_I66PepW9Wf-esyHGfSXp_FdzdrI1i7RweTEWBMLMgo,514
 thelogger/__logger.py,sha256=JTyQbecMYpi1n7zKoVe9sohS6tTy87Bx2UnCDHb4-N4,4234
 thelogger/__ver.py,sha256=v27jnS60TKa54IbFVzSTknhDiKMS4J3KCuFTOffZqRU,214
 thelogger/dirty_timer.py,sha256=NxlxGSQ09Q3BRRKYlIRgFahGFgvAn78a9xb-xrNKkXc,1049
 thelogger/sys_meta.py,sha256=_sjOQqeeIPDBX6YhX_LkYsOy060BMCCOxPt2qcC4Y80,4390
 thelogger/notify/__init__.py,sha256=X0cVRenLKIbnOoapwPN9KJvtwXaHycKVb-ZTZ8tmuWQ,140
 thelogger/notify/decorator.py,sha256=kiiVpcCayMsdtGtiOtswHaa_v8OzSQjXnKnoSvrt0Uk,3611
 thelogger/notify/exec_func.py,sha256=uN4mbHtdmG4-djWnEzomVeFfbOJ6jHqlNmydolX5QwU,6990
-thelogger-0.3.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-thelogger-0.3.4.dist-info/METADATA,sha256=HsKsoWw3ZGMSJj47xX_MHRlVgF7nyXRwt8P5eunPiA4,6692
-thelogger-0.3.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-thelogger-0.3.4.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
-thelogger-0.3.4.dist-info/RECORD,,
+thelogger-0.3.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+thelogger-0.3.5.dist-info/METADATA,sha256=pX7isIrFv2qonNpVBNI7vrSVUbtT0ZHBi2pqSPkquSQ,6692
+thelogger-0.3.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+thelogger-0.3.5.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
+thelogger-0.3.5.dist-info/RECORD,,
```

