# Comparing `tmp/influential-0.0.2.tar.gz` & `tmp/influential-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influential-0.0.2.tar", last modified: Thu Apr 20 02:09:52 2023, max compression
+gzip compressed data, was "influential-0.0.21.tar", last modified: Sat Jul 22 12:10:41 2023, max compression
```

## Comparing `influential-0.0.2.tar` & `influential-0.0.21.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-20 02:09:52.452801 influential-0.0.2/
--rw-r--r--   0 adriansalavaty   (501) staff       (20)     1548 2023-04-20 02:09:52.452651 influential-0.0.2/PKG-INFO
--rw-------   0 adriansalavaty   (501) staff       (20)     4401 2023-04-18 07:17:41.000000 influential-0.0.2/README.md
-drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-20 02:09:52.451481 influential-0.0.2/influential/
--rw-------   0 adriansalavaty   (501) staff       (20)      381 2023-04-20 02:01:31.000000 influential-0.0.2/influential/__init__.py
--rw-------   0 adriansalavaty   (501) staff       (20)    43384 2023-04-18 07:02:15.000000 influential-0.0.2/influential/centrality.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)    40515 2023-04-18 06:51:52.000000 influential-0.0.2/influential/exir.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)      997 2023-01-21 23:50:04.000000 influential-0.0.2/influential/ranNorm.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)      843 2023-04-18 06:52:36.000000 influential-0.0.2/influential/rank.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)     4011 2023-02-13 05:41:32.000000 influential-0.0.2/influential/sir.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)     4936 2023-04-18 06:52:30.000000 influential-0.0.2/influential/stats.py
-drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-20 02:09:52.452444 influential-0.0.2/influential/test/
--rw-------   0 adriansalavaty   (501) staff       (20)        0 2022-07-27 08:42:02.000000 influential-0.0.2/influential/test/__init__.py
--rw-r--r--   0 adriansalavaty   (501) staff       (20)    37338 2023-04-18 06:53:13.000000 influential-0.0.2/influential/visualize.py
-drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-04-20 02:09:52.452306 influential-0.0.2/influential.egg-info/
--rw-r--r--   0 adriansalavaty   (501) staff       (20)     1548 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/PKG-INFO
--rw-r--r--   0 adriansalavaty   (501) staff       (20)      399 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/SOURCES.txt
--rw-r--r--   0 adriansalavaty   (501) staff       (20)        1 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/dependency_links.txt
--rw-r--r--   0 adriansalavaty   (501) staff       (20)       76 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/requires.txt
--rw-r--r--   0 adriansalavaty   (501) staff       (20)       12 2023-04-20 02:09:52.000000 influential-0.0.2/influential.egg-info/top_level.txt
--rw-r--r--   0 adriansalavaty   (501) staff       (20)       38 2023-04-20 02:09:52.452850 influential-0.0.2/setup.cfg
--rw-------   0 adriansalavaty   (501) staff       (20)     1923 2023-04-20 02:03:16.000000 influential-0.0.2/setup.py
+drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-07-22 12:10:41.312842 influential-0.0.21/
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)     1569 2023-07-22 12:10:41.312701 influential-0.0.21/PKG-INFO
+-rw-------   0 adriansalavaty   (501) staff       (20)     4401 2023-04-18 07:17:41.000000 influential-0.0.21/README.md
+drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-07-22 12:10:41.311451 influential-0.0.21/influential/
+-rw-------   0 adriansalavaty   (501) staff       (20)      381 2023-04-20 02:01:31.000000 influential-0.0.21/influential/__init__.py
+-rw-------   0 adriansalavaty   (501) staff       (20)    43392 2023-07-22 11:52:03.000000 influential-0.0.21/influential/centrality.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)    40571 2023-07-22 11:53:43.000000 influential-0.0.21/influential/exir.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)      997 2023-01-21 23:50:04.000000 influential-0.0.21/influential/ranNorm.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)      843 2023-04-18 06:52:36.000000 influential-0.0.21/influential/rank.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)     4011 2023-02-13 05:41:32.000000 influential-0.0.21/influential/sir.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)     4936 2023-04-18 06:52:30.000000 influential-0.0.21/influential/stats.py
+drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-07-22 12:10:41.312481 influential-0.0.21/influential/test/
+-rw-------   0 adriansalavaty   (501) staff       (20)        0 2022-07-27 08:42:02.000000 influential-0.0.21/influential/test/__init__.py
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)    37346 2023-07-22 11:54:31.000000 influential-0.0.21/influential/visualize.py
+drwxr-xr-x   0 adriansalavaty   (501) staff       (20)        0 2023-07-22 12:10:41.312280 influential-0.0.21/influential.egg-info/
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)     1569 2023-07-22 12:10:41.000000 influential-0.0.21/influential.egg-info/PKG-INFO
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)      399 2023-07-22 12:10:41.000000 influential-0.0.21/influential.egg-info/SOURCES.txt
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)        1 2023-07-22 12:10:41.000000 influential-0.0.21/influential.egg-info/dependency_links.txt
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)       76 2023-07-22 12:10:41.000000 influential-0.0.21/influential.egg-info/requires.txt
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)       12 2023-07-22 12:10:41.000000 influential-0.0.21/influential.egg-info/top_level.txt
+-rw-r--r--   0 adriansalavaty   (501) staff       (20)       38 2023-07-22 12:10:41.312895 influential-0.0.21/setup.cfg
+-rw-------   0 adriansalavaty   (501) staff       (20)     1924 2023-07-22 12:06:10.000000 influential-0.0.21/setup.py
```

### Comparing `influential-0.0.2/PKG-INFO` & `influential-0.0.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: influential
-Version: 0.0.2
+Version: 0.0.21
 Summary: Identification and Classification of the Most Influential Nodes
 Home-page: http://pypi.python.org/pypi/influential/
 Author: Adrian Salavaty
 Author-email: abbas.salavaty@gmail.com
 License: GPL-3
 Keywords: influential
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
@@ -24,7 +25,9 @@
 Additionally, some functions have been provided for the assessment of dependence and 
 correlation of two network centrality measures as well as the conditional probability of 
 deviation from their corresponding means in opposite direction.
 Fred Viole and David Nawrocki (2013, ISBN:1490523995).
 Csardi G, Nepusz T (2006). 'The igraph software package for complex network research.' InterJournal, Complex Systems, 1695.
 Adopted algorithms and sources are referenced in function document.
 
+
+
```

### Comparing `influential-0.0.2/README.md` & `influential-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `influential-0.0.2/influential/centrality.py` & `influential-0.0.21/influential/centrality.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 import igraph
 from .ranNorm import rangeNormalize
 from .sir import simulate_sir
 from random import seed
 from statistics import mean
 from .rank import rank_cal
-from copy import copy
+from copy import deepcopy
 
 # =============================================================================
 #
 #    Neighborhood Connectivity
 #
 # =============================================================================
 
@@ -1071,15 +1071,15 @@
     all_mean_spread = mean(all_mean_spread)
 
     if verbose:
         print("The SIR simulation of the original network is done!")
 
     # Model the spread based on leave one out cross ranking (LOOCR)
     for s in range(len(node_names)):
-        temp_graph = copy(graph)
+        temp_graph = deepcopy(graph)
         temp_graph.delete_vertices(node_names[s])
         seed(model_seed)
 
         loocr_spread = simulate_sir(graph = temp_graph, beta = beta, gamma = gamma, no_sim = no_sim)
 
         loocr_mean_spread = []
```

### Comparing `influential-0.0.2/influential/exir.py` & `influential-0.0.21/influential/exir.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #! user/bin/env python3
 
 # Import the requirements
 import pandas as pd
 import numpy as np
-from copy import copy
+from copy import deepcopy
 from tqdm import trange
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.decomposition import PCA
 from scipy.stats import t, norm
 from .stats import fcor
 import igraph
 from .centrality import ivi
@@ -185,16 +185,16 @@
     # ProgressBar: Preparing the input data
     if verbose:
       pbar = trange(100)
       pbar.update(1)
       pbar.set_description("Preparing the input data")
 
       ## Make a copy of the data so that the original input data is not changed
-      Exptl_data = copy(Exptl_data)
-      Diff_data = copy(Diff_data)
+      Exptl_data = deepcopy(Exptl_data)
+      Diff_data = deepcopy(Diff_data)
 
     # Change the colnames of Diff_data
     Diff_data.columns = list(map(lambda x: x + '_source', list(Diff_data.columns)))
 
     # Change the Inf/-Inf diff values (applicable to sc-Data)
     for i in range(len(Diff_value)):
 
@@ -368,15 +368,15 @@
         mutualRank_mode = True
     else:
         mutualRank_mode = False
     
     temp_corr = fcor(data = Exptl_data[condition_less_columns], method = "spearman", mutualRank = mutualRank_mode)
 
     ## Save a second copy of all cor data
-    temp_corr_for_sec_round = copy(temp_corr)
+    temp_corr_for_sec_round = deepcopy(temp_corr)
 
     ###################################################
 
     # Check which items from subject satisfy the operator function respective to the source
     def which(subject, source, operator = 'in'):
 
         ## For each element in subject check if that satisfies the operator function respective to the source
@@ -407,31 +407,31 @@
 
     # Filter corr data for only those corr between diff features and themselves/others
     filter_corr_index = list(which(subject = list(temp_corr.row), source = list(rf_diff_exptl_pvalue.feature), operator = 'in').keys()) + list(which(subject = list(temp_corr.column), source = list(rf_diff_exptl_pvalue.feature), operator = 'in').keys())
     filter_corr_index = list(set(filter_corr_index))
     temp_corr = temp_corr.iloc[filter_corr_index]
 
     ## Filtering low level correlations
-    cor_thresh = copy(r)
-    mr_thresh = copy(mr)
+    cor_thresh = deepcopy(r)
+    mr_thresh = deepcopy(mr)
 
     if cor_thresh_method == "mr":
         temp_corr = temp_corr[temp_corr['mr'] < mr_thresh]
 
         if temp_corr.shape[0] > (max_connections*0.95):
             temp_corr_select_index = list(np.argsort(temp_corr.mr)[:round(max_connections*0.95)])
             temp_corr = temp_corr.iloc[temp_corr_select_index]
     elif cor_thresh_method == "cor.coefficient":
         temp_corr = temp_corr[abs(temp_corr['cor']) > cor_thresh]
 
         if temp_corr.shape[0] > (max_connections*0.95):
             temp_corr_select_index = list(np.argsort(temp_corr.cor)[-round(max_connections*0.95):])
             temp_corr = temp_corr.iloc[temp_corr_select_index]
 
-    diff_only_temp_corr = copy(temp_corr)
+    diff_only_temp_corr = deepcopy(temp_corr)
 
     # Getting the list of diff features and their correlated features
     diff_plus_corr_features = list(temp_corr.row) + list(temp_corr.column)
     diff_plus_corr_features = list(set(diff_plus_corr_features))
 
     # Find the diff features amongst diff_plus_corr_features
     non_diff_only_features = list(which(subject = diff_plus_corr_features, source = list(rf_diff_exptl_pvalue.feature), operator = 'not in').values())
@@ -439,26 +439,26 @@
     if verbose:
         pbar.update(10)
         pbar.set_description("Performing the first round of association analysis")
 
     if len(non_diff_only_features) > 0:
 
         ## Redo correlation analysis
-        temp_corr = copy(temp_corr_for_sec_round)
+        temp_corr = deepcopy(temp_corr_for_sec_round)
         del temp_corr_for_sec_round
 
         ## Filter corr data for only those corr between non_diff_only_features and themselves/others
         filter_corr_index = list(which(subject = temp_corr.row, source = non_diff_only_features, operator = 'in').keys()) + list(which(subject = temp_corr.column, source = non_diff_only_features, operator = 'in').keys())
         filter_corr_index = list(set(filter_corr_index))
         
         temp_corr = temp_corr.iloc[filter_corr_index]
 
         ## Filtering low level correlations
-        cor_thresh = copy(r)
-        mr_thresh = copy(mr)
+        cor_thresh = deepcopy(r)
+        mr_thresh = deepcopy(mr)
 
         if cor_thresh_method == "mr":
             temp_corr = temp_corr[temp_corr['mr'] < mr_thresh]
         elif cor_thresh_method == "cor.coefficient":
                 temp_corr = temp_corr[abs(temp_corr['cor']) > cor_thresh]
 
         ## Separate non_diff_only features
@@ -476,15 +476,15 @@
 
             temp_corr = temp_corr.iloc[temp_corr_select_index]
 
         ## Recombine the diff_only_temp_corr data and temp_corr
         temp_corr = pd.concat([temp_corr, diff_only_temp_corr], axis=0)
 
     else:
-        temp_corr = copy(diff_only_temp_corr)
+        temp_corr = deepcopy(diff_only_temp_corr)
         del diff_only_temp_corr
 
     if verbose:
         pbar.update(10)
         pbar.set_description("Network reconstruction")
     
     #d Graph reconstruction
@@ -563,15 +563,15 @@
     Diff_data.N_score = rangeNormalize(data = Diff_data.N_score, minimum = 1, maximum = 100)
 
     #c calculate the final driver score
     Diff_data['final_Driver_score'] = (Diff_data.first_Driver_Rank)*(Diff_data.N_score)
     Diff_data.final_Driver_score[Diff_data.final_Driver_score==0] = np.nan
 
     # Create the Drivers table
-    Driver_table = copy(Diff_data)
+    Driver_table = deepcopy(Diff_data)
 
     ## Remove the rows/features with NA in the final driver score
     Driver_table = Driver_table[Driver_table.final_Driver_score != np.nan]
 
     ## Filter the driver table by the desired list (if provided)
     if Desired_list is not None:
         Driver_table_row_index = list(which(subject = list(Driver_table.index), source = Desired_list, operator = 'in').keys())
@@ -627,15 +627,15 @@
 
     if verbose:
         pbar.update(5)
         pbar.set_description("Preparation of the biomarker table")
 
     # Create the Biomarker table
 
-    Biomarker_table = copy(Diff_data)
+    Biomarker_table = deepcopy(Diff_data)
 
     ## Remove the rows/features with NA in the final driver score
     Biomarker_table = Biomarker_table[Biomarker_table.final_Driver_score != np.nan]
 
     ## Filter the biomarker table by the desired list (if provided)
     if Desired_list is not None:
         Biomarker_table_row_index = list(which(subject = list(Biomarker_table.index), source = Desired_list, operator= 'in').keys())
@@ -719,15 +719,15 @@
 
     if verbose:
         pbar.update(5)
         pbar.set_description("Preparation of the DE-mediator table")
 
     # Create the DE mediators table
 
-    DE_mediator_table = copy(Diff_data)
+    DE_mediator_table = deepcopy(Diff_data)
 
     ## Include only rows/features with NaN in the final driver score (which are mediators)
     DE_mediator_table_index = list(i for i, x in enumerate(list(np.isnan(DE_mediator_table.final_Driver_score))) if x)
     
     DE_mediator_table = DE_mediator_table.iloc[DE_mediator_table_index]
 
     DE_mediator_table['DE_mediator_score'] = DE_mediator_table.sum_Sig_value * DE_mediator_table.IVI * DE_mediator_table.N_score
```

### Comparing `influential-0.0.2/influential/ranNorm.py` & `influential-0.0.21/influential/ranNorm.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.2/influential/rank.py` & `influential-0.0.21/influential/rank.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.2/influential/sir.py` & `influential-0.0.21/influential/sir.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.2/influential/stats.py` & `influential-0.0.21/influential/stats.py`

 * *Files identical despite different names*

### Comparing `influential-0.0.2/influential/visualize.py` & `influential-0.0.21/influential/visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import igraph
 from random import seed
 from plotnine import ggplot, aes, geoms, arrow, scale_color_cmap, scale_color_cmap_d, scale_color_manual, scale_fill_gradient, scale_size_identity, scale_x_continuous, scale_y_continuous, ggtitle, labs, guides, guide_legend, facet_wrap, scale_size_continuous, themes
 from plotnine.utils import to_inches
 from .ranNorm import rangeNormalize
 from .rank import rank_cal
 from functools import reduce
-from copy import copy
+from copy import deepcopy
 
 # =============================================================================
 #
 #    Visualization of a graph based on centrality measures
 #
 # =============================================================================
 
@@ -704,15 +704,15 @@
         ## Return a dictionary including match indices as keys and their corresponding values as the values
         return dict(zip(match_index, match_values))
     
     ###################################################
 
     ## correct the features names
     if synonyms_table is not None:
-        synonyms_table = copy(synonyms_table)
+        synonyms_table = deepcopy(synonyms_table)
         synonyms_table.index = list(synonyms_table.iloc[:,0])
         synonyms_index = list(which(subject = list(exir_for_plot.Feature), source = list(synonyms_table.index), operator= 'in').values())
         exir_for_plot.Feature.iloc[list(which(subject = list(exir_for_plot.Feature), source = synonyms_index, operator= 'in').keys())] = list(synonyms_table.loc[synonyms_index, synonyms_table.columns[1]])
 
     ## remove undesired classes
     if show_drivers is False and any(exir_for_plot.Class == "Driver"):
       exir_for_plot = exir_for_plot.drop(list(i for i,j in enumerate(list(exir_for_plot.Class == "Driver")) if j), axis=0)
```

### Comparing `influential-0.0.2/influential.egg-info/PKG-INFO` & `influential-0.0.21/influential.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: influential
-Version: 0.0.2
+Version: 0.0.21
 Summary: Identification and Classification of the Most Influential Nodes
 Home-page: http://pypi.python.org/pypi/influential/
 Author: Adrian Salavaty
 Author-email: abbas.salavaty@gmail.com
 License: GPL-3
 Keywords: influential
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
@@ -24,7 +25,9 @@
 Additionally, some functions have been provided for the assessment of dependence and 
 correlation of two network centrality measures as well as the conditional probability of 
 deviation from their corresponding means in opposite direction.
 Fred Viole and David Nawrocki (2013, ISBN:1490523995).
 Csardi G, Nepusz T (2006). 'The igraph software package for complex network research.' InterJournal, Complex Systems, 1695.
 Adopted algorithms and sources are referenced in function document.
 
+
+
```

### Comparing `influential-0.0.2/setup.py` & `influential-0.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.21'
 DESCRIPTION = 'Identification and Classification of the Most Influential Nodes'
 LONG_DESCRIPTION = """
 
 Contains functions for the classification and ranking of top candidate features, reconstruction of networks from
 adjacency matrices and data frames, analysis of the topology of the network 
 and calculation of centrality measures, and identification of the most
 influential nodes. Also, a function is provided for running SIRIR model, which
```

