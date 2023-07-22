# Comparing `tmp/doi2pdf-0.1.1.tar.gz` & `tmp/doi2pdf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doi2pdf-0.1.1.tar", max compression
+gzip compressed data, was "doi2pdf-0.1.2.tar", max compression
```

## Comparing `doi2pdf-0.1.1.tar` & `doi2pdf-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1072 2022-10-23 18:14:18.019789 doi2pdf-0.1.1/LICENSE
--rw-r--r--   0        0        0     1075 2022-10-23 19:18:16.152642 doi2pdf-0.1.1/README.md
--rw-r--r--   0        0        0       26 2022-10-23 18:12:34.951386 doi2pdf-0.1.1/doi2pdf/__init__.py
--rw-r--r--   0        0        0     4909 2022-10-23 18:12:35.123387 doi2pdf-0.1.1/doi2pdf/main.py
--rw-r--r--   0        0        0      458 2022-11-02 15:37:43.653107 doi2pdf-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 doi2pdf-0.1.1/setup.py
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 doi2pdf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-10-23 18:14:18.019789 doi2pdf-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1075 2022-10-23 19:18:16.152642 doi2pdf-0.1.2/README.md
+-rw-r--r--   0        0        0       26 2022-10-23 18:12:34.951386 doi2pdf-0.1.2/doi2pdf/__init__.py
+-rw-r--r--   0        0        0     5161 2023-07-22 15:10:05.639816 doi2pdf-0.1.2/doi2pdf/main.py
+-rw-r--r--   0        0        0      458 2023-07-22 15:09:44.099685 doi2pdf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 doi2pdf-0.1.2/PKG-INFO
```

### Comparing `doi2pdf-0.1.1/LICENSE` & `doi2pdf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doi2pdf-0.1.1/README.md` & `doi2pdf-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `doi2pdf-0.1.1/doi2pdf/main.py` & `doi2pdf-0.1.2/doi2pdf/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,24 @@
         raise NotFoundError("Paper not found.")
 
     metadata = api_res.json()
     if metadata.get("results") is not None:
         metadata = metadata["results"][0]
 
     if metadata.get("doi") is not None:
-        doi = metadata["doi"][len("https://doi.org/") :]
+        doi = metadata["doi"][len("https://doi.org/"):]
     title = metadata["display_name"]
     pdf_url = metadata["open_access"]["oa_url"]
     if pdf_url is None:
-        pdf_url = metadata["host_venue"]["url"]
+        if metadata.get("host_venue") is not None:
+            pdf_url = metadata["host_venue"]["url"]
+        elif metadata.get("primary_location") is not None:
+            pdf_url = metadata['primary_location']['landing_page_url']
+        else:
+            raise NotFoundError("PDF URL not found.")
 
     print("Found paper: ", title)
     return doi, title, pdf_url
 
 
 def get_html(url):
     """Returns bs4 object that you can iterate through based on html elements and attributes."""
```

### Comparing `doi2pdf-0.1.1/PKG-INFO` & `doi2pdf-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doi2pdf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Retrieve research paper PDF from DOI, name or URL of the research paper
 License: MIT
 Author: croumegous
 Author-email: cyril.roumegous@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

