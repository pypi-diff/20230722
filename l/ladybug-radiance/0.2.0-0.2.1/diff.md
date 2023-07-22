# Comparing `tmp/ladybug-radiance-0.2.0.tar.gz` & `tmp/ladybug-radiance-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-radiance-0.2.0.tar", last modified: Wed Feb  1 00:33:00 2023, max compression
+gzip compressed data, was "dist/ladybug-radiance-0.2.1.tar", last modified: Sat Jul 22 02:31:25 2023, max compression
```

## Comparing `ladybug-radiance-0.2.0.tar` & `ladybug-radiance-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/ladybug_radiance/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/skymatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/ladybug_radiance/study/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/study/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/study/directsun.py
--rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/study/radiation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/ladybug_radiance/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/visualize/raddome.py
--rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/visualize/radrose.py
--rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/ladybug_radiance/visualize/skydome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/ladybug_radiance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/ladybug_radiance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/ladybug_radiance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/ladybug_radiance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/ladybug_radiance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/ladybug_radiance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-01 00:33:00.000000 ladybug-radiance-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-01 00:31:53.000000 ladybug-radiance-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/display-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/ladybug_radiance/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/skymatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/ladybug_radiance/study/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/study/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/study/directsun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/study/radiation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/ladybug_radiance/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/visualize/raddome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/visualize/radrose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/ladybug_radiance/visualize/skydome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/ladybug_radiance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/ladybug_radiance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/ladybug_radiance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/ladybug_radiance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/ladybug_radiance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/ladybug_radiance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 02:31:25.000000 ladybug-radiance-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-22 02:30:22.000000 ladybug-radiance-0.2.1/setup.py
```

### Comparing `ladybug-radiance-0.2.0/LICENSE` & `ladybug-radiance-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.0/PKG-INFO` & `ladybug-radiance-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ladybug-radiance
-Version: 0.2.0
+Version: 0.2.1
 Summary: Radiance extension for Ladybug, used for all radiation studies and graphics.
 Home-page: https://github.com/ladybug-tools/ladybug-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: display
 License-File: LICENSE
 
 
 ![Ladybug](http://www.ladybug.tools/assets/img/ladybug.png)
 
 [![Build Status](https://github.com/ladybug-tools/ladybug-radiance/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-radiance/actions)
```

### Comparing `ladybug-radiance-0.2.0/README.md` & `ladybug-radiance-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.0/dev-requirements.txt` & `ladybug-radiance-0.2.1/dev-requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 coverage==5.5
 coveralls==1.7.0;python_version<'3.0'
 coveralls==2.2.0;python_version>='3.6'
 pytest==4.6.9;python_version<'3.0'
 pytest==6.2.4;python_version>='3.6'
 pytest-cov==2.12.0
 Sphinx==1.8.5;python_version<'3.0'
-Sphinx==3.3.1;python_version>='3.6'
+Sphinx==5.3.0;python_version>='3.6'
 docutils==0.17;python_version>='3.6'
 sphinx-bootstrap-theme==0.8.1
 sphinxcontrib-fulltoc==1.2.0
 sphinxcontrib-websupport==1.1.2;python_version<'3.0'
 sphinxcontrib-websupport==1.2.4;python_version>='3.6'
-sphinx-click==2.7.1
+sphinx-click==4.4.0
 twine==1.13.0;python_version<'3.0'
 twine==3.4.1;python_version>='3.6'
 wheel==0.38.1
 setuptools==44.1.0;python_version<'3.0'
 setuptools==65.5.1;python_version>='3.6'
 importlib-metadata==2.0.0;python_version<'3.0'
-importlib-metadata==4.0.1;python_version>='3.6'
-jinja2==3.0.3;python_version>='3.6'
-markupsafe==2.0.1;python_version>='3.6'
+importlib-metadata==4.8.0;python_version>='3.6'
 jinja2==3.0.3;python_version>='3.6'
 markupsafe==2.0.1;python_version>='3.6'
```

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance/config.py` & `ladybug-radiance-0.2.1/ladybug_radiance/config.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance/intersection.py` & `ladybug-radiance-0.2.1/ladybug_radiance/intersection.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance/skymatrix.py` & `ladybug-radiance-0.2.1/ladybug_radiance/skymatrix.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance/study/directsun.py` & `ladybug-radiance-0.2.1/ladybug_radiance/study/directsun.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                  offset_distance=0, by_vertex=False, sim_folder=None):
         """Initialize RadiationDome."""
         # set default values, which will be overwritten when the study is run
         self._offset_distance = float(offset_distance)
         self._by_vertex = bool(by_vertex)
         # set the key properties of the object
         self.vectors = vectors
-        self.timestep = 1
+        self.timestep = timestep
         self.study_mesh = study_mesh
         self.context_geometry = context_geometry
         self.sim_folder = sim_folder
         # set default values, which will be overwritten when the study is run
         self._intersection_matrix = None
         self._direct_sun_hours = None
 
@@ -213,15 +213,15 @@
             sum(int_list) / t_step for int_list in self._intersection_matrix]
 
     def draw(self, legend_parameters=None):
         """Draw a colored study_mesh, compass, graphic/legend, and title.
 
         Args:
             legend_parameters: An optional LegendParameter object to change the display
-                of the radiation dome. If None, default legend parameters will be
+                of the direct sun study. If None, default legend parameters will be
                 used. (Default: None).
 
         Returns:
             colored_mesh: A colored Mesh3D for the study results.
             graphic: A GraphicContainer for the colored mesh, indicating the
                 legend and title location for the study.
             title: Text for the title of the study.
```

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance/study/radiation.py` & `ladybug-radiance-0.2.1/ladybug_radiance/study/radiation.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     __slots__ = (
         '_metadata', '_is_benefit', '_sky_matrix', '_study_mesh', '_context_geometry',
         '_offset_distance', '_by_vertex', '_study_points', '_study_normals',
         '_sim_folder', '_intersection_matrix', '_radiation_values')
 
     def __init__(self, sky_matrix, study_mesh, context_geometry,
                  offset_distance=0, by_vertex=False, sim_folder=None):
-        """Initialize RadiationDome."""
+        """Initialize RadiationStudy."""
         # set default values, which will be overwritten when the study is run
         self._offset_distance = float(offset_distance)
         self._by_vertex = bool(by_vertex)
         # set the key properties of the object
         self.sky_matrix = sky_matrix
         self.study_mesh = study_mesh
         self.context_geometry = context_geometry
@@ -247,15 +247,15 @@
         ]
 
     def draw(self, legend_parameters=None, plot_irradiance=False):
         """Draw a colored study_mesh, compass, graphic/legend, and title.
 
         Args:
             legend_parameters: An optional LegendParameter object to change the display
-                of the radiation dome. If None, default legend parameters will be
+                of the radiation study. If None, default legend parameters will be
                 used. (Default: None).
             plot_irradiance: Boolean to note whether the results should be plotted
                 with units of total Radiation (kWh/m2) [False] or with units of average
                 Irradiance (W/m2) [True]. (Default: False).
 
         Returns:
             colored_mesh: A colored Mesh3D for the study results.
```

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance/visualize/raddome.py` & `ladybug-radiance-0.2.1/ladybug_radiance/visualize/raddome.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance/visualize/radrose.py` & `ladybug-radiance-0.2.1/ladybug_radiance/visualize/radrose.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance/visualize/skydome.py` & `ladybug-radiance-0.2.1/ladybug_radiance/visualize/skydome.py`

 * *Files identical despite different names*

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance.egg-info/PKG-INFO` & `ladybug-radiance-0.2.1/ladybug_radiance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ladybug-radiance
-Version: 0.2.0
+Version: 0.2.1
 Summary: Radiance extension for Ladybug, used for all radiation studies and graphics.
 Home-page: https://github.com/ladybug-tools/ladybug-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: display
 License-File: LICENSE
 
 
 ![Ladybug](http://www.ladybug.tools/assets/img/ladybug.png)
 
 [![Build Status](https://github.com/ladybug-tools/ladybug-radiance/workflows/CI/badge.svg)](https://github.com/ladybug-tools/ladybug-radiance/actions)
```

### Comparing `ladybug-radiance-0.2.0/ladybug_radiance.egg-info/SOURCES.txt` & `ladybug-radiance-0.2.1/ladybug_radiance.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 dev-requirements.txt
+display-requirements.txt
 requirements.txt
 setup.cfg
 setup.py
 ladybug_radiance/__init__.py
 ladybug_radiance/config.json
 ladybug_radiance/config.py
 ladybug_radiance/intersection.py
```

### Comparing `ladybug-radiance-0.2.0/setup.py` & `ladybug-radiance-0.2.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
+with open('display-requirements.txt') as f:
+    display_requirements = f.read().splitlines()
+
 setuptools.setup(
     name="ladybug-radiance",
     use_scm_version=True,
     setup_requires=['setuptools_scm'],
     author="Ladybug Tools",
     author_email="info@ladybug.tools",
     description='Radiance extension for Ladybug, used for all radiation studies '
     'and graphics.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ladybug-tools/ladybug-radiance",
     packages=setuptools.find_packages(exclude=['tests']),
     include_package_data=True,
     install_requires=requirements,
+    extras_require={
+        'display': display_requirements
+    },
     classifiers=[
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: Implementation :: CPython",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent"
     ],
```

