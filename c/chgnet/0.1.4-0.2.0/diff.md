# Comparing `tmp/chgnet-0.1.4.tar.gz` & `tmp/chgnet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chgnet-0.1.4.tar", last modified: Sat Jun 24 04:56:41 2023, max compression
+gzip compressed data, was "chgnet-0.2.0.tar", last modified: Sat Jul 22 02:30:04 2023, max compression
```

## Comparing `chgnet-0.1.4.tar` & `chgnet-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.570674 chgnet-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-24 04:56:31.000000 chgnet-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-24 04:56:41.570674 chgnet-0.1.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9357 2023-06-24 04:56:31.000000 chgnet-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.558674 chgnet-0.1.4/chgnet/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.558674 chgnet-0.1.4/chgnet/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30798 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.558674 chgnet-0.1.4/chgnet/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/graph/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/graph/crystalgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/graph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.562674 chgnet-0.1.4/chgnet/model/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/composition_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20235 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    32348 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.562674 chgnet-0.1.4/chgnet/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)  4639235 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/pretrained/e30f77s348m32.pth.tar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.566674 chgnet-0.1.4/chgnet/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27116 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.570674 chgnet-0.1.4/chgnet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-06-24 04:56:31.000000 chgnet-0.1.4/chgnet/utils/vasp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.558674 chgnet-0.1.4/chgnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 04:56:41.000000 chgnet-0.1.4/chgnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-24 04:56:31.000000 chgnet-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 04:56:41.570674 chgnet-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:56:41.570674 chgnet-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_crystal_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_relaxation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-24 04:56:31.000000 chgnet-0.1.4/tests/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.774775 chgnet-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-22 02:29:53.000000 chgnet-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-07-22 02:30:04.774775 chgnet-0.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9801 2023-07-22 02:29:53.000000 chgnet-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.762775 chgnet-0.2.0/chgnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.762775 chgnet-0.2.0/chgnet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30724 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.762775 chgnet-0.2.0/chgnet/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/graph/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/graph/crystalgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/graph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.766775 chgnet-0.2.0/chgnet/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/model/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/model/composition_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/model/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/model/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32340 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.766775 chgnet-0.2.0/chgnet/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)  4639235 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/pretrained/e30f77s348m32.pth.tar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.770775 chgnet-0.2.0/chgnet/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27121 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.770775 chgnet-0.2.0/chgnet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-22 02:29:53.000000 chgnet-0.2.0/chgnet/utils/vasp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.762775 chgnet-0.2.0/chgnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-07-22 02:30:04.000000 chgnet-0.2.0/chgnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-22 02:30:04.000000 chgnet-0.2.0/chgnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 02:30:04.000000 chgnet-0.2.0/chgnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-22 02:30:04.000000 chgnet-0.2.0/chgnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-22 02:30:04.000000 chgnet-0.2.0/chgnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-22 02:29:53.000000 chgnet-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 02:30:04.774775 chgnet-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-22 02:29:53.000000 chgnet-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:30:04.774775 chgnet-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-22 02:29:53.000000 chgnet-0.2.0/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-07-22 02:29:53.000000 chgnet-0.2.0/tests/test_crystal_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-22 02:29:53.000000 chgnet-0.2.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-22 02:29:53.000000 chgnet-0.2.0/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-22 02:29:53.000000 chgnet-0.2.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-22 02:29:53.000000 chgnet-0.2.0/tests/test_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-07-22 02:29:53.000000 chgnet-0.2.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-22 02:29:53.000000 chgnet-0.2.0/tests/test_relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-22 02:29:53.000000 chgnet-0.2.0/tests/test_trainer.py
```

### Comparing `chgnet-0.1.4/LICENSE` & `chgnet-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.4/PKG-INFO` & `chgnet-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chgnet
-Version: 0.1.4
+Version: 0.2.0
 Summary: Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling
 Author-email: Bowen Deng <bowendeng@berkeley.edu>
 License: Modified BSD
 Project-URL: Source, https://github.com/CederGroupHub/chgnet
 Project-URL: Package, https://pypi.org/project/chgnet
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -16,92 +16,101 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: crystal-toolkit
+Provides-Extra: docs
 License-File: LICENSE
 
 <h1 align="center">CHGNet</h1>
 
 <h4 align="center">
 
 [![Tests](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml)
-[![Linting](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e3bdcea0382a495d96408e4f84408e85)](https://app.codacy.com/gh/CederGroupHub/chgnet/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.14231-blue)](https://arxiv.org/abs/2302.14231)
 ![GitHub repo size](https://img.shields.io/github/repo-size/CederGroupHub/chgnet)
 [![PyPI](https://img.shields.io/pypi/v/chgnet?logo=pypi&logoColor=white)](https://pypi.org/project/chgnet?logo=pypi&logoColor=white)
+[![Docs](https://img.shields.io/badge/API-Docs-blue)](https://chgnet.lbl.gov)
 
 </h4>
 
 A pretrained universal neural network potential for
 **charge**-informed atomistic modeling
-![chgnet](chgnet-logo.png)
+![Logo](https://raw.github.com/CederGroupHub/chgnet/main/site/static/chgnet-logo.png)
 **C**rystal **H**amiltonian **G**raph neural **Net**work is pretrained on the GGA/GGA+U static and relaxation trajectories from Materials Project,
 a comprehensive dataset consisting of 1.5 Million structures from 146k compounds spanning the whole periodic table.
 
 CHGNet highlights its ability to study electron interactions and charge distribution
 in atomistic modeling with near DFT accuracy. The charge inference is realized by regularizing the atom features with
 DFT magnetic moments, which carry rich information about both local ionic environments and charge distribution.
 
+Pretrained CHGNet achieves SOTA performance on materials stability prediction from unrelaxed structures according to [Matbench Discovery](https://matbench-discovery.materialsproject.org) [[repo](https://github.com/janosh/matbench-discovery)].
+
 ## Example notebooks
 
 | Notebooks                                                                                                                | Links&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;                                                                                                     | Descriptions                                                                                                                        |
 | ------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
-| [**CHGNet Basics**](https://github.com/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                     | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)             | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
+| [**CHGNet Basics**](https://github.com/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                             | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                      | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
 | [**Tuning CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                        | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                 | Examples of fine tuning the pretrained CHGNet to your system of interest.                                                           |
 | [**Visualize Relaxation**](https://github.com/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | Crystal Toolkit that visualizes atom positions, energies and forces of a structure during CHGNet relaxation.                        |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 
 ## Installation
 
 You can install `chgnet` through `pip`:
 
 ```sh
 pip install chgnet
 ```
 
+## Docs
+
+View [API docs](https://cedergrouphub.github.io/chgnet/api).
+
 ## Usage
 
 ### Direct Inference (Static Calculation)
 
 Pretrained `CHGNet` can predict the energy (eV/atom), force (eV/A), stress (GPa) and
 magmom ($\mu_B$) of a given structure.
 
 ```python
 from chgnet.model.model import CHGNet
 from pymatgen.core import Structure
 
 chgnet = CHGNet.load()
-structure = Structure.from_file('examples/o-LiMnO2_unit.cif')
+structure = Structure.from_file('examples/mp-18767-LiMnO2.cif')
 prediction = chgnet.predict_structure(structure)
 for key in ("energy", "forces", "stress", "magmom"):
     print(f"CHGNet-predicted {key}={prediction[key[0]]}\n")
 ```
 
 ### Molecular Dynamics
 
 Charge-informed molecular dynamics can be simulated with pretrained `CHGNet` through `ASE` environment
 
 ```python
 from chgnet.model.model import CHGNet
 from chgnet.model.dynamics import MolecularDynamics
 from pymatgen.core import Structure
+import warnings
+warnings.filterwarnings("ignore", module="pymatgen")
+warnings.filterwarnings("ignore", module="ase")
 
-structure = Structure.from_file("examples/o-LiMnO2_unit.cif")
+structure = Structure.from_file("examples/mp-18767-LiMnO2.cif")
 chgnet = CHGNet.load()
 
 md = MolecularDynamics(
     atoms=structure,
     model=chgnet,
     ensemble="nvt",
-    compressibility_au=1.6,
     temperature=1000,  # in K
     timestep=2,  # in femto-seconds
     trajectory="md_out.traj",
     logfile="md_out.log",
     loginterval=100,
     use_device="cpu",  # use 'cuda' for faster MD
 )
@@ -172,36 +181,36 @@
 trainer.train(train_loader, val_loader, test_loader)
 ```
 
 ### Note
 
 1. The energy used for training should be energy/atom if you're fine-tuning the pretrained `CHGNet`.
 2. The pretrained dataset of `CHGNet` comes from GGA+U DFT with [`MaterialsProject2020Compatibility`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/entries/compatibility.py#L826-L1102).
-The parameter for VASP is described in [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879).
-If you're fine-tuning with [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879), it is recommended to apply the [`MP2020`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/entries/compatibility.py#L826-L1102)
-compatibility to your energy labels so that they're consistent with the pretrained dataset.
+   The parameter for VASP is described in [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879).
+   If you're fine-tuning with [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879), it is recommended to apply the [`MP2020`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/entries/compatibility.py#L826-L1102)
+   compatibility to your energy labels so that they're consistent with the pretrained dataset.
 3. If you're fine-tuning to functionals other than GGA, we recommend you refit the [`AtomRef`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/model/composition_model.py).
 4. `CHGNet` stress is in unit GPa, and the unit conversion has already been included in
-[`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py). So `VASP` stress can be directly fed to `StructureData`
+   [`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py). So `VASP` stress can be directly fed to `StructureData`
 5. To save time from graph conversion step for each training, we recommend you use [`GraphData`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py) defined in
-[`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py), which reads graphs directly from saved directory. To create saved graphs,
-see [`examples/make_graphs.py`](https://github.com/CederGroupHub/chgnet/blob/main/examples/make_graphs.py).
+   [`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py), which reads graphs directly from saved directory. To create saved graphs,
+   see [`examples/make_graphs.py`](https://github.com/CederGroupHub/chgnet/blob/main/examples/make_graphs.py).
 6. Apple’s Metal Performance Shaders `MPS` is currently disabled until a stable version of `pytorch` for `MPS` is released.
 
 ## Reference
 
 link to our paper:
 <https://doi.org/10.48550/arXiv.2302.14231>
 
 Please cite the following:
 
 ```bib
-@article{deng2023_chgnet,
+@article{deng_2023_chgnet,
   title={{CHGNet: Pretrained universal neural network potential for charge-informed atomistic modeling}},
-  author={Deng, Bowen and Zhong, Peichen and Jun, KyuJung and Han, Kevin and Bartel, Christopher J and Ceder, Gerbrand},
+  author={Deng, Bowen and Zhong, Peichen and Jun, KyuJung and Riebesell, Janosh and Han, Kevin and Bartel, Christopher J and Ceder, Gerbrand},
   journal={arXiv preprint arXiv:2302.14231},
   year={2023},
   url = {https://arxiv.org/abs/2302.14231}
 }
 ```
 
 ## Development & Bugs
```

### Comparing `chgnet-0.1.4/README.md` & `chgnet-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,83 +1,91 @@
 <h1 align="center">CHGNet</h1>
 
 <h4 align="center">
 
 [![Tests](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml)
-[![Linting](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e3bdcea0382a495d96408e4f84408e85)](https://app.codacy.com/gh/CederGroupHub/chgnet/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.14231-blue)](https://arxiv.org/abs/2302.14231)
 ![GitHub repo size](https://img.shields.io/github/repo-size/CederGroupHub/chgnet)
 [![PyPI](https://img.shields.io/pypi/v/chgnet?logo=pypi&logoColor=white)](https://pypi.org/project/chgnet?logo=pypi&logoColor=white)
+[![Docs](https://img.shields.io/badge/API-Docs-blue)](https://chgnet.lbl.gov)
 
 </h4>
 
 A pretrained universal neural network potential for
 **charge**-informed atomistic modeling
-![chgnet](chgnet-logo.png)
+![Logo](https://raw.github.com/CederGroupHub/chgnet/main/site/static/chgnet-logo.png)
 **C**rystal **H**amiltonian **G**raph neural **Net**work is pretrained on the GGA/GGA+U static and relaxation trajectories from Materials Project,
 a comprehensive dataset consisting of 1.5 Million structures from 146k compounds spanning the whole periodic table.
 
 CHGNet highlights its ability to study electron interactions and charge distribution
 in atomistic modeling with near DFT accuracy. The charge inference is realized by regularizing the atom features with
 DFT magnetic moments, which carry rich information about both local ionic environments and charge distribution.
 
+Pretrained CHGNet achieves SOTA performance on materials stability prediction from unrelaxed structures according to [Matbench Discovery](https://matbench-discovery.materialsproject.org) [[repo](https://github.com/janosh/matbench-discovery)].
+
 ## Example notebooks
 
 | Notebooks                                                                                                                | Links&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;                                                                                                     | Descriptions                                                                                                                        |
 | ------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
-| [**CHGNet Basics**](https://github.com/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                     | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)             | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
+| [**CHGNet Basics**](https://github.com/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                             | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                      | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
 | [**Tuning CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                        | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                 | Examples of fine tuning the pretrained CHGNet to your system of interest.                                                           |
 | [**Visualize Relaxation**](https://github.com/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | Crystal Toolkit that visualizes atom positions, energies and forces of a structure during CHGNet relaxation.                        |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 
 ## Installation
 
 You can install `chgnet` through `pip`:
 
 ```sh
 pip install chgnet
 ```
 
+## Docs
+
+View [API docs](https://cedergrouphub.github.io/chgnet/api).
+
 ## Usage
 
 ### Direct Inference (Static Calculation)
 
 Pretrained `CHGNet` can predict the energy (eV/atom), force (eV/A), stress (GPa) and
 magmom ($\mu_B$) of a given structure.
 
 ```python
 from chgnet.model.model import CHGNet
 from pymatgen.core import Structure
 
 chgnet = CHGNet.load()
-structure = Structure.from_file('examples/o-LiMnO2_unit.cif')
+structure = Structure.from_file('examples/mp-18767-LiMnO2.cif')
 prediction = chgnet.predict_structure(structure)
 for key in ("energy", "forces", "stress", "magmom"):
     print(f"CHGNet-predicted {key}={prediction[key[0]]}\n")
 ```
 
 ### Molecular Dynamics
 
 Charge-informed molecular dynamics can be simulated with pretrained `CHGNet` through `ASE` environment
 
 ```python
 from chgnet.model.model import CHGNet
 from chgnet.model.dynamics import MolecularDynamics
 from pymatgen.core import Structure
+import warnings
+warnings.filterwarnings("ignore", module="pymatgen")
+warnings.filterwarnings("ignore", module="ase")
 
-structure = Structure.from_file("examples/o-LiMnO2_unit.cif")
+structure = Structure.from_file("examples/mp-18767-LiMnO2.cif")
 chgnet = CHGNet.load()
 
 md = MolecularDynamics(
     atoms=structure,
     model=chgnet,
     ensemble="nvt",
-    compressibility_au=1.6,
     temperature=1000,  # in K
     timestep=2,  # in femto-seconds
     trajectory="md_out.traj",
     logfile="md_out.log",
     loginterval=100,
     use_device="cpu",  # use 'cuda' for faster MD
 )
@@ -148,36 +156,36 @@
 trainer.train(train_loader, val_loader, test_loader)
 ```
 
 ### Note
 
 1. The energy used for training should be energy/atom if you're fine-tuning the pretrained `CHGNet`.
 2. The pretrained dataset of `CHGNet` comes from GGA+U DFT with [`MaterialsProject2020Compatibility`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/entries/compatibility.py#L826-L1102).
-The parameter for VASP is described in [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879).
-If you're fine-tuning with [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879), it is recommended to apply the [`MP2020`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/entries/compatibility.py#L826-L1102)
-compatibility to your energy labels so that they're consistent with the pretrained dataset.
+   The parameter for VASP is described in [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879).
+   If you're fine-tuning with [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879), it is recommended to apply the [`MP2020`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/entries/compatibility.py#L826-L1102)
+   compatibility to your energy labels so that they're consistent with the pretrained dataset.
 3. If you're fine-tuning to functionals other than GGA, we recommend you refit the [`AtomRef`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/model/composition_model.py).
 4. `CHGNet` stress is in unit GPa, and the unit conversion has already been included in
-[`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py). So `VASP` stress can be directly fed to `StructureData`
+   [`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py). So `VASP` stress can be directly fed to `StructureData`
 5. To save time from graph conversion step for each training, we recommend you use [`GraphData`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py) defined in
-[`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py), which reads graphs directly from saved directory. To create saved graphs,
-see [`examples/make_graphs.py`](https://github.com/CederGroupHub/chgnet/blob/main/examples/make_graphs.py).
+   [`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py), which reads graphs directly from saved directory. To create saved graphs,
+   see [`examples/make_graphs.py`](https://github.com/CederGroupHub/chgnet/blob/main/examples/make_graphs.py).
 6. Apple’s Metal Performance Shaders `MPS` is currently disabled until a stable version of `pytorch` for `MPS` is released.
 
 ## Reference
 
 link to our paper:
 <https://doi.org/10.48550/arXiv.2302.14231>
 
 Please cite the following:
 
 ```bib
-@article{deng2023_chgnet,
+@article{deng_2023_chgnet,
   title={{CHGNet: Pretrained universal neural network potential for charge-informed atomistic modeling}},
-  author={Deng, Bowen and Zhong, Peichen and Jun, KyuJung and Han, Kevin and Bartel, Christopher J and Ceder, Gerbrand},
+  author={Deng, Bowen and Zhong, Peichen and Jun, KyuJung and Riebesell, Janosh and Han, Kevin and Bartel, Christopher J and Ceder, Gerbrand},
   journal={arXiv preprint arXiv:2302.14231},
   year={2023},
   url = {https://arxiv.org/abs/2302.14231}
 }
 ```
 
 ## Development & Bugs
```

### Comparing `chgnet-0.1.4/chgnet/data/dataset.py` & `chgnet-0.2.0/chgnet/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,17 +272,17 @@
             self.excluded_graph = utils.read_json(exclude)
         elif isinstance(exclude, list):
             self.excluded_graph = exclude
         else:
             self.excluded_graph = []
 
         self.keys = []
-        for mp_id, dic in self.labels.items():
-            for graph_id in dic:
-                self.keys.append((mp_id, graph_id))
+        self.keys = [
+            (mp_id, graph_id) for mp_id, dic in self.labels.items() for graph_id in dic
+        ]
         random.shuffle(self.keys)
         print(f"{len(self.labels)} mp_ids, {len(self)} frames imported")
         if self.excluded_graph is not None:
             print(f"{len(self.excluded_graph)} graphs are pre-excluded")
 
         self.energy_key = energy_key
         self.force_key = force_key
@@ -385,18 +385,16 @@
             random.shuffle(mp_ids)
             n_train = int(train_ratio * len(mp_ids))
             n_val = int(val_ratio * len(mp_ids))
             train_key = mp_ids[:n_train]
             val_key = mp_ids[n_train : n_train + n_val]
             test_key = mp_ids[n_train + n_val :]
         for mp_id in train_key:
-            try:
+            if mp_id in self.labels:
                 train_labels[mp_id] = self.labels.pop(mp_id)
-            except KeyError:
-                continue
         train_dataset = GraphData(
             graph_path=self.graph_path,
             labels=train_labels,
             targets=self.targets,
             exclude=self.excluded_graph,
             energy_str=self.energy_str,
         )
@@ -407,18 +405,16 @@
             shuffle=True,
             num_workers=num_workers,
             pin_memory=pin_memory,
         )
 
         # Val
         for mp_id in val_key:
-            try:
+            if mp_id in self.labels:
                 val_labels[mp_id] = self.labels.pop(mp_id)
-            except KeyError:
-                continue
         val_dataset = GraphData(
             graph_path=self.graph_path,
             labels=val_labels,
             targets=self.targets,
             exclude=self.excluded_graph,
             energy_str=self.energy_str,
         )
@@ -430,18 +426,16 @@
             num_workers=num_workers,
             pin_memory=pin_memory,
         )
 
         # Test
         if test_key is not None:
             for mp_id in test_key:
-                try:
+                if mp_id in self.labels:
                     test_labels[mp_id] = self.labels.pop(mp_id)
-                except KeyError:
-                    continue
             test_dataset = GraphData(
                 graph_path=self.graph_path,
                 labels=test_labels,
                 targets=self.targets,
                 exclude=self.excluded_graph,
                 energy_str=self.energy_str,
             )
@@ -498,20 +492,20 @@
                         self.data.update(utils.read_json(os.path.join(data, json_path)))
             else:
                 print(f"Importing: {data}")
                 self.data.update(utils.read_json(data))
         elif isinstance(data, dict):
             self.data = data
         else:
-            raise Exception("please provide a json path or dictionary")
+            raise ValueError(f"data must be JSON path or dictionary, got {type(data)}")
 
         self.keys = []
-        for mp_id, dic in self.data.items():
-            for graph_id in dic:
-                self.keys.append((mp_id, graph_id))
+        self.keys = [
+            (mp_id, graph_id) for mp_id, dic in self.data.items() for graph_id in dic
+        ]
         random.shuffle(self.keys)
         print(f"{len(self.data)} mp_ids, {len(self)} structures imported")
         self.graph_converter = graph_converter
         self.energy_key = energy_key
         self.force_key = force_key
         self.stress_key = stress_key
         self.magmom_key = magmom_key
@@ -665,35 +659,38 @@
             )
         else:
             test_loader = None
         return train_loader, val_loader, test_loader
 
 
 def collate_graphs(batch_data: list):
-    """Collate of list of (graph, target) into batch data,.
+    """Collate of list of (graph, target) into batch data.
 
     Args:
         batch_data (list): list of (graph, target(dict))
 
     Returns:
         graphs (List): a list of graphs
         targets (Dict): dictionary of targets, where key and values are:
             e (Tensor): energies of the structures [batch_size]
             f (Tensor): forces of the structures [n_batch_atoms, 3]
             s (Tensor): stresses of the structures [3*batch_size, 3]
             m (Tensor): magmom of the structures [n_batch_atoms]
     """
-    graphs = []
+    graphs = [graph for graph, _ in batch_data]
     all_targets = {key: [] for key in batch_data[0][1]}
-    for graph, targets in batch_data:
-        graphs.append(graph)
+    all_targets["e"] = torch.tensor(
+        [targets["e"] for _, targets in batch_data], dtype=datatype
+    )
+
+    for _, targets in batch_data:
         for target, value in targets.items():
-            all_targets[target].append(value)
-    if "e" in all_targets:
-        all_targets["e"] = torch.tensor(all_targets["e"], dtype=datatype)
+            if target != "e":
+                all_targets[target].append(value)
+
     return graphs, all_targets
 
 
 def get_train_val_test_loader(
     dataset: Dataset,
     batch_size: int = 64,
     train_ratio: float = 0.8,
```

### Comparing `chgnet-0.1.4/chgnet/graph/crystalgraph.py` & `chgnet-0.2.0/chgnet/graph/crystalgraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,31 +34,40 @@
         Args:
             atomic_number (Tensor): the atomic numbers of atoms in the structure
                 [n_atom]
             atom_frac_coord (Tensor): the fractional coordinates of the atoms
                 [n_atom, 3]
             atom_graph (Tensor): a directed graph adjacency list,
                 (center atom indices, neighbor atom indices, undirected bond index)
-                for bonds in bond_fea [2*n_bond, 3]
+                for bonds in bond_fea
+                [num_directed_bonds, 2]
             atom_graph_cutoff (float): the cutoff radius to draw edges in atom_graph
             neighbor_image (Tensor): the periodic image specifying the location of
-                neighboring atom [2*n_bond, 2]
+                neighboring atom
+                see: https://github.com/materialsproject/pymatgen/blob/ca2175c762e37ea7
+                c9f3950ef249bc540e683da1/pymatgen/core/structure.py#L1485-L1541
+                [num_directed_bonds, 3]
             directed2undirected (Tensor): the mapping from directed edge index to
-                undirected edge index for the atom graph [2*n_bond]
+                undirected edge index for the atom graph
+                [num_directed_bonds]
             undirected2directed (Tensor): the mapping from undirected edge index to
                 one of its directed edge index, this is essentially the inverse
                 mapping of the directed2undirected this tensor is needed for
-                computation efficiency. [n_bond]
+                computation efficiency.
+                Note that num_directed_bonds = 2 * num_undirected_bonds
+                [num_undirected_bonds]
             bond_graph (Tensor): a directed graph adjacency list,
                 (atom indices, 1st undirected bond idx, 1st directed bond idx,
                  2nd undirected bond idx, 2nd directed bond idx)
-                for angles in angle_fea [n_angle, 5]
+                for angles in angle_fea
+                [n_angle, 5]
             bond_graph_cutoff (float): the cutoff bond length to include bond
                 as nodes in bond_graph
-            lattice (Tensor): lattices of the input structure [3, 3]
+            lattice (Tensor): lattices of the input structure
+                [3, 3]
             graph_id (str or None): an id to keep track of this crystal graph
                 Default = None
             mp_id (str) or None: Materials Project id of this structure
                 Default = None
             composition: Chemical composition of the compound, used just for
                 better tracking of the graph
                 Default = None.
```

### Comparing `chgnet-0.1.4/chgnet/graph/graph.py` & `chgnet-0.2.0/chgnet/graph/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
                 [0, 1, 1, 4, 23],
                 [1, 4, 23, 5, 66],
                 ... ...  ]
                 the fist column specifies node(atom) index at this angle,
                 the second column specifies 1st undirected edge(left bond) index,
                 the third column specifies 1st directed edge(left bond) index,
                 the fourth column specifies 2nd undirected edge(right bond) index,
-                the fifth column specifies 2snd directed edge(right bond) index,.
+                the fifth column specifies 2nd directed edge(right bond) index,.
             undirected2directed:
                 [32, 45, ...]
                 a list of length = num_undirected_edge that
                 maps the undirected edge index to one of its directed edges indices
         """
         assert len(self.directed_edges_list) == 2 * len(self.undirected_edges_list), (
             f"Error: number of directed edges={len(self.directed_edges_list)} != 2 * "
@@ -315,18 +315,18 @@
                             )
         return line_graph, undirected2directed
 
     def undirected2directed(self):
         """The index map from undirected_edge index to one of its directed_edge
         index.
         """
-        out = []
-        for undirected_edge in self.undirected_edges_list:
-            out.append(undirected_edge.info["directed_edge_index"][0])
-        return out
+        return [
+            undirected_edge.info["directed_edge_index"][0]
+            for undirected_edge in self.undirected_edges_list
+        ]
 
     def as_dict(self):
         """Return dictionary serialization of a Graph."""
         return {
             "nodes": self.nodes,
             "directed_edges": self.directed_edges,
             "directed_edges_list": self.directed_edges_list,
```

### Comparing `chgnet-0.1.4/chgnet/model/basis.py` & `chgnet-0.2.0/chgnet/model/basis.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.4/chgnet/model/composition_model.py` & `chgnet-0.2.0/chgnet/model/composition_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,17 @@
         composition_feas = torch.zeros([num_data, self.max_num_elements])
         e = torch.zeros([num_data])
         for index, (structure, energy) in enumerate(
             zip(structures_or_graphs, energies)
         ):
             if isinstance(structure, Structure):
                 atomic_number = torch.tensor(
-                    [i.specie.Z for i in structure], dtype=int, requires_grad=False
+                    [site.specie.Z for site in structure],
+                    dtype=int,
+                    requires_grad=False,
                 )
             else:
                 atomic_number = structure.atomic_number
             composition_fea = torch.bincount(
                 atomic_number - 1, minlength=self.max_num_elements
             )
             if self.is_intensive:
```

### Comparing `chgnet-0.1.4/chgnet/model/dynamics.py` & `chgnet-0.2.0/chgnet/model/dynamics.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,36 +55,37 @@
         use_device: str | None = None,
         stress_weight: float | None = 1 / 160.21766208,
         **kwargs,
     ) -> None:
         """Provide a CHGNet instance to calculate various atomic properties using ASE.
 
         Args:
-            model (CHGNet): instance of a chgnet model
+            model (CHGNet): instance of a chgnet model. If set to None,
+                the pretrained CHGNet is loaded.
+                Default = None
             use_device (str, optional): The device to be used for predictions,
                 either "cpu", "cuda", or "mps". If not specified, the default device is
                 automatically selected based on the available options.
+                Default = None
             stress_weight (float): the conversion factor to convert GPa to eV/A^3.
-                Default = 1/160.21.
+                Default = 1/160.21
             **kwargs: Passed to the Calculator parent class.
         """
         super().__init__(**kwargs)
 
         # mps is disabled before stable version of pytorch on apple mps is released
         if use_device == "mps":
-            raise NotImplementedError("mps is not supported yet")
+            raise NotImplementedError("'mps' backend is not supported yet")
         # elif torch.backends.mps.is_available():
         #     self.device = 'mps'
         # Determine the device to use
         self.device = use_device or ("cuda" if torch.cuda.is_available() else "cpu")
 
         # Move the model to the specified device
-        if model is None:
-            model = CHGNet.load()
-        self.model = model.to(self.device)
+        self.model = (model or CHGNet.load()).to(self.device)
         self.stress_weight = stress_weight
         print(f"CHGNet will run on {self.device}")
 
     def calculate(
         self,
         atoms: Atoms | None = None,
         properties: list | None = None,
@@ -132,29 +133,32 @@
         optimizer_class: Optimizer | str | None = "FIRE",
         use_device: str | None = None,
         stress_weight: float = 1 / 160.21766208,
     ) -> None:
         """Provide a trained CHGNet model and an optimizer to relax crystal structures.
 
         Args:
-            model (CHGNet): instance of a chgnet model
+            model (CHGNet): instance of a chgnet model. If set to None,
+                the pretrained CHGNet is loaded.
+                Default = None
             optimizer_class (Optimizer,str): choose optimizer from ASE.
-                Default = FIRE
+                Default = "FIRE"
             use_device (str, optional): The device to be used for predictions,
                 either "cpu", "cuda", or "mps". If not specified, the default device is
                 automatically selected based on the available options.
+                Default = None
             stress_weight (float): the conversion factor to convert GPa to eV/A^3.
-                Default = 1/160.21.
+                Default = 1/160.21
         """
         if isinstance(optimizer_class, str):
             if optimizer_class in OPTIMIZERS:
                 optimizer_class = OPTIMIZERS[optimizer_class]
             else:
                 raise ValueError(
-                    f"Optimizer instance not found. Select one from {list(OPTIMIZERS)}"
+                    f"Optimizer instance not found. Select from {list(OPTIMIZERS)}"
                 )
 
         self.optimizer_class: Optimizer = optimizer_class
         self.calculator = CHGNetCalculator(
             model=model, stress_weight=stress_weight, use_device=use_device
         )
 
@@ -184,16 +188,16 @@
             trajectory_save_interval (int | None): Trajectory save interval.
                 Default = 1
             verbose (bool): Whether to print the output of the ASE optimizer.
                 Default = True
             **kwargs: Additional parameters for the optimizer.
 
         Returns:
-            dict[str, Structure | TrajectoryObserver]: A dictionary with keys 'final_structure'
-                and 'trajectory'.
+            dict[str, Structure | TrajectoryObserver]:
+                A dictionary with 'final_structure' and 'trajectory'.
         """
         if isinstance(atoms, Structure):
             atoms = AseAtomsAdaptor.get_atoms(atoms)
 
         atoms.calc = self.calculator  # assign model used to predict forces
 
         stream = sys.stdout if verbose else io.StringIO()
@@ -208,18 +212,18 @@
 
         if save_path is not None:
             obs.save(save_path)
 
         if isinstance(atoms, ExpCellFilter):
             atoms = atoms.atoms
         struct = AseAtomsAdaptor.get_structure(atoms)
-        for k in struct.site_properties:
-            struct.remove_site_property(property_name=k)
+        for key in struct.site_properties:
+            struct.remove_site_property(property_name=key)
         struct.add_site_property(
-            "magmom", [float(i) for i in atoms.get_magnetic_moments()]
+            "magmom", [float(magmom) for magmom in atoms.get_magnetic_moments()]
         )
         return {"final_structure": struct, "trajectory": obs}
 
 
 class TrajectoryObserver:
     """Trajectory observer is a hook in the relaxation process that saves the
     intermediate structures.
@@ -308,20 +312,21 @@
                 Default = "nvt"
             temperature (float): temperature for MD simulation, in K
                 Default = 300
             timestep (float): time step in fs
                 Default = 2
             pressure (float): pressure in eV/A^3
                 Default = 1.01325 * units.bar
-            taut (float): time constant for Berendsen temperature coupling
-                Default = None
-            taup (float): time constant for pressure coupling
-                Default = None
-            compressibility_au (float): compressibility of the material in A^3/eV,
-                this value is needed for npt ensemble
+            taut (float): time constant for Berendsen temperature coupling in fs
+                Default = 100 * timestep
+            taup (float): time constant for pressure coupling in fs
+                Default = 1000 * timestep
+            compressibility_au (float): compressibility of the material in A^3/eV
+                for npt ensemble, if not provided, it will be calculated by CHGNet
+                through Birch Murnaghan equation of state
                 Default = None
             trajectory (str or Trajectory): Attach trajectory object
                 Default = None
             logfile (str): open this file for recording MD outputs
                 Default = None
             loginterval (int): write to log file every interval steps
                 Default = 1
@@ -345,15 +350,15 @@
             """
             Berendsen (constant N, V, T) molecular dynamics.
             """
             self.dyn = NVTBerendsen(
                 atoms=self.atoms,
                 timestep=timestep * units.fs,
                 temperature_K=temperature,
-                taut=taut,
+                taut=taut * units.fs,
                 trajectory=trajectory,
                 logfile=logfile,
                 loginterval=loginterval,
                 append_trajectory=append_trajectory,
             )
         else:
             if compressibility_au is None:
@@ -376,16 +381,16 @@
                 """
 
                 self.dyn = Inhomogeneous_NPTBerendsen(
                     atoms=self.atoms,
                     timestep=timestep * units.fs,
                     temperature_K=temperature,
                     pressure_au=pressure,
-                    taut=taut,
-                    taup=taup,
+                    taut=taut * units.fs,
+                    taup=taup * units.fs,
                     compressibility_au=compressibility_au,
                     trajectory=trajectory,
                     logfile=logfile,
                     loginterval=loginterval,
                 )
 
             elif ensemble.lower() == "npt_berendsen":
@@ -397,16 +402,16 @@
                 """
 
                 self.dyn = NPTBerendsen(
                     atoms=self.atoms,
                     timestep=timestep * units.fs,
                     temperature_K=temperature,
                     pressure_au=pressure,
-                    taut=taut,
-                    taup=taup,
+                    taut=taut * units.fs,
+                    taup=taup * units.fs,
                     compressibility_au=compressibility_au,
                     trajectory=trajectory,
                     logfile=logfile,
                     loginterval=loginterval,
                     append_trajectory=append_trajectory,
                 )
 
@@ -449,22 +454,25 @@
         optimizer_class: Optimizer | str | None = "FIRE",
         use_device: str | None = None,
         stress_weight: float = 1 / 160.21766208,
     ) -> None:
         """Initialize a structure optimizer object for calculation of bulk modulus.
 
         Args:
-            model (CHGNet): instance of a chgnet model
+            model (CHGNet): instance of a chgnet model. If set to None,
+                the pretrained CHGNet is loaded.
+                Default = None
             optimizer_class (Optimizer,str): choose optimizer from ASE.
-                Default = FIRE
+                Default = "FIRE"
             use_device (str, optional): The device to be used for predictions,
                 either "cpu", "cuda", or "mps". If not specified, the default device is
                 automatically selected based on the available options.
+                Default = None
             stress_weight (float): the conversion factor to convert GPa to eV/A^3.
-                Default = 1/160.21.
+                Default = 1/160.21
         """
         self.relaxer = StructOptimizer(
             model=model,
             optimizer_class=optimizer_class,
             use_device=use_device,
             stress_weight=stress_weight,
         )
@@ -491,32 +499,32 @@
 
         Returns:
             Bulk Modulus (float)
         """
         if isinstance(atoms, Atoms):
             atoms = AseAtomsAdaptor.get_structure(atoms)
         volumes, energies = [], []
-        for i in np.linspace(-0.1, 0.1, n_points):
+        for idx in np.linspace(-0.1, 0.1, n_points):
             structure_strained = atoms.copy()
-            structure_strained.apply_strain([i, i, i])
+            structure_strained.apply_strain([idx, idx, idx])
             result = self.relaxer.relax(
                 structure_strained,
                 relax_cell=False,
                 fmax=fmax,
                 steps=steps,
                 verbose=False,
                 **kwargs,
             )
             volumes.append(result["final_structure"].volume)
             energies.append(result["trajectory"].energies[-1])
         self.bm = BirchMurnaghan(volumes=volumes, energies=energies)
         self.bm.fit()
         self.fitted = True
 
-    def get_bulk_mudulus(self, unit: str = "eV/A^3"):
+    def get_bulk_modulus(self, unit: str = "eV/A^3"):
         """Get the bulk modulus of from the fitted Birch-Murnaghan equation of state.
 
         Args:
             unit (str): The unit of bulk modulus. Can be "eV/A^3" or "GPa"
                 Default = "eV/A^3"
 
         Returns:
```

### Comparing `chgnet-0.1.4/chgnet/model/encoders.py` & `chgnet-0.2.0/chgnet/model/encoders.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.4/chgnet/model/functions.py` & `chgnet-0.2.0/chgnet/model/functions.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.4/chgnet/model/layers.py` & `chgnet-0.2.0/chgnet/model/layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,39 +21,41 @@
         bond_fea_dim: int,
         hidden_dim: int = 64,
         dropout: float = 0,
         activation: str = "silu",
         norm: str | None = None,
         use_mlp_out: bool = True,
         resnet: bool = True,
-        gMLP_norm: str = "batch",
+        gMLP_norm: str | None = None,
     ) -> None:
-        """Args:
-        atom_fea_dim (int): The dimensionality of the input atom features.
-        bond_fea_dim (int): The dimensionality of the input bond features.
-        hidden_dim (int, optional): The dimensionality of the hidden layers in the
-            gated MLP.
-            Default = 64.
-        dropout (float, optional): The dropout probability to apply to the gated MLP.
-            Default = 0.
-        activation (str, optional): The name of the activation function to use in the
-            gated MLP.
-        Must be one of "relu", "silu", "tanh", or "gelu". Default = "silu".
-        norm (str, optional): The name of the normalization layer to use on the updated
-            atom features. Must be one of "batch", "layer", or None.
-            Default = None.
-        use_mlp_out (bool, optional): Whether to apply an MLP output layer to the
-            updated atom features.
-            Default = True.
-        resnet (bool, optional): Whether to apply a residual connection to the
-            updated atom features.
-            Default = True.
-        gMLP_norm (str, optional): The name of the normalization layer to use on the
-            gated MLP. Must be one of "batch", "layer", or None. Default = "batch".
-        **kwargs: Additional keyword arguments to pass to the normalization layer.
+        """Initialize the AtomConv layer.
+
+        Args:
+            atom_fea_dim (int): The dimensionality of the input atom features.
+            bond_fea_dim (int): The dimensionality of the input bond features.
+            hidden_dim (int, optional): The dimensionality of the hidden layers in the
+                gated MLP.
+                Default = 64
+            dropout (float, optional): The dropout rate to apply to the gated MLP.
+                Default = 0.
+            activation (str, optional): The name of the activation function to use in
+                the gated MLP. Must be one of "relu", "silu", "tanh", or "gelu".
+                Default = "silu"
+            norm (str, optional): The name of the normalization layer to use on the
+                updated atom features. Must be one of "batch", "layer", or None.
+                Default = None
+            use_mlp_out (bool, optional): Whether to apply an MLP output layer to the
+                updated atom features.
+                Default = True
+            resnet (bool, optional): Whether to apply a residual connection to the
+                updated atom features.
+                Default = True
+            gMLP_norm (str, optional): The name of the normalization layer to use on the
+                gated MLP. Must be one of "batch", "layer", or None.
+                Default = None
         """
         super().__init__()
         self.use_mlp_out = use_mlp_out
         self.resnet = resnet
         self.activation = find_activation(activation)
         self.twoBody_atom = GatedMLP(
             input_dim=2 * atom_fea_dim + bond_fea_dim,
@@ -136,50 +138,53 @@
         angle_fea_dim: int,
         hidden_dim: int = 64,
         dropout: float = 0,
         activation: str = "silu",
         norm: str | None = None,
         use_mlp_out: bool = True,
         resnet=True,
-        **kwargs,
+        gMLP_norm: str | None = None,
     ) -> None:
-        """Args:
-        atom_fea_dim (int): The dimensionality of the input atom features.
-        bond_fea_dim (int): The dimensionality of the input bond features.
-        angle_fea_dim (int): The dimensionality of the input angle features.
-        hidden_dim (int, optional): The dimensionality of the hidden layers
-            in the gated MLP.
-            Default = 64.
-        dropout (float, optional): The dropout probability to apply to the gated MLP.
-            Default = 0.
-        activation (str, optional): The name of the activation function to use
-            in the gated MLP.
-        Must be one of "relu", "silu", "tanh", or "gelu". Default = "silu".
-        norm (str, optional): The name of the normalization layer to use on the
-            updated atom features.
-        Must be one of "batch", "layer", or None.
-            Default = None.
-        use_mlp_out (bool, optional): Whether to apply an MLP output layer to the
-            updated atom features.
-            Default = True.
-        resnet (bool, optional): Whether to apply a residual connection to the
-            updated atom features.
-            Default = True.
-        **kwargs: Additional keyword arguments to pass to the normalization layer.
+        """Initialize the BondConv layer.
+
+        Args:
+            atom_fea_dim (int): The dimensionality of the input atom features.
+            bond_fea_dim (int): The dimensionality of the input bond features.
+            angle_fea_dim (int): The dimensionality of the input angle features.
+            hidden_dim (int, optional): The dimensionality of the hidden layers
+                in the gated MLP.
+                Default = 64
+            dropout (float, optional): The dropout rate to apply to the gated MLP.
+                Default = 0.
+            activation (str, optional): The name of the activation function to use
+                in the gated MLP. Must be one of "relu", "silu", "tanh", or "gelu".
+                Default = "silu"
+            norm (str, optional): The name of the normalization layer to use on the
+                updated atom features. Must be one of "batch", "layer", or None.
+                Default = None
+            use_mlp_out (bool, optional): Whether to apply an MLP output layer to the
+                updated atom features.
+                Default = True
+            resnet (bool, optional): Whether to apply a residual connection to the
+                updated atom features.
+                Default = True
+            gMLP_norm (str, optional): The name of the normalization layer to use on the
+                gated MLP. Must be one of "batch", "layer", or None.
+                Default = None
         """
         super().__init__()
         self.use_mlp_out = use_mlp_out
         self.resnet = resnet
         self.activation = find_activation(activation)
         self.twoBody_bond = GatedMLP(
             input_dim=atom_fea_dim + 2 * bond_fea_dim + angle_fea_dim,
             output_dim=bond_fea_dim,
             hidden_dim=hidden_dim,
             dropout=dropout,
-            norm=kwargs.pop("gMLP_norm", "batch"),
+            norm=gMLP_norm,
             activation=activation,
         )
         if self.use_mlp_out:
             self.mlp_out = MLP(
                 input_dim=bond_fea_dim, output_dim=bond_fea_dim, hidden_dim=0
             )
         self.bond_norm = find_normalization(name=norm, dim=bond_fea_dim)
@@ -198,21 +203,21 @@
             atom_feas (Tensor): atom features tensor with shape
                 [num_batch_atoms, atom_fea_dim]
             bond_feas (Tensor): bond features tensor with shape
                 [num_undirected_bonds, bond_fea_dim]
             bond_weights (Tensor): BondGraph bond weights with shape
                 [num_undirected_bonds, bond_fea_dim]
             angle_feas (Tensor): angle features tensor with shape
-                [num_batch_angles, atom_fea_dim]
+                [num_batch_angles, angle_fea_dim]
             bond_graph (Tensor): Directed BondGraph tensor with shape
                 [num_batched_angles, 3]
 
         Returns:
             new_bond_feas (Tensor): bond feature tensor with shape
-                [num_batch_atom, bond_fea_dim]
+                [num_undirected_bonds, bond_fea_dim]
 
         Notes:
             - num_batch_atoms = sum(num_atoms) in batch
         """
         # Make directional Message
         center_atoms = torch.index_select(atom_feas, 0, bond_graph[:, 0])
         bond_feas_i = torch.index_select(bond_feas, 0, bond_graph[:, 1])
@@ -253,48 +258,49 @@
         bond_fea_dim: int,
         angle_fea_dim: int,
         hidden_dim: int = 0,
         dropout: float = 0,
         activation: str = "silu",
         norm: str | None = None,
         resnet: bool = True,
-        **kwargs,
+        gMLP_norm: str | None = None,
     ) -> None:
-        """Create a new AngleUpdate instance.
+        """Initialize the AngleUpdate layer.
 
         Args:
             atom_fea_dim (int): The dimensionality of the input atom features.
             bond_fea_dim (int): The dimensionality of the input bond features.
             angle_fea_dim (int): The dimensionality of the input angle features.
             hidden_dim (int, optional): The dimensionality of the hidden layers
                 in the gated MLP.
-                Default = 0.
-            dropout (float, optional): The dropout probability to apply to the gated MLP.
+                Default = 0
+            dropout (float, optional): The dropout rate to apply to the gated MLP.
                 Default = 0.
             activation (str, optional): The name of the activation function to use
                 in the gated MLP. Must be one of "relu", "silu", "tanh", or "gelu".
-                Default = "silu".
+                Default = "silu"
             norm (str, optional): The name of the normalization layer to use on the
-                updated atom features.
-            Must be one of "batch", "layer", or None.
-                Default = None.
+                updated atom features. Must be one of "batch", "layer", or None.
+                Default = None
             resnet (bool, optional): Whether to apply a residual connection to the
                 updated atom features.
-                Default = True.
-            **kwargs: Additional keyword arguments to pass to the normalization layer.
+                Default = True
+            gMLP_norm (str, optional): The name of the normalization layer to use on the
+                gated MLP. Must be one of "batch", "layer", or None.
+                Default = None
         """
         super().__init__()
         self.resnet = resnet
         self.activation = find_activation(activation)
         self.twoBody_bond = GatedMLP(
             input_dim=atom_fea_dim + 2 * bond_fea_dim + angle_fea_dim,
             output_dim=angle_fea_dim,
             hidden_dim=hidden_dim,
             dropout=dropout,
-            norm=kwargs.pop("gMLP_norm", "batch"),
+            norm=gMLP_norm,
             activation=activation,
         )
         self.angle_norm = find_normalization(norm, dim=angle_fea_dim)
 
     def forward(
         self,
         atom_feas: Tensor,
@@ -306,21 +312,21 @@
 
         Args:
             atom_feas (Tensor): atom features tensor with shape
                 [num_batch_atoms, atom_fea_dim]
             bond_feas (Tensor): bond features tensor with shape
                 [num_undirected_bonds, bond_fea_dim]
             angle_feas (Tensor): angle features tensor with shape
-                [num_batch_angles, atom_fea_dim]
+                [num_batch_angles, angle_fea_dim]
             bond_graph (Tensor): Directed BondGraph tensor with shape
                 [num_batched_angles, 3]
 
         Returns:
             new_angle_feas (Tensor): angle features tensor with shape
-                [num_batch_angles, atom_fea_dim]
+                [num_batch_angles, angle_fea_dim]
 
         Notes:
             - num_batch_atoms = sum(num_atoms) in batch
         """
         # Assemble features
         center_atoms = torch.index_select(atom_feas, 0, bond_graph[:, 0])
         bond_feas_i = torch.index_select(bond_feas, 0, bond_graph[:, 1])
@@ -351,19 +357,21 @@
         self.average = average
 
     def forward(self, atom_feas: Tensor, atom_owner: Tensor) -> Tensor:
         """Merge the atom features that belong to same graph in a batched graph.
 
         Args:
             atom_feas (Tensor): batched atom features after convolution layers.
-                shape = [num_batch_atoms, atom_fea_dim]
-            atom_owner (Tensor): graph indices for each atom. shape = [num_batch_atoms]
+                [num_batch_atoms, atom_fea_dim or 1]
+            atom_owner (Tensor): graph indices for each atom.
+                [num_batch_atoms]
 
         Returns:
-            crystal_feas (Tensor): crystal feature matrix. shape = [n_crystals, atom_fea_dim]
+            crystal_feas (Tensor): crystal feature matrix.
+                [n_crystals, atom_fea_dim or 1]
         """
         return aggregate(atom_feas, atom_owner, average=self.average)
 
 
 class GraphAttentionReadOut(nn.Module):
     """Multi Head Attention Read Out Layer
     merge the information from atom_feas to crystal_fea.
@@ -388,19 +396,21 @@
         self.average = average
 
     def forward(self, atom_feas: Tensor, atom_owner: Tensor) -> Tensor:
         """Merge the atom features that belong to same graph in a batched graph.
 
         Args:
             atom_feas (Tensor): batched atom features after convolution layers.
-                shape = [num_batch_atoms, atom_fea_dim]
-            atom_owner (Tensor): graph indices for each atom. shape = [num_batch_atoms]
+                [num_batch_atoms, atom_fea_dim]
+            atom_owner (Tensor): graph indices for each atom.
+                [num_batch_atoms]
 
         Returns:
-            crystal_feas (Tensor): crystal feature matrix. shape = [n_crystals, atom_fea_dim]
+            crystal_feas (Tensor): crystal feature matrix.
+                [n_crystals, atom_fea_dim]
         """
         crystal_feas = []
         weights = self.key(atom_feas)  # [n_batch_atom, n_heads]
         bin_count = torch.bincount(atom_owner)
         start_index = 0
         for n_atom in bin_count:
             # find atoms belong to this crystal. shape = [n_atom, atom_fea_dim]
```

### Comparing `chgnet-0.1.4/chgnet/model/model.py` & `chgnet-0.2.0/chgnet/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,16 +48,17 @@
         conv_dropout: float = 0,
         read_out: str = "ave",
         mlp_hidden_dims: Sequence[int] | int = (64, 64),
         mlp_dropout: float = 0,
         mlp_first: bool = True,
         is_intensive: bool = True,
         non_linearity: Literal["silu", "relu", "tanh", "gelu"] = "silu",
-        atom_graph_cutoff: int = 5,
-        bond_graph_cutoff: int = 3,
+        atom_graph_cutoff: float = 5,
+        bond_graph_cutoff: float = 3,
+        graph_converter_algorithm: Literal["legacy", "fast"] = "fast",
         cutoff_coeff: int = 5,
         learnable_rbf: bool = True,
         **kwargs,
     ) -> None:
         """Initialize the CHGNet.
 
         Args:
@@ -67,15 +68,17 @@
                 Default = 64
             angle_fea_dim (int): angle feature vector embedding dimension.
                 Default = 64
             bond_fea_dim (int): angle feature vector embedding dimension.
                 Default = 64
             composition_model (nn.Module, optional): attach a composition model to
                 predict energy or initialize a pretrained linear regression (AtomRef).
-                Default = None
+                The default 'MPtrj' is the atom reference energy linear regression
+                trained on all Materials Project relaxation trajectories
+                Default = 'MPtrj'
             num_radial (int): number of radial basis used in bond basis expansion.
                 Default = 9
             num_angular (int): number of angular basis used in angle basis expansion.
                 Default = 9
             n_conv (int): number of interaction blocks.
                 Default = 4
                 Note: last interaction block contain only an atom_conv layer
@@ -105,22 +108,30 @@
                 Default = 0.
             is_intensive (bool): whether the energy training label is intensive
                 i.e. energy per atom.
                 Default = True
             non_linearity ('silu' | 'relu' | 'tanh' | 'gelu'): The name of the
                 activation function to use in the gated MLP.
                 Default = "silu".
-            mlp_first (bool): whether to apply mlp fist then pooling.
+            mlp_first (bool): whether to apply mlp first then pooling.
+                if set to True, then CHGNet is essentially calculating energy for each
+                atom, them sum them up, this is used for the pretrained model
                 Default = True
             atom_graph_cutoff (float): cutoff radius (A) in creating atom_graph,
                 this need to be consistent with the value in training dataloader
                 Default = 5
             bond_graph_cutoff (float): cutoff radius (A) in creating bond_graph,
                 this need to be consistent with value in training dataloader
                 Default = 3
+            graph_converter_algorithm ('legacy' | 'fast'): algorithm to use
+                for converting pymatgen.core.Structure to CrystalGraph.
+                'legacy': python implementation of graph creation
+                'fast': C implementation of graph creation, this is faster,
+                    but will need the cygraph.c file correctly compiled from pip install
+                default = 'fast'
             cutoff_coeff (float): cutoff strength used in graph smooth cutoff function.
                 the smaller this coeff is, the smoother the basis is
                 Default = 5
             learnable_rbf (bool): whether to set the frequencies in rbf and Fourier
                 basis functions learnable.
                 Default = True
             **kwargs: Additional keyword arguments
@@ -151,15 +162,18 @@
         if self.composition_model is not None:
             # fixed composition_model weights
             for param in self.composition_model.parameters():
                 param.requires_grad = False
 
         # Define Crystal Graph Converter
         self.graph_converter = CrystalGraphConverter(
-            atom_graph_cutoff=atom_graph_cutoff, bond_graph_cutoff=bond_graph_cutoff
+            atom_graph_cutoff=atom_graph_cutoff,
+            bond_graph_cutoff=bond_graph_cutoff,
+            algorithm=graph_converter_algorithm,
+            verbose=kwargs.pop("converter_verbose", False),
         )
 
         # Define embedding layers
         self.atom_embedding = AtomEmbedding(atom_feature_dim=atom_fea_dim)
         self.bond_basis_expansion = BondEncoder(
             atom_graph_cutoff=atom_graph_cutoff,
             bond_graph_cutoff=bond_graph_cutoff,
@@ -182,29 +196,28 @@
         self.angle_embedding = nn.Linear(
             in_features=num_angular, out_features=angle_fea_dim, bias=False
         )
 
         # Define convolutional layers
         conv_norm = kwargs.pop("conv_norm", None)
         gMLP_norm = kwargs.pop("gMLP_norm", None)
-        atom_graph_layers = []
-        for _i in range(n_conv):
-            atom_graph_layers.append(
-                AtomConv(
-                    atom_fea_dim=atom_fea_dim,
-                    bond_fea_dim=bond_fea_dim,
-                    hidden_dim=atom_conv_hidden_dim,
-                    dropout=conv_dropout,
-                    activation=non_linearity,
-                    norm=conv_norm,
-                    gMLP_norm=gMLP_norm,
-                    use_mlp_out=True,
-                    resnet=True,
-                )
+        atom_graph_layers = [
+            AtomConv(
+                atom_fea_dim=atom_fea_dim,
+                bond_fea_dim=bond_fea_dim,
+                hidden_dim=atom_conv_hidden_dim,
+                dropout=conv_dropout,
+                activation=non_linearity,
+                norm=conv_norm,
+                gMLP_norm=gMLP_norm,
+                use_mlp_out=True,
+                resnet=True,
             )
+            for _ in range(n_conv)
+        ]
         self.atom_conv_layers = nn.ModuleList(atom_graph_layers)
 
         if update_bond is True:
             bond_graph_layers = [
                 BondConv(
                     atom_fea_dim=atom_fea_dim,
                     bond_fea_dim=bond_fea_dim,
@@ -454,16 +467,15 @@
         if compute_force:
             # Need to retain_graph here, because energy is used in loss function,
             # so its gradient need to be calculated later
             # The graphs of force and stress need to be created for same reason.
             force = torch.autograd.grad(
                 energy.sum(), g.atom_positions, create_graph=True, retain_graph=True
             )
-            force = [-1 * i for i in force]
-            prediction["f"] = force
+            prediction["f"] = [-1 * force_dim for force_dim in force]
 
         # Compute stress
         if compute_stress:
             stress = torch.autograd.grad(
                 energy.sum(), g.strains, create_graph=True, retain_graph=True
             )
             # Convert Stress unit from eV/A^3 to GPa
@@ -481,19 +493,19 @@
     def predict_structure(
         self,
         structure: Structure | Sequence[Structure],
         task: PredTask = "efsm",
         return_atom_feas: bool = False,
         return_crystal_feas: bool = False,
         batch_size: int = 100,
-    ) -> dict[str, Tensor]:
+    ) -> dict[str, Tensor] | list[dict[str, Tensor]]:
         """Predict from pymatgen.core.Structure.
 
         Args:
-            structure (Structure, List(Structure)): structure or a list of structures
+            structure (Structure | Sequence[Structure]): structure or a list of structures
                 to predict.
             task (str): can be 'e' 'ef', 'em', 'efs', 'efsm'
                 Default = "efsm"
             return_atom_feas (bool): whether to return atom features.
                 Default = False
             return_crystal_feas (bool): whether to return crystal features.
                 only available if self.mlp_first is False
@@ -504,133 +516,108 @@
         Returns:
             prediction (dict[str, Tensor]): containing the keys:
                 e: energy of structures [batch_size, 1] in eV/atom
                 f: force on atoms [num_batch_atoms, 3] in eV/A
                 s: stress of structure [3 * batch_size, 3] in GPa
                 m: magnetic moments of sites [num_batch_atoms, 3] in Bohr magneton mu_B
         """
-        assert (
-            self.graph_converter is not None
-        ), "self.graph_converter needs to be initialized first!"
-        if type(structure) == Structure:
-            graph = self.graph_converter(structure)
-            return self.predict_graph(
-                graph,
-                task=task,
-                return_atom_feas=return_atom_feas,
-                return_crystal_feas=return_crystal_feas,
-                batch_size=batch_size,
-            )
-        if type(structure) == list:
-            graphs = [self.graph_converter(i) for i in structure]
-            return self.predict_graph(
-                graphs,
-                task=task,
-                return_atom_feas=return_atom_feas,
-                return_crystal_feas=return_crystal_feas,
-                batch_size=batch_size,
-            )
-        raise Exception("input should either be a structure or list of structures!")
+        if self.graph_converter is None:
+            raise ValueError("graph_converter cannot be None!")
+
+        structures = [structure] if isinstance(structure, Structure) else structure
+
+        graphs = [self.graph_converter(struct) for struct in structures]
+        return self.predict_graph(
+            graphs,
+            task=task,
+            return_atom_feas=return_atom_feas,
+            return_crystal_feas=return_crystal_feas,
+            batch_size=batch_size,
+        )
 
     def predict_graph(
         self,
         graph: CrystalGraph | Sequence[CrystalGraph],
         task: PredTask = "efsm",
         return_atom_feas: bool = False,
         return_crystal_feas: bool = False,
         batch_size: int = 100,
-    ) -> dict[str, Tensor]:
-        """Args:
-            graph (CrystalGraph): Crystal_Graph or a list of CrystalGraphs to predict.
+    ) -> dict[str, Tensor] | list[dict[str, Tensor]]:
+        """Predict from CrustalGraph.
+
+        Args:
+            graph (CrystalGraph | Sequence[CrystalGraph]): CrystalGraph(s) to predict.
             task (str): can be 'e' 'ef', 'em', 'efs', 'efsm'
                 Default = "efsm"
             return_atom_feas (bool): whether to return atom features.
                 Default = False
             return_crystal_feas (bool): whether to return crystal features.
                 only available if self.mlp_first is False
                 Default = False
             batch_size (int): batch_size for predict structures.
-                Default = 100.
+                Default = 100
 
         Returns:
             prediction (dict): containing the fields:
                 e (Tensor) : energy of structures [batch_size, 1]
                 f (Tensor) : force on atoms [num_batch_atoms, 3]
                 s (Tensor) : stress of structure [3 * batch_size, 3]
                 m (Tensor) : magnetic moments of sites [num_batch_atoms, 3]
         """
+        if not isinstance(graph, (CrystalGraph, Sequence)):
+            raise ValueError(
+                f"{type(graph)=} must be CrystalGraph or list of CrystalGraphs"
+            )
+
         model_device = next(self.parameters()).device
-        if type(graph) == CrystalGraph:
-            self.eval()
+
+        graphs = [graph] if isinstance(graph, CrystalGraph) else graph
+        self.eval()
+        predictions: list[dict[str, Tensor]] = [{} for _ in range(len(graphs))]
+        n_steps = math.ceil(len(graphs) / batch_size)
+        for step in range(n_steps):
             prediction = self.forward(
-                [graph.to(model_device)],
+                [
+                    g.to(model_device)
+                    for g in graphs[batch_size * step : batch_size * (step + 1)]
+                ],
                 task=task,
                 return_atom_feas=return_atom_feas,
                 return_crystal_feas=return_crystal_feas,
             )
-            out = {}
             for key, pred in prediction.items():
-                if key == "e":
-                    out[key] = pred.item()
-                elif key in ["f", "s", "m", "atom_fea"]:
-                    assert len(pred) == 1
-                    out[key] = pred[0].cpu().detach().numpy()
+                if key in ["e"]:
+                    for i, e in enumerate(pred.cpu().detach().numpy()):
+                        predictions[step * batch_size + i][key] = e
+                elif key in ["f", "s", "m"]:
+                    for i, tmp in enumerate(pred):
+                        predictions[step * batch_size + i][key] = (
+                            tmp.cpu().detach().numpy()
+                        )
+                elif key == "atom_fea":
+                    for i, atom_fea in enumerate(pred):
+                        predictions[step * batch_size + i][key] = (
+                            atom_fea.cpu().detach().numpy()
+                        )
                 elif key == "crystal_fea":
-                    out[key] = pred.view(-1).cpu().detach().numpy()
-            return out
-        if type(graph) == list:
-            self.eval()
-            predictions: list[dict[str, Tensor]] = [{} for _ in range(len(graph))]
-            n_steps = math.ceil(len(graph) / batch_size)
-            for n in range(n_steps):
-                prediction = self.forward(
-                    [
-                        g.to(model_device)
-                        for g in graph[batch_size * n : batch_size * (n + 1)]
-                    ],
-                    task=task,
-                    return_atom_feas=return_atom_feas,
-                    return_crystal_feas=return_crystal_feas,
-                )
-                for key, pred in prediction.items():
-                    if key in ["e"]:
-                        for i, e in enumerate(pred.cpu().detach().numpy()):
-                            predictions[n * batch_size + i][key] = e
-                    elif key in ["f", "s", "m"]:
-                        for i, tmp in enumerate(pred):
-                            predictions[n * batch_size + i][key] = (
-                                tmp.cpu().detach().numpy()
-                            )
-                    elif key == "atom_fea":
-                        for i, atom_fea in enumerate(pred):
-                            predictions[n * batch_size + i][key] = (
-                                atom_fea.cpu().detach().numpy()
-                            )
-                    elif key == "crystal_fea":
-                        for i, crystal_fea in enumerate(pred.cpu().detach().numpy()):
-                            predictions[n * batch_size + i][key] = crystal_fea
-            return predictions
-        raise Exception("input should either be a graph or list of graphs!")
-
-    @staticmethod
-    def split(x: Tensor, n: Tensor) -> Sequence[Tensor]:
-        """Split a batched result Tensor into a list of Tensors."""
-        print(x, n)
-        start = 0
-        result = []
-        for i in n:
-            result.append(x[start : start + i])
-            start += i
-        assert start == len(x), "Error: source tensor not correctly split!"
-        return result
+                    for i, crystal_fea in enumerate(pred.cpu().detach().numpy()):
+                        predictions[step * batch_size + i][key] = crystal_fea
+
+        return predictions[0] if len(graphs) == 1 else predictions
 
     def as_dict(self):
         """Return the CHGNet weights and args in a dictionary."""
         return {"state_dict": self.state_dict(), "model_args": self.model_args}
 
+    def todict(self):
+        """Needed for ASE JSON serialization when saving CHGNet potential to
+        trajectory file (https://github.com/CederGroupHub/chgnet/issues/48).
+        """
+        return {"model_name": type(self).__name__, "model_args": self.model_args}
+
     @classmethod
     def from_dict(cls, dict, **kwargs):
         """Build a CHGNet from a saved dictionary."""
         chgnet = CHGNet(**dict["model_args"])
         chgnet.load_state_dict(dict["state_dict"], **kwargs)
         return chgnet
 
@@ -644,45 +631,45 @@
     def load(cls, model_name="MPtrj-efsm"):
         """Load pretrained CHGNet."""
         current_dir = os.path.dirname(os.path.abspath(__file__))
         if model_name == "MPtrj-efsm":
             return cls.from_file(
                 os.path.join(current_dir, "../pretrained/e30f77s348m32.pth.tar")
             )
-        raise Exception("model_name not supported")
+        raise ValueError(f"Unknown {model_name=}")
 
 
 @dataclass
 class BatchedGraph:
     """Batched crystal graph for parallel computing.
 
     Attributes:
         atomic_numbers (Tensor): atomic numbers vector
             [num_batch_atoms]
         bond_bases_ag (Tensor): bond bases vector for atom_graph
-            [num_batch_bonds, num_radial]
+            [num_batch_bonds_ag, num_radial]
         bond_bases_bg (Tensor): bond bases vector for atom_graph
-            [num_batch_bonds, num_radial]
+            [num_batch_bonds_bg, num_radial]
         angle_bases (Tensor): angle bases vector
             [num_batch_angles, num_angular]
         batched_atom_graph (Tensor) : batched atom graph adjacency list
             [num_batch_bonds, 2]
         batched_bond_graph (Tensor) : bond graph adjacency list
-            [num_batch_angles, 2]
+            [num_batch_angles, 3]
         atom_owners (Tensor): graph indices for each atom, used aggregate batched
             graph back to single graph
             [num_batch_atoms]
         directed2undirected (Tensor): the utility tensor used to quickly
             map directed edges to undirected edges in graph
             [num_directed]
         atom_positions (list[Tensor]): cartesian coordinates of the atoms
             from structures
-            [num_batch_atoms]
+            [[num_atoms_1, 3], [num_atoms_2, 3], ...]
         strains (list[Tensor]): a list of strains that's initialized to be zeros
-            [batch_size]
+            [[3, 3], [3, 3], ...]
         volumes (Tensor): the volume of each structure in the batch
             [batch_size]
     """
 
     atomic_numbers: Tensor
     bond_bases_ag: Tensor
     bond_bases_bg: Tensor
@@ -752,14 +739,17 @@
             bond_bases_bg.append(bond_basis_bg)
 
             # Indexes
             batched_atom_graph.append(graph.atom_graph + atom_offset_idx)
             directed2undirected.append(graph.directed2undirected + n_undirected)
 
             # Angles
+            # Here we use directed edges to calculate angles, and
+            # keep only the undirected graph index in the bond_graph,
+            # So the number of columns in bond_graph reduce from 5 to 3
             if len(graph.bond_graph) != 0:
                 bond_vecs_i = torch.index_select(
                     bond_vectors, 0, graph.bond_graph[:, 2]
                 )
                 bond_vecs_j = torch.index_select(
                     bond_vectors, 0, graph.bond_graph[:, 4]
                 )
```

### Comparing `chgnet-0.1.4/chgnet/pretrained/e30f77s348m32.pth.tar` & `chgnet-0.2.0/chgnet/pretrained/e30f77s348m32.pth.tar`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.4/chgnet/trainer/trainer.py` & `chgnet-0.2.0/chgnet/trainer/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,16 +248,15 @@
                 test_mae = self._validate(
                     test_loader, is_test=True, test_result_save_path=save_dir
                 )
             else:
                 test_mae = self._validate(
                     test_loader, is_test=True, test_result_save_path=None
                 )
-            for key in self.targets:
-                self.training_history[key]["test"].append(test_mae[key])
+            self.training_history[key]["test"] = [test_mae[key] for key in self.targets]
 
     def _train(self, train_loader: DataLoader, current_epoch: int) -> dict:
         """Train all data for one epoch.
 
         Args:
             train_loader (DataLoader): train loader to update CHGNet weights
             current_epoch (int): used for resume unfinished training
@@ -265,16 +264,16 @@
         Returns:
             dictionary of training errors
         """
         batch_time = AverageMeter()
         data_time = AverageMeter()
         losses = AverageMeter()
         mae_errors = {}
-        for i in self.targets:
-            mae_errors[i] = AverageMeter()
+        for target in self.targets:
+            mae_errors[target] = AverageMeter()
 
         # switch to train mode
         self.model.train()
 
         start = time.perf_counter()  # start timer
         for idx, (graphs, targets) in enumerate(train_loader):
             # measure data loading time
@@ -444,16 +443,17 @@
             message += f"{key}_MAE ({mae_errors[key].avg:.3f}) \t"
         print(message)
         return {k: round(mae_error.avg, 6) for k, mae_error in mae_errors.items()}
 
     def get_best_model(self):
         """Get best model recorded in the trainer."""
         if self.best_model is None:
-            raise Exception("the model needs to be trained first")
-        print("Best model has val MAE = ", min(self.training_history["e"]["val"]))
+            raise RuntimeError("the model needs to be trained first")
+        MAE = min(self.training_history["e"]["val"])
+        print(f"Best model has val {MAE = :.4}")
         return self.best_model
 
     @property
     def _init_keys(self):
         return [
             key
             for key in list(inspect.signature(Trainer.__init__).parameters)
@@ -474,15 +474,15 @@
     def save_checkpoint(
         self, epoch: int, mae_error: dict, save_dir: str | None = None
     ) -> None:
         """Function to save CHGNet trained weights after each epoch.
 
         Args:
             epoch (int): the epoch number
-            mae_error (dict): dictionary that stores the mae errors
+            mae_error (dict): dictionary that stores the MAEs
             save_dir (str): the directory to save trained weights
         """
         for fname in os.listdir(save_dir):
             if fname.startswith("epoch"):
                 os.remove(os.path.join(save_dir, fname))
 
         rounded_mae_e = round(mae_error["e"] * 1000)
```

### Comparing `chgnet-0.1.4/chgnet/utils/common_utils.py` & `chgnet-0.2.0/chgnet/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.4/chgnet/utils/vasp_utils.py` & `chgnet-0.2.0/chgnet/utils/vasp_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     charge = []
     mag_x = []
     mag_y = []
     mag_z = []
     header = []
     all_lines = []
 
-    for line in reverse_readfile(outcar_filename):  # filename : self.filenaem
+    for line in reverse_readfile(outcar_filename):  # filename : self.filename
         clean = line.strip()
         all_lines.append(clean)
 
     all_lines.reverse()
     # For single atom systems, VASP doesn't print a total line, so
     # reverse parsing is very difficult
     read_charge = False
@@ -56,24 +56,24 @@
         if read_charge or read_mag_x or read_mag_y or read_mag_z:
             if clean.startswith("# of ion"):
                 header = re.split(r"\s{2,}", clean.strip())
                 header.pop(0)
             else:
                 m = re.match(r"\s*(\d+)\s+(([\d\.\-]+)\s+)+", clean)
                 if m:
-                    toks = [float(i) for i in re.findall(r"[\d\.\-]+", clean)]
-                    toks.pop(0)
+                    tokens = [float(token) for token in re.findall(r"[\d\.\-]+", clean)]
+                    tokens.pop(0)
                     if read_charge:
-                        charge.append(dict(zip(header, toks)))
+                        charge.append(dict(zip(header, tokens)))
                     elif read_mag_x:
-                        mag_x.append(dict(zip(header, toks)))
+                        mag_x.append(dict(zip(header, tokens)))
                     elif read_mag_y:
-                        mag_y.append(dict(zip(header, toks)))
+                        mag_y.append(dict(zip(header, tokens)))
                     elif read_mag_z:
-                        mag_z.append(dict(zip(header, toks)))
+                        mag_z.append(dict(zip(header, tokens)))
                 elif clean.startswith("tot"):
                     if ion_step_count == (len(mag_x_all) + 1):
                         mag_x_all.append(mag_x)
                     read_charge = False
                     read_mag_x = False
                     read_mag_y = False
                     read_mag_z = False
@@ -104,24 +104,26 @@
         print("Unfinished OUTCAR")
         mag_x_all = mag_x_all
     elif len(oszicar.ionic_steps) == (len(mag_x_all) - 1):  ## finished job
         mag_x_all.pop(-1)
 
     n_atoms = len(vasprun_orig.ionic_steps[0]["structure"])
     dataset = {
-        "structure": [i["structure"] for i in vasprun_orig.ionic_steps],
-        "uncorrected_total_energy": [i["e_0_energy"] for i in vasprun_orig.ionic_steps],
+        "structure": [step["structure"] for step in vasprun_orig.ionic_steps],
+        "uncorrected_total_energy": [
+            step["e_0_energy"] for step in vasprun_orig.ionic_steps
+        ],
         "energy_per_atom": [
-            i["e_0_energy"] / n_atoms for i in vasprun_orig.ionic_steps
+            step["e_0_energy"] / n_atoms for step in vasprun_orig.ionic_steps
         ],
-        "force": [i["forces"] for i in vasprun_orig.ionic_steps],
-        "magmom": [[i["tot"] for i in j] for j in mag_x_all],
+        "force": [step["forces"] for step in vasprun_orig.ionic_steps],
+        "magmom": [[step["tot"] for step in j] for j in mag_x_all],
     }
     if "stress" in vasprun_orig.ionic_steps[0]:
-        dataset["stress"] = [i["stress"] for i in vasprun_orig.ionic_steps]
+        dataset["stress"] = [step["stress"] for step in vasprun_orig.ionic_steps]
     else:
         dataset["stress"] = None
 
     return dataset
 
 
 def solve_charge_by_mag(
@@ -130,44 +132,42 @@
     ox_ranges: dict[str, dict[tuple[float, float], int]] | None = None,
 ):
     """Solve oxidation states by magmom.
 
     Args:
         structure: input pymatgen structure
         default_ox (dict[str, float]): default oxidation state for elements.
-            Default = {"Li": 1, "O": -2}
-        ox_ranges (dict[str, dict[tuple[float, float], int]]): user defined range to
+            Default = dict(Li=1, O=-2)
+        ox_ranges (dict[str, dict[tuple[float, float], int]]): user-defined range to
             convert magmoms into formal valence.
             Example for Mn (Default):
-                {"Mn": {
-                (0.5, 1.5): 2,
-                (1.5, 2.5): 3,
-                (2.5, 3.5): 4,
-                (3.5, 4.2): 3,
-                (4.2, 5): 2
-                }}
+                ("Mn": (
+                    (0.5, 1.5): 2,
+                    (1.5, 2.5): 3,
+                    (2.5, 3.5): 4,
+                    (3.5, 4.2): 3,
+                    (4.2, 5): 2
+                ))
     """
     ox_list = []
     solved_ox = True
     default_ox = default_ox or {"Li": 1, "O": -2}
     ox_ranges = ox_ranges or {
         "Mn": {(0.5, 1.5): 2, (1.5, 2.5): 3, (2.5, 3.5): 4, (3.5, 4.2): 3, (4.2, 5): 2}
     }
 
-    mag_key = (
-        "final_magmom" if "final_magmom" in structure.site_properties else "magmom"
+    mag = structure.site_properties.get(
+        "final_magmom", structure.site_properties.get("magmom")
     )
 
-    mag = structure.site_properties[mag_key]
-
-    for site_i, site in enumerate(structure.sites):
+    for idx, site in enumerate(structure):
         assigned = False
         if site.species_string in ox_ranges:
             for (minmag, maxmag), magox in ox_ranges[site.species_string].items():
-                if mag[site_i] >= minmag and mag[site_i] < maxmag:
+                if mag[idx] >= minmag and mag[idx] < maxmag:
                     ox_list.append(magox)
                     assigned = True
                     break
         elif site.species_string in default_ox:
             ox_list.append(default_ox[site.species_string])
             assigned = True
         if not assigned:
```

### Comparing `chgnet-0.1.4/chgnet.egg-info/PKG-INFO` & `chgnet-0.2.0/chgnet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chgnet
-Version: 0.1.4
+Version: 0.2.0
 Summary: Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling
 Author-email: Bowen Deng <bowendeng@berkeley.edu>
 License: Modified BSD
 Project-URL: Source, https://github.com/CederGroupHub/chgnet
 Project-URL: Package, https://pypi.org/project/chgnet
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -16,92 +16,101 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: crystal-toolkit
+Provides-Extra: docs
 License-File: LICENSE
 
 <h1 align="center">CHGNet</h1>
 
 <h4 align="center">
 
 [![Tests](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml)
-[![Linting](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/lint.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e3bdcea0382a495d96408e4f84408e85)](https://app.codacy.com/gh/CederGroupHub/chgnet/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.14231-blue)](https://arxiv.org/abs/2302.14231)
 ![GitHub repo size](https://img.shields.io/github/repo-size/CederGroupHub/chgnet)
 [![PyPI](https://img.shields.io/pypi/v/chgnet?logo=pypi&logoColor=white)](https://pypi.org/project/chgnet?logo=pypi&logoColor=white)
+[![Docs](https://img.shields.io/badge/API-Docs-blue)](https://chgnet.lbl.gov)
 
 </h4>
 
 A pretrained universal neural network potential for
 **charge**-informed atomistic modeling
-![chgnet](chgnet-logo.png)
+![Logo](https://raw.github.com/CederGroupHub/chgnet/main/site/static/chgnet-logo.png)
 **C**rystal **H**amiltonian **G**raph neural **Net**work is pretrained on the GGA/GGA+U static and relaxation trajectories from Materials Project,
 a comprehensive dataset consisting of 1.5 Million structures from 146k compounds spanning the whole periodic table.
 
 CHGNet highlights its ability to study electron interactions and charge distribution
 in atomistic modeling with near DFT accuracy. The charge inference is realized by regularizing the atom features with
 DFT magnetic moments, which carry rich information about both local ionic environments and charge distribution.
 
+Pretrained CHGNet achieves SOTA performance on materials stability prediction from unrelaxed structures according to [Matbench Discovery](https://matbench-discovery.materialsproject.org) [[repo](https://github.com/janosh/matbench-discovery)].
+
 ## Example notebooks
 
 | Notebooks                                                                                                                | Links&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;                                                                                                     | Descriptions                                                                                                                        |
 | ------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
-| [**CHGNet Basics**](https://github.com/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                     | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)             | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
+| [**CHGNet Basics**](https://github.com/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                             | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/basics.ipynb)                      | Examples for loading pre-trained CHGNet, predicting energy, force, stress, magmom as well as running structure optimization and MD. |
 | [**Tuning CHGNet**](https://github.com/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                        | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/fine_tuning.ipynb)                 | Examples of fine tuning the pretrained CHGNet to your system of interest.                                                           |
 | [**Visualize Relaxation**](https://github.com/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/CederGroupHub/chgnet/blob/main/examples/crystaltoolkit_relax_viewer.ipynb) | Crystal Toolkit that visualizes atom positions, energies and forces of a structure during CHGNet relaxation.                        |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 
 ## Installation
 
 You can install `chgnet` through `pip`:
 
 ```sh
 pip install chgnet
 ```
 
+## Docs
+
+View [API docs](https://cedergrouphub.github.io/chgnet/api).
+
 ## Usage
 
 ### Direct Inference (Static Calculation)
 
 Pretrained `CHGNet` can predict the energy (eV/atom), force (eV/A), stress (GPa) and
 magmom ($\mu_B$) of a given structure.
 
 ```python
 from chgnet.model.model import CHGNet
 from pymatgen.core import Structure
 
 chgnet = CHGNet.load()
-structure = Structure.from_file('examples/o-LiMnO2_unit.cif')
+structure = Structure.from_file('examples/mp-18767-LiMnO2.cif')
 prediction = chgnet.predict_structure(structure)
 for key in ("energy", "forces", "stress", "magmom"):
     print(f"CHGNet-predicted {key}={prediction[key[0]]}\n")
 ```
 
 ### Molecular Dynamics
 
 Charge-informed molecular dynamics can be simulated with pretrained `CHGNet` through `ASE` environment
 
 ```python
 from chgnet.model.model import CHGNet
 from chgnet.model.dynamics import MolecularDynamics
 from pymatgen.core import Structure
+import warnings
+warnings.filterwarnings("ignore", module="pymatgen")
+warnings.filterwarnings("ignore", module="ase")
 
-structure = Structure.from_file("examples/o-LiMnO2_unit.cif")
+structure = Structure.from_file("examples/mp-18767-LiMnO2.cif")
 chgnet = CHGNet.load()
 
 md = MolecularDynamics(
     atoms=structure,
     model=chgnet,
     ensemble="nvt",
-    compressibility_au=1.6,
     temperature=1000,  # in K
     timestep=2,  # in femto-seconds
     trajectory="md_out.traj",
     logfile="md_out.log",
     loginterval=100,
     use_device="cpu",  # use 'cuda' for faster MD
 )
@@ -172,36 +181,36 @@
 trainer.train(train_loader, val_loader, test_loader)
 ```
 
 ### Note
 
 1. The energy used for training should be energy/atom if you're fine-tuning the pretrained `CHGNet`.
 2. The pretrained dataset of `CHGNet` comes from GGA+U DFT with [`MaterialsProject2020Compatibility`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/entries/compatibility.py#L826-L1102).
-The parameter for VASP is described in [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879).
-If you're fine-tuning with [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879), it is recommended to apply the [`MP2020`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/entries/compatibility.py#L826-L1102)
-compatibility to your energy labels so that they're consistent with the pretrained dataset.
+   The parameter for VASP is described in [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879).
+   If you're fine-tuning with [`MPRelaxSet`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/io/vasp/sets.py#L862-L879), it is recommended to apply the [`MP2020`](https://github.com/materialsproject/pymatgen/blob/v2023.2.28/pymatgen/entries/compatibility.py#L826-L1102)
+   compatibility to your energy labels so that they're consistent with the pretrained dataset.
 3. If you're fine-tuning to functionals other than GGA, we recommend you refit the [`AtomRef`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/model/composition_model.py).
 4. `CHGNet` stress is in unit GPa, and the unit conversion has already been included in
-[`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py). So `VASP` stress can be directly fed to `StructureData`
+   [`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py). So `VASP` stress can be directly fed to `StructureData`
 5. To save time from graph conversion step for each training, we recommend you use [`GraphData`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py) defined in
-[`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py), which reads graphs directly from saved directory. To create saved graphs,
-see [`examples/make_graphs.py`](https://github.com/CederGroupHub/chgnet/blob/main/examples/make_graphs.py).
+   [`dataset.py`](https://github.com/CederGroupHub/chgnet/blob/main/chgnet/data/dataset.py), which reads graphs directly from saved directory. To create saved graphs,
+   see [`examples/make_graphs.py`](https://github.com/CederGroupHub/chgnet/blob/main/examples/make_graphs.py).
 6. Apple’s Metal Performance Shaders `MPS` is currently disabled until a stable version of `pytorch` for `MPS` is released.
 
 ## Reference
 
 link to our paper:
 <https://doi.org/10.48550/arXiv.2302.14231>
 
 Please cite the following:
 
 ```bib
-@article{deng2023_chgnet,
+@article{deng_2023_chgnet,
   title={{CHGNet: Pretrained universal neural network potential for charge-informed atomistic modeling}},
-  author={Deng, Bowen and Zhong, Peichen and Jun, KyuJung and Han, Kevin and Bartel, Christopher J and Ceder, Gerbrand},
+  author={Deng, Bowen and Zhong, Peichen and Jun, KyuJung and Riebesell, Janosh and Han, Kevin and Bartel, Christopher J and Ceder, Gerbrand},
   journal={arXiv preprint arXiv:2302.14231},
   year={2023},
   url = {https://arxiv.org/abs/2302.14231}
 }
 ```
 
 ## Development & Bugs
```

### Comparing `chgnet-0.1.4/chgnet.egg-info/SOURCES.txt` & `chgnet-0.2.0/chgnet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.py
 chgnet/__init__.py
 chgnet.egg-info/PKG-INFO
 chgnet.egg-info/SOURCES.txt
 chgnet.egg-info/dependency_links.txt
 chgnet.egg-info/requires.txt
 chgnet.egg-info/top_level.txt
 chgnet/data/__init__.py
```

### Comparing `chgnet-0.1.4/pyproject.toml` & `chgnet-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
-requires = ["setuptools>=65.0"]
+requires = ["Cython", "setuptools>=65.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chgnet"
-version = "0.1.04"
+version = "0.2.0"
 description = "Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling"
 authors = [{ name = "Bowen Deng", email = "bowendeng@berkeley.edu" }]
 requires-python = ">=3.8"
 readme = "README.md"
 license = { text = "Modified BSD" }
 dependencies = [
     "ase>=3.22.0",
+    "cython>=0.29.26",
     "numpy>=1.21.6",
     "pymatgen>=2022.4.19",
     "torch>=1.11.0",
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
@@ -29,14 +30,15 @@
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 # needed to run interactive example notebooks
 crystal-toolkit = ["crystal-toolkit"]
+docs = ["lazydocs"]
 
 [project.urls]
 Source = "https://github.com/CederGroupHub/chgnet"
 Package = "https://pypi.org/project/chgnet"
 
 [tool.setuptools.packages]
 find = { include = ["chgnet*"], exclude = ["tests", "tests*"] }
@@ -44,14 +46,15 @@
 [tool.setuptools.package-data]
 "chgnet" = ["*.json"]
 "chgnet.pretrained" = ["*.tar"]
 
 [tool.ruff]
 target-version = "py38"
 line-length = 95
+include = ["**/pyproject.toml", "*.ipynb", "*.py", "*.pyi"]
 select = [
     "B",    # flake8-bugbear
     "C4",   # flake8-comprehensions
     "D",    # pydocstyle
     "E",    # pycodestyle error
     "EXE",  # flake8-executable
     "F",    # pyflakes
@@ -92,14 +95,14 @@
     "PT013",   # pytest-incorrect-pytest-import
 ]
 pydocstyle.convention = "google"
 isort.required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["D103"]
-"examples/*" = ["E402"] # E402 Module level import not at top of file
+"examples/*" = ["E402", "I002"] # E402 Module level import not at top of file
 
 [tool.coverage.run]
 source = ["chgnet"]
 
 [tool.coverage.report]
 omit = ["tests/*"]
```

### Comparing `chgnet-0.1.4/tests/test_converter.py` & `chgnet-0.2.0/tests/test_converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,22 +11,30 @@
 coords = [[0, 0, 0], [0.5, 0.5, 0.5]]
 NaCl = Structure(lattice, species, coords)
 
 
 @pytest.mark.parametrize(
     "atom_graph_cutoff, bond_graph_cutoff", [(5, 3), (5, None), (4, 2)]
 )
-def test_crystal_graph_converter_init(atom_graph_cutoff, bond_graph_cutoff):
+def test_crystal_graph_converter_cutoff(atom_graph_cutoff, bond_graph_cutoff):
     converter = CrystalGraphConverter(
         atom_graph_cutoff=atom_graph_cutoff, bond_graph_cutoff=bond_graph_cutoff
     )
     assert converter.atom_graph_cutoff == atom_graph_cutoff
     assert converter.bond_graph_cutoff == bond_graph_cutoff or atom_graph_cutoff
 
 
+@pytest.mark.parametrize("algorithm", ["legacy", "fast"])
+def test_crystal_graph_converter_algorithm(algorithm):
+    converter = CrystalGraphConverter(
+        atom_graph_cutoff=5, bond_graph_cutoff=3, algorithm=algorithm
+    )
+    assert converter.algorithm == algorithm
+
+
 @pytest.mark.parametrize("on_isolated_atoms", ["ignore", "warn", "error"])
 def test_crystal_graph_converter_forward(
     on_isolated_atoms, capsys: CaptureFixture[str]
 ):
     converter = CrystalGraphConverter(atom_graph_cutoff=5, bond_graph_cutoff=3)
     strained = NaCl.copy()
     strained.apply_strain(5)
@@ -54,17 +62,16 @@
 
 def test_crystal_graph_converter_get_neighbors():
     converter = CrystalGraphConverter()
     center_index, neighbor_index, image, _distance = converter.get_neighbors(NaCl)
 
     assert list(center_index) == [0] * 14 + [1] * 14
     assert list(neighbor_index) == [
-        # fmt: off
-        1, 1, 1, 1, 0, 1, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1
-        # fmt: on
+        *(1, 1, 1, 1, 0, 1, 1, 0, 1, 0, 0, 0, 0, 1),
+        *(1, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1),
     ]
     expected_image = [
         [-1, -1, -1],
         [-1, -1, 0],
         [-1, 0, -1],
         [-1, 0, 0],
         [-1, 0, 0],
@@ -95,8 +102,11 @@
     for img, expected in zip(image, expected_image):
         assert list(img) == expected
 
 
 def test_crystal_graph_converter_as_dict_round_trip():
     expected = {"atom_graph_cutoff": 5, "bond_graph_cutoff": 3}
     converter = CrystalGraphConverter(**expected)
-    assert CrystalGraphConverter.from_dict(converter.as_dict()).as_dict() == expected
+    converter2 = CrystalGraphConverter.from_dict(converter.as_dict())
+    assert converter.atom_graph_cutoff == converter2.atom_graph_cutoff
+    assert converter.bond_graph_cutoff == converter2.bond_graph_cutoff
+    assert converter.algorithm == converter2.algorithm
```

### Comparing `chgnet-0.1.4/tests/test_dataset.py` & `chgnet-0.2.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.4/tests/test_encoders.py` & `chgnet-0.2.0/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.4/tests/test_graph.py` & `chgnet-0.2.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.1.4/tests/test_md.py` & `chgnet-0.2.0/tests/test_md.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 from __future__ import annotations
 
 import os
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
+import pytest
 from ase import Atoms
 from ase.md.nptberendsen import Inhomogeneous_NPTBerendsen
 from ase.md.nvtberendsen import NVTBerendsen
 from pymatgen.core import Structure
 from pytest import MonkeyPatch, approx
 
 from chgnet import ROOT
+from chgnet.graph import CrystalGraphConverter
 from chgnet.model import StructOptimizer
 from chgnet.model.dynamics import CHGNetCalculator, EquationOfState, MolecularDynamics
 from chgnet.model.model import CHGNet
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 relaxer = StructOptimizer()
-structure = Structure.from_file(f"{ROOT}/examples/o-LiMnO2_unit.cif")
+structure = Structure.from_file(f"{ROOT}/examples/mp-18767-LiMnO2.cif")
 chgnet = CHGNet.load()
 
 
 def test_eos():
     eos = EquationOfState()
     eos.fit(atoms=structure)
-    print(eos.get_bulk_mudulus())
-    print(eos.get_bulk_mudulus(unit="GPa"))
-    print(eos.get_compressibility())
-    print(eos.get_compressibility(unit="GPa^-1"))
-    assert eos.get_bulk_mudulus() == approx(0.6621170816, rel=1e-5)
-    assert eos.get_bulk_mudulus(unit="GPa") == approx(106.08285172, rel=1e-5)
+    assert eos.get_bulk_modulus() == approx(0.6621170816, rel=1e-5)
+    assert eos.get_bulk_modulus(unit="GPa") == approx(106.08285172, rel=1e-5)
     assert eos.get_compressibility() == approx(1.510306904, rel=1e-5)
     assert eos.get_compressibility(unit="GPa^-1") == approx(0.009426594, rel=1e-5)
 
 
-def test_md_nvt(tmp_path: Path, monkeypatch: MonkeyPatch):
-    # cd into the temporary directory
-    monkeypatch.chdir(tmp_path)
+@pytest.mark.parametrize("algorithm", ["legacy", "fast"])
+def test_md_nvt(
+    tmp_path: Path, monkeypatch: MonkeyPatch, algorithm: Literal["legacy", "fast"]
+):
+    monkeypatch.chdir(tmp_path)  # run MD in temporary directory
+
+    chgnet_legacy = CHGNet.load()
+    converter_legacy = CrystalGraphConverter(
+        atom_graph_cutoff=5, bond_graph_cutoff=3, algorithm=algorithm
+    )
+    assert converter_legacy.algorithm == algorithm
+
+    chgnet_legacy.graph_converter = converter_legacy
 
     md = MolecularDynamics(
         atoms=structure,
-        model=chgnet,
+        model=chgnet_legacy,
         ensemble="nvt",
         temperature=1000,  # in k
         timestep=2,  # in fs
         trajectory="md_out.traj",
         logfile="md_out.log",
         loginterval=100,
         use_device="cpu",
@@ -62,34 +70,33 @@
     assert logs == (
         "Time[ps]      Etot[eV]     Epot[eV]     Ekin[eV]    T[K]\n"
         "0.0000         -58.9727     -58.9727       0.0000     0.0\n"
     )
 
 
 def test_md_npt_inhomogeneous_berendsen(tmp_path: Path, monkeypatch: MonkeyPatch):
-    # cd into the temporary directory
-    monkeypatch.chdir(tmp_path)
+    monkeypatch.chdir(tmp_path)  # run MD in temporary directory
 
     md = MolecularDynamics(
         atoms=structure,
         model=chgnet,
         ensemble="npt",
         temperature=1000,  # in k
         timestep=2,  # in fs
+        compressibility_au=1.5103069,
         trajectory="md_out.traj",
         logfile="md_out.log",
         loginterval=100,
     )
     md.run(10)
 
     assert isinstance(md.atoms, Atoms)
     assert isinstance(md.atoms.calc, CHGNetCalculator)
     assert isinstance(md.dyn, Inhomogeneous_NPTBerendsen)
     assert md.dyn.pressure == approx(6.324209e-07, rel=1e-5)
-    assert md.dyn.compressibility == approx(1.5103069, rel=1e-5)
     assert os.path.isfile("md_out.traj")
     assert os.path.isfile("md_out.log")
     with open("md_out.log") as log_file:
         logs = log_file.read()
     assert logs == (
         "Time[ps]      Etot[eV]     Epot[eV]     Ekin[eV]    T[K]\n"
         "0.0000         -58.9727     -58.9727       0.0000     0.0\n"
```

### Comparing `chgnet-0.1.4/tests/test_relaxation.py` & `chgnet-0.2.0/tests/test_relaxation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 from __future__ import annotations
 
+from typing import Literal
+
+import pytest
 import torch
 from pymatgen.core import Structure
 from pytest import approx, mark, param
 
 from chgnet import ROOT
-from chgnet.model import StructOptimizer
+from chgnet.graph import CrystalGraphConverter
+from chgnet.model import CHGNet, StructOptimizer
 
-relaxer = StructOptimizer()
-structure = Structure.from_file(f"{ROOT}/examples/o-LiMnO2_unit.cif")
+structure = Structure.from_file(f"{ROOT}/examples/mp-18767-LiMnO2.cif")
 
 
-def test_relaxation():
-    result = relaxer.relax(structure, verbose=True)
+@pytest.mark.parametrize("algorithm", ["legacy", "fast"])
+def test_relaxation(algorithm: Literal["legacy", "fast"]):
+    chgnet = CHGNet.load()
+    converter = CrystalGraphConverter(
+        atom_graph_cutoff=5, bond_graph_cutoff=3, algorithm=algorithm
+    )
+    assert converter.algorithm == algorithm
 
+    chgnet.graph_converter = converter
+    relaxer = StructOptimizer(model=chgnet)
+    result = relaxer.relax(structure, verbose=True)
     assert list(result) == ["final_structure", "trajectory"]
 
     traj = result["trajectory"]
     # make sure trajectory has expected attributes
-    assert list(traj.__dict__) == [
+    assert {*traj.__dict__} == {
         "atoms",
         "energies",
         "forces",
         "stresses",
         "magmoms",
         "atom_positions",
         "cells",
-    ]
+    }
     assert len(traj) == 4
 
     # make sure final structure is more relaxed than initial one
     assert traj.energies[0] > traj.energies[-1]
-
     assert traj.energies[-1] == approx(-58.972927)
 
 
 no_cuda = mark.skipif(not torch.cuda.is_available(), reason="No CUDA device")
 no_mps = mark.skipif(not hasattr(torch.backends, "mps"), reason="No MPS device")
 
 
@@ -44,8 +54,8 @@
 )
 def test_structure_optimizer_passes_kwargs_to_model(use_device) -> None:
     try:
         relaxer = StructOptimizer(use_device=use_device)
         assert relaxer.calculator.device == use_device
     except NotImplementedError as exc:
         # TODO: remove try/except once mps is supported
-        assert str(exc) == "mps is not supported yet"  # noqa: PT017
+        assert str(exc) == "'mps' backend is not supported yet"  # noqa: PT017
```

### Comparing `chgnet-0.1.4/tests/test_trainer.py` & `chgnet-0.2.0/tests/test_trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,13 +44,11 @@
         epochs=5,
     )
     dir_name = "test_tmp_dir"
     test_dir = tmp_path / dir_name
     trainer.train(train_loader, val_loader, save_dir=test_dir)
     assert test_dir.is_dir(), "Training dir was not created"
 
-    saved_weight = [f for f in test_dir.iterdir() if f.name.startswith("epoch")]
-    best_e_weight = [f for f in test_dir.iterdir() if f.name.startswith("bestE")]
-    best_f_weight = [f for f in test_dir.iterdir() if f.name.startswith("bestF")]
-    assert len(saved_weight) == 1
-    assert len(best_e_weight) == 1
-    assert len(best_f_weight) == 1
+    output_files = list(test_dir.iterdir())
+    for prefix in ("epoch", "bestE", "bestF"):
+        n_matches = sum(file.name.startswith(prefix) for file in output_files)
+        assert n_matches == 1
```

