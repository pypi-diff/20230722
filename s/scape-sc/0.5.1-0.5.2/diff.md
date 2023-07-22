# Comparing `tmp/scape-sc-0.5.1.tar.gz` & `tmp/scape-sc-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scape-sc-0.5.1.tar", last modified: Sun Feb 19 04:02:47 2023, max compression
+gzip compressed data, was "/home/liyuzhe/Notebook/SCAPE_v5/code/dist/.tmp-rtae_bpt/scape-sc-0.5.2.tar", last modified: Sat Jul 22 08:01:58 2023, max compression
```

## Comparing `scape-sc-0.5.1.tar` & `scape-sc-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 liyuzhe    (501) staff       (20)        0 2023-02-19 04:02:47.147940 scape-sc-0.5.1/
--rw-rw-r--   0 liyuzhe    (501) staff       (20)     1065 2022-04-21 10:34:47.000000 scape-sc-0.5.1/LICENSE
--rw-r--r--   0 liyuzhe    (501) staff       (20)     1201 2023-02-19 04:02:47.147824 scape-sc-0.5.1/PKG-INFO
--rw-rw-r--   0 liyuzhe    (501) staff       (20)      523 2023-02-13 04:43:02.000000 scape-sc-0.5.1/README.md
--rw-r--r--   0 liyuzhe    (501) staff       (20)     1074 2023-02-19 03:59:22.000000 scape-sc-0.5.1/pyproject.toml
--rw-r--r--   0 liyuzhe    (501) staff       (20)       38 2023-02-19 04:02:47.147978 scape-sc-0.5.1/setup.cfg
-drwxr-xr-x   0 liyuzhe    (501) staff       (20)        0 2023-02-19 04:02:47.145360 scape-sc-0.5.1/src/
-drwxr-xr-x   0 liyuzhe    (501) staff       (20)        0 2023-02-19 04:02:47.146985 scape-sc-0.5.1/src/scape/
--rw-rw-r--   0 liyuzhe    (501) staff       (20)      110 2023-02-19 04:00:47.000000 scape-sc-0.5.1/src/scape/__init__.py
--rw-r--r--   0 liyuzhe    (501) staff       (20)     6188 2023-02-19 04:01:25.000000 scape-sc-0.5.1/src/scape/function.py
--rw-r--r--   0 liyuzhe    (501) staff       (20)      718 2023-02-13 03:23:02.000000 scape-sc-0.5.1/src/scape/loss.py
--rw-r--r--   0 liyuzhe    (501) staff       (20)     4420 2023-02-13 03:13:48.000000 scape-sc-0.5.1/src/scape/model.py
--rw-r--r--   0 liyuzhe    (501) staff       (20)     5483 2023-02-13 03:24:58.000000 scape-sc-0.5.1/src/scape/train.py
-drwxr-xr-x   0 liyuzhe    (501) staff       (20)        0 2023-02-19 04:02:47.147679 scape-sc-0.5.1/src/scape_sc.egg-info/
--rw-r--r--   0 liyuzhe    (501) staff       (20)     1201 2023-02-19 04:02:47.000000 scape-sc-0.5.1/src/scape_sc.egg-info/PKG-INFO
--rw-r--r--   0 liyuzhe    (501) staff       (20)      311 2023-02-19 04:02:47.000000 scape-sc-0.5.1/src/scape_sc.egg-info/SOURCES.txt
--rw-r--r--   0 liyuzhe    (501) staff       (20)        1 2023-02-19 04:02:47.000000 scape-sc-0.5.1/src/scape_sc.egg-info/dependency_links.txt
--rw-r--r--   0 liyuzhe    (501) staff       (20)      186 2023-02-19 04:02:47.000000 scape-sc-0.5.1/src/scape_sc.egg-info/requires.txt
--rw-r--r--   0 liyuzhe    (501) staff       (20)        6 2023-02-19 04:02:47.000000 scape-sc-0.5.1/src/scape_sc.egg-info/top_level.txt
+drwxr-x---   0 liyuzhe   (7189) zhangqflab  (9018)        0 2023-07-22 08:01:58.724934 scape-sc-0.5.2/
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)     1065 2023-07-22 07:52:54.000000 scape-sc-0.5.2/LICENSE
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)     1201 2023-07-22 08:01:58.724934 scape-sc-0.5.2/PKG-INFO
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)      523 2023-07-22 07:52:54.000000 scape-sc-0.5.2/README.md
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)      997 2023-07-22 07:52:54.000000 scape-sc-0.5.2/pyproject.toml
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)       38 2023-07-22 08:01:58.724934 scape-sc-0.5.2/setup.cfg
+drwxr-x---   0 liyuzhe   (7189) zhangqflab  (9018)        0 2023-07-22 08:01:58.724934 scape-sc-0.5.2/src/
+drwxr-x---   0 liyuzhe   (7189) zhangqflab  (9018)        0 2023-07-22 08:01:58.724934 scape-sc-0.5.2/src/scape/
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)      110 2023-07-22 07:53:10.000000 scape-sc-0.5.2/src/scape/__init__.py
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)     4991 2023-07-22 07:53:10.000000 scape-sc-0.5.2/src/scape/function.py
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)     1075 2023-07-22 07:53:10.000000 scape-sc-0.5.2/src/scape/loss.py
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)     4945 2023-07-22 07:53:10.000000 scape-sc-0.5.2/src/scape/model.py
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)     5578 2023-07-22 07:53:10.000000 scape-sc-0.5.2/src/scape/train.py
+drwxr-x---   0 liyuzhe   (7189) zhangqflab  (9018)        0 2023-07-22 08:01:58.724934 scape-sc-0.5.2/src/scape_sc.egg-info/
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)     1201 2023-07-22 08:01:58.000000 scape-sc-0.5.2/src/scape_sc.egg-info/PKG-INFO
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)      311 2023-07-22 08:01:58.000000 scape-sc-0.5.2/src/scape_sc.egg-info/SOURCES.txt
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)        1 2023-07-22 08:01:58.000000 scape-sc-0.5.2/src/scape_sc.egg-info/dependency_links.txt
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)      122 2023-07-22 08:01:58.000000 scape-sc-0.5.2/src/scape_sc.egg-info/requires.txt
+-rw-r-----   0 liyuzhe   (7189) zhangqflab  (9018)        6 2023-07-22 08:01:58.000000 scape-sc-0.5.2/src/scape_sc.egg-info/top_level.txt
```

### Comparing `scape-sc-0.5.1/LICENSE` & `scape-sc-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scape-sc-0.5.1/PKG-INFO` & `scape-sc-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scape-sc
-Version: 0.5.1
+Version: 0.5.2
 Summary: Single-Cell data Analysis via Perturbation Estimation
 Author-email: Yuzhe Li <liyuzhezju@gmail.com>
 Project-URL: Homepage, https://github.com/ericli0419/SCAPE
 Project-URL: Bug Tracker, https://github.com/ericli0419/SCAPE/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scape-sc-0.5.1/README.md` & `scape-sc-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `scape-sc-0.5.1/pyproject.toml` & `scape-sc-0.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42.0","wheel","build","packaging","tomli"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scape-sc"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Yuzhe Li", email="liyuzhezju@gmail.com" },
 ]
 description = "Single-Cell data Analysis via Perturbation Estimation"
 readme = "README.md"
 requires-python = ">3.6.0"
 classifiers = [
@@ -20,22 +20,20 @@
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 dependencies = [
     "build",
     "packaging",
     "pyparsing",
     "tomli",
-    "numpy>=1.17.2",
-    "pandas>=0.25.1",
-    "scipy>=1.3.1",
-    "scikit-learn>=0.22.1",
+    "numpy",
+    "pandas",
+    "scipy",
+    "scikit-learn",
     "scanpy>=1.4.5",
     "tqdm>=4.28.1",
-    "matplotlib>=3.0.3",
-    "seaborn>=0.9.0",
     "leidenalg>=0.8.3",
     "scvelo>=0.2.4"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ericli0419/SCAPE"
-"Bug Tracker" = "https://github.com/ericli0419/SCAPE/issues"
+"Bug Tracker" = "https://github.com/ericli0419/SCAPE/issues"
```

### Comparing `scape-sc-0.5.1/src/scape/function.py` & `scape-sc-0.5.2/src/scape/function.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,52 +6,45 @@
 @author: liyuzhe
 """
 import os
 import random
 import pandas as pd
 import numpy as np
 import scanpy as sc
+import scipy as sci
 import scvelo as scv
 import torch
 
-from .model import VAE
-from .train import train
+from model import VAE
+from train import train
 
 
 
-def SCAPE(adata,adata_raw,genes,perturbation='KO',epoch=1000,lr=0.0005,patience=10,seed=42,GPU=0,batch_size=128,n_jobs=1,a=50,outdir='./',verbose=False):
+def SCAPE(adata,adata_raw,genes,perturbation='KO',epoch=1000,lr=0.0005,patience=10,seed=9,GPU=0,batch_size=128,n_jobs=1,a=0.9,outdir='./',verbose=False):
     """
-    Single-Cell data Analysis via Perturbation Estimation
+    Single-Cell integrative Analysis via Latent feature Extraction
     
     Parameters
     ----------
     adata
-        An AnnData Object with cell x gene matrix stored.
-    adata_raw
-        An AnnData Object with cell x gene matrix stored.
-    genes
-        The list of genes for in silico genetic perturbation.
-    perturbation
-        The type of perturbation, including KO, KD, and OE. 
+        An AnnData Object with spot/cell x gene matrix stored.
+    k
+        The number cells consider when constructing Adjacency Matrix. Default: 20.
+    alpha
+        The relative ratio of reconstruction loss of Adjacency Matrix. Default: 0.05 (0.5 was recommanded for Visium data's domain finding).
     lr
-        Learning rate. Default: 5e-4.
+        Learning rate. Default: 2e-4.
     patience
-        Patience in early stopping. Default: 10.
+        Patience in early stopping. Default: 50.
     epoch
-        Max epochs for training. Default: 1000.
-    seed
-        Random seed. Default: 42. 
+        Max iterations for training. Default: 2000.
+    loss_type
+        Loss Function of feature matrix reconstruction loss. Default: MSE (BCE was recommanded for Visium data's domain finding). 
     GPU
         Index of GPU to use if GPU is available. Default: 0.
-    batch_size
-        Number of samples of each batch in training.
-    n_jobs
-        Number of CPUs.
-    a
-        The ratio of reconstruction loss.
     outdir
         Output directory. Default: '.'.
     verbose
         Verbosity, True or False. Default: False.
     
     
     Returns
@@ -63,23 +56,25 @@
     checkpoint
         model.pt contains the variables of the model.
     """
     
     np.random.seed(seed) 
     torch.manual_seed(seed)
     random.seed(seed)
-    
     os.makedirs(outdir, exist_ok=True)
+
+    adata.var["cond_genes"]=False
+    adata.var["cond_genes"].loc[genes]=True
+    cond = torch.from_numpy(adata.layers["velocity"][:,adata.var["cond_genes"]].astype(np.float32).copy())
+
     for i in genes:
         if i in list(adata.var[adata.var["velocity_genes"]].index):
             adata.var['velocity_genes'][[i]]=False
-    # adata.var['velocity_genes'][genes]=False
     velocity_genes=adata.var[adata.var["velocity_genes"]].index.copy()
     
-    cond = torch.from_numpy(adata_raw[:,genes].X.A.astype(np.float32).copy())
     data = torch.from_numpy(adata_raw[:, velocity_genes].X.A.astype(np.float32).copy())
     vel = torch.from_numpy(adata.layers["velocity"][:, adata.var["velocity_genes"]].astype(np.float32).copy())
     
     x_dim=data.shape[1]
     c_dim=cond.shape[1]
     
     model=VAE(x_dim, c_dim)
@@ -100,60 +95,37 @@
     
     latent_g = model.predict(data,out='z_p') 
     adata.obsm['latent_g']=latent_g.copy()
 
     if perturbation=='KO':
         recon_x = model.predict(data,out='x',device=device) 
         recon_x_ = model.predict_ko(data,device=device)
-      
-        adata.layers['velocity_scvelo']=adata.layers['velocity'].copy()
         
+        adata.layers['velocity_scvelo']=adata.layers['velocity'].copy()
         gene_subset=adata.var["velocity_genes"]
-        
         adata.layers['velocity_scape_unp'] = np.ones(adata.shape) * np.nan
         adata.layers['velocity_scape_unp'][:, gene_subset] = recon_x.copy()
         adata.layers['velocity_scape'] = np.ones(adata.shape) * np.nan
         adata.layers['velocity_scape'][:, gene_subset] = recon_x_.copy()
         velocity_delta = adata.layers['velocity_scape']-adata.layers['velocity_scape_unp']
         adata.layers['velocity_delta']=velocity_delta.copy()
 
     elif perturbation=='OE':
         recon_x = model.predict(data, out='x',device=device) 
-
-        df=pd.DataFrame(adata_raw[:,genes].X.A,index=adata.obs.index,columns=genes)
-        idx=df.sort_values(by=genes,ascending=False).index[:int(adata.shape[0] * 0.01)]
-        z_p = torch.from_numpy(adata[idx].obsm['latent_g'].mean(axis=0)).float().repeat(adata.shape[0],1)
-        recon_x_ = model.predict_oe(data,z_p,device=device) 
+        recon_x_ = model.predict_oe(data,device=device) 
         
         adata.layers['velocity_scvelo']=adata.layers['velocity'].copy()
         gene_subset=adata.var["velocity_genes"]
         adata.layers['velocity_scape_unp'] = np.ones(adata.shape) * np.nan
         adata.layers['velocity_scape_unp'][:, gene_subset] = recon_x.copy()
         adata.layers['velocity_scape'] = np.ones(adata.shape) * np.nan
         adata.layers['velocity_scape'][:, gene_subset] = recon_x_.copy()
         velocity_delta = adata.layers['velocity_scape']-adata.layers['velocity_scape_unp']
         adata.layers['velocity_delta']=velocity_delta.copy()
 
-    elif perturbation=='KD':
-        recon_x = model.predict(data, out='x',device=device) 
-
-        df=pd.DataFrame(adata_raw[:,genes].X.A,index=adata.obs.index,columns=genes)
-        idx=df[df[genes]==0].index
-        z_p = torch.from_numpy(adata[idx].obsm['latent_g'].mean(axis=0)).float().repeat(adata.shape[0],1)
-        recon_x_ = model.predict_oe(data,z_p,device=device) 
-        
-        adata.layers['velocity_scvelo']=adata.layers['velocity'].copy()
-        gene_subset=adata.var["velocity_genes"]
-        adata.layers['velocity_scape_unp'] = np.ones(adata.shape) * np.nan
-        adata.layers['velocity_scape_unp'][:, gene_subset] = recon_x.copy()
-        adata.layers['velocity_scape'] = np.ones(adata.shape) * np.nan
-        adata.layers['velocity_scape'][:, gene_subset] = recon_x_.copy()
-        velocity_delta = adata.layers['velocity_scape']-adata.layers['velocity_scape_unp']
-        adata.layers['velocity_delta']=velocity_delta.copy()
-    
     adata.layers['velocity']=adata.layers['velocity_scape'].copy()
     scv.tl.velocity_graph(adata,n_jobs=n_jobs)
 
     #Output
     adata.write(os.path.join(outdir,'adata.h5ad'))   
     
     return adata
```

### Comparing `scape-sc-0.5.1/src/scape/model.py` & `scape-sc-0.5.2/src/scape/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,32 +5,43 @@
 
 @author: liyuzhe
 """
 import torch
 import torch.nn as nn
 
 
+class weightConstraint(object):
+    def __init__(self):
+        pass
+    
+    def __call__(self,module):
+        if hasattr(module,'weight'):
+            w=module.weight.data
+            w=w.clamp(min=0)
+            module.weight.data=w
+            
+
 class VAE(nn.Module):
     def __init__(self, x_dim, c_dim):
         super(VAE, self).__init__() 
+        constraints=weightConstraint()
         
         # encoder layer
         self.e_fc1 = self.fc_layer(x_dim, 1024,activation=3)
         self.e_fc2 = self.fc_layer(1024, 128,activation=3)
         
         self.mu_enc = nn.Linear(128, 10)
         self.var_enc = nn.Linear(128, 10)
         self.g_enc = nn.Linear(128, 10)
-        
+
 
         # decoder layer
-        self.d_fc1 = self.fc_layer(10, 128,activation=3)
-        self.d_fc2 = self.fc_layer(128, 1024,activation=3)
-        self.d_fc3 = self.fc_layer(1024, x_dim, activation=2)
-        self.d_fc4 = self.fc_layer(10, c_dim, activation=1)
+        self.d_fc1 = self.fc_layer(10, x_dim, activation=2)
+        self.d_fc2 = self.fc_layer(10, c_dim, activation=6)
+        self.d_fc2.apply(constraints)
 
 
     def reparameterize(self, mu, log_var):
         # vae reparameterization trick
         std = torch.exp(0.5*log_var)
         eps = torch.randn_like(std)
         
@@ -59,16 +70,16 @@
         
         return mu, log_var, g
       
     
     def decoder(self, z, g):
         # z_g = torch.cat((z,g),dim=1)
         z_g=z+g
-        recon_x= self.d_fc3(self.d_fc2(self.d_fc1(z_g)))
-        recon_g = self.d_fc4(g)
+        recon_x = self.d_fc1(z_g)
+        recon_g = self.d_fc2(g)
        
         return recon_x,recon_g
  
     
     def fc_layer(self, in_dim, out_dim, activation=0):
         if activation == 1:
             layer = nn.Sequential(
@@ -76,24 +87,40 @@
                 nn.ReLU())
         elif activation == 2:
             layer = nn.Sequential(
                 nn.Linear(in_dim, out_dim))
         elif activation == 3:
             layer = nn.Sequential(
                 nn.Linear(in_dim, out_dim),
+                # nn.Dropout(0.3),
                 nn.BatchNorm1d(out_dim),
                 nn.LeakyReLU())
-        
+        elif activation == 4:
+            layer = nn.Sequential(
+                nn.Linear(in_dim, out_dim),
+                nn.Sigmoid())
+        elif activation == 5:
+            layer = nn.Sequential(
+                nn.Linear(in_dim, out_dim,bias=False),
+                nn.ReLU())
+        elif activation == 6:
+            layer = nn.Sequential(
+                nn.Linear(in_dim, out_dim,bias=False))
+        elif activation == 7:
+            layer = nn.Sequential(
+                nn.Linear(in_dim, out_dim),
+                nn.Tanh())
         return layer  
     
     def predict(self, data, device='cuda', out='z'):
         x = data.float().to(device)
         
         mu, log_var, g = self.encoder(x)
-        z = self.reparameterize(mu, log_var)
+        # z = self.reparameterize(mu, log_var)
+        z = mu
         # g_0 = torch.zeros_like(g)
         
         if out == 'latent':
             z_g=z+g
             output=z_g.detach().cpu().data.numpy()
         elif out == 'z':
             output=z.detach().cpu().data.numpy()
@@ -104,47 +131,40 @@
             output = recon_x.detach().cpu().data.numpy()
         elif out == 'g':
             recon_x, recon_g = self.decoder(z,g)
             output = recon_g.detach().cpu().data.numpy()
         return output
     
     
-    def predict_oe(self, data, z_p, device='cuda'):
+    def predict_oe(self, data, device='cuda'):
         x = data.float().to(device)
         mu, log_var,g = self.encoder(x)
-        z = self.reparameterize(mu, log_var)
-        z_p = z_p.float().to(device)
+        # z = self.reparameterize(mu, log_var)
+        z = mu
+        g_0 = torch.ones_like(g)
         
-        recon_x, recon_g = self.decoder(z,z_p)
+        recon_x, recon_g = self.decoder(z,g_0)
+        # recon_x, recon_g = self.decoder(z,z_p)
         output = recon_x.detach().cpu().data.numpy()
         
         return output
 
     def predict_ko(self, data, device='cuda'):
         x = data.float().to(device)
         mu, log_var,g = self.encoder(x)
-        z = self.reparameterize(mu, log_var)
-        g_0 = torch.zeros_like(g)
+        # z = self.reparameterize(mu, log_var)
+        z = mu
+        # g_0 = torch.zeros_like(g)
+        g_0 = -1*torch.ones_like(g)
         
         recon_x, recon_g = self.decoder(z,g_0)
         output = recon_x.detach().cpu().data.numpy()
         
         return output
-    
-    def predict_kd(self, data, z_p, device='cuda'):
-        x = data.float().to(device)
-        mu, log_var,g = self.encoder(x)
-        z = self.reparameterize(mu, log_var)
-        z_p = z_p.float().to(device)
-        
-        recon_x, recon_g = self.decoder(z,z_p)
-        output = recon_x.detach().cpu().data.numpy()
         
-        return output
-    
     
     def load_model(self, path):
         pretrained_dict = torch.load(path, map_location=lambda storage, loc: storage)
         model_dict = self.state_dict()
         pretrained_dict = {k: v for k, v in pretrained_dict.items() if k in model_dict}
         model_dict.update(pretrained_dict) 
         self.load_state_dict(model_dict)
```

### Comparing `scape-sc-0.5.1/src/scape/train.py` & `scape-sc-0.5.2/src/scape/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import torch
 from torch.utils.data import DataLoader
 from torch.autograd import Variable
 import numpy as np
 from tqdm.auto import tqdm
 import matplotlib.pyplot as plt
-from .loss import compute_mmd, mse_loss
+from loss import compute_mmd, mse_loss, binary_cross_entropy,kl_divergence
 import random
 
       
 
 def adjust_learning_rate(init_lr, optimizer, iteration,seperation):
     lr = max(init_lr * (0.9 ** (iteration//seperation)), 0.0001)
     for param_group in optimizer.param_groups:
@@ -73,15 +73,15 @@
         if self.verbose:
             print(f'Loss decreased ({self.loss_min:.6f} --> {loss:.6f}).  Saving model ...')
         torch.save(model.state_dict(), self.checkpoint_file)
         self.loss_min = loss
 
 
 
-def train(model, data, condition, velocity,epoch, batch_size, lr, weight_decay,patience,GPU, seed,verbose, outdir,a):
+def train(model, data, condition, velocity, epoch, batch_size, lr, weight_decay,patience,GPU, seed,verbose, outdir,a):
     
     if torch.cuda.is_available(): # cuda device
         device='cuda'
         torch.cuda.set_device(GPU)
         torch.cuda.manual_seed(seed)
         torch.cuda.manual_seed_all(seed)
     else:
@@ -120,18 +120,19 @@
             v=data_list[2].to(device)
             optimizer.zero_grad()
             recon_x, recon_g = model(x)
             mu, log_var,g = model.encoder(x)     
             z = model.reparameterize(mu, log_var)
             
             true_samples = Variable(torch.randn(x.shape[0], 10), requires_grad=False)
-            mmd = 100*compute_mmd(true_samples.to(device), z)
-            
-            mse1=a*mse_loss(recon_x,v)
-            mse2=mse_loss(recon_g,c)
+            mmd = 50*compute_mmd(true_samples.to(device), z)
+            # mmd=kl_divergence(mu,log_var)
+           
+            mse1= 10* a * mse_loss(recon_x,v)
+            mse2= 10*(1-a)*mse_loss(recon_g,c)
             mse = mse1+mse2 
             loss=mse+mmd 
             loss.backward()      
             optimizer.step()  
             
             MSE1_loss += mse1.item()
             MSE2_loss += mse2.item()
```

### Comparing `scape-sc-0.5.1/src/scape_sc.egg-info/PKG-INFO` & `scape-sc-0.5.2/src/scape_sc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scape-sc
-Version: 0.5.1
+Version: 0.5.2
 Summary: Single-Cell data Analysis via Perturbation Estimation
 Author-email: Yuzhe Li <liyuzhezju@gmail.com>
 Project-URL: Homepage, https://github.com/ericli0419/SCAPE
 Project-URL: Bug Tracker, https://github.com/ericli0419/SCAPE/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

