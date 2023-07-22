# Comparing `tmp/dompare-0.1.100.tar.gz` & `tmp/dompare-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dompare-0.1.100.tar", last modified: Sat Oct 29 01:17:56 2022, max compression
+gzip compressed data, was "dompare-0.2.0.tar", last modified: Sat Jul 22 04:25:10 2023, max compression
```

## Comparing `dompare-0.1.100.tar` & `dompare-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 yunfeng   (1000) yunfeng   (1000)        0 2022-10-29 01:17:56.700151 dompare-0.1.100/
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)     1069 2022-10-28 01:03:00.000000 dompare-0.1.100/LICENSE
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)     3451 2022-10-29 01:17:56.700151 dompare-0.1.100/PKG-INFO
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)     3109 2022-10-28 14:28:50.000000 dompare-0.1.100/README.md
-drwxr-xr-x   0 yunfeng   (1000) yunfeng   (1000)        0 2022-10-29 01:17:56.700151 dompare-0.1.100/dompare/
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)     6907 2022-10-28 14:29:07.000000 dompare-0.1.100/dompare/__init__.py
-drwxr-xr-x   0 yunfeng   (1000) yunfeng   (1000)        0 2022-10-29 01:17:56.700151 dompare-0.1.100/dompare.egg-info/
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)     3451 2022-10-29 01:17:56.000000 dompare-0.1.100/dompare.egg-info/PKG-INFO
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)      234 2022-10-29 01:17:56.000000 dompare-0.1.100/dompare.egg-info/SOURCES.txt
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)        1 2022-10-29 01:17:56.000000 dompare-0.1.100/dompare.egg-info/dependency_links.txt
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)       50 2022-10-29 01:17:56.000000 dompare-0.1.100/dompare.egg-info/entry_points.txt
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)       37 2022-10-29 01:17:56.000000 dompare-0.1.100/dompare.egg-info/requires.txt
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)        8 2022-10-29 01:17:56.000000 dompare-0.1.100/dompare.egg-info/top_level.txt
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)       38 2022-10-29 01:17:56.700151 dompare-0.1.100/setup.cfg
--rw-r--r--   0 yunfeng   (1000) yunfeng   (1000)      730 2022-10-29 01:17:45.000000 dompare-0.1.100/setup.py
+drwxr-xr-x   0 yunfeng    (502) staff       (20)        0 2023-07-22 04:25:10.633448 dompare-0.2.0/
+-rw-r--r--   0 yunfeng    (502) staff       (20)     1069 2022-10-26 05:45:27.000000 dompare-0.2.0/LICENSE
+-rw-r--r--   0 yunfeng    (502) staff       (20)      374 2023-07-22 04:25:10.633267 dompare-0.2.0/PKG-INFO
+-rw-r--r--   0 yunfeng    (502) staff       (20)     3109 2022-10-28 05:52:51.000000 dompare-0.2.0/README.md
+drwxr-xr-x   0 yunfeng    (502) staff       (20)        0 2023-07-22 04:25:10.631298 dompare-0.2.0/dompare/
+-rw-r--r--   0 yunfeng    (502) staff       (20)     7123 2023-07-22 04:23:51.000000 dompare-0.2.0/dompare/__init__.py
+drwxr-xr-x   0 yunfeng    (502) staff       (20)        0 2023-07-22 04:25:10.632677 dompare-0.2.0/dompare.egg-info/
+-rw-r--r--   0 yunfeng    (502) staff       (20)      374 2023-07-22 04:25:10.000000 dompare-0.2.0/dompare.egg-info/PKG-INFO
+-rw-r--r--   0 yunfeng    (502) staff       (20)      255 2023-07-22 04:25:10.000000 dompare-0.2.0/dompare.egg-info/SOURCES.txt
+-rw-r--r--   0 yunfeng    (502) staff       (20)        1 2023-07-22 04:25:10.000000 dompare-0.2.0/dompare.egg-info/dependency_links.txt
+-rw-r--r--   0 yunfeng    (502) staff       (20)       50 2023-07-22 04:25:10.000000 dompare-0.2.0/dompare.egg-info/entry_points.txt
+-rw-r--r--   0 yunfeng    (502) staff       (20)       26 2023-07-22 04:25:10.000000 dompare-0.2.0/dompare.egg-info/requires.txt
+-rw-r--r--   0 yunfeng    (502) staff       (20)        8 2023-07-22 04:25:10.000000 dompare-0.2.0/dompare.egg-info/top_level.txt
+-rw-r--r--   0 yunfeng    (502) staff       (20)       38 2023-07-22 04:25:10.633497 dompare-0.2.0/setup.cfg
+-rw-r--r--   0 yunfeng    (502) staff       (20)      699 2023-07-22 04:21:54.000000 dompare-0.2.0/setup.py
+drwxr-xr-x   0 yunfeng    (502) staff       (20)        0 2023-07-22 04:25:10.632861 dompare-0.2.0/tests/
+-rw-r--r--   0 yunfeng    (502) staff       (20)       40 2022-10-26 05:45:27.000000 dompare-0.2.0/tests/test_sample.py
```

### Comparing `dompare-0.1.100/LICENSE` & `dompare-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dompare-0.1.100/PKG-INFO` & `dompare-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: dompare
-Version: 0.1.100
-Summary: A program to diff two directories recursively
-Home-page: https://github.com/vra/dompare
-Author: Yunfeng Wang
-Author-email: wyf.brz@gmail.com
-License: MIT Licence
-Keywords: dompare,Linux,diff,directories
-Platform: any
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # dompare
 
 [![BUILD](https://github.com/vra/dompare/actions/workflows/python-package.yml/badge.svg)](https://github.com/vra/dompare/actions)
 
 A command line tool to diff two directories recursively.
```

### Comparing `dompare-0.1.100/dompare/__init__.py` & `dompare-0.2.0/dompare/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,119 +1,111 @@
 """A command line tool to diff two directories recursively."""
 import argparse
 import difflib
 from http.server import HTTPServer, SimpleHTTPRequestHandler
 import logging
-import logging.config
 import os
+import sys
 import tempfile
 
-import coloredlogs
 from binaryornot.check import is_binary
+from loguru import logger
 
 
-def create_logger(is_verbose):
-    # Suppress logging info from third-party packages
-    logging.getLogger("binaryornot").setLevel(logging.ERROR)
-    logging.getLogger("chardet").setLevel(logging.ERROR)
-
-    FIELD_STYLES = dict(
-        asctime=dict(color="red"),
-        hostname=dict(color="magenta"),
-        levelname=dict(color="yellow"),
-        filename=dict(color="magenta"),
-        name=dict(color="blue"),
-        threadName=dict(color="green"),
-    )
-
-    LEVEL_STYLES = dict(
-        debug=dict(color="white"),
-        info=dict(color="cyan"),
-        warning=dict(color="red"),
-        error=dict(color="red"),
-        critical=dict(color="red"),
-    )
-
-    logger = logging.getLogger("dompare")
-    level = "DEBUG" if is_verbose else "INFO"
-    logging_level = logging.DEBUG if is_verbose else logging.INFO
-    logger.setLevel(logging_level)
-
-    coloredlogs.install(
-        level=level,
-        fmt="[%(levelname)s] [%(asctime)s] [%(name)s] %(message)s",
-        level_styles=LEVEL_STYLES,
-        field_styles=FIELD_STYLES,
-    )
+def is_binary_string(filename):
+    with open(filename, "rb") as f:
+        bytes = f.read(1024)
+        textchars = bytearray(
+            {7, 8, 9, 10, 12, 13, 27} | set(range(0x20, 0x100)) - {0x7F}
+        )
+        return bool(bytes.translate(None, textchars))
 
-    return logger
+
+def is_binary_file(filename):
+    with open(filename, "rb") as f:
+        # Read the first 1024 bytes of the file
+        data = f.read(1024)
+        # Check for null bytes
+        return b"\0" in data
 
 
 def parse_parameters():
     parser = argparse.ArgumentParser("dompare")
     parser.add_argument("dir1", help="Path to the first directory")
     parser.add_argument("dir2", help="Path to the second directory")
     parser.add_argument("--host", type=str, default="localhost", help="host to bind")
     parser.add_argument("--port", type=str, default=5240, help="port to listen")
     parser.add_argument(
-        "--verbose", action="store_true", help="Show detailed information"
+        "-v", "--verbose", action="store_true", help="Show detailed information"
     )
     parser.add_argument(
         "--exclude-dot",
         action="store_true",
         dest="exclude_dot",
         help="Ignore All hidden folders and files beginning with .",
     )
     parser.add_argument(
         "--show-same",
         action="store_true",
         dest="show_same",
         help="Show files that no difference in html file",
     )
     parser.add_argument(
-        "--exclude", type=str, nargs="+", help="Ignore listed directories when diff"
+        "-e",
+        "--exclude",
+        type=str,
+        nargs="+",
+        help="Ignore listed directories when diff",
     )
 
     return parser.parse_args()
 
 
+def detect_file_encoding(path):
+    import chardet
+
+    with open(path, "rb") as f:
+        return chardet.detect(f.read())["encoding"]
+
+
 def diff_two_files(path1, path2, root_html_path, show_same):
     content1 = ""
     content2 = ""
-    with open(path1, encoding="utf-8") as f:
-        content1 = f.readlines()
-    with open(path2, encoding="utf-8") as f:
-        content2 = f.readlines()
+    try:
+        with open(path1, encoding=detect_file_encoding(path1)) as f:
+            content1 = f.readlines()
+        with open(path2, encoding=detect_file_encoding(path2)) as f:
+            content2 = f.readlines()
+    except UnicodeDecodeError:
+        logger.warning("Open file error: {}".format(path1))
+        return
 
     hd = difflib.HtmlDiff(tabsize=4, wrapcolumn=80)
     diff_content = hd.make_file(
         content1, content2, fromdesc=path1, todesc=path2, context=True
     )
     diff_content = remove_legends(diff_content)
 
     need_write = True if show_same else "No Differences Found" not in diff_content
     if need_write:
         with open(root_html_path.name, "a+") as f:
             f.write(diff_content)
             f.close()
 
 
-def diff_two_directories(logger, dir1, dir2, tmp_file, exclude, exclude_dot, show_same):
+def diff_two_directories(dir1, dir2, tmp_file, exclude, exclude_dot, show_same):
     if exclude is not None:
         exclude += [".git"]
     else:
         exclude = [".git"]
 
     # Add comparsion betwen two files
     if os.path.isfile(dir1) and os.path.isfile(dir2):
         target_path = os.path.basename(dir1)
         target_path1 = os.path.basename(dir2)
-        assert (
-            target_path == target_path1
-        ), "dompare only support files with the same name!"
         dir1 = os.path.dirname(dir1)
         dir2 = os.path.dirname(dir2)
         all_paths = os.listdir(dir1)
         for path in all_paths:
             if path != target_path:
                 exclude.append(path)
 
@@ -127,22 +119,37 @@
             if ex in paths:
                 logger.debug("Ignore {}".format(ex))
                 paths.remove(ex)
 
     for path in paths:
         path1 = os.path.join(dir1, path)
         path2 = os.path.join(dir2, path)
+        need_skip = False
+        for ex in exclude:
+            if ex in path1:
+                need_skip = True
+                break
+            if ex in path1:
+                need_skip = True
+                break
+        if need_skip:
+            logger.debug("Ignore {}".format(path1))
+            continue
 
         if os.path.isdir(path1):
             logger.debug("Processing dir {}".format(path1))
             diff_two_directories(
-                logger, path1, path2, tmp_file, exclude, exclude_dot, show_same
+                path1, path2, tmp_file, exclude, exclude_dot, show_same
             )
 
-        elif is_binary(path1):
+        elif os.path.islink(path1):
+            logger.debug("Ignore symlink file {}".format(path1))
+            continue
+
+        elif is_binary(path1) or is_binary_file(path1) or is_binary_string(path1):
             logger.debug("Ignore binary file {}".format(path1))
             continue
 
         elif not os.path.exists(os.path.join(dir2, path)):
             logger.debug(
                 "Ignore single file (no same name file in dir2) {}".format(path1)
             )
@@ -175,40 +182,44 @@
     if content == "":
         content = "No diff is found"
 
     with open(tmp_file.name, "w") as f:
         f.write(content)
 
 
-def run_http_server(logger, tmp_dir, host, port):
+def run_http_server(tmp_dir, host, port):
     logger.debug("Run http.server in dir: {}, host: {}:{}".format(tmp_dir, host, port))
     os.chdir(tmp_dir)
     httpd = HTTPServer((host, int(port)), SimpleHTTPRequestHandler)
     httpd.serve_forever()
 
 
 def main():
     args = parse_parameters()
 
+    logger.remove()
+    if args.verbose:
+        logger.add(sys.stdout, level="DEBUG")
+    else:
+        logger.add(sys.stdout, level="INFO")
+
+    logger.info("Running, please wait...")
     out_dir1 = os.path.realpath(args.dir1)
     out_dir2 = os.path.realpath(args.dir2)
 
     assert os.path.exists(out_dir1), "path1 {} is not exist!".format(out_dir1)
     assert os.path.exists(out_dir2), "path2 {} is not exist!".format(out_dir2)
 
     tmp_file = tempfile.NamedTemporaryFile(
         prefix="dompare-", suffix=".html", delete=False
     )
     tmp_dir = os.path.dirname(tmp_file.name)
 
-    logger = create_logger(args.verbose)
-
     try:
         diff_two_directories(
-            logger,
             out_dir1,
             out_dir2,
             tmp_file,
             args.exclude,
             args.exclude_dot,
             args.show_same,
         )
@@ -217,15 +228,15 @@
             args.host, args.port, os.path.basename(tmp_file.name)
         )
         logger.info(
             "Compare finished. Please visit {} to see diff file (Press Ctrl-C to stop)".format(
                 url
             )
         )
-        run_http_server(logger, tmp_dir, args.host, args.port)
+        run_http_server(tmp_dir, args.host, args.port)
     finally:
         tmp_file.close()
         os.remove(tmp_file.name)
 
 
 if __name__ == "__main__":
     main()
```

