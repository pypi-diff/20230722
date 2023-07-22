# Comparing `tmp/deepcellpredictor-0.9.5.tar.gz` & `tmp/deepcellpredictor-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepcellpredictor-0.9.5.tar", last modified: Sat Jul 22 21:27:23 2023, max compression
+gzip compressed data, was "deepcellpredictor-0.9.6.tar", last modified: Sat Jul 22 21:38:45 2023, max compression
```

## Comparing `deepcellpredictor-0.9.5.tar` & `deepcellpredictor-0.9.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-22 21:27:23.818172 deepcellpredictor-0.9.5/
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-22 21:27:23.818172 deepcellpredictor-0.9.5/DCP/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.5/DCP/ModelPlanner.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8298 2023-07-20 22:39:47.000000 deepcellpredictor-0.9.5/DCP/VAEtorch.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.5/DCP/__init__.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11700 2023-07-22 21:21:48.000000 deepcellpredictor-0.9.5/DCP/deep_predictor.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.5/DCP/flow.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.5/DCP/utils.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.5/LICENSE
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-22 21:27:23.818172 deepcellpredictor-0.9.5/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      465 2023-07-21 12:53:17.000000 deepcellpredictor-0.9.5/README.md
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-22 21:27:23.818172 deepcellpredictor-0.9.5/deepcellpredictor.egg-info/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-22 21:27:23.000000 deepcellpredictor-0.9.5/deepcellpredictor.egg-info/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-22 21:27:23.000000 deepcellpredictor-0.9.5/deepcellpredictor.egg-info/SOURCES.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-22 21:27:23.000000 deepcellpredictor-0.9.5/deepcellpredictor.egg-info/dependency_links.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       90 2023-07-22 21:27:23.000000 deepcellpredictor-0.9.5/deepcellpredictor.egg-info/requires.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-22 21:27:23.000000 deepcellpredictor-0.9.5/deepcellpredictor.egg-info/top_level.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-22 21:27:23.818172 deepcellpredictor-0.9.5/setup.cfg
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      798 2023-07-22 21:27:18.000000 deepcellpredictor-0.9.5/setup.py
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-22 21:38:45.261356 deepcellpredictor-0.9.6/
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-22 21:38:45.257357 deepcellpredictor-0.9.6/DCP/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.6/DCP/ModelPlanner.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8298 2023-07-20 22:39:47.000000 deepcellpredictor-0.9.6/DCP/VAEtorch.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.6/DCP/__init__.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11680 2023-07-22 21:37:20.000000 deepcellpredictor-0.9.6/DCP/deep_predictor.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.6/DCP/flow.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.9.6/DCP/utils.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.9.6/LICENSE
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-22 21:38:45.261356 deepcellpredictor-0.9.6/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      465 2023-07-21 12:53:17.000000 deepcellpredictor-0.9.6/README.md
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-22 21:38:45.261356 deepcellpredictor-0.9.6/deepcellpredictor.egg-info/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      444 2023-07-22 21:38:44.000000 deepcellpredictor-0.9.6/deepcellpredictor.egg-info/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-22 21:38:45.000000 deepcellpredictor-0.9.6/deepcellpredictor.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-22 21:38:44.000000 deepcellpredictor-0.9.6/deepcellpredictor.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       90 2023-07-22 21:38:45.000000 deepcellpredictor-0.9.6/deepcellpredictor.egg-info/requires.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-22 21:38:45.000000 deepcellpredictor-0.9.6/deepcellpredictor.egg-info/top_level.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-22 21:38:45.261356 deepcellpredictor-0.9.6/setup.cfg
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      798 2023-07-22 21:37:38.000000 deepcellpredictor-0.9.6/setup.py
```

### Comparing `deepcellpredictor-0.9.5/DCP/ModelPlanner.py` & `deepcellpredictor-0.9.6/DCP/ModelPlanner.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.5/DCP/VAEtorch.py` & `deepcellpredictor-0.9.6/DCP/VAEtorch.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.5/DCP/deep_predictor.py` & `deepcellpredictor-0.9.6/DCP/deep_predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from .flow import PlanarFlow
 from .flow import Flow
 import pytorch_lightning
 from pytorch_lightning import LightningDataModule, LightningModule
 from anndata import AnnData
 from pytorch_lightning import Trainer
 from typing import List
-from flow import * 
 import scanpy as sc 
 from scipy import sparse
 import scipy.stats as ss
 
 class DeepPredictor():
 	def __init__(self, adata : AnnData, likelihood,latent_dim:int = 50, hidden_layers :List=None,flow_length:int = 32,workers:int=5,parameters=[1,0,1,0,0],batch_size:int = 100,log_sigma_coff:int = 1):
 		super(DeepPredictor,self).__init__()
```

### Comparing `deepcellpredictor-0.9.5/DCP/flow.py` & `deepcellpredictor-0.9.6/DCP/flow.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.5/DCP/utils.py` & `deepcellpredictor-0.9.6/DCP/utils.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.5/LICENSE` & `deepcellpredictor-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.9.5/setup.py` & `deepcellpredictor-0.9.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.9.5'
+VERSION = '0.9.6'
 DESCRIPTION = "a transfer learning approach that explicitly models changes in transcriptional variance using a combination of variational autoencoders and normalizing flows"
 
 setup(
     name='deepcellpredictor',
     version=VERSION,
     description='transfer learning approach',
     long_description=DESCRIPTION,
```

