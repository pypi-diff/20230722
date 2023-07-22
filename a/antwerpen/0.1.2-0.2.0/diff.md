# Comparing `tmp/antwerpen-0.1.2.tar.gz` & `tmp/antwerpen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antwerpen-0.1.2.tar", max compression
+gzip compressed data, was "antwerpen-0.2.0.tar", max compression
```

## Comparing `antwerpen-0.1.2.tar` & `antwerpen-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-07-22 15:45:23.102554 antwerpen-0.1.2/LICENSE
--rw-r--r--   0        0        0     8479 2023-07-22 15:45:23.102554 antwerpen-0.1.2/README.md
--rw-r--r--   0        0        0     3760 2023-07-22 15:45:39.062557 antwerpen-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      341 2023-07-22 15:45:23.102554 antwerpen-0.1.2/src/antwerpen/__init__.py
--rw-r--r--   0        0        0     4543 2023-07-22 15:45:23.102554 antwerpen-0.1.2/src/antwerpen/antwerpen.py
--rw-r--r--   0        0        0      290 2023-07-22 15:45:23.102554 antwerpen-0.1.2/src/antwerpen/exceptions.py
--rw-r--r--   0        0        0     1854 2023-07-22 15:45:23.102554 antwerpen-0.1.2/src/antwerpen/models.py
--rw-r--r--   0        0        0        0 2023-07-22 15:45:23.102554 antwerpen-0.1.2/src/antwerpen/py.typed
--rw-r--r--   0        0        0     9817 1970-01-01 00:00:00.000000 antwerpen-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-22 19:49:07.752493 antwerpen-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8478 2023-07-22 19:49:07.752493 antwerpen-0.2.0/README.md
+-rw-r--r--   0        0        0     3760 2023-07-22 19:49:22.036670 antwerpen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-07-22 19:49:07.756493 antwerpen-0.2.0/src/antwerpen/__init__.py
+-rw-r--r--   0        0        0     4543 2023-07-22 19:49:07.756493 antwerpen-0.2.0/src/antwerpen/antwerpen.py
+-rw-r--r--   0        0        0      290 2023-07-22 19:49:07.756493 antwerpen-0.2.0/src/antwerpen/exceptions.py
+-rw-r--r--   0        0        0     1849 2023-07-22 19:49:07.756493 antwerpen-0.2.0/src/antwerpen/models.py
+-rw-r--r--   0        0        0        0 2023-07-22 19:49:07.756493 antwerpen-0.2.0/src/antwerpen/py.typed
+-rw-r--r--   0        0        0     9816 1970-01-01 00:00:00.000000 antwerpen-0.2.0/PKG-INFO
```

### Comparing `antwerpen-0.1.2/LICENSE` & `antwerpen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antwerpen-0.1.2/README.md` & `antwerpen-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 pip install antwerpen
 ```
 
 ## Datasets
 
 You can read the following datasets with this package:
 
-- [Disabled parking spaces / Parkeerplaatsen voor personen met een handicap][disabled_parkings] (1666 locations)
+- [Disabled parking spaces / Parkeerplaatsen voor personen met een handicap][disabled_parkings] (1664 locations)
 
 ---
 
 There are a number of parameters you can set to retrieve the data:
 
 - **limit** (default: 10) - How many results you want to retrieve.
 
@@ -50,15 +50,15 @@
 ### Disabled parking spaces
 
 | Variable | Type | Description |
 | :------- | :--- | :---------- |
 | `entry_id` | integer | The ID of this location |
 | `number` | integer | The number of parking spots on this location |
 | `orientation` | string | The orientation of this location |
-| `destination` | string | The destination of this location |
+| `destiny` | string | What is the purpose of the location |
 | `window_time` | string (none) | The window time of this location |
 | `lined` | boolean | Whether this location is lined |
 | `status` | string | The status of this location |
 | `gis_id` | string | The GIS ID of this location |
 | `created_at` | datetime | The date this location was added to the dataset, not all locations have a value |
 | `coordinates` | list (float) | The coordinates of this location |
```

### Comparing `antwerpen-0.1.2/pyproject.toml` & `antwerpen-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antwerpen"
-version = "0.1.2"
+version = "0.2.0"
 description = "Asynchronous Python client providing Open Data information of Antwerpen"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-antwerpen"
 repository = "https://github.com/klaasnicolaas/python-antwerpen"
@@ -32,15 +32,15 @@
 pytz = "^2023.3"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-antwerpen/issues"
 Changelog = "https://github.com/klaasnicolaas/python-antwerpen/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.0.278"
+ruff = "0.0.280"
 aresponses = "2.1.6"
 black = "23.7.0"
 blacken-docs = "1.15.0"
 codespell = "2.2.5"
 coverage = {version = "7.2.7", extras = ["toml"]}
 mypy = "1.4.1"
 pre-commit = "3.3.3"
```

### Comparing `antwerpen-0.1.2/src/antwerpen/antwerpen.py` & `antwerpen-0.2.0/src/antwerpen/antwerpen.py`

 * *Files identical despite different names*

### Comparing `antwerpen-0.1.2/src/antwerpen/models.py` & `antwerpen-0.2.0/src/antwerpen/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 @dataclass
 class DisabledParking:
     """Object representing a disabled parking."""
 
     entry_id: int
     number: int
     orientation: str
-    destination: str
+    destiny: str
     window_time: str | None
     lined: bool
     status: str
     gis_id: str
     created_at: datetime | None
     coordinates: list[float]
 
@@ -36,21 +36,21 @@
             A DisabledParking object.
         """
         attr = data["properties"]
         return cls(
             entry_id=attr.get("OBJECTID"),
             number=attr.get("Capaciteit"),
             orientation=attr.get("Orientatie"),
-            destination=attr.get("Bestemming"),
+            destiny=attr.get("Bestemming"),
             window_time=attr.get("VENSTERTIJD_BESCHR"),
             lined=attr.get("GELIJND") == "Ja",
             status=attr.get("STATUS"),
             gis_id=attr.get("GISID"),
             created_at=fromtimestamp(attr.get("EBDD")),
-            coordinates=data["geometry"]["coordinates"],
+            coordinates=data["geometry"]["coordinates"][0],
         )
 
 
 def fromtimestamp(epoch_time: int, default: None = None) -> Any:
     """Fromtimestamp function with default value.
 
     Args:
```

### Comparing `antwerpen-0.1.2/PKG-INFO` & `antwerpen-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antwerpen
-Version: 0.1.2
+Version: 0.2.0
 Summary: Asynchronous Python client providing Open Data information of Antwerpen
 Home-page: https://github.com/klaasnicolaas/python-antwerpen
 License: MIT
 Keywords: open,data,platform,antwerpen,parking,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -62,15 +62,15 @@
 pip install antwerpen
 ```
 
 ## Datasets
 
 You can read the following datasets with this package:
 
-- [Disabled parking spaces / Parkeerplaatsen voor personen met een handicap][disabled_parkings] (1666 locations)
+- [Disabled parking spaces / Parkeerplaatsen voor personen met een handicap][disabled_parkings] (1664 locations)
 
 ---
 
 There are a number of parameters you can set to retrieve the data:
 
 - **limit** (default: 10) - How many results you want to retrieve.
 
@@ -80,15 +80,15 @@
 ### Disabled parking spaces
 
 | Variable | Type | Description |
 | :------- | :--- | :---------- |
 | `entry_id` | integer | The ID of this location |
 | `number` | integer | The number of parking spots on this location |
 | `orientation` | string | The orientation of this location |
-| `destination` | string | The destination of this location |
+| `destiny` | string | What is the purpose of the location |
 | `window_time` | string (none) | The window time of this location |
 | `lined` | boolean | Whether this location is lined |
 | `status` | string | The status of this location |
 | `gis_id` | string | The GIS ID of this location |
 | `created_at` | datetime | The date this location was added to the dataset, not all locations have a value |
 | `coordinates` | list (float) | The coordinates of this location |
```

