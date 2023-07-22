# Comparing `tmp/Final2x-core-1.0.3.tar.gz` & `tmp/Final2x-core-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Final2x-core-1.0.3.tar", last modified: Mon Jul 17 02:23:42 2023, max compression
+gzip compressed data, was "Final2x-core-1.0.4.tar", last modified: Sat Jul 22 07:28:42 2023, max compression
```

## Comparing `Final2x-core-1.0.3.tar` & `Final2x-core-1.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.574713 Final2x-core-1.0.3/Final2x_core/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-17 02:23:21.000000 Final2x-core-1.0.3/Final2x_core/Final2x-core-pip.md
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.574713 Final2x-core-1.0.3/Final2x_core/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/Final2x_core/src/SRFactory/
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/REALCUGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/REALESRGAN.py
--rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRBaseClass.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRFactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRMD.py
--rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/WAIFU2X.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRFactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/Final2x_core/src/SRncnn/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRncnn/REALCUGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRncnn/REALESRGANncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRncnn/SRMDncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/SRqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/Final2x_core/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/utils/getConfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/utils/progressLog.py
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core/src/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 02:23:42.574713 Final2x-core-1.0.3/Final2x_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8293 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-17 02:23:42.000000 Final2x-core-1.0.3/Final2x_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-17 02:23:21.000000 Final2x-core-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-17 02:23:21.000000 Final2x-core-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8293 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7587 2023-07-17 02:23:21.000000 Final2x-core-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 02:23:42.578713 Final2x-core-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-17 02:23:23.000000 Final2x-core-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 07:28:42.480753 Final2x-core-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 07:28:42.476753 Final2x-core-1.0.4/Final2x_core/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-22 07:28:16.000000 Final2x-core-1.0.4/Final2x_core/Final2x-core-pip.md
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 07:28:42.476753 Final2x-core-1.0.4/Final2x_core/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 07:28:42.476753 Final2x-core-1.0.4/Final2x_core/src/SRFactory/
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRFactory/REALCUGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRFactory/REALESRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRFactory/SRBaseClass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRFactory/SRFactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRFactory/SRMD.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRFactory/WAIFU2X.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRFactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 07:28:42.480753 Final2x-core-1.0.4/Final2x_core/src/SRncnn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRncnn/REALCUGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRncnn/REALESRGANncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRncnn/SRMDncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRncnn/WAIFU2Xncnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/SRqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 07:28:42.480753 Final2x-core-1.0.4/Final2x_core/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     5535 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/utils/getConfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/utils/progressLog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-07-22 07:28:41.000000 Final2x-core-1.0.4/Final2x_core/src/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 07:28:42.476753 Final2x-core-1.0.4/Final2x_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8257 2023-07-22 07:28:42.000000 Final2x-core-1.0.4/Final2x_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-22 07:28:42.000000 Final2x-core-1.0.4/Final2x_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 07:28:42.000000 Final2x-core-1.0.4/Final2x_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-22 07:28:42.000000 Final2x-core-1.0.4/Final2x_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-22 07:28:42.000000 Final2x-core-1.0.4/Final2x_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-22 07:28:42.000000 Final2x-core-1.0.4/Final2x_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-22 07:28:16.000000 Final2x-core-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-22 07:28:16.000000 Final2x-core-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8257 2023-07-22 07:28:42.480753 Final2x-core-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7551 2023-07-22 07:28:16.000000 Final2x-core-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-22 07:28:42.480753 Final2x-core-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-22 07:28:17.000000 Final2x-core-1.0.4/setup.py
```

### Comparing `Final2x-core-1.0.3/Final2x_core/__main__.py` & `Final2x-core-1.0.4/Final2x_core/__main__.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/config.yaml` & `Final2x-core-1.0.4/Final2x_core/config.yaml`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRFactory/REALCUGAN.py` & `Final2x-core-1.0.4/Final2x_core/src/SRFactory/REALCUGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRFactory/REALESRGAN.py` & `Final2x-core-1.0.4/Final2x_core/src/SRFactory/REALESRGAN.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRBaseClass.py` & `Final2x-core-1.0.4/Final2x_core/src/SRFactory/SRBaseClass.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRFactory.py` & `Final2x-core-1.0.4/Final2x_core/src/SRFactory/SRFactory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from loguru import logger
 
 
 class SRFactory:
     @staticmethod
     @logger.catch(reraise=True)
     def getSR():
-
+        """
+        get a SR model instance according to config
+        :return:
+        """
         try:
             from src.utils.getConfig import SRCONFIG
         except ImportError:
             # for pip cli
             from Final2x_core.src.utils.getConfig import SRCONFIG
 
         config = SRCONFIG()
```

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRFactory/SRMD.py` & `Final2x-core-1.0.4/Final2x_core/src/SRFactory/SRMD.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRFactory/WAIFU2X.py` & `Final2x-core-1.0.4/Final2x_core/src/SRFactory/WAIFU2X.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRFactory/__init__.py` & `Final2x-core-1.0.4/Final2x_core/src/SRFactory/__init__.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRncnn/REALCUGANncnn.py` & `Final2x-core-1.0.4/Final2x_core/src/SRncnn/REALCUGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRncnn/REALESRGANncnn.py` & `Final2x-core-1.0.4/Final2x_core/src/SRncnn/REALESRGANncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRncnn/SRMDncnn.py` & `Final2x-core-1.0.4/Final2x_core/src/SRncnn/SRMDncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRncnn/WAIFU2Xncnn.py` & `Final2x-core-1.0.4/Final2x_core/src/SRncnn/WAIFU2Xncnn.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core/src/SRqueue.py` & `Final2x-core-1.0.4/Final2x_core/src/SRqueue.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     # for pip cli
     from Final2x_core.src.SRFactory import SRFactory
     from Final2x_core.src.utils.getConfig import SRCONFIG
     from Final2x_core.src.utils.progressLog import PrintProgressLog
 
 
 def SR_queue():
+    """
+    Super-resolution queue. Process all RGBA images according to the config.
+    :return:
+    """
     config = SRCONFIG()
     input_path: list = config.inputpath
     output_path: Path = Path(config.outputpath) / "outputs"
     output_path.mkdir(parents=True, exist_ok=True)  # create output folder
     sr = SRFactory.getSR()
 
     logger.info("Processing------[ 0.0% ]")
```

### Comparing `Final2x-core-1.0.3/Final2x_core/src/utils/getConfig.py` & `Final2x-core-1.0.4/Final2x_core/src/utils/getConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,37 +24,43 @@
         self._model: str = "RealCUGAN-pro"
         self._modelscale: int = 2
         self._modelnoise: int = 0
         self._inputpath: list = []
 
     @logger.catch(reraise=True)
     def getConfigfromYaml(self, configpath: str = "", modelpath: str = "") -> None:
+        """
+        get config from yaml file
+        :param configpath: absolute path to config file
+        :param modelpath: absolute path to model folder
+        :return:
+        """
         self._modelpath: str = modelpath
         with open(configpath, 'r', encoding="utf-8") as f:
             config = yaml.safe_load(f)
         self._setConfig(config)
 
     @logger.catch(reraise=True)
     def getConfigfromJson(self, config: str = "", modelpath: str = "") -> None:
         """
         get config from json string
         :param config: a json string
-        :param modelpath: path to model folder
+        :param modelpath: absolute path to model folder
         :return:
         """
         self._modelpath = modelpath
         config = json.loads(config)
         self._setConfig(config)
 
     @logger.catch(reraise=True)
     def getConfigfromBase64toJson(self, config: str = "", modelpath: str = "") -> None:
         """
         get config from base64 string
         :param config: a base64 string
-        :param modelpath: path to model folder
+        :param modelpath: absolute path to model folder
         :return:
         """
         self._modelpath = modelpath
 
         config = config.encode('utf-8')
         config = base64.b64decode(config).decode("utf-8")
         config = json.loads(config)
```

### Comparing `Final2x-core-1.0.3/Final2x_core/src/utils/progressLog.py` & `Final2x-core-1.0.4/Final2x_core/src/utils/progressLog.py`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/Final2x_core.egg-info/PKG-INFO` & `Final2x-core-1.0.4/Final2x_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Final2x-core
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/Tohrusky/Final2x-core
 Author: Tohrusky
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,19 +15,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<a href="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light">
+<a href="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo-dark.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Dark" />
-    <source media="(prefers-color-scheme: light)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
-    <img alt="Socialify Image" src="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
+    <source media="(prefers-color-scheme: dark)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo-dark.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Dark" />
+    <source media="(prefers-color-scheme: light)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
+    <img alt="Socialify Image" src="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
   </picture>
 </a>
 
 
 ![MacOS x64](https://img.shields.io/badge/Support-MacOS%20x64-blue?logo=Apple&style=flat-square)
 ![MacOS arm64](https://img.shields.io/badge/Support-MacOS%20arm64-blue?logo=Apple&style=flat-square)
 ![Windows x64](https://img.shields.io/badge/Support-Windows%20x64-blue?logo=Windows&style=flat-square)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Final2x-core Version: 1.0.3 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: Final2x-core Version: 1.0.4 Summary: UNKNOWN Home-
 page: https://github.com/Tohrusky/Final2x-core Author: Tohrusky License:
 UNKNOWN Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `Final2x-core-1.0.3/Final2x_core.egg-info/SOURCES.txt` & `Final2x-core-1.0.4/Final2x_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/LICENSE` & `Final2x-core-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Final2x-core-1.0.3/PKG-INFO` & `Final2x-core-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Final2x-core
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/Tohrusky/Final2x-core
 Author: Tohrusky
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,19 +15,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<a href="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light">
+<a href="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo-dark.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Dark" />
-    <source media="(prefers-color-scheme: light)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
-    <img alt="Socialify Image" src="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
+    <source media="(prefers-color-scheme: dark)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo-dark.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Dark" />
+    <source media="(prefers-color-scheme: light)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
+    <img alt="Socialify Image" src="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
   </picture>
 </a>
 
 
 ![MacOS x64](https://img.shields.io/badge/Support-MacOS%20x64-blue?logo=Apple&style=flat-square)
 ![MacOS arm64](https://img.shields.io/badge/Support-MacOS%20arm64-blue?logo=Apple&style=flat-square)
 ![Windows x64](https://img.shields.io/badge/Support-Windows%20x64-blue?logo=Windows&style=flat-square)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Final2x-core Version: 1.0.3 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: Final2x-core Version: 1.0.4 Summary: UNKNOWN Home-
 page: https://github.com/Tohrusky/Final2x-core Author: Tohrusky License:
 UNKNOWN Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `Final2x-core-1.0.3/README.md` & `Final2x-core-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-<a href="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light">
+<a href="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo-dark.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Dark" />
-    <source media="(prefers-color-scheme: light)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
-    <img alt="Socialify Image" src="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
+    <source media="(prefers-color-scheme: dark)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo-dark.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Dark" />
+    <source media="(prefers-color-scheme: light)" srcset="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
+    <img alt="Socialify Image" src="https://socialify.git.ci/Tohrusky/Final2x-core/image?description=1&forks=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FTohrusky%2FTohrusky%2Fmain%2Ficon%2Flogo.png&name=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light" />
   </picture>
 </a>
 
 
 ![MacOS x64](https://img.shields.io/badge/Support-MacOS%20x64-blue?logo=Apple&style=flat-square)
 ![MacOS arm64](https://img.shields.io/badge/Support-MacOS%20arm64-blue?logo=Apple&style=flat-square)
 ![Windows x64](https://img.shields.io/badge/Support-Windows%20x64-blue?logo=Windows&style=flat-square)
```

### Comparing `Final2x-core-1.0.3/setup.py` & `Final2x-core-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-_version: str = "1.0.3"
+_version: str = "1.0.4"
 
 
 def My_find_packages(*tops):
     packages = []
     for d in tops:
         for root, dirs, files in os.walk(d, followlinks=True):
             packages.append(root)
```

