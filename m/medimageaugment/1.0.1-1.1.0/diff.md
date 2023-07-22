# Comparing `tmp/medimageaugment-1.0.1.tar.gz` & `tmp/medimageaugment-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimageaugment-1.0.1.tar", last modified: Sat Jul 22 05:34:51 2023, max compression
+gzip compressed data, was "medimageaugment-1.1.0.tar", last modified: Sat Jul 22 06:20:21 2023, max compression
```

## Comparing `medimageaugment-1.0.1.tar` & `medimageaugment-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 05:34:51.580158 medimageaugment-1.0.1/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 05:26:51.000000 medimageaugment-1.0.1/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 05:34:51.579577 medimageaugment-1.0.1/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15124 2023-07-22 05:26:40.000000 medimageaugment-1.0.1/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 05:34:51.578259 medimageaugment-1.0.1/medimageaugment.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 05:34:51.580543 medimageaugment-1.0.1/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      996 2023-07-22 05:32:28.000000 medimageaugment-1.0.1/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:20:21.138333 medimageaugment-1.1.0/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 06:19:31.000000 medimageaugment-1.1.0/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:20:21.137699 medimageaugment-1.1.0/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15277 2023-07-22 06:19:55.000000 medimageaugment-1.1.0/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:20:21.136724 medimageaugment-1.1.0/medimageaugment.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:20:21.138599 medimageaugment-1.1.0/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      996 2023-07-22 06:19:47.000000 medimageaugment-1.1.0/setup.py
```

### Comparing `medimageaugment-1.0.1/LICENSE` & `medimageaugment-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.0.1/PKG-INFO` & `medimageaugment-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.0.1/README.md` & `medimageaugment-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 import cv2
 from typing import Optional, Callable, List, Tuple
 from scipy.ndimage import gaussian_filter, map_coordinates, shift, zoom
 from sklearn.model_selection import ParameterGrid
 from skimage.transform import AffineTransform, warp
 from skimage.util import random_noise
 import random
-from skimage.filters.rank import anisotropic_diffusion
+from scipy.sparse import diags
+from scipy.sparse.linalg import spsolve
 
 class MedImageAugment:
     # Class implementation...
 ```
 
 ### Instantiate the `MedImageAugment` class:
 
@@ -337,19 +338,20 @@
       - `pepper_prob` (float): Probability of adding pepper noise.
 
 28. `add_poisson_noise(self, lam: float = 1.)`:
     - Adds Poisson noise augmentation to the list of augmentations.
     - Inputs:
       - `lam` (float): Poisson parameter (mean) for the noise. Defaults to 1.
 
-29. `add_anisotropic_diffusion(self, max_iter=10, sigma=1.0)`:
+29. `add_anisotropic_diffusion(self, max_iter=10, dt=0.1, kappa=50)`:
     - Adds anisotropic diffusion augmentation to the list of augmentations.
     - Inputs:
       - `max_iter` (int): Maximum number of iterations for anisotropic diffusion. Defaults to 10.
-      - `sigma` (float): Conductance parameter for anisotropic diffusion. Defaults to 1.0.
+      - `dt` (float): Time step parameter for anisotropic diffusion. Defaults to 0.1.
+      - `kappa` (float): Conductance parameter for anisotropic diffusion. Larger values reduce diffusion across edges. Defaults to 50.
 
 ## Conclusion
 
 With the `MedImageAugment` class and the ability to generate a parameter grid, you have a powerful tool to augment your 2D and 3D images and perform hyperparameter search to find the best augmentation settings for your particular use case. Experiment with different combinations of augmentations and hyperparameters to optimize the performance of your deep learning models and enhance their generalization capabilities.
 
 ## Note:
 Remember that the module contains both 2D and 3D augmentations. When working with 3D images, ensure that the image dimensions are correct for 3D-specific augmentations. Additionally, this documentation does not include the description of the 'add_random_shear', 'add_random_shift', 'add_random_blur', 'add_motion_blur', 'add_gaussian_noise', 'add_salt_pepper_noise', and 'add_poisson_noise' methods, as their usages are quite similar to other provided augmentations.
```

### Comparing `medimageaugment-1.0.1/medimageaugment.egg-info/PKG-INFO` & `medimageaugment-1.1.0/medimageaugment.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.0.1/setup.py` & `medimageaugment-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medimageaugment',
-    version='1.0.1',
+    version='1.1.0',
     description='A Python class for image augmentation',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/himanalot/medimageaugment',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

