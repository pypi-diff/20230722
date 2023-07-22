# Comparing `tmp/pytest-testdox-3.0.1.tar.gz` & `tmp/pytest-testdox-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-testdox-3.0.1.tar", last modified: Tue Apr 19 19:12:25 2022, max compression
+gzip compressed data, was "pytest-testdox-3.1.0.tar", last modified: Sat Jul 22 03:42:43 2023, max compression
```

## Comparing `pytest-testdox-3.0.1.tar` & `pytest-testdox-3.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 19:12:25.750813 pytest-testdox-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-04-19 19:12:25.750813 pytest-testdox-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 19:12:25.750813 pytest-testdox-3.0.1/pytest_testdox/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/pytest_testdox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/pytest_testdox/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/pytest_testdox/formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/pytest_testdox/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4343 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/pytest_testdox/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/pytest_testdox/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 19:12:25.750813 pytest-testdox-3.0.1/pytest_testdox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-04-19 19:12:25.000000 pytest-testdox-3.0.1/pytest_testdox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-04-19 19:12:25.000000 pytest-testdox-3.0.1/pytest_testdox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-19 19:12:25.000000 pytest-testdox-3.0.1/pytest_testdox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-04-19 19:12:25.000000 pytest-testdox-3.0.1/pytest_testdox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-19 19:12:25.000000 pytest-testdox-3.0.1/pytest_testdox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-19 19:12:25.000000 pytest-testdox-3.0.1/pytest_testdox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-04-19 19:12:25.750813 pytest-testdox-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-04-19 19:12:10.000000 pytest-testdox-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 03:42:43.126234 pytest-testdox-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-22 03:42:43.126234 pytest-testdox-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 03:42:43.126234 pytest-testdox-3.1.0/pytest_testdox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/pytest_testdox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/pytest_testdox/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/pytest_testdox/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/pytest_testdox/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/pytest_testdox/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/pytest_testdox/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/pytest_testdox/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 03:42:43.126234 pytest-testdox-3.1.0/pytest_testdox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-22 03:42:43.000000 pytest-testdox-3.1.0/pytest_testdox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-22 03:42:43.000000 pytest-testdox-3.1.0/pytest_testdox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 03:42:43.000000 pytest-testdox-3.1.0/pytest_testdox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 03:42:43.000000 pytest-testdox-3.1.0/pytest_testdox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 03:42:43.000000 pytest-testdox-3.1.0/pytest_testdox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 03:42:43.000000 pytest-testdox-3.1.0/pytest_testdox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-22 03:42:43.126234 pytest-testdox-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-22 03:42:25.000000 pytest-testdox-3.1.0/setup.py
```

### Comparing `pytest-testdox-3.0.1/LICENSE` & `pytest-testdox-3.1.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2016 Renan Ivo Martins <renanivom@gmail.com>
+Copyright (c) 2016-2022 Renan Ivo Martins <renanivom@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pytest-testdox-3.0.1/PKG-INFO` & `pytest-testdox-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: pytest-testdox
-Version: 3.0.1
+Version: 3.1.0
 Summary: A testdox format reporter for pytest
 Home-page: https://github.com/renanivo/pytest-testdox
 Author: Renan Ivo
 Author-email: renanivom@gmail.com
 License: UNKNOWN
 Keywords: pytest testdox test report bdd
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest-testdox
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-testdox.svg?color=brightgreen)](https://pypi.org/project/pytest-testdox/)
 [![Continuous Integration Status](https://github.com/renanivo/pytest-testdox/workflows/Continuous%20Integration/badge.svg)](https://github.com/renanivo/pytest-testdox/actions?query=workflow%3A%22Continuous+Integration%22)
```

### Comparing `pytest-testdox-3.0.1/README.md` & `pytest-testdox-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-testdox-3.0.1/pytest_testdox/formatters.py` & `pytest-testdox-3.1.0/pytest_testdox/formatters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import os
 import re
+from typing import List
 
 TRIM_SPACES_REGEX = r'(^[\s]+|[\s]+$)'
 
 
-def format_title(title, patterns):
+def format_title(title, patterns: List[str]):
     return _remove_patterns(title, patterns).replace('_', ' ').strip()
 
 
-def format_class_name(class_name, patterns):
+def format_class_name(class_name: str, patterns: List[str]):
     formatted = ''
 
     class_name = _remove_patterns(class_name, patterns)
 
     for index, letter in enumerate(class_name):
         if letter.isupper() and _has_lower_letter_besides(index, class_name):
             formatted += ' '
 
         formatted += letter
 
     return formatted.strip()
 
 
-def format_module_name(module_name, patterns):
+def format_module_name(module_name: str, patterns: List[str]):
     return format_title(module_name.split('/')[-1], patterns)
 
 
-def format_result_str(outcome, node_str):
+def format_result_str(outcome: str, node_str: str):
     lines = node_str.split(os.linesep)
     if len(lines) == 1:
         return outcome + node_str
 
     characters_length = len(outcome)
     result = []
     result.append(outcome + lines[0])
@@ -41,33 +42,33 @@
 
         pad = len(line) + characters_length
         result.append(line.rjust(pad))
 
     return os.linesep.join(result)
 
 
-def trim_multi_line_text(text):
+def trim_multi_line_text(text: str):
     return re.sub(TRIM_SPACES_REGEX, '', text, flags=re.MULTILINE)
 
 
-def include_parametrized(title, original_title):
+def include_parametrized(title: str, original_title: str):
     first_bracket = original_title.find('[')
     last_bracket = original_title.rfind(']')
 
     has_parameters = last_bracket > first_bracket
 
     if not has_parameters:
         return title
 
     parameters = original_title[first_bracket + 1 : last_bracket]
 
     return '{title}[{parameters}]'.format(title=title, parameters=parameters)
 
 
-def _remove_patterns(statement, patterns):
+def _remove_patterns(statement: str, patterns: List[str]):
     for glob_pattern in patterns:
         pattern = glob_pattern.replace('*', '')
 
         if glob_pattern.startswith('*'):
             pattern = '{}$'.format(pattern)
             statement = re.sub(pattern, '', statement)
 
@@ -84,12 +85,12 @@
         else:
             pattern = '^{}'.format(pattern)
             statement = re.sub(pattern, '', statement)
 
     return statement
 
 
-def _has_lower_letter_besides(index, string):
+def _has_lower_letter_besides(index: int, string: str):
     letter_before = string[index - 1] if index > 0 else ''
     letter_after = string[index + 1] if index < len(string) - 1 else ''
 
     return letter_before.islower() or letter_after.islower()
```

### Comparing `pytest-testdox-3.0.1/pytest_testdox/models.py` & `pytest-testdox-3.1.0/pytest_testdox/data_structures.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from collections import namedtuple
+from __future__ import annotations
 
-from . import formatters
+from dataclasses import dataclass
+from typing import List, NamedTuple
 
-PatternConfig = namedtuple('PatternConfig', 'files functions classes')
+from _pytest.reports import TestReport
 
+from pytest_testdox import formatters
 
+
+class PatternConfig(NamedTuple):
+    files: List[str]
+    functions: List[str]
+    classes: List[str]
+
+
+@dataclass
 class Node:
-    def __init__(self, title, class_name, module_name):
-        self.title = title
-        self.class_name = class_name
-        self.module_name = module_name
+    module_name: str
+    title: str | None
+    class_name: str | None
 
     def __str__(self):
         return self.title
 
-    def __repr__(self):
-        return '{}(title={!r}, class_name={!r}, module_name={!r})'.format(
-            type(self).__name__, self.title, self.class_name, self.module_name
-        )
-
-    def __eq__(self, other):
-        return (
-            type(self) == type(other)
-            and self.title == other.title
-            and self.class_name == other.class_name
-            and self.module_name == other.module_name
-        )
-
     @classmethod
-    def parse(cls, nodeid, pattern_config, title=None, class_name=None):
+    def parse(
+        cls,
+        nodeid: str,
+        pattern_config: PatternConfig,
+        title: str | None = None,
+        class_name: str | None = None,
+    ):
         node_parts = nodeid.split('::')
 
         if title:
             title = formatters.include_parametrized(
                 formatters.trim_multi_line_text(title), node_parts[-1]
             )
         else:
@@ -55,56 +57,52 @@
                 class_name = formatters.format_class_name(
                     node_parts[-2], pattern_config.classes
                 )
 
         return cls(title=title, class_name=class_name, module_name=module_name)
 
 
+@dataclass(frozen=True)
 class Result:
+    outcome: str
+    node: Node
 
     _OUTCOME_REPRESENTATION = {
         'passed': ' [x] ',
         'failed': ' [ ] ',
         'skipped': ' >>> ',
     }
     _default_outcome_representation = '>>>'
 
-    def __init__(self, outcome, node):
-        self.outcome = outcome
-        self.node = node
-
-    def __repr__(self):
-        return '{}(outcome={!r}, node={!r})'.format(
-            type(self).__name__, self.outcome, self.node
-        )
-
-    def __str__(self):
+    def __str__(self) -> str:
         representation = self._OUTCOME_REPRESENTATION.get(
             self.outcome, self._default_outcome_representation
         )
 
         return formatters.format_result_str(
             outcome=representation, node_str=str(self.node)
         )
 
     @property
-    def header(self):
-        return self.node.class_name or self.node.module_name
+    def header(self) -> str:
+        return self.node.class_name or self.node.module_name  # type: ignore
 
     @property
-    def header_id(self):
+    def header_id(self) -> str:
         """
         Return the same value when the result should be aggregated under the
         same class or module (this is not guaranteed in "header" property,
         which should be used when displaying to the user)
         """
         return self.node.module_name + (self.node.class_name or '')
 
     @classmethod
-    def create(cls, report, pattern_config):
+    def create(
+        cls, report: TestReport, pattern_config: PatternConfig
+    ) -> Result:
         title = getattr(report, 'testdox_title', None)
         class_name = getattr(report, 'testdox_class_name', None)
 
         node = Node.parse(
             nodeid=report.nodeid,
             pattern_config=pattern_config,
             title=title,
```

### Comparing `pytest-testdox-3.0.1/pytest_testdox.egg-info/PKG-INFO` & `pytest-testdox-3.1.0/pytest_testdox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: pytest-testdox
-Version: 3.0.1
+Version: 3.1.0
 Summary: A testdox format reporter for pytest
 Home-page: https://github.com/renanivo/pytest-testdox
 Author: Renan Ivo
 Author-email: renanivom@gmail.com
 License: UNKNOWN
 Keywords: pytest testdox test report bdd
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest-testdox
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-testdox.svg?color=brightgreen)](https://pypi.org/project/pytest-testdox/)
 [![Continuous Integration Status](https://github.com/renanivo/pytest-testdox/workflows/Continuous%20Integration/badge.svg)](https://github.com/renanivo/pytest-testdox/actions?query=workflow%3A%22Continuous+Integration%22)
```

### Comparing `pytest-testdox-3.0.1/setup.py` & `pytest-testdox-3.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,36 +8,35 @@
     path = os.path.join(os.path.dirname(__file__), fname)
     with open(path) as f:
         return f.read()
 
 
 setup(
     name='pytest-testdox',
-    version='3.0.1',
+    version='3.1.0',
     description='A testdox format reporter for pytest',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='Renan Ivo',
     author_email='renanivom@gmail.com',
     url='https://github.com/renanivo/pytest-testdox',
     keywords='pytest testdox test report bdd',
     install_requires=[
         'pytest>=4.6.0',
     ],
     packages=['pytest_testdox'],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: Pytest',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Programming Language :: Python',
```

