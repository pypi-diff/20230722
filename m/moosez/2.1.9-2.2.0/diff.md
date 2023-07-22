# Comparing `tmp/moosez-2.1.9.tar.gz` & `tmp/moosez-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.1.9.tar", last modified: Mon Jul 10 10:12:47 2023, max compression
+gzip compressed data, was "moosez-2.2.0.tar", last modified: Sat Jul 22 09:05:26 2023, max compression
```

## Comparing `moosez-2.1.9.tar` & `moosez-2.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:12:47.490094 moosez-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 10:12:36.000000 moosez-2.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-10 10:12:47.490094 moosez-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-10 10:12:36.000000 moosez-2.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:12:47.486094 moosez-2.1.9/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:12:47.490094 moosez-2.1.9/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:12:47.490094 moosez-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-10 10:12:36.000000 moosez-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:05:26.737471 moosez-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 09:05:17.000000 moosez-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-22 09:05:26.737471 moosez-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-07-22 09:05:17.000000 moosez-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:05:26.737471 moosez-2.2.0/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-22 09:05:17.000000 moosez-2.2.0/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:05:26.737471 moosez-2.2.0/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-22 09:05:26.000000 moosez-2.2.0/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-22 09:05:26.000000 moosez-2.2.0/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 09:05:26.000000 moosez-2.2.0/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-22 09:05:26.000000 moosez-2.2.0/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-22 09:05:26.000000 moosez-2.2.0/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-22 09:05:26.000000 moosez-2.2.0/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 09:05:26.737471 moosez-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-22 09:05:17.000000 moosez-2.2.0/setup.py
```

### Comparing `moosez-2.1.9/LICENSE` & `moosez-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.1.9/PKG-INFO` & `moosez-2.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.9
+Version: 2.2.0
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
-Author: Lalith Kumar Shiyam Sundar
+Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `moosez-2.1.9/README.md` & `moosez-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Moose-logo](Images/Moose-logo.png)
+![Moose-logo](Images/Moose-logo-new-2.png)
 
 ![](https://komarev.com/ghpvc/?username=QIMP-Team&color=blueviolet&style=for-the-badge)[![image](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PLZQERorVWrbcG4AMkDQ9KrL_Rr77D1-6k) [![image](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/9uTHYhWCA5) [![image](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/qimp/) [![Share on Twitter](https://img.shields.io/badge/Twitter-share%20on%20twitter-blue?logo=twitter&style=for-the-badge)](https://twitter.com/intent/tweet?text=Check%20out%20MOOSE%20(Multi-organ%20objective%20segmentation%20:https://github.com/QIMP-Team/MOOSE)%20a%20data-centric%20AI%20solution%20that%20generates%20multilabel%20organ%20segmentations%20to%20facilitate%20systemic%20TB%20whole-person%20research.) 
 
 
 ## MOOSE 2.0 🫎 - Leaner. Meaner. Stronger 💪
 
 Unveiling a new dimension in 3D medical image segmentation: MOOSE 2.0 🚀
```

### Comparing `moosez-2.1.9/moosez/constants.py` & `moosez-2.2.0/moosez/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from moosez import file_utilities
 
 project_root = file_utilities.get_virtual_env_root()
 
 NNUNET_RESULTS_FOLDER = os.path.join(project_root, 'models', 'nnunet_trained_models')
 MOOSEZ_MODEL_FOLDER = os.path.join(NNUNET_RESULTS_FOLDER, 'nnUNet', '3d_fullres')
-ALLOWED_MODALITIES = ['CT', 'FDG_PT', 'MR']
+ALLOWED_MODALITIES = ['CT', 'PT', 'MR']
 TEMP_FOLDER = 'temp'
 
 # COLOR CODES
 ANSI_ORANGE = '\033[38;5;208m'
 ANSI_GREEN = '\033[38;5;40m'
 ANSI_VIOLET = '\033[38;5;141m'
 ANSI_RESET = '\033[0m'
@@ -40,27 +40,23 @@
 # FOLDER NAMES
 
 SEGMENTATIONS_FOLDER = 'segmentations'
 STATS_FOLDER = 'stats'
 
 # PREPROCESSING PARAMETERS
 
-CLINICAL_VOXEL_SPACING = [1.5, 1.5, 1.5]
-PRECLINICAL_VOXEL_SPACING = [0.15, 0.15, 0.15]
 MATRIX_THRESHOLD = 200 * 200 * 600
 Z_AXIS_THRESHOLD = 200
 MARGIN_PADDING = 20
 INTERPOLATION = 'bspline'
 CHUNK_THRESHOLD = 200
 
-# FILE NAMES PREFIX
+# POSTPROCESSING PARAMETERS
 
-ORGANS_MULTILABEL_PREFIX = 'Organs-Multilabel-'
-LUNGS_MULTILABEL_PREFIX = 'Lungs-Multilabel-'
-MULTILABEL_PREFIX = 'MULTILABEL-'
+TUMOR_LABEL = 12
 
 # FILE NAMES
 
 RESAMPLED_IMAGE_FILE_NAME = 'resampled_image_0000.nii.gz'
 RESAMPLED_MASK_FILE_NAME = 'resampled_mask.nii.gz'
 CHUNK_FILENAMES = ["chunk01_0000.nii.gz", "chunk02_0000.nii.gz", "chunk03_0000.nii.gz"]
 CHUNK_PREFIX = 'chunk'
@@ -89,10 +85,18 @@
     },
     "clin_ct_lungs": {
         1: "lung_upper_lobe_left",
         2: "lung_lower_lobe_left",
         3: "lung_upper_lobe_right",
         4: "lung_middle_lobe_right",
         5: "lung_lower_lobe_right"
+    },
+    "clin_ct_body": {
+        1: "whole-body"
+    },
+    "clin_pt_fdg_tumor": {
+        1: "tumor"
     }
     # More index-to-name dictionaries for other models...
-}
+}
+
+
```

### Comparing `moosez-2.1.9/moosez/display.py` & `moosez-2.2.0/moosez/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # The functions in this module can be imported and used in other modules within the moosez to show predefined display
 # messages.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import logging
 
+import emoji
 import pyfiglet
 
 from moosez import constants
 
 
 def logo():
     """
@@ -51,17 +52,18 @@
         "clin_ct_ribs": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Ribs"},
         "clin_ct_vertebrae": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Vertebral bodies"},
         "clin_ct_muscles": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Muscles"},
         "clin_ct_lungs": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Lungs"},
         "clin_ct_fat": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Fat"},
         "clin_ct_vessels": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Vessels"},
         "clin_ct_organs": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Organs"},
-        "clin_pt_fdg_tumor": {"Imaging": "Clinical", "Modality": "FDG-PET", "Tissue of interest": "Tumor"},
+        "clin_pt_fdg_tumor": {"Imaging": "Clinical", "Modality": "PET", "Tissue of interest": "Tumor"},
         "clin_ct_all": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "All regions"},
         "clin_fdg_pt_ct_all": {"Imaging": "Clinical", "Modality": "FDG-PET-CT", "Tissue of interest": "All regions"},
+        "clin_ct_body": {"Imaging": "Clinical", "Modality": "CT", "Tissue of interest": "Body"},
         "preclin_mr_all": {"Imaging": "Pre-clinical", "Modality": "MR", "Tissue of interest": "All regions"},
     }
 
     if model_name in models:
         model = models[model_name]
         model["Model name"] = model_name
         return model
@@ -71,15 +73,15 @@
 
 
 def citation():
     """
         Display manuscript citation
         :return:
         """
-    print(f"{constants.ANSI_VIOLET} CITATION:{constants.ANSI_RESET}")
+    print(f'{constants.ANSI_VIOLET} {emoji.emojize(":scroll:")} CITATION:{constants.ANSI_RESET}')
     print(" ")
     print(
         " Shiyam Sundar LK, Yu J, Muzik O, et al. Fully-automated, semantic segmentation of whole-body 18F-FDG PET/CT "
         "images based on data-centric artificial intelligence. J Nucl Med. June 2022.")
     print(" Copyright 2022, Quantitative Imaging and Medical Physics Team, Medical University of Vienna")
```

### Comparing `moosez-2.1.9/moosez/download.py` & `moosez-2.2.0/moosez/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez to download the necessary
 # binaries and models for the moosez.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 import requests
+from rich.progress import Progress
 
 from moosez import constants
 from moosez import resources
-from rich.progress import Progress
+
 
 def binary(system_info, url):
     """
     Downloads the binary for the current system.
     :param system_info: A dictionary containing the system information.
     :param url: The url to download the binary from.
     """
@@ -35,16 +36,14 @@
     print("Binary to download: " + binary_name)
     response = requests.get(url + binary_name)
 
     with open(binary_name, "wb") as f:
         f.write(response.content)
 
 
-
-
 def model(model_name, model_path):
     """
     Downloads the model for the current system.
     :param model_name: The name of the model to download.
     :param model_path: The path to store the model.
     """
     model_info = resources.MODELS[model_name]
```

### Comparing `moosez-2.1.9/moosez/file_utilities.py` & `moosez-2.2.0/moosez/file_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # This module contains the functions for performing file operations for the moosez.
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez to perform file operations.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
-import os
 import glob
+import os
 import shutil
 import sys
 from datetime import datetime
 from multiprocessing import Pool
 
 from moosez import constants
 
@@ -98,15 +98,15 @@
     :param modality_tag: The modality tag to be selected.
     :return: The list of selected files.
     """
     selected_files = []
     for subject in moose_compliant_subjects:
         files = os.listdir(subject)
         for file in files:
-            if file.startswith(modality_tag) and file.endswith('.nii') or file.endswith('.nii.gz'):
+            if file.startswith(modality_tag) and (file.endswith('.nii') or file.endswith('.nii.gz')):
                 selected_files.append(os.path.join(subject, file))
     return selected_files
 
 
 def organise_files_by_modality(moose_compliant_subjects: list, modalities: list, moose_dir) -> None:
     """
     Organises the files by modality.
@@ -117,15 +117,15 @@
     for modality in modalities:
         files_to_copy = select_files_by_modality(moose_compliant_subjects, modality)
         copy_files_to_destination(files_to_copy, os.path.join(moose_dir, modality))
 
 
 def find_pet_file(folder):
     # Searching for files with 'PET' in their name and ending with either .nii or .nii.gz
-    pet_files = glob.glob(os.path.join(folder, '*PET*.nii*'))
+    pet_files = glob.glob(os.path.join(folder, 'PET*.nii*')) # Files should start with PET
 
     if len(pet_files) == 1:
         return pet_files[0]
     elif len(pet_files) > 1:
         raise ValueError("More than one PET file found in the directory.")
     else:
         return None
```

### Comparing `moosez-2.1.9/moosez/image_processing.py` & `moosez-2.2.0/moosez/image_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 #
 # Usage:
 # The functions in this module can be imported and used in other modules within the moosez for image processing.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import os
-import numpy as np
-import nibabel
+import dask
 import SimpleITK as sitk
-from moosez.constants import MATRIX_THRESHOLD, Z_AXIS_THRESHOLD, CHUNK_THRESHOLD, MARGIN_PADDING, ORGAN_INDICES, \
-    CHUNK_FILENAMES
 import dask.array as da
-from mpire import WorkerPool
+import nibabel
+import numpy as np
 import pandas as pd
 
+from moosez.constants import MATRIX_THRESHOLD, Z_AXIS_THRESHOLD, CHUNK_THRESHOLD, MARGIN_PADDING, ORGAN_INDICES, \
+    CHUNK_FILENAMES
+
 
 def get_intensity_statistics(image: sitk.Image, mask_image: sitk.Image, model_name: str, out_csv: str) -> None:
     """
     Get the intensity statistics of a NIFTI image file
     :param image: Source image from which the intensity statistics are calculated
     :param mask_image: Multilabel mask image
     :param model_name: Name of the model
@@ -52,63 +53,72 @@
             regions_present.append(organ_indices_dict[label])
         else:
             continue
     stats_df.insert(0, 'Regions-Present', np.array(regions_present))
     stats_df.to_csv(out_csv)
 
 
-def split_and_save(shared_image: tuple, chunk_index: list, image_chunk_path: str) -> None:
+def split_and_save(image_chunk: da.Array, image_affine, image_chunk_path: str) -> None:
     """
-    Split the image into chunks and save each part.
+    Get a chunk of the image and save it.
 
     Args:
-        shared_image: (image_data, image_affine) tuple.
-        chunk_index: List of tuples containing start and end indices for each chunk.
+        image_chunk: Dask array chunk.
+        image_affine: Image affine transformation.
         image_chunk_path: The path to save the image chunk.
     """
-    image_data, image_affine = shared_image
-    chunk_part = nibabel.Nifti1Image(image_data[:, :, chunk_index[0]:chunk_index[1]], image_affine)
+    chunk_part = nibabel.Nifti1Image(image_chunk, image_affine)
     nibabel.save(chunk_part, image_chunk_path)
 
 
-def write_image(image: nibabel.Nifti1Image, out_image_path: str, large_image: bool = False) -> None:
+@dask.delayed
+def delayed_split_and_save(image_chunk, image_affine, image_chunk_path):
+    split_and_save(image_chunk, image_affine, image_chunk_path)
+
+
+def write_image(image: nibabel.Nifti1Image, out_image_path: str, large_image: bool = False, is_label: bool = False) -> None:
     """
     Writes an image either as a single file or multiple files depending on the image size.
 
     Args:
         image: The image to save.
         out_image_path: The path to save the image.
         large_image: Indicates whether the image classifies as large or not.
+        is_label: Indicates whether the image is a label or not.
     """
     image_shape = image.shape
-    image_data = image.get_fdata()
+    image_data = da.from_array(image.get_fdata(), chunks=(image_shape[0], image_shape[1], image_shape[2] // 3))
     image_affine = image.affine
 
     if large_image:
         # Calculate indices for image chunks
         num_chunks = 3
         chunk_size = image_shape[2] // num_chunks
         chunk_indices = [(0, chunk_size + MARGIN_PADDING),
                          (chunk_size + 1 - MARGIN_PADDING, chunk_size * 2 + MARGIN_PADDING),
                          (chunk_size * 2 + 1 - MARGIN_PADDING, None)]
         filenames = CHUNK_FILENAMES
         save_dir = os.path.dirname(out_image_path)
         chunk_paths = [os.path.join(save_dir, filename) for filename in filenames]
 
-        chunk_data = []
-        for chunk_index, chunk_path in zip(chunk_indices, chunk_paths):
-            chunk_data.append({"chunk_index": chunk_index, "image_chunk_path": chunk_path})
+        tasks = []
+        for i, chunk_path in enumerate(chunk_paths):
+            tasks.append(delayed_split_and_save(image_data[:, :, chunk_indices[i][0]:chunk_indices[i][1]].compute(),
+                                                image_affine, chunk_path))
 
-        shared_data = (image_data, image_affine)
+        dask.compute(*tasks)
 
-        with WorkerPool(n_jobs=num_chunks, shared_objects=shared_data) as pool:
-            pool.map(split_and_save, chunk_data)
     else:
-        resampled_image_path = out_image_path
-        nibabel.save(image, resampled_image_path)
+        if is_label:
+            resampled_image_path = out_image_path
+            image_as_uint8 = nibabel.Nifti1Image(image.get_fdata().astype(np.uint8), image.affine)
+            nibabel.save(image_as_uint8, resampled_image_path)
+        else:
+            resampled_image_path = out_image_path
+            nibabel.save(image, resampled_image_path)
 
 
 class NiftiPreprocessor:
     """
     A class for processing NIfTI images using nibabel and SimpleITK.
 
     Attributes:
```

### Comparing `moosez-2.1.9/moosez/input_validation.py` & `moosez-2.2.0/moosez/input_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
           f"{len(subject_paths)} {constants.ANSI_RESET}")
     logging.info(f" Number of moose compliant subjects: {len(moose_compliant_subjects)} out of "
                  f"{len(subject_paths)}")
 
     return moose_compliant_subjects
 
 
-
 def check_file_for_nnunet_compatibility(filename: str, input_dir: str) -> None:
     """
     Checks if the file is nnUNet compatible. If not, compresses the file and renames it to include the required tag.
 
     Parameters:
         filename (str): The name of the file to check.
         input_dir (str): The path to the directory containing the file.
@@ -85,15 +84,14 @@
         os.remove(os.path.join(input_dir, filename))
         if not new_filename.endswith('_0000.nii.gz'):
             # Rename the file to include the required tag
             new_filename_with_zeroes = new_filename.replace('.nii.gz', '_0000.nii.gz')
             os.rename(os.path.join(input_dir, new_filename), os.path.join(input_dir, new_filename_with_zeroes))
 
 
-
 def make_nnunet_compatible(input_dir: str) -> None:
     """
     Checks the files in the specified directory to ensure they comply with the nnUNet requirements. If a file does not
     comply, it is compressed (if it is not already) and renamed to include the required tag.
 
     Parameters:
         input_dir (str): The path to the directory containing the files to check.
```

### Comparing `moosez-2.1.9/moosez/moosez.py` & `moosez-2.2.0/moosez/moosez.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,34 +13,36 @@
 #
 # Usage:
 # The main function in this module is executed when the mooseZ is run.
 #
 # ----------------------------------------------------------------------------------------------------------------------
 
 import argparse
+import glob
 import logging
 import os
-import glob
 import time
+import emoji
 from datetime import datetime
 
 import SimpleITK
 import colorama
 from halo import Halo
 
 from moosez import constants
 from moosez import display
 from moosez import download
 from moosez import file_utilities
 from moosez import image_conversion
+from moosez import image_processing
 from moosez import input_validation
 from moosez import predict
 from moosez import resources
 from moosez.image_processing import ImageResampler
-from moosez import image_processing
+from moosez.resources import MODELS
 
 logging.basicConfig(format='%(asctime)s %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s', level=logging.INFO,
                     filename=datetime.now().strftime('moosez-v.2.0.0.%H-%M-%d-%m-%Y.log'),
                     filemode='w')
 
 
 def main():
@@ -59,14 +61,15 @@
                                  "clin_ct_lungs",
                                  "clin_ct_fat",
                                  "clin_ct_vessels",
                                  "clin_ct_organs",
                                  "clin_pt_fdg_tumor",
                                  "clin_ct_all",
                                  "clin_fdg_pt_ct_all",
+                                 "clin_ct_body",
                                  "preclin_mr_all"], required=True)
     args = parser.parse_args()
 
     parent_folder = os.path.abspath(args.main_directory)
     model_name = args.model_name
 
     display.logo()
@@ -81,36 +84,37 @@
     # ----------------------------------
 
     logging.info(' ')
     logging.info('- Main directory: ' + parent_folder)
     logging.info('- Model name: ' + model_name)
     logging.info(' ')
     print(' ')
-    print(f'{constants.ANSI_VIOLET} NOTE:{constants.ANSI_RESET}')
+    print(f'{constants.ANSI_VIOLET} {emoji.emojize(":memo:")} NOTE:{constants.ANSI_RESET}')
     print(' ')
     modalities = display.expectations(model_name)
     accelerator = resources.check_cuda()
 
     # ----------------------------------
     # DOWNLOADING THE MODEL
     # ----------------------------------
 
     print('')
-    print(f'{constants.ANSI_VIOLET} MODEL DOWNLOAD:{constants.ANSI_RESET}')
+    print(f'{constants.ANSI_VIOLET} {emoji.emojize(":globe_with_meridians:")} MODEL DOWNLOAD:{constants.ANSI_RESET}')
     print('')
     model_path = constants.NNUNET_RESULTS_FOLDER
     file_utilities.create_directory(model_path)
     download.model(model_name, model_path)
 
     # ----------------------------------
     # INPUT STANDARDIZATION
     # ----------------------------------
 
     print('')
-    print(f'{constants.ANSI_VIOLET} STANDARDIZING INPUT DATA TO NIFTI:{constants.ANSI_RESET}')
+    print(
+        f'{constants.ANSI_VIOLET} {emoji.emojize(":magnifying_glass_tilted_left:")} STANDARDIZING INPUT DATA TO NIFTI:{constants.ANSI_RESET}')
     print('')
     logging.info(' ')
     logging.info(' STANDARDIZING INPUT DATA TO NIFTI:')
     logging.info(' ')
     image_conversion.standardize_to_nifti(parent_folder)
     print(f"{constants.ANSI_GREEN} Standardization complete.{constants.ANSI_RESET}")
     logging.info(" Standardization complete.")
@@ -124,84 +128,90 @@
     moose_compliant_subjects = input_validation.select_moose_compliant_subjects(subjects, modalities)
 
     # -------------------------------------------------
     # RUN PREDICTION ONLY FOR MOOSE COMPLIANT SUBJECTS
     # -------------------------------------------------
 
     print('')
-    print(f'{constants.ANSI_VIOLET} PERFORMING PREDICTION:{constants.ANSI_RESET}')
+    print(f'{constants.ANSI_VIOLET} {emoji.emojize(":crystal_ball:")} PREDICT:{constants.ANSI_RESET}')
     print('')
     logging.info(' ')
     logging.info(' PERFORMING PREDICTION:')
     logging.info(' ')
 
     spinner = Halo(text=' Initiating', spinner='dots')
     spinner.start()
     start_total_time = time.time()
-    for subject in moose_compliant_subjects:
+    num_subjects = len(moose_compliant_subjects)
+    for i, subject in enumerate(moose_compliant_subjects):
         # SETTING UP DIRECTORY STRUCTURE
-        spinner.text = f' Setting up directory structure for {os.path.basename(subject)}...'
+        spinner.text = f'[{i + 1}/{num_subjects}] Setting up directory structure for {os.path.basename(subject)}...'
         logging.info(' ')
         logging.info(f'{constants.ANSI_VIOLET} SETTING UP MOOSE-Z DIRECTORY:'
                      f'{constants.ANSI_RESET}')
         logging.info(' ')
         moose_dir, input_dirs, output_dir, stats_dir = file_utilities.moose_folder_structure(subject, model_name,
                                                                                              modalities)
         logging.info(f" MOOSE directory for subject {os.path.basename(subject)} at: {moose_dir}")
 
         # ORGANISE DATA ACCORDING TO MODALITY
-        spinner.text = f' Organising data according to modality for {os.path.basename(subject)}...'
+        spinner.text = f'[{i + 1}/{num_subjects}] Organising data according to modality for {os.path.basename(subject)}...'
         file_utilities.organise_files_by_modality([subject], modalities, moose_dir)
 
         # PREPARE THE DATA FOR PREDICTION
-        spinner.text = f' Preparing data for prediction for {os.path.basename(subject)}...'
+        spinner.text = f'[{i + 1}/{num_subjects}] Preparing data for prediction for {os.path.basename(subject)}...'
         for input_dir in input_dirs:
             input_validation.make_nnunet_compatible(input_dir)
         logging.info(f" {constants.ANSI_GREEN}Data preparation complete using {model_name} for subject "
                      f"{os.path.basename(subject)}{constants.ANSI_RESET}")
 
         # RUN PREDICTION
         start_time = time.time()
         logging.info(' ')
         logging.info(' RUNNING PREDICTION:')
         logging.info(' ')
-        spinner.text = f' Running prediction for {os.path.basename(subject)} using {model_name}...'
+        spinner.text = f'[{i + 1}/{num_subjects}] Running prediction for {os.path.basename(subject)} using {model_name}...'
 
         for input_dir in input_dirs:
             predict.predict(model_name, input_dir, output_dir, accelerator)
         logging.info(f"Prediction complete using {model_name}.")
 
         end_time = time.time()
         elapsed_time = end_time - start_time
-        spinner.text = f' {constants.ANSI_GREEN}Prediction done for {os.path.basename(subject)} using {model_name}!' \
+        spinner.text = f' {constants.ANSI_GREEN}[{i + 1}/{num_subjects}] Prediction done for {os.path.basename(subject)} using {model_name}!' \
                        f' | Elapsed time: {round(elapsed_time / 60, 1)} min{constants.ANSI_RESET}'
         time.sleep(3)
-
+        logging.info(
+            f' {constants.ANSI_GREEN}[{i + 1}/{num_subjects}] Prediction done for {os.path.basename(subject)} using {model_name}!' f' | Elapsed time: {round(elapsed_time / 60, 1)} min{constants.ANSI_RESET}')
         # ----------------------------------
         # EXTRACT PET ACTIVITY
         # ----------------------------------
         pet_file = file_utilities.find_pet_file(subject)
         if pet_file is not None:
             pet_image = SimpleITK.ReadImage(pet_file)
-            spinner.text = f' Extracting PET activity for {os.path.basename(subject)}...'
-            multilabel_file = glob.glob(os.path.join(output_dir, constants.MULTILABEL_PREFIX + '*nii*'))[0]
+            spinner.text = f'[{i + 1}/{num_subjects}] Extracting PET activity for {os.path.basename(subject)}...'
+            multilabel_file = glob.glob(os.path.join(output_dir, MODELS[model_name]["multilabel_prefix"] + '*nii*'))[0]
             multilabel_image = SimpleITK.ReadImage(multilabel_file)
             resampled_multilabel_image = ImageResampler.reslice_identity(reference_image=pet_image,
                                                                          moving_image=multilabel_image,
                                                                          is_label_image=True)
             out_csv = os.path.join(stats_dir, os.path.basename(subject) + '_pet_activity.csv')
             image_processing.get_intensity_statistics(pet_image, resampled_multilabel_image, model_name, out_csv)
-            spinner.text = f'{constants.ANSI_GREEN} PET activity extracted for {os.path.basename(subject)}! ' \
+            spinner.text = f'{constants.ANSI_GREEN} [{i + 1}/{num_subjects}] PET activity extracted for {os.path.basename(subject)}! ' \
                            f'{constants.ANSI_RESET}'
             time.sleep(3)
 
     end_total_time = time.time()
     total_elapsed_time = (end_total_time - start_total_time) / 60
     time_per_dataset = total_elapsed_time / len(moose_compliant_subjects)
 
     spinner.succeed(f'{constants.ANSI_GREEN} All predictions done! | Total elapsed time for '
                     f'{len(moose_compliant_subjects)} datasets: {round(total_elapsed_time, 1)} min'
                     f' | Time per dataset: {round(time_per_dataset, 2)} min {constants.ANSI_RESET}')
 
 
+def moose(model_name: str, input_dir: str, output_dir: str, accelerator: str):
+    predict.predict(model_name, input_dir, output_dir, accelerator)
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `moosez-2.1.9/moosez/predict.py` & `moosez-2.2.0/moosez/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 # ----------------------------------------------------------------------------------------------------------------------
 
 import glob
 import os
 import shutil
 import subprocess
 
-import SimpleITK
 import nibabel as nib
 import numpy as np
 from halo import Halo
 from mpire import WorkerPool
+
 from moosez import constants
 from moosez import file_utilities
 from moosez import image_processing
-from moosez.image_processing import NiftiPreprocessor
 from moosez.image_processing import ImageResampler
+from moosez.image_processing import NiftiPreprocessor
+from moosez.resources import MODELS
 
 
 def map_model_name_to_task_number(model_name: str):
     """
     Maps the model name to the task number.
     :param model_name: The name of the model.
     :return: The task number.
@@ -52,21 +53,23 @@
     elif model_name == "clin_ct_fat":
         return 206
     elif model_name == "clin_ct_vessels":
         return 207
     elif model_name == "clin_ct_organs":
         return 123
     elif model_name == "clin_pt_fdg_tumor":
-        return 209
+        return 789
     elif model_name == "clin_ct_all":
         return 210
     elif model_name == "clin_fdg_pt_ct_all":
         return 211
     elif model_name == "preclin_mr_all":
         return 234
+    elif model_name == "clin_ct_body":
+        return 696
     else:
         raise Exception(f"Error: The model name '{model_name}' is not valid.")
 
 
 def predict(model_name: str, input_dir: str, output_dir: str, accelerator: str):
     """
     Runs the prediction using nnunet_predict.
@@ -81,16 +84,16 @@
     os.environ["nnUNet_results"] = constants.NNUNET_RESULTS_FOLDER
 
     # Preprocess the image
     temp_input_dir, resampled_image, moose_image_object = preprocess(input_dir, model_name)
     resampled_image_shape = resampled_image.shape
     resampled_image_affine = resampled_image.affine
 
-    # Check if the model is a clinical model or preclinical model
-    trainer = 'nnUNetTrainer_2000epochs_NoMirroring' if model_name.startswith('clin') else 'nnUNetTrainerNoMirroring'
+    # choose the appropriate trainer for the model
+    trainer = MODELS[model_name]["trainer"]
 
     # Construct the command
     command = f'nnUNetv2_predict -i {temp_input_dir} -o {output_dir} -d {task_number} -c 3d_fullres' \
               f' -f all -tr {trainer} --disable_tta -device {accelerator}'
 
     # Run the command
     subprocess.run(command, shell=True, stdout=subprocess.DEVNULL, env=os.environ)
@@ -98,15 +101,15 @@
     original_image_files = file_utilities.get_files(input_dir, '.nii.gz')
 
     # Postprocess the label
     # if temp_input_dir has more than one nifti file, run logic below
 
     if len(file_utilities.get_files(output_dir, '.nii.gz')) > 1:
         merge_image_parts(output_dir, resampled_image_shape, resampled_image_affine)
-    postprocess(original_image_files[0], output_dir)
+    postprocess(original_image_files[0], output_dir, model_name)
 
     shutil.rmtree(temp_input_dir)
 
 
 def preprocess(original_image_directory: str, model_name: str):
     """
     Preprocesses the original images.
@@ -116,43 +119,59 @@
     """
     # create the temp directory
     temp_folder = os.path.join(original_image_directory, constants.TEMP_FOLDER)
     os.makedirs(temp_folder, exist_ok=True)
     original_image_files = file_utilities.get_files(original_image_directory, '.nii.gz')
     org_image = nib.load(original_image_files[0])
     moose_image_object = NiftiPreprocessor(org_image)
-    # check if the model is a clinical model or preclinical model
-    desired_spacing = constants.CLINICAL_VOXEL_SPACING if model_name.startswith(
-        'clin') else constants.PRECLINICAL_VOXEL_SPACING
+
+    # choose the target spacing for the model to enable preprocessing
+    desired_spacing = MODELS[model_name]["voxel_spacing"]
 
     resampled_image = ImageResampler.resample_image(moose_img_object=moose_image_object,
                                                     interpolation=constants.INTERPOLATION,
                                                     desired_spacing=desired_spacing)
-    image_processing.write_image(resampled_image, os.path.join(temp_folder, constants.RESAMPLED_IMAGE_FILE_NAME),
-                                 moose_image_object.is_large)
+    # if model name has tumor in it, run logic below
+    if "tumor" in model_name:
+        image_processing.write_image(resampled_image, os.path.join(temp_folder, constants.RESAMPLED_IMAGE_FILE_NAME),
+                                     False, False)
+    else:
+        image_processing.write_image(resampled_image, os.path.join(temp_folder, constants.RESAMPLED_IMAGE_FILE_NAME),
+                                     moose_image_object.is_large, False)
     return temp_folder, resampled_image, moose_image_object
 
 
-def postprocess(original_image, output_dir):
+def postprocess(original_image, output_dir, model_name):
     """
     Postprocesses the predicted images.
     :param original_image: The path to the original image.
     :param output_dir: The output directory containing the label image.
+    :param model_name: The name of the model.
     :return: None
     """
     # [1] Resample the predicted image to the original image's voxel spacing
     predicted_image = file_utilities.get_files(output_dir, '.nii.gz')[0]
-    multilabel_image = os.path.join(output_dir, constants.MULTILABEL_PREFIX + os.path.basename(original_image))
     original_header = nib.load(original_image).header
     native_spacing = original_header.get_zooms()
     native_size = original_header.get_data_shape()
     resampled_prediction = ImageResampler.resample_segmentations(input_image_path=predicted_image,
                                                                  desired_spacing=native_spacing,
                                                                  desired_size=native_size)
-    image_processing.write_image(resampled_prediction, multilabel_image, False)
+    multilabel_image = os.path.join(output_dir, MODELS[model_name]["multilabel_prefix"] +
+                                    os.path.basename(original_image))
+    # if model_name has tumor in it, run logic below
+    if "tumor" in model_name:
+        resampled_prediction_data = resampled_prediction.get_fdata()
+        resampled_prediction_data[resampled_prediction_data != constants.TUMOR_LABEL] = 0
+        resampled_prediction_data[resampled_prediction_data == constants.TUMOR_LABEL] = 1
+        resampled_prediction_new = nib.Nifti1Image(resampled_prediction_data, resampled_prediction.affine,
+                                                   resampled_prediction.header)
+        image_processing.write_image(resampled_prediction_new, multilabel_image, False, True)
+    else:
+        image_processing.write_image(resampled_prediction, multilabel_image, False, True)
     os.remove(predicted_image)
 
 
 def count_output_files(output_dir):
     """
     Counts the number of files in the specified output directory.
     Parameters:
@@ -275,15 +294,15 @@
         os.path.join(save_dir, predicted_chunk_filenames[2])).get_fdata()[
                                                   :, :, constants.MARGIN_PADDING - 1:]
 
     # Create a new Nifti1Image with the merged data and the original image's affine transformation
     merged_image = nib.Nifti1Image(merged_image_data, original_image_affine)
 
     # remove the split image parts
-    files_to_remove = glob.glob(os.path.join(save_dir, constants.CHUNK_PREFIX+"*"))
+    files_to_remove = glob.glob(os.path.join(save_dir, constants.CHUNK_PREFIX + "*"))
     for file in files_to_remove:
         os.remove(file)
 
     # write the merged image to disk
     merged_image_path = os.path.join(save_dir, constants.RESAMPLED_IMAGE_FILE_NAME)
     nib.save(merged_image, merged_image_path)
```

### Comparing `moosez-2.1.9/moosez.egg-info/PKG-INFO` & `moosez-2.2.0/moosez.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.9
+Version: 2.2.0
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
-Author: Lalith Kumar Shiyam Sundar
+Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `moosez-2.1.9/setup.py` & `moosez-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from setuptools import setup, find_packages
 
-
 setup(
     name='moosez',
-    version='2.1.9',
-    author='Lalith Kumar Shiyam Sundar',
+    version='2.2.0',
+    author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
                      'reliable tool for medical imaging applications.',
@@ -36,26 +35,27 @@
         'nibabel~=3.2.2',
         'halo~=0.0.31',
         'pandas~=1.4.1',
         'SimpleITK~=2.2.1',
         'pydicom~=2.2.2',
         'argparse~=1.4.0',
         'imageio~=2.16.1',
-        'numpy~=1.22.3',
+        'numpy',
         'mpire~=2.3.3',
         'openpyxl~=3.0.9',
         'matplotlib',
         'pyfiglet~=0.8.post1',
         'natsort~=8.1.0',
         'pillow>=9.2.0',
         'colorama~=0.4.6',
-        'dask~=2023.6.0',
+        'dask',
         'rich',
         'pandas',
-        'dcm2niix'
+        'dicom2nifti~=2.4.8',
+        'emoji',
     ],
     entry_points={
         'console_scripts': [
             'moosez=moosez.moosez:main',
         ],
     },
 )
```

