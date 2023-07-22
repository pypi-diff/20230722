# Comparing `tmp/advent-of-code-data-2.0.0.tar.gz` & `tmp/advent-of-code-data-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advent-of-code-data-2.0.0.tar", last modified: Thu Jul 20 06:13:51 2023, max compression
+gzip compressed data, was "advent-of-code-data-2.0.1.tar", last modified: Sat Jul 22 18:34:19 2023, max compression
```

## Comparing `advent-of-code-data-2.0.0.tar` & `advent-of-code-data-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2023-07-20 06:13:51.280844 advent-of-code-data-2.0.0/
--rw-r--r--   0 wim        (501) staff       (20)     1066 2020-12-01 08:27:42.000000 advent-of-code-data-2.0.0/LICENSE
--rw-r--r--   0 wim        (501) staff       (20)    11833 2023-07-20 06:13:51.280629 advent-of-code-data-2.0.0/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)    11235 2023-07-20 06:01:49.000000 advent-of-code-data-2.0.0/README.rst
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2023-07-20 06:13:51.277401 advent-of-code-data-2.0.0/advent_of_code_data.egg-info/
--rw-r--r--   0 wim        (501) staff       (20)    11833 2023-07-20 06:13:51.000000 advent-of-code-data-2.0.0/advent_of_code_data.egg-info/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)      735 2023-07-20 06:13:51.000000 advent-of-code-data-2.0.0/advent_of_code_data.egg-info/SOURCES.txt
--rw-r--r--   0 wim        (501) staff       (20)        1 2023-07-20 06:13:51.000000 advent-of-code-data-2.0.0/advent_of_code_data.egg-info/dependency_links.txt
--rw-r--r--   0 wim        (501) staff       (20)      136 2023-07-20 06:13:51.000000 advent-of-code-data-2.0.0/advent_of_code_data.egg-info/entry_points.txt
--rw-r--r--   0 wim        (501) staff       (20)      127 2023-07-20 06:13:51.000000 advent-of-code-data-2.0.0/advent_of_code_data.egg-info/requires.txt
--rw-r--r--   0 wim        (501) staff       (20)        5 2023-07-20 06:13:51.000000 advent-of-code-data-2.0.0/advent_of_code_data.egg-info/top_level.txt
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2023-07-20 06:13:51.278879 advent-of-code-data-2.0.0/aocd/
--rw-r--r--   0 wim        (501) staff       (20)     1113 2023-07-15 01:11:47.000000 advent-of-code-data-2.0.0/aocd/__init__.py
--rw-r--r--   0 wim        (501) staff       (20)      952 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.0/aocd/_ipykernel.py
--rw-r--r--   0 wim        (501) staff       (20)     3711 2023-07-15 01:11:47.000000 advent-of-code-data-2.0.0/aocd/cli.py
--rw-r--r--   0 wim        (501) staff       (20)     4822 2023-07-15 00:19:07.000000 advent-of-code-data-2.0.0/aocd/cookies.py
--rw-r--r--   0 wim        (501) staff       (20)    10847 2023-07-19 07:52:28.000000 advent-of-code-data-2.0.0/aocd/examples.py
--rw-r--r--   0 wim        (501) staff       (20)      543 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.0/aocd/exceptions.py
--rw-r--r--   0 wim        (501) staff       (20)     6088 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.0/aocd/get.py
--rw-r--r--   0 wim        (501) staff       (20)    34840 2023-07-19 07:52:28.000000 advent-of-code-data-2.0.0/aocd/models.py
--rw-r--r--   0 wim        (501) staff       (20)     2259 2023-07-19 07:52:28.000000 advent-of-code-data-2.0.0/aocd/post.py
--rw-r--r--   0 wim        (501) staff       (20)    13237 2023-07-20 05:42:33.000000 advent-of-code-data-2.0.0/aocd/runner.py
--rw-r--r--   0 wim        (501) staff       (20)     8195 2023-07-19 07:52:28.000000 advent-of-code-data-2.0.0/aocd/utils.py
--rw-r--r--   0 wim        (501) staff       (20)     1259 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.0/pyproject.toml
--rw-r--r--   0 wim        (501) staff       (20)       38 2023-07-20 06:13:51.280885 advent-of-code-data-2.0.0/setup.cfg
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2023-07-20 06:13:51.280444 advent-of-code-data-2.0.0/tests/
--rw-r--r--   0 wim        (501) staff       (20)     1960 2023-03-26 03:44:00.000000 advent-of-code-data-2.0.0/tests/test_aocd.py
--rw-r--r--   0 wim        (501) staff       (20)     1063 2023-03-13 04:28:20.000000 advent-of-code-data-2.0.0/tests/test_auth.py
--rw-r--r--   0 wim        (501) staff       (20)     3476 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.0/tests/test_cli.py
--rw-r--r--   0 wim        (501) staff       (20)      352 2021-09-30 08:00:05.000000 advent-of-code-data-2.0.0/tests/test_cookies.py
--rw-r--r--   0 wim        (501) staff       (20)     1465 2020-12-01 08:27:42.000000 advent-of-code-data-2.0.0/tests/test_date_finding.py
--rw-r--r--   0 wim        (501) staff       (20)     2832 2023-03-26 03:44:00.000000 advent-of-code-data-2.0.0/tests/test_date_introspection.py
--rw-r--r--   0 wim        (501) staff       (20)     2417 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.0/tests/test_example_parser.py
--rw-r--r--   0 wim        (501) staff       (20)     5557 2023-03-26 03:44:00.000000 advent-of-code-data-2.0.0/tests/test_get_data.py
--rw-r--r--   0 wim        (501) staff       (20)    20693 2023-07-19 05:22:48.000000 advent-of-code-data-2.0.0/tests/test_models.py
--rw-r--r--   0 wim        (501) staff       (20)    10303 2023-07-20 05:42:33.000000 advent-of-code-data-2.0.0/tests/test_runner.py
--rw-r--r--   0 wim        (501) staff       (20)    11906 2023-07-19 05:22:48.000000 advent-of-code-data-2.0.0/tests/test_submit.py
--rw-r--r--   0 wim        (501) staff       (20)     2143 2023-03-24 06:12:49.000000 advent-of-code-data-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2023-07-22 18:34:19.968902 advent-of-code-data-2.0.1/
+-rw-r--r--   0 wim        (501) staff       (20)     1066 2020-12-01 08:27:42.000000 advent-of-code-data-2.0.1/LICENSE
+-rw-r--r--   0 wim        (501) staff       (20)    11913 2023-07-22 18:34:19.968654 advent-of-code-data-2.0.1/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)    11315 2023-07-20 06:53:45.000000 advent-of-code-data-2.0.1/README.rst
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2023-07-22 18:34:19.965514 advent-of-code-data-2.0.1/advent_of_code_data.egg-info/
+-rw-r--r--   0 wim        (501) staff       (20)    11913 2023-07-22 18:34:19.000000 advent-of-code-data-2.0.1/advent_of_code_data.egg-info/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)      735 2023-07-22 18:34:19.000000 advent-of-code-data-2.0.1/advent_of_code_data.egg-info/SOURCES.txt
+-rw-r--r--   0 wim        (501) staff       (20)        1 2023-07-22 18:34:19.000000 advent-of-code-data-2.0.1/advent_of_code_data.egg-info/dependency_links.txt
+-rw-r--r--   0 wim        (501) staff       (20)      136 2023-07-22 18:34:19.000000 advent-of-code-data-2.0.1/advent_of_code_data.egg-info/entry_points.txt
+-rw-r--r--   0 wim        (501) staff       (20)      127 2023-07-22 18:34:19.000000 advent-of-code-data-2.0.1/advent_of_code_data.egg-info/requires.txt
+-rw-r--r--   0 wim        (501) staff       (20)        5 2023-07-22 18:34:19.000000 advent-of-code-data-2.0.1/advent_of_code_data.egg-info/top_level.txt
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2023-07-22 18:34:19.966945 advent-of-code-data-2.0.1/aocd/
+-rw-r--r--   0 wim        (501) staff       (20)     1113 2023-07-15 01:11:47.000000 advent-of-code-data-2.0.1/aocd/__init__.py
+-rw-r--r--   0 wim        (501) staff       (20)      952 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.1/aocd/_ipykernel.py
+-rw-r--r--   0 wim        (501) staff       (20)     3700 2023-07-22 18:16:18.000000 advent-of-code-data-2.0.1/aocd/cli.py
+-rw-r--r--   0 wim        (501) staff       (20)     4822 2023-07-15 00:19:07.000000 advent-of-code-data-2.0.1/aocd/cookies.py
+-rw-r--r--   0 wim        (501) staff       (20)    10838 2023-07-22 18:16:18.000000 advent-of-code-data-2.0.1/aocd/examples.py
+-rw-r--r--   0 wim        (501) staff       (20)      543 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.1/aocd/exceptions.py
+-rw-r--r--   0 wim        (501) staff       (20)     6088 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.1/aocd/get.py
+-rw-r--r--   0 wim        (501) staff       (20)    34818 2023-07-22 18:16:18.000000 advent-of-code-data-2.0.1/aocd/models.py
+-rw-r--r--   0 wim        (501) staff       (20)     2259 2023-07-19 07:52:28.000000 advent-of-code-data-2.0.1/aocd/post.py
+-rw-r--r--   0 wim        (501) staff       (20)    13237 2023-07-20 05:42:33.000000 advent-of-code-data-2.0.1/aocd/runner.py
+-rw-r--r--   0 wim        (501) staff       (20)     8195 2023-07-19 07:52:28.000000 advent-of-code-data-2.0.1/aocd/utils.py
+-rw-r--r--   0 wim        (501) staff       (20)     1259 2023-07-22 18:16:18.000000 advent-of-code-data-2.0.1/pyproject.toml
+-rw-r--r--   0 wim        (501) staff       (20)       38 2023-07-22 18:34:19.968942 advent-of-code-data-2.0.1/setup.cfg
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2023-07-22 18:34:19.968471 advent-of-code-data-2.0.1/tests/
+-rw-r--r--   0 wim        (501) staff       (20)     1960 2023-03-26 03:44:00.000000 advent-of-code-data-2.0.1/tests/test_aocd.py
+-rw-r--r--   0 wim        (501) staff       (20)     1063 2023-03-13 04:28:20.000000 advent-of-code-data-2.0.1/tests/test_auth.py
+-rw-r--r--   0 wim        (501) staff       (20)     3476 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.1/tests/test_cli.py
+-rw-r--r--   0 wim        (501) staff       (20)      352 2021-09-30 08:00:05.000000 advent-of-code-data-2.0.1/tests/test_cookies.py
+-rw-r--r--   0 wim        (501) staff       (20)     1465 2020-12-01 08:27:42.000000 advent-of-code-data-2.0.1/tests/test_date_finding.py
+-rw-r--r--   0 wim        (501) staff       (20)     2832 2023-03-26 03:44:00.000000 advent-of-code-data-2.0.1/tests/test_date_introspection.py
+-rw-r--r--   0 wim        (501) staff       (20)     2417 2023-07-14 02:56:54.000000 advent-of-code-data-2.0.1/tests/test_example_parser.py
+-rw-r--r--   0 wim        (501) staff       (20)     5557 2023-03-26 03:44:00.000000 advent-of-code-data-2.0.1/tests/test_get_data.py
+-rw-r--r--   0 wim        (501) staff       (20)    20693 2023-07-19 05:22:48.000000 advent-of-code-data-2.0.1/tests/test_models.py
+-rw-r--r--   0 wim        (501) staff       (20)    10303 2023-07-20 05:42:33.000000 advent-of-code-data-2.0.1/tests/test_runner.py
+-rw-r--r--   0 wim        (501) staff       (20)    11906 2023-07-19 05:22:48.000000 advent-of-code-data-2.0.1/tests/test_submit.py
+-rw-r--r--   0 wim        (501) staff       (20)     2143 2023-03-24 06:12:49.000000 advent-of-code-data-2.0.1/tests/test_utils.py
```

### Comparing `advent-of-code-data-2.0.0/LICENSE` & `advent-of-code-data-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/PKG-INFO` & `advent-of-code-data-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advent-of-code-data
-Version: 2.0.0
+Version: 2.0.1
 Summary: Get your puzzle data with a single import
 Author-email: Wim Glenn <hey@wimglenn.com>
 License: MIT
 Project-URL: Homepage, https://github.com/wimglenn/advent-of-code-data
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -101,16 +101,18 @@
 
 **Puzzle inputs differ by user.**   So export your session ID, for example:
 
 .. code-block:: bash
 
    export AOC_SESSION=cafef00db01dfaceba5eba11deadbeef
 
-This is a cookie which is set when you login to AoC.  You can find it with
-your browser inspector.  If you're hacking on AoC at all you probably already
+*Note:* Windows users should use ``set`` instead of ``export`` here.
+
+The session ID is a cookie which is set when you login to AoC.  You can find it
+with your browser inspector.  If you're hacking on AoC at all you probably already
 know these kind of tricks, but if you need help with that part then you can
 `look here <https://github.com/wimglenn/advent-of-code/issues/1>`_.
 
 *Note:* If you don't like the env var, you could also keep your token(s) in files.
 By default the location is ``~/.config/aocd/token``. Set the ``AOCD_DIR`` environment
 variable to some existing directory if you wish to use another location to store token(s).
```

### Comparing `advent-of-code-data-2.0.0/README.rst` & `advent-of-code-data-2.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,18 @@
 
 **Puzzle inputs differ by user.**   So export your session ID, for example:
 
 .. code-block:: bash
 
    export AOC_SESSION=cafef00db01dfaceba5eba11deadbeef
 
-This is a cookie which is set when you login to AoC.  You can find it with
-your browser inspector.  If you're hacking on AoC at all you probably already
+*Note:* Windows users should use ``set`` instead of ``export`` here.
+
+The session ID is a cookie which is set when you login to AoC.  You can find it
+with your browser inspector.  If you're hacking on AoC at all you probably already
 know these kind of tricks, but if you need help with that part then you can
 `look here <https://github.com/wimglenn/advent-of-code/issues/1>`_.
 
 *Note:* If you don't like the env var, you could also keep your token(s) in files.
 By default the location is ``~/.config/aocd/token``. Set the ``AOCD_DIR`` environment
 variable to some existing directory if you wish to use another location to store token(s).
```

### Comparing `advent-of-code-data-2.0.0/advent_of_code_data.egg-info/PKG-INFO` & `advent-of-code-data-2.0.1/advent_of_code_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advent-of-code-data
-Version: 2.0.0
+Version: 2.0.1
 Summary: Get your puzzle data with a single import
 Author-email: Wim Glenn <hey@wimglenn.com>
 License: MIT
 Project-URL: Homepage, https://github.com/wimglenn/advent-of-code-data
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -101,16 +101,18 @@
 
 **Puzzle inputs differ by user.**   So export your session ID, for example:
 
 .. code-block:: bash
 
    export AOC_SESSION=cafef00db01dfaceba5eba11deadbeef
 
-This is a cookie which is set when you login to AoC.  You can find it with
-your browser inspector.  If you're hacking on AoC at all you probably already
+*Note:* Windows users should use ``set`` instead of ``export`` here.
+
+The session ID is a cookie which is set when you login to AoC.  You can find it
+with your browser inspector.  If you're hacking on AoC at all you probably already
 know these kind of tricks, but if you need help with that part then you can
 `look here <https://github.com/wimglenn/advent-of-code/issues/1>`_.
 
 *Note:* If you don't like the env var, you could also keep your token(s) in files.
 By default the location is ``~/.config/aocd/token``. Set the ``AOCD_DIR`` environment
 variable to some existing directory if you wish to use another location to store token(s).
```

### Comparing `advent-of-code-data-2.0.0/advent_of_code_data.egg-info/SOURCES.txt` & `advent-of-code-data-2.0.1/advent_of_code_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/aocd/__init__.py` & `advent-of-code-data-2.0.1/aocd/__init__.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/aocd/_ipykernel.py` & `advent-of-code-data-2.0.1/aocd/_ipykernel.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/aocd/cli.py` & `advent-of-code-data-2.0.1/aocd/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     )
     if plugins:
         parser.add_argument(
             "-e",
             "--example-parser",
             nargs="?",
             choices=plugins,
-            const="aocd_examples_canned",
+            const="reference",
             help="get the example(s) data, if any",
         )
     if len(users) > 1:
         parser.add_argument(
             "-u",
             "--user",
             help=(
```

### Comparing `advent-of-code-data-2.0.0/aocd/cookies.py` & `advent-of-code-data-2.0.1/aocd/cookies.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/aocd/examples.py` & `advent-of-code-data-2.0.1/aocd/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     strs = [p.read_text(encoding="utf-8") for p in paths]
     return list({}.fromkeys(strs))
 
 
 def main():
     """
     Summarize an example parser's results with historical puzzles' prose, and
-    compare the performance against a reference implementation (aocd_examples_canned)
+    compare the performance against a reference implementation
     """
     try:
         from rich.console import Console
         from rich.table import Table
     except ImportError:
         sys.exit(
             f"To use example parser, please install rich:\n"
@@ -162,20 +162,21 @@
     aoc_now = datetime.now(tz=AOC_TZ)
     all_years = range(2015, aoc_now.year + int(aoc_now.month == 12))
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-e",
         "--example-parser",
         choices=list(plugins),
-        default="aocd_examples_canned",
+        default="reference",
         help="plugin to use for example extraction testing (default: %(default)s)",
     )
     parser.add_argument(
         "-y",
         "--years",
+        metavar="2015+",
         nargs="+",
         help="years to run the parser against (can specify multiple)",
         choices=all_years,
         type=int,
         action="extend",
     )
     parser.add_argument(
```

### Comparing `advent-of-code-data-2.0.0/aocd/exceptions.py` & `advent-of-code-data-2.0.1/aocd/exceptions.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/aocd/get.py` & `advent-of-code-data-2.0.1/aocd/get.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/aocd/models.py` & `advent-of-code-data-2.0.1/aocd/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         every puzzle has usable examples), or it might have several examples, but it
         will usually have one element. The list, and the examples themselves, may be
         different depending on whether or not part b of the puzzle prose has been
         unlocked (i.e. part a has already been solved correctly).
         """
         return self._get_examples()
 
-    def _get_examples(self, parser_name="aocd_examples_canned"):
+    def _get_examples(self, parser_name="reference"):
         # invoke a named example parser to extract examples from cached prose.
         # logs warning and returns an empty list if the parser plugin raises an
         # exception for any reason.
         try:
             page = examples.Page.from_raw(html=self._get_prose())
             parser = _load_example_parser(name=parser_name)
             if getattr(parser, "uses_real_datas", True):
@@ -820,15 +820,15 @@
         users = json.loads(path.read_text(encoding="utf-8"))
     except FileNotFoundError:
         users = {"default": default_user().token}
     return users
 
 
 @cache
-def _load_example_parser(group="adventofcode.examples", name="aocd_examples_canned"):
+def _load_example_parser(group="adventofcode.examples", name="reference"):
     # lazy-loads a plugin used to parse sample data, and cache it
     try:
         # Python 3.10+ - group/name selectable entry points
         eps = entry_points().select(group=group, name=name)
     except AttributeError:
         # Python 3.9 - dict interface
         eps = [ep for ep in entry_points()[group] if ep.name == name]
```

### Comparing `advent-of-code-data-2.0.0/aocd/post.py` & `advent-of-code-data-2.0.1/aocd/post.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/aocd/runner.py` & `advent-of-code-data-2.0.1/aocd/runner.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/aocd/utils.py` & `advent-of-code-data-2.0.1/aocd/utils.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/pyproject.toml` & `advent-of-code-data-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "advent-of-code-data"
-version = "2.0.0"
+version = "2.0.1"
 description = "Get your puzzle data with a single import"
 requires-python = ">=3.9"
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries",
     "Topic :: Games/Entertainment :: Puzzle Games",
 ]
 dependencies = [
     "beautifulsoup4",
     "pebble",
     "urllib3",
     'tzdata ; platform_system == "Windows"',
-    "aocd-example-parser >= 2023.1",
+    "aocd-example-parser >= 2023.2",
 ]
 
 [[project.authors]]
 name = "Wim Glenn"
 email = "hey@wimglenn.com"
 
 [project.license]
```

### Comparing `advent-of-code-data-2.0.0/tests/test_aocd.py` & `advent-of-code-data-2.0.1/tests/test_aocd.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_auth.py` & `advent-of-code-data-2.0.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_cli.py` & `advent-of-code-data-2.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_date_finding.py` & `advent-of-code-data-2.0.1/tests/test_date_finding.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_date_introspection.py` & `advent-of-code-data-2.0.1/tests/test_date_introspection.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_example_parser.py` & `advent-of-code-data-2.0.1/tests/test_example_parser.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_get_data.py` & `advent-of-code-data-2.0.1/tests/test_get_data.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_models.py` & `advent-of-code-data-2.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_runner.py` & `advent-of-code-data-2.0.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_submit.py` & `advent-of-code-data-2.0.1/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `advent-of-code-data-2.0.0/tests/test_utils.py` & `advent-of-code-data-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

