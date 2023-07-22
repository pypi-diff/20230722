# Comparing `tmp/ddbox-0.1.3.tar.gz` & `tmp/ddbox-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddbox-0.1.3.tar", max compression
+gzip compressed data, was "ddbox-0.1.4.tar", max compression
```

## Comparing `ddbox-0.1.3.tar` & `ddbox-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0        0 2023-07-21 18:14:30.198837 ddbox-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-02 16:40:01.000000 ddbox-0.1.3/ddbox/__init__.py
--rw-r--r--   0        0        0     6148 2023-07-21 12:57:54.261925 ddbox-0.1.3/ddbox/bin/.DS_Store
--rwxr-xr-x   0        0        0  4089576 2023-07-21 12:57:33.278474 ddbox-0.1.3/ddbox/bin/vina_1.2.5_linux_x86_64
--rwxr-xr-x   0        0        0  1297344 2023-07-21 12:57:33.571825 ddbox-0.1.3/ddbox/bin/vina_1.2.5_mac_x86_64
--rw-r--r--   0        0        0      279 2023-07-21 18:49:24.527234 ddbox-0.1.3/ddbox/configs.py
--rw-r--r--   0        0        0     1763 2023-07-22 08:31:29.751506 ddbox-0.1.3/ddbox/data/torch.py
--rw-r--r--   0        0        0        0 2023-07-21 17:42:23.416142 ddbox-0.1.3/ddbox/data/utils/__init__.py
--rw-r--r--   0        0        0     4476 2023-07-22 08:29:22.913023 ddbox-0.1.3/ddbox/data/utils/loaders.py
--rw-r--r--   0        0        0      320 2023-05-27 09:00:08.000000 ddbox-0.1.3/ddbox/datasets/smallworld.py
--rw-r--r--   0        0        0      495 2023-05-27 08:58:38.000000 ddbox-0.1.3/ddbox/datasets/zinc.py
--rw-r--r--   0        0        0        0 2023-07-21 18:52:46.441179 ddbox-0.1.3/ddbox/docking/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 15:41:03.059597 ddbox-0.1.3/ddbox/docking/utils/__init__.py
--rw-r--r--   0        0        0     4048 2023-07-21 18:26:43.606148 ddbox-0.1.3/ddbox/docking/utils/vina.py
--rw-r--r--   0        0        0     1409 2023-07-21 18:52:26.381364 ddbox-0.1.3/ddbox/docking/vina.py
--rw-r--r--   0        0        0     6148 2023-07-21 11:44:43.785208 ddbox-0.1.3/ddbox/metrics/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-05 17:27:37.000000 ddbox-0.1.3/ddbox/metrics/SA_Score/__init__.py
--rw-r--r--   0        0        0  3848394 2023-06-05 17:33:36.000000 ddbox-0.1.3/ddbox/metrics/SA_Score/fpscores.pkl.gz
--rw-r--r--   0        0        0     5815 2023-06-07 15:48:53.000000 ddbox-0.1.3/ddbox/metrics/SA_Score/sascorer.py
--rw-r--r--   0        0        0      262 2023-06-17 07:00:52.000000 ddbox-0.1.3/ddbox/metrics/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 11:44:48.652936 ddbox-0.1.3/ddbox/metrics/benchmarks/__init__.py
--rw-r--r--   0        0        0     3267 2023-07-21 11:44:48.653147 ddbox-0.1.3/ddbox/metrics/benchmarks/moses.py
--rw-r--r--   0        0        0      739 2023-06-04 17:35:43.000000 ddbox-0.1.3/ddbox/metrics/data/mcf.csv
--rw-r--r--   0        0        0   207419 2023-06-07 15:48:53.000000 ddbox-0.1.3/ddbox/metrics/data/wehi_pains.csv
--rw-r--r--   0        0        0     2096 2023-07-21 18:26:42.682662 ddbox-0.1.3/ddbox/metrics/distribution_difference.py
--rw-r--r--   0        0        0      415 2023-07-21 18:26:42.668963 ddbox-0.1.3/ddbox/metrics/fcd.py
--rw-r--r--   0        0        0     1636 2023-07-21 18:26:42.678205 ddbox-0.1.3/ddbox/metrics/fraction_passes.py
--rw-r--r--   0        0        0      630 2023-07-21 18:26:42.683229 ddbox-0.1.3/ddbox/metrics/fraction_unique.py
--rw-r--r--   0        0        0      458 2023-06-11 15:03:10.000000 ddbox-0.1.3/ddbox/metrics/fraction_valid.py
--rw-r--r--   0        0        0      906 2023-07-21 18:26:42.679502 ddbox-0.1.3/ddbox/metrics/fragment.py
--rw-r--r--   0        0        0      638 2023-07-21 18:26:42.662217 ddbox-0.1.3/ddbox/metrics/intdiv.py
--rw-r--r--   0        0        0        0 2023-06-17 06:53:06.000000 ddbox-0.1.3/ddbox/metrics/novelty.py
--rw-r--r--   0        0        0     1171 2023-07-21 18:26:42.667781 ddbox-0.1.3/ddbox/metrics/scaffold.py
--rw-r--r--   0        0        0      434 2023-07-21 18:26:42.668394 ddbox-0.1.3/ddbox/metrics/snn.py
--rw-r--r--   0        0        0     3468 2023-06-07 15:48:54.000000 ddbox-0.1.3/ddbox/metrics/utils.py
--rw-r--r--   0        0        0       76 2023-07-21 18:26:42.680031 ddbox-0.1.3/ddbox/molecule/__init__.py
--rw-r--r--   0        0        0     4445 2023-07-21 18:26:42.671450 ddbox-0.1.3/ddbox/molecule/descriptors.py
--rw-r--r--   0        0        0    10805 2023-07-21 18:26:43.660690 ddbox-0.1.3/ddbox/molecule/objects.py
--rw-r--r--   0        0        0       66 2023-06-11 15:02:40.000000 ddbox-0.1.3/ddbox/registries.py
--rw-r--r--   0        0        0     1265 2023-07-21 18:26:43.685212 ddbox-0.1.3/ddbox/utils.py
--rw-r--r--   0        0        0      472 2023-07-22 09:03:28.927351 ddbox-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 ddbox-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 18:14:30.198837 ddbox-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 16:40:01.000000 ddbox-0.1.4/ddbox/__init__.py
+-rw-r--r--   0        0        0     6148 2023-07-21 12:57:54.261925 ddbox-0.1.4/ddbox/bin/.DS_Store
+-rwxr-xr-x   0        0        0  4089576 2023-07-21 12:57:33.278474 ddbox-0.1.4/ddbox/bin/vina_1.2.5_linux_x86_64
+-rwxr-xr-x   0        0        0  1297344 2023-07-21 12:57:33.571825 ddbox-0.1.4/ddbox/bin/vina_1.2.5_mac_x86_64
+-rw-r--r--   0        0        0      279 2023-07-21 18:49:24.527234 ddbox-0.1.4/ddbox/configs.py
+-rw-r--r--   0        0        0     1763 2023-07-22 08:31:29.751506 ddbox-0.1.4/ddbox/data/torch.py
+-rw-r--r--   0        0        0        0 2023-07-21 17:42:23.416142 ddbox-0.1.4/ddbox/data/utils/__init__.py
+-rw-r--r--   0        0        0     4476 2023-07-22 08:29:22.913023 ddbox-0.1.4/ddbox/data/utils/loaders.py
+-rw-r--r--   0        0        0      320 2023-05-27 09:00:08.000000 ddbox-0.1.4/ddbox/datasets/smallworld.py
+-rw-r--r--   0        0        0      495 2023-05-27 08:58:38.000000 ddbox-0.1.4/ddbox/datasets/zinc.py
+-rw-r--r--   0        0        0        0 2023-07-21 18:52:46.441179 ddbox-0.1.4/ddbox/docking/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:41:03.059597 ddbox-0.1.4/ddbox/docking/utils/__init__.py
+-rw-r--r--   0        0        0     4048 2023-07-21 18:26:43.606148 ddbox-0.1.4/ddbox/docking/utils/vina.py
+-rw-r--r--   0        0        0     2358 2023-07-22 09:12:17.349865 ddbox-0.1.4/ddbox/docking/vina.py
+-rw-r--r--   0        0        0     6148 2023-07-21 11:44:43.785208 ddbox-0.1.4/ddbox/metrics/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-05 17:27:37.000000 ddbox-0.1.4/ddbox/metrics/SA_Score/__init__.py
+-rw-r--r--   0        0        0  3848394 2023-06-05 17:33:36.000000 ddbox-0.1.4/ddbox/metrics/SA_Score/fpscores.pkl.gz
+-rw-r--r--   0        0        0     5815 2023-06-07 15:48:53.000000 ddbox-0.1.4/ddbox/metrics/SA_Score/sascorer.py
+-rw-r--r--   0        0        0      262 2023-06-17 07:00:52.000000 ddbox-0.1.4/ddbox/metrics/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:44:48.652936 ddbox-0.1.4/ddbox/metrics/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3267 2023-07-21 11:44:48.653147 ddbox-0.1.4/ddbox/metrics/benchmarks/moses.py
+-rw-r--r--   0        0        0      739 2023-06-04 17:35:43.000000 ddbox-0.1.4/ddbox/metrics/data/mcf.csv
+-rw-r--r--   0        0        0   207419 2023-06-07 15:48:53.000000 ddbox-0.1.4/ddbox/metrics/data/wehi_pains.csv
+-rw-r--r--   0        0        0     2096 2023-07-21 18:26:42.682662 ddbox-0.1.4/ddbox/metrics/distribution_difference.py
+-rw-r--r--   0        0        0      415 2023-07-21 18:26:42.668963 ddbox-0.1.4/ddbox/metrics/fcd.py
+-rw-r--r--   0        0        0     1636 2023-07-21 18:26:42.678205 ddbox-0.1.4/ddbox/metrics/fraction_passes.py
+-rw-r--r--   0        0        0      630 2023-07-21 18:26:42.683229 ddbox-0.1.4/ddbox/metrics/fraction_unique.py
+-rw-r--r--   0        0        0      458 2023-06-11 15:03:10.000000 ddbox-0.1.4/ddbox/metrics/fraction_valid.py
+-rw-r--r--   0        0        0      906 2023-07-21 18:26:42.679502 ddbox-0.1.4/ddbox/metrics/fragment.py
+-rw-r--r--   0        0        0      638 2023-07-21 18:26:42.662217 ddbox-0.1.4/ddbox/metrics/intdiv.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:53:06.000000 ddbox-0.1.4/ddbox/metrics/novelty.py
+-rw-r--r--   0        0        0     1171 2023-07-21 18:26:42.667781 ddbox-0.1.4/ddbox/metrics/scaffold.py
+-rw-r--r--   0        0        0      434 2023-07-21 18:26:42.668394 ddbox-0.1.4/ddbox/metrics/snn.py
+-rw-r--r--   0        0        0     3468 2023-06-07 15:48:54.000000 ddbox-0.1.4/ddbox/metrics/utils.py
+-rw-r--r--   0        0        0       76 2023-07-21 18:26:42.680031 ddbox-0.1.4/ddbox/molecule/__init__.py
+-rw-r--r--   0        0        0     4445 2023-07-21 18:26:42.671450 ddbox-0.1.4/ddbox/molecule/descriptors.py
+-rw-r--r--   0        0        0    10805 2023-07-21 18:26:43.660690 ddbox-0.1.4/ddbox/molecule/objects.py
+-rw-r--r--   0        0        0       66 2023-06-11 15:02:40.000000 ddbox-0.1.4/ddbox/registries.py
+-rw-r--r--   0        0        0     1265 2023-07-21 18:26:43.685212 ddbox-0.1.4/ddbox/utils.py
+-rw-r--r--   0        0        0      472 2023-07-22 09:12:47.664826 ddbox-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 ddbox-0.1.4/PKG-INFO
```

### Comparing `ddbox-0.1.3/ddbox/bin/.DS_Store` & `ddbox-0.1.4/ddbox/bin/.DS_Store`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/bin/vina_1.2.5_linux_x86_64` & `ddbox-0.1.4/ddbox/bin/vina_1.2.5_linux_x86_64`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/bin/vina_1.2.5_mac_x86_64` & `ddbox-0.1.4/ddbox/bin/vina_1.2.5_mac_x86_64`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/data/torch.py` & `ddbox-0.1.4/ddbox/data/torch.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/data/utils/loaders.py` & `ddbox-0.1.4/ddbox/data/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/docking/utils/vina.py` & `ddbox-0.1.4/ddbox/docking/utils/vina.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/docking/vina.py` & `ddbox-0.1.4/ddbox/docking/vina.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,7 +42,36 @@
     output, err = p.communicate()
     if p.returncode != 0:
         raise Exception(err.decode())
 
     *name, ext = ligand_path.split('.')
     name = '.'.join(name)
     return '%s_out.%s' % (name, ext)
+
+
+def vina_docking_files(receptor_path: str, ligand_path: str, config_path: str, center: Tuple[float, float, float] | None = None, size: Tuple[float, float, float] | None = None):
+    command = [
+        get_vina_filepath(),
+        '--receptor', receptor_path,
+        '--ligand', ligand_path,
+        '--config', config_path,
+    ]
+    if center is not None:
+        command.extend([
+            '--center_x', str(center[0]),
+            '--center_y', str(center[1]),
+            '--center_z', str(center[2]),
+        ])
+    if size is not None:
+        command.extend([
+            '--size_x', str(size[0]),
+            '--size_y', str(size[1]),
+            '--size_z', str(size[2]),
+        ])
+    p = Popen(command, stdout=PIPE, stderr=PIPE)
+    output, err = p.communicate()
+    if p.returncode != 0:
+        raise Exception(err.decode())
+
+    *name, ext = ligand_path.split('.')
+    name = '.'.join(name)
+    return '%s_out.%s' % (name, ext)
```

### Comparing `ddbox-0.1.3/ddbox/metrics/.DS_Store` & `ddbox-0.1.4/ddbox/metrics/.DS_Store`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/SA_Score/fpscores.pkl.gz` & `ddbox-0.1.4/ddbox/metrics/SA_Score/fpscores.pkl.gz`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/SA_Score/sascorer.py` & `ddbox-0.1.4/ddbox/metrics/SA_Score/sascorer.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/benchmarks/moses.py` & `ddbox-0.1.4/ddbox/metrics/benchmarks/moses.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/data/mcf.csv` & `ddbox-0.1.4/ddbox/metrics/data/mcf.csv`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/data/wehi_pains.csv` & `ddbox-0.1.4/ddbox/metrics/data/wehi_pains.csv`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/distribution_difference.py` & `ddbox-0.1.4/ddbox/metrics/distribution_difference.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/fraction_passes.py` & `ddbox-0.1.4/ddbox/metrics/fraction_passes.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/fraction_unique.py` & `ddbox-0.1.4/ddbox/metrics/fraction_unique.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/fragment.py` & `ddbox-0.1.4/ddbox/metrics/fragment.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/intdiv.py` & `ddbox-0.1.4/ddbox/metrics/intdiv.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/scaffold.py` & `ddbox-0.1.4/ddbox/metrics/scaffold.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/metrics/utils.py` & `ddbox-0.1.4/ddbox/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/molecule/descriptors.py` & `ddbox-0.1.4/ddbox/molecule/descriptors.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/molecule/objects.py` & `ddbox-0.1.4/ddbox/molecule/objects.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/ddbox/utils.py` & `ddbox-0.1.4/ddbox/utils.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.3/PKG-INFO` & `ddbox-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddbox
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Azamat
 Author-email: unawares15@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

