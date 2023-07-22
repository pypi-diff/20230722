# Comparing `tmp/rapid_videocr-2.2.4-py3-none-any.whl.zip` & `tmp/rapid_videocr-2.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18371 bytes, number of entries: 11
--rw-r--r--  2.0 unx      174 b- defN 23-Jul-19 06:30 rapid_videocr/__init__.py
--rw-r--r--  2.0 unx    10508 b- defN 23-Jul-19 06:30 rapid_videocr/main.py
--rw-r--r--  2.0 unx    13571 b- defN 23-Jul-19 06:30 rapid_videocr/rapid_videocr.py
--rw-r--r--  2.0 unx     5423 b- defN 23-Jul-19 06:30 rapid_videocr/utils.py
--rw-r--r--  2.0 unx     3025 b- defN 23-Jul-19 06:30 rapid_videocr/video_sub_finder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     8165 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      935 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/RECORD
-11 files, 53323 bytes uncompressed, 16781 bytes compressed:  68.5%
+Zip file size: 18362 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      174 b- defN 23-Jul-22 04:40 rapid_videocr/__init__.py
+-rw-r--r--  2.0 unx    10508 b- defN 23-Jul-22 04:40 rapid_videocr/main.py
+-rw-r--r--  2.0 unx    13571 b- defN 23-Jul-22 04:40 rapid_videocr/rapid_videocr.py
+-rw-r--r--  2.0 unx     5423 b- defN 23-Jul-22 04:40 rapid_videocr/utils.py
+-rw-r--r--  2.0 unx     2996 b- defN 23-Jul-22 04:40 rapid_videocr/video_sub_finder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8165 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      935 b- defN 23-Jul-22 04:40 rapid_videocr-2.2.5.dist-info/RECORD
+11 files, 53294 bytes uncompressed, 16772 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: rapid_videocr/utils.py
 Comment: 
 
 Filename: rapid_videocr/video_sub_finder.py
 Comment: 
 
-Filename: rapid_videocr-2.2.4.dist-info/LICENSE
+Filename: rapid_videocr-2.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: rapid_videocr-2.2.4.dist-info/METADATA
+Filename: rapid_videocr-2.2.5.dist-info/METADATA
 Comment: 
 
-Filename: rapid_videocr-2.2.4.dist-info/WHEEL
+Filename: rapid_videocr-2.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_videocr-2.2.4.dist-info/entry_points.txt
+Filename: rapid_videocr-2.2.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.4.dist-info/top_level.txt
+Filename: rapid_videocr-2.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.4.dist-info/RECORD
+Filename: rapid_videocr-2.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_videocr/video_sub_finder.py

```diff
@@ -66,15 +66,14 @@
             else:
                 run_list.extend([f"--{k}", str(v)])
 
         self.run_list = run_list
 
     def __call__(self, video_path: str, output_dir: str) -> str:
         self.run_list.extend(["--input_video", video_path, "--output_dir", output_dir])
-        print(self.run_list)
 
         try:
             subprocess.run(
                 self.run_list,
                 check=False,
             )
             return output_dir
```

## Comparing `rapid_videocr-2.2.4.dist-info/LICENSE` & `rapid_videocr-2.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapid_videocr-2.2.4.dist-info/METADATA` & `rapid_videocr-2.2.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-videocr
-Version: 2.2.4
+Version: 2.2.5
 Summary: Tool for extracting hard subtitles from videos.
 Home-page: https://github.com/SWHL/RapidVideOCR.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr,videocr,subtitle
 Platform: Any
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.4 Summary: Tool for
+Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.5 Summary: Tool for
 extracting hard subtitles from videos. Home-page: https://github.com/SWHL/
 RapidVideOCR.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: rapidocr,videocr,subtitle Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

## Comparing `rapid_videocr-2.2.4.dist-info/RECORD` & `rapid_videocr-2.2.5.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 rapid_videocr/__init__.py,sha256=eODelyqvjJaceBues-U7fmLAE3JTDkVLUTbcsWivf_Q,174
 rapid_videocr/main.py,sha256=e8Zkkfil3HlXtVX9BxD2qQLh3iuE0_1G-7yNlXlf8_g,10508
 rapid_videocr/rapid_videocr.py,sha256=IL5wXVxPXdWOGmGEAGmCFv2KrtNGJTX6yQIwoRMOtOM,13571
 rapid_videocr/utils.py,sha256=tNYWmQGHVu_yjQisyPed9nVluYOvEiefz_HJ9kbxhso,5423
-rapid_videocr/video_sub_finder.py,sha256=Vqdg3r8uKoTm5IXAys7_szXuumL4LS3kN4Wlvull8kE,3025
-rapid_videocr-2.2.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-rapid_videocr-2.2.4.dist-info/METADATA,sha256=lcpm1qs1mlyNm9l0iXwuKYd7MqGDdui75FyvSFBq0sY,8165
-rapid_videocr-2.2.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-rapid_videocr-2.2.4.dist-info/entry_points.txt,sha256=-keKc5D46wZRqKWIPVZqb5paoQwqLf-OiXKtztK9VqA,59
-rapid_videocr-2.2.4.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
-rapid_videocr-2.2.4.dist-info/RECORD,,
+rapid_videocr/video_sub_finder.py,sha256=FilAtJl0a2e81ZGDpPiL8n-JvYe3vRQrbw2rxLJyjIE,2996
+rapid_videocr-2.2.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+rapid_videocr-2.2.5.dist-info/METADATA,sha256=28C_pWNj0hqvlAp1oDqavWjveqWZx-FU2wNv2ScJssE,8165
+rapid_videocr-2.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+rapid_videocr-2.2.5.dist-info/entry_points.txt,sha256=-keKc5D46wZRqKWIPVZqb5paoQwqLf-OiXKtztK9VqA,59
+rapid_videocr-2.2.5.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
+rapid_videocr-2.2.5.dist-info/RECORD,,
```

