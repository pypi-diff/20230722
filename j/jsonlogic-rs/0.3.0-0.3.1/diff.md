# Comparing `tmp/jsonlogic-rs-0.3.0.tar.gz` & `tmp/jsonlogic-rs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonlogic-rs-0.3.0.tar", last modified: Fri Jul 21 20:32:20 2023, max compression
+gzip compressed data, was "jsonlogic-rs-0.3.1.tar", last modified: Sat Jul 22 13:15:41 2023, max compression
```

## Comparing `jsonlogic-rs-0.3.0.tar` & `jsonlogic-rs-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/py/jsonlogic_rs/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/bin.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/func.rs
--rw-r--r--   0 runner    (1001) docker     (123)    41847 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/js_op.rs
--rw-r--r--   0 runner    (1001) docker     (123)    48168 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/src/op/
--rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/array.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/data.rs
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/impure.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/logic.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/string.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/value.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:15:41.796040 jsonlogic-rs-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-07-22 13:15:41.796040 jsonlogic-rs-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:15:41.792040 jsonlogic-rs-0.3.1/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:15:41.792040 jsonlogic-rs-0.3.1/py/jsonlogic_rs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/py/jsonlogic_rs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:15:41.796040 jsonlogic-rs-0.3.1/py/jsonlogic_rs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-07-22 13:15:41.000000 jsonlogic-rs-0.3.1/py/jsonlogic_rs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-22 13:15:41.000000 jsonlogic-rs-0.3.1/py/jsonlogic_rs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 13:15:41.000000 jsonlogic-rs-0.3.1/py/jsonlogic_rs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 13:15:41.000000 jsonlogic-rs-0.3.1/py/jsonlogic_rs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 13:15:41.000000 jsonlogic-rs-0.3.1/py/jsonlogic_rs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 13:15:41.796040 jsonlogic-rs-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:15:41.796040 jsonlogic-rs-0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/bin.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/func.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    41847 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/js_op.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    48168 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:15:41.796040 jsonlogic-rs-0.3.1/src/op/
+-rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/op/array.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/op/data.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/op/impure.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/op/logic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/op/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/op/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/op/string.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-22 13:15:01.000000 jsonlogic-rs-0.3.1/src/value.rs
```

### Comparing `jsonlogic-rs-0.3.0/Cargo.toml` & `jsonlogic-rs-0.3.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 edition = "2018"
 homepage = "https://github.com/bestowinc/json-logic-rs"
 keywords = ["json", "jsonlogic", "s-expressions", "web", "logic"]
 license = "MIT"
 name = "jsonlogic-rs"
 readme = "README.md"
 repository = "https://github.com/bestowinc/json-logic-rs"
-version = "0.3.0"
+version = "0.3.1"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 # cdylib for CFFI and python integration
 # lib for regular rust stuff
 crate-type = ["cdylib", "lib"]
```

### Comparing `jsonlogic-rs-0.3.0/LICENSE` & `jsonlogic-rs-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/PKG-INFO` & `jsonlogic-rs-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonlogic-rs
-Version: 0.3.0
+Version: 0.3.1
 Summary: JsonLogic implemented with a Rust backend
 Home-page: https://www.github.com/bestowinc/json-logic-rs
 Author: Matthew Planchard
 Author-email: msplanchard@gmail.com
 Maintainer-email: msplanchard@gmail.com
 Keywords: json,jsonlogic,s-expressions,rust
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,15 +49,15 @@
 Being built in Rust, we are able to provide the package in a variety of
 languages. The table below describes current language support:
 
 | **Language**         | **Available Via**                                                          |
 | -------------------- | -------------------------------------------------------------------------- |
 | Rust                 | [Cargo](https://crates.io/crates/jsonlogic-rs)                             |
 | JavaScript (as WASM) | Node Package via [NPM](https://www.npmjs.com/package/@bestow/jsonlogic-rs) |
-| Python               | [PyPI](https://test.pypi.org/project/jsonlogic-rs/0.1.0/)                  |
+| Python               | [PyPI](https://pypi.org/project/jsonlogic-rs/)                  |
 
 ## Installation
 
 ### Rust
 
 To use as a Rust library, add to your `Cargo.toml`:
```

### Comparing `jsonlogic-rs-0.3.0/README.md` & `jsonlogic-rs-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 Being built in Rust, we are able to provide the package in a variety of
 languages. The table below describes current language support:
 
 | **Language**         | **Available Via**                                                          |
 | -------------------- | -------------------------------------------------------------------------- |
 | Rust                 | [Cargo](https://crates.io/crates/jsonlogic-rs)                             |
 | JavaScript (as WASM) | Node Package via [NPM](https://www.npmjs.com/package/@bestow/jsonlogic-rs) |
-| Python               | [PyPI](https://test.pypi.org/project/jsonlogic-rs/0.1.0/)                  |
+| Python               | [PyPI](https://pypi.org/project/jsonlogic-rs/)                  |
 
 ## Installation
 
 ### Rust
 
 To use as a Rust library, add to your `Cargo.toml`:
```

### Comparing `jsonlogic-rs-0.3.0/py/jsonlogic_rs/__init__.py` & `jsonlogic-rs-0.3.1/py/jsonlogic_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/PKG-INFO` & `jsonlogic-rs-0.3.1/py/jsonlogic_rs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonlogic-rs
-Version: 0.3.0
+Version: 0.3.1
 Summary: JsonLogic implemented with a Rust backend
 Home-page: https://www.github.com/bestowinc/json-logic-rs
 Author: Matthew Planchard
 Author-email: msplanchard@gmail.com
 Maintainer-email: msplanchard@gmail.com
 Keywords: json,jsonlogic,s-expressions,rust
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,15 +49,15 @@
 Being built in Rust, we are able to provide the package in a variety of
 languages. The table below describes current language support:
 
 | **Language**         | **Available Via**                                                          |
 | -------------------- | -------------------------------------------------------------------------- |
 | Rust                 | [Cargo](https://crates.io/crates/jsonlogic-rs)                             |
 | JavaScript (as WASM) | Node Package via [NPM](https://www.npmjs.com/package/@bestow/jsonlogic-rs) |
-| Python               | [PyPI](https://test.pypi.org/project/jsonlogic-rs/0.1.0/)                  |
+| Python               | [PyPI](https://pypi.org/project/jsonlogic-rs/)                  |
 
 ## Installation
 
 ### Rust
 
 To use as a Rust library, add to your `Cargo.toml`:
```

### Comparing `jsonlogic-rs-0.3.0/setup.py` & `jsonlogic-rs-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/bin.rs` & `jsonlogic-rs-0.3.1/src/bin.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/error.rs` & `jsonlogic-rs-0.3.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/func.rs` & `jsonlogic-rs-0.3.1/src/func.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/js_op.rs` & `jsonlogic-rs-0.3.1/src/js_op.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/lib.rs` & `jsonlogic-rs-0.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/op/array.rs` & `jsonlogic-rs-0.3.1/src/op/array.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/op/data.rs` & `jsonlogic-rs-0.3.1/src/op/data.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/op/logic.rs` & `jsonlogic-rs-0.3.1/src/op/logic.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/op/mod.rs` & `jsonlogic-rs-0.3.1/src/op/mod.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/op/numeric.rs` & `jsonlogic-rs-0.3.1/src/op/numeric.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/op/string.rs` & `jsonlogic-rs-0.3.1/src/op/string.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.0/src/value.rs` & `jsonlogic-rs-0.3.1/src/value.rs`

 * *Files identical despite different names*

