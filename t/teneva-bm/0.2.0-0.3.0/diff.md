# Comparing `tmp/teneva_bm-0.2.0.tar.gz` & `tmp/teneva_bm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.2.0.tar", last modified: Mon Jul 17 20:18:42 2023, max compression
+gzip compressed data, was "teneva_bm-0.3.0.tar", last modified: Sat Jul 22 18:08:27 2023, max compression
```

## Comparing `teneva_bm-0.2.0.tar` & `teneva_bm-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,67 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.787340 teneva_bm-0.2.0/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.2.0/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       54 2023-04-26 09:54:29.000000 teneva_bm-0.2.0/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)    13380 2023-07-17 20:18:42.787765 teneva_bm-0.2.0/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)    12119 2023-07-17 20:06:47.000000 teneva_bm-0.2.0/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      652 2023-07-17 09:21:50.000000 teneva_bm-0.2.0/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-17 20:18:42.789018 teneva_bm-0.2.0/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.2.0/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.769823 teneva_bm-0.2.0/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      169 2023-07-17 20:06:24.000000 teneva_bm-0.2.0/teneva_bm/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)    14607 2023-07-17 19:17:31.000000 teneva_bm-0.2.0/teneva_bm/bm.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.778434 teneva_bm-0.2.0/teneva_bm/func/
--rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.2.0/teneva_bm/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2973 2023-07-17 14:30:03.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2444 2023-07-17 14:32:24.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2423 2023-07-17 14:32:05.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2438 2023-07-17 14:32:52.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2886 2023-07-17 14:33:30.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3008 2023-07-17 14:34:01.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 14:34:28.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2550 2023-07-17 14:34:49.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     2873 2023-07-17 14:35:06.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3189 2023-07-17 14:35:23.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2171 2023-07-17 14:35:48.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     2824 2023-07-17 14:36:05.000000 teneva_bm-0.2.0/teneva_bm/func/bm_func_schwefel.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.779935 teneva_bm-0.2.0/teneva_bm/oc/
--rw-r--r--   0 andrei     (501) staff       (20)       87 2023-07-13 07:42:11.000000 teneva_bm-0.2.0/teneva_bm/oc/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     3326 2023-07-17 18:44:45.000000 teneva_bm-0.2.0/teneva_bm/oc/bm_oc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     2180 2023-07-17 18:45:47.000000 teneva_bm-0.2.0/teneva_bm/oc/bm_oc_simple_constr.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.783177 teneva_bm-0.2.0/teneva_bm/qubo/
--rw-r--r--   0 andrei     (501) staff       (20)      168 2023-07-13 07:41:50.000000 teneva_bm-0.2.0/teneva_bm/qubo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2886 2023-07-17 19:08:37.000000 teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_knap_amba.py
--rw-r--r--   0 andrei     (501) staff       (20)     1866 2023-07-17 19:22:24.000000 teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2662 2023-07-17 15:10:35.000000 teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2668 2023-07-17 19:22:18.000000 teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)     3270 2023-07-17 20:15:06.000000 teneva_bm-0.2.0/teneva_bm/teneva_bm_demo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.786674 teneva_bm-0.2.0/teneva_bm/various/
--rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.2.0/teneva_bm/various/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     6982 2023-07-17 20:05:20.000000 teneva_bm-0.2.0/teneva_bm/various/bm_matmul.py
--rw-r--r--   0 andrei     (501) staff       (20)    11422 2023-07-17 19:32:33.000000 teneva_bm-0.2.0/teneva_bm/various/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1919 2023-07-17 19:22:56.000000 teneva_bm-0.2.0/teneva_bm/various/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-17 20:18:42.771859 teneva_bm-0.2.0/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)    13380 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1105 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-17 20:18:42.000000 teneva_bm-0.2.0/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.962700 teneva_bm-0.3.0/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.3.0/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       54 2023-04-26 09:54:29.000000 teneva_bm-0.3.0/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    15443 2023-07-22 18:08:27.962983 teneva_bm-0.3.0/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)    14182 2023-07-22 18:08:03.000000 teneva_bm-0.3.0/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      652 2023-07-17 09:21:50.000000 teneva_bm-0.3.0/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-22 18:08:27.964205 teneva_bm-0.3.0/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.3.0/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.935247 teneva_bm-0.3.0/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      187 2023-07-22 18:07:52.000000 teneva_bm-0.3.0/teneva_bm/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)    18025 2023-07-22 17:43:46.000000 teneva_bm-0.3.0/teneva_bm/bm.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.943879 teneva_bm-0.3.0/teneva_bm/func/
+-rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.3.0/teneva_bm/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2973 2023-07-17 14:30:03.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2444 2023-07-17 14:32:24.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2423 2023-07-17 14:32:05.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2438 2023-07-17 14:32:52.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2886 2023-07-17 14:33:30.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3008 2023-07-17 14:34:01.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 14:34:28.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2550 2023-07-17 14:34:49.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2873 2023-07-17 14:35:06.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3189 2023-07-17 14:35:23.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2171 2023-07-17 14:35:48.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2824 2023-07-17 14:36:05.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_schwefel.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.945509 teneva_bm-0.3.0/teneva_bm/hs/
+-rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.3.0/teneva_bm/hs/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1624 2023-07-22 16:16:15.000000 teneva_bm-0.3.0/teneva_bm/hs/bm_hs_func001.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2120 2023-07-22 17:59:30.000000 teneva_bm-0.3.0/teneva_bm/hs/bm_hs_func006.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.949583 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.954177 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.955936 teneva_bm-0.3.0/teneva_bm/oc/
+-rw-r--r--   0 andrei     (501) staff       (20)       87 2023-07-13 07:42:11.000000 teneva_bm-0.3.0/teneva_bm/oc/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3326 2023-07-17 18:44:45.000000 teneva_bm-0.3.0/teneva_bm/oc/bm_oc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-22 17:35:02.000000 teneva_bm-0.3.0/teneva_bm/oc/bm_oc_simple_constr.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.959602 teneva_bm-0.3.0/teneva_bm/qubo/
+-rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.3.0/teneva_bm/qubo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7130 2023-07-22 16:59:19.000000 teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_knap_det.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1866 2023-07-17 19:22:24.000000 teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2662 2023-07-17 15:10:35.000000 teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2668 2023-07-17 19:22:18.000000 teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3270 2023-07-17 20:15:06.000000 teneva_bm-0.3.0/teneva_bm/teneva_bm_demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.962088 teneva_bm-0.3.0/teneva_bm/various/
+-rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.3.0/teneva_bm/various/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6982 2023-07-17 20:05:20.000000 teneva_bm-0.3.0/teneva_bm/various/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)    11422 2023-07-17 19:32:33.000000 teneva_bm-0.3.0/teneva_bm/various/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1919 2023-07-17 19:22:56.000000 teneva_bm-0.3.0/teneva_bm/various/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.937422 teneva_bm-0.3.0/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    15443 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     1945 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.2.0/LICENSE.txt` & `teneva_bm-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/PKG-INFO` & `teneva_bm-0.3.0/teneva_bm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: teneva_bm
-Version: 0.2.0
+Name: teneva-bm
+Version: 0.3.0
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,15 +30,15 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.2.0".
+> Current version "0.3.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
 
@@ -52,30 +52,34 @@
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
 bm = BmQuboMaxcut().prep()
 print(bm.info())
 ```
 
-You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_amba`). You can also use a function from the `teneva_bm` package to run all or only one demo:
+You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
-teneva_bm_demo('bm_qubo_knap_amba', with_info=True)
+teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
+> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.2`).
+
 
 ## Available benchmarks
 
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores.
 
+- `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
+
 - `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
 
-- `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapAmba`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
-    > The exact global minimum is known only for `BmQuboKnapAmba` benchmark.
+- `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
+    > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
 
 - `various` - a collection of heterogeneous benchmarks that are not suitable for any other collection (note that in this case, we do not use the name of the collection in the name of the benchmarks, unlike all other sets). The collection includes the following benchmarks: `BmMatmul`, `BmTopopt` (draft!), `BmWallSimple`.
 
 
 ## Usage
 
 A typical scenario for working with a benchmark is as follows.
@@ -101,19 +105,23 @@
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
 - `bm.set_grid_kind(kind)` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
 
+- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm._c`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned).
+
 - `bm.set_max(i, x, y)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
 - `bm.set_min(i, x, y)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_cache(True)` - when calling this function with the `True` argument, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values.
+- `bm.set_log(True, cond, step, prefix)` - when calling this function with the `True` argument, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log.
+
+- `bm.set_cache(True)` - when calling this function with the `True` argument, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
 
 - `bm.set_quantization(True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
 ##### Computing benchmark values
 
@@ -174,12 +182,19 @@
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
 
-If you have interesting benchmarks, then we are happy to invite you to become a contributor. Please see detailed instructions for developers in `workflow.md`.
+
+## Contributors
+
+- [Anastasia Batsheva](https://github.com/anabatsh)
+
+We are happy to invite you to become a contributor, especially if you have interesting benchmarks ;) Please see detailed instructions for developers in `workflow.md`.
+
 
 ---
 
+
 > ✭__🚂  The stars that you give to **teneva_bm**, motivate us to develop faster and add new interesting features to the code 😃
```

### Comparing `teneva_bm-0.2.0/README.md` & `teneva_bm-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.2.0".
+> Current version "0.3.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
 
@@ -26,30 +26,34 @@
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
 bm = BmQuboMaxcut().prep()
 print(bm.info())
 ```
 
-You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_amba`). You can also use a function from the `teneva_bm` package to run all or only one demo:
+You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
-teneva_bm_demo('bm_qubo_knap_amba', with_info=True)
+teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
+> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.2`).
+
 
 ## Available benchmarks
 
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores.
 
+- `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
+
 - `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
 
-- `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapAmba`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
-    > The exact global minimum is known only for `BmQuboKnapAmba` benchmark.
+- `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
+    > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
 
 - `various` - a collection of heterogeneous benchmarks that are not suitable for any other collection (note that in this case, we do not use the name of the collection in the name of the benchmarks, unlike all other sets). The collection includes the following benchmarks: `BmMatmul`, `BmTopopt` (draft!), `BmWallSimple`.
 
 
 ## Usage
 
 A typical scenario for working with a benchmark is as follows.
@@ -75,19 +79,23 @@
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
 - `bm.set_grid_kind(kind)` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
 
+- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm._c`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned).
+
 - `bm.set_max(i, x, y)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
 - `bm.set_min(i, x, y)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_cache(True)` - when calling this function with the `True` argument, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values.
+- `bm.set_log(True, cond, step, prefix)` - when calling this function with the `True` argument, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log.
+
+- `bm.set_cache(True)` - when calling this function with the `True` argument, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
 
 - `bm.set_quantization(True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
 ##### Computing benchmark values
 
@@ -148,12 +156,19 @@
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
 
-If you have interesting benchmarks, then we are happy to invite you to become a contributor. Please see detailed instructions for developers in `workflow.md`.
+
+## Contributors
+
+- [Anastasia Batsheva](https://github.com/anabatsh)
+
+We are happy to invite you to become a contributor, especially if you have interesting benchmarks ;) Please see detailed instructions for developers in `workflow.md`.
+
 
 ---
 
+
 > ✭__🚂  The stars that you give to **teneva_bm**, motivate us to develop faster and add new interesting features to the code 😃
```

### Comparing `teneva_bm-0.2.0/demo.py` & `teneva_bm-0.3.0/demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/setup.py` & `teneva_bm-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/bm.py` & `teneva_bm-0.3.0/teneva_bm/bm.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 
         self.set_size(d, n)
         self.set_quantization()
 
         self.set_name(name)
         self.set_desc(desc)
 
+        self.set_constr()
+
         self.set_min()
         self.set_max()
 
         self.set_grid()
         self.set_grid_kind()
 
         self.set_opts()
 
         self.set_cache()
 
+        self.set_log()
+
     def __call__(self, X):
         """Return a value or batch of values for provided x-point."""
         return self.get_poi(X)
 
     def __getitem__(self, I):
         """Return a value or batch of values for provided multi-index."""
         return self.get(I)
@@ -59,14 +63,26 @@
         return not self.is_n_even
 
     @property
     def is_tens(self):
         """Check if BM relates to tensor (i.e., discrete function)."""
         return not self.is_func
 
+    @property
+    def n0(self):
+        """Return the mode size value if it is constant."""
+        if not self.is_n_equal:
+            raise ValueError('Mode size is not constant, can not get n0')
+        return self.n[0]
+
+    @property
+    def with_constr(self):
+        """Return True if benchmark has a constant."""
+        return False
+
     def build_cores(self):
         """Return exact TT-cores for the TT-representation of the tensor."""
         if self.is_tens:
             msg = 'Construction of the TT-cores does not work for tensors'
             raise ValueError(msg)
 
         I = np.array([teneva.grid_flat(k) for k in self.n], dtype=int).T
@@ -102,18 +118,14 @@
 
     def check(self):
         """Check that benchmark's configuration is valid."""
         if not self.is_prep:
             msg = 'Run "prep" method for BM before call it'
             self.set_err(msg)
 
-        if self.with_constr and self.penalty_constr is None:
-            msg = 'Penalty for constraint ("bm.penalty_constr") is not set'
-            self.set_err(msg)
-
         return self.check_err()
 
     def check_err(self):
         """Check that benchmark has not errors."""
         if len(self.err):
             msg = f'BM "{self.name}" is not ready'
             for e in self.err:
@@ -226,27 +238,64 @@
         elif self.y_max is not None:
             text += 'Maximum (found)                          : '
             text += f'{self.y_max:-10.3e}\n'
 
         text += '=' * 78 + '\n'
         return text
 
+    def log(self, postfix='', out=False):
+        self.log_m_last = self.m
+        t = tpc() - self.log_t
+
+        text = ''
+
+        if self.log_prefix:
+            text += self.log_prefix + ' > '
+
+        text += f'm {self.m:-7.1e}'
+        if self.with_cache:
+            text += f' [+ {self.m_cache:-7.1e}]'
+        text += ' | '
+
+        text += f't {t:-7.1e} | '
+
+        if self.log_with_min:
+            text += f'min {self.y_min:-10.3e} | '
+
+        if self.log_with_max:
+            text += f'max {self.y_max:-10.3e} | '
+
+        if postfix:
+            text = text + postfix
+
+        if out:
+            print(text)
+
+        return text
+
     def prep(self):
         """A function with a specific benchmark preparation code."""
         # Note that when inherited, the function in the child class
         # must starts with the following line:
         self.check_err()
 
         # and should ends with the following two lines:
         self.is_prep = True
         return self
 
-    def set_cache(self, with_cache=False, cache=None):
+    def set_cache(self, with_cache=False, cache=None, m_max=1.E+8):
         self.with_cache = with_cache
         self.cache = {} if cache is None else cache
+        self.cache_m_max = int(m_max) if m_max else None
+
+    def set_constr(self, penalty=1.E+42, eps=1.E-16, with_amplitude=True):
+        """Set constraint options."""
+        self.constr_penalty = penalty
+        self.constr_eps = eps
+        self.constr_with_amplitude = with_amplitude
 
     def set_desc(self, desc=''):
         """Set text description of the problem."""
         self.desc = desc
 
     def set_err(self, err=''):
         """Set the error text (can not import external module, etc.)."""
@@ -269,26 +318,55 @@
         """
         self.grid_kind = kind
 
         if not self.grid_kind in ['uni', 'cheb']:
             msg = f'Invalid kind of the grid (should be "uni" or "cheb")'
             raise ValueError(msg)
 
+    def set_log(self, with_log=False, cond='min-max', step=1000, prefix='bm',
+                with_min=True, with_max=True):
+        """Set the log options."""
+        self.with_log = with_log
+        self.log_cond = cond
+        self.log_step = int(step) if step else None
+        self.log_prefix = prefix
+        self.log_with_min = with_min
+        self.log_with_max = with_max
+
+        self.log_t = tpc()
+
+        if not self.log_cond in ['min', 'max', 'min-max', 'step']:
+            raise ValueError('Invalid "log_cond" argument')
+
     def set_max(self, i=None, x=None, y=None):
         """Set exact (real) global maximum (index, point and related value)."""
         self.i_max_real = i
         self.x_max_real = x
         self.y_max_real = y
 
+        if self.i_max_real is not None:
+            self.i_max_real = np.asanyarray(self.i_max_real, dtype=int)
+        if self.x_max_real is not None:
+            self.x_max_real = np.asanyarray(self.x_max_real, dtype=float)
+        if self.y_max_real is not None:
+            self.y_max_real = float(self.y_max_real)
+
     def set_min(self, i=None, x=None, y=None):
         """Set exact (real) global minimum (index, point and related value)."""
         self.i_min_real = i
         self.x_min_real = x
         self.y_min_real = y
 
+        if self.i_min_real is not None:
+            self.i_min_real = np.asanyarray(self.i_min_real, dtype=int)
+        if self.x_min_real is not None:
+            self.x_min_real = np.asanyarray(self.x_min_real, dtype=float)
+        if self.y_min_real is not None:
+            self.y_min_real = float(self.y_min_real)
+
     def set_name(self, name=''):
         """Set display name for the problem."""
         self.name = name
 
     def set_opts(self):
         """Setting options specific to the benchmark."""
         return
@@ -312,30 +390,35 @@
             raise ValueError(msg)
 
     def set_size(self, d=None, n=None):
         """Set dimension (d) and sizes for all d-modes (n: int or list)."""
         self.d = None if d is None else int(d)
         self.n = teneva.grid_prep_opt(n, self.d, int)
 
+    def _c(self, x):
+        """Function that check constraint for a given point/index."""
+        return self._c_batch(np.array(x).reshape(1, -1))[0]
+
+    def _c_batch(self, X):
+        """Function that check constraint for a given batch of poi./indices."""
+        return np.array([self._c(x) for x in X])
+
     def _compute(self, X):
         if not self.with_constr:
             return self._f_batch(X)
 
-        y = np.ones(X.shape[0]) * self.penalty_constr
-        ind = self._constr_batch(X)
-        y[ind] = self._f_batch(X[ind])
-        return y
+        y = np.ones(X.shape[0]) * self.constr_penalty
+        c = self._c_batch(X)
+        ind = c < self.constr_eps
 
-    def _constr(self, x):
-        """Function that check constraint for a given point/index."""
-        return self._constr_batch(np.array(x).reshape(1, -1))[0]
+        y[ind] = self._f_batch(X[ind])
+        if self.constr_with_amplitude:
+            y[~ind] *= c[~ind]
 
-    def _constr_batch(self, X):
-        """Function that check constraint for a given batch of poi./indices."""
-        return np.array([self._constr(x) for x in X])
+        return y
 
     def _cores(self, X):
         """Return the exact TT-cores for the provided points."""
         raise NotImplementedError()
 
     def _cores_add(self, X, a0=0):
         """Helper function for the construction of the TT-cores."""
@@ -364,34 +447,51 @@
     def _f_batch(self, X):
         """Function that computes values for a given batch of points/indices."""
         return np.array([self._f(x) for x in X])
 
     def _init(self):
         self.err = []
 
+        self.is_y_max_new = False
         self.i_max = None
         self.x_max = None
         self.y_max = None
 
+        self.is_y_min_new = False
         self.i_min = None
         self.x_min = None
         self.y_min = None
 
         self.y_list = []
 
         self.m = 0
         self.m_cache = 0
         self.time = 0.
 
-        self.penalty_constr = None
+        self.log_m_last = 0
 
         self.is_prep = False
-        self.with_constr = False
         self.with_cores = False
 
+    def _log_check(self):
+        if not self.with_log:
+            return False
+
+        if self.log_cond == 'min':
+            return self.is_y_min_new
+
+        if self.log_cond == 'max':
+            return self.is_y_max_new
+
+        if self.log_cond == 'min-max':
+            return self.is_y_min_new or self.is_y_max_new
+
+        if self.log_cond == 'step':
+            return self.log_step and self.m - self.log_m_last > self.log_step
+
     def _parse_input(self, I=None, X=None):
         if I is not None and X is not None:
             raise ValueError('Invalid case')
 
         if I is None and X is None:
             raise ValueError('Invalid case')
 
@@ -437,23 +537,37 @@
         self.m += y.shape[0] - dm_cache
         self.m_cache += dm_cache
 
         self.time += tpc() - t
 
         ind = np.argmax(y)
         if self.y_max is None or self.y_max < y[ind]:
+            self.is_y_max_new = True
             self.i_max = I[ind, :] if I is not None else None
             self.x_max = X[ind, :] if X is not None else None
             self.y_max = y[ind]
+        else:
+            self.is_y_max_new = False
+
 
         ind = np.argmin(y)
         if self.y_min is None or self.y_min > y[ind]:
+            self.is_y_min_new = True
             self.i_min = I[ind, :] if I is not None else None
             self.x_min = X[ind, :] if X is not None else None
             self.y_min = y[ind]
+        else:
+            self.is_y_min_new = False
+
+        if self._log_check():
+            print(self.log())
+
+        if self.cache_m_max and len(self.cache.keys()) > self.cache_m_max:
+            self._wrn('The maximum cache size has been exceeded. Cache cleared')
+            self.cache = {}
 
         return y if is_batch else y[0]
 
     def _unquantize(self, I_qtt):
         if len(I_qtt.shape) == 1:
             is_many = False
             I_qtt = I_qtt.reshape(1, -1)
@@ -467,7 +581,11 @@
 
         I = np.zeros((m, d), dtype=I_qtt.dtype)
         for k in range(d):
             I_qtt_curr = I_qtt[:, q*k:q*(k+1)].T
             I[:, k] = np.ravel_multi_index(I_qtt_curr, n, order='F')
 
         return I if is_many else I[0, :]
+
+    def _wrn(self, text):
+        text = '!!! BM-WARNING | ' + text
+        print(text)
```

### Comparing `teneva_bm-0.2.0/teneva_bm/func/__init__.py` & `teneva_bm-0.3.0/teneva_bm/func/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_ackley.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_ackley.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_alpine.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_alpine.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_dixon.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_dixon.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_exp.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_exp.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_griewank.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_griewank.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_michalewicz.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_michalewicz.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_piston.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_piston.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_qing.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_qing.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_rastrigin.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_rastrigin.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_rosenbrock.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_schaffer.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_schaffer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/func/bm_func_schwefel.py` & `teneva_bm-0.3.0/teneva_bm/func/bm_func_schwefel.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/oc/bm_oc_simple.py` & `teneva_bm-0.3.0/teneva_bm/oc/bm_oc_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/oc/bm_oc_simple_constr.py` & `teneva_bm-0.3.0/teneva_bm/oc/bm_oc_simple_constr.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,40 +4,44 @@
 
 from teneva_bm.oc import BmOcSimple
 
 
 DESC = """
     Discrete optimal control (OC) problem with constraint of the special
     form. This benchmark is the same as "BmOcSimple", except the constraint.
-    Please see the description of BmOcSimple for more details. Note that in
-    the case if constraint fails, we return the penalty value "1.E+42".
+    Please see the description of BmOcSimple for more details.
     The dimension may be any (default is 50), and the mode size should be 2.
     The benchmark needs "gekko==1.0.6" library (it is used for ODE solution).
+    Note that the default penalty for the constraint is "1.E+42"
+    and the amplitude of the constraint does not used.
 """
 
 
 class BmOcSimpleConstr(BmOcSimple):
     def __init__(self, d=50, n=2, name='OcSimpleConstr', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.penalty_constr = 1.E+42
-        self.with_constr = True
+        self.set_constr(penalty=1.E+42, with_amplitude=True)
 
-    def _constr(self, i):
+    @property
+    def with_constr(self):
+        return True
+
+    def _c(self, i):
         s = ''.join([str(k) for k in i])
 
         condition_false = False
         condition_false = condition_false or s.startswith('10')
         condition_false = condition_false or s.startswith('110')
         condition_false = condition_false or s.startswith('01')
         condition_false = condition_false or s.startswith('011')
         condition_false = condition_false or s.startswith('010')
         condition_false = condition_false or s.startswith('0110')
 
-        return not condition_false
+        return 1. if condition_false else -1.
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmOcSimpleConstr().prep()
     print(bm.info())
```

### Comparing `teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_knap_amba.py` & `teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,90 +2,89 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Binary knapsack problem with fixed weights wi in [5, 20], profits pi in
-    [50, 100] (i = 1, 2, . . . , d) and the maximum capacity C = 1000. It is
-    from the work (Dong et al., 2021) (problem k3; d = 50), where angle
-    modulated bat algorithm (AMBA) was proposed for high-dimensional binary
-    optimization problems with application to antenna topology optimization.
-    The dimension should be 50, and the mode size should be 2; the exact
-    global minimum is known: i = [1, 1, 0, ...] (see code), y = -3103.
+    Continuous optimal control (OC) problem with constraints:
+    .------------------------------.
+    | F(i) -> min s.t. C(i) = True |
+    .------------------------------.
+    i - integer control
+        i[0] = 4.9 | >= -10 | <= 10
+        i[1] = 0.1 | >= -10 | <= 10
+    F - objective function
+        (i[0] - 5)^2 + i[1]^2 - 25
+    C - constraints
+        i[0]^2 <= i[1]
+    The best value is ~-8.498 and the corresponding solution is [~1.23, ~1.52]
+    The dimension d is 2, and the mode size is 21.
 """
 
 
-class BmQuboKnapAmba(Bm):
-    def __init__(self, d=50, n=2, name='QuboKnapAmba', desc=DESC):
+class BmHS011(Bm):
+    def __init__(self, d=3, n=21, name='hs11', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        if self.d != 50:
-            self.set_err('Dimension should be "50"')
-        if not self.is_n_equal or self.n[0] != 2:
-            self.set_err('Mode size (n) should be "2"')
-
-        self.set_min(i=np.array([
-            1, 1, 0, 1, 0, 1, 0, 1, 1, 1, 1, 0, 1, 1, 0, 1, 1, 0,
-            1, 1, 0, 1, 1, 1, 1, 1, 1, 1, 0, 1, 0, 0, 0, 0, 1, 0,
-            1, 0, 0, 1, 1, 0, 0, 0, 0, 0, 1, 0, 0, 0], dtype=int),
-            y=-3103.)
+        self.set_grid(-10, 10)
+
+        self.set_min(
+            i=None,
+            x=np.array([1.23, 1.52]),
+            y=-8.498
+        )
 
     @property
-    def is_tens(self):
+    def is_func(self):
         return True
-
-    def prep(self):
-        self.check_err()
-        
-        self.bm_w = [
-            80, 82, 85, 70, 72, 70, 66, 50, 55, 25, 50, 55, 40, 48, 59, 32, 22,
-            60, 30, 32, 40, 38, 35, 32, 25, 28, 30, 22, 50, 30, 45, 30, 60, 50,
-            20, 65, 20, 25, 30, 10, 20, 25, 15, 10, 10, 10, 4, 4, 2, 1]
-
-        self.bm_p = [
-            220, 208, 198, 192, 180, 180, 165, 162, 160, 158, 155, 130, 125,
-            122, 120, 118, 115, 110, 105, 101, 100, 100, 98, 96, 95, 90, 88, 82,
-            80, 77, 75, 73, 72, 70, 69, 66, 65, 63, 60, 58, 56, 50, 30, 20, 15,
-            10, 8, 5, 3, 1]
-
-        self.bm_C = 1000
-
-        self.is_prep = True
-        return self
-
-    def _f(self, i):
-        cost = np.dot(self.bm_p, i)
-        constr = np.dot(self.bm_w, i)
-        return 0 if constr > self.bm_C else -cost
+    
+    def bm_constr(self, X):
+        y = X[:, 0] ** 2 <= X[:, 1]
+        return ~y
+
+    def _f_batch_good(self, X):
+        y = (X[:, 0] - 5) ** 2 + X[:, 1] ** 2 - 25
+        return y
+
+    def _f_batch(self, X):
+        mask = self.bm_constr(X)
+        y = np.zeros(X.shape[0])
+        y[~mask] = 1.E+10
+        if any(mask):
+            y[mask] = self._f_batch_good(X[mask])
+        return y
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmQuboKnapAmba().prep()
+    bm = BmHS011().prep()
     print(bm.info())
 
-    I_trn, y_trn = bm.build_trn(1.E+4)
-    print(bm.info_history())
+    text = 'Range of y for 10 random samples : '
+    bm.build_trn(1.E+1)
+    text += f'[{np.min(bm.y_trn):-10.3e},'
+    text += f' {np.max(bm.y_trn):-10.3e}] '
+    text += f'(avg: {np.mean(bm.y_trn):-10.3e})'
+    print(text)
 
-    text = 'Value at a random multi-index            :  '
+    text = 'Value at a random multi-index     :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices          :  '
+    text = 'Value at 3 random multi-indices   :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    text = 'Value at the minimum (real vs calc)      :  '
+    text = 'Value at minimum (real vs calc)   :  '
     y_real = bm.y_min_real
-    y_calc = bm[bm.i_min_real]
-    text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
+    y_calc = bm(bm.x_min_real)
+    text += f'{y_real:-10.3e}/ {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_knap_quad.py` & `teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_knap_quad.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_maxcut.py` & `teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_maxcut.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/qubo/bm_qubo_mvc.py` & `teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_mvc.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/teneva_bm_demo.py` & `teneva_bm-0.3.0/teneva_bm/teneva_bm_demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/various/bm_matmul.py` & `teneva_bm-0.3.0/teneva_bm/various/bm_matmul.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/various/bm_topopt.py` & `teneva_bm-0.3.0/teneva_bm/various/bm_topopt.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm/various/bm_wall_simple.py` & `teneva_bm-0.3.0/teneva_bm/various/bm_wall_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.2.0/teneva_bm.egg-info/PKG-INFO` & `teneva_bm-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: teneva-bm
-Version: 0.2.0
+Name: teneva_bm
+Version: 0.3.0
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,15 +30,15 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.2.0".
+> Current version "0.3.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
 
@@ -52,30 +52,34 @@
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
 bm = BmQuboMaxcut().prep()
 print(bm.info())
 ```
 
-You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_amba`). You can also use a function from the `teneva_bm` package to run all or only one demo:
+You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
-teneva_bm_demo('bm_qubo_knap_amba', with_info=True)
+teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
+> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.2`).
+
 
 ## Available benchmarks
 
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
     > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores.
 
+- `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
+
 - `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
 
-- `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapAmba`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
-    > The exact global minimum is known only for `BmQuboKnapAmba` benchmark.
+- `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
+    > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
 
 - `various` - a collection of heterogeneous benchmarks that are not suitable for any other collection (note that in this case, we do not use the name of the collection in the name of the benchmarks, unlike all other sets). The collection includes the following benchmarks: `BmMatmul`, `BmTopopt` (draft!), `BmWallSimple`.
 
 
 ## Usage
 
 A typical scenario for working with a benchmark is as follows.
@@ -101,19 +105,23 @@
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
 - `bm.set_grid_kind(kind)` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
 
+- `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm._c`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned).
+
 - `bm.set_max(i, x, y)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
 - `bm.set_min(i, x, y)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_cache(True)` - when calling this function with the `True` argument, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values.
+- `bm.set_log(True, cond, step, prefix)` - when calling this function with the `True` argument, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log.
+
+- `bm.set_cache(True)` - when calling this function with the `True` argument, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
 
 - `bm.set_quantization(True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
 ##### Computing benchmark values
 
@@ -174,12 +182,19 @@
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
 
-If you have interesting benchmarks, then we are happy to invite you to become a contributor. Please see detailed instructions for developers in `workflow.md`.
+
+## Contributors
+
+- [Anastasia Batsheva](https://github.com/anabatsh)
+
+We are happy to invite you to become a contributor, especially if you have interesting benchmarks ;) Please see detailed instructions for developers in `workflow.md`.
+
 
 ---
 
+
 > ✭__🚂  The stars that you give to **teneva_bm**, motivate us to develop faster and add new interesting features to the code 😃
```

