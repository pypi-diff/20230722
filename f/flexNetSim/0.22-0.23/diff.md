# Comparing `tmp/flexNetSim-0.22.tar.gz` & `tmp/flexNetSim-0.23.tar.gz`

## Comparing `flexNetSim-0.22.tar` & `flexNetSim-0.23.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 18:53:46.000000 flexNetSim-0.22/
-drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 18:53:46.000000 flexNetSim-0.22/flexnetsim/
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     2528 2022-09-13 18:08:54.000000 flexNetSim-0.22/flexnetsim/bitrate.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     3333 2022-09-13 18:08:54.000000 flexNetSim-0.22/flexnetsim/connection.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     8732 2022-09-13 18:08:54.000000 flexNetSim-0.22/flexnetsim/controller.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     2266 2022-09-13 18:08:54.000000 flexNetSim-0.22/flexnetsim/event.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     2730 2022-09-13 18:08:54.000000 flexNetSim-0.22/flexnetsim/link.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)    20823 2022-09-13 18:08:54.000000 flexNetSim-0.22/flexnetsim/network.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      955 2022-09-13 18:08:54.000000 flexNetSim-0.22/flexnetsim/node.py
-drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 18:53:59.000000 flexNetSim-0.22/flexnetsim/random/
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      480 2022-09-16 14:36:18.000000 flexNetSim-0.22/flexnetsim/random/exp_variable.cpp
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1616 2022-09-13 18:08:54.000000 flexNetSim-0.22/flexnetsim/random/exp_variable.hpp
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      242 2022-09-21 18:24:43.000000 flexNetSim-0.22/flexnetsim/random/pyexponentialvariable.pxd
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)   164167 2022-09-21 18:53:32.000000 flexNetSim-0.22/flexnetsim/random/pyexpvariable.cpp
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      439 2022-09-21 18:25:11.000000 flexNetSim-0.22/flexnetsim/random/pyexpvariable.pyx
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      305 2022-09-20 23:31:48.000000 flexNetSim-0.22/flexnetsim/random/pyuniformvariable.pxd
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)   167446 2022-09-21 18:53:32.000000 flexNetSim-0.22/flexnetsim/random/pyunivariable.cpp
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      533 2022-09-21 17:36:55.000000 flexNetSim-0.22/flexnetsim/random/pyunivariable.pyx
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      518 2022-09-20 23:31:48.000000 flexNetSim-0.22/flexnetsim/random/uniform_variable.cpp
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1743 2022-09-20 23:31:48.000000 flexNetSim-0.22/flexnetsim/random/uniform_variable.hpp
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      148 2022-09-21 15:25:28.000000 flexNetSim-0.22/flexnetsim/random/__init__.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)    12253 2022-09-21 18:36:23.000000 flexNetSim-0.22/flexnetsim/simulator.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      354 2022-09-13 18:08:54.000000 flexNetSim-0.22/flexnetsim/__init__.py
-drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 18:53:45.000000 flexNetSim-0.22/flexNetSim.egg-info/
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        1 2022-09-21 18:53:32.000000 flexNetSim-0.22/flexNetSim.egg-info/dependency_links.txt
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        1 2022-09-21 18:42:01.000000 flexNetSim-0.22/flexNetSim.egg-info/not-zip-safe
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      345 2022-09-21 18:53:32.000000 flexNetSim-0.22/flexNetSim.egg-info/PKG-INFO
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)       13 2022-09-21 18:53:32.000000 flexNetSim-0.22/flexNetSim.egg-info/requires.txt
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      638 2022-09-21 18:53:33.000000 flexNetSim-0.22/flexNetSim.egg-info/SOURCES.txt
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)       11 2022-09-21 18:53:32.000000 flexNetSim-0.22/flexNetSim.egg-info/top_level.txt
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1103 2022-09-21 13:36:52.000000 flexNetSim-0.22/LICENSE.md
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      345 2022-09-21 18:53:35.000000 flexNetSim-0.22/PKG-INFO
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      715 2022-09-13 18:08:54.000000 flexNetSim-0.22/README.md
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      106 2022-09-21 18:53:35.000000 flexNetSim-0.22/setup.cfg
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1728 2022-09-21 18:52:12.000000 flexNetSim-0.22/setup.py
-drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 18:53:46.000000 flexNetSim-0.22/test/
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     3320 2022-09-13 18:08:54.000000 flexNetSim-0.22/test/test_bitrate.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      702 2022-09-13 18:08:54.000000 flexNetSim-0.22/test/test_connection.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     4092 2022-09-13 18:08:54.000000 flexNetSim-0.22/test/test_controller.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1866 2022-09-13 18:08:54.000000 flexNetSim-0.22/test/test_link.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)    10588 2022-09-13 18:08:54.000000 flexNetSim-0.22/test/test_network.py
--rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      884 2022-09-13 18:08:54.000000 flexNetSim-0.22/test/test_node.py
+drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 19:53:22.000000 flexNetSim-0.23/
+drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 19:53:22.000000 flexNetSim-0.23/flexnetsim/
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     2528 2022-09-13 18:08:54.000000 flexNetSim-0.23/flexnetsim/bitrate.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     3333 2022-09-13 18:08:54.000000 flexNetSim-0.23/flexnetsim/connection.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     8732 2022-09-13 18:08:54.000000 flexNetSim-0.23/flexnetsim/controller.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     2266 2022-09-13 18:08:54.000000 flexNetSim-0.23/flexnetsim/event.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     2730 2022-09-13 18:08:54.000000 flexNetSim-0.23/flexnetsim/link.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)    20823 2022-09-13 18:08:54.000000 flexNetSim-0.23/flexnetsim/network.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      955 2022-09-13 18:08:54.000000 flexNetSim-0.23/flexnetsim/node.py
+drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 19:53:30.000000 flexNetSim-0.23/flexnetsim/random/
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      480 2022-09-16 14:36:18.000000 flexNetSim-0.23/flexnetsim/random/exp_variable.cpp
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1616 2022-09-13 18:08:54.000000 flexNetSim-0.23/flexnetsim/random/exp_variable.hpp
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      242 2022-09-21 18:24:43.000000 flexNetSim-0.23/flexnetsim/random/pyexponentialvariable.pxd
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)   164167 2022-09-21 19:53:07.000000 flexNetSim-0.23/flexnetsim/random/pyexpvariable.cpp
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      439 2022-09-21 18:25:11.000000 flexNetSim-0.23/flexnetsim/random/pyexpvariable.pyx
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      305 2022-09-20 23:31:48.000000 flexNetSim-0.23/flexnetsim/random/pyuniformvariable.pxd
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)   167446 2022-09-21 19:53:07.000000 flexNetSim-0.23/flexnetsim/random/pyunivariable.cpp
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      533 2022-09-21 17:36:55.000000 flexNetSim-0.23/flexnetsim/random/pyunivariable.pyx
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      518 2022-09-20 23:31:48.000000 flexNetSim-0.23/flexnetsim/random/uniform_variable.cpp
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1743 2022-09-20 23:31:48.000000 flexNetSim-0.23/flexnetsim/random/uniform_variable.hpp
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      148 2022-09-21 15:25:28.000000 flexNetSim-0.23/flexnetsim/random/__init__.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)    12253 2022-09-21 18:36:23.000000 flexNetSim-0.23/flexnetsim/simulator.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      354 2022-09-13 18:08:54.000000 flexNetSim-0.23/flexnetsim/__init__.py
+drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 19:53:22.000000 flexNetSim-0.23/flexNetSim.egg-info/
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        1 2022-09-21 19:53:07.000000 flexNetSim-0.23/flexNetSim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        1 2022-09-21 19:49:35.000000 flexNetSim-0.23/flexNetSim.egg-info/not-zip-safe
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      345 2022-09-21 19:53:07.000000 flexNetSim-0.23/flexNetSim.egg-info/PKG-INFO
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)       13 2022-09-21 19:53:08.000000 flexNetSim-0.23/flexNetSim.egg-info/requires.txt
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      653 2022-09-21 19:53:08.000000 flexNetSim-0.23/flexNetSim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)       11 2022-09-21 19:53:08.000000 flexNetSim-0.23/flexNetSim.egg-info/top_level.txt
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1103 2022-09-21 13:36:52.000000 flexNetSim-0.23/LICENSE.md
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      345 2022-09-21 19:53:11.000000 flexNetSim-0.23/PKG-INFO
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)       60 2022-09-21 19:46:11.000000 flexNetSim-0.23/pyproject.toml
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      715 2022-09-13 18:08:54.000000 flexNetSim-0.23/README.md
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      106 2022-09-21 19:53:11.000000 flexNetSim-0.23/setup.cfg
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1728 2022-09-21 19:52:41.000000 flexNetSim-0.23/setup.py
+drwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)        0 2022-09-21 19:53:22.000000 flexNetSim-0.23/test/
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     3320 2022-09-13 18:08:54.000000 flexNetSim-0.23/test/test_bitrate.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      702 2022-09-13 18:08:54.000000 flexNetSim-0.23/test/test_connection.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     4092 2022-09-13 18:08:54.000000 flexNetSim-0.23/test/test_controller.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)     1866 2022-09-13 18:08:54.000000 flexNetSim-0.23/test/test_link.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)    10588 2022-09-13 18:08:54.000000 flexNetSim-0.23/test/test_network.py
+-rwxrwxrwx   0 gonzalo   (1000) gonzalo   (1000)      884 2022-09-13 18:08:54.000000 flexNetSim-0.23/test/test_node.py
```

### Comparing `flexNetSim-0.22/flexnetsim/bitrate.py` & `flexNetSim-0.23/flexnetsim/bitrate.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/connection.py` & `flexNetSim-0.23/flexnetsim/connection.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/controller.py` & `flexNetSim-0.23/flexnetsim/controller.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/event.py` & `flexNetSim-0.23/flexnetsim/event.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/link.py` & `flexNetSim-0.23/flexnetsim/link.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/network.py` & `flexNetSim-0.23/flexnetsim/network.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/node.py` & `flexNetSim-0.23/flexnetsim/node.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/random/exp_variable.hpp` & `flexNetSim-0.23/flexnetsim/random/exp_variable.hpp`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/random/pyexpvariable.cpp` & `flexNetSim-0.23/flexnetsim/random/pyexpvariable.cpp`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/random/pyunivariable.cpp` & `flexNetSim-0.23/flexnetsim/random/pyunivariable.cpp`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/random/pyunivariable.pyx` & `flexNetSim-0.23/flexnetsim/random/pyunivariable.pyx`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/random/uniform_variable.cpp` & `flexNetSim-0.23/flexnetsim/random/uniform_variable.cpp`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/random/uniform_variable.hpp` & `flexNetSim-0.23/flexnetsim/random/uniform_variable.hpp`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexnetsim/simulator.py` & `flexNetSim-0.23/flexnetsim/simulator.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/flexNetSim.egg-info/SOURCES.txt` & `flexNetSim-0.23/flexNetSim.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE.md
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 flexNetSim.egg-info/PKG-INFO
 flexNetSim.egg-info/SOURCES.txt
 flexNetSim.egg-info/dependency_links.txt
 flexNetSim.egg-info/not-zip-safe
 flexNetSim.egg-info/requires.txt
```

### Comparing `flexNetSim-0.22/LICENSE.md` & `flexNetSim-0.23/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/README.md` & `flexNetSim-0.23/README.md`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/setup.py` & `flexNetSim-0.23/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pathlib
 from setuptools import find_packages, setup
 from distutils.core import setup, Extension
 from Cython.Build import cythonize
 
-setup_requires = ["setuptools", "wheel", "Cython"]
+SETUP_REQUIRES = ["setuptools", "wheel", "Cython"]
 
 INSTALL_REQUIRES = [
     'numpy',
     'enum34'
 ]
 
 setup(name='flexNetSim',
-      version='0.22',
+      version='0.23',
       license='MIT',
       description='Python Package of Event-Oriented Simulation for Flexible Grid Optical Networks',
       author='Gonzalo España, Danilo Bórquez-Paredes',
       author_email='danilo.borquez.p@uai.cl',
       url='https://gitlab.com/DaniloBorquez/flex-net-sim-python/',
       packages=['flexnetsim'],
       install_requires=INSTALL_REQUIRES,
```

### Comparing `flexNetSim-0.22/test/test_bitrate.py` & `flexNetSim-0.23/test/test_bitrate.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/test/test_connection.py` & `flexNetSim-0.23/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/test/test_controller.py` & `flexNetSim-0.23/test/test_controller.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/test/test_link.py` & `flexNetSim-0.23/test/test_link.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/test/test_network.py` & `flexNetSim-0.23/test/test_network.py`

 * *Files identical despite different names*

### Comparing `flexNetSim-0.22/test/test_node.py` & `flexNetSim-0.23/test/test_node.py`

 * *Files identical despite different names*

