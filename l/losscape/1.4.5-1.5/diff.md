# Comparing `tmp/losscape-1.4.5.tar.gz` & `tmp/losscape-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.4.5.tar", last modified: Sat Jul 22 09:13:33 2023, max compression
+gzip compressed data, was "losscape-1.5.tar", last modified: Sat Jul 22 17:56:18 2023, max compression
```

## Comparing `losscape-1.4.5.tar` & `losscape-1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 09:13:33.168268 losscape-1.4.5/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 09:13:33.168268 losscape-1.4.5/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.4.5/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 09:13:33.168268 losscape-1.4.5/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.4.5/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.4.5/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.4.5/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16226 2023-07-22 07:56:43.000000 losscape-1.4.5/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.4.5/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 09:13:33.168268 losscape-1.4.5/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-22 09:13:33.000000 losscape-1.4.5/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-22 09:13:33.168268 losscape-1.4.5/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      596 2023-07-22 09:13:26.000000 losscape-1.4.5/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 17:56:18.597458 losscape-1.5/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3583 2023-07-22 17:56:18.597458 losscape-1.5/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.5/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 17:56:18.597458 losscape-1.5/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.5/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1708 2023-07-22 17:55:05.000000 losscape-1.5/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.5/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16290 2023-07-22 17:53:16.000000 losscape-1.5/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.5/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 17:56:18.597458 losscape-1.5/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3583 2023-07-22 17:56:18.000000 losscape-1.5/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-22 17:56:18.000000 losscape-1.5/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-22 17:56:18.000000 losscape-1.5/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-07-22 17:56:18.000000 losscape-1.5/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-22 17:56:18.000000 losscape-1.5/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-22 17:56:18.597458 losscape-1.5/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      594 2023-07-22 17:56:11.000000 losscape-1.5/setup.py
```

### Comparing `losscape-1.4.5/PKG-INFO` & `losscape-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.4.5
+Version: 1.5
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.4.5/README.md` & `losscape-1.5/README.md`

 * *Files identical despite different names*

### Comparing `losscape-1.4.5/losscape/create_directions.py` & `losscape-1.5/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.5/losscape/create_landscape.py` & `losscape-1.5/losscape/create_landscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 #todo : plot anim la traj d'une optim avec PCA
 #todo : losscape avec le test loss
 #todo pour la lib : possiblité de tout foutre dans un fichier, et il fait les exps automatiquement ? (genre on met model + dataloader + optim + loss et il loop sur les models + optims)
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 
-def create_2D_losscape(model, train_loader_unshuffled, direction=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '', x_min:float=-1., x_max:float=1., num_points:int=50):
+def create_2D_losscape(model, train_loader_unshuffled=None, get_batch=None, direction=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '', x_min:float=-1., x_max:float=1., num_points:int=50):
     """
     Create a 2D losscape of the given model.
 
     Parameters
     ----------
     model : the torch model which will be used to create the losscape.
     train_loader_unshuffled : the torch dataloader. It is supposed to be fixed so that all the calls to this function will use the same data.
@@ -49,30 +49,30 @@
 
     coords = np.linspace(x_min, x_max, num_points)
     losses = []
 
     for x in coords:
         _set_weights(model, init_weights, direction, x)
 
-        loss = compute_loss(model, train_loader_unshuffled, criterion, num_batches)
+        loss = compute_loss(model, train_loader_unshuffled, get_batch, criterion, num_batches)
         losses.append(loss)
 
     _reset_weights(model, init_weights)
     
     plt.plot(coords, losses)
     plt.savefig(os.path.join(output_path, '2d_losscape.png'), dpi=300)
 
     if not save_only:
         plt.show()
     
     plt.clf()
 
     return coords, losses
 
-def create_3D_losscape(model, train_loader_unshuffled, directions=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '', output_vtp:bool = False, output_h5:bool = True, x_min:float=-1., x_max:float=1., y_min:float=-1., y_max:float=1., num_points:int=50):
+def create_3D_losscape(model, train_loader_unshuffled=None, get_batch=None, directions=None, criterion = None, num_batches:int = 8, save_only:bool = False, output_path:str = '', output_vtp:bool = False, output_h5:bool = True, x_min:float=-1., x_max:float=1., y_min:float=-1., y_max:float=1., num_points:int=50):
     """
     Create a 3D losscape of the given model.
 
     Parameters
     ----------
     model : the torch model which will be used to create the losscape.
     train_loader_unshuffled : the torch dataloader. It is supposed to be fixed so that all the calls to this function will use the same data.
@@ -114,15 +114,15 @@
     count = 0
     total = X.shape[0] * X.shape[1]
 
     for i in range(X.shape[0]):
         for j in range(X.shape[1]):
             _set_weights(model, init_weights, directions, np.array([X[i, j], Y[i, j]]))
 
-            loss = compute_loss(model, train_loader_unshuffled, criterion, num_batches)
+            loss = compute_loss(model, train_loader_unshuffled, get_batch, criterion, num_batches)
             losses[i, j] = loss
 
             count += 1
             if count%(total/10) == 0:
                 print("{}%".format(count/total * 100.))
 
     _reset_weights(model, init_weights)
```

### Comparing `losscape-1.4.5/losscape/train.py` & `losscape-1.5/losscape/train.py`

 * *Files identical despite different names*

### Comparing `losscape-1.4.5/losscape.egg-info/PKG-INFO` & `losscape-1.5/losscape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.4.5
+Version: 1.5
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.4.5/setup.py` & `losscape-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 current_dir = Path(__file__).parent
 desc = (current_dir / "README.md").read_text()
 
 setup(
     name='losscape',
-    version='1.4.5',
+    version='1.5',
     url='https://github.com/Procuste34/losscape',
     author='Alexandre TL',
     author_email='alexandretl3434@gmail.com',
     description='Visualize easily the loss landscape of your neural networks',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

