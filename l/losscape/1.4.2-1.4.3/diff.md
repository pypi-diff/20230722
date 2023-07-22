# Comparing `tmp/losscape-1.4.2.tar.gz` & `tmp/losscape-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.4.2.tar", last modified: Fri Jul 21 13:44:15 2023, max compression
+gzip compressed data, was "losscape-1.4.3.tar", last modified: Sat Jul 22 07:48:33 2023, max compression
```

## Comparing `losscape-1.4.2.tar` & `losscape-1.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:44:15.164334 losscape-1.4.2/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-21 13:44:15.164334 losscape-1.4.2/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.4.2/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:44:15.160334 losscape-1.4.2/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.4.2/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.4.2/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.4.2/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15961 2023-07-21 07:27:43.000000 losscape-1.4.2/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.4.2/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 13:44:15.164334 losscape-1.4.2/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 13:44:15.000000 losscape-1.4.2/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 13:44:15.164334 losscape-1.4.2/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      588 2023-07-21 13:44:09.000000 losscape-1.4.2/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 07:48:33.963505 losscape-1.4.3/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 07:48:33.963505 losscape-1.4.3/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.4.3/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 07:48:33.959505 losscape-1.4.3/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.4.3/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.4.3/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.4.3/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16275 2023-07-22 07:47:06.000000 losscape-1.4.3/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.4.3/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 07:48:33.963505 losscape-1.4.3/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 07:48:33.000000 losscape-1.4.3/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-22 07:48:33.000000 losscape-1.4.3/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-22 07:48:33.000000 losscape-1.4.3/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-22 07:48:33.000000 losscape-1.4.3/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-22 07:48:33.000000 losscape-1.4.3/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-22 07:48:33.963505 losscape-1.4.3/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      588 2023-07-22 07:47:46.000000 losscape-1.4.3/setup.py
```

### Comparing `losscape-1.4.2/PKG-INFO` & `losscape-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.4.2
+Version: 1.4.3
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.4.2/README.md` & `losscape-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `losscape-1.4.2/losscape/compute_loss.py` & `losscape-1.4.3/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.2/losscape/create_directions.py` & `losscape-1.4.3/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.2/losscape/create_landscape.py` & `losscape-1.4.3/losscape/create_landscape.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import torch
 
 import math
 import numpy as np
 from scipy import interpolate
 import matplotlib.pyplot as plt
 import h5py
+import os
 
 from losscape.compute_loss import compute_loss
 from losscape.create_directions import create_random_direction, create_random_directions
 
 #todo : plot anim la traj d'une optim avec PCA
 #todo : losscape avec le test loss
 #todo pour la lib : possiblité de tout foutre dans un fichier, et il fait les exps automatiquement ? (genre on met model + dataloader + optim + loss et il loop sur les models + optims)
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 
-def create_2D_losscape(model, train_loader_unshuffled, direction=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '1d_losscape.png', x_min:float=-1., x_max:float=1., num_points:int=50):
+def create_2D_losscape(model, train_loader_unshuffled, direction=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '', x_min:float=-1., x_max:float=1., num_points:int=50):
     """
     Create a 2D losscape of the given model.
 
     Parameters
     ----------
     model : the torch model which will be used to create the losscape.
     train_loader_unshuffled : the torch dataloader. It is supposed to be fixed so that all the calls to this function will use the same data.
     optimizer : the optimizer used for training (should follow the same API as torch optimizers).(default to Adam)
     criterion : the criterion used to compute the loss. (default to F.cross_entropy)
     num_batches : number of batches to evaluate the model with. (default to 8)
     save_only : only save the plot and don't display it. (default to False)
-    output_path : path where the plot will be saved. (default to '1d_losscape.png')
+    output_path : path where the plot will be saved. (default to '2d_losscape.png')
     x_min : min x value (that multiply the sampled direction). (default to -1.) 
     x_max : max x value (that multiply the sampled direction). (default to 1.)
     num_points : number of points to evaluate the loss, from x_min to x_max. (default to 50)
 
     Returns
     ----------
     coords : numpy array containing the x coords used to create the landscape
@@ -54,36 +55,36 @@
 
         loss = compute_loss(model, train_loader_unshuffled, criterion, num_batches)
         losses.append(loss)
 
     _reset_weights(model, init_weights)
     
     plt.plot(coords, losses)
-    plt.savefig(output_path, dpi=300)
+    plt.savefig(os.path.join(output_path, '2d_losscape.png'), dpi=300)
 
     if not save_only:
         plt.show()
     
     plt.clf()
 
     return coords, losses
 
-def create_3D_losscape(model, train_loader_unshuffled, directions=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '2d_losscape.png', output_vtp:bool = False, output_h5:bool = True, log_vtp:bool = True, x_min:float=-1., x_max:float=1., y_min:float=-1., y_max:float=1., num_points:int=50):
+def create_3D_losscape(model, train_loader_unshuffled, directions=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '', output_vtp:bool = False, output_h5:bool = True, log_vtp:bool = True, x_min:float=-1., x_max:float=1., y_min:float=-1., y_max:float=1., num_points:int=50):
     """
     Create a 3D losscape of the given model.
 
     Parameters
     ----------
     model : the torch model which will be used to create the losscape.
     train_loader_unshuffled : the torch dataloader. It is supposed to be fixed so that all the calls to this function will use the same data.
     optimizer : the optimizer used for training (should follow the same API as torch optimizers).(default to Adam)
     criterion : the criterion used to compute the loss. (default to F.cross_entropy)
     num_batches : number of batches to evaluate the model with. (default to 8)
     save_only : only save the plot and don't display it. (default to False)
-    output_path : path where the plot will be saved. (default to '1d_losscape.png')
+    output_path : path where the plot will be saved. (default to '3d_losscape.png')
     output_vpt : whether or not to also create a .vtp file, used to 3D visualize the losscape. (default to False)
     output_h5 : whether or not to also create a .h5 file, containing the data generated by this function (default to True)
     log_vtp : whether or not to visualize log values of loss in the vtp file (default to True)
     x_min : min x value (that multiply the first sampled direction). (default to -1.) 
     x_max : max x value (that multiply the first sampled direction). (default to 1.)
     y_min : min x value (that multiply the second sampled direction). (default to -1.) 
     y_max : max x value (that multiply the second sampled direction). (default to 1.)
@@ -107,37 +108,44 @@
         directions = create_random_directions(model)
 
     init_weights = [p.data for p in model.parameters()]
 
     X, Y = np.meshgrid(np.linspace(x_min, x_max, num_points), np.linspace(y_min, y_max, num_points))
     losses = np.empty_like(X)
 
+    count = 0
+    total = X.shape[0] * X.shape[1]
+
     for i in range(X.shape[0]):
         for j in range(X.shape[1]):
             _set_weights(model, init_weights, directions, np.array([X[i, j], Y[i, j]]))
 
             loss = compute_loss(model, train_loader_unshuffled, criterion, num_batches)
             losses[i, j] = loss
 
+            count += 1
+            if count%(total/10) == 0:
+                print("{}%".format(count/total * 100.))
+
     _reset_weights(model, init_weights)
 
     cp = plt.contour(X, Y, losses, cmap='summer')
     plt.clabel(cp, inline=1, fontsize=8)
-    plt.savefig(output_path, dpi=300)
-
+    plt.savefig(os.path.join(output_path, '3d_losscape.png'), dpi=300)
+    
     if not save_only:
         plt.show()
     
     plt.clf()
 
     if output_vtp:
-        _create_vtp(X, Y, losses, log=log_vtp)
+        _create_vtp(X, Y, losses, log=log_vtp, output_path=output_path)
 
     if output_h5:
-        with h5py.File('data.h5', 'w') as hf:
+        with h5py.File(os.path.join(output_path, 'data.h5'), 'w') as hf:
             hf.create_dataset("X", data=X)
             hf.create_dataset("Y", data=Y)
             hf.create_dataset("losses", data=losses)
 
     return X, Y, losses
 
 def _set_weights(model, weights, directions, step):
@@ -153,15 +161,15 @@
         p.data = w + d
 
 def _reset_weights(model, weights):
     for (p, w) in zip(model.parameters(), weights):
         p.data.copy_(w.type(type(p.data)))
 
 # as in https://github.com/tomgoldstein/loss-landscape
-def _create_vtp(X, Y, losses, log=False, zmax=-1, interp=-1):
+def _create_vtp(X, Y, losses, log=False, zmax=-1, interp=-1, output_path=''):
     #set this to True to generate points
     show_points = False
     #set this to True to generate polygons
     show_polys = True
 
     xcoordinates = X
     ycoordinates = Y
@@ -178,15 +186,15 @@
         y_array = np.linspace(min(y_array), max(y_array), interp)
         z_array = m(x_array, y_array).ravel()
 
         x_array, y_array = np.meshgrid(x_array, y_array)
         x_array = x_array.ravel()
         y_array = y_array.ravel()
 
-    vtp_file = 'losscape'
+    vtp_file = os.path.join(output_path, 'losscape')
     if zmax > 0:
         z_array[z_array > zmax] = zmax
         vtp_file +=  "_zmax=" + str(zmax)
 
     if log:
         z_array = np.log(z_array + 0.1)
         vtp_file +=  "_log"
```

### Comparing `losscape-1.4.2/losscape/train.py` & `losscape-1.4.3/losscape/train.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.2/losscape.egg-info/PKG-INFO` & `losscape-1.4.3/losscape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.4.2
+Version: 1.4.3
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.4.2/setup.py` & `losscape-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 current_dir = Path(__file__).parent
 desc = (current_dir / "README.md").read_text()
 
 setup(
     name='losscape',
-    version='1.4.2',
+    version='1.4.3',
     url='https://github.com/Procuste34/losscape',
     author='Alexandre TL',
     author_email='alexandretl3434@gmail.com',
     description='Visualize easily the loss landscape of your neural networks',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

