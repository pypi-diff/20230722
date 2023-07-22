# Comparing `tmp/fanorona-aec-1.0.0.tar.gz` & `tmp/fanorona-aec-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fanorona-aec-1.0.0.tar", last modified: Thu Apr 22 20:53:03 2021, max compression
+gzip compressed data, was "fanorona-aec-2.0.0.tar", last modified: Sat Jul 22 04:00:25 2023, max compression
```

## Comparing `fanorona-aec-1.0.0.tar` & `fanorona-aec-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 akrish13  (1000) akrish13  (1000)        0 2021-04-22 20:53:03.540000 fanorona-aec-1.0.0/
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)     1937 2021-04-22 20:53:03.540000 fanorona-aec-1.0.0/PKG-INFO
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)     1081 2021-04-22 20:28:02.000000 fanorona-aec-1.0.0/README.md
-drwxr-xr-x   0 akrish13  (1000) akrish13  (1000)        0 2021-04-22 20:53:03.540000 fanorona-aec-1.0.0/fanorona_aec/
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)       26 2021-04-22 20:28:02.000000 fanorona-aec-1.0.0/fanorona_aec/__init__.py
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)     5478 2021-04-22 20:28:02.000000 fanorona-aec-1.0.0/fanorona_aec/fanorona_env.py
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)       39 2021-04-22 20:28:02.000000 fanorona-aec-1.0.0/fanorona_aec/fanorona_v0.py
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)     3779 2021-04-22 20:28:02.000000 fanorona-aec-1.0.0/fanorona_aec/move.py
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)    19406 2021-04-22 20:28:02.000000 fanorona-aec-1.0.0/fanorona_aec/state.py
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)     6293 2021-04-22 20:28:02.000000 fanorona-aec-1.0.0/fanorona_aec/utils.py
-drwxr-xr-x   0 akrish13  (1000) akrish13  (1000)        0 2021-04-22 20:53:03.540000 fanorona-aec-1.0.0/fanorona_aec.egg-info/
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)     1937 2021-04-22 20:53:03.000000 fanorona-aec-1.0.0/fanorona_aec.egg-info/PKG-INFO
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)      344 2021-04-22 20:53:03.000000 fanorona-aec-1.0.0/fanorona_aec.egg-info/SOURCES.txt
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)        1 2021-04-22 20:53:03.000000 fanorona-aec-1.0.0/fanorona_aec.egg-info/dependency_links.txt
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)       11 2021-04-22 20:53:03.000000 fanorona-aec-1.0.0/fanorona_aec.egg-info/requires.txt
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)       13 2021-04-22 20:53:03.000000 fanorona-aec-1.0.0/fanorona_aec.egg-info/top_level.txt
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)       38 2021-04-22 20:53:03.540000 fanorona-aec-1.0.0/setup.cfg
--rw-r--r--   0 akrish13  (1000) akrish13  (1000)      829 2021-04-22 20:45:38.000000 fanorona-aec-1.0.0/setup.py
+drwxr-xr-x   0 akrish13  (1000) akrish13  (1000)        0 2023-07-22 04:00:25.777449 fanorona-aec-2.0.0/
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)     1078 2023-07-22 03:54:14.000000 fanorona-aec-2.0.0/LICENSE
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)     2023 2023-07-22 04:00:25.777449 fanorona-aec-2.0.0/PKG-INFO
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)     1472 2023-07-22 03:56:40.000000 fanorona-aec-2.0.0/README.md
+drwxr-xr-x   0 akrish13  (1000) akrish13  (1000)        0 2023-07-22 04:00:25.777449 fanorona-aec-2.0.0/fanorona_aec/
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)       27 2023-07-22 03:54:14.000000 fanorona-aec-2.0.0/fanorona_aec/__init__.py
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)       44 2023-07-22 03:54:14.000000 fanorona-aec-2.0.0/fanorona_aec/fanorona_v1.py
+drwxr-xr-x   0 akrish13  (1000) akrish13  (1000)        0 2023-07-22 04:00:25.777449 fanorona-aec-2.0.0/fanorona_aec.egg-info/
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)     2023 2023-07-22 04:00:25.000000 fanorona-aec-2.0.0/fanorona_aec.egg-info/PKG-INFO
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)      344 2023-07-22 04:00:25.000000 fanorona-aec-2.0.0/fanorona_aec.egg-info/SOURCES.txt
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)        1 2023-07-22 04:00:25.000000 fanorona-aec-2.0.0/fanorona_aec.egg-info/dependency_links.txt
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)       11 2023-07-22 04:00:25.000000 fanorona-aec-2.0.0/fanorona_aec.egg-info/requires.txt
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)       13 2023-07-22 04:00:25.000000 fanorona-aec-2.0.0/fanorona_aec.egg-info/top_level.txt
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)       38 2023-07-22 04:00:25.777449 fanorona-aec-2.0.0/setup.cfg
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)      855 2023-07-22 03:54:14.000000 fanorona-aec-2.0.0/setup.py
+drwxr-xr-x   0 akrish13  (1000) akrish13  (1000)        0 2023-07-22 04:00:25.777449 fanorona-aec-2.0.0/tests/
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)     1979 2023-07-22 03:59:28.000000 fanorona-aec-2.0.0/tests/test_fanorona_env.py
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)     3435 2023-07-22 03:54:14.000000 fanorona-aec-2.0.0/tests/test_move.py
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)     4237 2023-07-22 03:54:14.000000 fanorona-aec-2.0.0/tests/test_state.py
+-rw-r--r--   0 akrish13  (1000) akrish13  (1000)     4765 2023-07-22 03:54:14.000000 fanorona-aec-2.0.0/tests/test_utils.py
```

### Comparing `fanorona-aec-1.0.0/PKG-INFO` & `fanorona-aec-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 Metadata-Version: 2.1
 Name: fanorona-aec
-Version: 1.0.0
+Version: 2.0.0
 Summary: A PettingZoo AECEnv implementation of the Fanorona board game.
 Home-page: https://github.com/AbhijeetKrishnan/fanorona-aec
 Author: Abhijeet Krishnan
 Author-email: abhijeet.krishnan@gmail.com
 License: MIT
-Description: # Fanorona AEC Environment
-        
-        [![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        This is an implementation of the Fanorona board game as a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) [AEC](https://arxiv.org/abs/2009.13051) game.
-        The rules have been sourced from [here](https://www.mindsports.nl/index.php/the-pit/528-fanorona).
-        An additional rule where games exceeding 45 moves end in a draw has been implemented, since the
-        original rules do not have explicit draw conditions.
-        
-        ## Installation
-        
-        ```bash
-        git clone https://github.com/AbhijeetKrishnan/fanorona-aec.git
-        cd fanorona-aec
-        pip install -e .
-        ```
-        
-        ## Usage
-        
-        ### Setting up a basic environment
-        
-        In a Python shell, run the following:
-        
-        ```python
-        import pettingzoo
-        import fanorona_aec
-        env = fanorona_v0.env()
-        ```
-        
-        ## Testing
-        
-        We use [pytest](http://doc.pytest.org/) for tests. You can run them via:
-        
-        ```bash
-        pytest
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Fanorona AEC Environment
+
+[![PyPI v2.0.0](https://img.shields.io/pypi/v/fanorona-aec)](https://pypi.org/project/fanorona-aec/2.0.0/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+![Fanorona board](/assets/1920px-Fanorona-1.svg.png)
+
+This is an implementation of the Fanorona board game as a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) [AEC](https://arxiv.org/abs/2009.13051) game.
+The rules have been sourced from [here](https://www.mindsports.nl/index.php/the-pit/528-fanorona).
+An additional rule where games exceeding $44$ moves end in a draw has been implemented, since the
+original rules do not have explicit draw conditions.
+
+## Installation
+
+### Using pip (recommended)
+
+```bash
+pip install fanorona-aec
+```
+
+### Local
+
+```bash
+git clone https://github.com/AbhijeetKrishnan/fanorona-aec.git
+cd fanorona-aec
+pip install -e .
+```
+
+## Usage
+
+### Setting up a basic environment
+
+In a Python shell, run the following:
+
+```python
+import fanorona_aec
+env = fanorona_v1.env()
+```
+
+See [`demo.py`](./demo.py) for a script that implements a simple random policy to interact with the environment.
+
+## Testing
+
+We use [pytest](http://doc.pytest.org/) for tests. You can run them via:
+
+```bash
+git clone https://github.com/AbhijeetKrishnan/fanorona-aec.git
+cd fanorona-aec
+pytest
+```
```

### Comparing `fanorona-aec-1.0.0/README.md` & `fanorona-aec-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 # Fanorona AEC Environment
 
-[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
+[![PyPI v2.0.0](https://img.shields.io/pypi/v/fanorona-aec)](https://pypi.org/project/fanorona-aec/2.0.0/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+![Fanorona board](/assets/1920px-Fanorona-1.svg.png)
+
 This is an implementation of the Fanorona board game as a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) [AEC](https://arxiv.org/abs/2009.13051) game.
 The rules have been sourced from [here](https://www.mindsports.nl/index.php/the-pit/528-fanorona).
-An additional rule where games exceeding 45 moves end in a draw has been implemented, since the
+An additional rule where games exceeding $44$ moves end in a draw has been implemented, since the
 original rules do not have explicit draw conditions.
 
 ## Installation
 
+### Using pip (recommended)
+
+```bash
+pip install fanorona-aec
+```
+
+### Local
+
 ```bash
 git clone https://github.com/AbhijeetKrishnan/fanorona-aec.git
 cd fanorona-aec
 pip install -e .
 ```
 
 ## Usage
 
 ### Setting up a basic environment
 
 In a Python shell, run the following:
 
 ```python
-import pettingzoo
 import fanorona_aec
-env = fanorona_v0.env()
+env = fanorona_v1.env()
 ```
 
+See [`demo.py`](./demo.py) for a script that implements a simple random policy to interact with the environment.
+
 ## Testing
 
 We use [pytest](http://doc.pytest.org/) for tests. You can run them via:
 
 ```bash
+git clone https://github.com/AbhijeetKrishnan/fanorona-aec.git
+cd fanorona-aec
 pytest
 ```
```

### Comparing `fanorona-aec-1.0.0/fanorona_aec.egg-info/PKG-INFO` & `fanorona-aec-2.0.0/fanorona_aec.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 Metadata-Version: 2.1
 Name: fanorona-aec
-Version: 1.0.0
+Version: 2.0.0
 Summary: A PettingZoo AECEnv implementation of the Fanorona board game.
 Home-page: https://github.com/AbhijeetKrishnan/fanorona-aec
 Author: Abhijeet Krishnan
 Author-email: abhijeet.krishnan@gmail.com
 License: MIT
-Description: # Fanorona AEC Environment
-        
-        [![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        This is an implementation of the Fanorona board game as a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) [AEC](https://arxiv.org/abs/2009.13051) game.
-        The rules have been sourced from [here](https://www.mindsports.nl/index.php/the-pit/528-fanorona).
-        An additional rule where games exceeding 45 moves end in a draw has been implemented, since the
-        original rules do not have explicit draw conditions.
-        
-        ## Installation
-        
-        ```bash
-        git clone https://github.com/AbhijeetKrishnan/fanorona-aec.git
-        cd fanorona-aec
-        pip install -e .
-        ```
-        
-        ## Usage
-        
-        ### Setting up a basic environment
-        
-        In a Python shell, run the following:
-        
-        ```python
-        import pettingzoo
-        import fanorona_aec
-        env = fanorona_v0.env()
-        ```
-        
-        ## Testing
-        
-        We use [pytest](http://doc.pytest.org/) for tests. You can run them via:
-        
-        ```bash
-        pytest
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Fanorona AEC Environment
+
+[![PyPI v2.0.0](https://img.shields.io/pypi/v/fanorona-aec)](https://pypi.org/project/fanorona-aec/2.0.0/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+![Fanorona board](/assets/1920px-Fanorona-1.svg.png)
+
+This is an implementation of the Fanorona board game as a [PettingZoo](https://github.com/PettingZoo-Team/PettingZoo) [AEC](https://arxiv.org/abs/2009.13051) game.
+The rules have been sourced from [here](https://www.mindsports.nl/index.php/the-pit/528-fanorona).
+An additional rule where games exceeding $44$ moves end in a draw has been implemented, since the
+original rules do not have explicit draw conditions.
+
+## Installation
+
+### Using pip (recommended)
+
+```bash
+pip install fanorona-aec
+```
+
+### Local
+
+```bash
+git clone https://github.com/AbhijeetKrishnan/fanorona-aec.git
+cd fanorona-aec
+pip install -e .
+```
+
+## Usage
+
+### Setting up a basic environment
+
+In a Python shell, run the following:
+
+```python
+import fanorona_aec
+env = fanorona_v1.env()
+```
+
+See [`demo.py`](./demo.py) for a script that implements a simple random policy to interact with the environment.
+
+## Testing
+
+We use [pytest](http://doc.pytest.org/) for tests. You can run them via:
+
+```bash
+git clone https://github.com/AbhijeetKrishnan/fanorona-aec.git
+cd fanorona-aec
+pytest
+```
```

### Comparing `fanorona-aec-1.0.0/setup.py` & `fanorona-aec-2.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setup(
-    name="fanorona-aec",
-    version="1.0.0",
-    description="A PettingZoo AECEnv implementation of the Fanorona board game.",
-    url="https://github.com/AbhijeetKrishnan/fanorona-aec",
-    author="Abhijeet Krishnan",
-    author_email="abhijeet.krishnan@gmail.com",
-    license="MIT",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    packages=["fanorona_aec"],
-    python_requires=">=3.8",
-    install_requires=["pettingzoo"],
-    tests_require=["pytest"],
-)
+from setuptools import setup
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setup(
+    name="fanorona-aec",
+    version="2.0.0",
+    description="A PettingZoo AECEnv implementation of the Fanorona board game.",
+    url="https://github.com/AbhijeetKrishnan/fanorona-aec",
+    author="Abhijeet Krishnan",
+    author_email="abhijeet.krishnan@gmail.com",
+    license="MIT",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    packages=["fanorona_aec"],
+    python_requires=">=3.8",
+    install_requires=["pettingzoo"],
+    tests_require=["pytest"],
+)
```

