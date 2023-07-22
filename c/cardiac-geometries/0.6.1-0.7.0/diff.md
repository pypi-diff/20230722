# Comparing `tmp/cardiac_geometries-0.6.1.tar.gz` & `tmp/cardiac_geometries-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardiac_geometries-0.6.1.tar", last modified: Tue Jun 27 08:40:01 2023, max compression
+gzip compressed data, was "cardiac_geometries-0.7.0.tar", last modified: Sat Jul 22 20:23:46 2023, max compression
```

## Comparing `cardiac_geometries-0.6.1.tar` & `cardiac_geometries-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1547 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.162262 cardiac_geometries-0.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.166262 cardiac_geometries-0.6.1/src/cardiac_geometries/
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.166262 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/
--rw-r--r--   0 root         (0) root         (0)      602 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12783 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     9594 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_slab.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/utils.py
--rw-r--r--   0 root         (0) root         (0)      778 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_import_checks.py
--rw-r--r--   0 root         (0) root         (0)    21343 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.166262 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_biv.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_lv.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_utils.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/calculus.py
--rw-r--r--   0 root         (0) root         (0)    19764 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/cli.py
--rw-r--r--   0 root         (0) root         (0)     4615 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/dolfin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     5490 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     4187 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_slab.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_utils.py
--rw-r--r--   0 root         (0) root         (0)    16326 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/geometry.py
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/utils.py
--rw-r--r--   0 root         (0) root         (0)     9979 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/src/cardiac_geometries/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.166262 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 08:39:49.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-27 08:40:01.000000 cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 08:40:01.170262 cardiac_geometries-0.6.1/tests/
--rw-r--r--   0 root         (0) root         (0)     1970 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4569 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/tests/test_gmsh.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-06-27 08:39:48.000000 cardiac_geometries-0.6.1/tests/test_mshr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      384 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.963562 cardiac_geometries-0.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.967562 cardiac_geometries-0.7.0/src/cardiac_geometries/
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.967562 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/
+-rw-r--r--   0 root         (0) root         (0)      602 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12783 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/utils.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_import_checks.py
+-rw-r--r--   0 root         (0) root         (0)    21911 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_biv.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_lv.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/calculus.py
+-rw-r--r--   0 root         (0) root         (0)    19764 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/cli.py
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/dolfin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     4187 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16326 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9979 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.967562 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 20:23:33.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/tests/test_gmsh.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/tests/test_mshr.py
```

### Comparing `cardiac_geometries-0.6.1/LICENSE` & `cardiac_geometries-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/PKG-INFO` & `cardiac_geometries-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac_geometries
-Version: 0.6.1
+Version: 0.7.0
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.6.1/setup.cfg` & `cardiac_geometries-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardiac_geometries
-version = 0.6.1
+version = 0.7.0
 description = A python library for cardiac geometries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ComputationalPhysiology/cardiac_geometries
 author = Henrik Finsberg
 author_email = henriknf@simula.no
 license = MIT
@@ -49,15 +49,14 @@
 	ldrb
 pypi = 
 	build
 test = 
 	ldrb
 	pytest
 	pytest-cov
-	pytest-mpi
 viz = 
 	h5py
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
```

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/__init__.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/__init__.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/_gmsh/_slab.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/_import_checks.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/_import_checks.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/_mesh.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 __version__ = meta["Version"]
 
 
 def create_biv_ellipsoid(
     outdir: Union[str, Path, None] = None,
     char_length: float = 0.5,
     center_lv_y: float = 0.0,
+    center_lv_z: float = 0.0,
     a_endo_lv: float = 2.5,
     b_endo_lv: float = 1.0,
     c_endo_lv: float = 1.0,
     a_epi_lv: float = 3.0,
     b_epi_lv: float = 1.5,
     c_epi_lv: float = 1.5,
     center_rv_y: float = 0.5,
+    center_rv_z: float = 0.0,
     a_endo_rv: float = 3.0,
     b_endo_rv: float = 1.5,
     c_endo_rv: float = 1.5,
     a_epi_rv: float = 4.0,
     b_epi_rv: float = 2.5,
     c_epi_rv: float = 2.0,
     create_fibers: bool = False,
@@ -46,28 +48,32 @@
     outdir : Union[str, Path, None], optional
         Directory where to save the results. If not provided a temporary
         directory will be created, by default None, by default None
     char_length : float, optional
         Characteristic length of mesh, by default 0.5
     center_lv_y : float, optional
         Y-coordinate for the center of the lv, by default 0.0
+    center_lv_z : float, optional
+        Z-coordinate for the center of the lv, by default 0.0
     a_endo_lv : float, optional
         Dilation of lv endo ellipsoid in the x-direction, by default 2.5
     b_endo_lv : float, optional
        Dilation of lv endo ellipsoid in the y-direction, by default 1.0
     c_endo_lv : float, optional
        Dilation of lv endo ellipsoid in the z-direction, by default 1.0
     a_epi_lv : float, optional
         Dilation of lv epi ellipsoid in the x-direction, by default 3.0
     b_epi_lv : float, optional
         Dilation of lv epi ellipsoid in the y-direction, by default 1.5
     c_epi_lv : float, optional
         Dilation of lv epi ellipsoid in the z-direction, by default 1.5
     center_rv_y : float, optional
         Y-coordinate for the center of the rv, by default 0.5
+    center_rv_z : float, optional
+        Z-coordinate for the center of the rv, by default 0.0
     a_endo_rv : float, optional
        Dilation of rv endo ellipsoid in the x-direction, by default 3.0
     b_endo_rv : float, optional
        Dilation of rv endo ellipsoid in the y-direction, by default 1.5
     c_endo_rv : float, optional
        Dilation of rv endo ellipsoid in the z-direction, by default 1.5
     a_epi_rv : float, optional
@@ -109,22 +115,22 @@
     outdir = Path(outdir)
     outdir.mkdir(exist_ok=True, parents=True)
 
     with open(outdir / "info.json", "w") as f:
         json.dump(
             {
                 "char_length": char_length,
-                "center_lv": (0.0, center_lv_y, 0.0),
+                "center_lv": (0.0, center_lv_y, center_lv_z),
                 "a_endo_lv": a_endo_lv,
                 "b_endo_lv": b_endo_lv,
                 "c_endo_lv": c_endo_lv,
                 "a_epi_lv": a_epi_lv,
                 "b_epi_lv": b_epi_lv,
                 "c_epi_lv": c_epi_lv,
-                "center_rv": (0.0, center_rv_y, 0.0),
+                "center_rv": (0.0, center_rv_y, center_rv_z),
                 "a_endo_rv": a_endo_rv,
                 "b_endo_rv": b_endo_rv,
                 "c_endo_rv": c_endo_rv,
                 "a_epi_rv": a_epi_rv,
                 "b_epi_rv": b_epi_rv,
                 "c_epi_rv": c_epi_rv,
                 "create_fibers": create_fibers,
@@ -141,22 +147,22 @@
         )
 
     mesh_name = outdir / "biv_ellipsoid.msh"
 
     biv_ellipsoid(
         mesh_name=mesh_name.as_posix(),
         char_length=char_length,
-        center_lv=(0.0, center_lv_y, 0.0),
+        center_lv=(0.0, center_lv_y, center_lv_z),
         a_endo_lv=a_endo_lv,
         b_endo_lv=b_endo_lv,
         c_endo_lv=c_endo_lv,
         a_epi_lv=a_epi_lv,
         b_epi_lv=b_epi_lv,
         c_epi_lv=c_epi_lv,
-        center_rv=(0.0, center_rv_y, 0.0),
+        center_rv=(0.0, center_rv_y, center_rv_z),
         a_endo_rv=a_endo_rv,
         b_endo_rv=b_endo_rv,
         c_endo_rv=c_endo_rv,
         a_epi_rv=a_epi_rv,
         b_epi_rv=b_epi_rv,
         c_epi_rv=c_epi_rv,
     )
@@ -197,21 +203,23 @@
     char_length: float = 0.5,
     heart_as_surface: bool = True,
     torso_length: float = 20.0,
     torso_width: float = 20.0,
     torso_height: float = 20.0,
     rotation_angle: float = math.pi / 6,
     center_lv_y: float = 0.0,
+    center_lv_z: float = 0.0,
     a_endo_lv: float = 2.5,
     b_endo_lv: float = 1.0,
     c_endo_lv: float = 1.0,
     a_epi_lv: float = 3.0,
     b_epi_lv: float = 1.5,
     c_epi_lv: float = 1.5,
     center_rv_y: float = 0.5,
+    center_rv_z: float = 0.0,
     a_endo_rv: float = 3.0,
     b_endo_rv: float = 1.5,
     c_endo_rv: float = 1.5,
     a_epi_rv: float = 4.0,
     b_epi_rv: float = 2.5,
     c_epi_rv: float = 2.0,
     create_fibers: bool = False,
@@ -238,28 +246,32 @@
     torso_height : float, optional
         Length of torso in the z-direction, by default 20.0
     rotation_angle: float, optional
         Angle to rotate the torso in order to object realistic position of
         the heart in a torso, by default pi / 6
     center_lv_y : float, optional
         Y-coordinate for the center of the lv, by default 0.0
+    center_lv_z : float, optional
+        Z-coordinate for the center of the lv, by default 0.0
     a_endo_lv : float, optional
         Dilation of lv endo ellipsoid in the x-direction, by default 2.5
     b_endo_lv : float, optional
        Dilation of lv endo ellipsoid in the y-direction, by default 1.0
     c_endo_lv : float, optional
        Dilation of lv endo ellipsoid in the z-direction, by default 1.0
     a_epi_lv : float, optional
         Dilation of lv epi ellipsoid in the x-direction, by default 3.0
     b_epi_lv : float, optional
         Dilation of lv epi ellipsoid in the y-direction, by default 1.5
     c_epi_lv : float, optional
         Dilation of lv epi ellipsoid in the z-direction, by default 1.5
     center_rv_y : float, optional
         Y-coordinate for the center of the rv, by default 0.5
+    center_rv_z : float, optional
+        Z-coordinate for the center of the rv, by default 0.0
     a_endo_rv : float, optional
        Dilation of rv endo ellipsoid in the x-direction, by default 3.0
     b_endo_rv : float, optional
        Dilation of rv endo ellipsoid in the y-direction, by default 1.5
     c_endo_rv : float, optional
        Dilation of rv endo ellipsoid in the z-direction, by default 1.5
     a_epi_rv : float, optional
@@ -306,22 +318,22 @@
             {
                 "char_length": char_length,
                 "heart_as_surface": heart_as_surface,
                 "torso_length": torso_length,
                 "torso_width": torso_width,
                 "torso_height": torso_height,
                 "rotation_angle": rotation_angle,
-                "center_lv": (0.0, center_lv_y, 0.0),
+                "center_lv": (0.0, center_lv_y, center_lv_z),
                 "a_endo_lv": a_endo_lv,
                 "b_endo_lv": b_endo_lv,
                 "c_endo_lv": c_endo_lv,
                 "a_epi_lv": a_epi_lv,
                 "b_epi_lv": b_epi_lv,
                 "c_epi_lv": c_epi_lv,
-                "center_rv": (0.0, center_rv_y, 0.0),
+                "center_rv": (0.0, center_rv_y, center_rv_z),
                 "a_endo_rv": a_endo_rv,
                 "b_endo_rv": b_endo_rv,
                 "c_endo_rv": c_endo_rv,
                 "a_epi_rv": a_epi_rv,
                 "b_epi_rv": b_epi_rv,
                 "c_epi_rv": c_epi_rv,
                 "create_fibers": create_fibers,
@@ -343,22 +355,22 @@
         mesh_name=mesh_name.as_posix(),
         char_length=char_length,
         heart_as_surface=heart_as_surface,
         torso_length=torso_length,
         torso_height=torso_height,
         torso_width=torso_width,
         rotation_angle=rotation_angle,
-        center_lv=(0.0, center_lv_y, 0.0),
+        center_lv=(0.0, center_lv_y, center_lv_z),
         a_endo_lv=a_endo_lv,
         b_endo_lv=b_endo_lv,
         c_endo_lv=c_endo_lv,
         a_epi_lv=a_epi_lv,
         b_epi_lv=b_epi_lv,
         c_epi_lv=c_epi_lv,
-        center_rv=(0.0, center_rv_y, 0.0),
+        center_rv=(0.0, center_rv_y, center_rv_z),
         a_endo_rv=a_endo_rv,
         b_endo_rv=b_endo_rv,
         c_endo_rv=c_endo_rv,
         a_epi_rv=a_epi_rv,
         b_epi_rv=b_epi_rv,
         c_epi_rv=c_epi_rv,
     )
```

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_biv.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_biv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/_mshr/_lv.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_lv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/calculus.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/calculus.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/cli.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/cli.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/dolfin_utils.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/dolfin_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_slab.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/fibers/_utils.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/geometry.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/geometry.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries/viz.py` & `cardiac_geometries-0.7.0/src/cardiac_geometries/viz.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/PKG-INFO` & `cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac-geometries
-Version: 0.6.1
+Version: 0.7.0
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.6.1/src/cardiac_geometries.egg-info/SOURCES.txt` & `cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/tests/test_cli.py` & `cardiac_geometries-0.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.6.1/tests/test_geometry.py` & `cardiac_geometries-0.7.0/tests/test_geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,46 +47,46 @@
         info2=info2,
         mesh2=mesh2,
         ffun2=ffun2,
         f02=f02,
     )
 
 
-def test_load_invalid_schema(mpi_tmp_path):
+def test_load_invalid_schema(tmp_path):
     schema = {
         "mesh": dict(h5group="/mesh", is_mesh=True, invalid_key=42),
         "ffun": dict(h5group="/ffun", is_meshfunction=True, dim=2),
         "f0": dict(h5group="/f0", is_function=True),
     }
-    path = mpi_tmp_path / "schema.json"
+    path = tmp_path / "schema.json"
     path.write_text(json.dumps(schema, indent=2))
     new_schema = load_schema(path)
     for name, d in schema.items():
         for k, v in d.items():
             if k == "invalid_key":
                 continue
             assert getattr(new_schema[name], k) == v
 
 
-def test_save_load_simple(mpi_tmp_path, example_data):
+def test_save_load_simple(tmp_path, example_data):
     # import logging
 
     # logging.basicConfig(
     #     level=logging.DEBUG,
     #     format="%(process)d - %(levelname)s - %(filename)s: %(lineno)d - %(message)s",
     # )
     schema = {
         "info": H5Path(h5group="/info", is_dolfin=False),
         "mesh": H5Path(h5group="/mesh", is_mesh=True),
         "ffun": H5Path(h5group="/ffun", is_meshfunction=True, dim=2, mesh_key="mesh"),
         "f0": H5Path(h5group="/f0", is_function=True, mesh_key="mesh"),
     }
     geo = Geometry(**example_data._asdict(), schema=schema)
 
-    path = mpi_tmp_path / "geo.h5"
+    path = tmp_path / "geo.h5"
     schema_path = path.with_suffix(".json")
     geo.save(path, schema_path=schema_path)
 
     assert path.is_file()
 
     new_geo = Geometry.from_file(path, schema_path=schema_path)
     assert new_geo.schema == geo.schema
```

### Comparing `cardiac_geometries-0.6.1/tests/test_gmsh.py` & `cardiac_geometries-0.7.0/tests/test_gmsh.py`

 * *Files identical despite different names*

