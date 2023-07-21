# Comparing `tmp/appeal-0.6.tar.gz` & `tmp/appeal-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeal-0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "appeal-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `appeal-0.6.tar` & `appeal-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.6/.gitignore
--rw-r--r--   0        0        0     1090 2023-04-27 05:54:38.102243 appeal-0.6/LICENSE
--rw-r--r--   0        0        0    83589 2023-07-20 13:32:28.219271 appeal-0.6/README.md
--rw-r--r--   0        0        0   278507 2023-07-20 13:28:58.640891 appeal-0.6/appeal/__init__.py
--rw-r--r--   0        0        0    23888 2023-06-22 08:40:31.452281 appeal-0.6/appeal/argument_grouping.py
--rwxr-xr-x   0        0        0     4637 2023-07-20 13:28:58.640891 appeal-0.6/appeal/cpp.py
--rw-r--r--   0        0        0    19692 2023-05-02 08:57:46.416604 appeal-0.6/appeal/text.py
--rwxr-xr-x   0        0        0     4721 2023-07-20 13:28:58.644891 appeal-0.6/appeal/want_prints.py
--rw-r--r--   0        0        0      595 2023-07-20 13:28:58.644891 appeal-0.6/pyproject.toml
--rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.6/resources/images/appeal.logo.png
--rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.6/resources/images/give.your.program.appeal.png
--rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.6/resources/links.txt
--rw-r--r--   0        0        0      715 2023-07-20 13:28:58.644891 appeal-0.6/tests/read_corpus/multiperky1.pky
--rw-r--r--   0        0        0      319 2023-07-20 13:28:58.644891 appeal-0.6/tests/read_corpus/multiperky2.pky
--rw-r--r--   0        0        0      274 2023-07-20 13:28:58.644891 appeal-0.6/tests/read_corpus/multiperky3.pky
--rw-r--r--   0        0        0      323 2023-07-20 13:28:58.644891 appeal-0.6/tests/read_corpus/perkytest1.pky
--rw-r--r--   0        0        0    49711 2023-07-20 13:28:58.648891 appeal-0.6/tests/read_corpus/starvote_ballots_best_akali_skins.csv
--rw-r--r--   0        0        0      290 2023-07-20 13:28:58.648891 appeal-0.6/tests/read_corpus/tomltest1.toml
--rw-r--r--   0        0        0    77772 2023-07-20 13:28:58.648891 appeal-0.6/tests/test_all.py
--rw-r--r--   0        0        0    12963 2023-07-20 13:28:58.648891 appeal-0.6/tests/test_read.py
--rw-r--r--   0        0        0     1136 2023-06-17 11:18:04.335043 appeal-0.6/tests/want_prints_test_corpus/README.md
--rw-r--r--   0        0        0      975 2023-06-17 11:13:44.684903 appeal-0.6/tests/want_prints_test_corpus/commented.py
--rw-r--r--   0        0        0      917 2023-06-17 11:13:17.480679 appeal-0.6/tests/want_prints_test_corpus/uncommented.py
--rw-r--r--   0        0        0    84177 1970-01-01 00:00:00.000000 appeal-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1191 2023-07-21 23:35:13.108973 appeal-0.6.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1373 2023-07-21 23:35:13.108973 appeal-0.6.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       38 2023-07-21 23:35:13.108973 appeal-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1090 2023-04-27 05:54:38.102243 appeal-0.6.1/LICENSE
+-rw-r--r--   0        0        0    84407 2023-07-21 23:35:13.108973 appeal-0.6.1/README.md
+-rw-r--r--   0        0        0   278608 2023-07-21 23:38:17.730790 appeal-0.6.1/appeal/__init__.py
+-rw-r--r--   0        0        0    23888 2023-06-22 08:40:31.452281 appeal-0.6.1/appeal/argument_grouping.py
+-rwxr-xr-x   0        0        0     4637 2023-07-20 13:28:58.640891 appeal-0.6.1/appeal/cpp.py
+-rw-r--r--   0        0        0    19692 2023-05-02 08:57:46.416604 appeal-0.6.1/appeal/text.py
+-rwxr-xr-x   0        0        0     4741 2023-07-21 23:35:13.108973 appeal-0.6.1/appeal/want_prints.py
+-rw-r--r--   0        0        0      905 2023-07-21 23:35:13.108973 appeal-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.6.1/resources/images/appeal.logo.png
+-rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.6.1/resources/images/give.your.program.appeal.png
+-rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.6.1/resources/links.txt
+-rw-r--r--   0        0        0      715 2023-07-20 13:28:58.644891 appeal-0.6.1/tests/read_corpus/multiperky1.pky
+-rw-r--r--   0        0        0      319 2023-07-20 13:28:58.644891 appeal-0.6.1/tests/read_corpus/multiperky2.pky
+-rw-r--r--   0        0        0      274 2023-07-20 13:28:58.644891 appeal-0.6.1/tests/read_corpus/multiperky3.pky
+-rw-r--r--   0        0        0      323 2023-07-20 13:28:58.644891 appeal-0.6.1/tests/read_corpus/perkytest1.pky
+-rw-r--r--   0        0        0    49711 2023-07-20 13:28:58.648891 appeal-0.6.1/tests/read_corpus/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0      290 2023-07-20 13:28:58.648891 appeal-0.6.1/tests/read_corpus/tomltest1.toml
+-rw-r--r--   0        0        0    77772 2023-07-20 13:28:58.648891 appeal-0.6.1/tests/test_all.py
+-rw-r--r--   0        0        0    12963 2023-07-20 13:28:58.648891 appeal-0.6.1/tests/test_read.py
+-rw-r--r--   0        0        0     1136 2023-06-17 11:18:04.335043 appeal-0.6.1/tests/want_prints_test_corpus/README.md
+-rw-r--r--   0        0        0      975 2023-06-17 11:13:44.684903 appeal-0.6.1/tests/want_prints_test_corpus/commented.py
+-rw-r--r--   0        0        0      917 2023-06-17 11:13:17.480679 appeal-0.6.1/tests/want_prints_test_corpus/uncommented.py
+-rw-r--r--   0        0        0    85342 1970-01-01 00:00:00.000000 appeal-0.6.1/PKG-INFO
```

### Comparing `appeal-0.6/LICENSE` & `appeal-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appeal-0.6/README.md` & `appeal-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ![## Appeal](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/appeal.logo.png)
 
 ![## Give your program Appeal!](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/give.your.program.appeal.png)
 
 ##### Copyright 2021-2023 by Larry Hastings
 
+[![# test badge](https://img.shields.io/github/actions/workflow/status/larryhastings/appeal/test.yml?branch=master&label=test)](https://github.com/larryhastings/appeal/actions/workflows/test.yml) [![# python versions badge](https://img.shields.io/pypi/pyversions/appeal.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/appeal/)
+
 
 ## Quickstart
 
 ```Python
 import appeal
 import sys
 
@@ -2291,15 +2293,29 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
-**0.6**
+**0.6.1**  *2023/07/22*
+
+* Fixed 3.6 and 3.7 support--some equals-sign-in-f-strings
+  uses crept in.
+* Added GitHub Actions integration.  Tests and
+  coverage are run in the cloud after every checkin.
+  Thanks to [Dan Pope](https://github.com/lordmauve)
+  for gently walking me through this!
+* Fixed metadata in the `pyproject.toml` file.
+* Added badges for testing and supported Python
+  versions.  (Didn't add the coverage badge yet...
+  it's too embarassing!)
+
+
+**0.6** *2023/07/20*
 
 A huge upgrade!
 
 * A new feature: Appeal can now read configuration files!
   Check out the new APIs `Appeal.read_mapping`,
   `Appeal.read_iterable`, and even `Appeal.read_csv`.
   This was a massive undertaking and involved a big
```

### Comparing `appeal-0.6/appeal/__init__.py` & `appeal-0.6.1/appeal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 "A powerful & Pythonic command-line parsing library.  Give your program Appeal!"
-__version__ = "0.6"
+__version__ = "0.6.1"
 
 
 # please leave this copyright notice in binary distributions.
 license = """
 appeal/__init__.py
 part of the Appeal software package
 Copyright 2021-2023 by Larry Hastings
@@ -3358,15 +3358,15 @@
                         seen.add(value_id)
                     continue
                 if slot == "callable":
                     value = value.__name__ if value is not None else value
                 elif slot == "address":
                     assert value is not None
                     label_names = ", ".join(f"'{s}'" for s in labels.get(value, ()))
-                    assert label_names, f"didn't have any labels for index {value=}, {labels=}"
+                    assert label_names, f"didn't have any labels for index value={value!r}, labels={labels!r}"
                     value = f"{value} # {label_names}"
                 elif value == empty:
                     value = "(empty)"
                 elif isinstance(value, ArgumentGroup):
                     value = value.summary()
                 else:
                     value = repr(value)
@@ -3605,15 +3605,15 @@
             for op in ops:
                 options.append(denormalize_option(op.option))
                 # these are grouped by program_id, so, op.key will
                 # be the same for all of them
                 if key is None:
                     key = op.key
                 else:
-                    assert key == op.key, f"expected identical keys, but {key=} != {op.key=}"
+                    assert key == op.key, f"expected identical keys, but key {key!r} != op.key {op.key!r}"
             callable = key_to_callable[key]
             full_name = f"{callable.__name__}.{op.parameter.name}"
             option_value = "|".join(options)
             option_values[full_name] = option_value
 
             usage.append("[")
             usage.append(option_value)
@@ -5208,15 +5208,15 @@
             for name, converter in self.kwargs_converters.items():
                 if converter and isinstance(converter, Converter):
                     converter = converter.execute(processor)
                 self.kwargs[name] = converter
         except ValueError as e:
             # we can examine "converter", the exception must have
             # happened in an execute call.
-            raise AppealUsageError(f"invalid value something something {converter=}, {dir(converter)=} {converter.args=}")
+            raise AppealUsageError(f"invalid value something something converter {converter!r}, converter.args={converter.args!r}")
 
     def execute(self, processor):
         executor = processor.execute_preparers(self.callable)
         return executor(*self.args, **self.kwargs)
 
 
 class InferredConverter(Converter):
@@ -5278,15 +5278,15 @@
         return f"<{self.__class__.__name__} {self.callable} args_converters={self.args_converters} kwargs_converters={self.kwargs_converters} value={self.value}>"
 
     def convert(self, processor):
         # if 1:
         if self.value is not None:
             raise RuntimeError("why a second time, fool")
         argument_count = (len(self.args_converters) + len(self.kwargs_converters))
-        assert 0 <= argument_count <= 1, f"{self.__class__.__name__}: {argument_count=}, should be 0 or 1, {self.args_converters=} {self.kwargs_converters=}"
+        assert 0 <= argument_count <= 1, f"{self.__class__.__name__}: argument_count={argument_count!r}, should be 0 or 1, self.args_converters={self.args_converters!r} self.kwargs_converters={self.kwargs_converters!r}"
         if not argument_count:
             # explicitly allow "make -j"
             if self.default is not empty:
                 return self.default
             raise AppealUsageError(f"no argument supplied for {self}, we should have raised an error earlier huh.")
         try:
             if self.kwargs_converters:
```

### Comparing `appeal-0.6/appeal/argument_grouping.py` & `appeal-0.6.1/appeal/argument_grouping.py`

 * *Files identical despite different names*

### Comparing `appeal-0.6/appeal/cpp.py` & `appeal-0.6.1/appeal/cpp.py`

 * *Files identical despite different names*

### Comparing `appeal-0.6/appeal/text.py` & `appeal-0.6.1/appeal/text.py`

 * *Files identical despite different names*

### Comparing `appeal-0.6/appeal/want_prints.py` & `appeal-0.6.1/appeal/want_prints.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     # start block
     if comment:
         assert stripped == if_want_prints, f"failed on line {info.line_number}: expected '{if_want_prints}' but got '{stripped}'"
         append(block_indent + comment_string + if_want_prints)
         continue
 
     # uncomment
-    assert comment_string in line, f"failed on line {info.line_number}: expected {comment_string=} in {line=} but none was found"
+    assert comment_string in line, f"failed on line {info.line_number}: expected comment string {comment_string!r} in line {line} but none was found"
     block_indent, octothorpe, line = line.partition(comment_string)
     assert octothorpe
     # append("## START BLOCK")
     append(block_indent + if_want_prints)
     continue
 
 flush_empty_lines()
```

### Comparing `appeal-0.6/resources/images/appeal.logo.png` & `appeal-0.6.1/resources/images/appeal.logo.png`

 * *Files identical despite different names*

### Comparing `appeal-0.6/resources/images/give.your.program.appeal.png` & `appeal-0.6.1/resources/images/give.your.program.appeal.png`

 * *Files identical despite different names*

### Comparing `appeal-0.6/tests/read_corpus/multiperky1.pky` & `appeal-0.6.1/tests/read_corpus/multiperky1.pky`

 * *Files identical despite different names*

### Comparing `appeal-0.6/tests/read_corpus/starvote_ballots_best_akali_skins.csv` & `appeal-0.6.1/tests/read_corpus/starvote_ballots_best_akali_skins.csv`

 * *Files identical despite different names*

### Comparing `appeal-0.6/tests/test_all.py` & `appeal-0.6.1/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `appeal-0.6/tests/test_read.py` & `appeal-0.6.1/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `appeal-0.6/tests/want_prints_test_corpus/README.md` & `appeal-0.6.1/tests/want_prints_test_corpus/README.md`

 * *Files identical despite different names*

### Comparing `appeal-0.6/tests/want_prints_test_corpus/commented.py` & `appeal-0.6.1/tests/want_prints_test_corpus/commented.py`

 * *Files identical despite different names*

### Comparing `appeal-0.6/tests/want_prints_test_corpus/uncommented.py` & `appeal-0.6.1/tests/want_prints_test_corpus/uncommented.py`

 * *Files identical despite different names*

### Comparing `appeal-0.6/PKG-INFO` & `appeal-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: appeal
-Version: 0.6
+Version: 0.6.1
 Summary: A powerful & Pythonic command-line parsing library.  Give your program Appeal!
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: big >= 0.7.1
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: big >= 0.9.2
 Requires-Dist: perky ; extra == "dev"
 Requires-Dist: tomli ; extra == "dev"
 Project-URL: Source, https://github.com/larryhastings/appeal/
 Provides-Extra: dev
 
 ![## Appeal](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/appeal.logo.png)
 
 ![## Give your program Appeal!](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/give.your.program.appeal.png)
 
 ##### Copyright 2021-2023 by Larry Hastings
 
+[![# test badge](https://img.shields.io/github/actions/workflow/status/larryhastings/appeal/test.yml?branch=master&label=test)](https://github.com/larryhastings/appeal/actions/workflows/test.yml) [![# python versions badge](https://img.shields.io/pypi/pyversions/appeal.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/appeal/)
+
 
 ## Quickstart
 
 ```Python
 import appeal
 import sys
 
@@ -2307,15 +2316,29 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
-**0.6**
+**0.6.1**  *2023/07/22*
+
+* Fixed 3.6 and 3.7 support--some equals-sign-in-f-strings
+  uses crept in.
+* Added GitHub Actions integration.  Tests and
+  coverage are run in the cloud after every checkin.
+  Thanks to [Dan Pope](https://github.com/lordmauve)
+  for gently walking me through this!
+* Fixed metadata in the `pyproject.toml` file.
+* Added badges for testing and supported Python
+  versions.  (Didn't add the coverage badge yet...
+  it's too embarassing!)
+
+
+**0.6** *2023/07/20*
 
 A huge upgrade!
 
 * A new feature: Appeal can now read configuration files!
   Check out the new APIs `Appeal.read_mapping`,
   `Appeal.read_iterable`, and even `Appeal.read_csv`.
   This was a massive undertaking and involved a big
```

