# Comparing `tmp/gp2-0.5.25.23.tar.gz` & `tmp/gp2-0.7.22.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2-0.5.25.23.tar", last modified: Fri May 19 02:26:08 2023, max compression
+gzip compressed data, was "gp2-0.7.22.23.tar", last modified: Sat Jul 22 14:20:56 2023, max compression
```

## Comparing `gp2-0.5.25.23.tar` & `gp2-0.7.22.23.tar`

### file list

```diff
@@ -1,45 +1,53 @@
-drwxr-xr-x   0  1981811  1981811        0 2023-05-19 02:18:58.000000 gp2-0.5.25.23/
--rw-rw-r--   0  1981811  1981811     1068 2023-05-03 06:05:46.000000 gp2-0.5.25.23/LICENSE
--rw-r--r--   0  1981811  1981811      630 2023-05-19 02:18:58.000000 gp2-0.5.25.23/PKG-INFO
--rw-rw-r--   0  1981811  1981811     3677 2023-05-03 06:16:48.000000 gp2-0.5.25.23/README.md
-drwxr-xr-x   0  1981811  1981811        0 2023-05-19 02:18:21.000000 gp2-0.5.25.23/gp2/
--rw-rw-r--   0  1981811  1981811       91 2023-05-18 21:13:26.000000 gp2-0.5.25.23/gp2/__init__.py
--rw-r--r--   0  1981811  1981811       53 2023-05-19 02:16:24.000000 gp2-0.5.25.23/gp2/__version__.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-19 02:18:32.000000 gp2-0.5.25.23/gp2/data/
--rw-rw-r--   0  1981811  1981811       89 2023-05-18 21:21:25.000000 gp2-0.5.25.23/gp2/data/__init__.py
--rw-rw-r--   0  1981811  1981811     3004 2023-05-19 00:50:31.000000 gp2-0.5.25.23/gp2/data/collection.py
--rw-rw-r--   0  1981811  1981811     5051 2023-05-03 06:31:35.000000 gp2-0.5.25.23/gp2/data/manager.py
--rw-rw-r--   0  1981811  1981811      296 2023-05-03 06:25:06.000000 gp2-0.5.25.23/gp2/data/point.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-19 02:18:35.000000 gp2-0.5.25.23/gp2/gp2/
--rw-rw-r--   0  1981811  1981811      118 2023-05-03 03:30:40.000000 gp2-0.5.25.23/gp2/gp2/__init__.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-19 02:18:51.000000 gp2-0.5.25.23/gp2/gp2/classifiers/
--rw-rw-r--   0  1981811  1981811      458 2023-05-18 21:21:50.000000 gp2-0.5.25.23/gp2/gp2/classifiers/__init__.py
--rw-rw-r--   0  1981811  1981811     3954 2023-05-19 01:14:46.000000 gp2-0.5.25.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py
--rw-rw-r--   0  1981811  1981811      829 2023-05-03 03:30:40.000000 gp2-0.5.25.23/gp2/gp2/classifiers/classifier.py
--rw-rw-r--   0  1981811  1981811     7140 2023-05-19 00:58:17.000000 gp2-0.5.25.23/gp2/gp2/classifiers/k_att_unet2d.py
--rw-rw-r--   0  1981811  1981811     5030 2023-05-19 00:58:55.000000 gp2-0.5.25.23/gp2/gp2/classifiers/k_r2_unet2d.py
--rw-rw-r--   0  1981811  1981811     5808 2023-05-19 00:59:46.000000 gp2-0.5.25.23/gp2/gp2/classifiers/k_res_unet2d.py
--rw-rw-r--   0  1981811  1981811     5586 2023-05-19 01:04:40.000000 gp2-0.5.25.23/gp2/gp2/classifiers/k_unet.py
--rw-rw-r--   0  1981811  1981811     6371 2023-05-19 01:05:30.000000 gp2-0.5.25.23/gp2/gp2/classifiers/k_unet2d.py
--rw-rw-r--   0  1981811  1981811     8266 2023-05-19 01:06:51.000000 gp2-0.5.25.23/gp2/gp2/classifiers/k_unet3_plus2d.py
--rw-rw-r--   0  1981811  1981811     6710 2023-05-19 01:08:28.000000 gp2-0.5.25.23/gp2/gp2/classifiers/k_unet_plus2d.py
--rw-rw-r--   0  1981811  1981811     5148 2023-05-19 01:10:48.000000 gp2-0.5.25.23/gp2/gp2/classifiers/k_vnet2d.py
--rw-rw-r--   0  1981811  1981811    10236 2023-05-19 00:56:09.000000 gp2-0.5.25.23/gp2/gp2/classifiers/unet.py
--rw-rw-r--   0  1981811  1981811     6248 2023-05-03 03:30:40.000000 gp2-0.5.25.23/gp2/gp2/classifiers/unet_plus.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-19 02:18:57.000000 gp2-0.5.25.23/gp2/gp2/discriminators/
--rw-rw-r--   0  1981811  1981811      206 2023-05-18 21:22:00.000000 gp2-0.5.25.23/gp2/gp2/discriminators/__init__.py
--rw-rw-r--   0  1981811  1981811     4430 2023-05-03 03:30:40.000000 gp2-0.5.25.23/gp2/gp2/discriminators/base_cnn_discriminator.py
--rw-rw-r--   0  1981811  1981811     4787 2023-05-19 01:29:10.000000 gp2-0.5.25.23/gp2/gp2/discriminators/cnn_discriminator_plus.py
--rw-rw-r--   0  1981811  1981811     6170 2023-05-19 01:24:00.000000 gp2-0.5.25.23/gp2/gp2/discriminators/cnndiscriminator.py
--rw-rw-r--   0  1981811  1981811      505 2023-05-03 03:30:40.000000 gp2-0.5.25.23/gp2/gp2/discriminators/discriminator.py
--rw-rw-r--   0  1981811  1981811     8120 2023-05-19 02:13:05.000000 gp2-0.5.25.23/gp2/gp2/util.py
--rw-rw-r--   0  1981811  1981811    29218 2023-05-19 00:49:41.000000 gp2-0.5.25.23/gp2/runner.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-19 02:18:26.000000 gp2-0.5.25.23/gp2.egg-info/
--rw-r--r--   0  1981811  1981811      630 2023-05-19 02:18:09.000000 gp2-0.5.25.23/gp2.egg-info/PKG-INFO
--rw-r--r--   0  1981811  1981811     1019 2023-05-19 02:18:13.000000 gp2-0.5.25.23/gp2.egg-info/SOURCES.txt
--rw-r--r--   0  1981811  1981811        1 2023-05-19 02:18:09.000000 gp2-0.5.25.23/gp2.egg-info/dependency_links.txt
--rw-r--r--   0  1981811  1981811       97 2023-05-19 02:18:10.000000 gp2-0.5.25.23/gp2.egg-info/requires.txt
--rw-r--r--   0  1981811  1981811        4 2023-05-19 02:18:10.000000 gp2-0.5.25.23/gp2.egg-info/top_level.txt
--rw-r--r--   0  1981811  1981811      141 2023-05-18 21:33:10.000000 gp2-0.5.25.23/pyproject.toml
--rw-r--r--   0  1981811  1981811       38 2023-05-19 02:18:58.000000 gp2-0.5.25.23/setup.cfg
--rw-r--r--   0  1981811  1981811      993 2023-05-18 21:44:28.000000 gp2-0.5.25.23/setup.py
+drwxr-xr-x   0 ryazur    (1000) ryazur    (1000)        0 2023-07-22 14:20:56.307762 gp2-0.7.22.23/
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     1089 2023-07-01 15:12:55.000000 gp2-0.7.22.23/LICENSE
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      675 2023-07-22 14:20:56.307762 gp2-0.7.22.23/PKG-INFO
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     5653 2023-07-01 15:12:55.000000 gp2-0.7.22.23/README.md
+drwxr-xr-x   0 ryazur    (1000) ryazur    (1000)        0 2023-07-22 14:20:56.297762 gp2-0.7.22.23/deepsight/
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)       39 2023-07-01 15:12:55.000000 gp2-0.7.22.23/deepsight/__init__.py
+drwxr-xr-x   0 ryazur    (1000) ryazur    (1000)        0 2023-07-22 14:20:56.297762 gp2-0.7.22.23/deepsight/kaggle_explorer/
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)       96 2023-07-01 15:12:55.000000 gp2-0.7.22.23/deepsight/kaggle_explorer/__init__.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     6418 2023-07-01 15:12:55.000000 gp2-0.7.22.23/deepsight/kaggle_explorer/dicom_copy_machine.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     7177 2023-07-01 15:12:55.000000 gp2-0.7.22.23/deepsight/kaggle_explorer/dicom_data_fixer.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)    36265 2023-07-01 15:12:55.000000 gp2-0.7.22.23/deepsight/kaggle_sight.py
+drwxr-xr-x   0 ryazur    (1000) ryazur    (1000)        0 2023-07-22 14:20:56.297762 gp2-0.7.22.23/gp2/
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      154 2023-07-22 14:17:06.000000 gp2-0.7.22.23/gp2/__init__.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)       53 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/__version__.py
+drwxr-xr-x   0 ryazur    (1000) ryazur    (1000)        0 2023-07-22 14:20:56.297762 gp2-0.7.22.23/gp2/data/
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)       92 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/data/__init__.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     3143 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/data/collection.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     5097 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/data/data_converter.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     5228 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/data/manager.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      312 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/data/point.py
+drwxr-xr-x   0 ryazur    (1000) ryazur    (1000)        0 2023-07-22 14:20:56.297762 gp2-0.7.22.23/gp2/gp2/
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      118 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/gp2/__init__.py
+drwxr-xr-x   0 ryazur    (1000) ryazur    (1000)        0 2023-07-22 14:20:56.297762 gp2-0.7.22.23/gp2/gp2/classifiers/
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      458 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/gp2/classifiers/__init__.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     3954 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      851 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/classifier.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     7131 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/k_att_unet2d.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     5030 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/k_r2_unet2d.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     5813 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/k_res_unet2d.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     5591 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/k_unet.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     6374 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/k_unet2d.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     8269 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/k_unet3_plus2d.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     6717 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/k_unet_plus2d.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     5151 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/k_vnet2d.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)    10509 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/unet.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     6217 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/classifiers/unet_plus.py
+drwxr-xr-x   0 ryazur    (1000) ryazur    (1000)        0 2023-07-22 14:20:56.307762 gp2-0.7.22.23/gp2/gp2/discriminators/
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      206 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/gp2/discriminators/__init__.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     4430 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/gp2/discriminators/base_cnn_discriminator.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     4787 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/gp2/discriminators/cnn_discriminator_plus.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     6336 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/gp2/discriminators/cnndiscriminator.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      513 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/gp2/discriminators/discriminator.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     8392 2023-07-01 15:12:55.000000 gp2-0.7.22.23/gp2/gp2/util.py
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)    32760 2023-07-22 13:37:35.000000 gp2-0.7.22.23/gp2/runner.py
+drwxr-xr-x   0 ryazur    (1000) ryazur    (1000)        0 2023-07-22 14:20:56.297762 gp2-0.7.22.23/gp2.egg-info/
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      675 2023-07-22 14:20:56.000000 gp2-0.7.22.23/gp2.egg-info/PKG-INFO
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)     1226 2023-07-22 14:20:56.000000 gp2-0.7.22.23/gp2.egg-info/SOURCES.txt
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)        1 2023-07-22 14:20:56.000000 gp2-0.7.22.23/gp2.egg-info/dependency_links.txt
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)       97 2023-07-22 14:20:56.000000 gp2-0.7.22.23/gp2.egg-info/requires.txt
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)       14 2023-07-22 14:20:56.000000 gp2-0.7.22.23/gp2.egg-info/top_level.txt
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      141 2023-07-01 15:12:55.000000 gp2-0.7.22.23/pyproject.toml
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)       38 2023-07-22 14:20:56.307762 gp2-0.7.22.23/setup.cfg
+-rw-r--r--   0 ryazur    (1000) ryazur    (1000)      981 2023-07-22 14:08:19.000000 gp2-0.7.22.23/setup.py
```

### Comparing `gp2-0.5.25.23/LICENSE` & `gp2-0.7.22.23/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ryan Zurrin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Ryan Zurrin
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
```

### Comparing `gp2-0.5.25.23/gp2/data/manager.py` & `gp2-0.7.22.23/gp2/data/manager.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-from .collection import Collection
-from .point import Point
-
-import pickle
-
-
-class Manager:
-    """ A class to manage collections of data."""
-
-    def __init__(self):
-        """ Initialize the manager."""
-        self.collections = {}
-        self.names = {}
-
-    def register(self, collection, name=None):
-        """ Register a collection with the manager.
-        Parameters
-        ----------
-        collection : Collection
-            The collection to register.
-        name : str
-            The name to register the collection with.
-        """
-        # here we need to remove the old collection
-        if name:
-            for c in self.names:
-                if self.names[c] == name:
-                    old_collection_id = c
-                    del self.collections[old_collection_id]
-                    del self.names[c]
-                    # print('Unregistered stale collection:', name)
-                    break
-
-        # register this collection + name if given
-        self.collections[collection.id] = collection
-
-        if name:
-            self.names[collection.id] = name
-
-    def get(self, name):
-        """ Get a collection by name.
-        Parameters
-        ----------
-        name : str
-            The name of the collection to get.
-        Returns
-        -------
-        Collection
-            The collection with the given name.
-        """
-        # get name
-        for c in self.names:
-            if self.names[c] == name:
-                return self.collections[c]
-
-    @staticmethod
-    def add(collection, datapoint):
-        """ Add a datapoint to a collection.
-        Parameters
-        ----------
-        collection : Collection
-            The collection to add the datapoint to.
-        datapoint : Point
-            The datapoint to add.
-        Returns
-        -------
-        Collection
-            The collection with the added datapoint.
-        """
-        collection.add(datapoint)
-        return collection
-
-    @staticmethod
-    def remove(collection, datapoint):
-        """ Remove a datapoint from a collection.
-        Parameters
-        ----------
-        collection : Collection
-            The collection to remove the datapoint from.
-        datapoint : Point
-            The datapoint to remove.
-        Returns
-        -------
-        Collection
-            The collection with the removed datapoint.
-        """
-        collection.remove(datapoint)
-        return collection
-
-    @staticmethod
-    def remove_and_add(old_collection, new_collection, datapoint):
-        """ Remove a datapoint from one collection and add it to another.
-        Parameters
-        ----------
-        old_collection : Collection
-            The collection to remove the datapoint from.
-        new_collection : Collection
-            The collection to add the datapoint to.
-        datapoint : Point
-            The datapoint to remove and add.
-        Returns
-        -------
-        Collection
-            The old collection with the removed datapoint.
-        Collection
-            The new collection with the added datapoint.
-        """
-        old_collection.remove(datapoint)
-        new_collection.add(datapoint)
-
-        return old_collection, new_collection
-
-    def find(self, datapoint_id, show_names=False):
-        """ Find a collection by datapoint id.
-        Parameters
-        ----------
-        datapoint_id : int
-            The id of the datapoint to find.
-        show_names : bool
-            Whether to return the collection names instead of the collections.
-        Returns
-        -------
-        list
-            The collections containing the datapoint.
-        """
-        collections = []
-
-        # also support point objects
-        if type(datapoint_id) == Point:
-            datapoint_id = datapoint_id.id
-
-        for c in self.collections:
-
-            if datapoint_id in self.collections[c].data:
-                collections.append(self.collections[c])
-
-        # just lookup names if requested
-        collections_with_names = {}
-
-        if show_names:
-            for i, c in enumerate(collections):
-
-                if collections[i].id in self.names:
-                    name = self.names[collections[i].id]
-                else:
-                    name = 'unknown' + str(i)
-                collections_with_names[name] = collections[i]
-            collections = collections_with_names
-
-        return collections
-
-    def save(self, filepath):
-        """ Save the manager to a file.
-        Parameters
-        ----------
-        filepath : str
-            The filepath to save the manager to.
-        """
-        with open(filepath, 'wb') as f:
-            pickle.dump(self, f)
-
-    @staticmethod
-    def load(filepath):
-        """ Load a manager from a file.
-        Parameters
-        ----------
-        filepath : str
-            The filepath to load the manager from.
-        Returns
-        -------
-        Manager
-            The loaded manager.
-        """
-        with open(filepath, 'rb') as f:
-            m = pickle.load(f)
-
-        return m
+from .collection import Collection
+from .point import Point
+
+import pickle
+
+
+class Manager:
+    """ A class to manage collections of data."""
+
+    def __init__(self):
+        """ Initialize the manager."""
+        self.collections = {}
+        self.names = {}
+
+    def register(self, collection, name=None):
+        """ Register a collection with the manager.
+        Parameters
+        ----------
+        collection : Collection
+            The collection to register.
+        name : str
+            The name to register the collection with.
+        """
+        # here we need to remove the old collection
+        if name:
+            for c in self.names:
+                if self.names[c] == name:
+                    old_collection_id = c
+                    del self.collections[old_collection_id]
+                    del self.names[c]
+                    # print('Unregistered stale collection:', name)
+                    break
+
+        # register this collection + name if given
+        self.collections[collection.id] = collection
+
+        if name:
+            self.names[collection.id] = name
+
+    def get(self, name):
+        """ Get a collection by name.
+        Parameters
+        ----------
+        name : str
+            The name of the collection to get.
+        Returns
+        -------
+        Collection
+            The collection with the given name.
+        """
+        # get name
+        for c in self.names:
+            if self.names[c] == name:
+                return self.collections[c]
+
+    @staticmethod
+    def add(collection, datapoint):
+        """ Add a datapoint to a collection.
+        Parameters
+        ----------
+        collection : Collection
+            The collection to add the datapoint to.
+        datapoint : Point
+            The datapoint to add.
+        Returns
+        -------
+        Collection
+            The collection with the added datapoint.
+        """
+        collection.add(datapoint)
+        return collection
+
+    @staticmethod
+    def remove(collection, datapoint):
+        """ Remove a datapoint from a collection.
+        Parameters
+        ----------
+        collection : Collection
+            The collection to remove the datapoint from.
+        datapoint : Point
+            The datapoint to remove.
+        Returns
+        -------
+        Collection
+            The collection with the removed datapoint.
+        """
+        collection.remove(datapoint)
+        return collection
+
+    @staticmethod
+    def remove_and_add(old_collection, new_collection, datapoint):
+        """ Remove a datapoint from one collection and add it to another.
+        Parameters
+        ----------
+        old_collection : Collection
+            The collection to remove the datapoint from.
+        new_collection : Collection
+            The collection to add the datapoint to.
+        datapoint : Point
+            The datapoint to remove and add.
+        Returns
+        -------
+        Collection
+            The old collection with the removed datapoint.
+        Collection
+            The new collection with the added datapoint.
+        """
+        old_collection.remove(datapoint)
+        new_collection.add(datapoint)
+
+        return old_collection, new_collection
+
+    def find(self, datapoint_id, show_names=False):
+        """ Find a collection by datapoint id.
+        Parameters
+        ----------
+        datapoint_id : int
+            The id of the datapoint to find.
+        show_names : bool
+            Whether to return the collection names instead of the collections.
+        Returns
+        -------
+        list
+            The collections containing the datapoint.
+        """
+        collections = []
+
+        # also support point objects
+        if type(datapoint_id) == Point:
+            datapoint_id = datapoint_id.id
+
+        for c in self.collections:
+
+            if datapoint_id in self.collections[c].data:
+                collections.append(self.collections[c])
+
+        # just lookup names if requested
+        collections_with_names = {}
+
+        if show_names:
+            for i, c in enumerate(collections):
+
+                if collections[i].id in self.names:
+                    name = self.names[collections[i].id]
+                else:
+                    name = 'unknown' + str(i)
+                collections_with_names[name] = collections[i]
+            collections = collections_with_names
+
+        return collections
+
+    def save(self, filepath):
+        """ Save the manager to a file.
+        Parameters
+        ----------
+        filepath : str
+            The filepath to save the manager to.
+        """
+        with open(filepath, 'wb') as f:
+            pickle.dump(self, f)
+
+    @staticmethod
+    def load(filepath):
+        """ Load a manager from a file.
+        Parameters
+        ----------
+        filepath : str
+            The filepath to load the manager from.
+        Returns
+        -------
+        Manager
+            The loaded manager.
+        """
+        with open(filepath, 'rb') as f:
+            m = pickle.load(f)
+
+        return m
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/classifier.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/classifier.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-from abc import ABC, abstractmethod
-
-
-class Classifier(ABC):
-    """ Abstract Base class for classifiers
-
-    """
-
-    def __init__(self, verbose=True, workingdir='/tmp', **kwargs):
-        """ Initialize the Classifier class.
-
-        Parameters
-        ----------
-        verbose : bool
-            Whether to print the model summary.
-        workingdir : str
-            The working directory to use for saving the model.
-        **kwargs : dict
-            Additional keyword arguments.
-
-        """
-        self.verbose = verbose
-        self.workingdir = workingdir
-        pass
-
-    @abstractmethod
-    def build(self):
-        pass
-
-    @abstractmethod
-    def train(self, X_train, y_train, X_val, y_val, patience_counter):
-        pass
-
-    @abstractmethod
-    def predict(self, X_test, y_pred, threshold):
-        pass
+from abc import ABC, abstractmethod
+
+
+class Classifier(ABC):
+    """ Abstract Base class for classifiers
+
+    """
+
+    def __init__(self, verbose=True, workingdir='/tmp', **kwargs):
+        """ Initialize the Classifier class.
+
+        Parameters
+        ----------
+        verbose : bool
+            Whether to print the model summary.
+        workingdir : str
+            The working directory to use for saving the model.
+        **kwargs : dict
+            Additional keyword arguments.
+
+        """
+        self.verbose = verbose
+        self.workingdir = workingdir
+
+    @abstractmethod
+    def build(self):
+        pass
+
+    @abstractmethod
+    def train(self, X_train, y_train, X_val, y_val, patience_counter):
+        pass
+
+    @abstractmethod
+    def predict(self, X_test, y_pred, threshold):
+        pass
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/k_att_unet2d.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/k_att_unet2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
                  stack_num_up=2,
                  activation='ReLU',
                  atten_activation='ReLU',
                  attention='add',
                  output_activation='Sigmoid',
                  batch_norm=True,
                  pool=True,
-                 unpool=True,
+                 unpool=False,
                  backbone=None,
                  weights='imagenet',
                  freeze_backbone=True,
                  freeze_batch_norm=True,
-                 name='attunet',
+                 name='kattunet2d',
                  optimizer=None,
                  loss=None,
                  metric=None,
                  verbose=False,
                  workingdir='/tmp',
                  ):
         """
@@ -91,15 +91,15 @@
         """
         from keras import losses
         from tensorflow.keras import optimizers
         from keras_unet_collection import models
         super().__init__(verbose=verbose, workingdir=workingdir)
 
         self.input_size = input_size
-        self.filter_num = filter_num or [32, 64, 128, 256, 512, 1024, 2048]
+        self.filter_num = filter_num or [16, 32, 64, 128, 256]
         self.n_labels = n_labels
         self.stack_num_down = stack_num_down
         self.stack_num_up = stack_num_up
         self.activation = activation
         self.atten_activation = atten_activation
         self.attention = attention
         self.output_activation = output_activation
@@ -126,15 +126,15 @@
                                         batch_norm=self.batch_norm,
                                         pool=self.pool, unpool=self.unpool,
                                         backbone=self.backbone,
                                         weights=self.weights,
                                         freeze_backbone=self.freeze_backbone,
                                         freeze_batch_norm=self.freeze_batch_norm,
                                         name=self.name)
-        print('*** GP2 KATTUnet2D ***')
+        print('*** GP2 KATTUNet2D ***')
         print('Working directory:', self.workingdir)
 
         self.build()
 
         if self.verbose:
             print('Verbose mode active!')
             print(self)
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/k_r2_unet2d.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/k_r2_unet2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     def __init__(self,
                  input_size=(512, 512, 1),
                  filter_num=None,
                  n_labels=1,
                  stack_num_down=2,
                  stack_num_up=2,
                  recur_num=2,
-                 activation='PReLU',
+                 activation='ReLU',
                  output_activation='Sigmoid',
-                 batch_norm=False,
-                 pool=False,
+                 batch_norm=True,
+                 pool=True,
                  unpool=False,
-                 name='r2_unet',
+                 name='kr2unet2d',
                  optimizer=None,
                  loss=None,
                  metric=None,
                  verbose=False,
                  workingdir='/tmp',
                  ):
         """
@@ -96,15 +96,15 @@
                                        activation=self.activation,
                                        output_activation=self.output_activation,
                                        batch_norm=self.batch_norm,
                                        pool=self.pool,
                                        unpool=self.unpool,
                                        name=self.name)
 
-        print('*** GP2 R2UNet2dD ***')
+        print('*** GP2 KR2UNet2dD ***')
         print('Working directory:', self.workingdir)
 
         self.build()
 
         if verbose:
             print('Verbose mode active!')
             print(self)
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/k_res_unet2d.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/k_res_unet2d.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     """
 
     def __init__(self,
                  input_size=(512, 512, 1),
                  filter_num=None,
                  dilation_num=None,
                  n_labels=1,
-                 aspp_num_down=16,
-                 aspp_num_up=8,
-                 activation='PReLU',
+                 aspp_num_down=None,
+                 aspp_num_up=None,
+                 activation='ReLU',
                  output_activation='Sigmoid',
-                 batch_norm=False,
-                 pool=False,
+                 batch_norm=True,
+                 pool=True,
                  unpool=False,
-                 name='resunet',
+                 name='kresunet2d',
                  optimizer=None,
                  loss=None,
                  metric=None,
                  verbose=False,
                  workingdir='/tmp',
                  ):
         """
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/k_unet.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/k_unet.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                             use_dropout_on_upsampling=self.use_dropout_on_upsampling,
                             use_attention=self.use_attention,
                             filters=self.filters,
                             num_layers=self.num_layers,
                             output_activation=self.output_activation
                             )
 
-        print('*** GP2 KUnet ***')
+        print('*** GP2 Keras UNet ***')
         print('Working directory:', self.workingdir)
 
         self.build()
 
         if verbose:
             print('Verbose mode active!')
             print(self)
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/k_unet2d.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/k_unet2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                  batch_norm=True,
                  pool=True,
                  unpool=True,
                  backbone=None,
                  weights='imagenet',
                  freeze_backbone=True,
                  freeze_batch_norm=True,
-                 name='unet',
+                 name='kunet2d',
                  optimizer=None,
                  loss=None,
                  metric=None,
                  verbose=False,
                  workingdir='/tmp',
                  ):
         """
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/k_unet3_plus2d.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/k_unet3_plus2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                  stack_num_up=3,
                  activation='ReLU',
                  output_activation='Sigmoid',
                  batch_norm=False,
                  pool=True,
                  unpool=True,
                  deep_supervision=False,
-                 name='unet3plus',
+                 name='kunet3plus2d',
                  optimizer=None,
                  loss=None,
                  metric=None,
                  verbose=False,
                  workingdir='/tmp',
                  ):
         """
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/k_unet_plus2d.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/k_unet_plus2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  pool=True,
                  unpool=True,
                  deep_supervision=False,
                  backbone=None,
                  weights='imagenet',
                  freeze_backbone=True,
                  freeze_batch_norm=True,
-                 name='xnet',
+                 name='kunetplus2d',
                  optimizer=None,
                  loss=None,
                  metric=None,
                  verbose=False,
                  workingdir='/tmp',
                  ):
         """
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/k_vnet2d.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/k_vnet2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                  res_num_ini=1,
                  res_num_max=2,
                  activation='ReLU',
                  output_activation='Sigmoid',
                  batch_norm=True,
                  pool=False,
                  unpool=False,
-                 name='vnet',
+                 name='kvnet2d',
                  optimizer=None,
                  loss=None,
                  metric=None,
                  verbose=False,
                  workingdir='/tmp',
                  ):
         """
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/unet.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/unet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,243 +1,243 @@
-from .classifier import Classifier
-from gp2.gp2.util import Util
-
-import os
-import pickle
-
-
-class UNet(Classifier):
-
-    def __init__(self, verbose=True, workingdir='/tmp'):
-        super().__init__(verbose, workingdir)
-
-        print('*** GP2  Unet ***')
-        print('Working directory:', self.workingdir)
-
-        self.model = self.build()
-
-    def build(self, input_shape=(512, 512, 1), num_classes=1):
-        from tensorflow.keras.models import Model
-        from tensorflow.keras.layers import Input, concatenate, Conv2D, \
-            MaxPooling2D,  Activation, UpSampling2D, BatchNormalization
-        from tensorflow.keras.optimizers import RMSprop
-        super().build()
-
-        inputs = Input(shape=input_shape)
-        # 512
-
-        encoder1 = Conv2D(16, (3, 3), padding='same', input_shape=input_shape)(
-            inputs)
-        encoder1 = BatchNormalization()(encoder1)
-        encoder1 = Activation('relu')(encoder1)
-        encoder1 = Conv2D(16, (3, 3), padding='same')(encoder1)
-        encoder1 = BatchNormalization()(encoder1)
-        encoder1 = Activation('relu')(encoder1)
-        encoder1_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder1)
-        # 256
-
-        encoder2 = Conv2D(32, (3, 3), padding='same')(encoder1_layer)
-        encoder2 = BatchNormalization()(encoder2)
-        encoder2 = Activation('relu')(encoder2)
-        encoder2 = Conv2D(32, (3, 3), padding='same')(encoder2)
-        encoder2 = BatchNormalization()(encoder2)
-        encoder2 = Activation('relu')(encoder2)
-        encoder2_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder2)
-        # 128
-
-        encoder3 = Conv2D(64, (3, 3), padding='same')(encoder2_layer)
-        encoder3 = BatchNormalization()(encoder3)
-        encoder3 = Activation('relu')(encoder3)
-        encoder3 = Conv2D(64, (3, 3), padding='same')(encoder3)
-        encoder3 = BatchNormalization()(encoder3)
-        encoder3 = Activation('relu')(encoder3)
-        encoder3_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder3)
-        # 64
-
-        encoder4 = Conv2D(128, (3, 3), padding='same')(encoder3_layer)
-        encoder4 = BatchNormalization()(encoder4)
-        encoder4 = Activation('relu')(encoder4)
-        encoder4 = Conv2D(128, (3, 3), padding='same')(encoder4)
-        encoder4 = BatchNormalization()(encoder4)
-        encoder4 = Activation('relu')(encoder4)
-        encoder4_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder4)
-        # 32
-
-        encoder5 = Conv2D(256, (3, 3), padding='same')(encoder4_layer)
-        encoder5 = BatchNormalization()(encoder5)
-        encoder5 = Activation('relu')(encoder5)
-        encoder5 = Conv2D(256, (3, 3), padding='same')(encoder5)
-        encoder5 = BatchNormalization()(encoder5)
-        encoder5 = Activation('relu')(encoder5)
-        encoder5_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder5)
-        # 16
-
-        encoder6 = Conv2D(512, (3, 3), padding='same')(encoder5_layer)
-        encoder6 = BatchNormalization()(encoder6)
-        encoder6 = Activation('relu')(encoder6)
-        encoder6 = Conv2D(512, (3, 3), padding='same')(encoder6)
-        encoder6 = BatchNormalization()(encoder6)
-        encoder6 = Activation('relu')(encoder6)
-        encoder6_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder6)
-        # 8
-
-        middle = Conv2D(1024, (3, 3), padding='same')(encoder6_layer)
-        middle = BatchNormalization()(middle)
-        middle = Activation('relu')(middle)
-        middle = Conv2D(1024, (3, 3), padding='same')(middle)
-        middle = BatchNormalization()(middle)
-        middle = Activation('relu')(middle)
-        # middle
-
-        decoder6 = UpSampling2D((2, 2))(middle)
-        decoder6 = concatenate([encoder6, decoder6], axis=3)
-        decoder6 = Conv2D(512, (3, 3), padding='same')(decoder6)
-        decoder6 = BatchNormalization()(decoder6)
-        decoder6 = Activation('relu')(decoder6)
-        decoder6 = Conv2D(512, (3, 3), padding='same')(decoder6)
-        decoder6 = BatchNormalization()(decoder6)
-        decoder6 = Activation('relu')(decoder6)
-        decoder6 = Conv2D(512, (3, 3), padding='same')(decoder6)
-        decoder6 = BatchNormalization()(decoder6)
-        decoder6 = Activation('relu')(decoder6)
-        # 16
-
-        decoder5 = UpSampling2D((2, 2))(decoder6)
-        decoder5 = concatenate([encoder5, decoder5], axis=3)
-        decoder5 = Conv2D(256, (3, 3), padding='same')(decoder5)
-        decoder5 = BatchNormalization()(decoder5)
-        decoder5 = Activation('relu')(decoder5)
-        decoder5 = Conv2D(256, (3, 3), padding='same')(decoder5)
-        decoder5 = BatchNormalization()(decoder5)
-        decoder5 = Activation('relu')(decoder5)
-        decoder5 = Conv2D(256, (3, 3), padding='same')(decoder5)
-        decoder5 = BatchNormalization()(decoder5)
-        decoder5 = Activation('relu')(decoder5)
-        # 32
-
-        decoder4 = UpSampling2D((2, 2))(decoder5)
-        decoder4 = concatenate([encoder4, decoder4], axis=3)
-        decoder4 = Conv2D(128, (3, 3), padding='same')(decoder4)
-        decoder4 = BatchNormalization()(decoder4)
-        decoder4 = Activation('relu')(decoder4)
-        decoder4 = Conv2D(128, (3, 3), padding='same')(decoder4)
-        decoder4 = BatchNormalization()(decoder4)
-        decoder4 = Activation('relu')(decoder4)
-        decoder4 = Conv2D(128, (3, 3), padding='same')(decoder4)
-        decoder4 = BatchNormalization()(decoder4)
-        decoder4 = Activation('relu')(decoder4)
-        # 64
-
-        decoder3 = UpSampling2D((2, 2))(decoder4)
-        decoder3 = concatenate([encoder3, decoder3], axis=3)
-        decoder3 = Conv2D(64, (3, 3), padding='same')(decoder3)
-        decoder3 = BatchNormalization()(decoder3)
-        decoder3 = Activation('relu')(decoder3)
-        decoder3 = Conv2D(64, (3, 3), padding='same')(decoder3)
-        decoder3 = BatchNormalization()(decoder3)
-        decoder3 = Activation('relu')(decoder3)
-        decoder3 = Conv2D(64, (3, 3), padding='same')(decoder3)
-        decoder3 = BatchNormalization()(decoder3)
-        decoder3 = Activation('relu')(decoder3)
-        # 128
-
-        decoder2 = UpSampling2D((2, 2))(decoder3)
-        decoder2 = concatenate([encoder2, decoder2], axis=3)
-        decoder2 = Conv2D(32, (3, 3), padding='same')(decoder2)
-        decoder2 = BatchNormalization()(decoder2)
-        decoder2 = Activation('relu')(decoder2)
-        decoder2 = Conv2D(32, (3, 3), padding='same')(decoder2)
-        decoder2 = BatchNormalization()(decoder2)
-        decoder2 = Activation('relu')(decoder2)
-        decoder2 = Conv2D(32, (3, 3), padding='same')(decoder2)
-        decoder2 = BatchNormalization()(decoder2)
-        decoder2 = Activation('relu')(decoder2)
-        # 256
-
-        decoder1 = UpSampling2D((2, 2))(decoder2)
-        decoder1 = concatenate([encoder1, decoder1], axis=3)
-        decoder1 = Conv2D(16, (3, 3), padding='same')(decoder1)
-        decoder1 = BatchNormalization()(decoder1)
-        decoder1 = Activation('relu')(decoder1)
-        decoder1 = Conv2D(16, (3, 3), padding='same')(decoder1)
-        decoder1 = BatchNormalization()(decoder1)
-        decoder1 = Activation('relu')(decoder1)
-        decoder1 = Conv2D(16, (3, 3), padding='same')(decoder1)
-        decoder1 = BatchNormalization()(decoder1)
-        decoder1 = Activation('relu')(decoder1)
-        # 512
-
-        out = Conv2D(num_classes, (1, 1), activation='sigmoid')(decoder1)
-
-        model = Model(inputs=[inputs], outputs=[out])
-
-        model.compile(optimizer=RMSprop(learning_rate=0.0001),
-                      loss=UNet.bce_dice_loss,
-                      metrics=[UNet.dice_coeff])
-
-        return model
-
-    def train(self, X_train, y_train, X_val, y_val,
-              patience_counter=2, batch_size=64, epochs=100):
-        from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint, \
-            ReduceLROnPlateau
-        super().train(X_train, y_train, X_val, y_val, patience_counter)
-
-        checkpoint_file = os.path.join(self.workingdir, 'unet')
-        checkpoint_file = Util.create_numbered_file(checkpoint_file, '.model')
-
-        callbacks = [EarlyStopping(patience=patience_counter,
-                                   monitor='loss',
-                                   verbose=0),
-                     ModelCheckpoint(filepath=checkpoint_file,
-                                     save_weights_only=False,
-                                     monitor='val_loss',
-                                     mode='min',
-                                     verbose=0,
-                                     save_best_only=True)]
-
-        history = self.model.fit(X_train, y_train,
-                                 batch_size=batch_size,
-                                 epochs=epochs,
-                                 callbacks=callbacks,
-                                 validation_data=(X_val, y_val),
-                                 verbose=int(self.verbose))
-
-        history_file = os.path.join(self.workingdir, 'history')
-        history_file = Util.create_numbered_file(history_file, '.pickle')
-
-        with open(history_file, 'wb') as f:
-            pickle.dump(history.history, f)
-
-        print('Model saved to', checkpoint_file)
-        print('History saved to', history_file)
-
-        return history
-
-    def predict(self, X_test, y_test):
-        predictions = self.model.predict(X_test)
-
-        predictions[predictions >= 0.5] = 1.0
-        predictions[predictions < 0.5] = 0.0
-
-        scores = self.model.evaluate(X_test, y_test)
-
-        return predictions, scores
-
-    @staticmethod
-    def bce_dice_loss(y_true, y_pred):
-        import tensorflow as tf
-        y_true_f = tf.reshape(y_true, [-1])
-        y_pred_f = tf.reshape(y_pred, [-1])
-        return tf.keras.losses.binary_crossentropy(y_true, y_pred) + (
-                    1 - UNet.dice_coeff(y_true, y_pred))
-
-    @staticmethod
-    def dice_coeff(y_true, y_pred):
-        import tensorflow as tf
-        y_true_f = tf.reshape(y_true, [-1])
-        y_pred_f = tf.reshape(y_pred, [-1])
-        intersection = tf.math.reduce_sum(y_true_f * y_pred_f)
-        smoothing_const = 1e-9
-        return (2. * intersection + smoothing_const) / (
-                    tf.math.reduce_sum(y_true_f) + tf.math.reduce_sum(
+from .classifier import Classifier
+from gp2.gp2.util import Util
+
+import os
+import pickle
+
+
+class UNet(Classifier):
+
+    def __init__(self, verbose=True, workingdir='/tmp'):
+        super().__init__(verbose, workingdir)
+
+        print('*** GP2  Unet ***')
+        print('Working directory:', self.workingdir)
+
+        self.model = self.build()
+
+    def build(self, input_shape=(512, 512, 1), num_classes=1):
+        from tensorflow.keras.models import Model
+        from tensorflow.keras.layers import Input, concatenate, Conv2D, \
+            MaxPooling2D,  Activation, UpSampling2D, BatchNormalization
+        from tensorflow.keras.optimizers import RMSprop
+        super().build()
+
+        inputs = Input(shape=input_shape)
+        # 512
+
+        encoder1 = Conv2D(16, (3, 3), padding='same', input_shape=input_shape)(
+            inputs)
+        encoder1 = BatchNormalization()(encoder1)
+        encoder1 = Activation('relu')(encoder1)
+        encoder1 = Conv2D(16, (3, 3), padding='same')(encoder1)
+        encoder1 = BatchNormalization()(encoder1)
+        encoder1 = Activation('relu')(encoder1)
+        encoder1_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder1)
+        # 256
+
+        encoder2 = Conv2D(32, (3, 3), padding='same')(encoder1_layer)
+        encoder2 = BatchNormalization()(encoder2)
+        encoder2 = Activation('relu')(encoder2)
+        encoder2 = Conv2D(32, (3, 3), padding='same')(encoder2)
+        encoder2 = BatchNormalization()(encoder2)
+        encoder2 = Activation('relu')(encoder2)
+        encoder2_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder2)
+        # 128
+
+        encoder3 = Conv2D(64, (3, 3), padding='same')(encoder2_layer)
+        encoder3 = BatchNormalization()(encoder3)
+        encoder3 = Activation('relu')(encoder3)
+        encoder3 = Conv2D(64, (3, 3), padding='same')(encoder3)
+        encoder3 = BatchNormalization()(encoder3)
+        encoder3 = Activation('relu')(encoder3)
+        encoder3_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder3)
+        # 64
+
+        encoder4 = Conv2D(128, (3, 3), padding='same')(encoder3_layer)
+        encoder4 = BatchNormalization()(encoder4)
+        encoder4 = Activation('relu')(encoder4)
+        encoder4 = Conv2D(128, (3, 3), padding='same')(encoder4)
+        encoder4 = BatchNormalization()(encoder4)
+        encoder4 = Activation('relu')(encoder4)
+        encoder4_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder4)
+        # 32
+
+        encoder5 = Conv2D(256, (3, 3), padding='same')(encoder4_layer)
+        encoder5 = BatchNormalization()(encoder5)
+        encoder5 = Activation('relu')(encoder5)
+        encoder5 = Conv2D(256, (3, 3), padding='same')(encoder5)
+        encoder5 = BatchNormalization()(encoder5)
+        encoder5 = Activation('relu')(encoder5)
+        encoder5_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder5)
+        # 16
+
+        encoder6 = Conv2D(512, (3, 3), padding='same')(encoder5_layer)
+        encoder6 = BatchNormalization()(encoder6)
+        encoder6 = Activation('relu')(encoder6)
+        encoder6 = Conv2D(512, (3, 3), padding='same')(encoder6)
+        encoder6 = BatchNormalization()(encoder6)
+        encoder6 = Activation('relu')(encoder6)
+        encoder6_layer = MaxPooling2D((2, 2), strides=(2, 2))(encoder6)
+        # 8
+
+        middle = Conv2D(1024, (3, 3), padding='same')(encoder6_layer)
+        middle = BatchNormalization()(middle)
+        middle = Activation('relu')(middle)
+        middle = Conv2D(1024, (3, 3), padding='same')(middle)
+        middle = BatchNormalization()(middle)
+        middle = Activation('relu')(middle)
+        # middle
+
+        decoder6 = UpSampling2D((2, 2))(middle)
+        decoder6 = concatenate([encoder6, decoder6], axis=3)
+        decoder6 = Conv2D(512, (3, 3), padding='same')(decoder6)
+        decoder6 = BatchNormalization()(decoder6)
+        decoder6 = Activation('relu')(decoder6)
+        decoder6 = Conv2D(512, (3, 3), padding='same')(decoder6)
+        decoder6 = BatchNormalization()(decoder6)
+        decoder6 = Activation('relu')(decoder6)
+        decoder6 = Conv2D(512, (3, 3), padding='same')(decoder6)
+        decoder6 = BatchNormalization()(decoder6)
+        decoder6 = Activation('relu')(decoder6)
+        # 16
+
+        decoder5 = UpSampling2D((2, 2))(decoder6)
+        decoder5 = concatenate([encoder5, decoder5], axis=3)
+        decoder5 = Conv2D(256, (3, 3), padding='same')(decoder5)
+        decoder5 = BatchNormalization()(decoder5)
+        decoder5 = Activation('relu')(decoder5)
+        decoder5 = Conv2D(256, (3, 3), padding='same')(decoder5)
+        decoder5 = BatchNormalization()(decoder5)
+        decoder5 = Activation('relu')(decoder5)
+        decoder5 = Conv2D(256, (3, 3), padding='same')(decoder5)
+        decoder5 = BatchNormalization()(decoder5)
+        decoder5 = Activation('relu')(decoder5)
+        # 32
+
+        decoder4 = UpSampling2D((2, 2))(decoder5)
+        decoder4 = concatenate([encoder4, decoder4], axis=3)
+        decoder4 = Conv2D(128, (3, 3), padding='same')(decoder4)
+        decoder4 = BatchNormalization()(decoder4)
+        decoder4 = Activation('relu')(decoder4)
+        decoder4 = Conv2D(128, (3, 3), padding='same')(decoder4)
+        decoder4 = BatchNormalization()(decoder4)
+        decoder4 = Activation('relu')(decoder4)
+        decoder4 = Conv2D(128, (3, 3), padding='same')(decoder4)
+        decoder4 = BatchNormalization()(decoder4)
+        decoder4 = Activation('relu')(decoder4)
+        # 64
+
+        decoder3 = UpSampling2D((2, 2))(decoder4)
+        decoder3 = concatenate([encoder3, decoder3], axis=3)
+        decoder3 = Conv2D(64, (3, 3), padding='same')(decoder3)
+        decoder3 = BatchNormalization()(decoder3)
+        decoder3 = Activation('relu')(decoder3)
+        decoder3 = Conv2D(64, (3, 3), padding='same')(decoder3)
+        decoder3 = BatchNormalization()(decoder3)
+        decoder3 = Activation('relu')(decoder3)
+        decoder3 = Conv2D(64, (3, 3), padding='same')(decoder3)
+        decoder3 = BatchNormalization()(decoder3)
+        decoder3 = Activation('relu')(decoder3)
+        # 128
+
+        decoder2 = UpSampling2D((2, 2))(decoder3)
+        decoder2 = concatenate([encoder2, decoder2], axis=3)
+        decoder2 = Conv2D(32, (3, 3), padding='same')(decoder2)
+        decoder2 = BatchNormalization()(decoder2)
+        decoder2 = Activation('relu')(decoder2)
+        decoder2 = Conv2D(32, (3, 3), padding='same')(decoder2)
+        decoder2 = BatchNormalization()(decoder2)
+        decoder2 = Activation('relu')(decoder2)
+        decoder2 = Conv2D(32, (3, 3), padding='same')(decoder2)
+        decoder2 = BatchNormalization()(decoder2)
+        decoder2 = Activation('relu')(decoder2)
+        # 256
+
+        decoder1 = UpSampling2D((2, 2))(decoder2)
+        decoder1 = concatenate([encoder1, decoder1], axis=3)
+        decoder1 = Conv2D(16, (3, 3), padding='same')(decoder1)
+        decoder1 = BatchNormalization()(decoder1)
+        decoder1 = Activation('relu')(decoder1)
+        decoder1 = Conv2D(16, (3, 3), padding='same')(decoder1)
+        decoder1 = BatchNormalization()(decoder1)
+        decoder1 = Activation('relu')(decoder1)
+        decoder1 = Conv2D(16, (3, 3), padding='same')(decoder1)
+        decoder1 = BatchNormalization()(decoder1)
+        decoder1 = Activation('relu')(decoder1)
+        # 512
+
+        out = Conv2D(num_classes, (1, 1), activation='sigmoid')(decoder1)
+
+        model = Model(inputs=[inputs], outputs=[out])
+
+        model.compile(optimizer=RMSprop(learning_rate=0.0001),
+                      loss=UNet.bce_dice_loss,
+                      metrics=[UNet.dice_coeff])
+
+        return model
+
+    def train(self, X_train, y_train, X_val, y_val,
+              patience_counter=2, batch_size=64, epochs=100):
+        from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint, \
+            ReduceLROnPlateau
+        super().train(X_train, y_train, X_val, y_val, patience_counter)
+
+        checkpoint_file = os.path.join(self.workingdir, 'unet')
+        checkpoint_file = Util.create_numbered_file(checkpoint_file, '.model')
+
+        callbacks = [EarlyStopping(patience=patience_counter,
+                                   monitor='loss',
+                                   verbose=0),
+                     ModelCheckpoint(filepath=checkpoint_file,
+                                     save_weights_only=False,
+                                     monitor='val_loss',
+                                     mode='min',
+                                     verbose=0,
+                                     save_best_only=True)]
+
+        history = self.model.fit(X_train, y_train,
+                                 batch_size=batch_size,
+                                 epochs=epochs,
+                                 callbacks=callbacks,
+                                 validation_data=(X_val, y_val),
+                                 verbose=int(self.verbose))
+
+        history_file = os.path.join(self.workingdir, 'history')
+        history_file = Util.create_numbered_file(history_file, '.pickle')
+
+        with open(history_file, 'wb') as f:
+            pickle.dump(history.history, f)
+
+        print('Model saved to', checkpoint_file)
+        print('History saved to', history_file)
+
+        return history
+
+    def predict(self, X_test, y_test, threshold=0.5):
+        predictions = self.model.predict(X_test)
+
+        predictions[predictions >= threshold] = 1.0
+        predictions[predictions < threshold] = 0.0
+
+        scores = self.model.evaluate(X_test, y_test)
+
+        return predictions, scores
+
+    @staticmethod
+    def bce_dice_loss(y_true, y_pred):
+        import tensorflow as tf
+        y_true_f = tf.reshape(y_true, [-1])
+        y_pred_f = tf.reshape(y_pred, [-1])
+        return tf.keras.losses.binary_crossentropy(y_true_f, y_pred_f) + (
+                1 - UNet.dice_coeff(y_true_f, y_pred_f))
+
+    @staticmethod
+    def dice_coeff(y_true, y_pred):
+        import tensorflow as tf
+        y_true_f = tf.reshape(y_true, [-1])
+        y_pred_f = tf.reshape(y_pred, [-1])
+        intersection = tf.math.reduce_sum(y_true_f * y_pred_f)
+        smoothing_const = 1e-9
+        return (2. * intersection + smoothing_const) / (
+                    tf.math.reduce_sum(y_true_f) + tf.math.reduce_sum(
                 y_pred_f) + smoothing_const)
```

### Comparing `gp2-0.5.25.23/gp2/gp2/classifiers/unet_plus.py` & `gp2-0.7.22.23/gp2/gp2/classifiers/unet_plus.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,55 +78,53 @@
         self.depth = depth
         self.num_layers = num_layers
         self.name = name
         self.optimizer = optimizer or optimizers.Adam(learning_rate=1e-4)
         self.loss = loss or losses.binary_crossentropy
         self.metrics = metrics or [Util.dice_coeff]
 
-        print('*** GP2  KUNet2D ***')
+        print('*** GP2  UNetPLUS ***')
         print('Working directory:', self.workingdir)
 
         self.model = self.build()
 
         if verbose:
             print('Verbose mode active!')
-            print(str(vars(self)))
+            print(vars(self))
             self.model.summary()
 
     def build(self):
         """ Build the model.
 
         Returns
         -------
         model : keras.Model
             The model.
         """
-        super().build()
-
         inputs = layers.Input(shape=self.input_shape)
 
         # Contracting path (encoder)
         x = inputs
         skips = []
         for i in range(self.depth):
-            for j in range(self.num_layers):
+            for _ in range(self.num_layers):
                 x = layers.Conv2D(self.base_filters * (2 ** i),
                                   self.kernel_size,
                                   padding=self.padding,
                                   strides=self.strides,
                                   activation=self.activation)(x)
                 if self.batchnorm:
                     x = layers.BatchNormalization()(x)
                 if self.dropout:
                     x = layers.Dropout(self.dropout)(x)
             skips.append(x)
             x = layers.MaxPooling2D((2, 2))(x)
 
         # Bottleneck (encoder)
-        for i in range(self.num_layers):
+        for _ in range(self.num_layers):
             x = layers.Conv2D(self.base_filters * (2 ** self.depth),
                               self.kernel_size,
                               padding=self.padding,
                               strides=self.strides,
                               activation=self.activation)(x)
             if self.batchnorm:
                 x = layers.BatchNormalization()(x)
@@ -136,15 +134,15 @@
         # Expansive path (decoder)
         for i in reversed(range(self.depth)):
             x = layers.Conv2DTranspose(self.base_filters * (2 ** i),
                                        (2, 2),
                                        strides=(2, 2),
                                        padding='same')(x)
             x = layers.concatenate([x, skips[i]])
-            for j in range(self.num_layers):
+            for _ in range(self.num_layers):
                 x = layers.Conv2D(self.base_filters * (2 ** i),
                                   self.kernel_size,
                                   padding=self.padding,
                                   strides=self.strides,
                                   activation=self.activation)(x)
                 if self.batchnorm:
                     x = layers.BatchNormalization()(x)
```

### Comparing `gp2-0.5.25.23/gp2/gp2/discriminators/base_cnn_discriminator.py` & `gp2-0.7.22.23/gp2/gp2/discriminators/base_cnn_discriminator.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.25.23/gp2/gp2/discriminators/cnn_discriminator_plus.py` & `gp2-0.7.22.23/gp2/gp2/discriminators/cnn_discriminator_plus.py`

 * *Files identical despite different names*

### Comparing `gp2-0.5.25.23/gp2/gp2/discriminators/cnndiscriminator.py` & `gp2-0.7.22.23/gp2/gp2/discriminators/cnndiscriminator.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-from .discriminator import Discriminator
-import os
-import pickle
-from gp2.gp2.util import Util
-
-class CNNDiscriminator(Discriminator):
-
-    def __init__(self, verbose=True, workingdir='/tmp'):
-        super().__init__(verbose, workingdir)
-
-        self.model = self.build()
-
-    def create_convolution_layers(self, input_img, input_shape):
-        """ Create the convolution layers
-
-        Args:
-            input_img:  (tf.keras.layers.Input) input layer
-            input_shape:  (tuple) input shape
-
-        Returns:
-        """
-        from tensorflow.keras.layers import Conv2D,  MaxPooling2D, LeakyReLU, Dropout
-        # 512
-        model = Conv2D(16, (3, 3), padding='same', input_shape=input_shape)(
-            input_img)
-        model = LeakyReLU(alpha=0.1)(model)
-        model = MaxPooling2D((2, 2), padding='same')(model)
-        model = Dropout(0.25)(model)
-        # 256
-
-        model = Conv2D(32, (3, 3), padding='same')(model)
-        model = LeakyReLU(alpha=0.1)(model)
-        model = MaxPooling2D((2, 2), padding='same')(model)
-        model = Dropout(0.25)(model)
-        # 128
-
-        model = Conv2D(64, (3, 3), padding='same')(model)
-        model = LeakyReLU(alpha=0.1)(model)
-        model = MaxPooling2D(pool_size=(2, 2), padding='same')(model)
-        model = Dropout(0.25)(model)
-        # 64
-
-        model = Conv2D(128, (3, 3), padding='same')(model)
-        model = LeakyReLU(alpha=0.1)(model)
-        model = MaxPooling2D(pool_size=(2, 2), padding='same')(model)
-        model = Dropout(0.4)(model)
-        # 32
-
-        model = Conv2D(256, (3, 3), padding='same')(model)
-        model = LeakyReLU(alpha=0.1)(model)
-        model = MaxPooling2D(pool_size=(2, 2), padding='same')(model)
-        model = Dropout(0.4)(model)
-        # 16
-
-        return model
-
-    def build(self, image_shape=(512, 512, 1), num_classes=2):
-        """ Builds the model.
-
-        :param image_shape: The shape of the input images.
-        :param num_classes: The number of classes.
-        :return: The model.
-        """
-        from tensorflow.keras.layers import Input, concatenate,  LeakyReLU, \
-            Dropout, Flatten, Dense
-        from tensorflow.keras.models import Model
-        super().build()
-
-        image_input = Input(shape=image_shape)
-        image_model = self.create_convolution_layers(image_input, image_shape)
-
-        mask_input = Input(shape=image_shape)
-        mask_model = self.create_convolution_layers(mask_input, image_shape)
-
-        conv = concatenate([image_model, mask_model])
-
-        conv = Flatten()(conv)
-
-        dense = Dense(512)(conv)
-        dense = LeakyReLU(alpha=0.1)(dense)
-        dense = Dropout(0.5)(dense)
-
-        output = Dense(num_classes, activation='softmax')(dense)
-
-        model = Model(inputs=[image_input, mask_input], outputs=[output])
-
-        # compile the model
-        model.compile(optimizer='Adam',
-                      loss='categorical_crossentropy',
-                      metrics=['accuracy'])
-
-        return model
-
-    def train(self, X_train_images, X_train_masks, y_train,
-              X_val_images, X_val_masks, y_val,
-              patience_counter=10, batch_size=64, epochs=100):
-        """ Trains the model.
-
-        :param X_train_images: The training images.
-        :param X_train_masks: The training masks.
-        :param y_train: The training labels.
-        :param X_val_images: The validation images.
-        :param X_val_masks: The validation masks.
-        :param y_val: The validation labels.
-        :param patience_counter: The patience counter for early stopping.
-        :param batch_size: The batch size.
-        :param epochs: The number of epochs.
-        :return:
-        """
-        from tensorflow.keras.utils import to_categorical
-        from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint
-        super().train(X_train_images, X_train_masks, y_train,
-                      X_val_images, X_val_masks, y_val)
-
-        checkpoint_file = os.path.join(self.workingdir, 'cnnd')
-        checkpoint_file = Util.create_numbered_file(checkpoint_file, '.model')
-
-        callbacks = [EarlyStopping(patience=patience_counter,
-                                   monitor='loss',
-                                   verbose=0),
-                     ModelCheckpoint(filepath=checkpoint_file,
-                                     save_weights_only=False,
-                                     monitor='val_loss',
-                                     mode='min',
-                                     verbose=0,
-                                     save_best_only=True)]
-
-        y_train = to_categorical(y_train)
-        y_val = to_categorical(y_val)
-
-        history = self.model.fit(x=[X_train_images, X_train_masks], y=y_train,
-                                 batch_size=batch_size,
-                                 epochs=epochs,
-                                 callbacks=callbacks,
-                                 validation_data=(
-                                 [X_val_images, X_val_masks], y_val),
-                                 verbose=0)
-
-        history_file = os.path.join(self.workingdir, 'cnnd_history')
-        history_file = Util.create_numbered_file(history_file, '.pickle')
-
-        with open(history_file, 'wb') as f:
-            pickle.dump(history.history, f)
-
-        print('Model saved to', checkpoint_file)
-        print('History saved to', history_file)
-
-    def predict(self, X_test_images, X_test_masks, y_test):
-        """ Predicts the labels for the given test data.
-
-        :param X_test_images: The test images.
-        :param X_test_masks: The test masks.
-        :param y_test: The test labels.
-        :return: The predicted labels and the scores.
-        """
-        import numpy as np
-        from tensorflow.keras.utils import to_categorical
-        predictions = self.model.predict(x=[X_test_images, X_test_masks])
-
-        # grab the most likely label from the categorical representation
-        predictions = np.argmax(predictions, axis=-1)
-
-        y_test = to_categorical(y_test)
-
-        scores = self.model.evaluate(x=[X_test_images, X_test_masks], y=y_test)
-
+from .discriminator import Discriminator
+import os
+import pickle
+from gp2.gp2.util import Util
+
+class CNNDiscriminator(Discriminator):
+
+    def __init__(self, verbose=True, workingdir='/tmp'):
+        super().__init__(verbose, workingdir)
+
+        self.model = self.build()
+
+    def create_convolution_layers(self, input_img, input_shape):
+        """ Create the convolution layers
+
+        Args:
+            input_img:  (tf.keras.layers.Input) input layer
+            input_shape:  (tuple) input shape
+
+        Returns:
+        """
+        from tensorflow.keras.layers import Conv2D,  MaxPooling2D, LeakyReLU, Dropout
+        # 512
+        model = Conv2D(16, (3, 3), padding='same', input_shape=input_shape)(
+            input_img)
+        model = LeakyReLU(alpha=0.1)(model)
+        model = MaxPooling2D((2, 2), padding='same')(model)
+        model = Dropout(0.25)(model)
+        # 256
+
+        model = Conv2D(32, (3, 3), padding='same')(model)
+        model = LeakyReLU(alpha=0.1)(model)
+        model = MaxPooling2D((2, 2), padding='same')(model)
+        model = Dropout(0.25)(model)
+        # 128
+
+        model = Conv2D(64, (3, 3), padding='same')(model)
+        model = LeakyReLU(alpha=0.1)(model)
+        model = MaxPooling2D(pool_size=(2, 2), padding='same')(model)
+        model = Dropout(0.25)(model)
+        # 64
+
+        model = Conv2D(128, (3, 3), padding='same')(model)
+        model = LeakyReLU(alpha=0.1)(model)
+        model = MaxPooling2D(pool_size=(2, 2), padding='same')(model)
+        model = Dropout(0.4)(model)
+        # 32
+
+        model = Conv2D(256, (3, 3), padding='same')(model)
+        model = LeakyReLU(alpha=0.1)(model)
+        model = MaxPooling2D(pool_size=(2, 2), padding='same')(model)
+        model = Dropout(0.4)(model)
+        # 16
+
+        return model
+
+    def build(self, image_shape=(512, 512, 1), num_classes=2):
+        """ Builds the model.
+
+        :param image_shape: The shape of the input images.
+        :param num_classes: The number of classes.
+        :return: The model.
+        """
+        from tensorflow.keras.layers import Input, concatenate,  LeakyReLU, \
+            Dropout, Flatten, Dense
+        from tensorflow.keras.models import Model
+        super().build()
+
+        image_input = Input(shape=image_shape)
+        image_model = self.create_convolution_layers(image_input, image_shape)
+
+        mask_input = Input(shape=image_shape)
+        mask_model = self.create_convolution_layers(mask_input, image_shape)
+
+        conv = concatenate([image_model, mask_model])
+
+        conv = Flatten()(conv)
+
+        dense = Dense(512)(conv)
+        dense = LeakyReLU(alpha=0.1)(dense)
+        dense = Dropout(0.5)(dense)
+
+        output = Dense(num_classes, activation='softmax')(dense)
+
+        model = Model(inputs=[image_input, mask_input], outputs=[output])
+
+        # compile the model
+        model.compile(optimizer='Adam',
+                      loss='categorical_crossentropy',
+                      metrics=['accuracy'])
+
+        return model
+
+    def train(self, X_train_images, X_train_masks, y_train,
+              X_val_images, X_val_masks, y_val,
+              patience_counter=10, batch_size=64, epochs=100):
+        """ Trains the model.
+
+        :param X_train_images: The training images.
+        :param X_train_masks: The training masks.
+        :param y_train: The training labels.
+        :param X_val_images: The validation images.
+        :param X_val_masks: The validation masks.
+        :param y_val: The validation labels.
+        :param patience_counter: The patience counter for early stopping.
+        :param batch_size: The batch size.
+        :param epochs: The number of epochs.
+        :return:
+        """
+        from tensorflow.keras.utils import to_categorical
+        from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint
+        super().train(X_train_images, X_train_masks, y_train,
+                      X_val_images, X_val_masks, y_val)
+
+        checkpoint_file = os.path.join(self.workingdir, 'cnnd')
+        checkpoint_file = Util.create_numbered_file(checkpoint_file, '.model')
+
+        callbacks = [EarlyStopping(patience=patience_counter,
+                                   monitor='loss',
+                                   verbose=0),
+                     ModelCheckpoint(filepath=checkpoint_file,
+                                     save_weights_only=False,
+                                     monitor='val_loss',
+                                     mode='min',
+                                     verbose=0,
+                                     save_best_only=True)]
+
+        y_train = to_categorical(y_train)
+        y_val = to_categorical(y_val)
+
+        history = self.model.fit(x=[X_train_images, X_train_masks], y=y_train,
+                                 batch_size=batch_size,
+                                 epochs=epochs,
+                                 callbacks=callbacks,
+                                 validation_data=(
+                                 [X_val_images, X_val_masks], y_val),
+                                 verbose=0)
+
+        history_file = os.path.join(self.workingdir, 'cnnd_history')
+        history_file = Util.create_numbered_file(history_file, '.pickle')
+
+        with open(history_file, 'wb') as f:
+            pickle.dump(history.history, f)
+
+        print('Model saved to', checkpoint_file)
+        print('History saved to', history_file)
+
+    def predict(self, X_test_images, X_test_masks, y_test):
+        """ Predicts the labels for the given test data.
+
+        :param X_test_images: The test images.
+        :param X_test_masks: The test masks.
+        :param y_test: The test labels.
+        :return: The predicted labels and the scores.
+        """
+        import numpy as np
+        from tensorflow.keras.utils import to_categorical
+        predictions = self.model.predict(x=[X_test_images, X_test_masks])
+
+        # grab the most likely label from the categorical representation
+        predictions = np.argmax(predictions, axis=-1)
+
+        y_test = to_categorical(y_test)
+
+        scores = self.model.evaluate(x=[X_test_images, X_test_masks], y=y_test)
+
         return predictions, scores
```

### Comparing `gp2-0.5.25.23/gp2/gp2/util.py` & `gp2-0.7.22.23/gp2/gp2/util.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-import logging
-import os
-import warnings
-
-
-class Util:
-    @staticmethod
-    def disable_tensorflow_logging():
-        import warnings
-        import os
-        os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
-        warnings.filterwarnings('ignore', category=UserWarning,
-                                module='tensorflow')
-        warnings.filterwarnings("ignore", category=DeprecationWarning)
-        warnings.filterwarnings("ignore", category=FutureWarning)
-        import logging
-        import tensorflow as tf
-        logger = tf.get_logger()
-        logger.setLevel(logging.ERROR)
-        from tensorflow.python.keras.utils.generic_utils import \
-            CustomMaskWarning
-        warnings.filterwarnings('ignore', category=CustomMaskWarning)
-
-    @staticmethod
-    def create_A_B_Z_split(images, labels, dataset_size=1000, weights=None):
-        """ Creates A, B, Z split from images and labels
-        Parameters
-        ----------
-        images : numpy array
-            The images to split
-        labels : numpy array
-            The labels to split
-        dataset_size : int
-            The size of the dataset
-        weights : dict
-            The weights to use for the split. If None, the split is 40/40/20
-        Returns
-        -------
-        A : numpy array
-            The A split
-        B : numpy array
-            The B split
-        Z : numpy array
-            The Z split
-        """
-        import numpy as np
-
-        A_split = int(0.4 * dataset_size)
-        B_split = int(0.2 * dataset_size)
-        Z_split = int(0.4 * dataset_size)
-
-        if weights:
-            A_split = int(weights['A'] * dataset_size)
-            B_split = int(weights['B'] * dataset_size)
-            Z_split = int(weights['Z'] * dataset_size)
-
-        # machine data
-        A = images[0:A_split, :, :, 0]
-        A_labels = labels[0:A_split, :, :, 0]
-
-        A = np.stack((A, A_labels), axis=-1)
-
-        # human data
-        B = images[A_split:A_split + B_split, :, :, 0]
-        B_labels = labels[A_split:A_split + B_split, :, :, 0]
-
-        B = np.stack((B, B_labels), axis=-1)
-
-        # we will also provide a Z array that
-        # can be used to funnel additional data later
-
-        # funnel data
-        Z = images[A_split + B_split:A_split + B_split + Z_split, :, :, 0]
-        Z_labels = labels[A_split + B_split:A_split + B_split + Z_split, :, :,
-                   0]
-
-        Z = np.stack((Z, Z_labels), axis=-1)
-
-        return A, B, Z
-
-    @staticmethod
-    def create_train_val_test_split(dataset,
-                                    train_count=200,
-                                    val_count=300,
-                                    test_count=250,
-                                    shuffle=True):
-        """ Creates a train, val, test split from a dataset
-
-        Parameters
-        ----------
-        dataset : numpy array
-            The dataset to split
-        train_count : int
-            The number of training samples
-        val_count : int
-            The number of validation samples
-        test_count : int
-            The number of test samples
-        shuffle : bool
-            Whether to shuffle the dataset before splitting
-
-        Returns
-        -------
-        train : numpy array
-            The training split
-        val : numpy array
-            The validation split
-        test : numpy array
-            The test split
-        """
-        import numpy as np
-        if shuffle:
-            np.random.shuffle(dataset)
-
-        train = dataset[0:train_count]
-        val = dataset[train_count:train_count + val_count]
-        test = dataset[
-               train_count + val_count:train_count + val_count + test_count]
-
-        return train, val, test
-
-    @staticmethod
-    def create_numbered_file(filename, extension):
-        """ Creates a numbered file
-
-        Parameters
-        ----------
-        filename : str
-            The filename
-        extension : str
-            The extension
-
-        Returns
-        -------
-        numbered_file : str
-            The numbered file
-        """
-        number = 0000
-        numbered_file = filename + '_' + str(number) + extension
-        while os.path.exists(numbered_file):
-            number += 1
-            numbered_file = filename + '_' + str(number) + extension
-
-        return numbered_file
-
-    @staticmethod
-    def plot_accuracies(x, y1, y2):
-        """ Plot line chart showing accuracies of classifier and discriminator
-
-        Parameters
-        ----------
-        x : range
-            The range of the x-axis
-        y1 : numpy.ndarray | list
-            The y-axis values for the classifier.
-        y2 : numpy.ndarray | list
-            The y-axis values for the discriminator.
-
-        Returns
-        -------
-        None
-        """
-        import matplotlib.pyplot as plt
-        fig, ax1 = plt.subplots(1, 1, figsize=(3, 3), dpi=80)
-        line1, = ax1.plot(x, y1, color='tab:red', label='Classifier')
-        line2, = ax1.plot(x, y2, color='tab:blue', label='Discriminator')
-        ax1.legend(handles=[line1, line2])
-        ax1.xaxis.set_major_locator(plt.MaxNLocator(integer=True))
-
-        ax1.set_xlabel('Cycle', color='tab:gray', fontsize=14)
-        ax1.tick_params(axis='x', rotation=0, labelsize=12,
-                        labelcolor='tab:gray')
-        ax1.set_ylabel('Accuracy', color='tab:red', fontsize=14)
-        ax1.tick_params(axis='y', rotation=0, labelcolor='tab:red')
-        ax1.grid(alpha=.4)
-        fig.tight_layout()
-        plt.show()
-
-    @staticmethod
-    def dice_coeff(y_true, y_pred, smooth=1e-9):
-        """ Calculate the dice coefficient.
-
-        Parameters
-        ----------
-        y_true : numpy.ndarray
-            The true masks.
-        y_pred : numpy.ndarray
-            The predicted masks.
-        smooth : float
-            The smoothing factor.
-
-        Returns
-        -------
-        float
-            The dice coefficient.
-        """
-        import tensorflow as tf
-        y_true_flat = tf.reshape(y_true, [-1])
-        y_pred_flat = tf.reshape(y_pred, [-1])
-        intersection = tf.reduce_sum(y_true_flat * y_pred_flat)
-        union = tf.reduce_sum(y_true_flat) + tf.reduce_sum(y_pred_flat)
-        dice = (2. * intersection + smooth) / (union + smooth)
-        return dice
-
-    @staticmethod
-    def bce_dice_loss(y_true, y_pred):
-        """ Calculate the loss.
-        Parameters
-        ----------
-        y_true : numpy.ndarray
-            The true masks.
-        y_pred : numpy.ndarray
-            The predicted masks.
-        Returns
-        -------
-        float
-            The loss.
-        """
-        import tensorflow as tf
-        return tf.keras.losses.binary_crossentropy(y_true, y_pred) + \
-            (1 - Util.dice_coeff(y_true, y_pred))
-
-    @staticmethod
-    def hybrid_loss(y_true, y_pred):
-        """ Calculate the loss.
-
-        Parameters
-        ----------
-        y_true : numpy.ndarray
-            The true masks.
-        y_pred : numpy.ndarray
-            The predicted masks.
-
-        Returns
-        -------
-        float
-            The loss.
-        """
-        import tensorflow as tf
-        from keras_unet_collection import losses
-        # check that the types of both y_true and y_pred are the same
-        y_true = tf.cast(y_true, tf.float32)
-        y_pred = tf.cast(y_pred, tf.float32)
-
-        loss_focal = losses.focal_tversky(y_true, y_pred, alpha=0.5,
-                                          gamma=4 / 3)
-        loss_iou = losses.iou_seg(y_true, y_pred)
-
-        # (x)
-        # loss_ssim = losses.ms_ssim(y_true, y_pred, max_val=1.0, filter_size=4)
-
-        return loss_focal + loss_iou  # +loss_ssim
-
-    @staticmethod
-    def dice_loss(y_true, y_pred, smooth=1):
-        """ Calculate the dice loss.
-
-        Parameters
-        ----------
-        y_true : numpy.ndarray
-            The true masks.
-        y_pred : numpy.ndarray
-            The predicted masks.
-        smooth : float
-            The smoothing factor.
-
-        Returns
-        -------
-        float
-            The dice loss.
-        """
-        return 1 - Util.dice_coeff(y_true, y_pred, smooth)
+import logging
+import os
+import warnings
+
+
+class Util:
+    @staticmethod
+    def disable_tensorflow_logging():
+        import warnings
+        import os
+        os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
+        warnings.filterwarnings('ignore', category=UserWarning,
+                                module='tensorflow')
+        warnings.filterwarnings("ignore", category=DeprecationWarning)
+        warnings.filterwarnings("ignore", category=FutureWarning)
+        import logging
+        import tensorflow as tf
+        logger = tf.get_logger()
+        logger.setLevel(logging.ERROR)
+        from tensorflow.python.keras.utils.generic_utils import \
+            CustomMaskWarning
+        warnings.filterwarnings('ignore', category=CustomMaskWarning)
+
+    @staticmethod
+    def create_A_B_Z_split(images, labels, dataset_size=1000, weights=None):
+        """ Creates A, B, Z split from images and labels
+        Parameters
+        ----------
+        images : numpy array
+            The images to split
+        labels : numpy array
+            The labels to split
+        dataset_size : int
+            The size of the dataset
+        weights : dict
+            The weights to use for the split. If None, the split is 40/40/20
+        Returns
+        -------
+        A : numpy array
+            The A split
+        B : numpy array
+            The B split
+        Z : numpy array
+            The Z split
+        """
+        import numpy as np
+
+        A_split = int(0.4 * dataset_size)
+        B_split = int(0.2 * dataset_size)
+        Z_split = int(0.4 * dataset_size)
+
+        if weights:
+            A_split = int(weights['A'] * dataset_size)
+            B_split = int(weights['B'] * dataset_size)
+            Z_split = int(weights['Z'] * dataset_size)
+
+        # machine data
+        A = images[0:A_split, :, :, 0]
+        A_labels = labels[0:A_split, :, :, 0]
+
+        A = np.stack((A, A_labels), axis=-1)
+
+        # human data
+        B = images[A_split:A_split + B_split, :, :, 0]
+        B_labels = labels[A_split:A_split + B_split, :, :, 0]
+
+        B = np.stack((B, B_labels), axis=-1)
+
+        # we will also provide a Z array that
+        # can be used to funnel additional data later
+
+        # funnel data
+        Z = images[A_split + B_split:A_split + B_split + Z_split, :, :, 0]
+        Z_labels = labels[A_split + B_split:A_split + B_split + Z_split, :, :,
+                   0]
+
+        Z = np.stack((Z, Z_labels), axis=-1)
+
+        return A, B, Z
+
+    @staticmethod
+    def create_train_val_test_split(dataset,
+                                    train_count=200,
+                                    val_count=300,
+                                    test_count=250,
+                                    shuffle=True):
+        """ Creates a train, val, test split from a dataset
+
+        Parameters
+        ----------
+        dataset : numpy array
+            The dataset to split
+        train_count : int
+            The number of training samples
+        val_count : int
+            The number of validation samples
+        test_count : int
+            The number of test samples
+        shuffle : bool
+            Whether to shuffle the dataset before splitting
+
+        Returns
+        -------
+        train : numpy array
+            The training split
+        val : numpy array
+            The validation split
+        test : numpy array
+            The test split
+        """
+        import numpy as np
+        if shuffle:
+            np.random.shuffle(dataset)
+
+        train = dataset[0:train_count]
+        val = dataset[train_count:train_count + val_count]
+        test = dataset[
+               train_count + val_count:train_count + val_count + test_count]
+
+        return train, val, test
+
+    @staticmethod
+    def create_numbered_file(filename, extension):
+        """ Creates a numbered file
+
+        Parameters
+        ----------
+        filename : str
+            The filename
+        extension : str
+            The extension
+
+        Returns
+        -------
+        numbered_file : str
+            The numbered file
+        """
+        number = 0000
+        numbered_file = filename + '_' + str(number) + extension
+        while os.path.exists(numbered_file):
+            number += 1
+            numbered_file = filename + '_' + str(number) + extension
+
+        return numbered_file
+
+    @staticmethod
+    def plot_accuracies(x, y1, y2):
+        """ Plot line chart showing accuracies of classifier and discriminator
+
+        Parameters
+        ----------
+        x : range
+            The range of the x-axis
+        y1 : numpy.ndarray | list
+            The y-axis values for the classifier.
+        y2 : numpy.ndarray | list
+            The y-axis values for the discriminator.
+
+        Returns
+        -------
+        None
+        """
+        import matplotlib.pyplot as plt
+        fig, ax1 = plt.subplots(1, 1, figsize=(3, 3), dpi=80)
+        line1, = ax1.plot(x, y1, color='tab:red', label='Classifier')
+        line2, = ax1.plot(x, y2, color='tab:blue', label='Discriminator')
+        ax1.legend(handles=[line1, line2])
+        ax1.xaxis.set_major_locator(plt.MaxNLocator(integer=True))
+
+        ax1.set_xlabel('Cycle', color='tab:gray', fontsize=14)
+        ax1.tick_params(axis='x', rotation=0, labelsize=12,
+                        labelcolor='tab:gray')
+        ax1.set_ylabel('Accuracy', color='tab:red', fontsize=14)
+        ax1.tick_params(axis='y', rotation=0, labelcolor='tab:red')
+        ax1.grid(alpha=.4)
+        fig.tight_layout()
+        plt.show()
+
+    @staticmethod
+    def dice_coeff(y_true, y_pred, smooth=1e-9):
+        """ Calculate the dice coefficient.
+
+        Parameters
+        ----------
+        y_true : numpy.ndarray
+            The true masks.
+        y_pred : numpy.ndarray
+            The predicted masks.
+        smooth : float
+            The smoothing factor.
+
+        Returns
+        -------
+        float
+            The dice coefficient.
+        """
+        import tensorflow as tf
+        y_true_flat = tf.reshape(y_true, [-1])
+        y_pred_flat = tf.reshape(y_pred, [-1])
+        intersection = tf.reduce_sum(y_true_flat * y_pred_flat)
+        union = tf.reduce_sum(y_true_flat) + tf.reduce_sum(y_pred_flat)
+        dice = (2. * intersection + smooth) / (union + smooth)
+        return dice
+
+    @staticmethod
+    def bce_dice_loss(y_true, y_pred):
+        """ Calculate the loss.
+        Parameters
+        ----------
+        y_true : numpy.ndarray
+            The true masks.
+        y_pred : numpy.ndarray
+            The predicted masks.
+        Returns
+        -------
+        float
+            The loss.
+        """
+        import tensorflow as tf
+        return tf.keras.losses.binary_crossentropy(y_true, y_pred) + \
+            (1 - Util.dice_coeff(y_true, y_pred))
+
+    @staticmethod
+    def hybrid_loss(y_true, y_pred):
+        """ Calculate the loss.
+
+        Parameters
+        ----------
+        y_true : numpy.ndarray
+            The true masks.
+        y_pred : numpy.ndarray
+            The predicted masks.
+
+        Returns
+        -------
+        float
+            The loss.
+        """
+        import tensorflow as tf
+        from keras_unet_collection import losses
+        # check that the types of both y_true and y_pred are the same
+        y_true = tf.cast(y_true, tf.float32)
+        y_pred = tf.cast(y_pred, tf.float32)
+
+        loss_focal = losses.focal_tversky(y_true, y_pred, alpha=0.5,
+                                          gamma=4 / 3)
+        loss_iou = losses.iou_seg(y_true, y_pred)
+
+        # (x)
+        # loss_ssim = losses.ms_ssim(y_true, y_pred, max_val=1.0, filter_size=4)
+
+        return loss_focal + loss_iou  # +loss_ssim
+
+    @staticmethod
+    def dice_loss(y_true, y_pred, smooth=1):
+        """ Calculate the dice loss.
+
+        Parameters
+        ----------
+        y_true : numpy.ndarray
+            The true masks.
+        y_pred : numpy.ndarray
+            The predicted masks.
+        smooth : float
+            The smoothing factor.
+
+        Returns
+        -------
+        float
+            The dice loss.
+        """
+        return 1 - Util.dice_coeff(y_true, y_pred, smooth)
```

### Comparing `gp2-0.5.25.23/gp2.egg-info/SOURCES.txt` & `gp2-0.7.22.23/gp2.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+deepsight/__init__.py
+deepsight/kaggle_sight.py
+deepsight/kaggle_explorer/__init__.py
+deepsight/kaggle_explorer/dicom_copy_machine.py
+deepsight/kaggle_explorer/dicom_data_fixer.py
 gp2/__init__.py
 gp2/__version__.py
 gp2/runner.py
 gp2.egg-info/PKG-INFO
 gp2.egg-info/SOURCES.txt
 gp2.egg-info/dependency_links.txt
 gp2.egg-info/requires.txt
 gp2.egg-info/top_level.txt
 gp2/data/__init__.py
 gp2/data/collection.py
+gp2/data/data_converter.py
 gp2/data/manager.py
 gp2/data/point.py
 gp2/gp2/__init__.py
 gp2/gp2/util.py
 gp2/gp2/classifiers/__init__.py
 gp2/gp2/classifiers/base_keras_segmentation_classifier.py
 gp2/gp2/classifiers/classifier.py
```

### Comparing `gp2-0.5.25.23/setup.py` & `gp2-0.7.22.23/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-from gp2.__version__ import __version__
+from gp2 import __version__
 
 setup(
     name='gp2',
     version=__version__,
     url='https://github.com/RyanZurrin/CS410-GP2',
     description='A framework for tuning segmentation classifiers and '
                 'discriminators',
```

