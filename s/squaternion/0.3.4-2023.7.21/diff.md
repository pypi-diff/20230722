# Comparing `tmp/squaternion-0.3.4.tar.gz` & `tmp/squaternion-2023.7.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squaternion-0.3.4.tar", max compression
+gzip compressed data, was "squaternion-2023.7.21.tar", max compression
```

## Comparing `squaternion-0.3.4.tar` & `squaternion-2023.7.21.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0     1070 2019-10-27 03:15:56.229710 squaternion-0.3.4/LICENSE
--rw-r--r--   0        0        0     1115 2022-06-18 19:35:32.917362 squaternion-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     5334 2022-06-18 19:39:57.653443 squaternion-0.3.4/readme.md
--rw-r--r--   0        0        0      440 2022-06-18 19:33:44.488847 squaternion-0.3.4/squaternion/__init__.py
--rw-r--r--   0        0        0     9614 2022-06-18 20:00:27.035583 squaternion-0.3.4/squaternion/squaternion.py
--rw-r--r--   0        0        0     6045 2022-06-18 20:03:07.411319 squaternion-0.3.4/setup.py
--rw-r--r--   0        0        0     6340 2022-06-18 20:03:07.411888 squaternion-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1162 2023-07-21 22:02:50.623935 squaternion-2023.7.21/pyproject.toml
+-rw-r--r--   0        0        0     5515 2023-07-12 03:07:44.745378 squaternion-2023.7.21/readme.md
+-rw-r--r--   0        0        0      397 2022-08-17 13:35:32.119902 squaternion-2023.7.21/squaternion/__init__.py
+-rw-r--r--   0        0        0     9533 2022-08-17 13:18:36.045496 squaternion-2023.7.21/squaternion/squaternion.py
+-rw-r--r--   0        0        0     6576 1970-01-01 00:00:00.000000 squaternion-2023.7.21/PKG-INFO
```

### Comparing `squaternion-0.3.4/pyproject.toml` & `squaternion-2023.7.21/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squaternion"
-version = "0.3.4"
+version = "2023.07.21"
 description = "Some simple functions for quaternion math"
 authors = ["walchko <walchko@users.noreply.github.com>"]
 readme = "readme.md"
 license = "MIT"
 homepage = "https://pypi.org/project/squaternion/"
 repository = 'http://github.com/MomsFriendlyRobotCompany/squaternion'
 # documentation = "http://..."
@@ -13,23 +13,23 @@
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Software Development :: Libraries :: Application Frameworks'
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-# attrs = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 numpy = "*"
 
 [build-system]
-requires = ["poetry>=1.0.0"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `squaternion-0.3.4/readme.md` & `squaternion-2023.7.21/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Generally I don't need all of the capabilities (or complexity) of `quaternion`
 math libraries. Basically I just need a way to convert between Euler and
 Quaternion representations and have a nice way to print them out.
 
 This has basically no imports outside of standard python 3.x libraries.
 It should be easier to get on embedded python systems without having to build
-`numpy`. Also, this tries to be *fast* by using a frozen class.
+`numpy`. Also, this tries to be *fast* by using a `frozen` `dataclass` available in python3.
 
 ## Install
 
 ```
 pip install squaternion
 ```
 
@@ -53,14 +53,17 @@
 # euler angles from_eluer(roll, pitch, yaw), default is radians, but set
 # degrees true if giving degrees
 q = Quaternion.from_euler(0, -90, 100, degrees=True)
 
 # can get the euler angles back out in degrees (set to True)
 e = q.to_euler(degrees=True)
 d = q.to_dict()
+t = q.to_tuple()
+r = q.to_rot() # returns a rotation matrix as tuple
+r = np.array( q.to_rot() ) # rotation matrix as numpy array
 
 # iterate through values
 for i in q:
     print(f"{i}")
 
 # indexing like a namedtuple
 z = q[3]
@@ -76,20 +79,20 @@
 a = q.angle      # returns angle of rotation in radians
 a = q.axis       # returns axis of rotation
 
 # useful attr functions
 q == q    # compare will return True
 q != q    # will return False
 
-print(q)  # pretty print
 w = q.w
 x = q.x
 y = q.y
 z = q.z
 
+print(q)  # pretty print => Quaternion(w,x,y,z)
 print(f"{q:.4f}") # print only 4 decimal places
 ```
 
 ## Alternatives
 
 This is a basic library that converts between Euler angles and Quaternions.
 There are other libraries that do so much more listed below ... but I don't
@@ -104,15 +107,15 @@
 
 - [Wikipedia Convert Between Quaternions and Euler Angles](https://en.wikipedia.org/wiki/Conversion_between_quaternions_and_Euler_angles)
 - [Wikipedia Euler Angle Definitions](https://en.wikipedia.org/wiki/Euler_angles#Conventions_2)
 - [Wikipedia Gimbal Lock](https://en.wikipedia.org/wiki/Gimbal_lock)
 
 # MIT License
 
-Copyright (c) 2018 Kevin Walchko
+Copyright (c) 2014 Kevin Walchko
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `squaternion-0.3.4/squaternion/squaternion.py` & `squaternion-2023.7.21/squaternion/squaternion.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 ##############################################
 # The MIT License (MIT)
 # Copyright (c) 2014 Kevin Walchko
 # see LICENSE for full details
 ##############################################
 from math import sin, cos, atan2, pi, sqrt, asin, acos
 from dataclasses import dataclass, field
-# from enum import IntFlag
 
-# Axis = IntFlag("Axis", "x y z")
 rad2deg = 180.0/pi
 deg2rad = pi/180
 
 @dataclass(frozen=True)
 class Quaternion:
     """
     This is a Hamiltonian quaternion [real, (x,y,z)].
@@ -86,26 +84,25 @@
         # print(f">> {r.__class__ == 'squaternion.squaternion.Quaternion'}")
         q = self
 
         # print(f"q:{self}  r:{r}")
 
         if isinstance(r, (float, int)):
             w=q.w*r; x=q.x*r; y=q.y*r; z=q.z*r
-        # elif isinstance(r, Quaternion):
-        else:
+        elif isinstance(r, Quaternion):
             # print(f"q:{self}  r:{r}")
             # print(f">> {r}: {type(r)} {r.__class__}")
             # print(f"++ {type(self)}")
             # print(f"++ {type(self) == type(r)}")
             w = q.w*r.w - q.x*r.x - q.y*r.y - q.z*r.z
             x = q.x*r.w + q.w*r.x - q.z*r.y + q.y*r.z
             y = q.y*r.w + q.z*r.x + q.w*r.y - q.x*r.z
             z = q.z*r.w - q.y*r.x + q.x*r.y + q.w*r.z
-        # else:
-        #     raise Exception("Quaternion.__mult__: invalide type:", type(r))
+        else:
+            raise Exception("Quaternion.__mult__: invalide type:", type(r))
 
         return Quaternion(w,x,y,z)
 
     def __rmul__(self, r):
         """Would handle things like: 2*q"""
         # raise NotImplementedError("Quaternion.__rmul__")
         q = self
```

### Comparing `squaternion-0.3.4/setup.py` & `squaternion-2023.7.21/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,158 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: squaternion
+Version: 2023.7.21
+Summary: Some simple functions for quaternion math
+Home-page: https://pypi.org/project/squaternion/
+License: MIT
+Keywords: rotations,quaternion,euler
+Author: walchko
+Author-email: walchko@users.noreply.github.com
+Requires-Python: >=3.8
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Repository, http://github.com/MomsFriendlyRobotCompany/squaternion
+Description-Content-Type: text/markdown
 
-packages = \
-['squaternion']
+![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Inscription_on_Broom_Bridge_%28Dublin%29_regarding_the_discovery_of_Quaternions_multiplication_by_Sir_William_Rowan_Hamilton.jpg/800px-Inscription_on_Broom_Bridge_%28Dublin%29_regarding_the_discovery_of_Quaternions_multiplication_by_Sir_William_Rowan_Hamilton.jpg)
 
-package_data = \
-{'': ['*']}
+# Simple Quaternions (`squaternion`)
 
-setup_kwargs = {
-    'name': 'squaternion',
-    'version': '0.3.4',
-    'description': 'Some simple functions for quaternion math',
-    'long_description': '![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Inscription_on_Broom_Bridge_%28Dublin%29_regarding_the_discovery_of_Quaternions_multiplication_by_Sir_William_Rowan_Hamilton.jpg/800px-Inscription_on_Broom_Bridge_%28Dublin%29_regarding_the_discovery_of_Quaternions_multiplication_by_Sir_William_Rowan_Hamilton.jpg)\n\n# Simple Quaternions (`squaternion`)\n\n[![Actions Status](https://github.com/MomsFriendlyRobotCompany/squaternion/workflows/CheckPackage/badge.svg)](https://github.com/MomsFriendlyRobotCompany/squaternion/actions)\n![GitHub](https://img.shields.io/github/license/MomsFriendlyRobotCompany/squaternion)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/squaternion)\n![PyPI](https://img.shields.io/pypi/v/squaternion)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/squaternion?color=aqua)\n\nGenerally I don\'t need all of the capabilities (or complexity) of `quaternion`\nmath libraries. Basically I just need a way to convert between Euler and\nQuaternion representations and have a nice way to print them out.\n\nThis has basically no imports outside of standard python 3.x libraries.\nIt should be easier to get on embedded python systems without having to build\n`numpy`. Also, this tries to be *fast* by using a frozen class.\n\n## Install\n\n```\npip install squaternion\n```\n\n## Usage\n\n```python\nfrom squaternion import Quaternion\n\n# if you know the values you want Quaternion(w, x, y, z), note this is a\n# attr frozen class so it is immutable once created\nq = Quaternion(1,0,0,0)\n\n# multiplication for scalar (int, double) and with another quaternion\nq = Quaternion(1,2,3,4)\nq*q => Quaternion(w=-28, x=4, y=6, z=8)\n3*q => Quaternion(w=3, x=6, y=9, z=12)\nq*3.0 => Quaternion(w=3.0, x=6.0, y=9.0, z=12.0)\n\n# Addition and subtraction\nq = Quaternion(1,2,3,4)\nq+q => Quaternion(w=2, x=4, y=6, z=8)\n\n# numpy can do some things, but it will change the tuple to an array, so you might\n# need to transform it back to a quaternion\nq = Quaternion(1,2,3,4)\nnp.dot(q,q) => 30\nnp.sqrt(np.dot(q,q)) => 5.477225575051661\nq/np.sqrt(np.dot(q,q)) => array([0.18257419, 0.36514837, 0.54772256, 0.73029674])\nQuaternion(*(q/np.sqrt(np.dot(q,q)))) => Quaternion(w=0.18257418583505536, x=0.3651483716701107, y=0.5477225575051661, z=0.7302967433402214)\n\n# however you typically don\'t think in 4 dimensions, so create from\n# euler angles from_eluer(roll, pitch, yaw), default is radians, but set\n# degrees true if giving degrees\nq = Quaternion.from_euler(0, -90, 100, degrees=True)\n\n# can get the euler angles back out in degrees (set to True)\ne = q.to_euler(degrees=True)\nd = q.to_dict()\n\n# iterate through values\nfor i in q:\n    print(f"{i}")\n\n# indexing like a namedtuple\nz = q[3]\nz = q[-1]\nv = q[-3:]\nw = q[0]\n\n# class properties\nv = q.vector     # returns a tuple (x,y,z)\ns = q.scalar     # returns a double (w)\nn = q.normalize  # returns unit quaternion\nm = q.magnitude  # returns the magnitude of the quaternion\na = q.angle      # returns angle of rotation in radians\na = q.axis       # returns axis of rotation\n\n# useful attr functions\nq == q    # compare will return True\nq != q    # will return False\n\nprint(q)  # pretty print\nw = q.w\nx = q.x\ny = q.y\nz = q.z\n\nprint(f"{q:.4f}") # print only 4 decimal places\n```\n\n## Alternatives\n\nThis is a basic library that converts between Euler angles and Quaternions.\nThere are other libraries that do so much more listed below ... but I don\'t\nneed all of that.\n\n- [scipy.spatial.transform.Rotation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.transform.Rotation.html#scipy.spatial.transform.Rotation): has everything you could want, with lots of imports\n- [tinyquaternion](https://github.com/rezaahmadzadeh/tinyquaternion): appears to be more functional but needs `numpy`\n- [quaternions](https://github.com/mjsobrep/quaternions): another good lightweight quaternion package\n- [pyrr](https://github.com/adamlwgriffiths/Pyrr): seems good, integrated with `numpy`\n\n## References\n\n- [Wikipedia Convert Between Quaternions and Euler Angles](https://en.wikipedia.org/wiki/Conversion_between_quaternions_and_Euler_angles)\n- [Wikipedia Euler Angle Definitions](https://en.wikipedia.org/wiki/Euler_angles#Conventions_2)\n- [Wikipedia Gimbal Lock](https://en.wikipedia.org/wiki/Gimbal_lock)\n\n# MIT License\n\nCopyright (c) 2018 Kevin Walchko\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n',
-    'author': 'walchko',
-    'author_email': 'walchko@users.noreply.github.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://pypi.org/project/squaternion/',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8',
-}
+[![Actions Status](https://github.com/MomsFriendlyRobotCompany/squaternion/workflows/CheckPackage/badge.svg)](https://github.com/MomsFriendlyRobotCompany/squaternion/actions)
+![GitHub](https://img.shields.io/github/license/MomsFriendlyRobotCompany/squaternion)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/squaternion)
+![PyPI](https://img.shields.io/pypi/v/squaternion)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/squaternion?color=aqua)
 
+Generally I don't need all of the capabilities (or complexity) of `quaternion`
+math libraries. Basically I just need a way to convert between Euler and
+Quaternion representations and have a nice way to print them out.
+
+This has basically no imports outside of standard python 3.x libraries.
+It should be easier to get on embedded python systems without having to build
+`numpy`. Also, this tries to be *fast* by using a `frozen` `dataclass` available in python3.
+
+## Install
+
+```
+pip install squaternion
+```
+
+## Usage
+
+```python
+from squaternion import Quaternion
+
+# if you know the values you want Quaternion(w, x, y, z), note this is a
+# attr frozen class so it is immutable once created
+q = Quaternion(1,0,0,0)
+
+# multiplication for scalar (int, double) and with another quaternion
+q = Quaternion(1,2,3,4)
+q*q => Quaternion(w=-28, x=4, y=6, z=8)
+3*q => Quaternion(w=3, x=6, y=9, z=12)
+q*3.0 => Quaternion(w=3.0, x=6.0, y=9.0, z=12.0)
+
+# Addition and subtraction
+q = Quaternion(1,2,3,4)
+q+q => Quaternion(w=2, x=4, y=6, z=8)
+
+# numpy can do some things, but it will change the tuple to an array, so you might
+# need to transform it back to a quaternion
+q = Quaternion(1,2,3,4)
+np.dot(q,q) => 30
+np.sqrt(np.dot(q,q)) => 5.477225575051661
+q/np.sqrt(np.dot(q,q)) => array([0.18257419, 0.36514837, 0.54772256, 0.73029674])
+Quaternion(*(q/np.sqrt(np.dot(q,q)))) => Quaternion(w=0.18257418583505536, x=0.3651483716701107, y=0.5477225575051661, z=0.7302967433402214)
+
+# however you typically don't think in 4 dimensions, so create from
+# euler angles from_eluer(roll, pitch, yaw), default is radians, but set
+# degrees true if giving degrees
+q = Quaternion.from_euler(0, -90, 100, degrees=True)
+
+# can get the euler angles back out in degrees (set to True)
+e = q.to_euler(degrees=True)
+d = q.to_dict()
+t = q.to_tuple()
+r = q.to_rot() # returns a rotation matrix as tuple
+r = np.array( q.to_rot() ) # rotation matrix as numpy array
+
+# iterate through values
+for i in q:
+    print(f"{i}")
+
+# indexing like a namedtuple
+z = q[3]
+z = q[-1]
+v = q[-3:]
+w = q[0]
+
+# class properties
+v = q.vector     # returns a tuple (x,y,z)
+s = q.scalar     # returns a double (w)
+n = q.normalize  # returns unit quaternion
+m = q.magnitude  # returns the magnitude of the quaternion
+a = q.angle      # returns angle of rotation in radians
+a = q.axis       # returns axis of rotation
+
+# useful attr functions
+q == q    # compare will return True
+q != q    # will return False
+
+w = q.w
+x = q.x
+y = q.y
+z = q.z
+
+print(q)  # pretty print => Quaternion(w,x,y,z)
+print(f"{q:.4f}") # print only 4 decimal places
+```
+
+## Alternatives
+
+This is a basic library that converts between Euler angles and Quaternions.
+There are other libraries that do so much more listed below ... but I don't
+need all of that.
+
+- [scipy.spatial.transform.Rotation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.transform.Rotation.html#scipy.spatial.transform.Rotation): has everything you could want, with lots of imports
+- [tinyquaternion](https://github.com/rezaahmadzadeh/tinyquaternion): appears to be more functional but needs `numpy`
+- [quaternions](https://github.com/mjsobrep/quaternions): another good lightweight quaternion package
+- [pyrr](https://github.com/adamlwgriffiths/Pyrr): seems good, integrated with `numpy`
+
+## References
+
+- [Wikipedia Convert Between Quaternions and Euler Angles](https://en.wikipedia.org/wiki/Conversion_between_quaternions_and_Euler_angles)
+- [Wikipedia Euler Angle Definitions](https://en.wikipedia.org/wiki/Euler_angles#Conventions_2)
+- [Wikipedia Gimbal Lock](https://en.wikipedia.org/wiki/Gimbal_lock)
+
+# MIT License
+
+Copyright (c) 2014 Kevin Walchko
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
 
-setup(**setup_kwargs)
```

