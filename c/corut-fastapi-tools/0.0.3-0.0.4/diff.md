# Comparing `tmp/corut_fastapi_tools-0.0.3-py3-none-any.whl.zip` & `tmp/corut_fastapi_tools-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5074 bytes, number of entries: 7
+Zip file size: 5091 bytes, number of entries: 7
 -rw-r--r--  2.0 unx     1161 b- defN 23-Apr-28 19:35 corut_fastapi_tools/__init__.py
 -rw-r--r--  2.0 unx     3119 b- defN 23-Jan-18 07:24 corut_fastapi_tools/_content_types.py
--rw-rw-r--  2.0 unx     1093 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2768 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      628 b- defN 23-Apr-28 19:45 corut_fastapi_tools-0.0.3.dist-info/RECORD
-7 files, 8881 bytes uncompressed, 3946 bytes compressed:  55.6%
+-rw-rw-r--  2.0 unx     1093 b- defN 23-Jul-22 09:34 corut_fastapi_tools-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2799 b- defN 23-Jul-22 09:34 corut_fastapi_tools-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 09:34 corut_fastapi_tools-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-22 09:34 corut_fastapi_tools-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      628 b- defN 23-Jul-22 09:34 corut_fastapi_tools-0.0.4.dist-info/RECORD
+7 files, 8912 bytes uncompressed, 3963 bytes compressed:  55.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: corut_fastapi_tools/__init__.py
 Comment: 
 
 Filename: corut_fastapi_tools/_content_types.py
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.3.dist-info/LICENSE
+Filename: corut_fastapi_tools-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.3.dist-info/METADATA
+Filename: corut_fastapi_tools-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.3.dist-info/WHEEL
+Filename: corut_fastapi_tools-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.3.dist-info/top_level.txt
+Filename: corut_fastapi_tools-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: corut_fastapi_tools-0.0.3.dist-info/RECORD
+Filename: corut_fastapi_tools-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `corut_fastapi_tools-0.0.3.dist-info/LICENSE` & `corut_fastapi_tools-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `corut_fastapi_tools-0.0.3.dist-info/METADATA` & `corut_fastapi_tools-0.0.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corut-fastapi-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Includes facilitating plugins for Fastapi
 Home-page: https://pypi.org/project/corut_fastapi_tools
 Author: ibrahim CÖRÜT
 Author-email: ibrhmcorut@gmail.com
 License: MIT License
 Project-URL: Documentation, https://www.ibrahimcorut.com/en/projects/pypi-corut_fastapi_tools
 Project-URL: Source Code, https://www.ibrahimcorut.com/en/projects/pypi-corut_fastapi_tools
@@ -20,15 +20,15 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiohttp-retry
 Requires-Dist: asyncpg
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: databases
-Requires-Dist: fastapi
+Requires-Dist: fastapi (==0.99.1)
 Requires-Dist: hypercorn
 Requires-Dist: importlib-metadata
 Requires-Dist: openai
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: psycopg2-binary
@@ -37,14 +37,15 @@
 Requires-Dist: pytest
 Requires-Dist: pytest-html
 Requires-Dist: python-multipart
 Requires-Dist: requests
 Requires-Dist: sqlalchemy
 Requires-Dist: starlette
 Requires-Dist: uvicorn
+Requires-Dist: pytz
 
 
  ## corut_fastapi_tools
 
 It is aimed to get rid of repetitive lines of code by integrating tools 
 that use multiple APIs for FastApi and facilitate repetitive operations.
```

## Comparing `corut_fastapi_tools-0.0.3.dist-info/RECORD` & `corut_fastapi_tools-0.0.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 corut_fastapi_tools/__init__.py,sha256=xdCv619UKPzAUSbu9B2B-HYH0xlWNBpSAx7m53JkzCc,1161
 corut_fastapi_tools/_content_types.py,sha256=keaB5aMigrtHWzqs10jqmyaLLkHwKOUBOrcpudymxL8,3119
-corut_fastapi_tools-0.0.3.dist-info/LICENSE,sha256=ZX_WMQQ5bWI_phl-V9VjROO1ua50MjHTKqDqB906AxQ,1093
-corut_fastapi_tools-0.0.3.dist-info/METADATA,sha256=U4rwsvegCKLJZaPN5_FFnbWP9z53mX1WWfhbvRtGXIk,2768
-corut_fastapi_tools-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-corut_fastapi_tools-0.0.3.dist-info/top_level.txt,sha256=SyS-IR2c9xSLfq0UcEtOgMUrQiWlpGaCY1dd-1dM5Xo,20
-corut_fastapi_tools-0.0.3.dist-info/RECORD,,
+corut_fastapi_tools-0.0.4.dist-info/LICENSE,sha256=ZX_WMQQ5bWI_phl-V9VjROO1ua50MjHTKqDqB906AxQ,1093
+corut_fastapi_tools-0.0.4.dist-info/METADATA,sha256=B8cjgk-442oa_qCyBUMTtp8gSgNzUJOjRrsqtCpvlUE,2799
+corut_fastapi_tools-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+corut_fastapi_tools-0.0.4.dist-info/top_level.txt,sha256=SyS-IR2c9xSLfq0UcEtOgMUrQiWlpGaCY1dd-1dM5Xo,20
+corut_fastapi_tools-0.0.4.dist-info/RECORD,,
```

