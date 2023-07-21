# Comparing `tmp/idem-k8s-1.0.1.tar.gz` & `tmp/idem-k8s-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-k8s-1.0.1.tar", last modified: Thu Jul 13 20:34:41 2023, max compression
+gzip compressed data, was "idem-k8s-2.0.0.tar", last modified: Fri Jul 21 22:10:09 2023, max compression
```

## Comparing `idem-k8s-1.0.1.tar` & `idem-k8s-2.0.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.011719 idem-k8s-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    11336 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7122 2023-07-13 20:34:41.011719 idem-k8s-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6284 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/acct/k8s/
--rw-r--r--   0 root         (0) root         (0)      547 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/acct/k8s/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/autogen/k8s/
--rw-r--r--   0 root         (0) root         (0)     1580 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/autogen/k8s/init.py
--rw-r--r--   0 root         (0) root         (0)     6464 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/autogen/k8s/openapi_spec_parser.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/autogen/k8s/plugin.py
--rw-r--r--   0 root         (0) root         (0)    10897 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/autogen/k8s/template.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/autogen/k8s/type.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/exec/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/exec/k8s/apiregistration_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)     3837 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/exec/k8s/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/exec/k8s/core/v1/
--rw-r--r--   0 root         (0) root         (0)     4356 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/exec/k8s/core/v1/service.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/exec/k8s/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/exec/k8s/rbac/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/exec/k8s/rbac/v1/
--rw-r--r--   0 root         (0) root         (0)     4595 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/exec/k8s/rbac/v1/role_binding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/states/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/states/k8s/apiregistration_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/states/k8s/apiregistration_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)     9891 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/states/k8s/apps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/states/k8s/apps/v1/
--rw-r--r--   0 root         (0) root         (0)    13115 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/apps/v1/daemon_set.py
--rw-r--r--   0 root         (0) root         (0)    13334 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/apps/v1/deployment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/states/k8s/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/
--rw-r--r--   0 root         (0) root         (0)    10073 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/config_map.py
--rw-r--r--   0 root         (0) root         (0)     9167 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/namespace.py
--rw-r--r--   0 root         (0) root         (0)    11017 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py
--rw-r--r--   0 root         (0) root         (0)     9756 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/secret.py
--rw-r--r--   0 root         (0) root         (0)    11114 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/service.py
--rw-r--r--   0 root         (0) root         (0)    10444 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/service_account.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/states/k8s/rbac/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/states/k8s/rbac/v1/
--rw-r--r--   0 root         (0) root         (0)     8356 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/rbac/v1/cluster_role.py
--rw-r--r--   0 root         (0) root         (0)     9040 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py
--rw-r--r--   0 root         (0) root         (0)     9953 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/rbac/v1/role_binding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/states/k8s/storage_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/states/k8s/storage_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)    10373 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/tool/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/tool/k8s/apiregistration_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)      653 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/tool/k8s/apps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/tool/k8s/apps/v1/
--rw-r--r--   0 root         (0) root         (0)      905 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py
--rw-r--r--   0 root         (0) root         (0)     3051 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/apps/v1/deployment_utils.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/client.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.003719 idem-k8s-1.0.1/idem_k8s/tool/k8s/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.011719 idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/
--rw-r--r--   0 root         (0) root         (0)      714 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/config_map_utils.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/namespace_utils.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/secret_utils.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/service_account_utils.py
--rw-r--r--   0 root         (0) root         (0)      845 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/service_utils.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/custom_waiter.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/marshaller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/tool/k8s/rbac/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.011719 idem-k8s-1.0.1/idem_k8s/tool/k8s/rbac/v1/
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/resolve.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s/tool/k8s/storage_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.011719 idem-k8s-1.0.1/idem_k8s/tool/k8s/storage_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)      848 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/idem_k8s/tool/k8s/waiter_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-13 20:34:40.000000 idem-k8s-1.0.1/idem_k8s/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:34:41.007719 idem-k8s-1.0.1/idem_k8s.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7122 2023-07-13 20:34:40.000000 idem-k8s-1.0.1/idem_k8s.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2225 2023-07-13 20:34:40.000000 idem-k8s-1.0.1/idem_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 20:34:40.000000 idem-k8s-1.0.1/idem_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-13 20:34:40.000000 idem-k8s-1.0.1/idem_k8s.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      144 2023-07-13 20:34:40.000000 idem-k8s-1.0.1/idem_k8s.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-13 20:34:40.000000 idem-k8s-1.0.1/idem_k8s.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 20:34:41.011719 idem-k8s-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2783 2023-07-13 20:34:26.000000 idem-k8s-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11336 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7123 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6284 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.407384 idem-k8s-2.0.0/idem_k8s/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/acct/k8s/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/acct/k8s/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.407384 idem-k8s-2.0.0/idem_k8s/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/autogen/k8s/
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/autogen/k8s/init.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/autogen/k8s/openapi_spec_parser.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/autogen/k8s/plugin.py
+-rw-r--r--   0 root         (0) root         (0)    10897 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/autogen/k8s/template.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/autogen/k8s/type.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.407384 idem-k8s-2.0.0/idem_k8s/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/exec/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/exec/k8s/apiregistration_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)     3837 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/exec/k8s/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/exec/k8s/core/v1/
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/exec/k8s/core/v1/service.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/exec/k8s/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/exec/k8s/rbac/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/exec/k8s/rbac/v1/
+-rw-r--r--   0 root         (0) root         (0)     4595 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/apiregistration_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)     9891 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/apps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/apps/v1/
+-rw-r--r--   0 root         (0) root         (0)    13115 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/apps/v1/daemon_set.py
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/apps/v1/deployment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/
+-rw-r--r--   0 root         (0) root         (0)    10073 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/config_map.py
+-rw-r--r--   0 root         (0) root         (0)     9167 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/namespace.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)     9756 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/secret.py
+-rw-r--r--   0 root         (0) root         (0)    11114 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/service.py
+-rw-r--r--   0 root         (0) root         (0)    10444 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/service_account.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/rbac/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/rbac/v1/
+-rw-r--r--   0 root         (0) root         (0)     8356 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py
+-rw-r--r--   0 root         (0) root         (0)     9040 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py
+-rw-r--r--   0 root         (0) root         (0)     9953 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/rbac/v1/role_binding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/states/k8s/storage_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/idem_k8s/states/k8s/storage_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)    10373 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/idem_k8s/tool/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/tool/k8s/apiregistration_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/tool/k8s/apps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/idem_k8s/tool/k8s/apps/v1/
+-rw-r--r--   0 root         (0) root         (0)      905 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/client.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/tool/k8s/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/
+-rw-r--r--   0 root         (0) root         (0)      714 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/secret_utils.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py
+-rw-r--r--   0 root         (0) root         (0)      845 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/service_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/custom_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/marshaller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/tool/k8s/rbac/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/idem_k8s/tool/k8s/rbac/v1/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/resolve.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s/tool/k8s/storage_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/idem_k8s/tool/k8s/storage_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)      848 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/idem_k8s/tool/k8s/waiter_utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-21 22:10:08.000000 idem-k8s-2.0.0/idem_k8s/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:10:09.411384 idem-k8s-2.0.0/idem_k8s.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7123 2023-07-21 22:10:09.000000 idem-k8s-2.0.0/idem_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-07-21 22:10:09.000000 idem-k8s-2.0.0/idem_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:10:09.000000 idem-k8s-2.0.0/idem_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-21 22:10:09.000000 idem-k8s-2.0.0/idem_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-21 22:10:09.000000 idem-k8s-2.0.0/idem_k8s.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-21 22:10:09.000000 idem-k8s-2.0.0/idem_k8s.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 22:10:09.415385 idem-k8s-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-07-21 22:09:55.000000 idem-k8s-2.0.0/setup.py
```

### Comparing `idem-k8s-1.0.1/LICENSE` & `idem-k8s-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/PKG-INFO` & `idem-k8s-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-k8s
-Version: 1.0.1
+Version: 2.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Naresh
 Author-email: nkumar5@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: autogen
 License-File: LICENSE
 
 ========
 idem-k8s
@@ -48,15 +48,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source or contributing to the project)*
 
   To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
```

### Comparing `idem-k8s-1.0.1/README.rst` & `idem-k8s-2.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source or contributing to the project)*
 
   To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
```

### Comparing `idem-k8s-1.0.1/idem_k8s/acct/k8s/init.py` & `idem-k8s-2.0.0/idem_k8s/acct/k8s/init.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/autogen/k8s/init.py` & `idem-k8s-2.0.0/idem_k8s/autogen/k8s/init.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/autogen/k8s/openapi_spec_parser.py` & `idem-k8s-2.0.0/idem_k8s/autogen/k8s/openapi_spec_parser.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/autogen/k8s/plugin.py` & `idem-k8s-2.0.0/idem_k8s/autogen/k8s/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/autogen/k8s/template.py` & `idem-k8s-2.0.0/idem_k8s/autogen/k8s/template.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/autogen/k8s/type.py` & `idem-k8s-2.0.0/idem_k8s/autogen/k8s/type.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py` & `idem-k8s-2.0.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py` & `idem-k8s-2.0.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/exec/k8s/core/v1/service.py` & `idem-k8s-2.0.0/idem_k8s/exec/k8s/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/exec/k8s/init.py` & `idem-k8s-2.0.0/idem_k8s/exec/k8s/init.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/exec/k8s/rbac/v1/role_binding.py` & `idem-k8s-2.0.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/apps/v1/daemon_set.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/apps/v1/daemon_set.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/apps/v1/deployment.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/config_map.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/namespace.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/secret.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/service.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/core/v1/service_account.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/rbac/v1/cluster_role.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/rbac/v1/role_binding.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/rbac/v1/role_binding.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py` & `idem-k8s-2.0.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/apps/v1/deployment_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/client.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/client.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/comment_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/config_map_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/namespace_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/secret_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/secret_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/service_account_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/core/v1/service_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/core/v1/service_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/custom_waiter.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/custom_waiter.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/marshaller.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/marshaller.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/resolve.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/resolve.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/state_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/test_state_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s/tool/k8s/waiter_utils.py` & `idem-k8s-2.0.0/idem_k8s/tool/k8s/waiter_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/idem_k8s.egg-info/PKG-INFO` & `idem-k8s-2.0.0/idem_k8s.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-k8s
-Version: 1.0.1
+Version: 2.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Naresh
 Author-email: nkumar5@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: autogen
 License-File: LICENSE
 
 ========
 idem-k8s
@@ -48,15 +48,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source or contributing to the project)*
 
   To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
```

### Comparing `idem-k8s-1.0.1/idem_k8s.egg-info/SOURCES.txt` & `idem-k8s-2.0.0/idem_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-k8s-1.0.1/setup.py` & `idem-k8s-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,25 +72,25 @@
     url="",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     entry_points={"console_scripts": [""]},
     cmdclass={"clean": Clean},
 )
```

