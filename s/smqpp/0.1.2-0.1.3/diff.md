# Comparing `tmp/smqpp-0.1.2.tar.gz` & `tmp/smqpp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smqpp-0.1.2.tar", last modified: Sat Nov  7 12:36:03 2020, max compression
+gzip compressed data, was "smqpp-0.1.3.tar", last modified: Sat Jul 22 17:21:52 2023, max compression
```

## Comparing `smqpp-0.1.2.tar` & `smqpp-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)        0 2020-11-07 12:36:03.000000 smqpp-0.1.2/
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)      422 2020-11-07 12:29:09.000000 smqpp-0.1.2/setup.py
-drwxrwsr-x   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)        0 2020-11-07 12:36:03.000000 smqpp-0.1.2/smqpp.egg-info/
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)       61 2020-11-07 12:36:03.000000 smqpp-0.1.2/smqpp.egg-info/requires.txt
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)      240 2020-11-07 12:36:03.000000 smqpp-0.1.2/smqpp.egg-info/PKG-INFO
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)        6 2020-11-07 12:36:03.000000 smqpp-0.1.2/smqpp.egg-info/top_level.txt
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)        1 2020-11-07 12:36:03.000000 smqpp-0.1.2/smqpp.egg-info/dependency_links.txt
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)      197 2020-11-07 12:36:03.000000 smqpp-0.1.2/smqpp.egg-info/SOURCES.txt
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)      240 2020-11-07 12:36:03.000000 smqpp-0.1.2/PKG-INFO
-drwxrwsr-x   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)        0 2020-11-07 12:36:03.000000 smqpp-0.1.2/smqpp/
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)    49516 2020-11-07 12:28:30.000000 smqpp-0.1.2/smqpp/__init__.py
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)       62 2020-11-07 12:28:54.000000 smqpp-0.1.2/smqpp/version.py
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)       38 2020-11-07 12:36:03.000000 smqpp-0.1.2/setup.cfg
--rw-rw-r--   0 xw251    (15554) rds-bg200-hphi-gottgens (41091)     1494 2020-05-07 10:59:12.000000 smqpp-0.1.2/README.md
+drwxrwsr-x   0 xw251    (15554) rds-SDzz0CATGms-users (90387)        0 2023-07-22 17:21:52.000000 smqpp-0.1.3/
+-rw-rw-r--   0 xw251    (15554) rds-SDzz0CATGms-users (90387)      201 2023-07-22 17:21:52.000000 smqpp-0.1.3/PKG-INFO
+-rwxrwxrwx   0 xw251    (15554) rds-SDzz0CATGms-users (90387)     1494 2020-05-07 10:59:12.000000 smqpp-0.1.3/README.md
+-rw-rw-r--   0 xw251    (15554) rds-SDzz0CATGms-users (90387)       38 2023-07-22 17:21:52.000000 smqpp-0.1.3/setup.cfg
+-rwxrwxrwx   0 xw251    (15554) rds-SDzz0CATGms-users (90387)      428 2023-07-22 17:06:02.000000 smqpp-0.1.3/setup.py
+drwxrwsr-x   0 xw251    (15554) rds-SDzz0CATGms-users (90387)        0 2023-07-22 17:21:51.000000 smqpp-0.1.3/smqpp/
+-rwxrwxr-x   0 xw251    (15554) rds-SDzz0CATGms-users (90387)    49533 2023-07-22 17:00:20.000000 smqpp-0.1.3/smqpp/__init__.py
+-rwxrwxrwx   0 xw251    (15554) rds-SDzz0CATGms-users (90387)       62 2023-07-22 17:00:28.000000 smqpp-0.1.3/smqpp/version.py
+drwxrwsr-x   0 xw251    (15554) rds-SDzz0CATGms-users (90387)        0 2023-07-22 17:21:52.000000 smqpp-0.1.3/smqpp.egg-info/
+-rwxrwxrwx   0 xw251    (15554) rds-SDzz0CATGms-users (90387)      201 2023-07-22 17:21:51.000000 smqpp-0.1.3/smqpp.egg-info/PKG-INFO
+-rwxrwxrwx   0 xw251    (15554) rds-SDzz0CATGms-users (90387)      197 2023-07-22 17:21:51.000000 smqpp-0.1.3/smqpp.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xw251    (15554) rds-SDzz0CATGms-users (90387)        1 2023-07-22 17:21:51.000000 smqpp-0.1.3/smqpp.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xw251    (15554) rds-SDzz0CATGms-users (90387)       67 2023-07-22 17:21:51.000000 smqpp-0.1.3/smqpp.egg-info/requires.txt
+-rwxrwxrwx   0 xw251    (15554) rds-SDzz0CATGms-users (90387)        6 2023-07-22 17:21:51.000000 smqpp-0.1.3/smqpp.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `smqpp-0.1.2/smqpp/__init__.py` & `smqpp-0.1.3/smqpp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,18 +362,18 @@
                 print('Calculate SF for erccs:')
                 sf_ercc = est_size_factor(adata.obsm['ERCC'], method=method)
                 adata.obs['sf_ercc'] = sf_ercc
     else:
         if 'sf_gene' not in adata.obs_keys():
             raise ValueError('sf_gene is not found in .obs, please set reCalSF=True.')
     
-    adata.X = np.log1p(adata.X/adata.obs['sf_gene'][:,None])
+    adata.X = np.log1p(adata.X/adata.obs['sf_gene'].values[:,None])
     if 'ERCC' in adata.obsm_keys():
         if adata.obsm['ERCC'].size !=0:
-            adata.obsm['ERCC_norm'] = np.log1p(adata.obsm['ERCC']/adata.obs['sf_ercc'][:,None])
+            adata.obsm['ERCC_norm'] = np.log1p(adata.obsm['ERCC']/adata.obs['sf_ercc'].values[:,None])
     if copy:
         return adata.copy()
 
 ############## BELOW is Quantile normalisation ########
 from scipy.stats import rankdata
 def quantile_norm(X):
     '''
@@ -508,15 +508,15 @@
     print('MeanForFit: ', str(meanForFit))
     useForFit = (sMean>=meanForFit)
     print(np.sum(useForFit))
     
     a1tilde = 1/sMean[useForFit]
     x = sm.add_constant(a1tilde, prepend=False)
     y = cv2s[useForFit]
-    link_func = sm.genmod.families.links.identity
+    link_func = sm.genmod.families.links.Identity()
     fit = sm.GLM(y, x, family=sm.families.Gamma(link=link_func)).fit()
 
     a0 = fit.params[1]
     a1t = fit.params[0]
     df = data.shape[0]-1
     m = data.shape[0]
     xi = None
@@ -594,16 +594,16 @@
     
     e_df = pd.DataFrame(adata.uns['varGenes']['ercc'])
     e_df = e_df.loc[e_df['mean']>0,]
     
     fig = plt.figure()
     ax = fig.add_subplot(111)
     plt.scatter(g_df.loc[~g_df['highVar'],:]['mean'], g_df.loc[~g_df['highVar'],:]['cv2'], color='grey', s=s)
-    ax.set_yscale('log',basey=10)
-    ax.set_xscale('log',basex=10)
+    ax.set_yscale('log',base=10)
+    ax.set_xscale('log',base=10)
     ax.set_ylabel(r'$\sigma^{2}/\mu^{2}$')
     ax.set_xlabel(r'$\mu$')
     ax.grid(False)
 
     plt.scatter(g_df.loc[g_df['highVar'],:]['mean'], g_df.loc[g_df['highVar'],:]['cv2'], color='red', s=s)
     
     xlim = np.log10(ax.get_xlim())
@@ -981,15 +981,16 @@
 
 def compute_connectivities_umap(
     knn_indices, knn_dists,
     n_obs, n_neighbors, set_op_mix_ratio=1.0,
     local_connectivity=1.0,
 ):
 
-    """    This code is copied from scanpy!!!
+    """\
+    This code is copied from scanpy!!!
     
     This is from umap.fuzzy_simplicial_set [McInnes18]_.
     Given a set of data X, a neighborhood size, and a measure of distance
     compute the fuzzy simplicial set (here represented as a fuzzy graph in
     the form of a sparse matrix) associated to the data. This is done by
     locally approximating geodesic distance at each point, creating a fuzzy
     simplicial set for each such point, and then combining all the local
@@ -1256,15 +1257,15 @@
             for i in range(len(cats)):
                 #print(cats[i])
                 idx = obs_term==cats[i]
                 ax.plot(dm_new[idx,components[0]],dm_new[idx,components[1]],dm_new[idx,components[2]], '.', markersize=markersize, c=color_pal[i], label = cats[i], alpha =alpha)
             ax.set_title(k)
             plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
         
-        plt.tight_layout()
+    plt.tight_layout()
     if save is not None:
         plt.savefig(save)
         
 
 ###################### BELOW is for pathway analysis ############################################
 def pathway_score_cal(adata, DBcont, minGS=5, maxGS=500):
     '''
@@ -1286,16 +1287,16 @@
     pnames = np.array([])
     TotalGenes = [x.upper() for x in adata.raw.var_names]
     for l in range(len(DBcont)):
         lcont = DBcont[l].split('\t')
         pathway = lcont[0]
         DBGenes = [x.upper() for x in lcont[2:]]
         DBGenes = np.in1d(TotalGenes, DBGenes)
-        if ((np.sum(DBGenes) < minGS) & (np.sum(DBGenes) > maxGS)): 
-            next
+        if ((np.sum(DBGenes) < minGS) or (np.sum(DBGenes) > maxGS)): 
+            continue
         else:
             Exp = np.mean(adata.raw[:, DBGenes].X, axis=1)
             expArray.append(Exp)
             pnames = np.append(pnames, pathway)
     expArray=pd.DataFrame(np.vstack(expArray).T)
     expArray.index = adata.obs_names
     expArray.columns = pnames
```

### Comparing `smqpp-0.1.2/README.md` & `smqpp-0.1.3/README.md`

 * *Files identical despite different names*

