# Comparing `tmp/ilcdlib-0.9.0.tar.gz` & `tmp/ilcdlib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-0.9.0.tar", max compression
+gzip compressed data, was "ilcdlib-1.0.0.tar", max compression
```

## Comparing `ilcdlib-0.9.0.tar` & `ilcdlib-1.0.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/LICENSE
--rw-r--r--   0        0        0     4949 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/README.md
--rw-r--r--   0        0        0     3489 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17413 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0     1796 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     4431 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     6375 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     2665 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     3638 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     2749 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3774 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     3304 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     1329 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2051 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3328 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    32071 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2050 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7667 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1900 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     1892 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     1737 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1705 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0    10655 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     1206 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     3329 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6059 1970-01-01 00:00:00.000000 ilcdlib-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-22 15:14:55.076063 ilcdlib-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5311 2023-07-22 15:14:55.076063 ilcdlib-1.0.0/README.md
+-rw-r--r--   0        0        0     3489 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17587 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0     1796 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     4431 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     6375 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     3361 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     3638 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     2749 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3774 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2023-07-22 15:14:55.080063 ilcdlib-1.0.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     3399 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     1329 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2051 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3328 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    32071 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2050 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7667 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1900 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     1892 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     1737 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1705 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    10655 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     2513 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/soda4lca/api_client_4x.py
+-rw-r--r--   0        0        0     1206 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     3329 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2023-07-22 15:14:55.084063 ilcdlib-1.0.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6421 1970-01-01 00:00:00.000000 ilcdlib-1.0.0/PKG-INFO
```

### Comparing `ilcdlib-0.9.0/LICENSE` & `ilcdlib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/README.md` & `ilcdlib-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,21 @@
 If you don't need CLI tool, you can omit `cli` extra. The following extras are available:
 
 * `lxml` - install lxml library for faster XML parsing
 * `cli` - install CLI tool so it could be used from command line via `ilcdtool` command.
 
 ## Usage
 
+**❗ ATTENTION**: Pick the right version. There are 2 versions of the library available:
+
+* Use version **below** `2.0.0` if your project uses Pydantic version below `2.0.0`
+* Use version `2.x.x` or higher if your project uses Pydantic version `2.0.0` or above
+
+Branch 1.x.x is not maintained anymore, so if you don't use pydantic 2.x.x should be your choice.
+
 ### CLI
 
 At the moment the primary function of the CLI tool is to convert ILCD XML files to openEPD (json) format. 
 
 Here is a simple example of how to use it to convert ILCD archive to openEPD format:
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -11,18 +11,23 @@
            github/v/release/cchangelabs/ilcdlib?style=for-the-badge]
 Python library providing parsing capabilities for ILCD XML files. ##
 Installation Install the library from PyPi. The following command will install
 the library with all optional dependencies: ```bash pip install "ilcdlib
 [lxml,cli]" ``` If you don't need CLI tool, you can omit `cli` extra. The
 following extras are available: * `lxml` - install lxml library for faster XML
 parsing * `cli` - install CLI tool so it could be used from command line via
-`ilcdtool` command. ## Usage ### CLI At the moment the primary function of the
-CLI tool is to convert ILCD XML files to openEPD (json) format. Here is a
-simple example of how to use it to convert ILCD archive to openEPD format:
-```bash ilcdtool --debug convert-epd -i ilcd+epd -o openEPD "
+`ilcdtool` command. ## Usage **â ATTENTION**: Pick the right version. There
+are 2 versions of the library available: * Use version **below** `2.0.0` if
+your project uses Pydantic version below `2.0.0` * Use version `2.x.x` or
+higher if your project uses Pydantic version `2.0.0` or above Branch 1.x.x is
+not maintained anymore, so if you don't use pydantic 2.x.x should be your
+choice. ### CLI At the moment the primary function of the CLI tool is to
+convert ILCD XML files to openEPD (json) format. Here is a simple example of
+how to use it to convert ILCD archive to openEPD format: ```bash ilcdtool --
+debug convert-epd -i ilcd+epd -o openEPD "
 o/archive.zip>" ``` It is also possible to point the tool to the http endpoint
 instead. At the moment Soda4Lca web UI and api endpoints are supported. ```bash
 ilcdtool convert-epd -i ilcd+epd -o openEPD "https://oekobaudat.de/OEKOBAU.DAT/
 datasetdetail/process.xhtml?uuid=ee8863aa-7276-4896-b07a-
 713937a3134d&version=00.00.018&stock=OBD_2021_II〈=en" ``` Another important
 feature is the ability to specify a **dialect**. Dialect is a set of rules that
 define how the handle provider specific data. It is useful for the cases when
```

### Comparing `ilcdlib-0.9.0/pyproject.toml` & `ilcdlib-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "0.9.0"
+version = "1.0.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
@@ -22,15 +22,15 @@
 [tool.poetry.scripts]
 ilcdtool = { callable = "ilcdlib:cli.entrypoint", extras = ["cli"] }
 
 [tool.poetry.dependencies]
 python = "^3.11"
 urllib3 = { version = ">=1.26.16,<2.0.0" }
 requests = { version = ">=2.1.0,<3.0.0" }
-openepd = { version = ">=0.11.1,<1.0.0" }
+openepd = { version = ">=0.11.1,<2.0.0" }
 
 # Optional dependencies
 lxml = { version = "~=4.9.2", optional = true }
 cli-rack = { version = ">=1.0.6", optional = true }
 
 [tool.poetry.dev-dependencies]
 wheel = { version ="~=0.40.0" }
@@ -60,15 +60,15 @@
 types-urllib3 = ">=1.26.2"
 
 [tool.poetry.extras]
 lxml = ["lxml"]
 cli = ["cli-rack"]
 
 [tool.commitizen]
-version = "0.9.0"
+version = "1.0.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/ilcdlib/__version__.py",
 ]
```

### Comparing `ilcdlib-0.9.0/src/ilcdlib/__init__.py` & `ilcdlib-1.0.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/__main__.py` & `ilcdlib-1.0.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/__version__.py` & `ilcdlib-1.0.0/src/ilcdlib/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.9.0"
+VERSION = "1.0.0"
```

### Comparing `ilcdlib-0.9.0/src/ilcdlib/cli.py` & `ilcdlib-1.0.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/common.py` & `ilcdlib-1.0.0/src/ilcdlib/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import abc
 import datetime
+import logging
 from typing import IO, Literal, Self, Sequence, TextIO, overload
 
 from openepd.model.epd import Epd
 from openepd.model.lcia import Impacts
 from openepd.model.pcr import Pcr
 
 from ilcdlib.const import IlcdDatasetType
@@ -193,14 +194,15 @@
                 fp="http://lca.jrc.it/ILCD/FlowProperty",
                 mm="http://www.matml.org/",
                 epd2013="http://www.iai.kit.edu/EPD/2013",
                 epd2019="http://www.iai.kit.edu/EPD/2019",
                 epd2019_indata="http://www.indata.network/EPD/2019",
             )
         )
+        self.__logger = logging.Logger(__name__)
 
     def remap_xml_ns(self, doc_ns_map: dict[str, str]) -> None:
         """Remap XML namespaces."""
         for n, url in doc_ns_map.items():
             if url and url.endswith("EPD/2019"):  # Some providers use outdated, non-standard namespace
                 self.xml_parser.xml_ns["epd2019"] = url
 
@@ -361,15 +363,19 @@
         :param root: The root element to search in.
         :param path: The path to the reference element (xpath in a form of tuple or string).
         :return: XML Element or None if not found.
         """
         ref = self._get_reference(root, path)
         if ref is None:
             return None
-        return self.get_xml_tree(ref.entity_type, ref.entity_id, ref.entity_version, allow_static_datasets=True)
+        try:
+            return self.get_xml_tree(ref.entity_type, ref.entity_id, ref.entity_version, allow_static_datasets=True)
+        except ValueError as e:
+            self.__logger.warning(e)
+            return None
 
     def _get_external_binary(self, root: T_ET.Element, path: XmlPath) -> IO[bytes] | None:
         """
         Read binary object from element reference.
 
         Path param must point to the reference element (xml element with refObjectId, type, [version]) attributes.
         This method will locate the reference, and then read the binary object from the referenced entity.
```

### Comparing `ilcdlib-0.9.0/src/ilcdlib/const.py` & `ilcdlib-1.0.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-1.0.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/dto.py` & `ilcdlib-1.0.0/src/ilcdlib/dto.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/category.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/category.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,23 +28,39 @@
     def __init__(
         self,
         element: T_ET.Element,
     ):
         super().__init__(NoopBaseReader())
         self._entity = element
         self.xml_parser.xml_ns["cat"] = "http://lca.jrc.it/ILCD/Categories"
+        self.xml_parser.xml_ns["sapi"] = "http://www.ilcd-network.org/ILCD/ServiceAPI"
 
     def get_categories_flat_list(self, data_type: str) -> list[Category]:
         """Get the UUID of the entity described by this data set."""
         result: list[Category] = []
         root = self._get_all_els(self._entity, (f'cat:categories[@dataType="{data_type}"]',))
         for x in root:
             self.__process_categories(x, result, [])
         return result
 
+    def get_categories_flat_list_4x(self, parent: Category | None = None) -> list[Category]:
+        """Get list of categories from XML for Soda4lca 4.x."""
+        result: list[Category] = []
+        root = self._get_all_els(self._entity, ("sapi:category",))
+        for x in root:
+            result.append(
+                Category(
+                    id=x.attrib.get("classId"),
+                    name=x.text,
+                    parent_id=parent.id if parent else None,
+                    full_path=([parent.name] if parent else []) + [x.text],
+                )
+            )
+        return result
+
     def __process_categories(
         self, current_el: T_ET.Element, result: list[Category], parent_cats: list[Category]
     ) -> list[Category]:
         parent_id = current_el.attrib.get("id") if current_el.attrib else None
         processed_categories: list[Category] = []
         for cat_el in self._get_all_els(current_el, ("cat:category",)):
             cat_id = cat_el.attrib.get("id") if cat_el.attrib else None
```

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/contact.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/exchage.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/exchage.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/flow.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/material.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/source.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/unit.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/entity/validation.py` & `ilcdlib-1.0.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-1.0.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/epd/cli.py` & `ilcdlib-1.0.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-1.0.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-1.0.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,24 +35,29 @@
             (
                 "process:modellingAndValidation",
                 "process:dataSourcesTreatmentAndRepresentativeness",
                 "process:referenceToDataSource",
             ),
         )
 
-        return (
+        url = (
             self._get_localized_text(
                 element,
                 ("source:sourceInformation", "source:dataSetInformation", "source:sourceDescriptionOrComment"),
                 lang,
             )
             if element
             else None
         )
 
+        if not url or "environdec.com" not in url:
+            return None
+
+        return url
+
     def get_validity_ends_date(self) -> datetime.date | None:
         """Return the date the EPD is valid until."""
         descr = self.__get_time_repr_description()
         if descr and self._TIME_REPR_DESC_DELIMITER in descr:
             try:
                 date_str = descr.split(self._TIME_REPR_DESC_DELIMITER)[1].strip().rsplit(" ", 1)[-1].strip()
                 return datetime.date.fromisoformat(date_str)
```

### Comparing `ilcdlib-0.9.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-1.0.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-1.0.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/epd/factory.py` & `ilcdlib-1.0.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/epd/reader.py` & `ilcdlib-1.0.0/src/ilcdlib/epd/reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/extension.py` & `ilcdlib-1.0.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/http_common.py` & `ilcdlib-1.0.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-1.0.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/mapping/common.py` & `ilcdlib-1.0.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-1.0.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-1.0.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-1.0.0/src/ilcdlib/mapping/impacts.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-1.0.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-1.0.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/mapping/units.py` & `ilcdlib-1.0.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-1.0.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/medium/archive.py` & `ilcdlib-1.0.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-1.0.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/reference_data.py` & `ilcdlib-1.0.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-1.0.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-1.0.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-1.0.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/sanitizing/text.py` & `ilcdlib-1.0.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-1.0.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-1.0.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/type.py` & `ilcdlib-1.0.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/utils.py` & `ilcdlib-1.0.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/src/ilcdlib/xml_parser.py` & `ilcdlib-1.0.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.9.0/PKG-INFO` & `ilcdlib-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 0.9.0
+Version: 1.0.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: cli
 Provides-Extra: lxml
 Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml"
-Requires-Dist: openepd (>=0.11.1,<1.0.0)
+Requires-Dist: openepd (>=0.11.1,<2.0.0)
 Requires-Dist: requests (>=2.1.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/cchangelabs/ilcdlib
 Description-Content-Type: text/markdown
 
 # ILCD Lib
 
@@ -54,14 +54,21 @@
 If you don't need CLI tool, you can omit `cli` extra. The following extras are available:
 
 * `lxml` - install lxml library for faster XML parsing
 * `cli` - install CLI tool so it could be used from command line via `ilcdtool` command.
 
 ## Usage
 
+**❗ ATTENTION**: Pick the right version. There are 2 versions of the library available:
+
+* Use version **below** `2.0.0` if your project uses Pydantic version below `2.0.0`
+* Use version `2.x.x` or higher if your project uses Pydantic version `2.0.0` or above
+
+Branch 1.x.x is not maintained anymore, so if you don't use pydantic 2.x.x should be your choice.
+
 ### CLI
 
 At the moment the primary function of the CLI tool is to convert ILCD XML files to openEPD (json) format. 
 
 Here is a simple example of how to use it to convert ILCD archive to openEPD format:
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 0.9.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 1.0.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Provides-Extra: cli
 Provides-Extra: lxml Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml" Requires-Dist: openepd
-(>=0.11.1,<1.0.0) Requires-Dist: requests (>=2.1.0,<3.0.0) Requires-Dist:
+(>=0.11.1,<2.0.0) Requires-Dist: requests (>=2.1.0,<3.0.0) Requires-Dist:
 urllib3 (>=1.26.16,<2.0.0) Project-URL: Repository, https://github.com/
 cchangelabs/ilcdlib Description-Content-Type: text/markdown # ILCD Lib
      [https://img.shields.io/pypi/l/ilcdlib?style=for-the-badge] [https://
      img.shields.io/pypi/pyversions/ilcdlib?style=for-the-badge] [https://
  img.shields.io/badge/Code%20Style-black-black?style=for-the-badge] [https://
   img.shields.io/pypi/v/ilcdlib?style=for-the-badge] [https://img.shields.io/
                      pypi/dm/ilcdlib?style=for-the-badge]
@@ -25,18 +25,23 @@
            github/v/release/cchangelabs/ilcdlib?style=for-the-badge]
 Python library providing parsing capabilities for ILCD XML files. ##
 Installation Install the library from PyPi. The following command will install
 the library with all optional dependencies: ```bash pip install "ilcdlib
 [lxml,cli]" ``` If you don't need CLI tool, you can omit `cli` extra. The
 following extras are available: * `lxml` - install lxml library for faster XML
 parsing * `cli` - install CLI tool so it could be used from command line via
-`ilcdtool` command. ## Usage ### CLI At the moment the primary function of the
-CLI tool is to convert ILCD XML files to openEPD (json) format. Here is a
-simple example of how to use it to convert ILCD archive to openEPD format:
-```bash ilcdtool --debug convert-epd -i ilcd+epd -o openEPD "
+`ilcdtool` command. ## Usage **â ATTENTION**: Pick the right version. There
+are 2 versions of the library available: * Use version **below** `2.0.0` if
+your project uses Pydantic version below `2.0.0` * Use version `2.x.x` or
+higher if your project uses Pydantic version `2.0.0` or above Branch 1.x.x is
+not maintained anymore, so if you don't use pydantic 2.x.x should be your
+choice. ### CLI At the moment the primary function of the CLI tool is to
+convert ILCD XML files to openEPD (json) format. Here is a simple example of
+how to use it to convert ILCD archive to openEPD format: ```bash ilcdtool --
+debug convert-epd -i ilcd+epd -o openEPD "
 o/archive.zip>" ``` It is also possible to point the tool to the http endpoint
 instead. At the moment Soda4Lca web UI and api endpoints are supported. ```bash
 ilcdtool convert-epd -i ilcd+epd -o openEPD "https://oekobaudat.de/OEKOBAU.DAT/
 datasetdetail/process.xhtml?uuid=ee8863aa-7276-4896-b07a-
 713937a3134d&version=00.00.018&stock=OBD_2021_II〈=en" ``` Another important
 feature is the ability to specify a **dialect**. Dialect is a set of rules that
 define how the handle provider specific data. It is useful for the cases when
```

