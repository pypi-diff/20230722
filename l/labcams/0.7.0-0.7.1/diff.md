# Comparing `tmp/labcams-0.7.0-py3-none-any.whl.zip` & `tmp/labcams-0.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 92476 bytes, number of entries: 23
+Zip file size: 92477 bytes, number of entries: 23
 -rw-rw-r--  2.0 unx      832 b- defN 22-Jun-16 04:03 labcams/__init__.py
 -rw-rw-r--  2.0 unx    13689 b- defN 23-Jul-12 17:13 labcams/avt.py
 -rw-rw-r--  2.0 unx     6684 b- defN 23-Jul-12 17:13 labcams/basler.py
 -rw-rw-r--  2.0 unx     8117 b- defN 22-Jun-16 04:03 labcams/cam_stim_trigger.py
 -rw-rw-r--  2.0 unx    35578 b- defN 23-Jul-18 01:12 labcams/cams.py
 -rw-rw-r--  2.0 unx    23524 b- defN 23-Jul-18 01:12 labcams/gui.py
 -rw-rw-r--  2.0 unx    49319 b- defN 23-Jul-18 01:12 labcams/io.py
@@ -12,14 +12,14 @@
 -rw-rw-r--  2.0 unx    30459 b- defN 23-Jul-12 17:13 labcams/pointgreycam.py
 -rw-rw-r--  2.0 unx     6310 b- defN 23-Jul-12 17:13 labcams/pvcam.py
 -rw-rw-r--  2.0 unx     6872 b- defN 23-Jul-12 17:13 labcams/qimaging.py
 -rw-rw-r--  2.0 unx    62774 b- defN 22-Apr-23 23:36 labcams/qimaging_dll.py
 -rw-rw-r--  2.0 unx    10107 b- defN 23-Jul-12 17:13 labcams/utils.py
 -rw-rw-r--  2.0 unx    47564 b- defN 23-Jul-18 01:12 labcams/widgets.py
 -rw-rw-r--  2.0 unx     5561 b- defN 23-Jul-12 17:13 labcams/ximeacam.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Jul-18 01:14 labcams-0.7.0.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     2285 b- defN 23-Jul-18 01:14 labcams-0.7.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-18 01:14 labcams-0.7.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 23-Jul-18 01:14 labcams-0.7.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jul-18 01:14 labcams-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1767 b- defN 23-Jul-18 01:14 labcams-0.7.0.dist-info/RECORD
-23 files, 366424 bytes uncompressed, 89690 bytes compressed:  75.5%
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Jul-22 02:54 labcams-0.7.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     2285 b- defN 23-Jul-22 02:54 labcams-0.7.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-22 02:54 labcams-0.7.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 23-Jul-22 02:54 labcams-0.7.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-22 02:54 labcams-0.7.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1767 b- defN 23-Jul-22 02:54 labcams-0.7.1.dist-info/RECORD
+23 files, 366424 bytes uncompressed, 89691 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -45,26 +45,26 @@
 
 Filename: labcams/widgets.py
 Comment: 
 
 Filename: labcams/ximeacam.py
 Comment: 
 
-Filename: labcams-0.7.0.dist-info/LICENSE.txt
+Filename: labcams-0.7.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: labcams-0.7.0.dist-info/METADATA
+Filename: labcams-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: labcams-0.7.0.dist-info/WHEEL
+Filename: labcams-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: labcams-0.7.0.dist-info/entry_points.txt
+Filename: labcams-0.7.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: labcams-0.7.0.dist-info/top_level.txt
+Filename: labcams-0.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: labcams-0.7.0.dist-info/RECORD
+Filename: labcams-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `labcams-0.7.0.dist-info/LICENSE.txt` & `labcams-0.7.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `labcams-0.7.0.dist-info/METADATA` & `labcams-0.7.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcams
-Version: 0.7.0
+Version: 0.7.1
 Summary: Multicamera video acquisition,online compression and automation
 Home-page: https://github.com/jcouto/labcams
 Author: Joao Couto
 Author-email: jpcouto@gmail.com
 License: GPL
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

## Comparing `labcams-0.7.0.dist-info/RECORD` & `labcams-0.7.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 labcams/pointgreycam.py,sha256=9F7UESNw0MxCRyO79dN8VoDzgmtw9PdIVmbMP3WShKM,30459
 labcams/pvcam.py,sha256=uJ8DWERqYAjDlFmiJTYdv8XIEMnsl4qfofJP2VGuPp0,6310
 labcams/qimaging.py,sha256=1Dwlg76AfOyeHyEndYfZ7AnnrYwnvflDW95QDpzp5HA,6872
 labcams/qimaging_dll.py,sha256=pGqfRq15BWLTMLe9pv-JcObz1yPwocnj-FdqXcw-T1A,62774
 labcams/utils.py,sha256=xpOb8joXHoMfUdhpOyT2nwVt7U3mxVnVlYEhi3JIbmU,10107
 labcams/widgets.py,sha256=5GSlMwVz8eBbnMjcR5DG67i525q69DX24s3ERh06m_w,47564
 labcams/ximeacam.py,sha256=hq9l2logmtrvFWRqaMVZmZ1zvOA_NRsxKsQrcopspU4,5561
-labcams-0.7.0.dist-info/LICENSE.txt,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-labcams-0.7.0.dist-info/METADATA,sha256=Gw7hyoX91RSwFzwOfs8z_7gdfRI2HIYwjeS1Cb0v8mA,2285
-labcams-0.7.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-labcams-0.7.0.dist-info/entry_points.txt,sha256=IXmap1X2QfMmEsUpJi0Z9V-zvkG0urpX9I3Ct_jwfKM,46
-labcams-0.7.0.dist-info/top_level.txt,sha256=id3KInKuvCHG2ofzEp-zvMNc843ixQ407p4RP89IsZ8,8
-labcams-0.7.0.dist-info/RECORD,,
+labcams-0.7.1.dist-info/LICENSE.txt,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+labcams-0.7.1.dist-info/METADATA,sha256=coga5LE7Rw4OCpcKwBEM-587WXQW-wgA_mscrrvq9mI,2285
+labcams-0.7.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+labcams-0.7.1.dist-info/entry_points.txt,sha256=IXmap1X2QfMmEsUpJi0Z9V-zvkG0urpX9I3Ct_jwfKM,46
+labcams-0.7.1.dist-info/top_level.txt,sha256=id3KInKuvCHG2ofzEp-zvMNc843ixQ407p4RP89IsZ8,8
+labcams-0.7.1.dist-info/RECORD,,
```

