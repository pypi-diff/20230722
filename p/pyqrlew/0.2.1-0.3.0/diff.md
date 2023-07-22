# Comparing `tmp/pyqrlew-0.2.1.tar.gz` & `tmp/pyqrlew-0.3.0.tar.gz`

## Comparing `pyqrlew-0.2.1.tar` & `pyqrlew-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 pyqrlew-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123     4542 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3539 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/.gitignore
--rw-r--r--   0     1001      123      818 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/.readthedocs.yaml
--rw-r--r--   0     1001      123      719 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/CHANGELOG.md
--rw-r--r--   0     1001      123    11357 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/LICENSE
--rw-r--r--   0     1001      123     1466 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/README.md
--rw-r--r--   0     1001      123      634 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/Makefile
--rw-r--r--   0     1001      123     1212 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/conf.py
--rw-r--r--   0     1001      123      224 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/contributing.md
--rw-r--r--   0     1001      123     1786 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/index.md
--rw-r--r--   0     1001      123      800 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/make.bat
--rw-r--r--   0     1001      123       61 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/requirements.txt
--rw-r--r--   0     1001      123    49678 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/PyQrlew.ipynb
--rw-r--r--   0     1001      123   146621 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/demo.ipynb
--rw-r--r--   0     1001      123      431 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/dataset.json
--rw-r--r--   0     1001      123     1032 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/install_db.sql
--rw-r--r--   0     1001      123      234 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/install_db_on_docker.sh
--rw-r--r--   0     1001      123    84990 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/schema.json
--rw-r--r--   0     1001      123    11484 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/size.json
--rw-r--r--   0     1001      123      133 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/requirements.txt
--rw-r--r--   0     1001      123      317 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/simple.py
--rw-r--r--   0     1001      123     1139 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123      112 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/python/pyqrlew/__init__.py
--rw-r--r--   0     1001      123       45 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/python/pyqrlew/io/__init__.py
--rw-r--r--   0     1001      123    10178 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/python/pyqrlew/io/database.py
--rw-r--r--   0     1001      123     2612 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/python/pyqrlew/io/postgresql.py
--rw-r--r--   0     1001      123    13493 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123      136 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/conftest.py
--rw-r--r--   0     1001      123     2481 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/queries/sql_unlimited_queries.sql
--rw-r--r--   0     1001      123     7054 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/queries/valid_queries.sql
--rw-r--r--   0     1001      123      178 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/requirements.txt
--rw-r--r--   0     1001      123     1399 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/test_financial_dataset.py
--rw-r--r--   0     1001      123    45460 2023-07-18 15:28:28.000000 pyqrlew-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pyqrlew-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 pyqrlew-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123     4542 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3539 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/.gitignore
+-rw-r--r--   0     1001      123      818 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/.readthedocs.yaml
+-rw-r--r--   0     1001      123      719 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/CHANGELOG.md
+-rw-r--r--   0     1001      123    11357 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/LICENSE
+-rw-r--r--   0     1001      123     1466 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/README.md
+-rw-r--r--   0     1001      123      634 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/Makefile
+-rw-r--r--   0     1001      123     1212 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/conf.py
+-rw-r--r--   0     1001      123      224 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/contributing.md
+-rw-r--r--   0     1001      123     1786 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/index.md
+-rw-r--r--   0     1001      123      800 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/make.bat
+-rw-r--r--   0     1001      123       61 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/requirements.txt
+-rw-r--r--   0     1001      123    49678 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/PyQrlew.ipynb
+-rw-r--r--   0     1001      123   146621 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/demo.ipynb
+-rw-r--r--   0     1001      123      431 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/dataset.json
+-rw-r--r--   0     1001      123     1032 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/install_db.sql
+-rw-r--r--   0     1001      123      234 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/install_db_on_docker.sh
+-rw-r--r--   0     1001      123    84990 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/schema.json
+-rw-r--r--   0     1001      123    11484 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/size.json
+-rw-r--r--   0     1001      123      133 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/requirements.txt
+-rw-r--r--   0     1001      123      317 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/simple.py
+-rw-r--r--   0     1001      123     1139 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123      112 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/python/pyqrlew/__init__.py
+-rw-r--r--   0     1001      123       45 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/python/pyqrlew/io/__init__.py
+-rw-r--r--   0     1001      123    10178 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/python/pyqrlew/io/database.py
+-rw-r--r--   0     1001      123     2612 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/python/pyqrlew/io/postgresql.py
+-rw-r--r--   0     1001      123    13493 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123      136 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/conftest.py
+-rw-r--r--   0     1001      123     2481 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/queries/sql_unlimited_queries.sql
+-rw-r--r--   0     1001      123     7054 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/queries/valid_queries.sql
+-rw-r--r--   0     1001      123      178 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/requirements.txt
+-rw-r--r--   0     1001      123     1399 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/test_financial_dataset.py
+-rw-r--r--   0     1001      123    48628 2023-07-22 10:43:08.000000 pyqrlew-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pyqrlew-0.3.0/PKG-INFO
```

### Comparing `pyqrlew-0.2.1/.github/workflows/CI.yml` & `pyqrlew-0.3.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/.gitignore` & `pyqrlew-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/.readthedocs.yaml` & `pyqrlew-0.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/CHANGELOG.md` & `pyqrlew-0.3.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/LICENSE` & `pyqrlew-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/README.md` & `pyqrlew-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/docs/Makefile` & `pyqrlew-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/docs/conf.py` & `pyqrlew-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/docs/index.md` & `pyqrlew-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/docs/make.bat` & `pyqrlew-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/examples/PyQrlew.ipynb` & `pyqrlew-0.3.0/examples/PyQrlew.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/examples/demo/demo.ipynb` & `pyqrlew-0.3.0/examples/demo/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/examples/demo/retail_data/install_db.sql` & `pyqrlew-0.3.0/examples/demo/retail_data/install_db.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/examples/demo/retail_data/schema.json` & `pyqrlew-0.3.0/examples/demo/retail_data/schema.json`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/examples/demo/retail_data/size.json` & `pyqrlew-0.3.0/examples/demo/retail_data/size.json`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/pyproject.toml` & `pyqrlew-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = [
   "SQLAlchemy ~= 2.0",
   "psycopg[binary, pool] ~= 3.0",
   "pymysql ~= 1.0",
-  "qrlew-datasets ~= 0.2.6",
+  "qrlew-datasets ~= 0.3.0",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest ~= 7.0",
   "mypy ~= 1.0",
 ]
```

### Comparing `pyqrlew-0.2.1/python/pyqrlew/io/database.py` & `pyqrlew-0.3.0/python/pyqrlew/io/database.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/python/pyqrlew/io/postgresql.py` & `pyqrlew-0.3.0/python/pyqrlew/io/postgresql.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/src/lib.rs` & `pyqrlew-0.3.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/tests/queries/sql_unlimited_queries.sql` & `pyqrlew-0.3.0/tests/queries/sql_unlimited_queries.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/tests/queries/valid_queries.sql` & `pyqrlew-0.3.0/tests/queries/valid_queries.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/tests/test_financial_dataset.py` & `pyqrlew-0.3.0/tests/test_financial_dataset.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.1/Cargo.lock` & `pyqrlew-0.3.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,23 @@
 [[package]]
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
+name = "approx"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "arrayvec"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
 
 [[package]]
 name = "async-trait"
@@ -185,14 +194,20 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "bytemuck"
+version = "1.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
+
+[[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "bytes"
@@ -540,23 +555,14 @@
  "io-lifetimes",
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.10.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
-dependencies = [
- "either",
-]
-
-[[package]]
-name = "itertools"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
@@ -584,14 +590,20 @@
 [[package]]
 name = "libc"
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
+name = "libm"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
+
+[[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
@@ -609,14 +621,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "matrixmultiply"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
+dependencies = [
+ "autocfg",
+ "rawpointer",
+]
+
+[[package]]
 name = "md-5"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6365506850d44bff6e2fbcb5176cf63650e48bd45ef2fe2665ae1570e0f4b9ca"
 dependencies = [
  "digest",
 ]
@@ -645,30 +667,80 @@
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "nalgebra"
+version = "0.29.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d506eb7e08d6329505faa8a3a00a5dcc6de9f76e0c77e4b75763ae3c770831ff"
+dependencies = [
+ "approx",
+ "matrixmultiply",
+ "nalgebra-macros",
+ "num-complex",
+ "num-rational",
+ "num-traits",
+ "rand",
+ "rand_distr",
+ "simba",
+ "typenum",
+]
+
+[[package]]
+name = "nalgebra-macros"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "01fcc0b8149b4632adc89ac3b7b31a12fb6099a0317a4eb2ebff574ef7de7218"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "num-complex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
+name = "num-rational"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
+ "libm",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
@@ -946,56 +1018,57 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyqrlew"
-version = "0.2.1"
+version = "0.3.0"
 dependencies = [
  "pyo3",
  "qrlew",
  "qrlew-sarus",
  "serde_json",
 ]
 
 [[package]]
 name = "qrlew"
-version = "0.1.7"
+version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6481b0b1b1e2e9fce9fffb3626959b8f9445c83e1caa8593745455899b33be16"
+checksum = "4b4449f36c9565aa300af891c90997d5440eafe4a00c93d8d6870e585cbc832a"
 dependencies = [
  "base64",
  "chrono",
  "colored",
  "dot",
  "env_logger",
- "itertools 0.10.5",
+ "itertools",
  "log",
  "paste",
  "postgres",
  "rand",
  "rust_decimal",
  "serde",
  "serde_json",
  "sqlparser",
+ "statrs",
 ]
 
 [[package]]
 name = "qrlew-sarus"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53055cfd1efb7aeeb2ad31ddefe40d661cf778fa44b92e8ddaa8b55930b38e52"
 dependencies = [
  "anyhow",
  "chrono",
  "colored",
  "env_logger",
  "glob",
- "itertools 0.11.0",
+ "itertools",
  "log",
  "paste",
  "protobuf",
  "protobuf-codegen",
  "protobuf-json-mapping",
  "qrlew",
  "serde",
@@ -1044,14 +1117,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
+name = "rand_distr"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
+dependencies = [
+ "num-traits",
+ "rand",
+]
+
+[[package]]
+name = "rawpointer"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
@@ -1156,14 +1245,23 @@
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
+name = "safe_arch"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
+dependencies = [
+ "bytemuck",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "seahash"
@@ -1210,14 +1308,27 @@
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
+name = "simba"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f0b7840f121a46d63066ee7a99fc81dcabbc6105e437cae43528cea199b5a05f"
+dependencies = [
+ "approx",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "wide",
+]
+
+[[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "siphasher"
@@ -1258,22 +1369,35 @@
 dependencies = [
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "sqlparser"
-version = "0.34.0"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "37d3706eefb17039056234df6b566b0014f303f867f2656108334a55b8096f59"
+checksum = "ca597d77c98894be1f965f2e4e2d2a61575d4998088e655476c73715c54b2b43"
 dependencies = [
  "log",
 ]
 
 [[package]]
+name = "statrs"
+version = "0.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2d08e5e1748192713cc281da8b16924fb46be7b0c2431854eadc785823e5696e"
+dependencies = [
+ "approx",
+ "lazy_static",
+ "nalgebra",
+ "num-traits",
+ "rand",
+]
+
+[[package]]
 name = "stringprep"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ee348cb74b87454fff4b551cbf727025810a004f88aeacae7f85b87f4e9a1c1"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
@@ -1588,14 +1712,24 @@
 dependencies = [
  "either",
  "libc",
  "once_cell",
 ]
 
 [[package]]
+name = "wide"
+version = "0.7.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa469ffa65ef7e0ba0f164183697b89b854253fd31aeb92358b7b6155177d62f"
+dependencies = [
+ "bytemuck",
+ "safe_arch",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
```

### Comparing `pyqrlew-0.2.1/PKG-INFO` & `pyqrlew-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pyqrlew
-Version: 0.2.1
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: SQLAlchemy ~= 2.0
 Requires-Dist: psycopg[binary, pool] ~= 3.0
 Requires-Dist: pymysql ~= 1.0
-Requires-Dist: qrlew-datasets ~= 0.2.6
+Requires-Dist: qrlew-datasets ~= 0.3.0
 Requires-Dist: pytest ~= 7.0; extra == 'test'
 Requires-Dist: mypy ~= 1.0; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: A library to manipulate SQL queries, designed with privacy application in mind.
 Keywords: SQL,Privecy,Differential Privacy,AST,Intermediate Representation,Rust
 Author-email: Nicolas Grislain <ng@sarus.tech>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/Qrlew/pyqrlew
-Project-URL: changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
 Project-URL: homepage, https://qrlew.github.io
 Project-URL: documentation, https://pyqrlew.readthedocs.io
+Project-URL: changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
 
 # [Qrlew](https://qrlew.github.io/) framework (by [Sarus](https://www.sarus.tech/))
 Open source SQL manipulation framework written in Rust
 
 ## What is [Qrlew](https://qrlew.github.io/)?
 [Qrlew](https://qrlew.github.io/) is an open source library that aims to parse and compile SQL queries into an Intermediate Representation (IR) that is well-suited for various rewriting tasks. Although it was originally designed for privacy-focused applications, it can be utilized for a wide range of purposes.
```

