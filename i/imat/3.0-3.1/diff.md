# Comparing `tmp/imat-3.0.tar.gz` & `tmp/imat-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imat-3.0.tar", last modified: Mon Jul 17 19:40:21 2023, max compression
+gzip compressed data, was "imat-3.1.tar", last modified: Sat Jul 22 04:18:47 2023, max compression
```

## Comparing `imat-3.0.tar` & `imat-3.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:21.365200 imat-3.0/
--rw-rw-rw-   0        0        0     1096 2023-07-17 17:26:37.000000 imat-3.0/LICENSE.txt
--rw-rw-rw-   0        0        0    12064 2023-07-17 19:40:21.358213 imat-3.0/PKG-INFO
--rw-rw-rw-   0        0        0    10845 2023-07-17 19:39:46.000000 imat-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:20.607381 imat-3.0/iMaT/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/__init__.py
--rw-rw-rw-   0        0        0     2430 2023-07-17 17:26:37.000000 imat-3.0/iMaT/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:20.615354 imat-3.0/iMaT/src/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:20.645274 imat-3.0/iMaT/src/analysis/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/analysis/__init__.py
--rw-rw-rw-   0        0        0    58077 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/analysis/functions.py
--rw-rw-rw-   0        0        0     5213 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/analysis/main.py
--rw-rw-rw-   0        0        0     3572 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:20.685172 imat-3.0/iMaT/src/cli/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/cli/__init__.py
--rw-rw-rw-   0        0        0    31663 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/cli/menu_constructors.py
--rw-rw-rw-   0        0        0    23891 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/cli/menu_entries.py
--rw-rw-rw-   0        0        0     7930 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:20.740031 imat-3.0/iMaT/src/conversion/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/conversion/__init__.py
--rw-rw-rw-   0        0        0     5090 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/conversion/main.py
--rw-rw-rw-   0        0        0    12992 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/conversion/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:20.768219 imat-3.0/iMaT/src/m21_environment/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/m21_environment/__init__.py
--rw-rw-rw-   0        0        0    10243 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/m21_environment/main.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:20.889480 imat-3.0/iMaT/src/pattern_search/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/pattern_search/__init__.py
--rw-rw-rw-   0        0        0    15880 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/pattern_search/functions.py
--rw-rw-rw-   0        0        0    10903 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/pattern_search/main.py
--rw-rw-rw-   0        0        0    10307 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/pattern_search/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:20.973242 imat-3.0/iMaT/src/score_selection/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/score_selection/__init__.py
--rw-rw-rw-   0        0        0    17704 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/score_selection/main.py
--rw-rw-rw-   0        0        0    14028 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/score_selection/name_parts.py
--rw-rw-rw-   0        0        0    12218 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/score_selection/select_parts_and_measures.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:21.005165 imat-3.0/iMaT/src/tokenization/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/tokenization/__init__.py
--rw-rw-rw-   0        0        0    19526 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/tokenization/main.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:21.060014 imat-3.0/iMaT/src/tokenization/refine_results/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/tokenization/refine_results/__init__.py
--rw-rw-rw-   0        0        0     6837 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/tokenization/refine_results/absolute_duration.py
--rw-rw-rw-   0        0        0     7020 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py
--rw-rw-rw-   0        0        0     4966 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/tokenization/refine_results/remove_prefixes.py
--rw-rw-rw-   0        0        0     5447 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/tokenization/refine_results/tokens_to_txt.py
--rw-rw-rw-   0        0        0    15349 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/tokenization/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:21.083945 imat-3.0/iMaT/src/utils/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3982 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/utils/error_handling.py
--rw-rw-rw-   0        0        0     6787 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:21.130820 imat-3.0/iMaT/src/visualizations/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/visualizations/__init__.py
--rw-rw-rw-   0        0        0    19214 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/visualizations/analysis_results_graphs.py
--rw-rw-rw-   0        0        0    10926 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/visualizations/m21_integrated.py
--rw-rw-rw-   0        0        0     3263 2023-07-17 17:26:37.000000 imat-3.0/iMaT/src/visualizations/main.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:40:21.347241 imat-3.0/imat.egg-info/
--rw-rw-rw-   0        0        0    12064 2023-07-17 19:40:18.000000 imat-3.0/imat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1561 2023-07-17 19:40:18.000000 imat-3.0/imat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 19:40:18.000000 imat-3.0/imat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-17 19:40:18.000000 imat-3.0/imat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      224 2023-07-17 19:40:18.000000 imat-3.0/imat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-17 19:40:18.000000 imat-3.0/imat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 19:40:21.366191 imat-3.0/setup.cfg
--rw-rw-rw-   0        0        0     2011 2023-07-17 19:07:47.000000 imat-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:47.060763 imat-3.1/
+-rw-rw-rw-   0        0        0     1096 2023-07-17 17:26:37.000000 imat-3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    12064 2023-07-22 04:18:47.055776 imat-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10845 2023-07-17 19:39:46.000000 imat-3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.679263 imat-3.1/iMaT/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/__init__.py
+-rw-rw-rw-   0        0        0     2430 2023-07-17 17:26:37.000000 imat-3.1/iMaT/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.684250 imat-3.1/iMaT/src/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.704197 imat-3.1/iMaT/src/analysis/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0    58077 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/analysis/functions.py
+-rw-rw-rw-   0        0        0     5213 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/analysis/main.py
+-rw-rw-rw-   0        0        0     3572 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.732123 imat-3.1/iMaT/src/cli/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/cli/__init__.py
+-rw-rw-rw-   0        0        0    31663 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/cli/menu_constructors.py
+-rw-rw-rw-   0        0        0    23891 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/cli/menu_entries.py
+-rw-rw-rw-   0        0        0     7930 2023-07-22 04:18:10.000000 imat-3.1/iMaT/src/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.746086 imat-3.1/iMaT/src/conversion/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/conversion/__init__.py
+-rw-rw-rw-   0        0        0     5090 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/conversion/main.py
+-rw-rw-rw-   0        0        0    12992 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/conversion/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.753067 imat-3.1/iMaT/src/m21_environment/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/m21_environment/__init__.py
+-rw-rw-rw-   0        0        0    10243 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/m21_environment/main.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.797946 imat-3.1/iMaT/src/pattern_search/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/pattern_search/__init__.py
+-rw-rw-rw-   0        0        0    15880 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/pattern_search/functions.py
+-rw-rw-rw-   0        0        0    10903 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/pattern_search/main.py
+-rw-rw-rw-   0        0        0    10307 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/pattern_search/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.848326 imat-3.1/iMaT/src/score_selection/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/score_selection/__init__.py
+-rw-rw-rw-   0        0        0    17704 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/score_selection/main.py
+-rw-rw-rw-   0        0        0    14028 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/score_selection/name_parts.py
+-rw-rw-rw-   0        0        0    12218 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/score_selection/select_parts_and_measures.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.897197 imat-3.1/iMaT/src/tokenization/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/tokenization/__init__.py
+-rw-rw-rw-   0        0        0    19526 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/tokenization/main.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.917150 imat-3.1/iMaT/src/tokenization/refine_results/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/tokenization/refine_results/__init__.py
+-rw-rw-rw-   0        0        0     6837 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/tokenization/refine_results/absolute_duration.py
+-rw-rw-rw-   0        0        0     7020 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py
+-rw-rw-rw-   0        0        0     4966 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/tokenization/refine_results/remove_prefixes.py
+-rw-rw-rw-   0        0        0     5447 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/tokenization/refine_results/tokens_to_txt.py
+-rw-rw-rw-   0        0        0    15349 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/tokenization/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.963021 imat-3.1/iMaT/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3982 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/utils/error_handling.py
+-rw-rw-rw-   0        0        0     6787 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:46.999921 imat-3.1/iMaT/src/visualizations/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/visualizations/__init__.py
+-rw-rw-rw-   0        0        0    19214 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/visualizations/analysis_results_graphs.py
+-rw-rw-rw-   0        0        0    10926 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/visualizations/m21_integrated.py
+-rw-rw-rw-   0        0        0     3263 2023-07-17 17:26:37.000000 imat-3.1/iMaT/src/visualizations/main.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:18:47.045807 imat-3.1/imat.egg-info/
+-rw-rw-rw-   0        0        0    12064 2023-07-22 04:18:44.000000 imat-3.1/imat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2023-07-22 04:18:44.000000 imat-3.1/imat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 04:18:44.000000 imat-3.1/imat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-22 04:18:44.000000 imat-3.1/imat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      266 2023-07-22 04:18:44.000000 imat-3.1/imat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-22 04:18:44.000000 imat-3.1/imat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 04:18:47.061756 imat-3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2079 2023-07-22 04:18:10.000000 imat-3.1/setup.py
```

### Comparing `imat-3.0/LICENSE.txt` & `imat-3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imat-3.0/PKG-INFO` & `imat-3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imat
-Version: 3.0
+Version: 3.1
 Summary: Interactive Music Analysis Tool (I-MaT)
 Home-page: https://github.com/sebastian-eck/I-MaT
 Author: Sebastian Oliver Eck
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `imat-3.0/README.md` & `imat-3.1/README.md`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/__main__.py` & `imat-3.1/iMaT/__main__.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/analysis/functions.py` & `imat-3.1/iMaT/src/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/analysis/main.py` & `imat-3.1/iMaT/src/analysis/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/analysis/utils.py` & `imat-3.1/iMaT/src/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/cli/menu_constructors.py` & `imat-3.1/iMaT/src/cli/menu_constructors.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/cli/menu_entries.py` & `imat-3.1/iMaT/src/cli/menu_entries.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/constants.py` & `imat-3.1/iMaT/src/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 TITLE_TEXT is a string that contains the title text for the application. It includes the name and version of the 
 application, the associated project and institution, the license information, and the copyright statement. This text 
 is used to display a title or header in the application's user interface.
 
 """
 
 TITLE_TEXT = (
-    '\nI-MaT - Interactive Music Analysis Tool, v3.0, (2023). Project: "Computer-Assisted Music Analysis"\n\n'
+    '\nI-MaT - Interactive Music Analysis Tool, v3.1, (2023). Project: "Computer-Assisted Music Analysis"\n\n'
     'Department of Musicology Weimar-Jena, University of Music Franz Liszt Weimar, Germany\n\n'
     'MIT License, Copyright (c) 2023 S.O. Eck.\n\n'
     '----------------------------------------------------------------------\n'
 )
 
 """
```

### Comparing `imat-3.0/iMaT/src/conversion/main.py` & `imat-3.1/iMaT/src/conversion/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/conversion/utils.py` & `imat-3.1/iMaT/src/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/m21_environment/main.py` & `imat-3.1/iMaT/src/m21_environment/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/pattern_search/functions.py` & `imat-3.1/iMaT/src/pattern_search/functions.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/pattern_search/main.py` & `imat-3.1/iMaT/src/pattern_search/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/pattern_search/utils.py` & `imat-3.1/iMaT/src/pattern_search/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/score_selection/main.py` & `imat-3.1/iMaT/src/score_selection/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/score_selection/name_parts.py` & `imat-3.1/iMaT/src/score_selection/name_parts.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/score_selection/select_parts_and_measures.py` & `imat-3.1/iMaT/src/score_selection/select_parts_and_measures.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/tokenization/main.py` & `imat-3.1/iMaT/src/tokenization/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/tokenization/refine_results/absolute_duration.py` & `imat-3.1/iMaT/src/tokenization/refine_results/absolute_duration.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py` & `imat-3.1/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/tokenization/refine_results/remove_prefixes.py` & `imat-3.1/iMaT/src/tokenization/refine_results/remove_prefixes.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/tokenization/refine_results/tokens_to_txt.py` & `imat-3.1/iMaT/src/tokenization/refine_results/tokens_to_txt.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/tokenization/utils.py` & `imat-3.1/iMaT/src/tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/utils/error_handling.py` & `imat-3.1/iMaT/src/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/utils/misc.py` & `imat-3.1/iMaT/src/utils/misc.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/visualizations/analysis_results_graphs.py` & `imat-3.1/iMaT/src/visualizations/analysis_results_graphs.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/visualizations/m21_integrated.py` & `imat-3.1/iMaT/src/visualizations/m21_integrated.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/iMaT/src/visualizations/main.py` & `imat-3.1/iMaT/src/visualizations/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.0/imat.egg-info/PKG-INFO` & `imat-3.1/imat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imat
-Version: 3.0
+Version: 3.1
 Summary: Interactive Music Analysis Tool (I-MaT)
 Home-page: https://github.com/sebastian-eck/I-MaT
 Author: Sebastian Oliver Eck
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `imat-3.0/imat.egg-info/SOURCES.txt` & `imat-3.1/imat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imat-3.0/setup.py` & `imat-3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     include_package_data=True,
     name='imat',
-    version='3.0',
+    version='3.1',
     author='Sebastian Oliver Eck',
     url="https://github.com/sebastian-eck/I-MaT",
     description='Interactive Music Analysis Tool (I-MaT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT License",
     packages=setuptools.find_packages(),
@@ -45,17 +45,20 @@
         "matplotlib~=3.7.1",
         "pandas~=2.0.2",
         "music21~=8.3.0",
         "miditok~=2.0.6",
         "tokenizers~=0.13.3",
         "requests~=2.31.0",
         "openpyxl~=3.1.2",
-        "tqdm~=4.65.0"
+        "tqdm~=4.65.0",
+        "seaborn~=0.12.2",
+        "scipy~=1.10.1"
+
     ],
     extras_require={
         "doc": ["sphinx~=7.0.0",
                 "sphinxcontrib-napoleon~=0.7",
                 "sphinx-autobuild",
                 "myst_parser",
-                "furo"]
+                "sphinx_rtd_theme"]
     }
 )
```

