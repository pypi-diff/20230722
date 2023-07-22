# Comparing `tmp/threemystic_cloud_data_client-0.1.28.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.29.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.28.tar` & `threemystic_cloud_data_client-0.1.29.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    21547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/hatch.toml
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/pyproject.toml
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.28/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    13579 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/hatch.toml
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.29/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files 13% similar despite different names*

```diff
@@ -100,22 +100,22 @@
               ]
 
           
       return return_data      
            
     except Exception as err:
       print(err)
-      return {} 
+      return {}
 
   async def __process_get_resources_vm_nics(self, account, public_ips, *args, **kwargs):    
     try:
       client = NetworkManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
       return_data = {}
       for nic in self.get_cloud_client().sdk_request(
-          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True),
           lambda_sdk_command=lambda: client.network_interfaces.list_all()
         ):
           if nic.virtual_machine is None:
             continue
           
           nic_data = self.get_common().helper_type().dictionary().merge_dictionary([
             {},
@@ -165,33 +165,63 @@
         return {self.get_cloud_client().get_resource_id(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
            tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
            lambda_sdk_command=lambda: resource_client.resources.list(filter="resourceType eq 'Microsoft.Compute/virtualMachines'", expand="createdTime,changedTime,provisioningState")
           )
         }
     except:
         return {}
+    
+  async def __process_get_resources_vm_statuses(self, account, client, *args, **kwargs):
+    try:
+        return {self.get_cloud_client().get_resource_id(resource= resource): self.get_cloud_client().serialize_resource(resource= resource) for resource in self.get_cloud_client().sdk_request(
+           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True),
+           lambda_sdk_command=lambda: client.virtual_machines.list_all(
+            status_only= True
+           )
+          )
+        }
+    except:
+        return {}
 
   async def _process_account_data_get_vm_load_balancers(self, vm_nics, load_balancers_by_nics, *args, **kwargs):
     return_load_balancers = []
     
     for nic in vm_nics:
       if load_balancers_by_nics.get(self.get_cloud_client().get_resource_id(resource= nic)) is None:
         continue
         
       return_load_balancers += (load_balancers_by_nics.get(self.get_cloud_client().get_resource_id(resource= nic)))
       # I might look into the whole private IP agress later, the issue is I have to validate networks
       
     
     return return_load_balancers
   
+  def __process_get_resources_vm_get_state(self, instanceView, *args, **kwargs):
+    if instanceView is None:
+      return None
+    
+    statuses = instanceView.get("statuses")
+    if statuses is None:
+      return None
+    
+    for status in statuses:
+      if "powerstate/" in self.get_common().helper_type().string().set_case(string_value= status.get("code"), case= "lower"):
+        return self.get_common().helper_type().string().set_case(string_value= self.get_common().helper_type().string().split(
+          string_value= status.get("code"),
+          separator= "[/]"
+        )[-1], case= "upper")
+      
+    return None
   async def _process_account_data(self, account, loop, *args, **kwargs):
     client = ComputeManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
+
     public_ips = await self.__process_get_resources_vm_public_ips(account= account)
     tasks = {
         "resource": loop.create_task(self.__process_get_resources_vm(account= account)),
+        "vm_statuses": loop.create_task(self.__process_get_resources_vm_statuses(account= account, client= client)),
         "availability_sets": loop.create_task(self.__process_get_resources_vm_availability_sets(client= client, account= account)),
         "nics": loop.create_task(self.__process_get_resources_vm_nics(account= account, public_ips= public_ips)),
         "load_balancers": loop.create_task(self.__process_get_resources_vm_load_balancers(account= account, public_ips= public_ips)),
     }
 
     await asyncio.wait(tasks.values())
 
@@ -201,23 +231,34 @@
             {},
             await self.get_base_return_data(
               account= self.get_cloud_client().serialize_resource(resource= account),
               resource_id= self.get_cloud_client().get_resource_id(resource= item),
               resource= item,
               region= self.get_cloud_client().get_resource_location(resource= item),
               resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
-            ),
+            ),            
             {
+              "properties": {
+                "instanceView": self.get_common().helper_type().general().get_container_value(
+                  container= tasks["vm_statuses"].result().get(self.get_cloud_client().get_resource_id(resource= item)), 
+                  value_key= ["properties", "instanceView"])
+              }
+            },
+            {
+              "extra_longlived": True,
+              "extra_state": self.__process_get_resources_vm_get_state(instanceView= self.get_common().helper_type().general().get_container_value(
+                  container= tasks["vm_statuses"].result().get(self.get_cloud_client().get_resource_id(resource= item)), 
+                  value_key= ["properties", "instanceView"])),              
               "extra_resource": self.get_cloud_client().serialize_resource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id(resource= item))),
               "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
               "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
               "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
                 vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id(resource= item)),
                 load_balancers_by_nics = tasks["load_balancers"].result()
               ),
             },
           ]) for item in self.get_cloud_client().sdk_request(
-           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True),
            lambda_sdk_command=lambda: client.virtual_machines.list_all()
           )
         ]
     }
```

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 from threemystic_common.base_class.base_provider import base
 from abc import abstractmethod
 import asyncio, concurrent.futures, socket, errno
 from tqdm.asyncio import tqdm
 
 class cloud_data_client_provider_base_data(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(*args, **kwargs)   
+    super().__init__(*args, **kwargs)
     
     self._set_cloud_data_client(*args, **kwargs)
     self._set_client_name(*args, **kwargs)
     self._set_max_process_pool(*args, **kwargs)
     self._set_max_thread_pool(*args, **kwargs)
     self._set_data_start(*args, **kwargs)
 
+    self._process_preloaded_data(*args, **kwargs)
+
+  
   @abstractmethod
   def get_accounts(self):
     pass
   
   @abstractmethod
-  async def _process_account_data(self, **kwargs):
+  async def _process_account_data(self, *args, **kwargs):
     raise Exception("_process_account_data is not DEFINED")
   
+  @property
+  def required_extra_data(self, *args, **kwargs):
+    if hasattr(self, "_required_extra_data"):
+      return self._required_extra_data
+    
+    return {}
+  
+  @required_extra_data.setter
+  def required_extra_data(self, value, *args, **kwargs):
+    self._required_extra_data = value
+
+  def _process_preloaded_data(self, preloaded_data = None, *args, **kwargs):
+    pass
+  
   def get_data_start(self, *args, **kwargs):
     return self.__data_start
   
   def _set_data_start(self, *args, **kwargs):
     self.__data_start = self.get_common().helper_type().datetime().get()
 
   def get_max_process_pool(self, *args, **kwargs):
@@ -53,15 +70,15 @@
 
   def get_client_name(self, *args, **kwargs):
     return self._client_name
   
   def _set_client_name(self, data_action, *args, **kwargs):
     self._client_name = f"{self.get_provider()}-{data_action}-data"
   
-  async def _pre_load_main_process(self, *args, **kwargs):
+  async def _pre_load_main_process(self, pool, *args, **kwargs):
     pass
 
   async def _get_environment(self, account = None, resource = None, *args, **kwargs):
     resource_name = self.get_common().helper_type().string().set_case(string_value= self.get_cloud_client().get_resource_name(resource= resource), case= "lower")
     account_name = self.get_common().helper_type().string().set_case(string_value= self.get_cloud_client().get_account_name(account= account), case= "lower")
     
     if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= resource_name):
@@ -137,14 +154,30 @@
     
     
       
     except socket.error as e:
       if e.errno != errno.EPIPE:
         raise
 
+  async def _process_get_data_by_id(self, results, id_override = None, *args, **kwargs):
+    results_by_id = {}
+    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= id_override):
+      id_override = "extra_id"
+    for _, result_data in results.items():
+      for data in result_data:
+        results_by_id[data[id_override]] = data
+    
+    return results_by_id 
+  
+  async def get_data_by_id(self, results = None, id_override = None, *args, **kwargs):
+    if results is None:
+      results = await self.main( *args, **kwargs)
+      
+    return await self._process_get_data_by_id(results= results, id_override= id_override) 
+  
   async def __main_poolexecutor(self, *args, **kwargs):   
     with concurrent.futures.ThreadPoolExecutor(self.get_max_thread_pool()) as pool:
         return await self.main_process(
           pool= pool,
           **kwargs
         )
   
@@ -204,15 +237,15 @@
   
   def _process_data_filter_condition_in(self, condition, condition_value, data_value, *args, **kwargs):
     condition_settings = self._process_data_filter_condition_settings("in", condition)
 
     if condition_settings.get("case_insensitive") is True:
       data_value = self.get_common().helper_type().string().set_case(string_value= data_value, case= "lower")
       if self.get_common().helper_type().general().is_type(obj= condition_value, type_check= str):
-        condition_value = self.get_common().helper_type().string().set_case(string_value= value, case= "lower")
+        condition_value = self.get_common().helper_type().string().set_case(string_value= condition_value, case= "lower")
       elif self.get_common().helper_type().general().is_type(obj= condition_value, type_check= list):
         condition_value = [self.get_common().helper_type().string().set_case(string_value= value, case= "lower") for value in condition_value]
       else:
         raise self.get_common().exception().exception(
           exception_type = "argument"
         ).not_implemented(
           logger= self.get_common().get_logger(),
```

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.29/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/.gitignore` & `threemystic_cloud_data_client-0.1.29/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/LICENSE` & `threemystic_cloud_data_client-0.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/README.md` & `threemystic_cloud_data_client-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/hatch.toml` & `threemystic_cloud_data_client-0.1.29/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.28/pyproject.toml` & `threemystic_cloud_data_client-0.1.29/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,20 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.15",
-  "threemystic-cloud-client >= 0.1.46",
+  "threemystic-common >= 0.1.17",
+  "threemystic-cloud-client >= 0.1.47",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
+  "azure-mgmt-compute >= 29",
   "azure-mgmt-cosmosdb >= 9",
   "azure-mgmt-costmanagement >= 4",
   "azure-mgmt-dns >= 8",
   "azure-mgmt-keyvault >= 10",
   "azure-mgmt-managementgroups >= 1",
   "azure-mgmt-monitor >= 5",
   "azure-mgmt-network >= 23",
```

### Comparing `threemystic_cloud_data_client-0.1.28/PKG-INFO` & `threemystic_cloud_data_client-0.1.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.28
+Version: 0.1.29
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: azure-keyvault-administration>=4
 Requires-Dist: azure-keyvault-certificates>=4
 Requires-Dist: azure-keyvault-keys>=4
 Requires-Dist: azure-keyvault-secrets>=4
+Requires-Dist: azure-mgmt-compute>=29
 Requires-Dist: azure-mgmt-cosmosdb>=9
 Requires-Dist: azure-mgmt-costmanagement>=4
 Requires-Dist: azure-mgmt-dns>=8
 Requires-Dist: azure-mgmt-keyvault>=10
 Requires-Dist: azure-mgmt-managementgroups>=1
 Requires-Dist: azure-mgmt-monitor>=5
 Requires-Dist: azure-mgmt-network>=23
@@ -34,16 +35,16 @@
 Requires-Dist: azure-mgmt-redis>=14
 Requires-Dist: azure-mgmt-resourcegraph>=8
 Requires-Dist: azure-mgmt-sql>=3
 Requires-Dist: azure-mgmt-sqlvirtualmachine>=0.6
 Requires-Dist: azure-mgmt-subscription>=3
 Requires-Dist: azure-mgmt-synapse>=2
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-cloud-client>=0.1.46
-Requires-Dist: threemystic-common>=0.1.15
+Requires-Dist: threemystic-cloud-client>=0.1.47
+Requires-Dist: threemystic-common>=0.1.17
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
 Currently supports AWS/Azure
```

