# Comparing `tmp/tmxpy-0.1.1.tar.gz` & `tmp/tmxpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmxpy-0.1.1.tar", last modified: Tue Jul 18 20:14:06 2023, max compression
+gzip compressed data, was "tmxpy-0.1.3.tar", last modified: Sat Jul 22 11:39:04 2023, max compression
```

## Comparing `tmxpy-0.1.1.tar` & `tmxpy-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 20:14:06.097128 tmxpy-0.1.1/
--rw-rw-rw-   0        0        0    35802 2023-07-18 17:55:20.000000 tmxpy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1387 2023-07-18 20:14:06.096128 tmxpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      820 2023-07-18 17:45:31.000000 tmxpy-0.1.1/README.md
--rw-rw-rw-   0        0        0      719 2023-07-18 19:53:49.000000 tmxpy-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 20:14:06.097128 tmxpy-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 20:14:06.075109 tmxpy-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 20:14:06.084118 tmxpy-0.1.1/src/tmxpy/
--rw-rw-rw-   0        0        0       24 2023-07-18 19:54:39.000000 tmxpy-0.1.1/src/tmxpy/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-07-18 20:12:31.000000 tmxpy-0.1.1/src/tmxpy/tmxpy.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:14:06.094125 tmxpy-0.1.1/src/tmxpy.egg-info/
--rw-rw-rw-   0        0        0     1387 2023-07-18 20:14:06.000000 tmxpy-0.1.1/src/tmxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-18 20:14:06.000000 tmxpy-0.1.1/src/tmxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 20:14:06.000000 tmxpy-0.1.1/src/tmxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-18 20:14:06.000000 tmxpy-0.1.1/src/tmxpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 20:14:06.000000 tmxpy-0.1.1/src/tmxpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 11:39:04.477935 tmxpy-0.1.3/
+-rw-rw-rw-   0        0        0    35802 2023-07-18 17:55:20.000000 tmxpy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1387 2023-07-22 11:39:04.476935 tmxpy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2023-07-18 17:45:31.000000 tmxpy-0.1.3/README.md
+-rw-rw-rw-   0        0        0      719 2023-07-22 11:38:46.000000 tmxpy-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 11:39:04.477935 tmxpy-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 11:39:04.455763 tmxpy-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 11:39:04.464769 tmxpy-0.1.3/src/tmxpy/
+-rw-rw-rw-   0        0        0       46 2023-07-19 11:58:59.000000 tmxpy-0.1.3/src/tmxpy/__init__.py
+-rw-rw-rw-   0        0        0     6793 2023-07-22 11:30:01.000000 tmxpy-0.1.3/src/tmxpy/tmxpy.py
+drwxrwxrwx   0        0        0        0 2023-07-22 11:39:04.474933 tmxpy-0.1.3/src/tmxpy.egg-info/
+-rw-rw-rw-   0        0        0     1387 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/top_level.txt
```

### Comparing `tmxpy-0.1.1/LICENSE` & `tmxpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tmxpy-0.1.1/PKG-INFO` & `tmxpy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmxpy
-Version: 0.1.1
+Version: 0.1.3
 Summary: A Python library for reading and writing TMX files.
 Author-email: AnotherPillow <redacted@email.xyz>
 Project-URL: Homepage, https://github.com/AnotherPillow/tmxpy
 Project-URL: Bug Tracker, https://github.com/AnotherPillow/tmxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `tmxpy-0.1.1/README.md` & `tmxpy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tmxpy-0.1.1/pyproject.toml` & `tmxpy-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tmxpy"
-version = "0.1.1"
+version = "0.1.3"
 authors = [
   { name="AnotherPillow", email="redacted@email.xyz" }
 ]
 description = "A Python library for reading and writing TMX files."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tmxpy-0.1.1/src/tmxpy/tmxpy.py` & `tmxpy-0.1.3/src/tmxpy/tmxpy.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,41 @@
 from collections.abc import Sequence
 from typing import cast
 
 # def hello(string: str) -> str:
 #     """Returns a string with a greeting."""
 #     return f"Hello, {string}!"
 
+def convertMapNameToFile(name: str) -> str:
+    match name:
+        case "IslandSouth":
+            return "Island_S"
+        case "IslandWest":
+            return "Island_W"
+        case "IslandNorth":
+            return "Island_N"
+        case "IslandEast":
+            return "Island_E"
+        case "IslandFarmCave":
+            return "Island_FarmCave"
+        case "CaptainRoom":
+            return "Island_CaptainRoom"
+        case "IslandSouthEast":
+            return "Island_SE"
+        case "IslandFieldOffice":
+            return "Island_FieldOffice"
+        case "IslandHut":
+            return "Island_Hut"
+        case "IslandShrine":
+            return "Island_Shrine"
+        case _:
+            return name
+        
+
+
 class TMXpy:
     spriteSheetFolderPaths: Sequence[Path|str] = []
     inputFile: bs4.BeautifulSoup
     tileDimensions: tuple[int, int] = (0, 0)
     tmxDimensions: tuple[int, int] = (0, 0)
     tiles: dict = {}
 
@@ -24,14 +51,15 @@
             self.inputFile = bs4.BeautifulSoup(open(path), "xml")
         elif xml != '':
             self.inputFile = bs4.BeautifulSoup(xml, "xml")
         else:
             raise Exception("TMXpy: No path or xml given")
 
         self.spriteSheetFolderPaths = sheets
+
     
     def generateGIDDict(self) -> None:
         """Generates a dictionary of GIDs to tile information"""
         tilesets = self.inputFile.find_all("tileset")
         layer1 = cast(dict, self.inputFile.find('layer'))
 
         
@@ -103,21 +131,47 @@
                 continue
             print(f'Rendering layer {layer["name"]} - {i}')
             layer = self.renderLayer(i)
             #stick it on top of the last layer, and not overwriting the transparent pixels
             img.paste(layer, (0, 0), layer)
             print(f'Layer {i} rendered, layer width: {layer.width}, layer height: {layer.height} - img width: {width}, img height: {height}')
         return img
-            
+    
+    def parseWarps(self) -> list[dict]:
+        #extract property[name="Warp"]
+        prop = cast(dict, self.inputFile.find("property", {"name": "Warp"}))
+        if prop is None or prop == {}:
+            return []
+        
+        value = prop["value"].split(" ")
+
+        #seperate value into a list of warps, each is 5 elements long
+        warps_list = [value[i:i + 5] for i in range(0, len(value), 5)]
+
+        warps = []
+        for warp in warps_list:
+            warps.append({
+                "map_x": int(warp[0]),
+                "map_y": int(warp[1]),
+                "destination": warp[2],
+                "dest_x": int(warp[3]),
+                "dest_y": int(warp[4]),
+            })
 
+        self.warps = warps
 
+        return warps
+    
+    def replace_warp(self, index: int, warp: dict):
+        if 'warps' not in self.__dict__:
+            self.parseWarps()
+        self.warps[index] = warp
 
-        
-        
 
+    def save(self, path: str or Path):
 
-        
+        self.inputFile.find("property", {"name": "Warp"})['value'] = " ".join([f"{w['map_x']} {w['map_y']} {w['destination']} {w['dest_x']} {w['dest_y']}" for w in self.warps]) # type: ignore
 
+        with open(path, "w") as f:
+            f.write(self.inputFile.prettify())
 
 
-    
-
```

### Comparing `tmxpy-0.1.1/src/tmxpy.egg-info/PKG-INFO` & `tmxpy-0.1.3/src/tmxpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmxpy
-Version: 0.1.1
+Version: 0.1.3
 Summary: A Python library for reading and writing TMX files.
 Author-email: AnotherPillow <redacted@email.xyz>
 Project-URL: Homepage, https://github.com/AnotherPillow/tmxpy
 Project-URL: Bug Tracker, https://github.com/AnotherPillow/tmxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

