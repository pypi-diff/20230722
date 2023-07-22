# Comparing `tmp/medimageaugment-1.2.0.tar.gz` & `tmp/medimageaugment-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimageaugment-1.2.0.tar", last modified: Sat Jul 22 06:45:36 2023, max compression
+gzip compressed data, was "medimageaugment-1.2.1.tar", last modified: Sat Jul 22 06:54:43 2023, max compression
```

## Comparing `medimageaugment-1.2.0.tar` & `medimageaugment-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:45:36.049198 medimageaugment-1.2.0/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 06:45:25.000000 medimageaugment-1.2.0/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:45:36.048135 medimageaugment-1.2.0/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15277 2023-07-22 06:45:00.000000 medimageaugment-1.2.0/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:45:36.047217 medimageaugment-1.2.0/medimageaugment.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:45:35.000000 medimageaugment-1.2.0/medimageaugment.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 06:45:35.000000 medimageaugment-1.2.0/medimageaugment.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:45:35.000000 medimageaugment-1.2.0/medimageaugment.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:45:35.000000 medimageaugment-1.2.0/medimageaugment.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:45:35.000000 medimageaugment-1.2.0/medimageaugment.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:45:36.049666 medimageaugment-1.2.0/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      996 2023-07-22 06:45:13.000000 medimageaugment-1.2.0/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:54:43.697354 medimageaugment-1.2.1/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 06:45:25.000000 medimageaugment-1.2.1/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:54:43.696391 medimageaugment-1.2.1/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14911 2023-07-22 06:53:59.000000 medimageaugment-1.2.1/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:54:43.694018 medimageaugment-1.2.1/medimageaugment.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:54:43.697779 medimageaugment-1.2.1/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      996 2023-07-22 06:54:40.000000 medimageaugment-1.2.1/setup.py
```

### Comparing `medimageaugment-1.2.0/LICENSE` & `medimageaugment-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.2.0/PKG-INFO` & `medimageaugment-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.2.0/README.md` & `medimageaugment-1.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,42 +16,30 @@
 
 ```bash
 pip install numpy opencv-python scipy scikit-image scikit-learn
 ```
 
 ## Usage
 
-### Import the module and create an instance of MedImageAugment:
+### Import the module and create an instance of ImageAugment:
 
 ```python
-import numpy as np
-import cv2
-from typing import Optional, Callable, List, Tuple
-from scipy.ndimage import gaussian_filter, map_coordinates, shift, zoom
-from sklearn.model_selection import ParameterGrid
-from skimage.transform import AffineTransform, warp
-from skimage.util import random_noise
-import random
-from scipy.sparse import diags
-from scipy.sparse.linalg import spsolve
-
-class MedImageAugment:
-    # Class implementation...
+from MedImageAugment.MedImageAugment import ImageAugment
 ```
 
-### Instantiate the `MedImageAugment` class:
+### Instantiate the `ImageAugment` class:
 
 ```python
-augmenter = MedImageAugment(seed=42, modality='MRI', random_rotation_3d=True, random_scaling_3d=True,
+augmenter = ImageAugment(seed=42, modality='MRI', random_rotation_3d=True, random_scaling_3d=True,
                          random_crop_3d=True, random_horizontal_flip_3d=True, random_vertical_flip_3d=True)
 ```
 
 ### Add augmentations:
 
-You can add specific augmentations to the `MedImageAugment` instance using the provided methods. For example:
+You can add specific augmentations to the `ImageAugment` instance using the provided methods. For example:
 
 ```python
 # Add some augmentations
 augmenter.add_random_brightness(max_delta=30)
 augmenter.add_random_contrast(lower=0.7, upper=1.3)
 augmenter.add_elastic_deformation(alpha=9, sigma=0.7)
 augmenter.add_speckle_noise(mean=0, std=10)
@@ -83,35 +71,36 @@
 
 # Augment the batch of images
 augmented_images = augmenter.augment_batch(images)
 ```
 
 ### Modality-specific augmentations:
 
-The module provides modality-specific augmentations for different medical imaging modalities, such as 'CT', 'X-ray', 'MRI', and 'Ultrasound'. When creating the `MedImageAugment` instance, you can specify the modality, and the augmentations will be automatically set accordingly.
+The module provides modality-specific augmentations for different medical imaging modalities, such as 'CT', 'X-ray', 'MRI', and 'Ultrasound'. When creating the `ImageAugment` instance, you can specify the modality, and the augmentations will be automatically set accordingly.
 
 ### Additional Notes:
 
 - Each augmentation function performs a specific image transformation.
-- You can add multiple augmentations to the `MedImageAugment` instance to apply them sequentially.
+- You can add multiple augmentations to the `ImageAugment` instance to apply them sequentially.
 - The augmentations are randomly shuffled before applying to introduce diversity.
-- Some augmentations support 3D images, but make sure to set the corresponding parameters when creating the `MedImageAugment` instance.
+- Some augmentations support 3D images, but make sure to set the corresponding parameters when creating the `ImageAugment` instance.
 
 ## Example:
-Here's an example of using the `MedImageAugment` class to augment a single 2D image:
+Here's an example of using the `ImageAugment` class to augment a single 2D image:
 
 ```python
 import cv2
+from MedImageAugment.MedImageAugment import ImageAugment
 
 # Load an image
 image_path = "path_to_your_image.png"
 image = cv2.imread(image_path, cv2.IMREAD_GRAYSCALE)
 
-# Instantiate the MedImageAugment class
-augmenter = MedImageAugment(seed=42, modality='X-ray')
+# Instantiate the ImageAugment class
+augmenter = ImageAugment(seed=42, modality='X-ray')
 
 # Add some augmentations
 augmenter.add_random_brightness(max_delta=30)
 augmenter.add_random_contrast(lower=0.7, upper=1.3)
 augmenter.add_speckle_noise(mean=0, std=10)
 augmenter.add_random_horizontal_flip()
 
@@ -123,20 +112,20 @@
 cv2.imshow("Augmented Image", augmented_image)
 cv2.waitKey(0)
 cv2.destroyAllWindows()
 ```
 
 ## Adding ParameterGrid for Hyperparameter Search
 
-In some cases, you may want to perform hyperparameter search to find the best combination of augmentation parameters for your specific use case. To facilitate this, you can add a method to the `MedImageAugment` class that generates a parameter grid containing all possible combinations of the augmentation parameters. Here's how you can do it:
+In some cases, you may want to perform hyperparameter search to find the best combination of augmentation parameters for your specific use case. To facilitate this, you can add a method to the `ImageAugment` class that generates a parameter grid containing all possible combinations of the augmentation parameters. Here's how you can do it:
 
 ```python
 from itertools import product
 
-class MedImageAugment:
+class ImageAugment:
     # Previous class implementation...
 
     def generate_parameter_grid(self) -> List[dict]:
         """Generate a parameter grid for hyperparameter search.
 
         Returns:
             List[dict]: A list of dictionaries representing all possible combinations of augmentation parameters.
@@ -161,20 +150,20 @@
 
         return param_grid
 ```
 
 Now, you can use this method to generate the parameter grid and then loop through all the combinations to evaluate the performance of your model with different augmentations during hyperparameter search.
 
 ```python
-augmenter = MedImageAugment(seed=42, modality='X-ray')
+augmenter = ImageAugment(seed=42, modality='X-ray')
 param_grid = augmenter.generate_parameter_grid()
 
 for params in param_grid:
-    # Instantiate the MedImageAugment class with specific parameters
-    augmenter = MedImageAugment(seed=42, modality='X-ray', random_rotation_3d=True, random_scaling_3d=True,
+    # Instantiate the ImageAugment class with specific parameters
+    augmenter = ImageAugment(seed=42, modality='X-ray', random_rotation_3d=True, random_scaling_3d=True,
                              random_crop_3d=True, random_horizontal_flip_3d=True, random_vertical_flip_3d=True)
     
     # Add augmentations with the specific hyperparameters
     augmenter.add_random_rotation_3d(max_angle=params['max_angle'])
     augmenter.add_random_scaling_3d(scale_range=params['scale_range'])
     augmenter.add_random_crop_3d(crop_size=params['crop_size'])
 
@@ -347,15 +336,15 @@
     - Inputs:
       - `max_iter` (int): Maximum number of iterations for anisotropic diffusion. Defaults to 10.
       - `dt` (float): Time step parameter for anisotropic diffusion. Defaults to 0.1.
       - `kappa` (float): Conductance parameter for anisotropic diffusion. Larger values reduce diffusion across edges. Defaults to 50.
 
 ## Conclusion
 
-With the `MedImageAugment` class and the ability to generate a parameter grid, you have a powerful tool to augment your 2D and 3D images and perform hyperparameter search to find the best augmentation settings for your particular use case. Experiment with different combinations of augmentations and hyperparameters to optimize the performance of your deep learning models and enhance their generalization capabilities.
+With the `ImageAugment` class and the ability to generate a parameter grid, you have a powerful tool to augment your 2D and 3D images and perform hyperparameter search to find the best augmentation settings for your particular use case. Experiment with different combinations of augmentations and hyperparameters to optimize the performance of your deep learning models and enhance their generalization capabilities.
 
 ## Note:
 Remember that the module contains both 2D and 3D augmentations. When working with 3D images, ensure that the image dimensions are correct for 3D-specific augmentations. Additionally, this documentation does not include the description of the 'add_random_shear', 'add_random_shift', 'add_random_blur', 'add_motion_blur', 'add_gaussian_noise', 'add_salt_pepper_noise', and 'add_poisson_noise' methods, as their usages are quite similar to other provided augmentations.
 
 Feel free to experiment with different combinations of augmentations to suit your specific needs and data.
 
 ## License
```

### Comparing `medimageaugment-1.2.0/medimageaugment.egg-info/PKG-INFO` & `medimageaugment-1.2.1/medimageaugment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.2.0/setup.py` & `medimageaugment-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medimageaugment',
-    version='1.2.0',
+    version='1.2.1',
     description='A Python class for image augmentation',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/himanalot/medimageaugment',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

