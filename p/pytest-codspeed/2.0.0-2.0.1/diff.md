# Comparing `tmp/pytest_codspeed-2.0.0.tar.gz` & `tmp/pytest_codspeed-2.0.1.tar.gz`

## Comparing `pytest_codspeed-2.0.0.tar` & `pytest_codspeed-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/__init__.py
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/plugin.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/.gitignore
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/__init__.py
--rw-r--r--   0        0        0    26531 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/dist_callgrind_wrapper.c
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/wrapper.c
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/wrapper.h
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/wrapper.pyi
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/LICENSE
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/README.md
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/__init__.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/plugin.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/.gitignore
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/wrapper.c
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/wrapper.h
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/wrapper.pyi
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/README.md
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/PKG-INFO
```

### Comparing `pytest_codspeed-2.0.0/src/pytest_codspeed/plugin.py` & `pytest_codspeed-2.0.1/src/pytest_codspeed/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import gc
 import os
 import pkgutil
 import sys
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import pytest
 from _pytest.fixtures import FixtureManager
 
 from . import __version__
 from ._wrapper import get_lib
 
@@ -162,29 +172,34 @@
     lib: "LibType", nodeId: str, fn: Callable[..., Any], *args, **kwargs
 ):
     is_gc_enabled = gc.isenabled()
     if is_gc_enabled:
         gc.collect()
         gc.disable()
 
+    result = None
+
     def __codspeed_root_frame__():
-        fn(*args, **kwargs)
+        nonlocal result
+        result = fn(*args, **kwargs)
 
     if SUPPORTS_PERF_TRAMPOLINE:
         # Warmup CPython performance map cache
         __codspeed_root_frame__()
 
     lib.zero_stats()
     lib.start_instrumentation()
     __codspeed_root_frame__()
     lib.stop_instrumentation()
     lib.dump_stats_at(f"{nodeId}".encode("ascii"))
     if is_gc_enabled:
         gc.enable()
 
+    return result
+
 
 @pytest.hookimpl(tryfirst=True)
 def pytest_runtest_protocol(item: "pytest.Item", nextitem: Union["pytest.Item", None]):
     plugin = get_plugin(item.config)
     if not plugin.is_codspeed_enabled or not should_benchmark_item(item):
         return (
             None  # Defer to the default test protocol since no benchmarking is needed
@@ -226,30 +241,35 @@
     ihook.pytest_runtest_logreport(report=teardown_report)
     reports.append(teardown_report)
     ihook.pytest_runtest_logfinish(nodeid=item.nodeid, location=item.location)
 
     return reports  # Deny further protocol hooks execution
 
 
+T = TypeVar("T")
+
+
 class BenchmarkFixture:
+    """The fixture that can be used to benchmark a function."""
+
     def __init__(self, request: "pytest.FixtureRequest"):
         self.extra_info: Dict = {}
 
         self._request = request
 
-    def __call__(self, func: Callable[..., Any], *args: Any, **kwargs: Any) -> Any:
+    def __call__(self, func: Callable[..., T], *args: Any, **kwargs: Any) -> T:
         plugin = get_plugin(self._request.config)
         plugin.benchmark_count += 1
         if plugin.is_codspeed_enabled and plugin.should_measure:
             assert plugin.lib is not None
-            _run_with_instrumentation(
+            return _run_with_instrumentation(
                 plugin.lib, self._request.node.nodeid, func, *args, **kwargs
             )
         else:
-            func(*args, **kwargs)
+            return func(*args, **kwargs)
 
 
 @pytest.fixture(scope="function")
 def codspeed_benchmark(request: "pytest.FixtureRequest") -> Callable:
     return BenchmarkFixture(request)
```

### Comparing `pytest_codspeed-2.0.0/src/pytest_codspeed/_wrapper/__init__.py` & `pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-2.0.0/.gitignore` & `pytest_codspeed-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-2.0.0/LICENSE` & `pytest_codspeed-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-2.0.0/README.md` & `pytest_codspeed-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-2.0.0/pyproject.toml` & `pytest_codspeed-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -33,27 +33,27 @@
     "Topic :: System :: Benchmark",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "cffi ~= 1.15.1",
     "pytest>=3.8",
-    "setuptools ~= 67.8.0; python_version >= '3.12'", # FIXME: remove when cffi supports directly python 3.12
+    "setuptools ~= 67.8.0; python_full_version >= '3.12.0b1'", # FIXME: remove when cffi supports directly python 3.12
 ]
 
 [project.optional-dependencies]
 lint = ["black ~= 23.3.0", "isort ~=5.12.0", "mypy ~= 1.3.0", "ruff ~= 0.0.275"]
 compat = ["pytest-benchmark ~= 4.0.0"]
 test = ["pytest ~= 7.0", "pytest-cov ~= 4.0.0"]
 
 [project.entry-points]
 pytest11 = { codspeed = "pytest_codspeed.plugin" }
 
 [tool.hatch.envs.default]
-python = "3.12"
+python = "3.11"
 features = ["lint", "test", "compat"]
 
 [tool.hatch.envs.test]
 features = ["test"]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
```

### Comparing `pytest_codspeed-2.0.0/PKG-INFO` & `pytest_codspeed-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-codspeed
-Version: 2.0.0
+Version: 2.0.1
 Summary: Pytest plugin to create CodSpeed benchmarks
 Project-URL: Homepage, https://codspeed.io/
 Project-URL: Documentation, https://docs.codspeed.io/
 Project-URL: Source, https://github.com/CodSpeedHQ/pytest-codspeed
 Author-email: Arthur Pastel <arthur@codspeed.io>
 License: The MIT License (MIT)
         
@@ -44,15 +44,15 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Benchmark
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: cffi~=1.15.1
 Requires-Dist: pytest>=3.8
-Requires-Dist: setuptools~=67.8.0; python_version >= '3.12'
+Requires-Dist: setuptools~=67.8.0; python_full_version >= '3.12.0b1'
 Provides-Extra: compat
 Requires-Dist: pytest-benchmark~=4.0.0; extra == 'compat'
 Provides-Extra: lint
 Requires-Dist: black~=23.3.0; extra == 'lint'
 Requires-Dist: isort~=5.12.0; extra == 'lint'
 Requires-Dist: mypy~=1.3.0; extra == 'lint'
 Requires-Dist: ruff~=0.0.275; extra == 'lint'
```

