# Comparing `tmp/ptulsconv-2.0.0.tar.gz` & `tmp/ptulsconv-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptulsconv-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ptulsconv-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ptulsconv-2.0.0.tar` & `ptulsconv-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-07-21 21:29:59.710680 ptulsconv-2.0.0/LICENSE
--rw-r--r--   0        0        0     1241 2023-07-21 21:29:59.710680 ptulsconv-2.0.0/README.md
--rw-r--r--   0        0        0      225 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/__init__.py
--rw-r--r--   0        0        0     4074 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/__main__.py
--rw-r--r--   0        0        0     4297 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/broadcast_timecode.py
--rw-r--r--   0        0        0     9317 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/commands.py
--rw-r--r--   0        0        0       68 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/docparser/__init__.py
--rw-r--r--   0        0        0     4641 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/docparser/adr_entity.py
--rw-r--r--   0        0        0     5835 2023-07-21 21:29:59.718680 ptulsconv-2.0.0/ptulsconv/docparser/doc_entity.py
--rw-r--r--   0        0        0       36 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/generic_entity.py
--rw-r--r--   0        0        0    10371 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/pt_doc_parser.py
--rw-r--r--   0        0        0     7997 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/tag_compiler.py
--rw-r--r--   0        0        0     2948 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/tag_mapping.py
--rw-r--r--   0        0        0     2872 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/docparser/tagged_string_parser_visitor.py
--rw-r--r--   0        0        0      754 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/footage.py
--rw-r--r--   0        0        0      477 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/movie_export.py
--rw-r--r--   0        0        0    12703 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/__init__.py
--rw-r--r--   0        0        0     2102 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/continuity.py
--rw-r--r--   0        0        0    11362 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/line_count.py
--rw-r--r--   0        0        0       91 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/recordist_log.py
--rw-r--r--   0        0        0     5826 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/summary_log.py
--rw-r--r--   0        0        0    10929 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/supervisor_1pg.py
--rw-r--r--   0        0        0     3188 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/pdf/talent_sides.py
--rw-r--r--   0        0        0     2244 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/reporting.py
--rw-r--r--   0        0        0     2869 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/validations.py
--rw-r--r--   0        0        0     5909 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/xml/common.py
--rw-r--r--   0        0        0     3275 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/xslt/AvidMarkers.xsl
--rw-r--r--   0        0        0     1529 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/ptulsconv/xslt/SRT.xsl
--rw-r--r--   0        0        0     1336 2023-07-21 21:29:59.722680 ptulsconv-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 ptulsconv-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-22 20:04:34.183446 ptulsconv-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1246 2023-07-22 20:04:34.183446 ptulsconv-2.0.1/README.md
+-rw-r--r--   0        0        0      225 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/__init__.py
+-rw-r--r--   0        0        0     4074 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/__main__.py
+-rw-r--r--   0        0        0     4297 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/broadcast_timecode.py
+-rw-r--r--   0        0        0     9319 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/commands.py
+-rw-r--r--   0        0        0       68 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/__init__.py
+-rw-r--r--   0        0        0     4641 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/adr_entity.py
+-rw-r--r--   0        0        0     5835 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/doc_entity.py
+-rw-r--r--   0        0        0       36 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/generic_entity.py
+-rw-r--r--   0        0        0    10371 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/pt_doc_parser.py
+-rw-r--r--   0        0        0     7997 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/tag_compiler.py
+-rw-r--r--   0        0        0     2948 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/tag_mapping.py
+-rw-r--r--   0        0        0     2872 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/docparser/tagged_string_parser_visitor.py
+-rw-r--r--   0        0        0      754 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/footage.py
+-rw-r--r--   0        0        0      477 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/movie_export.py
+-rw-r--r--   0        0        0    12703 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/__init__.py
+-rw-r--r--   0        0        0     2102 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/continuity.py
+-rw-r--r--   0        0        0    11362 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/line_count.py
+-rw-r--r--   0        0        0       91 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/recordist_log.py
+-rw-r--r--   0        0        0     5826 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/summary_log.py
+-rw-r--r--   0        0        0    10929 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/supervisor_1pg.py
+-rw-r--r--   0        0        0     3188 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/pdf/talent_sides.py
+-rw-r--r--   0        0        0     2244 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/reporting.py
+-rw-r--r--   0        0        0     2869 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/validations.py
+-rw-r--r--   0        0        0     5909 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/xml/common.py
+-rw-r--r--   0        0        0     3275 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/xslt/AvidMarkers.xsl
+-rw-r--r--   0        0        0     1529 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/ptulsconv/xslt/SRT.xsl
+-rw-r--r--   0        0        0     1336 2023-07-22 20:04:34.199447 ptulsconv-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 ptulsconv-2.0.1/PKG-INFO
```

### Comparing `ptulsconv-2.0.0/LICENSE` & `ptulsconv-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/README.md` & `ptulsconv-2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [![Documentation Status](https://readthedocs.org/projects/ptulsconv/badge/?version=latest)](https://ptulsconv.readthedocs.io/en/latest/?badge=latest)
 ![](https://img.shields.io/github/license/iluvcapra/ptulsconv.svg)
 ![](https://img.shields.io/pypi/pyversions/ptulsconv.svg) 
 [![](https://img.shields.io/pypi/v/ptulsconv.svg)][pypi]
-![GitHub last commit](https://img.shields.io/github/last-commit/iluvcapra/pycmx)
+![GitHub last commit](https://img.shields.io/github/last-commit/iluvcapra/ptulsconv)
 [![Lint and Test](https://github.com/iluvcapra/ptulsconv/actions/workflows/python-package.yml/badge.svg)](https://github.com/iluvcapra/ptulsconv/actions/workflows/python-package.yml)
 
 [pypi]: https://pypi.org/project/ptulsconv/
 
 
 # ptulsconv
 
-Read Pro Tools text exports and generate PDF reports, JSON output.
+Parse Pro Tools text exports and generate PDF reports, JSON output.
 
 ## Quick Start
 
 For a quick overview of how to cue ADR with `ptulsconv`, check out the [Quickstart][quickstart].
 
 
 ## Installation
```

### Comparing `ptulsconv-2.0.0/ptulsconv/__main__.py` & `ptulsconv-2.0.1/ptulsconv/__main__.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/broadcast_timecode.py` & `ptulsconv-2.0.1/ptulsconv/broadcast_timecode.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/commands.py` & `ptulsconv-2.0.1/ptulsconv/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             req = engine.export_session_as_text()
             req.utf8_encoding()
             req.include_track_edls()
             req.include_markers()
             req.time_type("tc")
             req.dont_show_crossfades()
             req.selected_tracks_only()
-            session_text = req.export_string
+            session_text = req.export_string()
 
     session = parse_document(session_text)
     session_tc_format = session.header.timecode_format
 
     if major_mode == 'raw':
         output.write(MyEncoder().encode(session))
```

### Comparing `ptulsconv-2.0.0/ptulsconv/docparser/adr_entity.py` & `ptulsconv-2.0.1/ptulsconv/docparser/adr_entity.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/docparser/doc_entity.py` & `ptulsconv-2.0.1/ptulsconv/docparser/doc_entity.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/docparser/pt_doc_parser.py` & `ptulsconv-2.0.1/ptulsconv/docparser/pt_doc_parser.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/docparser/tag_compiler.py` & `ptulsconv-2.0.1/ptulsconv/docparser/tag_compiler.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/docparser/tag_mapping.py` & `ptulsconv-2.0.1/ptulsconv/docparser/tag_mapping.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/docparser/tagged_string_parser_visitor.py` & `ptulsconv-2.0.1/ptulsconv/docparser/tagged_string_parser_visitor.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/footage.py` & `ptulsconv-2.0.1/ptulsconv/footage.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/pdf/__init__.py` & `ptulsconv-2.0.1/ptulsconv/pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/pdf/continuity.py` & `ptulsconv-2.0.1/ptulsconv/pdf/continuity.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/pdf/line_count.py` & `ptulsconv-2.0.1/ptulsconv/pdf/line_count.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/pdf/summary_log.py` & `ptulsconv-2.0.1/ptulsconv/pdf/summary_log.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/pdf/supervisor_1pg.py` & `ptulsconv-2.0.1/ptulsconv/pdf/supervisor_1pg.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/pdf/talent_sides.py` & `ptulsconv-2.0.1/ptulsconv/pdf/talent_sides.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/reporting.py` & `ptulsconv-2.0.1/ptulsconv/reporting.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/validations.py` & `ptulsconv-2.0.1/ptulsconv/validations.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/xml/common.py` & `ptulsconv-2.0.1/ptulsconv/xml/common.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/xslt/AvidMarkers.xsl` & `ptulsconv-2.0.1/ptulsconv/xslt/AvidMarkers.xsl`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/ptulsconv/xslt/SRT.xsl` & `ptulsconv-2.0.1/ptulsconv/xslt/SRT.xsl`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/pyproject.toml` & `ptulsconv-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ptulsconv-2.0.0/PKG-INFO` & `ptulsconv-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptulsconv
-Version: 2.0.0
+Version: 2.0.1
 Summary: Parse and convert Pro Tools text exports
 Keywords: text-processing,parsers,film,broadcast,editing,editorial
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia
@@ -26,23 +26,23 @@
 Project-URL: Source, https://github.com/iluvcapra/ptulsconv
 Provides-Extra: doc
 
 [![Documentation Status](https://readthedocs.org/projects/ptulsconv/badge/?version=latest)](https://ptulsconv.readthedocs.io/en/latest/?badge=latest)
 ![](https://img.shields.io/github/license/iluvcapra/ptulsconv.svg)
 ![](https://img.shields.io/pypi/pyversions/ptulsconv.svg) 
 [![](https://img.shields.io/pypi/v/ptulsconv.svg)][pypi]
-![GitHub last commit](https://img.shields.io/github/last-commit/iluvcapra/pycmx)
+![GitHub last commit](https://img.shields.io/github/last-commit/iluvcapra/ptulsconv)
 [![Lint and Test](https://github.com/iluvcapra/ptulsconv/actions/workflows/python-package.yml/badge.svg)](https://github.com/iluvcapra/ptulsconv/actions/workflows/python-package.yml)
 
 [pypi]: https://pypi.org/project/ptulsconv/
 
 
 # ptulsconv
 
-Read Pro Tools text exports and generate PDF reports, JSON output.
+Parse Pro Tools text exports and generate PDF reports, JSON output.
 
 ## Quick Start
 
 For a quick overview of how to cue ADR with `ptulsconv`, check out the [Quickstart][quickstart].
 
 
 ## Installation
```

