# Comparing `tmp/prodvana-0.1.9.tar.gz` & `tmp/prodvana-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.1.9.tar", max compression
+gzip compressed data, was "prodvana-0.2.0.tar", max compression
```

## Comparing `prodvana-0.1.9.tar` & `prodvana-0.2.0.tar`

### file list

```diff
@@ -1,332 +1,329 @@
--rw-r--r--   0        0        0       81 2023-05-30 13:39:12.483857 prodvana-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-05-30 13:39:12.483857 prodvana-0.1.9/prodvana/__init__.py
--rw-r--r--   0        0        0     3529 2023-05-30 13:39:12.483857 prodvana-0.1.9/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.238541 prodvana-0.1.9/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.238541 prodvana-0.1.9/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.254541 prodvana-0.1.9/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0    19183 2023-06-14 17:30:52.062541 prodvana-0.1.9/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    18983 2023-06-14 17:30:52.202541 prodvana-0.1.9/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    22573 2023-06-14 17:30:52.062541 prodvana-0.1.9/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     6760 2023-06-14 17:30:52.202541 prodvana-0.1.9/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.242541 prodvana-0.1.9/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     4200 2023-06-14 17:30:51.990541 prodvana-0.1.9/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     4693 2023-06-14 17:30:52.126541 prodvana-0.1.9/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.990541 prodvana-0.1.9/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.126541 prodvana-0.1.9/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    24873 2023-06-14 17:30:51.994541 prodvana-0.1.9/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16394 2023-06-14 17:30:52.130541 prodvana-0.1.9/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-06-14 17:30:51.990541 prodvana-0.1.9/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-06-14 17:30:52.134541 prodvana-0.1.9/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2801 2023-06-14 17:30:51.986541 prodvana-0.1.9/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-06-14 17:30:52.130541 prodvana-0.1.9/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.986541 prodvana-0.1.9/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.130541 prodvana-0.1.9/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2294 2023-06-14 17:30:51.994541 prodvana-0.1.9/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-06-14 17:30:52.126541 prodvana-0.1.9/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.990541 prodvana-0.1.9/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.130541 prodvana-0.1.9/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.258541 prodvana-0.1.9/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0    13908 2023-06-14 17:30:52.078541 prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-06-14 17:30:52.218541 prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-06-14 17:30:52.082541 prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-06-14 17:30:52.222541 prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     5071 2023-06-14 17:30:52.082541 prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-06-14 17:30:52.222541 prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.082541 prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.218541 prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.254541 prodvana-0.1.9/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2876 2023-06-14 17:30:52.054541 prodvana-0.1.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1129 2023-06-14 17:30:52.194541 prodvana-0.1.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     2704 2023-06-14 17:30:52.054541 prodvana-0.1.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0      895 2023-06-14 17:30:52.194541 prodvana-0.1.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.246541 prodvana-0.1.9/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     6823 2023-06-14 17:30:52.022541 prodvana-0.1.9/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-06-14 17:30:52.162541 prodvana-0.1.9/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.022541 prodvana-0.1.9/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.166541 prodvana-0.1.9/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.242541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-14 17:30:51.966541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-06-14 17:30:52.102541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.982541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.110541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     2659 2023-06-14 17:30:51.974541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     2017 2023-06-14 17:30:52.118541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.966541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.106541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     5636 2023-06-14 17:30:51.982541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5454 2023-06-14 17:30:52.102541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.974541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.118541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     3849 2023-06-14 17:30:51.978541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
--rw-r--r--   0        0        0     4110 2023-06-14 17:30:52.122541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.982541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.110541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     1890 2023-06-14 17:30:51.970541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-06-14 17:30:52.110541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.986541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.106541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1384 2023-06-14 17:30:51.970541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-06-14 17:30:52.106541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.970541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.122541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     2541 2023-06-14 17:30:51.962541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-06-14 17:30:52.114541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.978541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.114541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     2516 2023-06-14 17:30:51.966541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-06-14 17:30:52.122541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.982541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.110541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0    12624 2023-06-14 17:30:51.962541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0    10735 2023-06-14 17:30:52.122541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.978541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.118541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    13896 2023-06-14 22:11:59.895323 prodvana-0.1.9/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15627 2023-06-14 22:11:59.895323 prodvana-0.1.9/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.962541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.122541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     1837 2023-06-14 17:30:51.986541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/ref_pb2.py
--rw-r--r--   0        0        0      743 2023-06-14 17:30:52.114541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/ref_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.974541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.110541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
--rw-r--r--   0        0        0     3229 2023-06-14 17:30:51.974541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-06-14 17:30:52.114541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.978541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.126541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2867 2023-06-14 17:30:51.970541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     3495 2023-06-14 17:30:52.118541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.966541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.102541 prodvana-0.1.9/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.246541 prodvana-0.1.9/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3597 2023-06-14 17:30:52.014541 prodvana-0.1.9/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4171 2023-06-14 17:30:52.158541 prodvana-0.1.9/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.018541 prodvana-0.1.9/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.154541 prodvana-0.1.9/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.254541 prodvana-0.1.9/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1648 2023-06-14 17:30:52.050541 prodvana-0.1.9/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-06-14 17:30:52.186541 prodvana-0.1.9/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.046541 prodvana-0.1.9/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.186541 prodvana-0.1.9/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.254541 prodvana-0.1.9/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2652 2023-06-14 17:30:52.054541 prodvana-0.1.9/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-06-14 17:30:52.190541 prodvana-0.1.9/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.050541 prodvana-0.1.9/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.190541 prodvana-0.1.9/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.254541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/__init__.py
--rw-r--r--   0        0        0     7432 2023-06-14 17:30:52.058541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/config_pb2.py
--rw-r--r--   0        0        0     6911 2023-06-14 17:30:52.194541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.058541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.194541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11893 2023-06-14 17:30:52.062541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
--rw-r--r--   0        0        0     7309 2023-06-14 17:30:52.198541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
--rw-r--r--   0        0        0    11002 2023-06-14 17:30:52.058541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3288 2023-06-14 17:30:52.198541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2686 2023-06-14 17:30:52.054541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/object_pb2.py
--rw-r--r--   0        0        0     1862 2023-06-14 17:30:52.198541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.058541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.198541 prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.250541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    35437 2023-06-14 17:30:52.026541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    28895 2023-06-14 17:30:52.166541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    20037 2023-06-14 17:30:52.026541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     5752 2023-06-14 17:30:52.166541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.250541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    42401 2023-06-14 17:30:52.030541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0    70107 2023-06-14 17:30:52.170541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.030541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.170541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     4037 2023-06-14 17:30:52.026541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     7935 2023-06-14 17:30:52.170541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.030541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.166541 prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.250541 prodvana-0.1.9/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    20651 2023-06-14 17:30:52.046541 prodvana-0.1.9/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    27158 2023-06-14 17:30:52.182541 prodvana-0.1.9/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.042541 prodvana-0.1.9/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.186541 prodvana-0.1.9/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    18211 2023-06-14 17:30:52.046541 prodvana-0.1.9/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    14932 2023-06-14 17:30:52.186541 prodvana-0.1.9/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    17792 2023-06-14 17:30:52.046541 prodvana-0.1.9/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     5195 2023-06-14 17:30:52.186541 prodvana-0.1.9/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.258541 prodvana-0.1.9/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     6416 2023-06-14 17:30:52.090541 prodvana-0.1.9/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     5547 2023-06-14 17:30:52.230541 prodvana-0.1.9/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-06-14 17:30:52.090541 prodvana-0.1.9/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-06-14 17:30:52.234541 prodvana-0.1.9/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3627 2023-06-14 17:30:52.094541 prodvana-0.1.9/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4131 2023-06-14 17:30:52.234541 prodvana-0.1.9/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.094541 prodvana-0.1.9/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.230541 prodvana-0.1.9/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    15940 2023-06-14 17:30:52.090541 prodvana-0.1.9/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    30800 2023-06-14 17:30:52.230541 prodvana-0.1.9/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.090541 prodvana-0.1.9/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.230541 prodvana-0.1.9/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.254541 prodvana-0.1.9/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     3041 2023-06-14 17:30:52.050541 prodvana-0.1.9/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-06-14 17:30:52.190541 prodvana-0.1.9/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.050541 prodvana-0.1.9/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.190541 prodvana-0.1.9/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.246541 prodvana-0.1.9/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0    14774 2023-06-14 17:30:52.018541 prodvana-0.1.9/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-06-14 17:30:52.158541 prodvana-0.1.9/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-06-14 17:30:52.018541 prodvana-0.1.9/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-06-14 17:30:52.158541 prodvana-0.1.9/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.258541 prodvana-0.1.9/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     5507 2023-06-14 17:30:52.086541 prodvana-0.1.9/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-06-14 17:30:52.226541 prodvana-0.1.9/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.086541 prodvana-0.1.9/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.226541 prodvana-0.1.9/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.258541 prodvana-0.1.9/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     1844 2023-06-14 17:30:52.066541 prodvana-0.1.9/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     1957 2023-06-14 17:30:52.206541 prodvana-0.1.9/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.066541 prodvana-0.1.9/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.202541 prodvana-0.1.9/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.250541 prodvana-0.1.9/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0    16162 2023-06-14 17:30:52.034541 prodvana-0.1.9/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0     9762 2023-06-14 17:30:52.174541 prodvana-0.1.9/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    14668 2023-06-14 17:30:52.030541 prodvana-0.1.9/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4779 2023-06-14 17:30:52.174541 prodvana-0.1.9/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2859 2023-06-14 17:30:52.034541 prodvana-0.1.9/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-06-14 17:30:52.170541 prodvana-0.1.9/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.034541 prodvana-0.1.9/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.174541 prodvana-0.1.9/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.242541 prodvana-0.1.9/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     2598 2023-06-14 17:30:52.010541 prodvana-0.1.9/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0     2595 2023-06-14 17:30:52.154541 prodvana-0.1.9/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.010541 prodvana-0.1.9/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.150541 prodvana-0.1.9/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    10003 2023-06-14 17:30:52.014541 prodvana-0.1.9/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-06-14 17:30:52.150541 prodvana-0.1.9/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.010541 prodvana-0.1.9/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.150541 prodvana-0.1.9/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.242541 prodvana-0.1.9/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     3412 2023-06-14 17:30:51.998541 prodvana-0.1.9/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2828 2023-06-14 17:30:52.134541 prodvana-0.1.9/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.002541 prodvana-0.1.9/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.138541 prodvana-0.1.9/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1907 2023-06-14 17:30:51.994541 prodvana-0.1.9/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1545 2023-06-14 17:30:52.142541 prodvana-0.1.9/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.998541 prodvana-0.1.9/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.138541 prodvana-0.1.9/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     8407 2023-06-14 17:30:51.998541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0     8891 2023-06-14 17:30:52.134541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.002541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.138541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10471 2023-06-14 17:30:52.002541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     6767 2023-06-14 17:30:52.138541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    10450 2023-06-14 17:30:51.994541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3113 2023-06-14 17:30:52.134541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     6409 2023-06-14 17:30:51.998541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4997 2023-06-14 17:30:52.142541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.998541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.142541 prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.242541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     3574 2023-06-14 17:30:52.002541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-06-14 17:30:52.150541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.006541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.146541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    12100 2023-06-14 17:30:52.010541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    12611 2023-06-14 17:30:52.146541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.006541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.146541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11989 2023-06-14 17:30:52.006541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0     7509 2023-06-14 17:30:52.142541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    13099 2023-06-14 17:30:52.006541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4150 2023-06-14 17:30:52.146541 prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.246541 prodvana-0.1.9/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     2441 2023-06-14 17:30:52.022541 prodvana-0.1.9/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2315 2023-06-14 17:30:52.162541 prodvana-0.1.9/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.018541 prodvana-0.1.9/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.158541 prodvana-0.1.9/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.258541 prodvana-0.1.9/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0     1551 2023-06-14 17:30:52.082541 prodvana-0.1.9/prodvana/proto/prodvana/runtimes/features_pb2.py
--rw-r--r--   0        0        0     1320 2023-06-14 17:30:52.222541 prodvana-0.1.9/prodvana/proto/prodvana/runtimes/features_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.086541 prodvana-0.1.9/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.222541 prodvana-0.1.9/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
--rw-r--r--   0        0        0     7542 2023-06-14 17:30:52.086541 prodvana-0.1.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6671 2023-06-14 17:30:52.226541 prodvana-0.1.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.086541 prodvana-0.1.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.226541 prodvana-0.1.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.246541 prodvana-0.1.9/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-14 17:30:52.022541 prodvana-0.1.9/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-06-14 17:30:52.162541 prodvana-0.1.9/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.022541 prodvana-0.1.9/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.162541 prodvana-0.1.9/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.258541 prodvana-0.1.9/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0    10074 2023-06-14 17:30:52.066541 prodvana-0.1.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-06-14 17:30:52.206541 prodvana-0.1.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-06-14 17:30:52.066541 prodvana-0.1.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-06-14 17:30:52.206541 prodvana-0.1.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.258541 prodvana-0.1.9/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     5498 2023-06-14 17:30:52.070541 prodvana-0.1.9/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     5760 2023-06-14 17:30:52.218541 prodvana-0.1.9/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.074541 prodvana-0.1.9/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.214541 prodvana-0.1.9/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2655 2023-06-14 17:30:52.070541 prodvana-0.1.9/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-06-14 17:30:52.218541 prodvana-0.1.9/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.078541 prodvana-0.1.9/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.214541 prodvana-0.1.9/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    34055 2023-06-15 18:20:55.958562 prodvana-0.1.9/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    47738 2023-06-15 18:20:55.962562 prodvana-0.1.9/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.078541 prodvana-0.1.9/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.210541 prodvana-0.1.9/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    47994 2023-06-14 17:30:52.070541 prodvana-0.1.9/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    38013 2023-06-14 17:30:52.214541 prodvana-0.1.9/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    33828 2023-06-14 17:30:52.074541 prodvana-0.1.9/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0     9674 2023-06-14 17:30:52.210541 prodvana-0.1.9/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2934 2023-06-14 17:30:52.078541 prodvana-0.1.9/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-06-14 17:30:52.210541 prodvana-0.1.9/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.074541 prodvana-0.1.9/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.214541 prodvana-0.1.9/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.246541 prodvana-0.1.9/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.246541 prodvana-0.1.9/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     8509 2023-06-14 17:30:52.014541 prodvana-0.1.9/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     5677 2023-06-14 17:30:52.154541 prodvana-0.1.9/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0     8214 2023-06-14 17:30:52.014541 prodvana-0.1.9/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     2318 2023-06-14 17:30:52.154541 prodvana-0.1.9/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.242541 prodvana-0.1.9/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1530 2023-06-14 17:30:51.962541 prodvana-0.1.9/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-06-14 17:30:52.098541 prodvana-0.1.9/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.958541 prodvana-0.1.9/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.102541 prodvana-0.1.9/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.250541 prodvana-0.1.9/prodvana/proto/prodvana/template/__init__.py
--rw-r--r--   0        0        0     2429 2023-06-14 17:30:52.042541 prodvana-0.1.9/prodvana/proto/prodvana/template/service_pb2.py
--rw-r--r--   0        0        0     1768 2023-06-14 17:30:52.182541 prodvana-0.1.9/prodvana/proto/prodvana/template/service_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.042541 prodvana-0.1.9/prodvana/proto/prodvana/template/service_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.182541 prodvana-0.1.9/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.254541 prodvana-0.1.9/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1505 2023-06-14 17:30:52.066541 prodvana-0.1.9/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1451 2023-06-14 17:30:52.202541 prodvana-0.1.9/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.062541 prodvana-0.1.9/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.202541 prodvana-0.1.9/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.238541 prodvana-0.1.9/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     2142 2023-06-14 17:30:51.958541 prodvana-0.1.9/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2646 2023-06-14 17:30:52.098541 prodvana-0.1.9/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:51.958541 prodvana-0.1.9/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.098541 prodvana-0.1.9/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.250541 prodvana-0.1.9/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     4805 2023-06-14 17:30:52.042541 prodvana-0.1.9/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-06-14 17:30:52.182541 prodvana-0.1.9/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.038541 prodvana-0.1.9/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.178541 prodvana-0.1.9/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.250541 prodvana-0.1.9/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     5412 2023-06-14 17:30:52.038541 prodvana-0.1.9/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-06-14 17:30:52.178541 prodvana-0.1.9/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.034541 prodvana-0.1.9/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.178541 prodvana-0.1.9/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    70832 2023-06-14 18:11:31.066654 prodvana-0.1.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    52034 2023-06-14 18:11:31.066654 prodvana-0.1.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    57702 2023-06-14 18:11:31.066654 prodvana-0.1.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    16676 2023-06-14 18:11:31.066654 prodvana-0.1.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-14 17:30:52.262541 prodvana-0.1.9/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    21204 2023-06-14 17:30:52.094541 prodvana-0.1.9/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-06-14 17:30:52.238541 prodvana-0.1.9/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-14 17:30:52.094541 prodvana-0.1.9/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-14 17:30:52.234541 prodvana-0.1.9/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-30 13:39:12.503857 prodvana-0.1.9/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-05-30 13:39:12.503857 prodvana-0.1.9/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-05-30 13:39:12.503857 prodvana-0.1.9/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     4079 2023-05-30 13:39:12.503857 prodvana-0.1.9/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     7140 2023-05-30 13:39:12.503857 prodvana-0.1.9/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      746 2023-06-15 18:22:03.830562 prodvana-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-07-07 23:25:26.643463 prodvana-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 23:25:26.643463 prodvana-0.2.0/prodvana/__init__.py
+-rw-r--r--   0        0        0     3529 2023-07-07 23:25:26.643463 prodvana-0.2.0/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.421700 prodvana-0.2.0/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.421700 prodvana-0.2.0/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0     9562 2023-07-19 21:15:42.121700 prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    19141 2023-07-19 21:15:42.277700 prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    22573 2023-07-19 21:15:42.121700 prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6760 2023-07-19 21:15:42.277700 prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     3521 2023-07-19 21:15:42.233700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     3485 2023-07-19 21:15:42.401700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.241700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.397700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15907 2023-07-19 21:15:42.237700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16830 2023-07-19 21:15:42.393700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-07-19 21:15:42.241700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-07-19 21:15:42.393700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2235 2023-07-19 21:15:42.241700 prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-07-19 21:15:42.397700 prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.241700 prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.393700 prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2011 2023-07-19 21:15:42.237700 prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-07-19 21:15:42.397700 prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.237700 prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.397700 prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0     8480 2023-07-19 21:15:42.213700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-07-19 21:15:42.373700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-07-19 21:15:42.217700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-07-19 21:15:42.373700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3181 2023-07-19 21:15:42.217700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-07-19 21:15:42.377700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.213700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.373700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-19 21:15:42.149700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1129 2023-07-19 21:15:42.309700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     2704 2023-07-19 21:15:42.149700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      895 2023-07-19 21:15:42.305700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     4830 2023-07-19 21:15:42.113700 prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-07-19 21:15:42.273700 prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.113700 prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.269700 prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1988 2023-07-19 21:15:42.177700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2.py
+-rw-r--r--   0        0        0     1667 2023-07-19 21:15:42.321700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.157700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.317700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1366 2023-07-19 21:15:42.157700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-07-19 21:15:42.317700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.153700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.325700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2864 2023-07-19 21:15:42.161700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     2933 2023-07-19 21:15:42.325700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.173700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.337700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4272 2023-07-19 21:15:42.153700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5454 2023-07-19 21:15:42.329700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.165700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.321700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3013 2023-07-19 21:15:42.177700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
+-rw-r--r--   0        0        0     4537 2023-07-19 21:15:42.329700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.161700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.313700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1738 2023-07-19 21:15:42.169700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-07-19 21:15:42.325700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.153700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.333700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1338 2023-07-19 21:15:42.169700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-07-19 21:15:42.309700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.177700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.321700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1838 2023-07-19 21:15:42.173700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-07-19 21:15:42.317700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.169700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.321700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1866 2023-07-19 21:15:42.165700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-07-19 21:15:42.317700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.153700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.313700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7815 2023-07-19 21:15:42.161700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0    10735 2023-07-19 21:15:42.313700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.169700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.333700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9143 2023-07-19 21:15:42.173700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15928 2023-07-19 21:15:42.329700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.165700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.309700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2686 2023-07-19 21:15:42.165700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-07-19 21:15:42.333700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.157700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.329700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2804 2023-07-19 21:15:42.157700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     3946 2023-07-19 21:15:42.325700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.173700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.309700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-19 21:15:42.117700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4656 2023-07-19 21:15:42.273700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.117700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.273700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1388 2023-07-19 21:15:42.209700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-07-19 21:15:42.369700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.209700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.369700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.421700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2079 2023-07-19 21:15:42.109700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-07-19 21:15:42.265700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.105700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.261700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/__init__.py
+-rw-r--r--   0        0        0     6161 2023-07-19 21:15:42.125700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2.py
+-rw-r--r--   0        0        0     8052 2023-07-19 21:15:42.285700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.133700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.289700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9291 2023-07-19 21:15:42.129700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
+-rw-r--r--   0        0        0     8986 2023-07-19 21:15:42.289700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
+-rw-r--r--   0        0        0    13097 2023-07-19 21:15:42.129700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3909 2023-07-19 21:15:42.289700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2015 2023-07-19 21:15:42.129700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2.py
+-rw-r--r--   0        0        0     1862 2023-07-19 21:15:42.285700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.133700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.285700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    22956 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    30187 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    22004 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6317 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    26696 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0    76423 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.137700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.293700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3517 2023-07-19 21:15:42.133700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     7935 2023-07-19 21:15:42.293700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.137700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.293700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    16774 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    37710 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.245700 prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.401700 prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12870 2023-07-19 21:15:42.245700 prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    18334 2023-07-19 21:15:42.401700 prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    21499 2023-07-19 21:15:42.245700 prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6311 2023-07-19 21:15:42.401700 prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     4801 2023-07-19 21:15:42.253700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     5547 2023-07-19 21:15:42.417700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-07-19 21:15:42.257700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-07-19 21:15:42.417700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2688 2023-07-19 21:15:42.253700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4131 2023-07-19 21:15:42.409700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.257700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.413700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10353 2023-07-19 21:15:42.257700 prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    30800 2023-07-19 21:15:42.413700 prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.257700 prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.413700 prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     2205 2023-07-19 21:15:42.233700 prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-07-19 21:15:42.389700 prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.233700 prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.389700 prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0     8344 2023-07-19 21:15:42.201700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-07-19 21:15:42.357700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-07-19 21:15:42.197700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-07-19 21:15:42.357700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     3762 2023-07-19 21:15:42.125700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-07-19 21:15:42.281700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.125700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.281700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-19 21:15:42.145700 prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     1957 2023-07-19 21:15:42.301700 prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.145700 prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.305700 prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0     9808 2023-07-19 21:15:42.145700 prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0     9762 2023-07-19 21:15:42.301700 prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    14668 2023-07-19 21:15:42.141700 prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4779 2023-07-19 21:15:42.301700 prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2568 2023-07-19 21:15:42.141700 prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-07-19 21:15:42.297700 prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.141700 prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.301700 prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     2038 2023-07-19 21:15:42.201700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0     2595 2023-07-19 21:15:42.361700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.201700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.361700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6748 2023-07-19 21:15:42.205700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-07-19 21:15:42.361700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.201700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.361700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     2777 2023-07-19 21:15:42.225700 prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2860 2023-07-19 21:15:42.389700 prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.229700 prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.381700 prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1716 2023-07-19 21:15:42.225700 prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1545 2023-07-19 21:15:42.385700 prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.229700 prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.381700 prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6615 2023-07-19 21:15:42.229700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0    10041 2023-07-19 21:15:42.389700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.225700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.385700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8167 2023-07-19 21:15:42.225700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     8325 2023-07-19 21:15:42.381700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    12468 2023-07-19 21:15:42.221700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3716 2023-07-19 21:15:42.381700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3938 2023-07-19 21:15:42.221700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4997 2023-07-19 21:15:42.385700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.221700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.385700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     2453 2023-07-19 21:15:42.193700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-07-19 21:15:42.353700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.197700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.349700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7193 2023-07-19 21:15:42.193700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    12716 2023-07-19 21:15:42.353700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.189700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.349700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10119 2023-07-19 21:15:42.189700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0    11055 2023-07-19 21:15:42.349700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    15129 2023-07-19 21:15:42.193700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4757 2023-07-19 21:15:42.353700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     1701 2023-07-19 21:15:42.149700 prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2315 2023-07-19 21:15:42.305700 prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.145700 prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.305700 prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0     1434 2023-07-19 21:15:42.205700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2.py
+-rw-r--r--   0        0        0     1320 2023-07-19 21:15:42.369700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.209700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.365700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4579 2023-07-19 21:15:42.205700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6995 2023-07-19 21:15:42.365700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.205700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.365700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-19 21:15:42.121700 prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-07-19 21:15:42.281700 prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.125700 prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.281700 prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0     6361 2023-07-19 21:15:42.117700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-07-19 21:15:42.273700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-07-19 21:15:42.117700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-07-19 21:15:42.277700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     4358 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     7117 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.189700 prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.337700 prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1908 2023-07-19 21:15:42.181700 prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-07-19 21:15:42.337700 prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.185700 prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.345700 prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    26309 2023-07-19 21:15:42.185700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    54314 2023-07-19 21:15:42.341700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.189700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.345700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    31947 2023-07-19 21:15:42.185700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    38013 2023-07-19 21:15:42.341700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    33828 2023-07-19 21:15:42.185700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     9674 2023-07-19 21:15:42.345700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2198 2023-07-19 21:15:42.181700 prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-07-19 21:15:42.337700 prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.181700 prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.341700 prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-19 21:15:42.213700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     5677 2023-07-19 21:15:42.369700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0     8214 2023-07-19 21:15:42.213700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     2318 2023-07-19 21:15:42.373700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1317 2023-07-19 21:15:42.109700 prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-07-19 21:15:42.265700 prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.109700 prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.265700 prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1361 2023-07-19 21:15:42.221700 prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1451 2023-07-19 21:15:42.377700 prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.217700 prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.377700 prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-19 21:15:42.113700 prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2817 2023-07-19 21:15:42.269700 prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.109700 prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.269700 prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     3089 2023-07-19 21:15:42.197700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-07-19 21:15:42.357700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.197700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.357700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     3274 2023-07-19 21:15:42.249700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-07-19 21:15:42.405700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.249700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.409700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    36604 2023-07-19 21:15:42.249700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    52034 2023-07-19 21:15:42.409700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    57702 2023-07-19 21:15:42.253700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    16676 2023-07-19 21:15:42.405700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-19 21:15:42.449700 prodvana-0.2.0/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    13684 2023-07-19 21:15:42.261700 prodvana-0.2.0/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-07-19 21:15:42.417700 prodvana-0.2.0/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-19 21:15:42.261700 prodvana-0.2.0/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-19 21:15:42.421700 prodvana-0.2.0/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     1434 2023-07-20 20:38:16.234138 prodvana-0.2.0/prodvana/utils/parameters.py
+-rw-r--r--   0        0        0     1731 2023-07-20 20:38:16.234138 prodvana-0.2.0/prodvana/utils/protections.py
+-rw-r--r--   0        0        0     4079 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     7140 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      746 2023-07-22 13:46:43.126029 prodvana-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.2.0/PKG-INFO
```

### Comparing `prodvana-0.1.9/prodvana/client.py` & `prodvana-0.2.0/prodvana/client.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -383,26 +383,30 @@
 global___RecordRolloutResp = RecordRolloutResp
 
 class ProxyAPIServerReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RUNTIME_ID_FIELD_NUMBER: builtins.int
     BLOB_FIELD_NUMBER: builtins.int
+    CONN_ID_FIELD_NUMBER: builtins.int
     runtime_id: builtins.str
     """Header"""
     blob: builtins.bytes
     """Everything after header"""
+    conn_id: builtins.str
+    """Debugging/logging bits"""
     def __init__(
         self,
         *,
         runtime_id: builtins.str = ...,
         blob: builtins.bytes = ...,
+        conn_id: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["blob", b"blob", "msg", b"msg", "runtime_id", b"runtime_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["blob", b"blob", "msg", b"msg", "runtime_id", b"runtime_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["blob", b"blob", "conn_id", b"conn_id", "msg", b"msg", "runtime_id", b"runtime_id"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["msg", b"msg"]) -> typing_extensions.Literal["runtime_id", "blob"] | None: ...
 
 global___ProxyAPIServerReq = ProxyAPIServerReq
 
 class ProxyAPIServerResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/application/application_config.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.capability import capability_pb2 as prodvana_dot_capability_dot_capability__pb2
 from prodvana.proto.prodvana.common_config import notification_pb2 as prodvana_dot_common__config_dot_notification__pb2
 from prodvana.proto.prodvana.release_channel import release_channel_config_pb2 as prodvana_dot_release__channel_dot_release__channel__config__pb2
-from prodvana.proto.prodvana.template import service_pb2 as prodvana_dot_template_dot_service__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-prodvana/application/application_config.proto\x12\x14prodvana.application\x1a$prodvana/capability/capability.proto\x1a)prodvana/common_config/notification.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\x1fprodvana/template/service.proto\x1a*prodvana/workflow/integration_config.proto\x1a\x17validate/validate.proto\"\xe8\x04\n\x11\x41pplicationConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12H\n\x10release_channels\x18\x02 \x03(\x0b\x32..prodvana.release_channel.ReleaseChannelConfig\x12\x41\n\rnotifications\x18\x04 \x01(\x0b\x32*.prodvana.common_config.NotificationConfig\x12\x31\n\x06\x61lerts\x18\x05 \x01(\x0b\x32!.prodvana.workflow.AlertingConfig\x12J\n\x0c\x63\x61pabilities\x18\x06 \x03(\x0b\x32%.prodvana.capability.CapabilityConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12Z\n\x14\x63\x61pability_instances\x18\x07 \x03(\x0b\x32-.prodvana.capability.CapabilityInstanceConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12L\n\x11service_templates\x18\x08 \x03(\x0b\x32\".prodvana.template.ServiceTemplateB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12,\n$enable_custom_tasks_dynamic_delivery\x18\n \x01(\x08J\x04\x08\x03\x10\x04J\x04\x08\t\x10\nR\x12pipeline_templatesR\x14use_dynamic_deliveryBPZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/applicationb\x06proto3')
-
-
-
-_APPLICATIONCONFIG = DESCRIPTOR.message_types_by_name['ApplicationConfig']
-ApplicationConfig = _reflection.GeneratedProtocolMessageType('ApplicationConfig', (_message.Message,), {
-  'DESCRIPTOR' : _APPLICATIONCONFIG,
-  '__module__' : 'prodvana.application.application_config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.application.ApplicationConfig)
-  })
-_sym_db.RegisterMessage(ApplicationConfig)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-prodvana/application/application_config.proto\x12\x14prodvana.application\x1a$prodvana/capability/capability.proto\x1a)prodvana/common_config/notification.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a\x17validate/validate.proto\"\xb1\x04\n\x11\x41pplicationConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12H\n\x10release_channels\x18\x02 \x03(\x0b\x32..prodvana.release_channel.ReleaseChannelConfig\x12\x41\n\rnotifications\x18\x04 \x01(\x0b\x32*.prodvana.common_config.NotificationConfig\x12\x31\n\x06\x61lerts\x18\x05 \x01(\x0b\x32!.prodvana.workflow.AlertingConfig\x12J\n\x0c\x63\x61pabilities\x18\x06 \x03(\x0b\x32%.prodvana.capability.CapabilityConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12Z\n\x14\x63\x61pability_instances\x18\x07 \x03(\x0b\x32-.prodvana.capability.CapabilityInstanceConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01J\x04\x08\x03\x10\x04J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bR\x11service_templatesR\x12pipeline_templatesR\x14use_dynamic_deliveryR$enable_custom_tasks_dynamic_deliveryBPZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/applicationb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.application.application_config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/application'
   _APPLICATIONCONFIG.fields_by_name['name']._options = None
   _APPLICATIONCONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
   _APPLICATIONCONFIG.fields_by_name['capabilities']._options = None
   _APPLICATIONCONFIG.fields_by_name['capabilities']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _APPLICATIONCONFIG.fields_by_name['capability_instances']._options = None
   _APPLICATIONCONFIG.fields_by_name['capability_instances']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
-  _APPLICATIONCONFIG.fields_by_name['service_templates']._options = None
-  _APPLICATIONCONFIG.fields_by_name['service_templates']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
-  _APPLICATIONCONFIG._serialized_start=310
-  _APPLICATIONCONFIG._serialized_end=926
+  _globals['_APPLICATIONCONFIG']._serialized_start=277
+  _globals['_APPLICATIONCONFIG']._serialized_end=838
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import prodvana.proto.prodvana.capability.capability_pb2
 import prodvana.proto.prodvana.common_config.notification_pb2
 import prodvana.proto.prodvana.release_channel.release_channel_config_pb2
-import prodvana.proto.prodvana.template.service_pb2
 import prodvana.proto.prodvana.workflow.integration_config_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
@@ -26,16 +25,14 @@
 
     NAME_FIELD_NUMBER: builtins.int
     RELEASE_CHANNELS_FIELD_NUMBER: builtins.int
     NOTIFICATIONS_FIELD_NUMBER: builtins.int
     ALERTS_FIELD_NUMBER: builtins.int
     CAPABILITIES_FIELD_NUMBER: builtins.int
     CAPABILITY_INSTANCES_FIELD_NUMBER: builtins.int
-    SERVICE_TEMPLATES_FIELD_NUMBER: builtins.int
-    ENABLE_CUSTOM_TASKS_DYNAMIC_DELIVERY_FIELD_NUMBER: builtins.int
     name: builtins.str
     @property
     def release_channels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig]: ...
     @property
     def notifications(self) -> prodvana.proto.prodvana.common_config.notification_pb2.NotificationConfig: ...
     @property
     def alerts(self) -> prodvana.proto.prodvana.workflow.integration_config_pb2.AlertingConfig: ...
@@ -44,33 +41,21 @@
         """capabilities are dependencies that services in this applications can use"""
     @property
     def capability_instances(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.capability.capability_pb2.CapabilityInstanceConfig]:
         """optional capability instances that can be referenced by `capabilities`, useful to deduplication.
         for example, you may choose to have two database capability instances, staging and prod,
         and use them across release channels staging, beta, and prod, where beta and prod use the prod db.
         """
-    @property
-    def service_templates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.template.service_pb2.ServiceTemplate]:
-        """service templates are sets of service configurations that can be used as the base of a service.
-        this is useful for setting default values that are kept in sync when the templates change.
-        """
-    enable_custom_tasks_dynamic_delivery: builtins.bool
-    """if set and use_dynamic_delivery is set, transform custom tasks to DD preconditions for all services.
-    Only used for safely migrating prime capabilities to DD.
-    UNUSED: Remove from proto once the flag has been removed from all persisted configs.
-    """
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         release_channels: collections.abc.Iterable[prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig] | None = ...,
         notifications: prodvana.proto.prodvana.common_config.notification_pb2.NotificationConfig | None = ...,
         alerts: prodvana.proto.prodvana.workflow.integration_config_pb2.AlertingConfig | None = ...,
         capabilities: collections.abc.Iterable[prodvana.proto.prodvana.capability.capability_pb2.CapabilityConfig] | None = ...,
         capability_instances: collections.abc.Iterable[prodvana.proto.prodvana.capability.capability_pb2.CapabilityInstanceConfig] | None = ...,
-        service_templates: collections.abc.Iterable[prodvana.proto.prodvana.template.service_pb2.ServiceTemplate] | None = ...,
-        enable_custom_tasks_dynamic_delivery: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["alerts", b"alerts", "notifications", b"notifications"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["alerts", b"alerts", "capabilities", b"capabilities", "capability_instances", b"capability_instances", "enable_custom_tasks_dynamic_delivery", b"enable_custom_tasks_dynamic_delivery", "name", b"name", "notifications", b"notifications", "release_channels", b"release_channels", "service_templates", b"service_templates"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["alerts", b"alerts", "capabilities", b"capabilities", "capability_instances", b"capability_instances", "name", b"name", "notifications", b"notifications", "release_channels", b"release_channels"]) -> None: ...
 
 global___ApplicationConfig = ApplicationConfig
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -89,31 +89,39 @@
 class ConfigureApplicationReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLICATION_CONFIG_FIELD_NUMBER: builtins.int
     APPROVED_DANGEROUS_ACTION_IDS_FIELD_NUMBER: builtins.int
     SOURCE_FIELD_NUMBER: builtins.int
     SOURCE_METADATA_FIELD_NUMBER: builtins.int
+    BASE_VERSION_FIELD_NUMBER: builtins.int
     @property
     def application_config(self) -> prodvana.proto.prodvana.application.application_config_pb2.ApplicationConfig: ...
     @property
     def approved_dangerous_action_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType
     @property
     def source_metadata(self) -> prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata: ...
+    base_version: builtins.str
+    """optional, if this is not a new application, this is the existing version of 
+    this application config that this configuration was based on.
+    this can be used to avoid concurrent updates overwriting each other.
+    NOTE: this will eventually be required for updates
+    """
     def __init__(
         self,
         *,
         application_config: prodvana.proto.prodvana.application.application_config_pb2.ApplicationConfig | None = ...,
         approved_dangerous_action_ids: collections.abc.Iterable[builtins.str] | None = ...,
         source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType = ...,
         source_metadata: prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata | None = ...,
+        base_version: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["application_config", b"application_config", "source_metadata", b"source_metadata"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application_config", b"application_config", "approved_dangerous_action_ids", b"approved_dangerous_action_ids", "source", b"source", "source_metadata", b"source_metadata"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application_config", b"application_config", "approved_dangerous_action_ids", b"approved_dangerous_action_ids", "base_version", b"base_version", "source", b"source", "source_metadata", b"source_metadata"]) -> None: ...
 
 global___ConfigureApplicationReq = ConfigureApplicationReq
 
 class ConfigureApplicationResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/application/object.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.application import application_config_pb2 as prodvana_dot_application_dot_application__config__pb2
 from prodvana.proto.prodvana.application import user_metadata_pb2 as prodvana_dot_application_dot_user__metadata__pb2
 from prodvana.proto.prodvana.object import meta_pb2 as prodvana_dot_object_dot_meta__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/application/object.proto\x12\x14prodvana.application\x1a-prodvana/application/application_config.proto\x1a(prodvana/application/user_metadata.proto\x1a\x1aprodvana/object/meta.proto\"5\n\x10\x41pplicationStateJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03R\nis_defaultR\tis_legacy\"\xee\x01\n\x0b\x41pplication\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x37\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\'.prodvana.application.ApplicationConfig\x12\x35\n\x05state\x18\x03 \x01(\x0b\x32&.prodvana.application.ApplicationState\x12\x44\n\ruser_metadata\x18\x04 \x01(\x0b\x32-.prodvana.application.ApplicationUserMetadataBPZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/applicationb\x06proto3')
 
-
-
-_APPLICATIONSTATE = DESCRIPTOR.message_types_by_name['ApplicationState']
-_APPLICATION = DESCRIPTOR.message_types_by_name['Application']
-ApplicationState = _reflection.GeneratedProtocolMessageType('ApplicationState', (_message.Message,), {
-  'DESCRIPTOR' : _APPLICATIONSTATE,
-  '__module__' : 'prodvana.application.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.application.ApplicationState)
-  })
-_sym_db.RegisterMessage(ApplicationState)
-
-Application = _reflection.GeneratedProtocolMessageType('Application', (_message.Message,), {
-  'DESCRIPTOR' : _APPLICATION,
-  '__module__' : 'prodvana.application.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.application.Application)
-  })
-_sym_db.RegisterMessage(Application)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.application.object_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/application'
-  _APPLICATIONSTATE._serialized_start=176
-  _APPLICATIONSTATE._serialized_end=229
-  _APPLICATION._serialized_start=232
-  _APPLICATION._serialized_end=470
+  _globals['_APPLICATIONSTATE']._serialized_start=176
+  _globals['_APPLICATIONSTATE']._serialized_end=229
+  _globals['_APPLICATION']._serialized_start=232
+  _globals['_APPLICATION']._serialized_end=470
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/application/user_metadata.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.common_config import links_pb2 as prodvana_dot_common__config_dot_links__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(prodvana/application/user_metadata.proto\x12\x14prodvana.application\x1a\"prodvana/common_config/links.proto\x1a\x17validate/validate.proto\"\x9f\x01\n\x17\x41pplicationUserMetadata\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12+\n\x05links\x18\x02 \x03(\x0b\x32\x1c.prodvana.common_config.Link\x12\x42\n\rservice_links\x18\x03 \x03(\x0b\x32\x1c.prodvana.common_config.LinkB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42PZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/applicationb\x06proto3')
 
-
-
-_APPLICATIONUSERMETADATA = DESCRIPTOR.message_types_by_name['ApplicationUserMetadata']
-ApplicationUserMetadata = _reflection.GeneratedProtocolMessageType('ApplicationUserMetadata', (_message.Message,), {
-  'DESCRIPTOR' : _APPLICATIONUSERMETADATA,
-  '__module__' : 'prodvana.application.user_metadata_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.application.ApplicationUserMetadata)
-  })
-_sym_db.RegisterMessage(ApplicationUserMetadata)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.application.user_metadata_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/application'
   _APPLICATIONUSERMETADATA.fields_by_name['service_links']._options = None
   _APPLICATIONUSERMETADATA.fields_by_name['service_links']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
-  _APPLICATIONUSERMETADATA._serialized_start=128
-  _APPLICATIONUSERMETADATA._serialized_end=287
+  _globals['_APPLICATIONUSERMETADATA']._serialized_start=128
+  _globals['_APPLICATIONUSERMETADATA']._serialized_end=287
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/blobs/blobs_manager.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"prodvana/blobs/blobs_manager.proto\x12\x0eprodvana.blobs\x1a\x1cgoogle/api/annotations.proto\x1a\x17validate/validate.proto\"$\n\rGetCasBlobReq\x12\x13\n\x02id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x1f\n\x0eGetCasBlobResp\x12\r\n\x05\x62ytes\x18\x01 \x01(\x0c\x32{\n\x0c\x42lobsManager\x12k\n\nGetCasBlob\x12\x1d.prodvana.blobs.GetCasBlobReq\x1a\x1e.prodvana.blobs.GetCasBlobResp\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/blobs/cas/{id=*}0\x01\x42JZHgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/blobsb\x06proto3')
 
-
-
-_GETCASBLOBREQ = DESCRIPTOR.message_types_by_name['GetCasBlobReq']
-_GETCASBLOBRESP = DESCRIPTOR.message_types_by_name['GetCasBlobResp']
-GetCasBlobReq = _reflection.GeneratedProtocolMessageType('GetCasBlobReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETCASBLOBREQ,
-  '__module__' : 'prodvana.blobs.blobs_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.blobs.GetCasBlobReq)
-  })
-_sym_db.RegisterMessage(GetCasBlobReq)
-
-GetCasBlobResp = _reflection.GeneratedProtocolMessageType('GetCasBlobResp', (_message.Message,), {
-  'DESCRIPTOR' : _GETCASBLOBRESP,
-  '__module__' : 'prodvana.blobs.blobs_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.blobs.GetCasBlobResp)
-  })
-_sym_db.RegisterMessage(GetCasBlobResp)
-
-_BLOBSMANAGER = DESCRIPTOR.services_by_name['BlobsManager']
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.blobs.blobs_manager_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZHgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/blobs'
   _GETCASBLOBREQ.fields_by_name['id']._options = None
   _GETCASBLOBREQ.fields_by_name['id']._serialized_options = b'\372B\004r\002\020\001'
   _BLOBSMANAGER.methods_by_name['GetCasBlob']._options = None
   _BLOBSMANAGER.methods_by_name['GetCasBlob']._serialized_options = b'\202\323\344\223\002\026\022\024/v1/blobs/cas/{id=*}'
-  _GETCASBLOBREQ._serialized_start=109
-  _GETCASBLOBREQ._serialized_end=145
-  _GETCASBLOBRESP._serialized_start=147
-  _GETCASBLOBRESP._serialized_end=178
-  _BLOBSMANAGER._serialized_start=180
-  _BLOBSMANAGER._serialized_end=303
+  _globals['_GETCASBLOBREQ']._serialized_start=109
+  _globals['_GETCASBLOBREQ']._serialized_end=145
+  _globals['_GETCASBLOBRESP']._serialized_start=147
+  _globals['_GETCASBLOBRESP']._serialized_end=178
+  _globals['_BLOBSMANAGER']._serialized_start=180
+  _globals['_BLOBSMANAGER']._serialized_end=303
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/common_config/dangerous_action.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-prodvana/common_config/dangerous_action.proto\x12\x16prodvana.common_config\"2\n\x0f\x44\x61ngerousAction\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x65xplanation\x18\x02 \x01(\tBRZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
-
-
-_DANGEROUSACTION = DESCRIPTOR.message_types_by_name['DangerousAction']
-DangerousAction = _reflection.GeneratedProtocolMessageType('DangerousAction', (_message.Message,), {
-  'DESCRIPTOR' : _DANGEROUSACTION,
-  '__module__' : 'prodvana.common_config.dangerous_action_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.DangerousAction)
-  })
-_sym_db.RegisterMessage(DangerousAction)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.common_config.dangerous_action_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
-  _DANGEROUSACTION._serialized_start=73
-  _DANGEROUSACTION._serialized_end=123
+  _globals['_DANGEROUSACTION']._serialized_start=73
+  _globals['_DANGEROUSACTION']._serialized_end=123
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,42 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/common_config/env.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n prodvana/common_config/env.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\"w\n\x08\x45nvValue\x12\x0f\n\x05value\x18\x01 \x01(\tH\x00\x12\x14\n\nraw_secret\x18\x02 \x01(\tH\x00\x12\x30\n\x06secret\x18\x03 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x12\n\x0bvalue_oneof\x12\x03\xf8\x42\x01\"8\n\x06Secret\x12\x14\n\x03key\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07version\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
-
-
-
-_ENVVALUE = DESCRIPTOR.message_types_by_name['EnvValue']
-_SECRET = DESCRIPTOR.message_types_by_name['Secret']
-EnvValue = _reflection.GeneratedProtocolMessageType('EnvValue', (_message.Message,), {
-  'DESCRIPTOR' : _ENVVALUE,
-  '__module__' : 'prodvana.common_config.env_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.EnvValue)
-  })
-_sym_db.RegisterMessage(EnvValue)
-
-Secret = _reflection.GeneratedProtocolMessageType('Secret', (_message.Message,), {
-  'DESCRIPTOR' : _SECRET,
-  '__module__' : 'prodvana.common_config.env_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.Secret)
-  })
-_sym_db.RegisterMessage(Secret)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n prodvana/common_config/env.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\"\xbe\x01\n\x08\x45nvValue\x12\x0f\n\x05value\x18\x01 \x01(\tH\x00\x12\x14\n\nraw_secret\x18\x02 \x01(\tH\x00\x12\x30\n\x06secret\x18\x03 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x12\x45\n\x11kubernetes_secret\x18\x04 \x01(\x0b\x32(.prodvana.common_config.KubernetesSecretH\x00\x42\x12\n\x0bvalue_oneof\x12\x03\xf8\x42\x01\"8\n\x06Secret\x12\x14\n\x03key\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07version\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"F\n\x10KubernetesSecret\x12\x1c\n\x0bsecret_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x14\n\x03key\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.common_config.env_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
   _ENVVALUE.oneofs_by_name['value_oneof']._options = None
   _ENVVALUE.oneofs_by_name['value_oneof']._serialized_options = b'\370B\001'
   _SECRET.fields_by_name['key']._options = None
   _SECRET.fields_by_name['key']._serialized_options = b'\372B\004r\002\020\001'
   _SECRET.fields_by_name['version']._options = None
   _SECRET.fields_by_name['version']._serialized_options = b'\372B\004r\002\020\001'
-  _ENVVALUE._serialized_start=85
-  _ENVVALUE._serialized_end=204
-  _SECRET._serialized_start=206
-  _SECRET._serialized_end=262
+  _KUBERNETESSECRET.fields_by_name['secret_name']._options = None
+  _KUBERNETESSECRET.fields_by_name['secret_name']._serialized_options = b'\372B\004r\002\020\001'
+  _KUBERNETESSECRET.fields_by_name['key']._options = None
+  _KUBERNETESSECRET.fields_by_name['key']._serialized_options = b'\372B\004r\002\020\001'
+  _globals['_ENVVALUE']._serialized_start=86
+  _globals['_ENVVALUE']._serialized_end=276
+  _globals['_SECRET']._serialized_start=278
+  _globals['_SECRET']._serialized_end=334
+  _globals['_KUBERNETESSECRET']._serialized_start=336
+  _globals['_KUBERNETESSECRET']._serialized_end=406
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
+import google.protobuf.timestamp_pb2
+import prodvana.proto.prodvana.common_config.meta_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class EnvValue(google.protobuf.message.Message):
+class PipelineRunState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    VALUE_FIELD_NUMBER: builtins.int
-    RAW_SECRET_FIELD_NUMBER: builtins.int
-    SECRET_FIELD_NUMBER: builtins.int
-    value: builtins.str
-    raw_secret: builtins.str
-    """Raw secret value to be used for user-editable YAML and RPC calls."""
+    CREATION_TIMESTAMP_FIELD_NUMBER: builtins.int
+    LAST_UPDATE_TIMESTAMP_FIELD_NUMBER: builtins.int
+    STATE_FIELD_NUMBER: builtins.int
+    TERMINAL_FIELD_NUMBER: builtins.int
     @property
-    def secret(self) -> global___Secret:
-        """Externally stored secret."""
+    def creation_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def last_update_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    state: builtins.str
+    terminal: builtins.bool
+    """if pipeline run is in a terminal state"""
     def __init__(
         self,
         *,
-        value: builtins.str = ...,
-        raw_secret: builtins.str = ...,
-        secret: global___Secret | None = ...,
+        creation_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        last_update_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        state: builtins.str = ...,
+        terminal: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["raw_secret", b"raw_secret", "secret", b"secret", "value", b"value", "value_oneof", b"value_oneof"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["raw_secret", b"raw_secret", "secret", b"secret", "value", b"value", "value_oneof", b"value_oneof"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["value_oneof", b"value_oneof"]) -> typing_extensions.Literal["value", "raw_secret", "secret"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "last_update_timestamp", b"last_update_timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "last_update_timestamp", b"last_update_timestamp", "state", b"state", "terminal", b"terminal"]) -> None: ...
 
-global___EnvValue = EnvValue
+global___PipelineRunState = PipelineRunState
 
-class Secret(google.protobuf.message.Message):
+class PipelineRun(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    KEY_FIELD_NUMBER: builtins.int
-    VERSION_FIELD_NUMBER: builtins.int
-    key: builtins.str
-    version: builtins.str
+    META_FIELD_NUMBER: builtins.int
+    STATE_FIELD_NUMBER: builtins.int
+    @property
+    def meta(self) -> prodvana.proto.prodvana.common_config.meta_pb2.PipelineRunObjectMeta: ...
+    @property
+    def state(self) -> global___PipelineRunState: ...
     def __init__(
         self,
         *,
-        key: builtins.str = ...,
-        version: builtins.str = ...,
+        meta: prodvana.proto.prodvana.common_config.meta_pb2.PipelineRunObjectMeta | None = ...,
+        state: global___PipelineRunState | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "version", b"version"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["meta", b"meta", "state", b"state"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["meta", b"meta", "state", b"state"]) -> None: ...
 
-global___Secret = Secret
+global___PipelineRun = PipelineRun
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
+import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
@@ -16,21 +18,27 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class LocalConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PATH_FIELD_NUMBER: builtins.int
+    PATHS_FIELD_NUMBER: builtins.int
     path: builtins.str
+    """Specify a path to a local file or directory"""
+    @property
+    def paths(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Specify multiple paths. They will get concatenated."""
     def __init__(
         self,
         *,
         path: builtins.str = ...,
+        paths: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["path", b"path"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["path", b"path", "paths", b"paths"]) -> None: ...
 
 global___LocalConfig = LocalConfig
 
 class KubernetesConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Type:
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/common_config/links.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"prodvana/common_config/links.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\";\n\x04Link\x12\x14\n\x03url\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1d\n\x0c\x64isplay_name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
-
-
-_LINK = DESCRIPTOR.message_types_by_name['Link']
-Link = _reflection.GeneratedProtocolMessageType('Link', (_message.Message,), {
-  'DESCRIPTOR' : _LINK,
-  '__module__' : 'prodvana.common_config.links_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.Link)
-  })
-_sym_db.RegisterMessage(Link)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.common_config.links_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
   _LINK.fields_by_name['url']._options = None
   _LINK.fields_by_name['url']._serialized_options = b'\372B\004r\002\020\001'
   _LINK.fields_by_name['display_name']._options = None
   _LINK.fields_by_name['display_name']._serialized_options = b'\372B\004r\002\020\001'
-  _LINK._serialized_start=87
-  _LINK._serialized_end=146
+  _globals['_LINK']._serialized_start=87
+  _globals['_LINK']._serialized_end=146
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/common_config/maturity.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/common_config/maturity.proto\x12\x16prodvana.common_config*7\n\x08Maturity\x12\x12\n\x0e\x46\x41ST_ITERATION\x10\x00\x12\r\n\tPRELAUNCH\x10\x01\x12\x08\n\x04LIVE\x10\x02\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
-_MATURITY = DESCRIPTOR.enum_types_by_name['Maturity']
-Maturity = enum_type_wrapper.EnumTypeWrapper(_MATURITY)
-FAST_ITERATION = 0
-PRELAUNCH = 1
-LIVE = 2
-
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.common_config.maturity_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
-  _MATURITY._serialized_start=65
-  _MATURITY._serialized_end=120
+  _globals['_MATURITY']._serialized_start=65
+  _globals['_MATURITY']._serialized_end=120
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/common_config/notification.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/common_config/notification.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\"x\n\x12NotificationConfig\x12?\n\x05slack\x18\x01 \x01(\x0b\x32\x30.prodvana.common_config.NotificationConfig.Slack\x1a!\n\x05Slack\x12\x18\n\x07\x63hannel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
-
-
-_NOTIFICATIONCONFIG = DESCRIPTOR.message_types_by_name['NotificationConfig']
-_NOTIFICATIONCONFIG_SLACK = _NOTIFICATIONCONFIG.nested_types_by_name['Slack']
-NotificationConfig = _reflection.GeneratedProtocolMessageType('NotificationConfig', (_message.Message,), {
-
-  'Slack' : _reflection.GeneratedProtocolMessageType('Slack', (_message.Message,), {
-    'DESCRIPTOR' : _NOTIFICATIONCONFIG_SLACK,
-    '__module__' : 'prodvana.common_config.notification_pb2'
-    # @@protoc_insertion_point(class_scope:prodvana.common_config.NotificationConfig.Slack)
-    })
-  ,
-  'DESCRIPTOR' : _NOTIFICATIONCONFIG,
-  '__module__' : 'prodvana.common_config.notification_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.NotificationConfig)
-  })
-_sym_db.RegisterMessage(NotificationConfig)
-_sym_db.RegisterMessage(NotificationConfig.Slack)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.common_config.notification_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
   _NOTIFICATIONCONFIG_SLACK.fields_by_name['channel']._options = None
   _NOTIFICATIONCONFIG_SLACK.fields_by_name['channel']._serialized_options = b'\372B\004r\002\020\001'
-  _NOTIFICATIONCONFIG._serialized_start=94
-  _NOTIFICATIONCONFIG._serialized_end=214
-  _NOTIFICATIONCONFIG_SLACK._serialized_start=181
-  _NOTIFICATIONCONFIG_SLACK._serialized_end=214
+  _globals['_NOTIFICATIONCONFIG']._serialized_start=94
+  _globals['_NOTIFICATIONCONFIG']._serialized_end=214
+  _globals['_NOTIFICATIONCONFIG_SLACK']._serialized_start=181
+  _globals['_NOTIFICATIONCONFIG_SLACK']._serialized_end=214
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -262,14 +262,15 @@
     CMD_FIELD_NUMBER: builtins.int
     ENTRYPOINT_FIELD_NUMBER: builtins.int
     ENV_FIELD_NUMBER: builtins.int
     RESOURCES_FIELD_NUMBER: builtins.int
     HEALTH_CHECK_FIELD_NUMBER: builtins.int
     PORTS_FIELD_NUMBER: builtins.int
     TEMPLATE_COMPLETE_FIELD_NUMBER: builtins.int
+    WORKING_DIRECTORY_FIELD_NUMBER: builtins.int
     name: builtins.str
     image: builtins.str
     image_tag: builtins.str
     @property
     def image_registry_info(self) -> global___ImageRegistryInfo:
         """optional, not guaranteed to be compatible with `image` (e.g. if user decides to paste in a public image string)"""
     @property
@@ -287,31 +288,34 @@
         """empty list is ok, default from docker image will be used"""
     template_complete: builtins.bool
     """Only set when this ServiceConfig represents a ServiceTemplate
     When set, this program will be added in whole to the target service's
     programs in full, and will not partially apply to a program with the
     same name in the target service's config.
     """
+    working_directory: builtins.str
+    """working directory, defaults to runtime's implementation (usually the default working directory in the docker image)"""
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         image: builtins.str = ...,
         image_tag: builtins.str = ...,
         image_registry_info: global___ImageRegistryInfo | None = ...,
         cmd: collections.abc.Iterable[builtins.str] | None = ...,
         entrypoint: collections.abc.Iterable[builtins.str] | None = ...,
         env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
         resources: global___ResourceRequirements | None = ...,
         health_check: global___HealthCheck | None = ...,
         ports: collections.abc.Iterable[global___PortConfig] | None = ...,
         template_complete: builtins.bool = ...,
+        working_directory: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["health_check", b"health_check", "image_registry_info", b"image_registry_info", "resources", b"resources"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cmd", b"cmd", "entrypoint", b"entrypoint", "env", b"env", "health_check", b"health_check", "image", b"image", "image_registry_info", b"image_registry_info", "image_tag", b"image_tag", "name", b"name", "ports", b"ports", "resources", b"resources", "template_complete", b"template_complete"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cmd", b"cmd", "entrypoint", b"entrypoint", "env", b"env", "health_check", b"health_check", "image", b"image", "image_registry_info", b"image_registry_info", "image_tag", b"image_tag", "name", b"name", "ports", b"ports", "resources", b"resources", "template_complete", b"template_complete", "working_directory", b"working_directory"]) -> None: ...
 
 global___ProgramConfig = ProgramConfig
 
 class PerReleaseChannelProgramConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class EnvEntry(google.protobuf.message.Message):
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/ref_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/common_config/ref.proto
+# source: prodvana/common_config/constants.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n prodvana/common_config/ref.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\"+\n\x12ServiceTemplateRef\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
-
-
-
-_SERVICETEMPLATEREF = DESCRIPTOR.message_types_by_name['ServiceTemplateRef']
-ServiceTemplateRef = _reflection.GeneratedProtocolMessageType('ServiceTemplateRef', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICETEMPLATEREF,
-  '__module__' : 'prodvana.common_config.ref_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.ServiceTemplateRef)
-  })
-_sym_db.RegisterMessage(ServiceTemplateRef)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&prodvana/common_config/constants.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\"p\n\x08\x43onstant\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x38\n\x06string\x18\x03 \x01(\x0b\x32&.prodvana.common_config.StringConstantH\x00\x42\x13\n\x0c\x63onfig_oneof\x12\x03\xf8\x42\x01\"\x1f\n\x0eStringConstant\x12\r\n\x05value\x18\x01 \x01(\tBRZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.common_config.constants_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
-  _SERVICETEMPLATEREF.fields_by_name['name']._options = None
-  _SERVICETEMPLATEREF.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
-  _SERVICETEMPLATEREF._serialized_start=85
-  _SERVICETEMPLATEREF._serialized_end=128
+  _CONSTANT.oneofs_by_name['config_oneof']._options = None
+  _CONSTANT.oneofs_by_name['config_oneof']._serialized_options = b'\370B\001'
+  _CONSTANT.fields_by_name['name']._options = None
+  _CONSTANT.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
+  _globals['_CONSTANT']._serialized_start=91
+  _globals['_CONSTANT']._serialized_end=203
+  _globals['_STRINGCONSTANT']._serialized_start=205
+  _globals['_STRINGCONSTANT']._serialized_end=236
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/common_config/retry.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from prodvana.proto.prodvana.common_config import notification_pb2 as prodvana_dot_common__config_dot_notification__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"prodvana/common_config/retry.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\x1a\x1egoogle/protobuf/duration.proto\x1a)prodvana/common_config/notification.proto\"m\n\x0cNotification\x12\x43\n\x0f\x63onfig_override\x18\x01 \x01(\x0b\x32*.prodvana.common_config.NotificationConfig\x12\x18\n\x07message\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\xc1\x01\n\x0bRetryConfig\x12\x41\n\x12max_retry_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xfa\x42\x05\xaa\x01\x02*\x00H\x00\x12\x17\n\rretry_forever\x18\x02 \x01(\x08H\x00\x12H\n\x1a\x66irst_failure_notification\x18\x03 \x01(\x0b\x32$.prodvana.common_config.NotificationB\x0c\n\x05limit\x12\x03\xf8\x42\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
-
-
-_NOTIFICATION = DESCRIPTOR.message_types_by_name['Notification']
-_RETRYCONFIG = DESCRIPTOR.message_types_by_name['RetryConfig']
-Notification = _reflection.GeneratedProtocolMessageType('Notification', (_message.Message,), {
-  'DESCRIPTOR' : _NOTIFICATION,
-  '__module__' : 'prodvana.common_config.retry_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.Notification)
-  })
-_sym_db.RegisterMessage(Notification)
-
-RetryConfig = _reflection.GeneratedProtocolMessageType('RetryConfig', (_message.Message,), {
-  'DESCRIPTOR' : _RETRYCONFIG,
-  '__module__' : 'prodvana.common_config.retry_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.RetryConfig)
-  })
-_sym_db.RegisterMessage(RetryConfig)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.common_config.retry_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
   _NOTIFICATION.fields_by_name['message']._options = None
   _NOTIFICATION.fields_by_name['message']._serialized_options = b'\372B\004r\002\020\001'
   _RETRYCONFIG.oneofs_by_name['limit']._options = None
   _RETRYCONFIG.oneofs_by_name['limit']._serialized_options = b'\370B\001'
   _RETRYCONFIG.fields_by_name['max_retry_duration']._options = None
   _RETRYCONFIG.fields_by_name['max_retry_duration']._serialized_options = b'\372B\005\252\001\002*\000'
-  _NOTIFICATION._serialized_start=162
-  _NOTIFICATION._serialized_end=271
-  _RETRYCONFIG._serialized_start=274
-  _RETRYCONFIG._serialized_end=467
+  _globals['_NOTIFICATION']._serialized_start=162
+  _globals['_NOTIFICATION']._serialized_end=271
+  _globals['_RETRYCONFIG']._serialized_start=274
+  _globals['_RETRYCONFIG']._serialized_end=467
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/common_config/task.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
+from prodvana.proto.prodvana.volumes import volumes_pb2 as prodvana_dot_volumes_dot_volumes__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/common_config/task.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\x1a\"prodvana/common_config/retry.proto\x1a$prodvana/common_config/program.proto\"\x89\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x39\n\x0cretry_config\x18\x02 \x01(\x0b\x32#.prodvana.common_config.RetryConfig*\x9a\x01\n\rTaskLifecycle\x12\x1a\n\x16UNKNOWN_TASK_LIFECYCLE\x10\x00\x12\x15\n\x11\x43ONVERGENCE_START\x10\x01\x12\x10\n\x0cPRE_APPROVAL\x10\x02\x12\x0c\n\x08\x41PPROVAL\x10\x03\x12\x11\n\rPOST_APPROVAL\x10\x04\x12\x0e\n\nDEPLOYMENT\x10\x05\x12\x13\n\x0fPOST_DEPLOYMENT\x10\x06\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
-
-_TASKLIFECYCLE = DESCRIPTOR.enum_types_by_name['TaskLifecycle']
-TaskLifecycle = enum_type_wrapper.EnumTypeWrapper(_TASKLIFECYCLE)
-UNKNOWN_TASK_LIFECYCLE = 0
-CONVERGENCE_START = 1
-PRE_APPROVAL = 2
-APPROVAL = 3
-POST_APPROVAL = 4
-DEPLOYMENT = 5
-POST_DEPLOYMENT = 6
-
-
-_TASKCONFIG = DESCRIPTOR.message_types_by_name['TaskConfig']
-TaskConfig = _reflection.GeneratedProtocolMessageType('TaskConfig', (_message.Message,), {
-  'DESCRIPTOR' : _TASKCONFIG,
-  '__module__' : 'prodvana.common_config.task_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.TaskConfig)
-  })
-_sym_db.RegisterMessage(TaskConfig)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/common_config/task.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\x1a\"prodvana/common_config/retry.proto\x1a$prodvana/common_config/program.proto\x1a\x1eprodvana/volumes/volumes.proto\"\xc3\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x07volumes\x18\x03 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x39\n\x0cretry_config\x18\x02 \x01(\x0b\x32#.prodvana.common_config.RetryConfig*\x9a\x01\n\rTaskLifecycle\x12\x1a\n\x16UNKNOWN_TASK_LIFECYCLE\x10\x00\x12\x15\n\x11\x43ONVERGENCE_START\x10\x01\x12\x10\n\x0cPRE_APPROVAL\x10\x02\x12\x0c\n\x08\x41PPROVAL\x10\x03\x12\x11\n\rPOST_APPROVAL\x10\x04\x12\x0e\n\nDEPLOYMENT\x10\x05\x12\x13\n\x0fPOST_DEPLOYMENT\x10\x06\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.common_config.task_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
   _TASKCONFIG.fields_by_name['program']._options = None
   _TASKCONFIG.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _TASKLIFECYCLE._serialized_start=301
-  _TASKLIFECYCLE._serialized_end=455
-  _TASKCONFIG._serialized_start=161
-  _TASKCONFIG._serialized_end=298
+  _TASKCONFIG.fields_by_name['volumes']._options = None
+  _TASKCONFIG.fields_by_name['volumes']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
+  _globals['_TASKLIFECYCLE']._serialized_start=391
+  _globals['_TASKLIFECYCLE']._serialized_end=545
+  _globals['_TASKCONFIG']._serialized_start=193
+  _globals['_TASKCONFIG']._serialized_end=388
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
+import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import prodvana.proto.prodvana.common_config.program_pb2
 import prodvana.proto.prodvana.common_config.retry_pb2
+import prodvana.proto.prodvana.volumes.volumes_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
@@ -53,23 +56,27 @@
 """Runs after service push succeeds (pods are replaced and healthy, ...), before declaring the service CONVERGED."""
 global___TaskLifecycle = TaskLifecycle
 
 class TaskConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROGRAM_FIELD_NUMBER: builtins.int
+    VOLUMES_FIELD_NUMBER: builtins.int
     RETRY_CONFIG_FIELD_NUMBER: builtins.int
     @property
     def program(self) -> prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig: ...
     @property
+    def volumes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.volumes.volumes_pb2.Volume]: ...
+    @property
     def retry_config(self) -> prodvana.proto.prodvana.common_config.retry_pb2.RetryConfig:
         """If not set, the task will not be retried once it starts executing once."""
     def __init__(
         self,
         *,
         program: prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig | None = ...,
+        volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         retry_config: prodvana.proto.prodvana.common_config.retry_pb2.RetryConfig | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["program", b"program", "retry_config", b"retry_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["program", b"program", "retry_config", b"retry_config"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["program", b"program", "retry_config", b"retry_config", "volumes", b"volumes"]) -> None: ...
 
 global___TaskConfig = TaskConfig
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/config_file/config.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.application import application_config_pb2 as prodvana_dot_application_dot_application__config__pb2
 from prodvana.proto.prodvana.application import user_metadata_pb2 as prodvana_dot_application_dot_user__metadata__pb2
 from prodvana.proto.prodvana.environment import clusters_pb2 as prodvana_dot_environment_dot_clusters__pb2
 from prodvana.proto.prodvana.delivery_extension import config_pb2 as prodvana_dot_delivery__extension_dot_config__pb2
 from prodvana.proto.prodvana.protection import protection_config_pb2 as prodvana_dot_protection_dot_protection__config__pb2
+from prodvana.proto.prodvana.release_channel import release_channel_config_pb2 as prodvana_dot_release__channel_dot_release__channel__config__pb2
 from prodvana.proto.prodvana.service import service_config_pb2 as prodvana_dot_service_dot_service__config__pb2
 from prodvana.proto.prodvana.service import user_metadata_pb2 as prodvana_dot_service_dot_user__metadata__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/config_file/config.proto\x12\x14prodvana.config_file\x1a-prodvana/application/application_config.proto\x1a(prodvana/application/user_metadata.proto\x1a#prodvana/environment/clusters.proto\x1a(prodvana/delivery_extension/config.proto\x1a+prodvana/protection/protection_config.proto\x1a%prodvana/service/service_config.proto\x1a$prodvana/service/user_metadata.proto\x1a\x17validate/validate.proto\"\x86\x04\n\x0eProdvanaConfig\x12>\n\x0b\x61pplication\x18\x01 \x01(\x0b\x32\'.prodvana.application.ApplicationConfigH\x00\x12\x32\n\x07service\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfigH\x00\x12;\n\nprotection\x18\x03 \x01(\x0b\x32%.prodvana.protection.ProtectionConfigH\x00\x12\x36\n\x07runtime\x18\x04 \x01(\x0b\x32#.prodvana.environment.ClusterConfigH\x00\x12R\n\x12\x64\x65livery_extension\x18\x07 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12M\n\x14\x61pplication_metadata\x18\x05 \x01(\x0b\x32-.prodvana.application.ApplicationUserMetadataH\x01\x12\x41\n\x10service_metadata\x18\x06 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadataH\x01\x42\x13\n\x0c\x63onfig_oneof\x12\x03\xf8\x42\x01\x42\x10\n\x0emetadata_oneofBPZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_fileb\x06proto3')
-
-
-
-_PRODVANACONFIG = DESCRIPTOR.message_types_by_name['ProdvanaConfig']
-ProdvanaConfig = _reflection.GeneratedProtocolMessageType('ProdvanaConfig', (_message.Message,), {
-  'DESCRIPTOR' : _PRODVANACONFIG,
-  '__module__' : 'prodvana.config_file.config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.config_file.ProdvanaConfig)
-  })
-_sym_db.RegisterMessage(ProdvanaConfig)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/config_file/config.proto\x12\x14prodvana.config_file\x1a-prodvana/application/application_config.proto\x1a(prodvana/application/user_metadata.proto\x1a#prodvana/environment/clusters.proto\x1a(prodvana/delivery_extension/config.proto\x1a+prodvana/protection/protection_config.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a%prodvana/service/service_config.proto\x1a$prodvana/service/user_metadata.proto\x1a\x17validate/validate.proto\"\xd1\x04\n\x0eProdvanaConfig\x12>\n\x0b\x61pplication\x18\x01 \x01(\x0b\x32\'.prodvana.application.ApplicationConfigH\x00\x12\x32\n\x07service\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfigH\x00\x12;\n\nprotection\x18\x03 \x01(\x0b\x32%.prodvana.protection.ProtectionConfigH\x00\x12\x36\n\x07runtime\x18\x04 \x01(\x0b\x32#.prodvana.environment.ClusterConfigH\x00\x12R\n\x12\x64\x65livery_extension\x18\x07 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12I\n\x0frelease_channel\x18\x08 \x01(\x0b\x32..prodvana.release_channel.ReleaseChannelConfigH\x00\x12M\n\x14\x61pplication_metadata\x18\x05 \x01(\x0b\x32-.prodvana.application.ApplicationUserMetadataH\x01\x12\x41\n\x10service_metadata\x18\x06 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadataH\x01\x42\x13\n\x0c\x63onfig_oneof\x12\x03\xf8\x42\x01\x42\x10\n\x0emetadata_oneofBPZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_fileb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.config_file.config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_file'
   _PRODVANACONFIG.oneofs_by_name['config_oneof']._options = None
   _PRODVANACONFIG.oneofs_by_name['config_oneof']._serialized_options = b'\370B\001'
-  _PRODVANACONFIG._serialized_start=375
-  _PRODVANACONFIG._serialized_end=893
+  _globals['_PRODVANACONFIG']._serialized_start=430
+  _globals['_PRODVANACONFIG']._serialized_end=1023
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import google.protobuf.descriptor
 import google.protobuf.message
 import prodvana.proto.prodvana.application.application_config_pb2
 import prodvana.proto.prodvana.application.user_metadata_pb2
 import prodvana.proto.prodvana.delivery_extension.config_pb2
 import prodvana.proto.prodvana.environment.clusters_pb2
 import prodvana.proto.prodvana.protection.protection_config_pb2
+import prodvana.proto.prodvana.release_channel.release_channel_config_pb2
 import prodvana.proto.prodvana.service.service_config_pb2
 import prodvana.proto.prodvana.service.user_metadata_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
@@ -28,42 +29,46 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLICATION_FIELD_NUMBER: builtins.int
     SERVICE_FIELD_NUMBER: builtins.int
     PROTECTION_FIELD_NUMBER: builtins.int
     RUNTIME_FIELD_NUMBER: builtins.int
     DELIVERY_EXTENSION_FIELD_NUMBER: builtins.int
+    RELEASE_CHANNEL_FIELD_NUMBER: builtins.int
     APPLICATION_METADATA_FIELD_NUMBER: builtins.int
     SERVICE_METADATA_FIELD_NUMBER: builtins.int
     @property
     def application(self) -> prodvana.proto.prodvana.application.application_config_pb2.ApplicationConfig: ...
     @property
     def service(self) -> prodvana.proto.prodvana.service.service_config_pb2.ServiceConfig: ...
     @property
     def protection(self) -> prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig: ...
     @property
     def runtime(self) -> prodvana.proto.prodvana.environment.clusters_pb2.ClusterConfig: ...
     @property
     def delivery_extension(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig: ...
     @property
+    def release_channel(self) -> prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig: ...
+    @property
     def application_metadata(self) -> prodvana.proto.prodvana.application.user_metadata_pb2.ApplicationUserMetadata: ...
     @property
     def service_metadata(self) -> prodvana.proto.prodvana.service.user_metadata_pb2.ServiceUserMetadata: ...
     def __init__(
         self,
         *,
         application: prodvana.proto.prodvana.application.application_config_pb2.ApplicationConfig | None = ...,
         service: prodvana.proto.prodvana.service.service_config_pb2.ServiceConfig | None = ...,
         protection: prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig | None = ...,
         runtime: prodvana.proto.prodvana.environment.clusters_pb2.ClusterConfig | None = ...,
         delivery_extension: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
+        release_channel: prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig | None = ...,
         application_metadata: prodvana.proto.prodvana.application.user_metadata_pb2.ApplicationUserMetadata | None = ...,
         service_metadata: prodvana.proto.prodvana.service.user_metadata_pb2.ServiceUserMetadata | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["application", b"application", "application_metadata", b"application_metadata", "config_oneof", b"config_oneof", "delivery_extension", b"delivery_extension", "metadata_oneof", b"metadata_oneof", "protection", b"protection", "runtime", b"runtime", "service", b"service", "service_metadata", b"service_metadata"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "application_metadata", b"application_metadata", "config_oneof", b"config_oneof", "delivery_extension", b"delivery_extension", "metadata_oneof", b"metadata_oneof", "protection", b"protection", "runtime", b"runtime", "service", b"service", "service_metadata", b"service_metadata"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["application", b"application", "application_metadata", b"application_metadata", "config_oneof", b"config_oneof", "delivery_extension", b"delivery_extension", "metadata_oneof", b"metadata_oneof", "protection", b"protection", "release_channel", b"release_channel", "runtime", b"runtime", "service", b"service", "service_metadata", b"service_metadata"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "application_metadata", b"application_metadata", "config_oneof", b"config_oneof", "delivery_extension", b"delivery_extension", "metadata_oneof", b"metadata_oneof", "protection", b"protection", "release_channel", b"release_channel", "runtime", b"runtime", "service", b"service", "service_metadata", b"service_metadata"]) -> None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["application", "service", "protection", "runtime", "delivery_extension"] | None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["application", "service", "protection", "runtime", "delivery_extension", "release_channel"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["metadata_oneof", b"metadata_oneof"]) -> typing_extensions.Literal["application_metadata", "service_metadata"] | None: ...
 
 global___ProdvanaConfig = ProdvanaConfig
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/config_writeback/writeback.proto
+# source: prodvana/delivery/delivery_config.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
+from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/config_writeback/writeback.proto\x12\x19prodvana.config_writeback\"A\n\x13\x43onfigWritebackPath\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_path\x18\x02 \x01(\tBUZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writebackb\x06proto3')
-
-
-
-_CONFIGWRITEBACKPATH = DESCRIPTOR.message_types_by_name['ConfigWritebackPath']
-ConfigWritebackPath = _reflection.GeneratedProtocolMessageType('ConfigWritebackPath', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGWRITEBACKPATH,
-  '__module__' : 'prodvana.config_writeback.writeback_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.config_writeback.ConfigWritebackPath)
-  })
-_sym_db.RegisterMessage(ConfigWritebackPath)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'prodvana/delivery/delivery_config.proto\x12\x11prodvana.delivery\x1a\x1egoogle/protobuf/duration.proto\x1a\x17validate/validate.proto\"_\n\x0e\x43\x61naryProgress\x12 \n\rcanary_weight\x18\x01 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\"h\n\x0e\x44\x65liveryConfig\x12:\n\x0f\x63\x61nary_progress\x18\x01 \x03(\x0b\x32!.prodvana.delivery.CanaryProgress\x12\x1a\n\x12\x61nalysis_templates\x18\x02 \x03(\tBMZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/deliveryb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.delivery.delivery_config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writeback'
-  _CONFIGWRITEBACKPATH._serialized_start=72
-  _CONFIGWRITEBACKPATH._serialized_end=137
+  DESCRIPTOR._serialized_options = b'ZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery'
+  _CANARYPROGRESS.fields_by_name['canary_weight']._options = None
+  _CANARYPROGRESS.fields_by_name['canary_weight']._serialized_options = b'\372B\006\032\004\030d(\000'
+  _globals['_CANARYPROGRESS']._serialized_start=119
+  _globals['_CANARYPROGRESS']._serialized_end=214
+  _globals['_DELIVERYCONFIG']._serialized_start=216
+  _globals['_DELIVERYCONFIG']._serialized_end=320
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/delivery/delivery_config.proto
+# source: prodvana/service/user_metadata.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
+from prodvana.proto.prodvana.common_config import links_pb2 as prodvana_dot_common__config_dot_links__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'prodvana/delivery/delivery_config.proto\x12\x11prodvana.delivery\x1a\x1egoogle/protobuf/duration.proto\x1a\x17validate/validate.proto\"_\n\x0e\x43\x61naryProgress\x12 \n\rcanary_weight\x18\x01 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\"h\n\x0e\x44\x65liveryConfig\x12:\n\x0f\x63\x61nary_progress\x18\x01 \x03(\x0b\x32!.prodvana.delivery.CanaryProgress\x12\x1a\n\x12\x61nalysis_templates\x18\x02 \x03(\tBMZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/deliveryb\x06proto3')
-
-
-
-_CANARYPROGRESS = DESCRIPTOR.message_types_by_name['CanaryProgress']
-_DELIVERYCONFIG = DESCRIPTOR.message_types_by_name['DeliveryConfig']
-CanaryProgress = _reflection.GeneratedProtocolMessageType('CanaryProgress', (_message.Message,), {
-  'DESCRIPTOR' : _CANARYPROGRESS,
-  '__module__' : 'prodvana.delivery.delivery_config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery.CanaryProgress)
-  })
-_sym_db.RegisterMessage(CanaryProgress)
-
-DeliveryConfig = _reflection.GeneratedProtocolMessageType('DeliveryConfig', (_message.Message,), {
-  'DESCRIPTOR' : _DELIVERYCONFIG,
-  '__module__' : 'prodvana.delivery.delivery_config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery.DeliveryConfig)
-  })
-_sym_db.RegisterMessage(DeliveryConfig)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$prodvana/service/user_metadata.proto\x12\x10prodvana.service\x1a\"prodvana/common_config/links.proto\x1a\x17validate/validate.proto\"\xb6\x01\n\x13ServiceUserMetadata\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12:\n\x05links\x18\x02 \x03(\x0b\x32\x1c.prodvana.common_config.LinkB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12N\n\x11\x66ollow_repository\x18\x03 \x01(\x0b\x32\x33.prodvana.service.FollowContainerRepositorySettings\"4\n!FollowContainerRepositorySettings\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x42LZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.service.user_metadata_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery'
-  _CANARYPROGRESS.fields_by_name['canary_weight']._options = None
-  _CANARYPROGRESS.fields_by_name['canary_weight']._serialized_options = b'\372B\006\032\004\030d(\000'
-  _CANARYPROGRESS._serialized_start=119
-  _CANARYPROGRESS._serialized_end=214
-  _DELIVERYCONFIG._serialized_start=216
-  _DELIVERYCONFIG._serialized_end=320
+  DESCRIPTOR._serialized_options = b'ZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/service'
+  _SERVICEUSERMETADATA.fields_by_name['links']._options = None
+  _SERVICEUSERMETADATA.fields_by_name['links']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
+  _globals['_SERVICEUSERMETADATA']._serialized_start=120
+  _globals['_SERVICEUSERMETADATA']._serialized_end=302
+  _globals['_FOLLOWCONTAINERREPOSITORYSETTINGS']._serialized_start=304
+  _globals['_FOLLOWCONTAINERREPOSITORYSETTINGS']._serialized_end=356
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/config_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,59 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/delivery_extension/config.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.common_config import env_pb2 as prodvana_dot_common__config_dot_env__pb2
 from prodvana.proto.prodvana.common_config import kubernetes_config_pb2 as prodvana_dot_common__config_dot_kubernetes__config__pb2
 from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(prodvana/delivery_extension/config.proto\x12\x1bprodvana.delivery_extension\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a\'prodvana/common_config/parameters.proto\x1a\'prodvana/runtimes/runtimes_config.proto\"\xbb\x02\n\x17\x44\x65liveryExtensionConfig\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12\x39\n\x0btask_config\x18\x02 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x03 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12N\n\nparameters\x18\x04 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\x98\x01\n\x1f\x44\x65liveryExtensionInstanceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\nparameters\x18\x03 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"\xcf\x03\n\'CompiledDeliveryExtensionInstanceConfig\x12H\n\ndefinition\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x44\n\x11runtime_execution\x18\x02 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12\x83\x01\n\x03\x65nv\x18\x03 \x03(\x0b\x32M.prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12@\n\x10parameter_values\x18\x04 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01*@\n\x04Type\x12\x10\n\x0cUNKNOWN_TYPE\x10\x00\x12\x17\n\x13GLOBAL_USER_CREATED\x10\x01\x12\r\n\tEPHEMERAL\x10\x02\x42WZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
-
-_TYPE = DESCRIPTOR.enum_types_by_name['Type']
-Type = enum_type_wrapper.EnumTypeWrapper(_TYPE)
-UNKNOWN_TYPE = 0
-GLOBAL_USER_CREATED = 1
-EPHEMERAL = 2
-
-
-_DELIVERYEXTENSIONCONFIG = DESCRIPTOR.message_types_by_name['DeliveryExtensionConfig']
-_DELIVERYEXTENSIONINSTANCECONFIG = DESCRIPTOR.message_types_by_name['DeliveryExtensionInstanceConfig']
-_COMPILEDDELIVERYEXTENSIONINSTANCECONFIG = DESCRIPTOR.message_types_by_name['CompiledDeliveryExtensionInstanceConfig']
-_COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY = _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG.nested_types_by_name['EnvEntry']
-DeliveryExtensionConfig = _reflection.GeneratedProtocolMessageType('DeliveryExtensionConfig', (_message.Message,), {
-  'DESCRIPTOR' : _DELIVERYEXTENSIONCONFIG,
-  '__module__' : 'prodvana.delivery_extension.config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.DeliveryExtensionConfig)
-  })
-_sym_db.RegisterMessage(DeliveryExtensionConfig)
-
-DeliveryExtensionInstanceConfig = _reflection.GeneratedProtocolMessageType('DeliveryExtensionInstanceConfig', (_message.Message,), {
-  'DESCRIPTOR' : _DELIVERYEXTENSIONINSTANCECONFIG,
-  '__module__' : 'prodvana.delivery_extension.config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.DeliveryExtensionInstanceConfig)
-  })
-_sym_db.RegisterMessage(DeliveryExtensionInstanceConfig)
-
-CompiledDeliveryExtensionInstanceConfig = _reflection.GeneratedProtocolMessageType('CompiledDeliveryExtensionInstanceConfig', (_message.Message,), {
-
-  'EnvEntry' : _reflection.GeneratedProtocolMessageType('EnvEntry', (_message.Message,), {
-    'DESCRIPTOR' : _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY,
-    '__module__' : 'prodvana.delivery_extension.config_pb2'
-    # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig.EnvEntry)
-    })
-  ,
-  'DESCRIPTOR' : _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG,
-  '__module__' : 'prodvana.delivery_extension.config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig)
-  })
-_sym_db.RegisterMessage(CompiledDeliveryExtensionInstanceConfig)
-_sym_db.RegisterMessage(CompiledDeliveryExtensionInstanceConfig.EnvEntry)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(prodvana/delivery_extension/config.proto\x12\x1bprodvana.delivery_extension\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a\'prodvana/common_config/parameters.proto\x1a\'prodvana/runtimes/runtimes_config.proto\"\xfe\x03\n\x17\x44\x65liveryExtensionConfig\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12\x39\n\x0btask_config\x18\x02 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x03 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12N\n\nparameters\x18\x04 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12s\n\x03\x65nv\x18\x05 \x03(\x0b\x32=.prodvana.delivery_extension.DeliveryExtensionConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\x95\x01\n\x1c\x44\x65liveryExtensionInstanceRef\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\nparameters\x18\x03 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"\xcf\x03\n\'CompiledDeliveryExtensionInstanceConfig\x12H\n\ndefinition\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x44\n\x11runtime_execution\x18\x02 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12\x83\x01\n\x03\x65nv\x18\x03 \x03(\x0b\x32M.prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12@\n\x10parameter_values\x18\x04 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01*@\n\x04Type\x12\x10\n\x0cUNKNOWN_TYPE\x10\x00\x12\x17\n\x13GLOBAL_USER_CREATED\x10\x01\x12\r\n\tEPHEMERAL\x10\x02\x42WZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.delivery_extension.config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extension'
+  _DELIVERYEXTENSIONCONFIG_ENVENTRY._options = None
+  _DELIVERYEXTENSIONCONFIG_ENVENTRY._serialized_options = b'8\001'
   _DELIVERYEXTENSIONCONFIG.oneofs_by_name['exec_config']._options = None
   _DELIVERYEXTENSIONCONFIG.oneofs_by_name['exec_config']._serialized_options = b'\370B\001'
   _DELIVERYEXTENSIONCONFIG.fields_by_name['name']._options = None
   _DELIVERYEXTENSIONCONFIG.fields_by_name['name']._serialized_options = b'\372B)r\'\020\000\030?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$'
   _DELIVERYEXTENSIONCONFIG.fields_by_name['parameters']._options = None
   _DELIVERYEXTENSIONCONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
-  _DELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['name']._options = None
-  _DELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['env']._options = None
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['env']._serialized_options = b'\372B$\232\001!\030\001\"\035r\0332\031^[a-zA-Z_]+[a-zA-Z0-9_]*$'
+  _DELIVERYEXTENSIONINSTANCEREF.fields_by_name['name']._options = None
+  _DELIVERYEXTENSIONINSTANCEREF.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
   _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._options = None
   _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_options = b'8\001'
   _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['env']._options = None
   _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['env']._serialized_options = b'\372B$\232\001!\030\001\"\035r\0332\031^[a-zA-Z_]+[a-zA-Z0-9_]*$'
-  _TYPE._serialized_start=1236
-  _TYPE._serialized_end=1300
-  _DELIVERYEXTENSIONCONFIG._serialized_start=298
-  _DELIVERYEXTENSIONCONFIG._serialized_end=613
-  _DELIVERYEXTENSIONINSTANCECONFIG._serialized_start=616
-  _DELIVERYEXTENSIONINSTANCECONFIG._serialized_end=768
-  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG._serialized_start=771
-  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG._serialized_end=1234
-  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_start=1158
-  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_end=1234
+  _globals['_TYPE']._serialized_start=1428
+  _globals['_TYPE']._serialized_end=1492
+  _globals['_DELIVERYEXTENSIONCONFIG']._serialized_start=298
+  _globals['_DELIVERYEXTENSIONCONFIG']._serialized_end=808
+  _globals['_DELIVERYEXTENSIONCONFIG_ENVENTRY']._serialized_start=712
+  _globals['_DELIVERYEXTENSIONCONFIG_ENVENTRY']._serialized_end=788
+  _globals['_DELIVERYEXTENSIONINSTANCEREF']._serialized_start=811
+  _globals['_DELIVERYEXTENSIONINSTANCEREF']._serialized_end=960
+  _globals['_COMPILEDDELIVERYEXTENSIONINSTANCECONFIG']._serialized_start=963
+  _globals['_COMPILEDDELIVERYEXTENSIONINSTANCECONFIG']._serialized_end=1426
+  _globals['_COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY']._serialized_start=712
+  _globals['_COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY']._serialized_end=788
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -41,40 +41,62 @@
 EPHEMERAL: Type.ValueType  # 2
 """one-off delivery extensions inlined into other configs"""
 global___Type = Type
 
 class DeliveryExtensionConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    class EnvEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> prodvana.proto.prodvana.common_config.env_pb2.EnvValue: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: prodvana.proto.prodvana.common_config.env_pb2.EnvValue | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     NAME_FIELD_NUMBER: builtins.int
     TASK_CONFIG_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
+    ENV_FIELD_NUMBER: builtins.int
     name: builtins.str
     @property
     def task_config(self) -> prodvana.proto.prodvana.common_config.task_pb2.TaskConfig: ...
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
+    @property
+    def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
+        """optional env variables to inject and override from exec_config"""
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         task_config: prodvana.proto.prodvana.common_config.task_pb2.TaskConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
+        env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "task_config", b"task_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameters", b"parameters", "task_config", b"task_config"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["env", b"env", "exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameters", b"parameters", "task_config", b"task_config"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["exec_config", b"exec_config"]) -> typing_extensions.Literal["task_config", "kubernetes_config"] | None: ...
 
 global___DeliveryExtensionConfig = DeliveryExtensionConfig
 
-class DeliveryExtensionInstanceConfig(google.protobuf.message.Message):
+class DeliveryExtensionInstanceRef(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     name: builtins.str
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]: ...
@@ -82,15 +104,15 @@
         self,
         *,
         name: builtins.str = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "parameters", b"parameters"]) -> None: ...
 
-global___DeliveryExtensionInstanceConfig = DeliveryExtensionInstanceConfig
+global___DeliveryExtensionInstanceRef = DeliveryExtensionInstanceRef
 
 class CompiledDeliveryExtensionInstanceConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class EnvEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/manager_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,74 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/delivery_extension/manager.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from prodvana.proto.prodvana.delivery_extension import object_pb2 as prodvana_dot_delivery__extension_dot_object__pb2
 from prodvana.proto.prodvana.delivery_extension import config_pb2 as prodvana_dot_delivery__extension_dot_config__pb2
 from prodvana.proto.prodvana.version import source_metadata_pb2 as prodvana_dot_version_dot_source__metadata__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/delivery_extension/manager.proto\x12\x1bprodvana.delivery_extension\x1a\x1cgoogle/api/annotations.proto\x1a(prodvana/delivery_extension/object.proto\x1a(prodvana/delivery_extension/config.proto\x1a&prodvana/version/source_metadata.proto\x1a\x17validate/validate.proto\"\xe7\x01\n\x1d\x43onfigureDeliveryExtensionReq\x12\x61\n\x19\x64\x65livery_extension_config\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12(\n\x06source\x18\x02 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x03 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"P\n\x1e\x43onfigureDeliveryExtensionResp\x12\x1d\n\x15\x64\x65livery_extension_id\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"(\n&ValidateConfigureDeliveryExtensionResp\"B\n\x19ListDeliveryExtensionsReq\x12\x12\n\npage_token\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\"\x82\x01\n\x1aListDeliveryExtensionsResp\x12K\n\x13\x64\x65livery_extensions\x18\x01 \x03(\x0b\x32..prodvana.delivery_extension.DeliveryExtension\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\">\n\x17GetDeliveryExtensionReq\x12#\n\x12\x64\x65livery_extension\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"f\n\x18GetDeliveryExtensionResp\x12J\n\x12\x64\x65livery_extension\x18\x01 \x01(\x0b\x32..prodvana.delivery_extension.DeliveryExtension\"U\n\x1dGetDeliveryExtensionConfigReq\x12#\n\x12\x64\x65livery_extension\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0f\n\x07version\x18\x02 \x01(\t\"w\n\x1eGetDeliveryExtensionConfigResp\x12\x44\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x0f\n\x07version\x18\x02 \x01(\t2\xff\x07\n\x18\x44\x65liveryExtensionManager\x12\xc3\x01\n\x1a\x43onfigureDeliveryExtension\x12:.prodvana.delivery_extension.ConfigureDeliveryExtensionReq\x1a;.prodvana.delivery_extension.ConfigureDeliveryExtensionResp\",\x82\xd3\xe4\x93\x02&\"!/v1/delivery_extensions/configure:\x01*\x12\xdc\x01\n\"ValidateConfigureDeliveryExtension\x12:.prodvana.delivery_extension.ConfigureDeliveryExtensionReq\x1a\x43.prodvana.delivery_extension.ValidateConfigureDeliveryExtensionResp\"5\x82\xd3\xe4\x93\x02/\"*/v1/delivery_extensions/configure/validate:\x01*\x12\xaa\x01\n\x16ListDeliveryExtensions\x12\x36.prodvana.delivery_extension.ListDeliveryExtensionsReq\x1a\x37.prodvana.delivery_extension.ListDeliveryExtensionsResp\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/delivery_extensions\x12\xba\x01\n\x14GetDeliveryExtension\x12\x34.prodvana.delivery_extension.GetDeliveryExtensionReq\x1a\x35.prodvana.delivery_extension.GetDeliveryExtensionResp\"5\x82\xd3\xe4\x93\x02/\x12-/v1/delivery_extension/{delivery_extension=*}\x12\xd3\x01\n\x1aGetDeliveryExtensionConfig\x12:.prodvana.delivery_extension.GetDeliveryExtensionConfigReq\x1a;.prodvana.delivery_extension.GetDeliveryExtensionConfigResp\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/v1/delivery_extension/{delivery_extension=*}/configBWZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/delivery_extension/manager.proto\x12\x1bprodvana.delivery_extension\x1a\x1cgoogle/api/annotations.proto\x1a(prodvana/delivery_extension/object.proto\x1a(prodvana/delivery_extension/config.proto\x1a&prodvana/version/source_metadata.proto\x1a\x17validate/validate.proto\"\xe7\x01\n\x1d\x43onfigureDeliveryExtensionReq\x12\x61\n\x19\x64\x65livery_extension_config\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12(\n\x06source\x18\x02 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x03 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"P\n\x1e\x43onfigureDeliveryExtensionResp\x12\x1d\n\x15\x64\x65livery_extension_id\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"(\n&ValidateConfigureDeliveryExtensionResp\"B\n\x19ListDeliveryExtensionsReq\x12\x12\n\npage_token\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\"\x82\x01\n\x1aListDeliveryExtensionsResp\x12K\n\x13\x64\x65livery_extensions\x18\x01 \x03(\x0b\x32..prodvana.delivery_extension.DeliveryExtension\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\">\n\x17GetDeliveryExtensionReq\x12#\n\x12\x64\x65livery_extension\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"f\n\x18GetDeliveryExtensionResp\x12J\n\x12\x64\x65livery_extension\x18\x01 \x01(\x0b\x32..prodvana.delivery_extension.DeliveryExtension\"U\n\x1dGetDeliveryExtensionConfigReq\x12#\n\x12\x64\x65livery_extension\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0f\n\x07version\x18\x02 \x01(\t\"w\n\x1eGetDeliveryExtensionConfigResp\x12\x44\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x0f\n\x07version\x18\x02 \x01(\t\"i\n%GetDeliveryExtensionInstanceConfigReq\x12/\n\x1e\x64\x65livery_extension_instance_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x8f\x01\n&GetDeliveryExtensionInstanceConfigResp\x12T\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x44.prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig\x12\x0f\n\x07version\x18\x02 \x01(\t2\x82\n\n\x18\x44\x65liveryExtensionManager\x12\xc3\x01\n\x1a\x43onfigureDeliveryExtension\x12:.prodvana.delivery_extension.ConfigureDeliveryExtensionReq\x1a;.prodvana.delivery_extension.ConfigureDeliveryExtensionResp\",\x82\xd3\xe4\x93\x02&\"!/v1/delivery_extensions/configure:\x01*\x12\xdc\x01\n\"ValidateConfigureDeliveryExtension\x12:.prodvana.delivery_extension.ConfigureDeliveryExtensionReq\x1a\x43.prodvana.delivery_extension.ValidateConfigureDeliveryExtensionResp\"5\x82\xd3\xe4\x93\x02/\"*/v1/delivery_extensions/configure/validate:\x01*\x12\xaa\x01\n\x16ListDeliveryExtensions\x12\x36.prodvana.delivery_extension.ListDeliveryExtensionsReq\x1a\x37.prodvana.delivery_extension.ListDeliveryExtensionsResp\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/delivery_extensions\x12\xba\x01\n\x14GetDeliveryExtension\x12\x34.prodvana.delivery_extension.GetDeliveryExtensionReq\x1a\x35.prodvana.delivery_extension.GetDeliveryExtensionResp\"5\x82\xd3\xe4\x93\x02/\x12-/v1/delivery_extension/{delivery_extension=*}\x12\xd3\x01\n\x1aGetDeliveryExtensionConfig\x12:.prodvana.delivery_extension.GetDeliveryExtensionConfigReq\x1a;.prodvana.delivery_extension.GetDeliveryExtensionConfigResp\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/v1/delivery_extension/{delivery_extension=*}/config\x12\x80\x02\n\"GetDeliveryExtensionInstanceConfig\x12\x42.prodvana.delivery_extension.GetDeliveryExtensionInstanceConfigReq\x1a\x43.prodvana.delivery_extension.GetDeliveryExtensionInstanceConfigResp\"Q\x82\xd3\xe4\x93\x02K\x12I/v1/delivery_extension/instance/{delivery_extension_instance_id=*}/configBWZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
 
-
-
-_CONFIGUREDELIVERYEXTENSIONREQ = DESCRIPTOR.message_types_by_name['ConfigureDeliveryExtensionReq']
-_CONFIGUREDELIVERYEXTENSIONRESP = DESCRIPTOR.message_types_by_name['ConfigureDeliveryExtensionResp']
-_VALIDATECONFIGUREDELIVERYEXTENSIONRESP = DESCRIPTOR.message_types_by_name['ValidateConfigureDeliveryExtensionResp']
-_LISTDELIVERYEXTENSIONSREQ = DESCRIPTOR.message_types_by_name['ListDeliveryExtensionsReq']
-_LISTDELIVERYEXTENSIONSRESP = DESCRIPTOR.message_types_by_name['ListDeliveryExtensionsResp']
-_GETDELIVERYEXTENSIONREQ = DESCRIPTOR.message_types_by_name['GetDeliveryExtensionReq']
-_GETDELIVERYEXTENSIONRESP = DESCRIPTOR.message_types_by_name['GetDeliveryExtensionResp']
-_GETDELIVERYEXTENSIONCONFIGREQ = DESCRIPTOR.message_types_by_name['GetDeliveryExtensionConfigReq']
-_GETDELIVERYEXTENSIONCONFIGRESP = DESCRIPTOR.message_types_by_name['GetDeliveryExtensionConfigResp']
-ConfigureDeliveryExtensionReq = _reflection.GeneratedProtocolMessageType('ConfigureDeliveryExtensionReq', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGUREDELIVERYEXTENSIONREQ,
-  '__module__' : 'prodvana.delivery_extension.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ConfigureDeliveryExtensionReq)
-  })
-_sym_db.RegisterMessage(ConfigureDeliveryExtensionReq)
-
-ConfigureDeliveryExtensionResp = _reflection.GeneratedProtocolMessageType('ConfigureDeliveryExtensionResp', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGUREDELIVERYEXTENSIONRESP,
-  '__module__' : 'prodvana.delivery_extension.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ConfigureDeliveryExtensionResp)
-  })
-_sym_db.RegisterMessage(ConfigureDeliveryExtensionResp)
-
-ValidateConfigureDeliveryExtensionResp = _reflection.GeneratedProtocolMessageType('ValidateConfigureDeliveryExtensionResp', (_message.Message,), {
-  'DESCRIPTOR' : _VALIDATECONFIGUREDELIVERYEXTENSIONRESP,
-  '__module__' : 'prodvana.delivery_extension.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ValidateConfigureDeliveryExtensionResp)
-  })
-_sym_db.RegisterMessage(ValidateConfigureDeliveryExtensionResp)
-
-ListDeliveryExtensionsReq = _reflection.GeneratedProtocolMessageType('ListDeliveryExtensionsReq', (_message.Message,), {
-  'DESCRIPTOR' : _LISTDELIVERYEXTENSIONSREQ,
-  '__module__' : 'prodvana.delivery_extension.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ListDeliveryExtensionsReq)
-  })
-_sym_db.RegisterMessage(ListDeliveryExtensionsReq)
-
-ListDeliveryExtensionsResp = _reflection.GeneratedProtocolMessageType('ListDeliveryExtensionsResp', (_message.Message,), {
-  'DESCRIPTOR' : _LISTDELIVERYEXTENSIONSRESP,
-  '__module__' : 'prodvana.delivery_extension.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ListDeliveryExtensionsResp)
-  })
-_sym_db.RegisterMessage(ListDeliveryExtensionsResp)
-
-GetDeliveryExtensionReq = _reflection.GeneratedProtocolMessageType('GetDeliveryExtensionReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETDELIVERYEXTENSIONREQ,
-  '__module__' : 'prodvana.delivery_extension.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.GetDeliveryExtensionReq)
-  })
-_sym_db.RegisterMessage(GetDeliveryExtensionReq)
-
-GetDeliveryExtensionResp = _reflection.GeneratedProtocolMessageType('GetDeliveryExtensionResp', (_message.Message,), {
-  'DESCRIPTOR' : _GETDELIVERYEXTENSIONRESP,
-  '__module__' : 'prodvana.delivery_extension.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.GetDeliveryExtensionResp)
-  })
-_sym_db.RegisterMessage(GetDeliveryExtensionResp)
-
-GetDeliveryExtensionConfigReq = _reflection.GeneratedProtocolMessageType('GetDeliveryExtensionConfigReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETDELIVERYEXTENSIONCONFIGREQ,
-  '__module__' : 'prodvana.delivery_extension.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.GetDeliveryExtensionConfigReq)
-  })
-_sym_db.RegisterMessage(GetDeliveryExtensionConfigReq)
-
-GetDeliveryExtensionConfigResp = _reflection.GeneratedProtocolMessageType('GetDeliveryExtensionConfigResp', (_message.Message,), {
-  'DESCRIPTOR' : _GETDELIVERYEXTENSIONCONFIGRESP,
-  '__module__' : 'prodvana.delivery_extension.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.GetDeliveryExtensionConfigResp)
-  })
-_sym_db.RegisterMessage(GetDeliveryExtensionConfigResp)
-
-_DELIVERYEXTENSIONMANAGER = DESCRIPTOR.services_by_name['DeliveryExtensionManager']
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.delivery_extension.manager_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extension'
   _CONFIGUREDELIVERYEXTENSIONREQ.fields_by_name['delivery_extension_config']._options = None
   _CONFIGUREDELIVERYEXTENSIONREQ.fields_by_name['delivery_extension_config']._serialized_options = b'\372B\005\212\001\002\020\001'
   _GETDELIVERYEXTENSIONREQ.fields_by_name['delivery_extension']._options = None
   _GETDELIVERYEXTENSIONREQ.fields_by_name['delivery_extension']._serialized_options = b'\372B\004r\002\020\001'
   _GETDELIVERYEXTENSIONCONFIGREQ.fields_by_name['delivery_extension']._options = None
   _GETDELIVERYEXTENSIONCONFIGREQ.fields_by_name['delivery_extension']._serialized_options = b'\372B\004r\002\020\001'
+  _GETDELIVERYEXTENSIONINSTANCECONFIGREQ.fields_by_name['delivery_extension_instance_id']._options = None
+  _GETDELIVERYEXTENSIONINSTANCECONFIGREQ.fields_by_name['delivery_extension_instance_id']._serialized_options = b'\372B\004r\002\020\001'
   _DELIVERYEXTENSIONMANAGER.methods_by_name['ConfigureDeliveryExtension']._options = None
   _DELIVERYEXTENSIONMANAGER.methods_by_name['ConfigureDeliveryExtension']._serialized_options = b'\202\323\344\223\002&\"!/v1/delivery_extensions/configure:\001*'
   _DELIVERYEXTENSIONMANAGER.methods_by_name['ValidateConfigureDeliveryExtension']._options = None
   _DELIVERYEXTENSIONMANAGER.methods_by_name['ValidateConfigureDeliveryExtension']._serialized_options = b'\202\323\344\223\002/\"*/v1/delivery_extensions/configure/validate:\001*'
   _DELIVERYEXTENSIONMANAGER.methods_by_name['ListDeliveryExtensions']._options = None
   _DELIVERYEXTENSIONMANAGER.methods_by_name['ListDeliveryExtensions']._serialized_options = b'\202\323\344\223\002\031\022\027/v1/delivery_extensions'
   _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtension']._options = None
   _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtension']._serialized_options = b'\202\323\344\223\002/\022-/v1/delivery_extension/{delivery_extension=*}'
   _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtensionConfig']._options = None
   _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtensionConfig']._serialized_options = b'\202\323\344\223\0026\0224/v1/delivery_extension/{delivery_extension=*}/config'
-  _CONFIGUREDELIVERYEXTENSIONREQ._serialized_start=254
-  _CONFIGUREDELIVERYEXTENSIONREQ._serialized_end=485
-  _CONFIGUREDELIVERYEXTENSIONRESP._serialized_start=487
-  _CONFIGUREDELIVERYEXTENSIONRESP._serialized_end=567
-  _VALIDATECONFIGUREDELIVERYEXTENSIONRESP._serialized_start=569
-  _VALIDATECONFIGUREDELIVERYEXTENSIONRESP._serialized_end=609
-  _LISTDELIVERYEXTENSIONSREQ._serialized_start=611
-  _LISTDELIVERYEXTENSIONSREQ._serialized_end=677
-  _LISTDELIVERYEXTENSIONSRESP._serialized_start=680
-  _LISTDELIVERYEXTENSIONSRESP._serialized_end=810
-  _GETDELIVERYEXTENSIONREQ._serialized_start=812
-  _GETDELIVERYEXTENSIONREQ._serialized_end=874
-  _GETDELIVERYEXTENSIONRESP._serialized_start=876
-  _GETDELIVERYEXTENSIONRESP._serialized_end=978
-  _GETDELIVERYEXTENSIONCONFIGREQ._serialized_start=980
-  _GETDELIVERYEXTENSIONCONFIGREQ._serialized_end=1065
-  _GETDELIVERYEXTENSIONCONFIGRESP._serialized_start=1067
-  _GETDELIVERYEXTENSIONCONFIGRESP._serialized_end=1186
-  _DELIVERYEXTENSIONMANAGER._serialized_start=1189
-  _DELIVERYEXTENSIONMANAGER._serialized_end=2212
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtensionInstanceConfig']._options = None
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtensionInstanceConfig']._serialized_options = b'\202\323\344\223\002K\022I/v1/delivery_extension/instance/{delivery_extension_instance_id=*}/config'
+  _globals['_CONFIGUREDELIVERYEXTENSIONREQ']._serialized_start=254
+  _globals['_CONFIGUREDELIVERYEXTENSIONREQ']._serialized_end=485
+  _globals['_CONFIGUREDELIVERYEXTENSIONRESP']._serialized_start=487
+  _globals['_CONFIGUREDELIVERYEXTENSIONRESP']._serialized_end=567
+  _globals['_VALIDATECONFIGUREDELIVERYEXTENSIONRESP']._serialized_start=569
+  _globals['_VALIDATECONFIGUREDELIVERYEXTENSIONRESP']._serialized_end=609
+  _globals['_LISTDELIVERYEXTENSIONSREQ']._serialized_start=611
+  _globals['_LISTDELIVERYEXTENSIONSREQ']._serialized_end=677
+  _globals['_LISTDELIVERYEXTENSIONSRESP']._serialized_start=680
+  _globals['_LISTDELIVERYEXTENSIONSRESP']._serialized_end=810
+  _globals['_GETDELIVERYEXTENSIONREQ']._serialized_start=812
+  _globals['_GETDELIVERYEXTENSIONREQ']._serialized_end=874
+  _globals['_GETDELIVERYEXTENSIONRESP']._serialized_start=876
+  _globals['_GETDELIVERYEXTENSIONRESP']._serialized_end=978
+  _globals['_GETDELIVERYEXTENSIONCONFIGREQ']._serialized_start=980
+  _globals['_GETDELIVERYEXTENSIONCONFIGREQ']._serialized_end=1065
+  _globals['_GETDELIVERYEXTENSIONCONFIGRESP']._serialized_start=1067
+  _globals['_GETDELIVERYEXTENSIONCONFIGRESP']._serialized_end=1186
+  _globals['_GETDELIVERYEXTENSIONINSTANCECONFIGREQ']._serialized_start=1188
+  _globals['_GETDELIVERYEXTENSIONINSTANCECONFIGREQ']._serialized_end=1293
+  _globals['_GETDELIVERYEXTENSIONINSTANCECONFIGRESP']._serialized_start=1296
+  _globals['_GETDELIVERYEXTENSIONINSTANCECONFIGRESP']._serialized_end=1439
+  _globals['_DELIVERYEXTENSIONMANAGER']._serialized_start=1442
+  _globals['_DELIVERYEXTENSIONMANAGER']._serialized_end=2724
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -165,7 +165,44 @@
         config: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
         version: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["config", b"config"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "version", b"version"]) -> None: ...
 
 global___GetDeliveryExtensionConfigResp = GetDeliveryExtensionConfigResp
+
+class GetDeliveryExtensionInstanceConfigReq(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DELIVERY_EXTENSION_INSTANCE_ID_FIELD_NUMBER: builtins.int
+    VERSION_FIELD_NUMBER: builtins.int
+    delivery_extension_instance_id: builtins.str
+    version: builtins.str
+    """omit to get latest version"""
+    def __init__(
+        self,
+        *,
+        delivery_extension_instance_id: builtins.str = ...,
+        version: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extension_instance_id", b"delivery_extension_instance_id", "version", b"version"]) -> None: ...
+
+global___GetDeliveryExtensionInstanceConfigReq = GetDeliveryExtensionInstanceConfigReq
+
+class GetDeliveryExtensionInstanceConfigResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    CONFIG_FIELD_NUMBER: builtins.int
+    VERSION_FIELD_NUMBER: builtins.int
+    @property
+    def config(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.CompiledDeliveryExtensionInstanceConfig: ...
+    version: builtins.str
+    def __init__(
+        self,
+        *,
+        config: prodvana.proto.prodvana.delivery_extension.config_pb2.CompiledDeliveryExtensionInstanceConfig | None = ...,
+        version: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["config", b"config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "version", b"version"]) -> None: ...
+
+global___GetDeliveryExtensionInstanceConfigResp = GetDeliveryExtensionInstanceConfigResp
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,19 @@
                 response_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionResp.FromString,
                 )
         self.GetDeliveryExtensionConfig = channel.unary_unary(
                 '/prodvana.delivery_extension.DeliveryExtensionManager/GetDeliveryExtensionConfig',
                 request_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigReq.SerializeToString,
                 response_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigResp.FromString,
                 )
+        self.GetDeliveryExtensionInstanceConfig = channel.unary_unary(
+                '/prodvana.delivery_extension.DeliveryExtensionManager/GetDeliveryExtensionInstanceConfig',
+                request_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionInstanceConfigReq.SerializeToString,
+                response_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionInstanceConfigResp.FromString,
+                )
 
 
 class DeliveryExtensionManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ConfigureDeliveryExtension(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -70,14 +75,20 @@
 
     def GetDeliveryExtensionConfig(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetDeliveryExtensionInstanceConfig(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DeliveryExtensionManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ConfigureDeliveryExtension': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureDeliveryExtension,
                     request_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionReq.FromString,
                     response_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionResp.SerializeToString,
@@ -98,14 +109,19 @@
                     response_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionResp.SerializeToString,
             ),
             'GetDeliveryExtensionConfig': grpc.unary_unary_rpc_method_handler(
                     servicer.GetDeliveryExtensionConfig,
                     request_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigReq.FromString,
                     response_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigResp.SerializeToString,
             ),
+            'GetDeliveryExtensionInstanceConfig': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetDeliveryExtensionInstanceConfig,
+                    request_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionInstanceConfigReq.FromString,
+                    response_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionInstanceConfigResp.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'prodvana.delivery_extension.DeliveryExtensionManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -192,7 +208,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_extension.DeliveryExtensionManager/GetDeliveryExtensionConfig',
             prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigReq.SerializeToString,
             prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetDeliveryExtensionInstanceConfig(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_extension.DeliveryExtensionManager/GetDeliveryExtensionInstanceConfig',
+            prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionInstanceConfigReq.SerializeToString,
+            prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionInstanceConfigResp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionReq,
         prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionResp,
     ]
     GetDeliveryExtensionConfig: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionConfigReq,
         prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionConfigResp,
     ]
+    GetDeliveryExtensionInstanceConfig: grpc.UnaryUnaryMultiCallable[
+        prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionInstanceConfigReq,
+        prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionInstanceConfigResp,
+    ]
 
 class DeliveryExtensionManagerServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def ConfigureDeliveryExtension(
         self,
         request: prodvana.proto.prodvana.delivery_extension.manager_pb2.ConfigureDeliveryExtensionReq,
         context: grpc.ServicerContext,
@@ -56,9 +60,15 @@
     ) -> prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionResp: ...
     @abc.abstractmethod
     def GetDeliveryExtensionConfig(
         self,
         request: prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionConfigReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionConfigResp: ...
+    @abc.abstractmethod
+    def GetDeliveryExtensionInstanceConfig(
+        self,
+        request: prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionInstanceConfigReq,
+        context: grpc.ServicerContext,
+    ) -> prodvana.proto.prodvana.delivery_extension.manager_pb2.GetDeliveryExtensionInstanceConfigResp: ...
 
 def add_DeliveryExtensionManagerServicer_to_server(servicer: DeliveryExtensionManagerServicer, server: grpc.Server) -> None: ...
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -261,48 +261,48 @@
             key: builtins.str = ...,
             value: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     ENTITY_GRAPH_FIELD_NUMBER: builtins.int
+    CREATION_TIMESTAMP_FIELD_NUMBER: builtins.int
+    REPLACED_TIMESTAMP_FIELD_NUMBER: builtins.int
     STARTING_STATE_FIELD_NUMBER: builtins.int
     LAST_SEEN_STATE_FIELD_NUMBER: builtins.int
     DESIRED_STATE_FIELD_NUMBER: builtins.int
     STATUSES_FIELD_NUMBER: builtins.int
-    CREATION_TIMESTAMP_FIELD_NUMBER: builtins.int
     LAST_UPDATE_TIMESTAMP_FIELD_NUMBER: builtins.int
-    REPLACED_TIMESTAMP_FIELD_NUMBER: builtins.int
     PRECONDITION_STATUSES_FIELD_NUMBER: builtins.int
     STATUS_EXPLANATIONS_FIELD_NUMBER: builtins.int
     DEBUG_LOGS_FIELD_NUMBER: builtins.int
     ACTION_EXPLANATIONS_FIELD_NUMBER: builtins.int
     LAST_UPDATE_TIMESTAMPS_FIELD_NUMBER: builtins.int
     LAST_FETCHED_TIMESTAMPS_FIELD_NUMBER: builtins.int
     LAST_APPLIED_TIMESTAMPS_FIELD_NUMBER: builtins.int
     @property
     def entity_graph(self) -> prodvana.proto.prodvana.desired_state.model.entity_pb2.EntityGraph: ...
     @property
+    def creation_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def replaced_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
+        """will only be set if desired state has been replaced"""
+    @property
     def starting_state(self) -> prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State:
         """fields below are deprecated"""
     @property
     def last_seen_state(self) -> prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State: ...
     @property
     def desired_state(self) -> prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State: ...
     @property
     def statuses(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Status.ValueType]:
         """status of the desired state, all its descendents, and the root desired state."""
     @property
-    def creation_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    @property
     def last_update_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
-    def replaced_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
-        """will only be set if desired state has been replaced"""
-    @property
     def precondition_statuses(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.desired_state.model.desired_state_pb2.ConditionState]:
         """State of all preconditions involved in the desired state.
         Key format - "{desired_state_id}-{index}", e.g., "des-0752d6c76a6943abbfcf0515634584ba-0".
         """
     @property
     def status_explanations(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___StatusExplanations]: ...
     @property
@@ -316,21 +316,21 @@
     def last_fetched_timestamps(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, google.protobuf.timestamp_pb2.Timestamp]: ...
     @property
     def last_applied_timestamps(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, google.protobuf.timestamp_pb2.Timestamp]: ...
     def __init__(
         self,
         *,
         entity_graph: prodvana.proto.prodvana.desired_state.model.entity_pb2.EntityGraph | None = ...,
+        creation_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        replaced_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         starting_state: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State | None = ...,
         last_seen_state: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State | None = ...,
         desired_state: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State | None = ...,
         statuses: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Status.ValueType] | None = ...,
-        creation_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_update_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        replaced_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         precondition_statuses: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.desired_state.model.desired_state_pb2.ConditionState] | None = ...,
         status_explanations: collections.abc.Mapping[builtins.str, global___StatusExplanations] | None = ...,
         debug_logs: collections.abc.Mapping[builtins.str, global___DebugLogs] | None = ...,
         action_explanations: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.desired_state.model.desired_state_pb2.ActionExplanation] | None = ...,
         last_update_timestamps: collections.abc.Mapping[builtins.str, google.protobuf.timestamp_pb2.Timestamp] | None = ...,
         last_fetched_timestamps: collections.abc.Mapping[builtins.str, google.protobuf.timestamp_pb2.Timestamp] | None = ...,
         last_applied_timestamps: collections.abc.Mapping[builtins.str, google.protobuf.timestamp_pb2.Timestamp] | None = ...,
@@ -599,7 +599,38 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___BypassProtectionResp = BypassProtectionResp
+
+class ApproveRuntimeExtensionApplyReq(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
+    SOURCE_FIELD_NUMBER: builtins.int
+    APPROVAL_TIMESTAMP_FIELD_NUMBER: builtins.int
+    desired_state_id: builtins.str
+    source: builtins.str
+    @property
+    def approval_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    def __init__(
+        self,
+        *,
+        desired_state_id: builtins.str = ...,
+        source: builtins.str = ...,
+        approval_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["approval_timestamp", b"approval_timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["approval_timestamp", b"approval_timestamp", "desired_state_id", b"desired_state_id", "source", b"source"]) -> None: ...
+
+global___ApproveRuntimeExtensionApplyReq = ApproveRuntimeExtensionApplyReq
+
+class ApproveRuntimeExtensionApplyResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___ApproveRuntimeExtensionApplyResp = ApproveRuntimeExtensionApplyResp
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,19 @@
                 response_deserializer=prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryResp.FromString,
                 )
         self.BypassProtection = channel.unary_unary(
                 '/prodvana.desired_state.DesiredStateManager/BypassProtection',
                 request_serializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionReq.SerializeToString,
                 response_deserializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionResp.FromString,
                 )
+        self.ApproveRuntimeExtensionApply = channel.unary_unary(
+                '/prodvana.desired_state.DesiredStateManager/ApproveRuntimeExtensionApply',
+                request_serializer=prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyReq.SerializeToString,
+                response_deserializer=prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyResp.FromString,
+                )
 
 
 class DesiredStateManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def SetDesiredState(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -125,14 +130,20 @@
 
     def BypassProtection(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ApproveRuntimeExtensionApply(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DesiredStateManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'SetDesiredState': grpc.unary_unary_rpc_method_handler(
                     servicer.SetDesiredState,
                     request_deserializer=prodvana_dot_desired__state_dot_manager__pb2.SetDesiredStateReq.FromString,
                     response_serializer=prodvana_dot_desired__state_dot_manager__pb2.SetDesiredStateResp.SerializeToString,
@@ -178,14 +189,19 @@
                     response_serializer=prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryResp.SerializeToString,
             ),
             'BypassProtection': grpc.unary_unary_rpc_method_handler(
                     servicer.BypassProtection,
                     request_deserializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionReq.FromString,
                     response_serializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionResp.SerializeToString,
             ),
+            'ApproveRuntimeExtensionApply': grpc.unary_unary_rpc_method_handler(
+                    servicer.ApproveRuntimeExtensionApply,
+                    request_deserializer=prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyReq.FromString,
+                    response_serializer=prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyResp.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'prodvana.desired_state.DesiredStateManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -357,7 +373,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/prodvana.desired_state.DesiredStateManager/BypassProtection',
             prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionReq.SerializeToString,
             prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ApproveRuntimeExtensionApply(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/prodvana.desired_state.DesiredStateManager/ApproveRuntimeExtensionApply',
+            prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyReq.SerializeToString,
+            prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyResp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,18 @@
         prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryReq,
         prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryResp,
     ]
     BypassProtection: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionReq,
         prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionResp,
     ]
+    ApproveRuntimeExtensionApply: grpc.UnaryUnaryMultiCallable[
+        prodvana.proto.prodvana.desired_state.manager_pb2.ApproveRuntimeExtensionApplyReq,
+        prodvana.proto.prodvana.desired_state.manager_pb2.ApproveRuntimeExtensionApplyResp,
+    ]
 
 class DesiredStateManagerServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def SetDesiredState(
         self,
         request: prodvana.proto.prodvana.desired_state.manager_pb2.SetDesiredStateReq,
         context: grpc.ServicerContext,
@@ -106,9 +110,15 @@
     ) -> prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryResp: ...
     @abc.abstractmethod
     def BypassProtection(
         self,
         request: prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionResp: ...
+    @abc.abstractmethod
+    def ApproveRuntimeExtensionApply(
+        self,
+        request: prodvana.proto.prodvana.desired_state.manager_pb2.ApproveRuntimeExtensionApplyReq,
+        context: grpc.ServicerContext,
+    ) -> prodvana.proto.prodvana.desired_state.manager_pb2.ApproveRuntimeExtensionApplyResp: ...
 
 def add_DesiredStateManagerServicer_to_server(servicer: DesiredStateManagerServicer, server: grpc.Server) -> None: ...
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
+import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.program_pb2
 import prodvana.proto.prodvana.common_config.retry_pb2
 import prodvana.proto.prodvana.common_config.task_pb2
 import prodvana.proto.prodvana.environment.clusters_pb2
 import prodvana.proto.prodvana.protection.protection_reference_pb2
 import sys
 import typing
@@ -173,14 +174,16 @@
     RUNTIME_OBJECT_FAILED: _StatusReason.ValueType  # 6
     """after applying successfully, the object arrived at a failed state"""
     PRECONDITIONS_FAILED: _StatusReason.ValueType  # 7
     """a precondition failed in an unrecoverable way"""
     MANUAL_APPROVAL_REJECTED: _StatusReason.ValueType  # 8
     STUCK_ENTITY: _StatusReason.ValueType  # 9
     """Entity has not been updated in a long time"""
+    VERSION_DIRTY: _StatusReason.ValueType  # 10
+    """the active version is explicitly marked as dirty"""
 
 class StatusReason(_StatusReason, metaclass=_StatusReasonEnumTypeWrapper): ...
 
 REASON_UNKNOWN: StatusReason.ValueType  # 0
 NO_CURRENT_STATE: StatusReason.ValueType  # 1
 """Prodvana has not fetched the data it needs to act on the entity"""
 APPLY_FAILED: StatusReason.ValueType  # 2
@@ -194,14 +197,16 @@
 RUNTIME_OBJECT_FAILED: StatusReason.ValueType  # 6
 """after applying successfully, the object arrived at a failed state"""
 PRECONDITIONS_FAILED: StatusReason.ValueType  # 7
 """a precondition failed in an unrecoverable way"""
 MANUAL_APPROVAL_REJECTED: StatusReason.ValueType  # 8
 STUCK_ENTITY: StatusReason.ValueType  # 9
 """Entity has not been updated in a long time"""
+VERSION_DIRTY: StatusReason.ValueType  # 10
+"""the active version is explicitly marked as dirty"""
 global___StatusReason = StatusReason
 
 class _ActionType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _ActionTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ActionType.ValueType], builtins.type):  # noqa: F821
@@ -287,20 +292,22 @@
     V: typing_extensions.TypeAlias = ValueType
 
 class _SignalTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SignalType.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SIGNAL_UNKNOWN: _SignalType.ValueType  # 0
     DELIVERY_PROMOTION: _SignalType.ValueType  # 1
     PROTECTION_BYPASS: _SignalType.ValueType  # 2
+    RUNTIME_EXTENSION_APPROVAL: _SignalType.ValueType  # 3
 
 class SignalType(_SignalType, metaclass=_SignalTypeEnumTypeWrapper): ...
 
 SIGNAL_UNKNOWN: SignalType.ValueType  # 0
 DELIVERY_PROMOTION: SignalType.ValueType  # 1
 PROTECTION_BYPASS: SignalType.ValueType  # 2
+RUNTIME_EXTENSION_APPROVAL: SignalType.ValueType  # 3
 global___SignalType = SignalType
 
 class ProtectionLink(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LIFECYCLE_FIELD_NUMBER: builtins.int
     ATTACHMENT_ID_FIELD_NUMBER: builtins.int
@@ -354,21 +361,24 @@
         ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "release_channel", b"release_channel", "release_channel_id", b"release_channel_id", "service", b"service", "service_id", b"service_id", "service_version", b"service_version"]) -> None: ...
 
     class ManualApproval(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TOPIC_FIELD_NUMBER: builtins.int
+        DESCRIPTION_FIELD_NUMBER: builtins.int
         topic: builtins.str
+        description: builtins.str
         def __init__(
             self,
             *,
             topic: builtins.str = ...,
+            description: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["topic", b"topic"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "topic", b"topic"]) -> None: ...
 
     class CustomTaskSuccessfulCondition(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         class Protection(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -472,40 +482,44 @@
     PRECONDITIONS_FIELD_NUMBER: builtins.int
     INVARIANTS_FIELD_NUMBER: builtins.int
     SELF_FIELD_NUMBER: builtins.int
     DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     ROOT_DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     PROTECTION_LINKS_FIELD_NUMBER: builtins.int
     DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
+    TARGET_STATE_SET_BY_PARENT_FIELD_NUMBER: builtins.int
     @property
     def preconditions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Condition]: ...
     @property
     def invariants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Condition]: ...
     @property
     def self(self) -> global___Identifier: ...
     desired_state_id: builtins.str
     root_desired_state_id: builtins.str
     @property
     def protection_links(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ProtectionLink]: ...
     @property
     def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtension]: ...
+    target_state_set_by_parent: builtins.bool
+    """if true, the entity does not set its own target state. instead, the target state will be set when the parent decides to set target state."""
     def __init__(
         # pyright: reportSelfClsParameterName=false
         self_,
         *,
         preconditions: collections.abc.Iterable[global___Condition] | None = ...,
         invariants: collections.abc.Iterable[global___Condition] | None = ...,
         self: global___Identifier | None = ...,
         desired_state_id: builtins.str = ...,
         root_desired_state_id: builtins.str = ...,
         protection_links: collections.abc.Iterable[global___ProtectionLink] | None = ...,
         delivery_extensions: collections.abc.Iterable[global___DeliveryExtension] | None = ...,
+        target_state_set_by_parent: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["self", b"self"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery_extensions", b"delivery_extensions", "desired_state_id", b"desired_state_id", "invariants", b"invariants", "preconditions", b"preconditions", "protection_links", b"protection_links", "root_desired_state_id", b"root_desired_state_id", "self", b"self"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extensions", b"delivery_extensions", "desired_state_id", b"desired_state_id", "invariants", b"invariants", "preconditions", b"preconditions", "protection_links", b"protection_links", "root_desired_state_id", b"root_desired_state_id", "self", b"self", "target_state_set_by_parent", b"target_state_set_by_parent"]) -> None: ...
 
 global___Metadata = Metadata
 
 class StatusExplanation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBJECT_FIELD_NUMBER: builtins.int
@@ -564,39 +578,46 @@
 
     VERSION_FIELD_NUMBER: builtins.int
     REPLICAS_FIELD_NUMBER: builtins.int
     AVAILABLE_REPLICAS_FIELD_NUMBER: builtins.int
     PUSH_TIMESTAMP_FIELD_NUMBER: builtins.int
     ACTIVE_FIELD_NUMBER: builtins.int
     TARGET_REPLICAS_FIELD_NUMBER: builtins.int
+    DIRTY_FIELD_NUMBER: builtins.int
     version: builtins.str
     replicas: builtins.int
     """Created/running replicas, can be in any state"""
     available_replicas: builtins.int
     """Replicas which have passed healthchecks for required duration."""
     @property
     def push_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     active: builtins.bool
     """A version is active if it is the version in which the underlying object is converging to.
     A runtime object will have exactly one active version, while a service instance may have one or more
     depending on if it maps to more than one runtime object.
     """
     target_replicas: builtins.int
+    dirty: builtins.bool
+    """A version is dirty if its state no longer matches desired state and must be fixed by a redeploy.
+    For example, a terraform version is dirty if its plan output returns differences.
+    DD will only take action on dirty if the version is also active.
+    """
     def __init__(
         self,
         *,
         version: builtins.str = ...,
         replicas: builtins.int = ...,
         available_replicas: builtins.int = ...,
         push_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         active: builtins.bool = ...,
         target_replicas: builtins.int = ...,
+        dirty: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["push_timestamp", b"push_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["active", b"active", "available_replicas", b"available_replicas", "push_timestamp", b"push_timestamp", "replicas", b"replicas", "target_replicas", b"target_replicas", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["active", b"active", "available_replicas", b"available_replicas", "dirty", b"dirty", "push_timestamp", b"push_timestamp", "replicas", b"replicas", "target_replicas", b"target_replicas", "version", b"version"]) -> None: ...
 
 global___Version = Version
 
 class ServiceInstanceState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
@@ -812,23 +833,25 @@
     def ClearField(self, field_name: typing_extensions.Literal["canary_progress", b"canary_progress", "desired_state_id", b"desired_state_id", "first_run", b"first_run", "generation", b"generation", "message", b"message", "status", b"status"]) -> None: ...
 
 global___DeliveryState = DeliveryState
 
 class RuntimeExtensionFetchOutput(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    VERSIONS_FIELD_NUMBER: builtins.int
-    @property
-    def versions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Version]: ...
+    DIRTY_FIELD_NUMBER: builtins.int
+    MESSAGE_FIELD_NUMBER: builtins.int
+    dirty: builtins.bool
+    message: builtins.str
     def __init__(
         self,
         *,
-        versions: collections.abc.Iterable[global___Version] | None = ...,
+        dirty: builtins.bool = ...,
+        message: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["versions", b"versions"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dirty", b"dirty", "message", b"message"]) -> None: ...
 
 global___RuntimeExtensionFetchOutput = RuntimeExtensionFetchOutput
 
 class RuntimeObject(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Status:
@@ -845,105 +868,132 @@
     PENDING: RuntimeObject.Status.ValueType  # 0
     SUCCEEDED: RuntimeObject.Status.ValueType  # 1
     FAILED: RuntimeObject.Status.ValueType  # 2
 
     class RuntimeExtension(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+        APPLY_FIELD_NUMBER: builtins.int
         FETCH_FIELD_NUMBER: builtins.int
+        FETCH_INTERVAL_FIELD_NUMBER: builtins.int
+        FETCH_TIMEOUT_FIELD_NUMBER: builtins.int
         SERVICE_ID_FIELD_NUMBER: builtins.int
+        RELEASE_CHANNEL_ID_FIELD_NUMBER: builtins.int
+        PARAMETERS_FIELD_NUMBER: builtins.int
+        PARAMETER_VALUES_FIELD_NUMBER: builtins.int
+        TYPE_FIELD_NUMBER: builtins.int
+        @property
+        def apply(self) -> prodvana.proto.prodvana.environment.clusters_pb2.CompiledExtensionCommand:
+            """aggregate object will have all commands set. Fetcher will only have fetch set."""
         @property
         def fetch(self) -> prodvana.proto.prodvana.environment.clusters_pb2.CompiledExtensionCommand: ...
+        @property
+        def fetch_interval(self) -> google.protobuf.duration_pb2.Duration: ...
+        @property
+        def fetch_timeout(self) -> google.protobuf.duration_pb2.Duration: ...
         service_id: builtins.str
+        release_channel_id: builtins.str
+        @property
+        def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
+        @property
+        def parameter_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]: ...
+        type: prodvana.proto.prodvana.environment.clusters_pb2.ExtensionType.ValueType
+        """next tag: 10"""
         def __init__(
             self,
             *,
+            apply: prodvana.proto.prodvana.environment.clusters_pb2.CompiledExtensionCommand | None = ...,
             fetch: prodvana.proto.prodvana.environment.clusters_pb2.CompiledExtensionCommand | None = ...,
+            fetch_interval: google.protobuf.duration_pb2.Duration | None = ...,
+            fetch_timeout: google.protobuf.duration_pb2.Duration | None = ...,
             service_id: builtins.str = ...,
+            release_channel_id: builtins.str = ...,
+            parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
+            parameter_values: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
+            type: prodvana.proto.prodvana.environment.clusters_pb2.ExtensionType.ValueType = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["fetch", b"fetch"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["fetch", b"fetch", "service_id", b"service_id"]) -> None: ...
-
-    class OutputBlobIdsEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
-        value: builtins.str
-        def __init__(
-            self,
-            *,
-            key: builtins.str = ...,
-            value: builtins.str = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["apply", b"apply", "fetch", b"fetch", "fetch_interval", b"fetch_interval", "fetch_timeout", b"fetch_timeout"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["apply", b"apply", "fetch", b"fetch", "fetch_interval", b"fetch_interval", "fetch_timeout", b"fetch_timeout", "parameter_values", b"parameter_values", "parameters", b"parameters", "release_channel_id", b"release_channel_id", "service_id", b"service_id", "type", b"type"]) -> None: ...
 
     META_FIELD_NUMBER: builtins.int
     OBJECT_TYPE_FIELD_NUMBER: builtins.int
     NAMESPACE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     VERSIONS_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     ROLLBACK_VERSION_FIELD_NUMBER: builtins.int
     DELIVERY_FIELD_NUMBER: builtins.int
     VERSION_AGNOSTIC_FIELD_NUMBER: builtins.int
+    DESIRED_VERSION_DIRTY_ONLY_FIELD_NUMBER: builtins.int
     MESSAGE_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
-    OUTPUT_BLOB_IDS_FIELD_NUMBER: builtins.int
     INTERVAL_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
+    OUTPUT_BLOB_IDS_FIELD_NUMBER: builtins.int
+    EXIT_CODES_FIELD_NUMBER: builtins.int
+    REQUIRE_APPROVAL_BEFORE_APPLY_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> global___Metadata: ...
     object_type: builtins.str
     namespace: builtins.str
     name: builtins.str
     @property
     def versions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Version]: ...
     status: global___RuntimeObject.Status.ValueType
     @property
     def rollback_version(self) -> global___Version: ...
     @property
     def delivery(self) -> global___DeliveryState: ...
     version_agnostic: builtins.bool
     """This object just needs to exist - it doesn't change from version to version"""
+    desired_version_dirty_only: builtins.bool
+    """when checking for whether or not to apply, only use the desired version and check if it's active and not dirty. that is, active && at desired version && dirty = hasWork, no work otherwise."""
     message: builtins.str
     """Human readable message (typically for errors)."""
     @property
     def runtime_extension(self) -> global___RuntimeObject.RuntimeExtension:
         """additional config if this runtime object belongs to a runtime extension"""
     @property
-    def output_blob_ids(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
-        """if output is saved, this is the ID of the blob to retrieve it, by container name"""
-    @property
     def interval(self) -> google.protobuf.duration_pb2.Duration:
         """if set, runtime object is continuously applied instead of being done once when there is a version mismatch"""
     @property
     def timeout(self) -> google.protobuf.duration_pb2.Duration:
         """if set, runtime object is recreated when this timeout is hit if it has not converged by then."""
+    @property
+    def output_blob_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """output_blob_ids and exit_codes are in the same order, assuming output is saved
+        if output is saved, this is the ID of the blob to retrieve it, only for run-to-completion objects.
+        """
+    @property
+    def exit_codes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """exit codes, only for run-to-completion objects like jobs"""
+    require_approval_before_apply: builtins.bool
     def __init__(
         self,
         *,
         meta: global___Metadata | None = ...,
         object_type: builtins.str = ...,
         namespace: builtins.str = ...,
         name: builtins.str = ...,
         versions: collections.abc.Iterable[global___Version] | None = ...,
         status: global___RuntimeObject.Status.ValueType = ...,
         rollback_version: global___Version | None = ...,
         delivery: global___DeliveryState | None = ...,
         version_agnostic: builtins.bool = ...,
+        desired_version_dirty_only: builtins.bool = ...,
         message: builtins.str = ...,
         runtime_extension: global___RuntimeObject.RuntimeExtension | None = ...,
-        output_blob_ids: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         interval: google.protobuf.duration_pb2.Duration | None = ...,
         timeout: google.protobuf.duration_pb2.Duration | None = ...,
+        output_blob_ids: collections.abc.Iterable[builtins.str] | None = ...,
+        exit_codes: collections.abc.Iterable[builtins.int] | None = ...,
+        require_approval_before_apply: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "interval", b"interval", "meta", b"meta", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "timeout", b"timeout"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "interval", b"interval", "message", b"message", "meta", b"meta", "name", b"name", "namespace", b"namespace", "object_type", b"object_type", "output_blob_ids", b"output_blob_ids", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "status", b"status", "timeout", b"timeout", "version_agnostic", b"version_agnostic", "versions", b"versions"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "desired_version_dirty_only", b"desired_version_dirty_only", "exit_codes", b"exit_codes", "interval", b"interval", "message", b"message", "meta", b"meta", "name", b"name", "namespace", b"namespace", "object_type", b"object_type", "output_blob_ids", b"output_blob_ids", "require_approval_before_apply", b"require_approval_before_apply", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "status", b"status", "timeout", b"timeout", "version_agnostic", b"version_agnostic", "versions", b"versions"]) -> None: ...
 
 global___RuntimeObject = RuntimeObject
 
 class ConditionState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
@@ -962,14 +1012,16 @@
 
     ROLLBACK_FIELD_NUMBER: builtins.int
     PRECONDITION_STATES_FIELD_NUMBER: builtins.int
     INVARIANT_STATES_FIELD_NUMBER: builtins.int
     PAUSED_FIELD_NUMBER: builtins.int
     STATUS_EXPLANATIONS_FIELD_NUMBER: builtins.int
     ACTION_EXPLANATION_FIELD_NUMBER: builtins.int
+    LAST_FETCHED_TIMESTAMP_FIELD_NUMBER: builtins.int
+    LAST_APPLIED_TIMESTAMP_FIELD_NUMBER: builtins.int
     rollback: builtins.bool
     @property
     def precondition_states(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ConditionState]: ...
     @property
     def invariant_states(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ConditionState]: ...
     paused: builtins.bool
     """An entity is paused if itself or any of its ancestors have paused field set.
@@ -979,48 +1031,57 @@
     """
     @property
     def status_explanations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StatusExplanation]:
         """explanation for current status, will have more than one in the event multiple children have the same status"""
     @property
     def action_explanation(self) -> global___ActionExplanation:
         """What is DD doing now?"""
+    @property
+    def last_fetched_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def last_applied_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     def __init__(
         self,
         *,
         rollback: builtins.bool = ...,
         precondition_states: collections.abc.Iterable[global___ConditionState] | None = ...,
         invariant_states: collections.abc.Iterable[global___ConditionState] | None = ...,
         paused: builtins.bool = ...,
         status_explanations: collections.abc.Iterable[global___StatusExplanation] | None = ...,
         action_explanation: global___ActionExplanation | None = ...,
+        last_fetched_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        last_applied_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "invariant_states", b"invariant_states", "paused", b"paused", "precondition_states", b"precondition_states", "rollback", b"rollback", "status_explanations", b"status_explanations"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "invariant_states", b"invariant_states", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "paused", b"paused", "precondition_states", b"precondition_states", "rollback", b"rollback", "status_explanations", b"status_explanations"]) -> None: ...
 
 global___ControlState = ControlState
 
 class ManualApprovalState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     TOPIC_FIELD_NUMBER: builtins.int
+    DESCRIPTION_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> global___Metadata: ...
     status: global___ManualApprovalStatus.ValueType
     topic: builtins.str
+    description: builtins.str
     def __init__(
         self,
         *,
         meta: global___Metadata | None = ...,
         status: global___ManualApprovalStatus.ValueType = ...,
         topic: builtins.str = ...,
+        description: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["meta", b"meta"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["meta", b"meta", "status", b"status", "topic", b"topic"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "meta", b"meta", "status", b"status", "topic", b"topic"]) -> None: ...
 
 global___ManualApprovalState = ManualApprovalState
 
 class State(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVICE_FIELD_NUMBER: builtins.int
@@ -1360,32 +1421,55 @@
     class ProtectionBypass(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         def __init__(
             self,
         ) -> None: ...
 
+    class RuntimeExtensionApproval(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        TIMESTAMP_FIELD_NUMBER: builtins.int
+        @property
+        def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
+            """When was the approval issued?
+            If this is after last run timestamp, apply can proceed.
+            TODO: Add actor info - who/what approved and how?
+            TODO: Add some kind of token derived from corresponding fetch which can be passed down to apply.
+            """
+        def __init__(
+            self,
+            *,
+            timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> None: ...
+
     TYPE_FIELD_NUMBER: builtins.int
     DELIVERY_PROMOTION_FIELD_NUMBER: builtins.int
     PROTECTION_BYPASS_FIELD_NUMBER: builtins.int
+    RUNTIME_EXTENSION_APPROVAL_FIELD_NUMBER: builtins.int
     type: global___SignalType.ValueType
     @property
     def delivery_promotion(self) -> global___Signal.DeliveryPromotionConfig: ...
     @property
     def protection_bypass(self) -> global___Signal.ProtectionBypass: ...
+    @property
+    def runtime_extension_approval(self) -> global___Signal.RuntimeExtensionApproval: ...
     def __init__(
         self,
         *,
         type: global___SignalType.ValueType = ...,
         delivery_promotion: global___Signal.DeliveryPromotionConfig | None = ...,
         protection_bypass: global___Signal.ProtectionBypass | None = ...,
+        runtime_extension_approval: global___Signal.RuntimeExtensionApproval | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["config", b"config", "delivery_promotion", b"delivery_promotion", "protection_bypass", b"protection_bypass"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "delivery_promotion", b"delivery_promotion", "protection_bypass", b"protection_bypass", "type", b"type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config", b"config"]) -> typing_extensions.Literal["delivery_promotion", "protection_bypass"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["config", b"config", "delivery_promotion", b"delivery_promotion", "protection_bypass", b"protection_bypass", "runtime_extension_approval", b"runtime_extension_approval"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "delivery_promotion", b"delivery_promotion", "protection_bypass", b"protection_bypass", "runtime_extension_approval", b"runtime_extension_approval", "type", b"type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config", b"config"]) -> typing_extensions.Literal["delivery_promotion", "protection_bypass", "runtime_extension_approval"] | None: ...
 
 global___Signal = Signal
 
 class DebugLog(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TS_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/desired_state/model/entity.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.desired_state.model import desired_state_pb2 as prodvana_dot_desired__state_dot_model_dot_desired__state__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/desired_state/model/entity.proto\x12\x1cprodvana.desired_state.model\x1a!prodvana/common_config/task.proto\x1a\x30prodvana/desired_state/model/desired_state.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xb2\x08\n\x06\x45ntity\x12\x34\n\x02id\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x02 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x03 \x01(\t\x12>\n\x0b\x61nnotations\x18\x04 \x01(\x0b\x32).prodvana.desired_state.model.Annotations\x12\x34\n\x06status\x18\x05 \x01(\x0e\x32$.prodvana.desired_state.model.Status\x12\x41\n\rsimple_status\x18\x11 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12;\n\x0estarting_state\x18\x06 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12<\n\x0flast_seen_state\x18\x07 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12:\n\rdesired_state\x18\x08 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12K\n\x15precondition_statuses\x18\t \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12L\n\x13status_explanations\x18\n \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12\x34\n\x04logs\x18\x0b \x03(\x0b\x32&.prodvana.desired_state.model.DebugLog\x12K\n\x12\x61\x63tion_explanation\x18\x0c \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\x12\x39\n\x15last_update_timestamp\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_fetched_timestamp\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_applied_timestamp\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x0c\x64\x65pendencies\x18\x10 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x38\n\tlifecycle\x18\x12 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\"}\n\x0b\x45ntityGraph\x12\x36\n\x04root\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x36\n\x08\x65ntities\x18\x02 \x03(\x0b\x32$.prodvana.desired_state.model.EntityBXZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
 
-
-
-_ENTITY = DESCRIPTOR.message_types_by_name['Entity']
-_ENTITYGRAPH = DESCRIPTOR.message_types_by_name['EntityGraph']
-Entity = _reflection.GeneratedProtocolMessageType('Entity', (_message.Message,), {
-  'DESCRIPTOR' : _ENTITY,
-  '__module__' : 'prodvana.desired_state.model.entity_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.Entity)
-  })
-_sym_db.RegisterMessage(Entity)
-
-EntityGraph = _reflection.GeneratedProtocolMessageType('EntityGraph', (_message.Message,), {
-  'DESCRIPTOR' : _ENTITYGRAPH,
-  '__module__' : 'prodvana.desired_state.model.entity_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.EntityGraph)
-  })
-_sym_db.RegisterMessage(EntityGraph)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.desired_state.model.entity_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/model'
-  _ENTITY._serialized_start=194
-  _ENTITY._serialized_end=1268
-  _ENTITYGRAPH._serialized_start=1270
-  _ENTITYGRAPH._serialized_end=1395
+  _globals['_ENTITY']._serialized_start=194
+  _globals['_ENTITY']._serialized_end=1268
+  _globals['_ENTITYGRAPH']._serialized_start=1270
+  _globals['_ENTITYGRAPH']._serialized_end=1395
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
 import prodvana.proto.prodvana.common_config.env_pb2
 import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
 import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.task_pb2
 import prodvana.proto.prodvana.runtimes.runtimes_config_pb2
+import prodvana.proto.prodvana.volumes.volumes_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
@@ -32,24 +33,45 @@
 class _ClusterTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ClusterType.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     UNKNOWN: _ClusterType.ValueType  # 0
     K8S: _ClusterType.ValueType  # 1
     ECS: _ClusterType.ValueType  # 2
     FAKE: _ClusterType.ValueType  # 3
     EXTENSION: _ClusterType.ValueType  # 4
+    TERRAFORM_RUNNER: _ClusterType.ValueType  # 5
+    PULUMI_RUNNER: _ClusterType.ValueType  # 6
 
 class ClusterType(_ClusterType, metaclass=_ClusterTypeEnumTypeWrapper): ...
 
 UNKNOWN: ClusterType.ValueType  # 0
 K8S: ClusterType.ValueType  # 1
 ECS: ClusterType.ValueType  # 2
 FAKE: ClusterType.ValueType  # 3
 EXTENSION: ClusterType.ValueType  # 4
+TERRAFORM_RUNNER: ClusterType.ValueType  # 5
+PULUMI_RUNNER: ClusterType.ValueType  # 6
 global___ClusterType = ClusterType
 
+class _ExtensionType:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _ExtensionTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ExtensionType.ValueType], builtins.type):  # noqa: F821
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    GENERIC: _ExtensionType.ValueType  # 0
+    TERRAFORM: _ExtensionType.ValueType  # 1
+    PULUMI: _ExtensionType.ValueType  # 2
+
+class ExtensionType(_ExtensionType, metaclass=_ExtensionTypeEnumTypeWrapper): ...
+
+GENERIC: ExtensionType.ValueType  # 0
+TERRAFORM: ExtensionType.ValueType  # 1
+PULUMI: ExtensionType.ValueType  # 2
+global___ExtensionType = ExtensionType
+
 class ClusterAuth(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class ECSAuth(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         ACCESS_KEY_FIELD_NUMBER: builtins.int
@@ -88,22 +110,26 @@
                 *,
                 key: builtins.str = ...,
                 value: builtins.str = ...,
             ) -> None: ...
             def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
         AGENT_ENV_FIELD_NUMBER: builtins.int
+        AGENT_EXTERNALLY_MANAGED_FIELD_NUMBER: builtins.int
         @property
         def agent_env(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+        agent_externally_managed: builtins.bool
+        """The Prodvana agent lifecycle is handled by the user -- Prodvana will not install or update the agent."""
         def __init__(
             self,
             *,
             agent_env: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+            agent_externally_managed: builtins.bool = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["agent_env", b"agent_env"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["agent_env", b"agent_env", "agent_externally_managed", b"agent_externally_managed"]) -> None: ...
 
     ENDPOINT_FIELD_NUMBER: builtins.int
     CA_CERT_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     SERVICE_ACCOUNT_FIELD_NUMBER: builtins.int
     ECS_FIELD_NUMBER: builtins.int
     K8S_FIELD_NUMBER: builtins.int
@@ -223,70 +249,98 @@
     def ClearField(self, field_name: typing_extensions.Literal["crashing_programs", b"crashing_programs"]) -> None: ...
 
 global___FakeClusterConfig = FakeClusterConfig
 
 class ExtensionCommand(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    class EnvEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> prodvana.proto.prodvana.common_config.env_pb2.EnvValue: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: prodvana.proto.prodvana.common_config.env_pb2.EnvValue | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     TASK_CONFIG_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     POLL_INTERVAL_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
+    ENV_FIELD_NUMBER: builtins.int
     @property
     def task_config(self) -> prodvana.proto.prodvana.common_config.task_pb2.TaskConfig: ...
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def poll_interval(self) -> google.protobuf.duration_pb2.Duration:
         """customize intervals instead of using Prodvana default
         only used for fetch
         how often to run command after it succeeds
         """
     @property
     def timeout(self) -> google.protobuf.duration_pb2.Duration:
         """how long after a run has started to try another run if it has not completed yet"""
+    @property
+    def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
+        """optional env variables to inject and override from exec_config"""
     def __init__(
         self,
         *,
         task_config: prodvana.proto.prodvana.common_config.task_pb2.TaskConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         poll_interval: google.protobuf.duration_pb2.Duration | None = ...,
         timeout: google.protobuf.duration_pb2.Duration | None = ...,
+        env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["env", b"env", "exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["exec_config", b"exec_config"]) -> typing_extensions.Literal["task_config", "kubernetes_config"] | None: ...
 
 global___ExtensionCommand = ExtensionCommand
 
 class ExtensionClusterConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLY_FIELD_NUMBER: builtins.int
     FETCH_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PROXY_RUNTIME_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
+    REQUIRE_APPROVAL_BEFORE_APPLY_FIELD_NUMBER: builtins.int
     @property
     def apply(self) -> global___ExtensionCommand: ...
     @property
     def fetch(self) -> global___ExtensionCommand: ...
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
     @property
     def proxy_runtime(self) -> prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig: ...
+    type: global___ExtensionType.ValueType
+    require_approval_before_apply: builtins.bool
     def __init__(
         self,
         *,
         apply: global___ExtensionCommand | None = ...,
         fetch: global___ExtensionCommand | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         proxy_runtime: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig | None = ...,
+        type: global___ExtensionType.ValueType = ...,
+        require_approval_before_apply: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["apply", b"apply", "fetch", b"fetch", "proxy_runtime", b"proxy_runtime"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["apply", b"apply", "fetch", b"fetch", "parameters", b"parameters", "proxy_runtime", b"proxy_runtime"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["apply", b"apply", "fetch", b"fetch", "parameters", b"parameters", "proxy_runtime", b"proxy_runtime", "require_approval_before_apply", b"require_approval_before_apply", "type", b"type"]) -> None: ...
 
 global___ExtensionClusterConfig = ExtensionClusterConfig
 
 class CompiledExtensionCommand(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class EnvEntry(google.protobuf.message.Message):
@@ -326,14 +380,138 @@
         env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["command", b"command", "runtime_execution", b"runtime_execution"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["command", b"command", "env", b"env", "name_prefix", b"name_prefix", "runtime_execution", b"runtime_execution"]) -> None: ...
 
 global___CompiledExtensionCommand = CompiledExtensionCommand
 
+class IacRunnerCommand(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    CMD_FIELD_NUMBER: builtins.int
+    cmd: builtins.str
+    def __init__(
+        self,
+        *,
+        cmd: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cmd", b"cmd"]) -> None: ...
+
+global___IacRunnerCommand = IacRunnerCommand
+
+class TerraformRunnerConfig(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class EnvEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> prodvana.proto.prodvana.common_config.env_pb2.EnvValue: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: prodvana.proto.prodvana.common_config.env_pb2.EnvValue | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
+    PROXY_RUNTIME_FIELD_NUMBER: builtins.int
+    ENV_FIELD_NUMBER: builtins.int
+    VOLUMES_FIELD_NUMBER: builtins.int
+    PRE_RUN_FIELD_NUMBER: builtins.int
+    POLL_INTERVAL_FIELD_NUMBER: builtins.int
+    REQUIRE_APPROVAL_BEFORE_APPLY_FIELD_NUMBER: builtins.int
+    @property
+    def proxy_runtime(self) -> prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig: ...
+    @property
+    def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
+        """optional env variables to pass to terraform commands, can be useful for passing secrets"""
+    @property
+    def volumes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.volumes.volumes_pb2.Volume]:
+        """optional volumes to mount into terraform containers"""
+    @property
+    def pre_run(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IacRunnerCommand]:
+        """commands that must run before terraform can run, e.g. gcloud auth login"""
+    @property
+    def poll_interval(self) -> google.protobuf.duration_pb2.Duration:
+        """Poll interval for terraform plan, defaults to 2 minutes. Polling takes a lock on terraform state file, so increase this if you run terraform plan locally often."""
+    require_approval_before_apply: builtins.bool
+    """Require approval before every apply operation - this is on top of any release channel-level approvals."""
+    def __init__(
+        self,
+        *,
+        proxy_runtime: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig | None = ...,
+        env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
+        volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
+        pre_run: collections.abc.Iterable[global___IacRunnerCommand] | None = ...,
+        poll_interval: google.protobuf.duration_pb2.Duration | None = ...,
+        require_approval_before_apply: builtins.bool = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["poll_interval", b"poll_interval", "proxy_runtime", b"proxy_runtime"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["env", b"env", "poll_interval", b"poll_interval", "pre_run", b"pre_run", "proxy_runtime", b"proxy_runtime", "require_approval_before_apply", b"require_approval_before_apply", "volumes", b"volumes"]) -> None: ...
+
+global___TerraformRunnerConfig = TerraformRunnerConfig
+
+class PulumiRunnerConfig(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class EnvEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> prodvana.proto.prodvana.common_config.env_pb2.EnvValue: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: prodvana.proto.prodvana.common_config.env_pb2.EnvValue | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
+    PROXY_RUNTIME_FIELD_NUMBER: builtins.int
+    ENV_FIELD_NUMBER: builtins.int
+    VOLUMES_FIELD_NUMBER: builtins.int
+    PRE_RUN_FIELD_NUMBER: builtins.int
+    POLL_INTERVAL_FIELD_NUMBER: builtins.int
+    @property
+    def proxy_runtime(self) -> prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig: ...
+    @property
+    def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
+        """optional env variables to pass to pulumi commands, can be useful for passing secrets"""
+    @property
+    def volumes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.volumes.volumes_pb2.Volume]:
+        """optional volumes to mount into pulumi containers"""
+    @property
+    def pre_run(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IacRunnerCommand]:
+        """commands that must run before pulumi can run, e.g. gcloud auth login"""
+    @property
+    def poll_interval(self) -> google.protobuf.duration_pb2.Duration:
+        """Poll interval for pulumi preview, defaults to 2 minutes. Polling takes a lock on pulumi state file, so increase this if you run terraform plan locally often."""
+    def __init__(
+        self,
+        *,
+        proxy_runtime: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig | None = ...,
+        env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
+        volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
+        pre_run: collections.abc.Iterable[global___IacRunnerCommand] | None = ...,
+        poll_interval: google.protobuf.duration_pb2.Duration | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["poll_interval", b"poll_interval", "proxy_runtime", b"proxy_runtime"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["env", b"env", "poll_interval", b"poll_interval", "pre_run", b"pre_run", "proxy_runtime", b"proxy_runtime", "volumes", b"volumes"]) -> None: ...
+
+global___PulumiRunnerConfig = PulumiRunnerConfig
+
 class ClusterConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _CloudProvider:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -507,14 +685,16 @@
     ALB_INGRESS_FIELD_NUMBER: builtins.int
     ARGO_ROLLOUTS_FIELD_NUMBER: builtins.int
     GKE_INGRESS_FIELD_NUMBER: builtins.int
     SELF_MANAGED_GKE_INGRESS_FIELD_NUMBER: builtins.int
     CLOUD_PROVIDER_FIELD_NUMBER: builtins.int
     FAKE_FIELD_NUMBER: builtins.int
     EXTENSION_FIELD_NUMBER: builtins.int
+    TERRAFORM_RUNNER_FIELD_NUMBER: builtins.int
+    PULUMI_RUNNER_FIELD_NUMBER: builtins.int
     name: builtins.str
     disable_flagger: builtins.bool
     disable_istio: builtins.bool
     @property
     def kubecost(self) -> global___ClusterConfig.Kubecost: ...
     @property
     def datadog(self) -> global___ClusterConfig.Datadog: ...
@@ -531,14 +711,20 @@
         """
     cloud_provider: global___ClusterConfig.CloudProvider.ValueType
     @property
     def fake(self) -> global___FakeClusterConfig:
         """only used for fake runtimes"""
     @property
     def extension(self) -> global___ExtensionClusterConfig: ...
+    @property
+    def terraform_runner(self) -> global___TerraformRunnerConfig:
+        """terraform runner is a runtime that runs terraform via k8s jobs"""
+    @property
+    def pulumi_runner(self) -> global___TerraformRunnerConfig:
+        """pulumi runner is a runtime that runs pulumi via k8s jobs"""
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         disable_flagger: builtins.bool = ...,
         disable_istio: builtins.bool = ...,
         kubecost: global___ClusterConfig.Kubecost | None = ...,
@@ -546,13 +732,15 @@
         alb_ingress: global___ClusterConfig.ALBIngress | None = ...,
         argo_rollouts: global___ClusterConfig.ArgoRollouts | None = ...,
         gke_ingress: global___ClusterConfig.GKEIngress | None = ...,
         self_managed_gke_ingress: global___ClusterConfig.GKEIngress | None = ...,
         cloud_provider: global___ClusterConfig.CloudProvider.ValueType = ...,
         fake: global___FakeClusterConfig | None = ...,
         extension: global___ExtensionClusterConfig | None = ...,
+        terraform_runner: global___TerraformRunnerConfig | None = ...,
+        pulumi_runner: global___TerraformRunnerConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["alb_ingress", b"alb_ingress", "argo_rollouts", b"argo_rollouts", "cluster_oneof", b"cluster_oneof", "datadog", b"datadog", "extension", b"extension", "fake", b"fake", "gke_ingress", b"gke_ingress", "kubecost", b"kubecost", "self_managed_gke_ingress", b"self_managed_gke_ingress"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["alb_ingress", b"alb_ingress", "argo_rollouts", b"argo_rollouts", "cloud_provider", b"cloud_provider", "cluster_oneof", b"cluster_oneof", "datadog", b"datadog", "disable_flagger", b"disable_flagger", "disable_istio", b"disable_istio", "extension", b"extension", "fake", b"fake", "gke_ingress", b"gke_ingress", "kubecost", b"kubecost", "name", b"name", "self_managed_gke_ingress", b"self_managed_gke_ingress"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["cluster_oneof", b"cluster_oneof"]) -> typing_extensions.Literal["fake", "extension"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["alb_ingress", b"alb_ingress", "argo_rollouts", b"argo_rollouts", "cluster_oneof", b"cluster_oneof", "datadog", b"datadog", "extension", b"extension", "fake", b"fake", "gke_ingress", b"gke_ingress", "kubecost", b"kubecost", "pulumi_runner", b"pulumi_runner", "self_managed_gke_ingress", b"self_managed_gke_ingress", "terraform_runner", b"terraform_runner"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["alb_ingress", b"alb_ingress", "argo_rollouts", b"argo_rollouts", "cloud_provider", b"cloud_provider", "cluster_oneof", b"cluster_oneof", "datadog", b"datadog", "disable_flagger", b"disable_flagger", "disable_istio", b"disable_istio", "extension", b"extension", "fake", b"fake", "gke_ingress", b"gke_ingress", "kubecost", b"kubecost", "name", b"name", "pulumi_runner", b"pulumi_runner", "self_managed_gke_ingress", b"self_managed_gke_ingress", "terraform_runner", b"terraform_runner"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["cluster_oneof", b"cluster_oneof"]) -> typing_extensions.Literal["fake", "extension", "terraform_runner", "pulumi_runner"] | None: ...
 
 global___ClusterConfig = ClusterConfig
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,42 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+class GetClusterAgentApiTokenReq(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    NAME_FIELD_NUMBER: builtins.int
+    name: builtins.str
+    def __init__(
+        self,
+        *,
+        name: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["name", b"name"]) -> None: ...
+
+global___GetClusterAgentApiTokenReq = GetClusterAgentApiTokenReq
+
+class GetClusterAgentApiTokenResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    API_TOKEN_FIELD_NUMBER: builtins.int
+    api_token: builtins.str
+    def __init__(
+        self,
+        *,
+        api_token: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["api_token", b"api_token"]) -> None: ...
+
+global___GetClusterAgentApiTokenResp = GetClusterAgentApiTokenResp
+
 class LinkClusterReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     AUTH_FIELD_NUMBER: builtins.int
     PRODVANA_MANAGED_FIELD_NUMBER: builtins.int
     DISABLE_ISTIO_FIELD_NUMBER: builtins.int
@@ -62,31 +90,42 @@
 class LinkClusterResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUCCESS_FIELD_NUMBER: builtins.int
     MSG_FIELD_NUMBER: builtins.int
     CLUSTER_ID_FIELD_NUMBER: builtins.int
     K8S_AGENT_URL_FIELD_NUMBER: builtins.int
+    K8S_AGENT_IMAGE_FIELD_NUMBER: builtins.int
+    K8S_AGENT_ARGS_FIELD_NUMBER: builtins.int
+    K8S_AGENT_API_TOKEN_FIELD_NUMBER: builtins.int
     success: builtins.bool
     """LinkCluster will attempt to talk to the cluster to validate the
     credentials. If it fails, want to communicate back what the failure was.
     """
     msg: builtins.str
     cluster_id: builtins.str
     k8s_agent_url: builtins.str
     """Magic URL to install agent"""
+    k8s_agent_image: builtins.str
+    """agent details broken out for externally constructing the agent configuration"""
+    @property
+    def k8s_agent_args(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    k8s_agent_api_token: builtins.str
     def __init__(
         self,
         *,
         success: builtins.bool = ...,
         msg: builtins.str = ...,
         cluster_id: builtins.str = ...,
         k8s_agent_url: builtins.str = ...,
+        k8s_agent_image: builtins.str = ...,
+        k8s_agent_args: collections.abc.Iterable[builtins.str] | None = ...,
+        k8s_agent_api_token: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cluster_id", b"cluster_id", "k8s_agent_url", b"k8s_agent_url", "msg", b"msg", "success", b"success"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cluster_id", b"cluster_id", "k8s_agent_api_token", b"k8s_agent_api_token", "k8s_agent_args", b"k8s_agent_args", "k8s_agent_image", b"k8s_agent_image", "k8s_agent_url", b"k8s_agent_url", "msg", b"msg", "success", b"success"]) -> None: ...
 
 global___LinkClusterResp = LinkClusterResp
 
 class RemoveClusterReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
@@ -175,55 +214,97 @@
         ORIGIN_FIELD_NUMBER: builtins.int
         ENDPOINT_FIELD_NUMBER: builtins.int
         SERVICE_ACCOUNT_FIELD_NUMBER: builtins.int
         WRITEBACK_CONFIG_FIELD_NUMBER: builtins.int
         TYPE_FIELD_NUMBER: builtins.int
         ECS_FIELD_NUMBER: builtins.int
         LAST_HEARTBEAT_TIMESTAMP_FIELD_NUMBER: builtins.int
+        CONFIG_FIELD_NUMBER: builtins.int
+        AUTH_FIELD_NUMBER: builtins.int
         name: builtins.str
         id: builtins.str
         origin: prodvana.proto.prodvana.environment.clusters_pb2.Cluster.Origin.ValueType
         endpoint: builtins.str
         service_account: builtins.str
         @property
         def writeback_config(self) -> prodvana.proto.prodvana.config_writeback.writeback_pb2.ConfigWritebackPath: ...
         type: prodvana.proto.prodvana.environment.clusters_pb2.ClusterType.ValueType
         @property
         def ecs(self) -> global___ListClustersResp.ClusterInfo.EcsInfo: ...
         @property
         def last_heartbeat_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+        @property
+        def config(self) -> prodvana.proto.prodvana.environment.clusters_pb2.ClusterConfig: ...
+        @property
+        def auth(self) -> prodvana.proto.prodvana.environment.clusters_pb2.ClusterAuth: ...
         def __init__(
             self,
             *,
             name: builtins.str = ...,
             id: builtins.str = ...,
             origin: prodvana.proto.prodvana.environment.clusters_pb2.Cluster.Origin.ValueType = ...,
             endpoint: builtins.str = ...,
             service_account: builtins.str = ...,
             writeback_config: prodvana.proto.prodvana.config_writeback.writeback_pb2.ConfigWritebackPath | None = ...,
             type: prodvana.proto.prodvana.environment.clusters_pb2.ClusterType.ValueType = ...,
             ecs: global___ListClustersResp.ClusterInfo.EcsInfo | None = ...,
             last_heartbeat_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+            config: prodvana.proto.prodvana.environment.clusters_pb2.ClusterConfig | None = ...,
+            auth: prodvana.proto.prodvana.environment.clusters_pb2.ClusterAuth | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["ecs", b"ecs", "info", b"info", "last_heartbeat_timestamp", b"last_heartbeat_timestamp", "writeback_config", b"writeback_config"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["ecs", b"ecs", "endpoint", b"endpoint", "id", b"id", "info", b"info", "last_heartbeat_timestamp", b"last_heartbeat_timestamp", "name", b"name", "origin", b"origin", "service_account", b"service_account", "type", b"type", "writeback_config", b"writeback_config"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["auth", b"auth", "config", b"config", "ecs", b"ecs", "info", b"info", "last_heartbeat_timestamp", b"last_heartbeat_timestamp", "writeback_config", b"writeback_config"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["auth", b"auth", "config", b"config", "ecs", b"ecs", "endpoint", b"endpoint", "id", b"id", "info", b"info", "last_heartbeat_timestamp", b"last_heartbeat_timestamp", "name", b"name", "origin", b"origin", "service_account", b"service_account", "type", b"type", "writeback_config", b"writeback_config"]) -> None: ...
         def WhichOneof(self, oneof_group: typing_extensions.Literal["info", b"info"]) -> typing_extensions.Literal["ecs"] | None: ...
 
     CLUSTERS_FIELD_NUMBER: builtins.int
     @property
     def clusters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ListClustersResp.ClusterInfo]: ...
     def __init__(
         self,
         *,
         clusters: collections.abc.Iterable[global___ListClustersResp.ClusterInfo] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["clusters", b"clusters"]) -> None: ...
 
 global___ListClustersResp = ListClustersResp
 
+class GetClusterReq(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    RUNTIME_FIELD_NUMBER: builtins.int
+    INCLUDE_AUTH_FIELD_NUMBER: builtins.int
+    runtime: builtins.str
+    """name or id"""
+    include_auth: builtins.bool
+    def __init__(
+        self,
+        *,
+        runtime: builtins.str = ...,
+        include_auth: builtins.bool = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["include_auth", b"include_auth", "runtime", b"runtime"]) -> None: ...
+
+global___GetClusterReq = GetClusterReq
+
+class GetClusterResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    CLUSTER_FIELD_NUMBER: builtins.int
+    @property
+    def cluster(self) -> global___ListClustersResp.ClusterInfo: ...
+    def __init__(
+        self,
+        *,
+        cluster: global___ListClustersResp.ClusterInfo | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["cluster", b"cluster"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cluster", b"cluster"]) -> None: ...
+
+global___GetClusterResp = GetClusterResp
+
 class ConfigureClusterReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RUNTIME_NAME_FIELD_NUMBER: builtins.int
     CONFIG_FIELD_NUMBER: builtins.int
     SOURCE_FIELD_NUMBER: builtins.int
     SOURCE_METADATA_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,24 +10,34 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
+        self.GetClusterAgentApiToken = channel.unary_unary(
+                '/prodvana.environment.EnvironmentManager/GetClusterAgentApiToken',
+                request_serializer=prodvana_dot_environment_dot_environment__manager__pb2.GetClusterAgentApiTokenReq.SerializeToString,
+                response_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.GetClusterAgentApiTokenResp.FromString,
+                )
         self.LinkCluster = channel.unary_unary(
                 '/prodvana.environment.EnvironmentManager/LinkCluster',
                 request_serializer=prodvana_dot_environment_dot_environment__manager__pb2.LinkClusterReq.SerializeToString,
                 response_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.LinkClusterResp.FromString,
                 )
         self.ListClusters = channel.unary_unary(
                 '/prodvana.environment.EnvironmentManager/ListClusters',
                 request_serializer=prodvana_dot_environment_dot_environment__manager__pb2.ListClustersReq.SerializeToString,
                 response_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.ListClustersResp.FromString,
                 )
+        self.GetCluster = channel.unary_unary(
+                '/prodvana.environment.EnvironmentManager/GetCluster',
+                request_serializer=prodvana_dot_environment_dot_environment__manager__pb2.GetClusterReq.SerializeToString,
+                response_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.GetClusterResp.FromString,
+                )
         self.RemoveCluster = channel.unary_unary(
                 '/prodvana.environment.EnvironmentManager/RemoveCluster',
                 request_serializer=prodvana_dot_environment_dot_environment__manager__pb2.RemoveClusterReq.SerializeToString,
                 response_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.RemoveClusterResp.FromString,
                 )
         self.GetClusterAuth = channel.unary_unary(
                 '/prodvana.environment.EnvironmentManager/GetClusterAuth',
@@ -60,34 +70,47 @@
                 response_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.GetClusterStatusResp.FromString,
                 )
 
 
 class EnvironmentManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
+    def GetClusterAgentApiToken(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def LinkCluster(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListClusters(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetCluster(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def RemoveCluster(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetClusterAuth(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Deprecated.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetClusterConfig(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -117,24 +140,34 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_EnvironmentManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
+            'GetClusterAgentApiToken': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetClusterAgentApiToken,
+                    request_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.GetClusterAgentApiTokenReq.FromString,
+                    response_serializer=prodvana_dot_environment_dot_environment__manager__pb2.GetClusterAgentApiTokenResp.SerializeToString,
+            ),
             'LinkCluster': grpc.unary_unary_rpc_method_handler(
                     servicer.LinkCluster,
                     request_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.LinkClusterReq.FromString,
                     response_serializer=prodvana_dot_environment_dot_environment__manager__pb2.LinkClusterResp.SerializeToString,
             ),
             'ListClusters': grpc.unary_unary_rpc_method_handler(
                     servicer.ListClusters,
                     request_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.ListClustersReq.FromString,
                     response_serializer=prodvana_dot_environment_dot_environment__manager__pb2.ListClustersResp.SerializeToString,
             ),
+            'GetCluster': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCluster,
+                    request_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.GetClusterReq.FromString,
+                    response_serializer=prodvana_dot_environment_dot_environment__manager__pb2.GetClusterResp.SerializeToString,
+            ),
             'RemoveCluster': grpc.unary_unary_rpc_method_handler(
                     servicer.RemoveCluster,
                     request_deserializer=prodvana_dot_environment_dot_environment__manager__pb2.RemoveClusterReq.FromString,
                     response_serializer=prodvana_dot_environment_dot_environment__manager__pb2.RemoveClusterResp.SerializeToString,
             ),
             'GetClusterAuth': grpc.unary_unary_rpc_method_handler(
                     servicer.GetClusterAuth,
@@ -173,14 +206,31 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class EnvironmentManager(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
+    def GetClusterAgentApiToken(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/prodvana.environment.EnvironmentManager/GetClusterAgentApiToken',
+            prodvana_dot_environment_dot_environment__manager__pb2.GetClusterAgentApiTokenReq.SerializeToString,
+            prodvana_dot_environment_dot_environment__manager__pb2.GetClusterAgentApiTokenResp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def LinkCluster(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -207,14 +257,31 @@
         return grpc.experimental.unary_unary(request, target, '/prodvana.environment.EnvironmentManager/ListClusters',
             prodvana_dot_environment_dot_environment__manager__pb2.ListClustersReq.SerializeToString,
             prodvana_dot_environment_dot_environment__manager__pb2.ListClustersResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetCluster(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/prodvana.environment.EnvironmentManager/GetCluster',
+            prodvana_dot_environment_dot_environment__manager__pb2.GetClusterReq.SerializeToString,
+            prodvana_dot_environment_dot_environment__manager__pb2.GetClusterResp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def RemoveCluster(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -4,30 +4,39 @@
 """
 import abc
 import grpc
 import prodvana.proto.prodvana.environment.environment_manager_pb2
 
 class EnvironmentManagerStub:
     def __init__(self, channel: grpc.Channel) -> None: ...
+    GetClusterAgentApiToken: grpc.UnaryUnaryMultiCallable[
+        prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterAgentApiTokenReq,
+        prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterAgentApiTokenResp,
+    ]
     LinkCluster: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.environment.environment_manager_pb2.LinkClusterReq,
         prodvana.proto.prodvana.environment.environment_manager_pb2.LinkClusterResp,
     ]
     ListClusters: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.environment.environment_manager_pb2.ListClustersReq,
         prodvana.proto.prodvana.environment.environment_manager_pb2.ListClustersResp,
     ]
+    GetCluster: grpc.UnaryUnaryMultiCallable[
+        prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterReq,
+        prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterResp,
+    ]
     RemoveCluster: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.environment.environment_manager_pb2.RemoveClusterReq,
         prodvana.proto.prodvana.environment.environment_manager_pb2.RemoveClusterResp,
     ]
     GetClusterAuth: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterAuthReq,
         prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterAuthResp,
     ]
+    """Deprecated."""
     GetClusterConfig: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterConfigReq,
         prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterConfigResp,
     ]
     DetectClusterConfig: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.environment.environment_manager_pb2.DetectClusterConfigReq,
         prodvana.proto.prodvana.environment.environment_manager_pb2.DetectClusterConfigResp,
@@ -43,37 +52,50 @@
     GetClusterStatus: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterStatusReq,
         prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterStatusResp,
     ]
 
 class EnvironmentManagerServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
+    def GetClusterAgentApiToken(
+        self,
+        request: prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterAgentApiTokenReq,
+        context: grpc.ServicerContext,
+    ) -> prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterAgentApiTokenResp: ...
+    @abc.abstractmethod
     def LinkCluster(
         self,
         request: prodvana.proto.prodvana.environment.environment_manager_pb2.LinkClusterReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.environment.environment_manager_pb2.LinkClusterResp: ...
     @abc.abstractmethod
     def ListClusters(
         self,
         request: prodvana.proto.prodvana.environment.environment_manager_pb2.ListClustersReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.environment.environment_manager_pb2.ListClustersResp: ...
     @abc.abstractmethod
+    def GetCluster(
+        self,
+        request: prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterReq,
+        context: grpc.ServicerContext,
+    ) -> prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterResp: ...
+    @abc.abstractmethod
     def RemoveCluster(
         self,
         request: prodvana.proto.prodvana.environment.environment_manager_pb2.RemoveClusterReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.environment.environment_manager_pb2.RemoveClusterResp: ...
     @abc.abstractmethod
     def GetClusterAuth(
         self,
         request: prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterAuthReq,
         context: grpc.ServicerContext,
-    ) -> prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterAuthResp: ...
+    ) -> prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterAuthResp:
+        """Deprecated."""
     @abc.abstractmethod
     def GetClusterConfig(
         self,
         request: prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterConfigReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.environment.environment_manager_pb2.GetClusterConfigResp: ...
     @abc.abstractmethod
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/events/events_manager.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.events import events_pb2 as prodvana_dot_events_dot_events__pb2
 from prodvana.proto.prodvana.events import types_pb2 as prodvana_dot_events_dot_types__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$prodvana/events/events_manager.proto\x12\x0fprodvana.events\x1a\x1cgoogle/api/annotations.proto\x1a\x17validate/validate.proto\x1a\x1cprodvana/events/events.proto\x1a\x1bprodvana/events/types.proto\"G\n\rServiceLookup\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"V\n\x14ReleaseChannelLookup\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12 \n\x0frelease_channel\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\xe0\x01\n\x06Lookup\x12\x1f\n\x15root_desired_state_id\x18\x01 \x01(\tH\x00\x12\x1a\n\x10\x64\x65sired_state_id\x18\x03 \x01(\tH\x00\x12\x31\n\x07service\x18\x04 \x01(\x0b\x32\x1e.prodvana.events.ServiceLookupH\x00\x12@\n\x0frelease_channel\x18\x05 \x01(\x0b\x32%.prodvana.events.ReleaseChannelLookupH\x00\x42\x13\n\x0clookup_oneof\x12\x03\xf8\x42\x01J\x04\x08\x02\x10\x03R\tentity_id\"\xe9\x01\n\x0cGetEventsReq\x12\x39\n\x07lookups\x18\x01 \x03(\x0b\x32\x17.prodvana.events.LookupB\x0f\xfa\x42\x0c\x92\x01\t\x08\x01\"\x05\x8a\x01\x02\x10\x01\x12)\n\x05types\x18\x02 \x03(\x0e\x32\x1a.prodvana.events.EventType\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x1e\n\x16order_by_asc_timestamp\x18\x06 \x01(\x08\x12\r\n\x05useOr\x18\x07 \x01(\x08J\x04\x08\x05\x10\x06R\x17order_by_desc_timestamp\"P\n\rGetEventsResp\x12&\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x16.prodvana.events.Event\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t2r\n\rEventsManager\x12\x61\n\tGetEvents\x12\x1d.prodvana.events.GetEventsReq\x1a\x1e.prodvana.events.GetEventsResp\"\x15\x82\xd3\xe4\x93\x02\x0f\"\n/v1/events:\x01*BKZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/eventsb\x06proto3')
 
-
-
-_SERVICELOOKUP = DESCRIPTOR.message_types_by_name['ServiceLookup']
-_RELEASECHANNELLOOKUP = DESCRIPTOR.message_types_by_name['ReleaseChannelLookup']
-_LOOKUP = DESCRIPTOR.message_types_by_name['Lookup']
-_GETEVENTSREQ = DESCRIPTOR.message_types_by_name['GetEventsReq']
-_GETEVENTSRESP = DESCRIPTOR.message_types_by_name['GetEventsResp']
-ServiceLookup = _reflection.GeneratedProtocolMessageType('ServiceLookup', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICELOOKUP,
-  '__module__' : 'prodvana.events.events_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.events.ServiceLookup)
-  })
-_sym_db.RegisterMessage(ServiceLookup)
-
-ReleaseChannelLookup = _reflection.GeneratedProtocolMessageType('ReleaseChannelLookup', (_message.Message,), {
-  'DESCRIPTOR' : _RELEASECHANNELLOOKUP,
-  '__module__' : 'prodvana.events.events_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.events.ReleaseChannelLookup)
-  })
-_sym_db.RegisterMessage(ReleaseChannelLookup)
-
-Lookup = _reflection.GeneratedProtocolMessageType('Lookup', (_message.Message,), {
-  'DESCRIPTOR' : _LOOKUP,
-  '__module__' : 'prodvana.events.events_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.events.Lookup)
-  })
-_sym_db.RegisterMessage(Lookup)
-
-GetEventsReq = _reflection.GeneratedProtocolMessageType('GetEventsReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETEVENTSREQ,
-  '__module__' : 'prodvana.events.events_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.events.GetEventsReq)
-  })
-_sym_db.RegisterMessage(GetEventsReq)
-
-GetEventsResp = _reflection.GeneratedProtocolMessageType('GetEventsResp', (_message.Message,), {
-  'DESCRIPTOR' : _GETEVENTSRESP,
-  '__module__' : 'prodvana.events.events_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.events.GetEventsResp)
-  })
-_sym_db.RegisterMessage(GetEventsResp)
-
-_EVENTSMANAGER = DESCRIPTOR.services_by_name['EventsManager']
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.events.events_manager_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/events'
   _SERVICELOOKUP.fields_by_name['application']._options = None
   _SERVICELOOKUP.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
   _SERVICELOOKUP.fields_by_name['service']._options = None
@@ -77,20 +36,20 @@
   _RELEASECHANNELLOOKUP.fields_by_name['release_channel']._serialized_options = b'\372B\004r\002\020\001'
   _LOOKUP.oneofs_by_name['lookup_oneof']._options = None
   _LOOKUP.oneofs_by_name['lookup_oneof']._serialized_options = b'\370B\001'
   _GETEVENTSREQ.fields_by_name['lookups']._options = None
   _GETEVENTSREQ.fields_by_name['lookups']._serialized_options = b'\372B\014\222\001\t\010\001\"\005\212\001\002\020\001'
   _EVENTSMANAGER.methods_by_name['GetEvents']._options = None
   _EVENTSMANAGER.methods_by_name['GetEvents']._serialized_options = b'\202\323\344\223\002\017\"\n/v1/events:\001*'
-  _SERVICELOOKUP._serialized_start=171
-  _SERVICELOOKUP._serialized_end=242
-  _RELEASECHANNELLOOKUP._serialized_start=244
-  _RELEASECHANNELLOOKUP._serialized_end=330
-  _LOOKUP._serialized_start=333
-  _LOOKUP._serialized_end=557
-  _GETEVENTSREQ._serialized_start=560
-  _GETEVENTSREQ._serialized_end=793
-  _GETEVENTSRESP._serialized_start=795
-  _GETEVENTSRESP._serialized_end=875
-  _EVENTSMANAGER._serialized_start=877
-  _EVENTSMANAGER._serialized_end=991
+  _globals['_SERVICELOOKUP']._serialized_start=171
+  _globals['_SERVICELOOKUP']._serialized_end=242
+  _globals['_RELEASECHANNELLOOKUP']._serialized_start=244
+  _globals['_RELEASECHANNELLOOKUP']._serialized_end=330
+  _globals['_LOOKUP']._serialized_start=333
+  _globals['_LOOKUP']._serialized_end=557
+  _globals['_GETEVENTSREQ']._serialized_start=560
+  _globals['_GETEVENTSREQ']._serialized_end=793
+  _globals['_GETEVENTSRESP']._serialized_start=795
+  _globals['_GETEVENTSRESP']._serialized_end=875
+  _globals['_EVENTSMANAGER']._serialized_start=877
+  _globals['_EVENTSMANAGER']._serialized_end=991
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/events/events.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from prodvana.proto.prodvana.events import types_pb2 as prodvana_dot_events_dot_types__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cprodvana/events/events.proto\x12\x0fprodvana.events\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bprodvana/events/types.proto\"\xe5\x01\n\x05\x45vent\x12\n\n\x02id\x18\x01 \x01(\t\x12(\n\x04type\x18\x02 \x01(\x0e\x32\x1a.prodvana.events.EventType\x12\r\n\x05title\x18\x03 \x01(\t\x12.\n\x07\x64\x65tails\x18\x04 \x01(\x0b\x32\x1d.prodvana.events.EventDetails\x12-\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x0frelated_objects\x18\x06 \x01(\x0b\x32\x1f.prodvana.events.RelatedObjects\"\xa4\x02\n\x0eRelatedObjects\x12\x16\n\x0e\x61pplication_id\x18\x01 \x01(\t\x12\x12\n\nservice_id\x18\x02 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x03 \x01(\t\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x12\n\nruntime_id\x18\x06 \x01(\t\x12H\n\rexternal_logs\x18\x07 \x03(\x0b\x32\x31.prodvana.events.RelatedObjects.ExternalLogsEntry\x1a\x33\n\x11\x45xternalLogsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42KZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/eventsb\x06proto3')
 
-
-
-_EVENT = DESCRIPTOR.message_types_by_name['Event']
-_RELATEDOBJECTS = DESCRIPTOR.message_types_by_name['RelatedObjects']
-_RELATEDOBJECTS_EXTERNALLOGSENTRY = _RELATEDOBJECTS.nested_types_by_name['ExternalLogsEntry']
-Event = _reflection.GeneratedProtocolMessageType('Event', (_message.Message,), {
-  'DESCRIPTOR' : _EVENT,
-  '__module__' : 'prodvana.events.events_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.events.Event)
-  })
-_sym_db.RegisterMessage(Event)
-
-RelatedObjects = _reflection.GeneratedProtocolMessageType('RelatedObjects', (_message.Message,), {
-
-  'ExternalLogsEntry' : _reflection.GeneratedProtocolMessageType('ExternalLogsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _RELATEDOBJECTS_EXTERNALLOGSENTRY,
-    '__module__' : 'prodvana.events.events_pb2'
-    # @@protoc_insertion_point(class_scope:prodvana.events.RelatedObjects.ExternalLogsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _RELATEDOBJECTS,
-  '__module__' : 'prodvana.events.events_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.events.RelatedObjects)
-  })
-_sym_db.RegisterMessage(RelatedObjects)
-_sym_db.RegisterMessage(RelatedObjects.ExternalLogsEntry)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.events.events_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/events'
   _RELATEDOBJECTS_EXTERNALLOGSENTRY._options = None
   _RELATEDOBJECTS_EXTERNALLOGSENTRY._serialized_options = b'8\001'
-  _EVENT._serialized_start=112
-  _EVENT._serialized_end=341
-  _RELATEDOBJECTS._serialized_start=344
-  _RELATEDOBJECTS._serialized_end=636
-  _RELATEDOBJECTS_EXTERNALLOGSENTRY._serialized_start=585
-  _RELATEDOBJECTS_EXTERNALLOGSENTRY._serialized_end=636
+  _globals['_EVENT']._serialized_start=112
+  _globals['_EVENT']._serialized_end=341
+  _globals['_RELATEDOBJECTS']._serialized_start=344
+  _globals['_RELATEDOBJECTS']._serialized_end=636
+  _globals['_RELATEDOBJECTS_EXTERNALLOGSENTRY']._serialized_start=585
+  _globals['_RELATEDOBJECTS_EXTERNALLOGSENTRY']._serialized_end=636
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/insights/insights.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n prodvana/insights/insights.proto\x12\x11prodvana.insights\"\xba\x02\n\x07Insight\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\'\n\x05\x63lass\x18\x06 \x01(\x0e\x32\x18.prodvana.insights.Class\x12\x35\n\x07service\x18\x03 \x01(\x0b\x32\".prodvana.insights.Insight.SubjectH\x00\x12\x39\n\x0b\x61pplication\x18\x04 \x01(\x0b\x32\".prodvana.insights.Insight.SubjectH\x00\x12:\n\x0corganization\x18\x05 \x01(\x0b\x32\".prodvana.insights.Insight.SubjectH\x00\x1a#\n\x07Subject\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\tB\x0f\n\rsubject_oneof*\xce\x01\n\x05\x43lass\x12\x0b\n\x07UNKNOWN\x10\x00\x12,\n(SUCCESSFUL_DEPLOYMENT_FREQUENCY_DECREASE\x10\x01\x12$\n DEPLOYMENT_FAILURE_RATE_INCREASE\x10\x02\x12\x32\n.MEDIAN_SUCCESSFUL_DEPLOYMENT_DURATION_INCREASE\x10\x03\x12\x30\n,MEDIAN_SUCCESSFUL_ROLLBACK_DURATION_INCREASE\x10\x04\x42MZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/insightsb\x06proto3')
 
-_CLASS = DESCRIPTOR.enum_types_by_name['Class']
-Class = enum_type_wrapper.EnumTypeWrapper(_CLASS)
-UNKNOWN = 0
-SUCCESSFUL_DEPLOYMENT_FREQUENCY_DECREASE = 1
-DEPLOYMENT_FAILURE_RATE_INCREASE = 2
-MEDIAN_SUCCESSFUL_DEPLOYMENT_DURATION_INCREASE = 3
-MEDIAN_SUCCESSFUL_ROLLBACK_DURATION_INCREASE = 4
-
-
-_INSIGHT = DESCRIPTOR.message_types_by_name['Insight']
-_INSIGHT_SUBJECT = _INSIGHT.nested_types_by_name['Subject']
-Insight = _reflection.GeneratedProtocolMessageType('Insight', (_message.Message,), {
-
-  'Subject' : _reflection.GeneratedProtocolMessageType('Subject', (_message.Message,), {
-    'DESCRIPTOR' : _INSIGHT_SUBJECT,
-    '__module__' : 'prodvana.insights.insights_pb2'
-    # @@protoc_insertion_point(class_scope:prodvana.insights.Insight.Subject)
-    })
-  ,
-  'DESCRIPTOR' : _INSIGHT,
-  '__module__' : 'prodvana.insights.insights_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.insights.Insight)
-  })
-_sym_db.RegisterMessage(Insight)
-_sym_db.RegisterMessage(Insight.Subject)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.insights.insights_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/insights'
-  _CLASS._serialized_start=373
-  _CLASS._serialized_end=579
-  _INSIGHT._serialized_start=56
-  _INSIGHT._serialized_end=370
-  _INSIGHT_SUBJECT._serialized_start=318
-  _INSIGHT_SUBJECT._serialized_end=353
+  _globals['_CLASS']._serialized_start=373
+  _globals['_CLASS']._serialized_end=579
+  _globals['_INSIGHT']._serialized_start=56
+  _globals['_INSIGHT']._serialized_end=370
+  _globals['_INSIGHT_SUBJECT']._serialized_start=318
+  _globals['_INSIGHT_SUBJECT']._serialized_end=353
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/object/meta.proto
+# source: prodvana/pipelines/object.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from prodvana.proto.prodvana.version import source_metadata_pb2 as prodvana_dot_version_dot_source__metadata__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from prodvana.proto.prodvana.common_config import meta_pb2 as prodvana_dot_common__config_dot_meta__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aprodvana/object/meta.proto\x12\x0fprodvana.object\x1a&prodvana/version/source_metadata.proto\"\xb4\x01\n\nObjectMeta\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x16\n\x0e\x63onfig_version\x18\x04 \x01(\t\x12(\n\x06source\x18\x05 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x06 \x01(\x0b\x32 .prodvana.version.SourceMetadataBKZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/objectb\x06proto3')
-
-
-
-_OBJECTMETA = DESCRIPTOR.message_types_by_name['ObjectMeta']
-ObjectMeta = _reflection.GeneratedProtocolMessageType('ObjectMeta', (_message.Message,), {
-  'DESCRIPTOR' : _OBJECTMETA,
-  '__module__' : 'prodvana.object.meta_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.object.ObjectMeta)
-  })
-_sym_db.RegisterMessage(ObjectMeta)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fprodvana/pipelines/object.proto\x12\x12prodvana.pipelines\x1a\x1fgoogle/protobuf/timestamp.proto\x1a!prodvana/common_config/meta.proto\"\xa6\x01\n\x10PipelineRunState\x12\x36\n\x12\x63reation_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05state\x18\x03 \x01(\t\x12\x10\n\x08terminal\x18\x04 \x01(\x08\"\x7f\n\x0bPipelineRun\x12;\n\x04meta\x18\x01 \x01(\x0b\x32-.prodvana.common_config.PipelineRunObjectMeta\x12\x33\n\x05state\x18\x03 \x01(\x0b\x32$.prodvana.pipelines.PipelineRunStateBNZLgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/pipelinesb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.pipelines.object_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/object'
-  _OBJECTMETA._serialized_start=88
-  _OBJECTMETA._serialized_end=268
+  DESCRIPTOR._serialized_options = b'ZLgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/pipelines'
+  _globals['_PIPELINERUNSTATE']._serialized_start=124
+  _globals['_PIPELINERUNSTATE']._serialized_end=290
+  _globals['_PIPELINERUN']._serialized_start=292
+  _globals['_PIPELINERUN']._serialized_end=419
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,55 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
+import google.protobuf.internal.containers
 import google.protobuf.message
-import google.protobuf.timestamp_pb2
-import prodvana.proto.prodvana.common_config.meta_pb2
+import prodvana.proto.prodvana.common_config.links_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class PipelineRunState(google.protobuf.message.Message):
+class ServiceUserMetadata(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CREATION_TIMESTAMP_FIELD_NUMBER: builtins.int
-    LAST_UPDATE_TIMESTAMP_FIELD_NUMBER: builtins.int
-    STATE_FIELD_NUMBER: builtins.int
-    TERMINAL_FIELD_NUMBER: builtins.int
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    LINKS_FIELD_NUMBER: builtins.int
+    FOLLOW_REPOSITORY_FIELD_NUMBER: builtins.int
+    description: builtins.str
     @property
-    def creation_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    def links(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.links_pb2.Link]: ...
     @property
-    def last_update_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    state: builtins.str
-    terminal: builtins.bool
-    """if pipeline run is in a terminal state"""
+    def follow_repository(self) -> global___FollowContainerRepositorySettings: ...
     def __init__(
         self,
         *,
-        creation_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        last_update_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        state: builtins.str = ...,
-        terminal: builtins.bool = ...,
+        description: builtins.str = ...,
+        links: collections.abc.Iterable[prodvana.proto.prodvana.common_config.links_pb2.Link] | None = ...,
+        follow_repository: global___FollowContainerRepositorySettings | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "last_update_timestamp", b"last_update_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "last_update_timestamp", b"last_update_timestamp", "state", b"state", "terminal", b"terminal"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["follow_repository", b"follow_repository"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "follow_repository", b"follow_repository", "links", b"links"]) -> None: ...
 
-global___PipelineRunState = PipelineRunState
+global___ServiceUserMetadata = ServiceUserMetadata
 
-class PipelineRun(google.protobuf.message.Message):
+class FollowContainerRepositorySettings(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    META_FIELD_NUMBER: builtins.int
-    STATE_FIELD_NUMBER: builtins.int
-    @property
-    def meta(self) -> prodvana.proto.prodvana.common_config.meta_pb2.PipelineRunObjectMeta: ...
-    @property
-    def state(self) -> global___PipelineRunState: ...
+    ENABLED_FIELD_NUMBER: builtins.int
+    enabled: builtins.bool
     def __init__(
         self,
         *,
-        meta: prodvana.proto.prodvana.common_config.meta_pb2.PipelineRunObjectMeta | None = ...,
-        state: global___PipelineRunState | None = ...,
+        enabled: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["meta", b"meta", "state", b"state"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["meta", b"meta", "state", b"state"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["enabled", b"enabled"]) -> None: ...
 
-global___PipelineRun = PipelineRun
+global___FollowContainerRepositorySettings = FollowContainerRepositorySettings
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -34,34 +34,33 @@
 
 UNKNOWN: AttachmentType.ValueType  # 0
 RELEASE_CHANNEL: AttachmentType.ValueType  # 1
 SERVICE_INSTANCE: AttachmentType.ValueType  # 2
 CONVERGENCE: AttachmentType.ValueType  # 3
 global___AttachmentType = AttachmentType
 
-class ProtectionConvergenceAttachment(google.protobuf.message.Message):
-    """Protections attached to convergence. The desired state ID of the convergence is passed to the protection
-    and its lifecycle is tied to the convergence itself.
-    """
-
+class ProtectionAttachmentConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     REF_FIELD_NUMBER: builtins.int
     LIFECYCLE_FIELD_NUMBER: builtins.int
     name: builtins.str
     """optional, default to protection name"""
     @property
     def ref(self) -> prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionReference: ...
     @property
-    def lifecycle(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionLifecycle]: ...
+    def lifecycle(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionLifecycle]:
+        """if set, the attachment is automatically used in all deployments for the subject of this attachment.
+        e.g. for release channels, all service instances in that release channel will use the attachment.
+        """
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         ref: prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionReference | None = ...,
         lifecycle: collections.abc.Iterable[prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionLifecycle] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["ref", b"ref"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["lifecycle", b"lifecycle", "name", b"name", "ref", b"ref"]) -> None: ...
 
-global___ProtectionConvergenceAttachment = ProtectionConvergenceAttachment
+global___ProtectionAttachmentConfig = ProtectionAttachmentConfig
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/protection/object.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.object import meta_pb2 as prodvana_dot_object_dot_meta__pb2
 from prodvana.proto.prodvana.protection import protection_config_pb2 as prodvana_dot_protection_dot_protection__config__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n prodvana/protection/object.proto\x12\x13prodvana.protection\x1a\x1aprodvana/object/meta.proto\x1a+prodvana/protection/protection_config.proto\"\x7f\n\nProtection\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x35\n\x06\x63onfig\x18\x02 \x01(\x0b\x32%.prodvana.protection.ProtectionConfig\x12\x0f\n\x07\x62uiltin\x18\x03 \x01(\x08\x42OZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protectionb\x06proto3')
 
-
-
-_PROTECTION = DESCRIPTOR.message_types_by_name['Protection']
-Protection = _reflection.GeneratedProtocolMessageType('Protection', (_message.Message,), {
-  'DESCRIPTOR' : _PROTECTION,
-  '__module__' : 'prodvana.protection.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.protection.Protection)
-  })
-_sym_db.RegisterMessage(Protection)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.protection.object_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protection'
-  _PROTECTION._serialized_start=130
-  _PROTECTION._serialized_end=257
+  _globals['_PROTECTION']._serialized_start=130
+  _globals['_PROTECTION']._serialized_end=257
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -21,20 +21,38 @@
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class ProtectionConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    class EnvEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> prodvana.proto.prodvana.common_config.env_pb2.EnvValue: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: prodvana.proto.prodvana.common_config.env_pb2.EnvValue | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     NAME_FIELD_NUMBER: builtins.int
     TASK_CONFIG_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     POLL_INTERVAL_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
+    ENV_FIELD_NUMBER: builtins.int
     name: builtins.str
     @property
     def task_config(self) -> prodvana.proto.prodvana.common_config.task_pb2.TaskConfig:
         """Inline task config with retry, template support."""
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
@@ -43,26 +61,30 @@
         how often to run check even if it succeeds
         """
     @property
     def timeout(self) -> google.protobuf.duration_pb2.Duration:
         """how long after a run has started to try another run if it has not completed yet"""
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
+    @property
+    def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
+        """optional env variables to inject and override from exec_config"""
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         task_config: prodvana.proto.prodvana.common_config.task_pb2.TaskConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         poll_interval: google.protobuf.duration_pb2.Duration | None = ...,
         timeout: google.protobuf.duration_pb2.Duration | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
+        env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameters", b"parameters", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["env", b"env", "exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameters", b"parameters", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["exec_config", b"exec_config"]) -> typing_extensions.Literal["task_config", "kubernetes_config"] | None: ...
 
 global___ProtectionConfig = ProtectionConfig
 
 class CompiledProtectionAttachmentConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -3,169 +3,169 @@
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import prodvana.proto.prodvana.protection.object_pb2
-import prodvana.proto.prodvana.protection.protection_config_pb2
-import prodvana.proto.prodvana.version.source_metadata_pb2
+import prodvana.proto.prodvana.users.users_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class ConfigureProtectionReq(google.protobuf.message.Message):
+class SettingsUser(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PROTECTION_CONFIG_FIELD_NUMBER: builtins.int
-    SOURCE_FIELD_NUMBER: builtins.int
-    SOURCE_METADATA_FIELD_NUMBER: builtins.int
+    USER_FIELD_NUMBER: builtins.int
+    ROLES_FIELD_NUMBER: builtins.int
     @property
-    def protection_config(self) -> prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig: ...
-    source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType
+    def user(self) -> prodvana.proto.prodvana.users.users_pb2.User: ...
     @property
-    def source_metadata(self) -> prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata: ...
+    def roles(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
-        protection_config: prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig | None = ...,
-        source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType = ...,
-        source_metadata: prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata | None = ...,
+        user: prodvana.proto.prodvana.users.users_pb2.User | None = ...,
+        roles: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["protection_config", b"protection_config", "source_metadata", b"source_metadata"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["protection_config", b"protection_config", "source", b"source", "source_metadata", b"source_metadata"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user", b"user"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["roles", b"roles", "user", b"user"]) -> None: ...
 
-global___ConfigureProtectionReq = ConfigureProtectionReq
+global___SettingsUser = SettingsUser
 
-class ConfigureProtectionResp(google.protobuf.message.Message):
+class GetUserReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PROTECTION_ID_FIELD_NUMBER: builtins.int
-    VERSION_FIELD_NUMBER: builtins.int
-    protection_id: builtins.str
-    version: builtins.str
+    USER_ID_FIELD_NUMBER: builtins.int
+    user_id: builtins.str
     def __init__(
         self,
         *,
-        protection_id: builtins.str = ...,
-        version: builtins.str = ...,
+        user_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["protection_id", b"protection_id", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["user_id", b"user_id"]) -> None: ...
 
-global___ConfigureProtectionResp = ConfigureProtectionResp
+global___GetUserReq = GetUserReq
 
-class ValidateConfigureProtectionResp(google.protobuf.message.Message):
+class GetUserResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    USER_FIELD_NUMBER: builtins.int
+    @property
+    def user(self) -> global___SettingsUser: ...
     def __init__(
         self,
+        *,
+        user: global___SettingsUser | None = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user", b"user"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["user", b"user"]) -> None: ...
 
-global___ValidateConfigureProtectionResp = ValidateConfigureProtectionResp
+global___GetUserResp = GetUserResp
 
-class ListProtectionsReq(google.protobuf.message.Message):
+class ListRolesReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PAGE_TOKEN_FIELD_NUMBER: builtins.int
-    PAGE_SIZE_FIELD_NUMBER: builtins.int
-    page_token: builtins.str
-    page_size: builtins.int
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___ListRolesReq = ListRolesReq
+
+class RoleDefinition(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    NAME_FIELD_NUMBER: builtins.int
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    name: builtins.str
+    description: builtins.str
     def __init__(
         self,
         *,
-        page_token: builtins.str = ...,
-        page_size: builtins.int = ...,
+        name: builtins.str = ...,
+        description: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["page_size", b"page_size", "page_token", b"page_token"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "name", b"name"]) -> None: ...
 
-global___ListProtectionsReq = ListProtectionsReq
+global___RoleDefinition = RoleDefinition
 
-class ListProtectionsResp(google.protobuf.message.Message):
+class ListRolesResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PROTECTIONS_FIELD_NUMBER: builtins.int
-    NEXT_PAGE_TOKEN_FIELD_NUMBER: builtins.int
+    ROLES_FIELD_NUMBER: builtins.int
     @property
-    def protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.object_pb2.Protection]: ...
-    next_page_token: builtins.str
+    def roles(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RoleDefinition]: ...
     def __init__(
         self,
         *,
-        protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.object_pb2.Protection] | None = ...,
-        next_page_token: builtins.str = ...,
+        roles: collections.abc.Iterable[global___RoleDefinition] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["next_page_token", b"next_page_token", "protections", b"protections"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["roles", b"roles"]) -> None: ...
 
-global___ListProtectionsResp = ListProtectionsResp
+global___ListRolesResp = ListRolesResp
 
-class GetProtectionReq(google.protobuf.message.Message):
+class ListUsersReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PROTECTION_FIELD_NUMBER: builtins.int
-    protection: builtins.str
+    PAGE_TOKEN_FIELD_NUMBER: builtins.int
+    PAGE_SIZE_FIELD_NUMBER: builtins.int
+    page_token: builtins.str
+    page_size: builtins.int
     def __init__(
         self,
         *,
-        protection: builtins.str = ...,
+        page_token: builtins.str = ...,
+        page_size: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["protection", b"protection"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["page_size", b"page_size", "page_token", b"page_token"]) -> None: ...
 
-global___GetProtectionReq = GetProtectionReq
+global___ListUsersReq = ListUsersReq
 
-class GetProtectionResp(google.protobuf.message.Message):
+class ListUsersResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PROTECTION_FIELD_NUMBER: builtins.int
+    USERS_FIELD_NUMBER: builtins.int
+    NEXT_PAGE_TOKEN_FIELD_NUMBER: builtins.int
     @property
-    def protection(self) -> prodvana.proto.prodvana.protection.object_pb2.Protection: ...
+    def users(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SettingsUser]: ...
+    next_page_token: builtins.str
     def __init__(
         self,
         *,
-        protection: prodvana.proto.prodvana.protection.object_pb2.Protection | None = ...,
+        users: collections.abc.Iterable[global___SettingsUser] | None = ...,
+        next_page_token: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["protection", b"protection"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["protection", b"protection"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["next_page_token", b"next_page_token", "users", b"users"]) -> None: ...
 
-global___GetProtectionResp = GetProtectionResp
+global___ListUsersResp = ListUsersResp
 
-class GetProtectionConfigReq(google.protobuf.message.Message):
+class SetRolesReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PROTECTION_FIELD_NUMBER: builtins.int
-    VERSION_FIELD_NUMBER: builtins.int
-    protection: builtins.str
-    version: builtins.str
-    """omit to get latest version"""
+    USER_ID_FIELD_NUMBER: builtins.int
+    ROLES_FIELD_NUMBER: builtins.int
+    user_id: builtins.str
+    @property
+    def roles(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
-        protection: builtins.str = ...,
-        version: builtins.str = ...,
+        user_id: builtins.str = ...,
+        roles: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["protection", b"protection", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["roles", b"roles", "user_id", b"user_id"]) -> None: ...
 
-global___GetProtectionConfigReq = GetProtectionConfigReq
+global___SetRolesReq = SetRolesReq
 
-class GetProtectionConfigResp(google.protobuf.message.Message):
+class SetRolesResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CONFIG_FIELD_NUMBER: builtins.int
-    VERSION_FIELD_NUMBER: builtins.int
-    @property
-    def config(self) -> prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig: ...
-    version: builtins.str
     def __init__(
         self,
-        *,
-        config: prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig | None = ...,
-        version: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["config", b"config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "version", b"version"]) -> None: ...
 
-global___GetProtectionConfigResp = GetProtectionConfigResp
+global___SetRolesResp = SetRolesResp
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,19 @@
                 response_deserializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionResp.FromString,
                 )
         self.GetProtectionConfig = channel.unary_unary(
                 '/prodvana.protection.ProtectionManager/GetProtectionConfig',
                 request_serializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionConfigReq.SerializeToString,
                 response_deserializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionConfigResp.FromString,
                 )
+        self.GetProtectionAttachmentConfig = channel.unary_unary(
+                '/prodvana.protection.ProtectionManager/GetProtectionAttachmentConfig',
+                request_serializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionAttachmentConfigReq.SerializeToString,
+                response_deserializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionAttachmentConfigResp.FromString,
+                )
 
 
 class ProtectionManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ConfigureProtection(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -70,14 +75,20 @@
 
     def GetProtectionConfig(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetProtectionAttachmentConfig(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_ProtectionManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ConfigureProtection': grpc.unary_unary_rpc_method_handler(
                     servicer.ConfigureProtection,
                     request_deserializer=prodvana_dot_protection_dot_protection__manager__pb2.ConfigureProtectionReq.FromString,
                     response_serializer=prodvana_dot_protection_dot_protection__manager__pb2.ConfigureProtectionResp.SerializeToString,
@@ -98,14 +109,19 @@
                     response_serializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionResp.SerializeToString,
             ),
             'GetProtectionConfig': grpc.unary_unary_rpc_method_handler(
                     servicer.GetProtectionConfig,
                     request_deserializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionConfigReq.FromString,
                     response_serializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionConfigResp.SerializeToString,
             ),
+            'GetProtectionAttachmentConfig': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetProtectionAttachmentConfig,
+                    request_deserializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionAttachmentConfigReq.FromString,
+                    response_serializer=prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionAttachmentConfigResp.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'prodvana.protection.ProtectionManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -192,7 +208,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/prodvana.protection.ProtectionManager/GetProtectionConfig',
             prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionConfigReq.SerializeToString,
             prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionConfigResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetProtectionAttachmentConfig(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/prodvana.protection.ProtectionManager/GetProtectionAttachmentConfig',
+            prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionAttachmentConfigReq.SerializeToString,
+            prodvana_dot_protection_dot_protection__manager__pb2.GetProtectionAttachmentConfigResp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionReq,
         prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionResp,
     ]
     GetProtectionConfig: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionConfigReq,
         prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionConfigResp,
     ]
+    GetProtectionAttachmentConfig: grpc.UnaryUnaryMultiCallable[
+        prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionAttachmentConfigReq,
+        prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionAttachmentConfigResp,
+    ]
 
 class ProtectionManagerServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def ConfigureProtection(
         self,
         request: prodvana.proto.prodvana.protection.protection_manager_pb2.ConfigureProtectionReq,
         context: grpc.ServicerContext,
@@ -56,9 +60,15 @@
     ) -> prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionResp: ...
     @abc.abstractmethod
     def GetProtectionConfig(
         self,
         request: prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionConfigReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionConfigResp: ...
+    @abc.abstractmethod
+    def GetProtectionAttachmentConfig(
+        self,
+        request: prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionAttachmentConfigReq,
+        context: grpc.ServicerContext,
+    ) -> prodvana.proto.prodvana.protection.protection_manager_pb2.GetProtectionAttachmentConfigResp: ...
 
 def add_ProtectionManagerServicer_to_server(servicer: ProtectionManagerServicer, server: grpc.Server) -> None: ...
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import prodvana.proto.prodvana.common_config.constants_pb2
 import prodvana.proto.prodvana.common_config.env_pb2
 import prodvana.proto.prodvana.common_config.maturity_pb2
 import prodvana.proto.prodvana.pipelines.pipelines_pb2
 import prodvana.proto.prodvana.protection.attachments_pb2
-import prodvana.proto.prodvana.protection.protection_reference_pb2
 import prodvana.proto.prodvana.runtimes.runtimes_config_pb2
 import prodvana.proto.prodvana.workflow.integration_config_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
@@ -83,74 +83,59 @@
     MATURITY_FIELD_NUMBER: builtins.int
     POLICY_FIELD_NUMBER: builtins.int
     RUNTIMES_FIELD_NUMBER: builtins.int
     DEPLOY_ANNOTATIONS_FIELD_NUMBER: builtins.int
     PRECONDITIONS_FIELD_NUMBER: builtins.int
     PROTECTIONS_FIELD_NUMBER: builtins.int
     CONVERGENCE_PROTECTIONS_FIELD_NUMBER: builtins.int
+    SERVICE_INSTANCE_PROTECTIONS_FIELD_NUMBER: builtins.int
+    CONSTANTS_FIELD_NUMBER: builtins.int
     name: builtins.str
     """intentionally does not reference cluster - this allows us to copy release channels across clusters via the same config"""
     order: builtins.int
     maturity: prodvana.proto.prodvana.common_config.maturity_pb2.Maturity.ValueType
     """deprecated"""
     @property
     def policy(self) -> global___Policy: ...
     @property
     def runtimes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ReleaseChannelRuntimeConfig]: ...
     @property
     def deploy_annotations(self) -> prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig: ...
     @property
     def preconditions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Precondition]: ...
     @property
-    def protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ProtectionReleaseChannelAttachment]: ...
+    def protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]: ...
     @property
-    def convergence_protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionConvergenceAttachment]: ...
+    def convergence_protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]: ...
+    @property
+    def service_instance_protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]:
+        """protections that all service instances in this release channel should get"""
+    @property
+    def constants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.constants_pb2.Constant]:
+        """constants made available in template substitutions"""
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         order: builtins.int = ...,
         maturity: prodvana.proto.prodvana.common_config.maturity_pb2.Maturity.ValueType = ...,
         policy: global___Policy | None = ...,
         runtimes: collections.abc.Iterable[global___ReleaseChannelRuntimeConfig] | None = ...,
         deploy_annotations: prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig | None = ...,
         preconditions: collections.abc.Iterable[global___Precondition] | None = ...,
-        protections: collections.abc.Iterable[global___ProtectionReleaseChannelAttachment] | None = ...,
-        convergence_protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionConvergenceAttachment] | None = ...,
+        protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
+        convergence_protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
+        service_instance_protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
+        constants: collections.abc.Iterable[prodvana.proto.prodvana.common_config.constants_pb2.Constant] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["deploy_annotations", b"deploy_annotations", "policy", b"policy"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["convergence_protections", b"convergence_protections", "deploy_annotations", b"deploy_annotations", "maturity", b"maturity", "name", b"name", "order", b"order", "policy", b"policy", "preconditions", b"preconditions", "protections", b"protections", "runtimes", b"runtimes"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["constants", b"constants", "convergence_protections", b"convergence_protections", "deploy_annotations", b"deploy_annotations", "maturity", b"maturity", "name", b"name", "order", b"order", "policy", b"policy", "preconditions", b"preconditions", "protections", b"protections", "runtimes", b"runtimes", "service_instance_protections", b"service_instance_protections"]) -> None: ...
 
 global___ReleaseChannelConfig = ReleaseChannelConfig
 
-class ProtectionReleaseChannelAttachment(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    NAME_FIELD_NUMBER: builtins.int
-    REF_FIELD_NUMBER: builtins.int
-    LIFECYCLE_FIELD_NUMBER: builtins.int
-    name: builtins.str
-    """optional, default to protection name"""
-    @property
-    def ref(self) -> prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionReference: ...
-    @property
-    def lifecycle(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionLifecycle]:
-        """if set, this protection is automatically used as part of service pushes in this release channel"""
-    def __init__(
-        self,
-        *,
-        name: builtins.str = ...,
-        ref: prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionReference | None = ...,
-        lifecycle: collections.abc.Iterable[prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionLifecycle] | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["ref", b"ref"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["lifecycle", b"lifecycle", "name", b"name", "ref", b"ref"]) -> None: ...
-
-global___ProtectionReleaseChannelAttachment = ProtectionReleaseChannelAttachment
-
 class Precondition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class ReleaseChannelStable(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         RELEASE_CHANNEL_FIELD_NUMBER: builtins.int
@@ -166,17 +151,25 @@
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration", "release_channel", b"release_channel"]) -> None: ...
 
     class ManualApproval(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+        NAME_FIELD_NUMBER: builtins.int
+        DESCRIPTION_FIELD_NUMBER: builtins.int
+        name: builtins.str
+        description: builtins.str
         def __init__(
             self,
+            *,
+            name: builtins.str = ...,
+            description: builtins.str = ...,
         ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "name", b"name"]) -> None: ...
 
     class CustomTask(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TASK_NAME_FIELD_NUMBER: builtins.int
         CUSTOM_TASK_FIELD_NUMBER: builtins.int
         task_name: builtins.str
@@ -225,14 +218,15 @@
     """Optional identifier for this runtime connection within this release channel,
     useful if the release channel has multiple runtimes of the same type.
     Defaults to the value of `runtime``.
     """
     @property
     def container_orchestration(self) -> prodvana.proto.prodvana.runtimes.runtimes_config_pb2.ContainerOrchestrationRuntime: ...
     type: global___RuntimeConnectionType.ValueType
+    """set internally by prodvana, overridden even if set manually."""
     def __init__(
         self,
         *,
         runtime: builtins.str = ...,
         name: builtins.str = ...,
         container_orchestration: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.ContainerOrchestrationRuntime | None = ...,
         type: global___RuntimeConnectionType.ValueType = ...,
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,147 +1,79 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/release_channel/release_channel_manager.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from prodvana.proto.prodvana.events import events_pb2 as prodvana_dot_events_dot_events__pb2
 from prodvana.proto.prodvana.release_channel import object_pb2 as prodvana_dot_release__channel_dot_object__pb2
 from prodvana.proto.prodvana.release_channel import release_channel_config_pb2 as prodvana_dot_release__channel_dot_release__channel__config__pb2
+from prodvana.proto.prodvana.version import source_metadata_pb2 as prodvana_dot_version_dot_source__metadata__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n6prodvana/release_channel/release_channel_manager.proto\x12\x18prodvana.release_channel\x1a\x1cgoogle/api/annotations.proto\x1a\x1cprodvana/events/events.proto\x1a%prodvana/release_channel/object.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\x17validate/validate.proto\"\x8f\x01\n\x1a\x43onfigureReleaseChannelReq\x12G\n\x0frelease_channel\x18\x01 \x01(\x0b\x32..prodvana.release_channel.ReleaseChannelConfig\x12\x12\n\ncluster_id\x18\x02 \x01(\t\x12\x14\n\x0c\x63luster_name\x18\x03 \x01(\t\".\n\x1b\x43onfigureReleaseChannelResp\x12\x0f\n\x07version\x18\x01 \x01(\t\"2\n\x17\x44\x65leteReleaseChannelReq\x12\x17\n\x0frelease_channel\x18\x01 \x01(\t\"\x1a\n\x18\x44\x65leteReleaseChannelResp\"-\n\x16ListReleaseChannelsReq\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\"]\n\x17ListReleaseChannelsResp\x12\x42\n\x10release_channels\x18\x01 \x03(\x0b\x32(.prodvana.release_channel.ReleaseChannel\"D\n\x14GetReleaseChannelReq\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\"Z\n\x15GetReleaseChannelResp\x12\x41\n\x0frelease_channel\x18\x01 \x01(\x0b\x32(.prodvana.release_channel.ReleaseChannel\"\xa4\x01\n\x1aGetReleaseChannelEventsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12 \n\x0frelease_channel\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x1f\n\x17order_by_desc_timestamp\x18\x05 \x01(\x08\"^\n\x1bGetReleaseChannelEventsResp\x12&\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x16.prodvana.events.Event\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t2\xe1\x08\n\x15ReleaseChannelManager\x12\xb1\x01\n\x17\x43onfigureReleaseChannel\x12\x34.prodvana.release_channel.ConfigureReleaseChannelReq\x1a\x35.prodvana.release_channel.ConfigureReleaseChannelResp\")\x82\xd3\xe4\x93\x02#\"\x1e/v1/release-channels/configure:\x01*\x12\xb5\x01\n\x13ListReleaseChannels\x12\x30.prodvana.release_channel.ListReleaseChannelsReq\x1a\x31.prodvana.release_channel.ListReleaseChannelsResp\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v1/applications/{application=*}/release-channels\x12\xb6\x01\n\x14\x44\x65leteReleaseChannel\x12\x31.prodvana.release_channel.DeleteReleaseChannelReq\x1a\x32.prodvana.release_channel.DeleteReleaseChannelResp\"7\x82\xd3\xe4\x93\x02\x31*//v1/release-channels/{release_channel=*}/delete\x12~\n\x15ListReleaseChannelsV2\x12\x30.prodvana.release_channel.ListReleaseChannelsReq\x1a\x31.prodvana.release_channel.ListReleaseChannelsResp\"\x00\x12\xc3\x01\n\x11GetReleaseChannel\x12..prodvana.release_channel.GetReleaseChannelReq\x1a/.prodvana.release_channel.GetReleaseChannelResp\"M\x82\xd3\xe4\x93\x02G\x12\x45/v1/applications/{application=*}/release-channels/{release_channel=*}\x12\xdc\x01\n\x17GetReleaseChannelEvents\x12\x34.prodvana.release_channel.GetReleaseChannelEventsReq\x1a\x35.prodvana.release_channel.GetReleaseChannelEventsResp\"T\x82\xd3\xe4\x93\x02N\x12L/v1/applications/{application=*}/release-channels/{release_channel=*}/eventsBTZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/release_channelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n6prodvana/release_channel/release_channel_manager.proto\x12\x18prodvana.release_channel\x1a\x1cgoogle/api/annotations.proto\x1a\x1cprodvana/events/events.proto\x1a%prodvana/release_channel/object.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a&prodvana/version/source_metadata.proto\x1a\x17validate/validate.proto\"\x8e\x02\n\x1a\x43onfigureReleaseChannelReq\x12\x1c\n\x0b\x61pplication\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12G\n\x0frelease_channel\x18\x01 \x01(\x0b\x32..prodvana.release_channel.ReleaseChannelConfig\x12(\n\x06source\x18\x05 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x06 \x01(\x0b\x32 .prodvana.version.SourceMetadataJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\ncluster_idR\x0c\x63luster_name\".\n\x1b\x43onfigureReleaseChannelResp\x12\x0f\n\x07version\x18\x01 \x01(\t\"\xb5\x01\n\x17\x44\x65leteReleaseChannelReq\x12\x17\n\x0frelease_channel\x18\x01 \x01(\t\x12\x1c\n\x0b\x61pplication\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12(\n\x06source\x18\x03 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x04 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"+\n\x18\x44\x65leteReleaseChannelResp\x12\x0f\n\x07version\x18\x01 \x01(\t\"-\n\x16ListReleaseChannelsReq\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\"]\n\x17ListReleaseChannelsResp\x12\x42\n\x10release_channels\x18\x01 \x03(\x0b\x32(.prodvana.release_channel.ReleaseChannel\"D\n\x14GetReleaseChannelReq\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\"Z\n\x15GetReleaseChannelResp\x12\x41\n\x0frelease_channel\x18\x01 \x01(\x0b\x32(.prodvana.release_channel.ReleaseChannel\"d\n\x1aGetReleaseChannelConfigReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"\xb7\x01\n\x1bGetReleaseChannelConfigResp\x12>\n\x06\x63onfig\x18\x01 \x01(\x0b\x32..prodvana.release_channel.ReleaseChannelConfig\x12\x0f\n\x07version\x18\x02 \x01(\t\x12G\n\x0f\x63ompiled_config\x18\x03 \x01(\x0b\x32..prodvana.release_channel.ReleaseChannelConfig\"\xa4\x01\n\x1aGetReleaseChannelEventsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12 \n\x0frelease_channel\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x1f\n\x17order_by_desc_timestamp\x18\x05 \x01(\x08\"^\n\x1bGetReleaseChannelEventsResp\x12&\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x16.prodvana.events.Event\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t2\xdd\n\n\x15ReleaseChannelManager\x12\xce\x01\n\x17\x43onfigureReleaseChannel\x12\x34.prodvana.release_channel.ConfigureReleaseChannelReq\x1a\x35.prodvana.release_channel.ConfigureReleaseChannelResp\"F\x82\xd3\xe4\x93\x02@\";/v1/applications/{application=*}/release-channels/configure:\x01*\x12\xb5\x01\n\x13ListReleaseChannels\x12\x30.prodvana.release_channel.ListReleaseChannelsReq\x1a\x31.prodvana.release_channel.ListReleaseChannelsResp\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v1/applications/{application=*}/release-channels\x12\xb6\x01\n\x14\x44\x65leteReleaseChannel\x12\x31.prodvana.release_channel.DeleteReleaseChannelReq\x1a\x32.prodvana.release_channel.DeleteReleaseChannelResp\"7\x82\xd3\xe4\x93\x02\x31*//v1/release-channels/{release_channel=*}/delete\x12~\n\x15ListReleaseChannelsV2\x12\x30.prodvana.release_channel.ListReleaseChannelsReq\x1a\x31.prodvana.release_channel.ListReleaseChannelsResp\"\x00\x12\xc3\x01\n\x11GetReleaseChannel\x12..prodvana.release_channel.GetReleaseChannelReq\x1a/.prodvana.release_channel.GetReleaseChannelResp\"M\x82\xd3\xe4\x93\x02G\x12\x45/v1/applications/{application=*}/release-channels/{release_channel=*}\x12\xdc\x01\n\x17GetReleaseChannelConfig\x12\x34.prodvana.release_channel.GetReleaseChannelConfigReq\x1a\x35.prodvana.release_channel.GetReleaseChannelConfigResp\"T\x82\xd3\xe4\x93\x02N\x12L/v1/applications/{application=*}/release-channels/{release_channel=*}/config\x12\xdc\x01\n\x17GetReleaseChannelEvents\x12\x34.prodvana.release_channel.GetReleaseChannelEventsReq\x1a\x35.prodvana.release_channel.GetReleaseChannelEventsResp\"T\x82\xd3\xe4\x93\x02N\x12L/v1/applications/{application=*}/release-channels/{release_channel=*}/eventsBTZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/release_channelb\x06proto3')
 
-
-
-_CONFIGURERELEASECHANNELREQ = DESCRIPTOR.message_types_by_name['ConfigureReleaseChannelReq']
-_CONFIGURERELEASECHANNELRESP = DESCRIPTOR.message_types_by_name['ConfigureReleaseChannelResp']
-_DELETERELEASECHANNELREQ = DESCRIPTOR.message_types_by_name['DeleteReleaseChannelReq']
-_DELETERELEASECHANNELRESP = DESCRIPTOR.message_types_by_name['DeleteReleaseChannelResp']
-_LISTRELEASECHANNELSREQ = DESCRIPTOR.message_types_by_name['ListReleaseChannelsReq']
-_LISTRELEASECHANNELSRESP = DESCRIPTOR.message_types_by_name['ListReleaseChannelsResp']
-_GETRELEASECHANNELREQ = DESCRIPTOR.message_types_by_name['GetReleaseChannelReq']
-_GETRELEASECHANNELRESP = DESCRIPTOR.message_types_by_name['GetReleaseChannelResp']
-_GETRELEASECHANNELEVENTSREQ = DESCRIPTOR.message_types_by_name['GetReleaseChannelEventsReq']
-_GETRELEASECHANNELEVENTSRESP = DESCRIPTOR.message_types_by_name['GetReleaseChannelEventsResp']
-ConfigureReleaseChannelReq = _reflection.GeneratedProtocolMessageType('ConfigureReleaseChannelReq', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGURERELEASECHANNELREQ,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.ConfigureReleaseChannelReq)
-  })
-_sym_db.RegisterMessage(ConfigureReleaseChannelReq)
-
-ConfigureReleaseChannelResp = _reflection.GeneratedProtocolMessageType('ConfigureReleaseChannelResp', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGURERELEASECHANNELRESP,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.ConfigureReleaseChannelResp)
-  })
-_sym_db.RegisterMessage(ConfigureReleaseChannelResp)
-
-DeleteReleaseChannelReq = _reflection.GeneratedProtocolMessageType('DeleteReleaseChannelReq', (_message.Message,), {
-  'DESCRIPTOR' : _DELETERELEASECHANNELREQ,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.DeleteReleaseChannelReq)
-  })
-_sym_db.RegisterMessage(DeleteReleaseChannelReq)
-
-DeleteReleaseChannelResp = _reflection.GeneratedProtocolMessageType('DeleteReleaseChannelResp', (_message.Message,), {
-  'DESCRIPTOR' : _DELETERELEASECHANNELRESP,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.DeleteReleaseChannelResp)
-  })
-_sym_db.RegisterMessage(DeleteReleaseChannelResp)
-
-ListReleaseChannelsReq = _reflection.GeneratedProtocolMessageType('ListReleaseChannelsReq', (_message.Message,), {
-  'DESCRIPTOR' : _LISTRELEASECHANNELSREQ,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.ListReleaseChannelsReq)
-  })
-_sym_db.RegisterMessage(ListReleaseChannelsReq)
-
-ListReleaseChannelsResp = _reflection.GeneratedProtocolMessageType('ListReleaseChannelsResp', (_message.Message,), {
-  'DESCRIPTOR' : _LISTRELEASECHANNELSRESP,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.ListReleaseChannelsResp)
-  })
-_sym_db.RegisterMessage(ListReleaseChannelsResp)
-
-GetReleaseChannelReq = _reflection.GeneratedProtocolMessageType('GetReleaseChannelReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETRELEASECHANNELREQ,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.GetReleaseChannelReq)
-  })
-_sym_db.RegisterMessage(GetReleaseChannelReq)
-
-GetReleaseChannelResp = _reflection.GeneratedProtocolMessageType('GetReleaseChannelResp', (_message.Message,), {
-  'DESCRIPTOR' : _GETRELEASECHANNELRESP,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.GetReleaseChannelResp)
-  })
-_sym_db.RegisterMessage(GetReleaseChannelResp)
-
-GetReleaseChannelEventsReq = _reflection.GeneratedProtocolMessageType('GetReleaseChannelEventsReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETRELEASECHANNELEVENTSREQ,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.GetReleaseChannelEventsReq)
-  })
-_sym_db.RegisterMessage(GetReleaseChannelEventsReq)
-
-GetReleaseChannelEventsResp = _reflection.GeneratedProtocolMessageType('GetReleaseChannelEventsResp', (_message.Message,), {
-  'DESCRIPTOR' : _GETRELEASECHANNELEVENTSRESP,
-  '__module__' : 'prodvana.release_channel.release_channel_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.release_channel.GetReleaseChannelEventsResp)
-  })
-_sym_db.RegisterMessage(GetReleaseChannelEventsResp)
-
-_RELEASECHANNELMANAGER = DESCRIPTOR.services_by_name['ReleaseChannelManager']
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.release_channel.release_channel_manager_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/release_channel'
+  _CONFIGURERELEASECHANNELREQ.fields_by_name['application']._options = None
+  _CONFIGURERELEASECHANNELREQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
+  _DELETERELEASECHANNELREQ.fields_by_name['application']._options = None
+  _DELETERELEASECHANNELREQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
+  _GETRELEASECHANNELCONFIGREQ.fields_by_name['application']._options = None
+  _GETRELEASECHANNELCONFIGREQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
   _GETRELEASECHANNELEVENTSREQ.fields_by_name['application']._options = None
   _GETRELEASECHANNELEVENTSREQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
   _GETRELEASECHANNELEVENTSREQ.fields_by_name['release_channel']._options = None
   _GETRELEASECHANNELEVENTSREQ.fields_by_name['release_channel']._serialized_options = b'\372B\004r\002\020\001'
   _RELEASECHANNELMANAGER.methods_by_name['ConfigureReleaseChannel']._options = None
-  _RELEASECHANNELMANAGER.methods_by_name['ConfigureReleaseChannel']._serialized_options = b'\202\323\344\223\002#\"\036/v1/release-channels/configure:\001*'
+  _RELEASECHANNELMANAGER.methods_by_name['ConfigureReleaseChannel']._serialized_options = b'\202\323\344\223\002@\";/v1/applications/{application=*}/release-channels/configure:\001*'
   _RELEASECHANNELMANAGER.methods_by_name['ListReleaseChannels']._options = None
   _RELEASECHANNELMANAGER.methods_by_name['ListReleaseChannels']._serialized_options = b'\202\323\344\223\0023\0221/v1/applications/{application=*}/release-channels'
   _RELEASECHANNELMANAGER.methods_by_name['DeleteReleaseChannel']._options = None
   _RELEASECHANNELMANAGER.methods_by_name['DeleteReleaseChannel']._serialized_options = b'\202\323\344\223\0021*//v1/release-channels/{release_channel=*}/delete'
   _RELEASECHANNELMANAGER.methods_by_name['GetReleaseChannel']._options = None
   _RELEASECHANNELMANAGER.methods_by_name['GetReleaseChannel']._serialized_options = b'\202\323\344\223\002G\022E/v1/applications/{application=*}/release-channels/{release_channel=*}'
+  _RELEASECHANNELMANAGER.methods_by_name['GetReleaseChannelConfig']._options = None
+  _RELEASECHANNELMANAGER.methods_by_name['GetReleaseChannelConfig']._serialized_options = b'\202\323\344\223\002N\022L/v1/applications/{application=*}/release-channels/{release_channel=*}/config'
   _RELEASECHANNELMANAGER.methods_by_name['GetReleaseChannelEvents']._options = None
   _RELEASECHANNELMANAGER.methods_by_name['GetReleaseChannelEvents']._serialized_options = b'\202\323\344\223\002N\022L/v1/applications/{application=*}/release-channels/{release_channel=*}/events'
-  _CONFIGURERELEASECHANNELREQ._serialized_start=264
-  _CONFIGURERELEASECHANNELREQ._serialized_end=407
-  _CONFIGURERELEASECHANNELRESP._serialized_start=409
-  _CONFIGURERELEASECHANNELRESP._serialized_end=455
-  _DELETERELEASECHANNELREQ._serialized_start=457
-  _DELETERELEASECHANNELREQ._serialized_end=507
-  _DELETERELEASECHANNELRESP._serialized_start=509
-  _DELETERELEASECHANNELRESP._serialized_end=535
-  _LISTRELEASECHANNELSREQ._serialized_start=537
-  _LISTRELEASECHANNELSREQ._serialized_end=582
-  _LISTRELEASECHANNELSRESP._serialized_start=584
-  _LISTRELEASECHANNELSRESP._serialized_end=677
-  _GETRELEASECHANNELREQ._serialized_start=679
-  _GETRELEASECHANNELREQ._serialized_end=747
-  _GETRELEASECHANNELRESP._serialized_start=749
-  _GETRELEASECHANNELRESP._serialized_end=839
-  _GETRELEASECHANNELEVENTSREQ._serialized_start=842
-  _GETRELEASECHANNELEVENTSREQ._serialized_end=1006
-  _GETRELEASECHANNELEVENTSRESP._serialized_start=1008
-  _GETRELEASECHANNELEVENTSRESP._serialized_end=1102
-  _RELEASECHANNELMANAGER._serialized_start=1105
-  _RELEASECHANNELMANAGER._serialized_end=2226
+  _globals['_CONFIGURERELEASECHANNELREQ']._serialized_start=304
+  _globals['_CONFIGURERELEASECHANNELREQ']._serialized_end=574
+  _globals['_CONFIGURERELEASECHANNELRESP']._serialized_start=576
+  _globals['_CONFIGURERELEASECHANNELRESP']._serialized_end=622
+  _globals['_DELETERELEASECHANNELREQ']._serialized_start=625
+  _globals['_DELETERELEASECHANNELREQ']._serialized_end=806
+  _globals['_DELETERELEASECHANNELRESP']._serialized_start=808
+  _globals['_DELETERELEASECHANNELRESP']._serialized_end=851
+  _globals['_LISTRELEASECHANNELSREQ']._serialized_start=853
+  _globals['_LISTRELEASECHANNELSREQ']._serialized_end=898
+  _globals['_LISTRELEASECHANNELSRESP']._serialized_start=900
+  _globals['_LISTRELEASECHANNELSRESP']._serialized_end=993
+  _globals['_GETRELEASECHANNELREQ']._serialized_start=995
+  _globals['_GETRELEASECHANNELREQ']._serialized_end=1063
+  _globals['_GETRELEASECHANNELRESP']._serialized_start=1065
+  _globals['_GETRELEASECHANNELRESP']._serialized_end=1155
+  _globals['_GETRELEASECHANNELCONFIGREQ']._serialized_start=1157
+  _globals['_GETRELEASECHANNELCONFIGREQ']._serialized_end=1257
+  _globals['_GETRELEASECHANNELCONFIGRESP']._serialized_start=1260
+  _globals['_GETRELEASECHANNELCONFIGRESP']._serialized_end=1443
+  _globals['_GETRELEASECHANNELEVENTSREQ']._serialized_start=1446
+  _globals['_GETRELEASECHANNELEVENTSREQ']._serialized_end=1610
+  _globals['_GETRELEASECHANNELEVENTSRESP']._serialized_start=1612
+  _globals['_GETRELEASECHANNELEVENTSRESP']._serialized_end=1706
+  _globals['_RELEASECHANNELMANAGER']._serialized_start=1709
+  _globals['_RELEASECHANNELMANAGER']._serialized_end=3082
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -6,81 +6,102 @@
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import prodvana.proto.prodvana.events.events_pb2
 import prodvana.proto.prodvana.release_channel.object_pb2
 import prodvana.proto.prodvana.release_channel.release_channel_config_pb2
+import prodvana.proto.prodvana.version.source_metadata_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class ConfigureReleaseChannelReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    APPLICATION_FIELD_NUMBER: builtins.int
     RELEASE_CHANNEL_FIELD_NUMBER: builtins.int
-    CLUSTER_ID_FIELD_NUMBER: builtins.int
-    CLUSTER_NAME_FIELD_NUMBER: builtins.int
+    SOURCE_FIELD_NUMBER: builtins.int
+    SOURCE_METADATA_FIELD_NUMBER: builtins.int
+    application: builtins.str
     @property
     def release_channel(self) -> prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig: ...
-    cluster_id: builtins.str
-    """optional if there is only one cluster. If set, cluster_name should be empty."""
-    cluster_name: builtins.str
-    """optional if there is only one cluster. If set, cluster_id should be empty."""
+    source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType
+    @property
+    def source_metadata(self) -> prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata: ...
     def __init__(
         self,
         *,
+        application: builtins.str = ...,
         release_channel: prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig | None = ...,
-        cluster_id: builtins.str = ...,
-        cluster_name: builtins.str = ...,
+        source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType = ...,
+        source_metadata: prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["release_channel", b"release_channel"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cluster_id", b"cluster_id", "cluster_name", b"cluster_name", "release_channel", b"release_channel"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["release_channel", b"release_channel", "source_metadata", b"source_metadata"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "release_channel", b"release_channel", "source", b"source", "source_metadata", b"source_metadata"]) -> None: ...
 
 global___ConfigureReleaseChannelReq = ConfigureReleaseChannelReq
 
 class ConfigureReleaseChannelResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VERSION_FIELD_NUMBER: builtins.int
     version: builtins.str
+    """application version"""
     def __init__(
         self,
         *,
         version: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["version", b"version"]) -> None: ...
 
 global___ConfigureReleaseChannelResp = ConfigureReleaseChannelResp
 
 class DeleteReleaseChannelReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RELEASE_CHANNEL_FIELD_NUMBER: builtins.int
+    APPLICATION_FIELD_NUMBER: builtins.int
+    SOURCE_FIELD_NUMBER: builtins.int
+    SOURCE_METADATA_FIELD_NUMBER: builtins.int
     release_channel: builtins.str
+    application: builtins.str
+    source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType
+    @property
+    def source_metadata(self) -> prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata: ...
     def __init__(
         self,
         *,
         release_channel: builtins.str = ...,
+        application: builtins.str = ...,
+        source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType = ...,
+        source_metadata: prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["release_channel", b"release_channel"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["source_metadata", b"source_metadata"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "release_channel", b"release_channel", "source", b"source", "source_metadata", b"source_metadata"]) -> None: ...
 
 global___DeleteReleaseChannelReq = DeleteReleaseChannelReq
 
 class DeleteReleaseChannelResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    VERSION_FIELD_NUMBER: builtins.int
+    version: builtins.str
+    """application version"""
     def __init__(
         self,
+        *,
+        version: builtins.str = ...,
     ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["version", b"version"]) -> None: ...
 
 global___DeleteReleaseChannelResp = DeleteReleaseChannelResp
 
 class ListReleaseChannelsReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLICATION_FIELD_NUMBER: builtins.int
@@ -138,14 +159,60 @@
         release_channel: prodvana.proto.prodvana.release_channel.object_pb2.ReleaseChannel | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["release_channel", b"release_channel"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["release_channel", b"release_channel"]) -> None: ...
 
 global___GetReleaseChannelResp = GetReleaseChannelResp
 
+class GetReleaseChannelConfigReq(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    APPLICATION_FIELD_NUMBER: builtins.int
+    RELEASE_CHANNEL_FIELD_NUMBER: builtins.int
+    VERSION_FIELD_NUMBER: builtins.int
+    application: builtins.str
+    release_channel: builtins.str
+    version: builtins.str
+    """omit to get latest version"""
+    def __init__(
+        self,
+        *,
+        application: builtins.str = ...,
+        release_channel: builtins.str = ...,
+        version: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "release_channel", b"release_channel", "version", b"version"]) -> None: ...
+
+global___GetReleaseChannelConfigReq = GetReleaseChannelConfigReq
+
+class GetReleaseChannelConfigResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    CONFIG_FIELD_NUMBER: builtins.int
+    VERSION_FIELD_NUMBER: builtins.int
+    COMPILED_CONFIG_FIELD_NUMBER: builtins.int
+    @property
+    def config(self) -> prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig:
+        """config as passed in by user"""
+    version: builtins.str
+    @property
+    def compiled_config(self) -> prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig:
+        """config with defaults applied"""
+    def __init__(
+        self,
+        *,
+        config: prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig | None = ...,
+        version: builtins.str = ...,
+        compiled_config: prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelConfig | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["compiled_config", b"compiled_config", "config", b"config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["compiled_config", b"compiled_config", "config", b"config", "version", b"version"]) -> None: ...
+
+global___GetReleaseChannelConfigResp = GetReleaseChannelConfigResp
+
 class GetReleaseChannelEventsReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLICATION_FIELD_NUMBER: builtins.int
     RELEASE_CHANNEL_FIELD_NUMBER: builtins.int
     PAGE_TOKEN_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,19 @@
                 response_deserializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.ListReleaseChannelsResp.FromString,
                 )
         self.GetReleaseChannel = channel.unary_unary(
                 '/prodvana.release_channel.ReleaseChannelManager/GetReleaseChannel',
                 request_serializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelReq.SerializeToString,
                 response_deserializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelResp.FromString,
                 )
+        self.GetReleaseChannelConfig = channel.unary_unary(
+                '/prodvana.release_channel.ReleaseChannelManager/GetReleaseChannelConfig',
+                request_serializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelConfigReq.SerializeToString,
+                response_deserializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelConfigResp.FromString,
+                )
         self.GetReleaseChannelEvents = channel.unary_unary(
                 '/prodvana.release_channel.ReleaseChannelManager/GetReleaseChannelEvents',
                 request_serializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelEventsReq.SerializeToString,
                 response_deserializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelEventsResp.FromString,
                 )
 
 
@@ -76,14 +81,20 @@
 
     def GetReleaseChannel(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetReleaseChannelConfig(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetReleaseChannelEvents(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
@@ -110,14 +121,19 @@
                     response_serializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.ListReleaseChannelsResp.SerializeToString,
             ),
             'GetReleaseChannel': grpc.unary_unary_rpc_method_handler(
                     servicer.GetReleaseChannel,
                     request_deserializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelReq.FromString,
                     response_serializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelResp.SerializeToString,
             ),
+            'GetReleaseChannelConfig': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetReleaseChannelConfig,
+                    request_deserializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelConfigReq.FromString,
+                    response_serializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelConfigResp.SerializeToString,
+            ),
             'GetReleaseChannelEvents': grpc.unary_unary_rpc_method_handler(
                     servicer.GetReleaseChannelEvents,
                     request_deserializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelEventsReq.FromString,
                     response_serializer=prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelEventsResp.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -211,14 +227,31 @@
         return grpc.experimental.unary_unary(request, target, '/prodvana.release_channel.ReleaseChannelManager/GetReleaseChannel',
             prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelReq.SerializeToString,
             prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetReleaseChannelConfig(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/prodvana.release_channel.ReleaseChannelManager/GetReleaseChannelConfig',
+            prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelConfigReq.SerializeToString,
+            prodvana_dot_release__channel_dot_release__channel__manager__pb2.GetReleaseChannelConfigResp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetReleaseChannelEvents(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.ListReleaseChannelsResp,
     ]
     """identical to ListReleaseChannels, kept for backwards compatibility"""
     GetReleaseChannel: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelReq,
         prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelResp,
     ]
+    GetReleaseChannelConfig: grpc.UnaryUnaryMultiCallable[
+        prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelConfigReq,
+        prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelConfigResp,
+    ]
     GetReleaseChannelEvents: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelEventsReq,
         prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelEventsResp,
     ]
 
 class ReleaseChannelManagerServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
@@ -63,14 +67,20 @@
     @abc.abstractmethod
     def GetReleaseChannel(
         self,
         request: prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelResp: ...
     @abc.abstractmethod
+    def GetReleaseChannelConfig(
+        self,
+        request: prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelConfigReq,
+        context: grpc.ServicerContext,
+    ) -> prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelConfigResp: ...
+    @abc.abstractmethod
     def GetReleaseChannelEvents(
         self,
         request: prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelEventsReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.release_channel.release_channel_manager_pb2.GetReleaseChannelEventsResp: ...
 
 def add_ReleaseChannelManagerServicer_to_server(servicer: ReleaseChannelManagerServicer, server: grpc.Server) -> None: ...
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/repo/repo.proto
+# source: prodvana/delivery_extension/object.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from prodvana.proto.prodvana.object import meta_pb2 as prodvana_dot_object_dot_meta__pb2
+from prodvana.proto.prodvana.delivery_extension import config_pb2 as prodvana_dot_delivery__extension_dot_config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18prodvana/repo/repo.proto\x12\rprodvana.repo\"#\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\"^\n\x06\x43ommit\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12#\n\x06\x61uthor\x18\x04 \x01(\x0b\x32\x13.prodvana.repo.User\"1\n\x0b\x46uzzyCommit\x12\x12\n\ncommit_ish\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\tBIZGgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/repob\x06proto3')
-
-
-
-_USER = DESCRIPTOR.message_types_by_name['User']
-_COMMIT = DESCRIPTOR.message_types_by_name['Commit']
-_FUZZYCOMMIT = DESCRIPTOR.message_types_by_name['FuzzyCommit']
-User = _reflection.GeneratedProtocolMessageType('User', (_message.Message,), {
-  'DESCRIPTOR' : _USER,
-  '__module__' : 'prodvana.repo.repo_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.repo.User)
-  })
-_sym_db.RegisterMessage(User)
-
-Commit = _reflection.GeneratedProtocolMessageType('Commit', (_message.Message,), {
-  'DESCRIPTOR' : _COMMIT,
-  '__module__' : 'prodvana.repo.repo_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.repo.Commit)
-  })
-_sym_db.RegisterMessage(Commit)
-
-FuzzyCommit = _reflection.GeneratedProtocolMessageType('FuzzyCommit', (_message.Message,), {
-  'DESCRIPTOR' : _FUZZYCOMMIT,
-  '__module__' : 'prodvana.repo.repo_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.repo.FuzzyCommit)
-  })
-_sym_db.RegisterMessage(FuzzyCommit)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(prodvana/delivery_extension/object.proto\x12\x1bprodvana.delivery_extension\x1a\x1aprodvana/object/meta.proto\x1a(prodvana/delivery_extension/config.proto\"\xc8\x01\n\x11\x44\x65liveryExtension\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x44\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x42\n\x05state\x18\x03 \x01(\x0b\x32\x33.prodvana.delivery_extension.DeliveryExtensionState\"\x18\n\x16\x44\x65liveryExtensionStateBWZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.delivery_extension.object_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZGgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/repo'
-  _USER._serialized_start=43
-  _USER._serialized_end=78
-  _COMMIT._serialized_start=80
-  _COMMIT._serialized_end=174
-  _FUZZYCOMMIT._serialized_start=176
-  _FUZZYCOMMIT._serialized_end=225
+  DESCRIPTOR._serialized_options = b'ZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extension'
+  _globals['_DELIVERYEXTENSION']._serialized_start=144
+  _globals['_DELIVERYEXTENSION']._serialized_end=344
+  _globals['_DELIVERYEXTENSIONSTATE']._serialized_start=346
+  _globals['_DELIVERYEXTENSIONSTATE']._serialized_end=370
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/runtimes/features_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/runtimes/features.proto
+# source: prodvana/stat/efficiency.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n prodvana/runtimes/features.proto\x12\x11prodvana.runtimes*s\n\x0b\x46\x65\x61tureType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x13\n\x0f\x45XPOSED_SERVICE\x10\x01\x12\x0f\n\x0bTLS_SERVICE\x10\x02\x12\x11\n\rCOST_ANALYSIS\x10\x03\x12\x0b\n\x07\x44\x41TADOG\x10\x04\x12\x11\n\rARGO_ROLLOUTS\x10\x05\x42MZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/runtimesb\x06proto3')
-
-_FEATURETYPE = DESCRIPTOR.enum_types_by_name['FeatureType']
-FeatureType = enum_type_wrapper.EnumTypeWrapper(_FEATURETYPE)
-UNKNOWN = 0
-EXPOSED_SERVICE = 1
-TLS_SERVICE = 2
-COST_ANALYSIS = 3
-DATADOG = 4
-ARGO_ROLLOUTS = 5
-
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eprodvana/stat/efficiency.proto\x12\rprodvana.stat\"A\n\x0e\x45\x66\x66iciencyStat\x12\x13\n\x0bsaved_lines\x18\x01 \x01(\x05\x12\x1a\n\x12materialized_lines\x18\x02 \x01(\x05\x42IZGgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/statb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.stat.efficiency_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/runtimes'
-  _FEATURETYPE._serialized_start=55
-  _FEATURETYPE._serialized_end=170
+  DESCRIPTOR._serialized_options = b'ZGgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/stat'
+  _globals['_EFFICIENCYSTAT']._serialized_start=49
+  _globals['_EFFICIENCYSTAT']._serialized_end=114
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/runtimes/features_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -35,31 +35,35 @@
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     AGENT_IMAGE_FIELD_NUMBER: builtins.int
     AUTH_TOKEN_FIELD_NUMBER: builtins.int
     USE_RESOURCE_DEFAULT_FIELD_NUMBER: builtins.int
     INTERACTION_SERVER_ADDRESS_FIELD_NUMBER: builtins.int
     ENV_VARS_FIELD_NUMBER: builtins.int
+    AGENT_EXTERNALLY_MANAGED_FIELD_NUMBER: builtins.int
     agent_image: builtins.str
     auth_token: builtins.str
     use_resource_default: builtins.bool
     interaction_server_address: builtins.str
     @property
     def env_vars(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Env vars, mainly used to pass in proxy information. This is generally supplied by customers."""
+    agent_externally_managed: builtins.bool
+    """The Prodvana agent lifecycle is handled by the user -- Prodvana will not install or update the agent."""
     def __init__(
         self,
         *,
         agent_image: builtins.str = ...,
         auth_token: builtins.str = ...,
         use_resource_default: builtins.bool = ...,
         interaction_server_address: builtins.str = ...,
         env_vars: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        agent_externally_managed: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["agent_image", b"agent_image", "auth_token", b"auth_token", "env_vars", b"env_vars", "interaction_server_address", b"interaction_server_address", "use_resource_default", b"use_resource_default"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["agent_externally_managed", b"agent_externally_managed", "agent_image", b"agent_image", "auth_token", b"auth_token", "env_vars", b"env_vars", "interaction_server_address", b"interaction_server_address", "use_resource_default", b"use_resource_default"]) -> None: ...
 
 global___K8SRuntimeInitializationConfig = K8SRuntimeInitializationConfig
 
 class RuntimeInitializationConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     K8S_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/scm/types.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18prodvana/scm/types.proto\x12\x0cprodvana.scm*\"\n\x07ScmType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06GITHUB\x10\x01\x42HZFgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/scmb\x06proto3')
 
-_SCMTYPE = DESCRIPTOR.enum_types_by_name['ScmType']
-ScmType = enum_type_wrapper.EnumTypeWrapper(_SCMTYPE)
-UNKNOWN = 0
-GITHUB = 1
-
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.scm.types_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZFgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/scm'
-  _SCMTYPE._serialized_start=42
-  _SCMTYPE._serialized_end=76
+  _globals['_SCMTYPE']._serialized_start=42
+  _globals['_SCMTYPE']._serialized_end=76
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,43 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/service/object.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.object import meta_pb2 as prodvana_dot_object_dot_meta__pb2
 from prodvana.proto.prodvana.common_config import meta_pb2 as prodvana_dot_common__config_dot_meta__pb2
 from prodvana.proto.prodvana.service import service_config_pb2 as prodvana_dot_service_dot_service__config__pb2
 from prodvana.proto.prodvana.service import user_metadata_pb2 as prodvana_dot_service_dot_user__metadata__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dprodvana/service/object.proto\x12\x10prodvana.service\x1a\x1aprodvana/object/meta.proto\x1a!prodvana/common_config/meta.proto\x1a%prodvana/service/service_config.proto\x1a$prodvana/service/user_metadata.proto\"\x9a\x01\n\x0c\x45xternalAddr\x12\x0c\n\x04\x61\x64\x64r\x18\x01 \x01(\t\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.prodvana.service.ExternalAddr.Type\"I\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04\x41UTO\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02\x12\n\n\x06RAW_IP\x10\x03\x12\x10\n\x0cRAW_HOSTNAME\x10\x04\"8\n\x0cServiceStateJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03R\x15ongoing_pipeline_runsR\x05state\"\xd2\x01\n\x07Service\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12/\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12-\n\x05state\x18\x03 \x01(\x0b\x32\x1e.prodvana.service.ServiceState\x12<\n\ruser_metadata\x18\x04 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadata\"\xda\x02\n\x14ServiceInstanceState\x12\x36\n\x0e\x65xternal_addrs\x18\x07 \x03(\x0b\x32\x1e.prodvana.service.ExternalAddrJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rR\x05stateR\x0e\x61vailable_podsR\x0c\x64\x65sired_podsR\x1flatest_successful_prodvana_pushR2latest_successful_unknown_push_after_prodvana_pushR\x0congoing_pushR\x04podsR\nruntime_idR\x0cruntime_nameR\x10writeback_configR\x0e\x64\x65livery_state\"\xca\x01\n\x0fServiceInstance\x12?\n\x04meta\x18\x01 \x01(\x0b\x32\x31.prodvana.common_config.ServiceInstanceObjectMeta\x12?\n\x06\x63onfig\x18\x02 \x01(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\x12\x35\n\x05state\x18\x03 \x01(\x0b\x32&.prodvana.service.ServiceInstanceStateBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
-
-
-
-_EXTERNALADDR = DESCRIPTOR.message_types_by_name['ExternalAddr']
-_SERVICESTATE = DESCRIPTOR.message_types_by_name['ServiceState']
-_SERVICE = DESCRIPTOR.message_types_by_name['Service']
-_SERVICEINSTANCESTATE = DESCRIPTOR.message_types_by_name['ServiceInstanceState']
-_SERVICEINSTANCE = DESCRIPTOR.message_types_by_name['ServiceInstance']
-_EXTERNALADDR_TYPE = _EXTERNALADDR.enum_types_by_name['Type']
-ExternalAddr = _reflection.GeneratedProtocolMessageType('ExternalAddr', (_message.Message,), {
-  'DESCRIPTOR' : _EXTERNALADDR,
-  '__module__' : 'prodvana.service.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.ExternalAddr)
-  })
-_sym_db.RegisterMessage(ExternalAddr)
-
-ServiceState = _reflection.GeneratedProtocolMessageType('ServiceState', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICESTATE,
-  '__module__' : 'prodvana.service.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.ServiceState)
-  })
-_sym_db.RegisterMessage(ServiceState)
-
-Service = _reflection.GeneratedProtocolMessageType('Service', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICE,
-  '__module__' : 'prodvana.service.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.Service)
-  })
-_sym_db.RegisterMessage(Service)
-
-ServiceInstanceState = _reflection.GeneratedProtocolMessageType('ServiceInstanceState', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICEINSTANCESTATE,
-  '__module__' : 'prodvana.service.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.ServiceInstanceState)
-  })
-_sym_db.RegisterMessage(ServiceInstanceState)
-
-ServiceInstance = _reflection.GeneratedProtocolMessageType('ServiceInstance', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICEINSTANCE,
-  '__module__' : 'prodvana.service.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.ServiceInstance)
-  })
-_sym_db.RegisterMessage(ServiceInstance)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dprodvana/service/object.proto\x12\x10prodvana.service\x1a\x1aprodvana/object/meta.proto\x1a!prodvana/common_config/meta.proto\x1a%prodvana/service/service_config.proto\x1a$prodvana/service/user_metadata.proto\"~\n#ServiceInstanceProtectionAttachment\x12\x12\n\nprotection\x18\x01 \x01(\t\x12\x12\n\nattachment\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65sired_state_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\x9a\x01\n\x0c\x45xternalAddr\x12\x0c\n\x04\x61\x64\x64r\x18\x01 \x01(\t\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.prodvana.service.ExternalAddr.Type\"I\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04\x41UTO\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02\x12\n\n\x06RAW_IP\x10\x03\x12\x10\n\x0cRAW_HOSTNAME\x10\x04\"8\n\x0cServiceStateJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03R\x15ongoing_pipeline_runsR\x05state\"\xd2\x01\n\x07Service\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12/\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12-\n\x05state\x18\x03 \x01(\x0b\x32\x1e.prodvana.service.ServiceState\x12<\n\ruser_metadata\x18\x04 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadata\"\xb1\x03\n\x14ServiceInstanceState\x12\x36\n\x0e\x65xternal_addrs\x18\x07 \x03(\x0b\x32\x1e.prodvana.service.ExternalAddr\x12U\n\x16protection_attachments\x18\r \x03(\x0b\x32\x35.prodvana.service.ServiceInstanceProtectionAttachmentJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rR\x05stateR\x0e\x61vailable_podsR\x0c\x64\x65sired_podsR\x1flatest_successful_prodvana_pushR2latest_successful_unknown_push_after_prodvana_pushR\x0congoing_pushR\x04podsR\nruntime_idR\x0cruntime_nameR\x10writeback_configR\x0e\x64\x65livery_state\"\xca\x01\n\x0fServiceInstance\x12?\n\x04meta\x18\x01 \x01(\x0b\x32\x31.prodvana.common_config.ServiceInstanceObjectMeta\x12?\n\x06\x63onfig\x18\x02 \x01(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\x12\x35\n\x05state\x18\x03 \x01(\x0b\x32&.prodvana.service.ServiceInstanceStateBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.service.object_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/service'
-  _EXTERNALADDR._serialized_start=192
-  _EXTERNALADDR._serialized_end=346
-  _EXTERNALADDR_TYPE._serialized_start=273
-  _EXTERNALADDR_TYPE._serialized_end=346
-  _SERVICESTATE._serialized_start=348
-  _SERVICESTATE._serialized_end=404
-  _SERVICE._serialized_start=407
-  _SERVICE._serialized_end=617
-  _SERVICEINSTANCESTATE._serialized_start=620
-  _SERVICEINSTANCESTATE._serialized_end=966
-  _SERVICEINSTANCE._serialized_start=969
-  _SERVICEINSTANCE._serialized_end=1171
+  _globals['_SERVICEINSTANCEPROTECTIONATTACHMENT']._serialized_start=191
+  _globals['_SERVICEINSTANCEPROTECTIONATTACHMENT']._serialized_end=317
+  _globals['_EXTERNALADDR']._serialized_start=320
+  _globals['_EXTERNALADDR']._serialized_end=474
+  _globals['_EXTERNALADDR_TYPE']._serialized_start=401
+  _globals['_EXTERNALADDR_TYPE']._serialized_end=474
+  _globals['_SERVICESTATE']._serialized_start=476
+  _globals['_SERVICESTATE']._serialized_end=532
+  _globals['_SERVICE']._serialized_start=535
+  _globals['_SERVICE']._serialized_end=745
+  _globals['_SERVICEINSTANCESTATE']._serialized_start=748
+  _globals['_SERVICEINSTANCESTATE']._serialized_end=1181
+  _globals['_SERVICEINSTANCE']._serialized_start=1184
+  _globals['_SERVICEINSTANCE']._serialized_end=1386
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/service/parameters.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/service/parameters.proto\x12\x10prodvana.service\x1a\'prodvana/common_config/parameters.proto\"w\n PerReleaseChannelParameterValues\x12\x17\n\x0frelease_channel\x18\x01 \x01(\t\x12:\n\nparameters\x18\x02 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"\xa5\x01\n\x16ServiceParameterValues\x12:\n\nparameters\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12O\n\x13per_release_channel\x18\x02 \x03(\x0b\x32\x32.prodvana.service.PerReleaseChannelParameterValuesBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
-
-
-_PERRELEASECHANNELPARAMETERVALUES = DESCRIPTOR.message_types_by_name['PerReleaseChannelParameterValues']
-_SERVICEPARAMETERVALUES = DESCRIPTOR.message_types_by_name['ServiceParameterValues']
-PerReleaseChannelParameterValues = _reflection.GeneratedProtocolMessageType('PerReleaseChannelParameterValues', (_message.Message,), {
-  'DESCRIPTOR' : _PERRELEASECHANNELPARAMETERVALUES,
-  '__module__' : 'prodvana.service.parameters_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.PerReleaseChannelParameterValues)
-  })
-_sym_db.RegisterMessage(PerReleaseChannelParameterValues)
-
-ServiceParameterValues = _reflection.GeneratedProtocolMessageType('ServiceParameterValues', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICEPARAMETERVALUES,
-  '__module__' : 'prodvana.service.parameters_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.ServiceParameterValues)
-  })
-_sym_db.RegisterMessage(ServiceParameterValues)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.service.parameters_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/service'
-  _PERRELEASECHANNELPARAMETERVALUES._serialized_start=96
-  _PERRELEASECHANNELPARAMETERVALUES._serialized_end=215
-  _SERVICEPARAMETERVALUES._serialized_start=218
-  _SERVICEPARAMETERVALUES._serialized_end=383
+  _globals['_PERRELEASECHANNELPARAMETERVALUES']._serialized_start=96
+  _globals['_PERRELEASECHANNELPARAMETERVALUES']._serialized_end=215
+  _globals['_SERVICEPARAMETERVALUES']._serialized_start=218
+  _globals['_SERVICEPARAMETERVALUES']._serialized_end=383
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import prodvana.proto.prodvana.capability.capability_pb2
+import prodvana.proto.prodvana.common_config.constants_pb2
 import prodvana.proto.prodvana.common_config.env_pb2
 import prodvana.proto.prodvana.common_config.helm_pb2
 import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
 import prodvana.proto.prodvana.common_config.maturity_pb2
 import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.program_pb2
-import prodvana.proto.prodvana.common_config.ref_pb2
 import prodvana.proto.prodvana.common_config.retry_pb2
 import prodvana.proto.prodvana.common_config.task_pb2
 import prodvana.proto.prodvana.delivery.delivery_config_pb2
 import prodvana.proto.prodvana.delivery_extension.config_pb2
+import prodvana.proto.prodvana.protection.attachments_pb2
 import prodvana.proto.prodvana.protection.protection_reference_pb2
 import prodvana.proto.prodvana.release_channel.release_channel_config_pb2
 import prodvana.proto.prodvana.runtimes.runtimes_config_pb2
 import prodvana.proto.prodvana.service.parameters_pb2
 import prodvana.proto.prodvana.volumes.volumes_pb2
 import prodvana.proto.prodvana.workflow.integration_config_pb2
 import sys
@@ -202,14 +203,31 @@
     def WhichOneof(self, oneof_group: typing_extensions.Literal["certificate", b"certificate"]) -> typing_extensions.Literal["tls", "aws_acm_cert"] | None: ...
 
 global___Certificate = Certificate
 
 class PerReleaseChannelConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    class EnvEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> prodvana.proto.prodvana.common_config.env_pb2.EnvValue: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: prodvana.proto.prodvana.common_config.env_pb2.EnvValue | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     RELEASE_CHANNEL_FIELD_NUMBER: builtins.int
     CUSTOM_HOSTNAMES_FIELD_NUMBER: builtins.int
     PROGRAMS_FIELD_NUMBER: builtins.int
     CERT_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     REPLICAS_FIELD_NUMBER: builtins.int
@@ -217,14 +235,17 @@
     DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     RUNTIME_CONNECTION_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
+    ENV_FIELD_NUMBER: builtins.int
+    CONSTANTS_FIELD_NUMBER: builtins.int
+    PROTECTIONS_FIELD_NUMBER: builtins.int
     release_channel: builtins.str
     @property
     def custom_hostnames(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
     def programs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.program_pb2.PerReleaseChannelProgramConfig]: ...
     @property
     def cert(self) -> global___Certificate: ...
@@ -250,14 +271,26 @@
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def external_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig:
         """deprecated, pass this as kubernetes_config instead"""
     @property
     def helm(self) -> prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig: ...
+    @property
+    def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
+        """Additional env variables that are injected to the service.
+        This can be useful for injecting and/or overriding env variables from release channel
+        configs for Kubernetes and runtime extension configs.
+        Not supported for helm configs.
+        """
+    @property
+    def constants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.constants_pb2.Constant]:
+        """constants made available in template substitutions"""
+    @property
+    def protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]: ...
     def __init__(
         self,
         *,
         release_channel: builtins.str = ...,
         custom_hostnames: collections.abc.Iterable[builtins.str] | None = ...,
         programs: collections.abc.Iterable[prodvana.proto.prodvana.common_config.program_pb2.PerReleaseChannelProgramConfig] | None = ...,
         cert: global___Certificate | None = ...,
@@ -268,17 +301,20 @@
         delivery_extensions: collections.abc.Iterable[global___DeliveryExtensionConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         runtime_connection: builtins.str = ...,
         runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         external_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
+        env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
+        constants: collections.abc.Iterable[prodvana.proto.prodvana.common_config.constants_pb2.Constant] | None = ...,
+        protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "replicas", b"replicas", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "delivery_extensions", b"delivery_extensions", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "release_channel", b"release_channel", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "constants", b"constants", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "delivery_extensions", b"delivery_extensions", "env", b"env", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "protections", b"protections", "release_channel", b"release_channel", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "external_config", "helm"] | None: ...
 
 global___PerReleaseChannelConfig = PerReleaseChannelConfig
 
 class CapabilityReference(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -396,30 +432,69 @@
 
 global___ProtectionLink = ProtectionLink
 
 class DeliveryExtensionConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INLINED_FIELD_NUMBER: builtins.int
+    INSTANCE_FIELD_NUMBER: builtins.int
+    REF_FIELD_NUMBER: builtins.int
     LIFECYCLE_FIELD_NUMBER: builtins.int
     @property
-    def inlined(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig: ...
+    def inlined(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig:
+        """Inline definition of a delivery extension."""
+    instance: builtins.str
+    """A delivery instance defined in this service config."""
+    @property
+    def ref(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionInstanceRef:
+        """Reference to a delivery extension defined externally."""
     lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType
     def __init__(
         self,
         *,
         inlined: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
+        instance: builtins.str = ...,
+        ref: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionInstanceRef | None = ...,
         lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["definition", b"definition", "inlined", b"inlined"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["definition", b"definition", "inlined", b"inlined", "lifecycle", b"lifecycle"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["definition", b"definition"]) -> typing_extensions.Literal["inlined"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["definition", b"definition", "inlined", b"inlined", "instance", b"instance", "ref", b"ref"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["definition", b"definition", "inlined", b"inlined", "instance", b"instance", "lifecycle", b"lifecycle", "ref", b"ref"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["definition", b"definition"]) -> typing_extensions.Literal["inlined", "instance", "ref"] | None: ...
 
 global___DeliveryExtensionConfig = DeliveryExtensionConfig
 
+class DeliveryExtensionInstance(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    INLINED_FIELD_NUMBER: builtins.int
+    REF_FIELD_NUMBER: builtins.int
+    NAME_FIELD_NUMBER: builtins.int
+    LIFECYCLE_FIELD_NUMBER: builtins.int
+    @property
+    def inlined(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig:
+        """Inline definition of the delivery extension."""
+    @property
+    def ref(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionInstanceRef:
+        """Reference to a delivery extension defined externally."""
+    name: builtins.str
+    lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType
+    def __init__(
+        self,
+        *,
+        inlined: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
+        ref: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionInstanceRef | None = ...,
+        name: builtins.str = ...,
+        lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["definition", b"definition", "inlined", b"inlined", "ref", b"ref"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["definition", b"definition", "inlined", b"inlined", "lifecycle", b"lifecycle", "name", b"name", "ref", b"ref"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["definition", b"definition"]) -> typing_extensions.Literal["inlined", "ref"] | None: ...
+
+global___DeliveryExtensionInstance = DeliveryExtensionInstance
+
 class RuntimeSpecificConfig(google.protobuf.message.Message):
     """RuntimeSpecificConfig contains Service level configuration options that only make sense for a
     specific Runtime type. Configuration added here should only apply to a single Service; if the
     Runtime specific configuration relates to all services, it should be configured as at the
     Runtime cluster level (or as a runtime extension).
     """
 
@@ -493,38 +568,14 @@
         *,
         disabled: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["disabled", b"disabled"]) -> None: ...
 
 global___AutoRollbackConfig = AutoRollbackConfig
 
-class ProtectionConvergenceAttachment(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    NAME_FIELD_NUMBER: builtins.int
-    REF_FIELD_NUMBER: builtins.int
-    LIFECYCLE_FIELD_NUMBER: builtins.int
-    name: builtins.str
-    """optional, default to protection name"""
-    @property
-    def ref(self) -> prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionReference: ...
-    @property
-    def lifecycle(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionLifecycle]: ...
-    def __init__(
-        self,
-        *,
-        name: builtins.str = ...,
-        ref: prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionReference | None = ...,
-        lifecycle: collections.abc.Iterable[prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionLifecycle] | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["ref", b"ref"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["lifecycle", b"lifecycle", "name", b"name", "ref", b"ref"]) -> None: ...
-
-global___ProtectionConvergenceAttachment = ProtectionConvergenceAttachment
-
 class ServiceConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _ParametersAutogen:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -543,38 +594,58 @@
     NONE: ServiceConfig.ParametersAutogen.ValueType  # 1
     """no autogen"""
     IMAGE: ServiceConfig.ParametersAutogen.ValueType  # 2
     """autogen one parameter per program for the image"""
     IMAGE_AND_REPLICAS: ServiceConfig.ParametersAutogen.ValueType  # 3
     """IMAGE + autogen a parameter for replicas count"""
 
+    class EnvEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> prodvana.proto.prodvana.common_config.env_pb2.EnvValue: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: prodvana.proto.prodvana.common_config.env_pb2.EnvValue | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     NAME_FIELD_NUMBER: builtins.int
     APPLICATION_FIELD_NUMBER: builtins.int
     PROGRAMS_FIELD_NUMBER: builtins.int
     REPLICAS_FIELD_NUMBER: builtins.int
     RELEASE_STRATEGY_FIELD_NUMBER: builtins.int
     PER_RELEASE_CHANNEL_FIELD_NUMBER: builtins.int
     CAPABILITIES_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     DEPLOY_ANNOTATIONS_FIELD_NUMBER: builtins.int
-    BASE_TEMPLATE_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
     DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSION_INSTANCES_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     RUNTIME_CONNECTION_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
+    CONSTANTS_FIELD_NUMBER: builtins.int
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     PARAMETERS_AUTOGEN_FIELD_NUMBER: builtins.int
     AUTO_ROLLBACK_FIELD_NUMBER: builtins.int
+    NO_CLEANUP_ON_DELETE_FIELD_NUMBER: builtins.int
+    ENV_FIELD_NUMBER: builtins.int
     name: builtins.str
     application: builtins.str
     @property
     def programs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig]: ...
     @property
     def replicas(self) -> global___ReplicasConfig: ...
     @property
@@ -586,32 +657,35 @@
     @property
     def delivery_config(self) -> prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig: ...
     @property
     def volumes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.volumes.volumes_pb2.Volume]: ...
     @property
     def deploy_annotations(self) -> prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig: ...
     @property
-    def base_template(self) -> prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef: ...
-    @property
     def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]:
         """DEPRECATED: Replace with delivery_extensions once its implemented."""
     @property
     def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionConfig]: ...
     @property
+    def delivery_extension_instances(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionInstance]: ...
+    @property
     def runtime_specific(self) -> global___RuntimeSpecificConfig: ...
     runtime_connection: builtins.str
     """which runtime connection to use in each release channel.
     optional if only one runtime makes sense for the service config.
     """
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
     @property
     def parameter_values(self) -> prodvana.proto.prodvana.service.parameters_pb2.ServiceParameterValues:
         """only valid to set in compiled configs by Prodvana"""
     @property
+    def constants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.constants_pb2.Constant]:
+        """constants made available in template substitutions"""
+    @property
     def progress_deadline(self) -> google.protobuf.duration_pb2.Duration:
         """how long to wait before marking deployment as failed"""
     @property
     def runtime_extension(self) -> global___RuntimeExtensionConfig: ...
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
@@ -619,44 +693,56 @@
         """deprecated, pass this as kubernetes_config instead"""
     @property
     def helm(self) -> prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig: ...
     parameters_autogen: global___ServiceConfig.ParametersAutogen.ValueType
     """How to autogenerate parameters, defaults to IMAGE"""
     @property
     def auto_rollback(self) -> global___AutoRollbackConfig: ...
+    no_cleanup_on_delete: builtins.bool
+    """if set, do not attempt to delete the underlying runtime objects when deleting a service"""
+    @property
+    def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
+        """Additional env variables that are injected to the service.
+        This can be useful for injecting and/or overriding env variables from release channel
+        configs for Kubernetes and runtime extension configs.
+        Not supported for helm configs.
+        """
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         application: builtins.str = ...,
         programs: collections.abc.Iterable[prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig] | None = ...,
         replicas: global___ReplicasConfig | None = ...,
         release_strategy: global___ReleaseStrategyConfig | None = ...,
         per_release_channel: collections.abc.Iterable[global___PerReleaseChannelConfig] | None = ...,
         capabilities: collections.abc.Iterable[global___CapabilityReference] | None = ...,
         delivery_config: prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig | None = ...,
         volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         deploy_annotations: prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig | None = ...,
-        base_template: prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
         delivery_extensions: collections.abc.Iterable[global___DeliveryExtensionConfig] | None = ...,
+        delivery_extension_instances: collections.abc.Iterable[global___DeliveryExtensionInstance] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         runtime_connection: builtins.str = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         parameter_values: prodvana.proto.prodvana.service.parameters_pb2.ServiceParameterValues | None = ...,
+        constants: collections.abc.Iterable[prodvana.proto.prodvana.common_config.constants_pb2.Constant] | None = ...,
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
         runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         external_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
         parameters_autogen: global___ServiceConfig.ParametersAutogen.ValueType = ...,
         auto_rollback: global___AutoRollbackConfig | None = ...,
+        no_cleanup_on_delete: builtins.bool = ...,
+        env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["auto_rollback", b"auto_rollback", "base_template", b"base_template", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "parameter_values", b"parameter_values", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "auto_rollback", b"auto_rollback", "base_template", b"base_template", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["auto_rollback", b"auto_rollback", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "parameter_values", b"parameter_values", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "auto_rollback", b"auto_rollback", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "constants", b"constants", "delivery_config", b"delivery_config", "delivery_extension_instances", b"delivery_extension_instances", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "env", b"env", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "name", b"name", "no_cleanup_on_delete", b"no_cleanup_on_delete", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "external_config", "helm"] | None: ...
 
 global___ServiceConfig = ServiceConfig
 
 class CompiledServiceInstanceConfig(google.protobuf.message.Message):
     """a compiled version of ServiceConfig specific to a service instance, with release-channel configs applied"""
 
@@ -690,25 +776,28 @@
     CERT_FIELD_NUMBER: builtins.int
     RUNTIME_FIELD_NUMBER: builtins.int
     RUNTIME_EXECUTION_FIELD_NUMBER: builtins.int
     CAPABILITIES_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     DEPLOY_ANNOTATIONS_FIELD_NUMBER: builtins.int
-    BASE_TEMPLATE_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
     DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSION_INSTANCES_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
+    CONSTANTS_FIELD_NUMBER: builtins.int
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     ENV_FIELD_NUMBER: builtins.int
+    NO_CLEANUP_ON_DELETE_FIELD_NUMBER: builtins.int
+    PROTECTIONS_FIELD_NUMBER: builtins.int
     service: builtins.str
     application: builtins.str
     release_channel: builtins.str
     @property
     def programs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig]: ...
     @property
     def replicas(self) -> global___ReplicasConfig: ...
@@ -728,40 +817,46 @@
     @property
     def delivery_config(self) -> prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig: ...
     @property
     def volumes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.volumes.volumes_pb2.Volume]: ...
     @property
     def deploy_annotations(self) -> prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig: ...
     @property
-    def base_template(self) -> prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef: ...
-    @property
     def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]:
         """DEPRECATED: Replace with delivery_extensions once its implemented."""
     @property
     def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionConfig]: ...
     @property
+    def delivery_extension_instances(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionInstance]: ...
+    @property
     def runtime_specific(self) -> global___RuntimeSpecificConfig: ...
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
     @property
     def parameter_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]: ...
     @property
+    def constants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.constants_pb2.Constant]:
+        """constants made available in template substitutions"""
+    @property
     def progress_deadline(self) -> google.protobuf.duration_pb2.Duration:
         """how long to wait before marking deployment as failed"""
     @property
     def runtime_extension(self) -> global___RuntimeExtensionConfig: ...
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def helm(self) -> prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig: ...
     @property
     def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
         """The compiled environment for this instance's context, e.g.  Release Channel.
         This is used to inject these values into external configs.
         """
+    no_cleanup_on_delete: builtins.bool
+    @property
+    def protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]: ...
     def __init__(
         self,
         *,
         service: builtins.str = ...,
         application: builtins.str = ...,
         release_channel: builtins.str = ...,
         programs: collections.abc.Iterable[prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig] | None = ...,
@@ -772,28 +867,31 @@
         cert: global___Certificate | None = ...,
         runtime: prodvana.proto.prodvana.release_channel.release_channel_config_pb2.ReleaseChannelRuntimeConfig | None = ...,
         runtime_execution: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig | None = ...,
         capabilities: collections.abc.Iterable[global___CompiledCapabilityConfig] | None = ...,
         delivery_config: prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig | None = ...,
         volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         deploy_annotations: prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig | None = ...,
-        base_template: prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
         delivery_extensions: collections.abc.Iterable[global___DeliveryExtensionConfig] | None = ...,
+        delivery_extension_instances: collections.abc.Iterable[global___DeliveryExtensionInstance] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         parameter_values: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
+        constants: collections.abc.Iterable[prodvana.proto.prodvana.common_config.constants_pb2.Constant] | None = ...,
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
         runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
         env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
+        no_cleanup_on_delete: builtins.bool = ...,
+        protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["base_template", b"base_template", "cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "base_template", b"base_template", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "env", b"env", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "maturity", b"maturity", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "constants", b"constants", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "delivery_extension_instances", b"delivery_extension_instances", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "env", b"env", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "maturity", b"maturity", "no_cleanup_on_delete", b"no_cleanup_on_delete", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "protections", b"protections", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "helm"] | None: ...
 
 global___CompiledServiceInstanceConfig = CompiledServiceInstanceConfig
 
 class CompiledJobConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
-import collections.abc
 import google.protobuf.descriptor
-import google.protobuf.internal.containers
 import google.protobuf.message
-import prodvana.proto.prodvana.common_config.links_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class ServiceUserMetadata(google.protobuf.message.Message):
+class Constant(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DESCRIPTION_FIELD_NUMBER: builtins.int
-    LINKS_FIELD_NUMBER: builtins.int
-    FOLLOW_REPOSITORY_FIELD_NUMBER: builtins.int
-    description: builtins.str
+    NAME_FIELD_NUMBER: builtins.int
+    STRING_FIELD_NUMBER: builtins.int
+    name: builtins.str
+    """constant name, used in substitutions"""
     @property
-    def links(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.links_pb2.Link]: ...
-    @property
-    def follow_repository(self) -> global___FollowContainerRepositorySettings: ...
+    def string(self) -> global___StringConstant: ...
     def __init__(
         self,
         *,
-        description: builtins.str = ...,
-        links: collections.abc.Iterable[prodvana.proto.prodvana.common_config.links_pb2.Link] | None = ...,
-        follow_repository: global___FollowContainerRepositorySettings | None = ...,
+        name: builtins.str = ...,
+        string: global___StringConstant | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["follow_repository", b"follow_repository"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "follow_repository", b"follow_repository", "links", b"links"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["config_oneof", b"config_oneof", "string", b"string"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["config_oneof", b"config_oneof", "name", b"name", "string", b"string"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["string"] | None: ...
 
-global___ServiceUserMetadata = ServiceUserMetadata
+global___Constant = Constant
 
-class FollowContainerRepositorySettings(google.protobuf.message.Message):
+class StringConstant(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ENABLED_FIELD_NUMBER: builtins.int
-    enabled: builtins.bool
+    VALUE_FIELD_NUMBER: builtins.int
+    value: builtins.str
     def __init__(
         self,
         *,
-        enabled: builtins.bool = ...,
+        value: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["enabled", b"enabled"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
 
-global___FollowContainerRepositorySettings = FollowContainerRepositorySettings
+global___StringConstant = StringConstant
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,171 +1,112 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
-import collections.abc
 import google.protobuf.descriptor
-import google.protobuf.internal.containers
 import google.protobuf.message
-import prodvana.proto.prodvana.users.users_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class SettingsUser(google.protobuf.message.Message):
+class AlertingConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    USER_FIELD_NUMBER: builtins.int
-    ROLES_FIELD_NUMBER: builtins.int
-    @property
-    def user(self) -> prodvana.proto.prodvana.users.users_pb2.User: ...
-    @property
-    def roles(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    def __init__(
-        self,
-        *,
-        user: prodvana.proto.prodvana.users.users_pb2.User | None = ...,
-        roles: collections.abc.Iterable[builtins.str] | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["user", b"user"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["roles", b"roles", "user", b"user"]) -> None: ...
-
-global___SettingsUser = SettingsUser
-
-class GetUserReq(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    USER_ID_FIELD_NUMBER: builtins.int
-    user_id: builtins.str
-    def __init__(
-        self,
-        *,
-        user_id: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["user_id", b"user_id"]) -> None: ...
+    class PagerDuty(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-global___GetUserReq = GetUserReq
+        SERVICE_FIELD_NUMBER: builtins.int
+        service: builtins.str
+        def __init__(
+            self,
+            *,
+            service: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["service", b"service"]) -> None: ...
 
-class GetUserResp(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    USER_FIELD_NUMBER: builtins.int
+    PAGERDUTY_FIELD_NUMBER: builtins.int
     @property
-    def user(self) -> global___SettingsUser: ...
+    def pagerduty(self) -> global___AlertingConfig.PagerDuty: ...
     def __init__(
         self,
         *,
-        user: global___SettingsUser | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["user", b"user"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["user", b"user"]) -> None: ...
-
-global___GetUserResp = GetUserResp
-
-class ListRolesReq(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    def __init__(
-        self,
+        pagerduty: global___AlertingConfig.PagerDuty | None = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["pagerduty", b"pagerduty"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pagerduty", b"pagerduty"]) -> None: ...
 
-global___ListRolesReq = ListRolesReq
+global___AlertingConfig = AlertingConfig
 
-class RoleDefinition(google.protobuf.message.Message):
+class AnnotationsConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    NAME_FIELD_NUMBER: builtins.int
-    DESCRIPTION_FIELD_NUMBER: builtins.int
-    name: builtins.str
-    description: builtins.str
-    def __init__(
-        self,
-        *,
-        name: builtins.str = ...,
-        description: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "name", b"name"]) -> None: ...
+    class Honeycomb(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-global___RoleDefinition = RoleDefinition
+        ENVIRONMENT_FIELD_NUMBER: builtins.int
+        DATASET_FIELD_NUMBER: builtins.int
+        environment: builtins.str
+        dataset: builtins.str
+        def __init__(
+            self,
+            *,
+            environment: builtins.str = ...,
+            dataset: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["dataset", b"dataset", "environment", b"environment"]) -> None: ...
 
-class ListRolesResp(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    ROLES_FIELD_NUMBER: builtins.int
+    HONEYCOMB_FIELD_NUMBER: builtins.int
     @property
-    def roles(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RoleDefinition]: ...
+    def honeycomb(self) -> global___AnnotationsConfig.Honeycomb: ...
     def __init__(
         self,
         *,
-        roles: collections.abc.Iterable[global___RoleDefinition] | None = ...,
+        honeycomb: global___AnnotationsConfig.Honeycomb | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["roles", b"roles"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["honeycomb", b"honeycomb"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["honeycomb", b"honeycomb"]) -> None: ...
 
-global___ListRolesResp = ListRolesResp
+global___AnnotationsConfig = AnnotationsConfig
 
-class ListUsersReq(google.protobuf.message.Message):
+class TokenConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PAGE_TOKEN_FIELD_NUMBER: builtins.int
-    PAGE_SIZE_FIELD_NUMBER: builtins.int
-    page_token: builtins.str
-    page_size: builtins.int
+    TOKEN_SECRET_KEY_FIELD_NUMBER: builtins.int
+    TOKEN_SECRET_VERSION_FIELD_NUMBER: builtins.int
+    token_secret_key: builtins.str
+    token_secret_version: builtins.str
     def __init__(
         self,
         *,
-        page_token: builtins.str = ...,
-        page_size: builtins.int = ...,
+        token_secret_key: builtins.str = ...,
+        token_secret_version: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["page_size", b"page_size", "page_token", b"page_token"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["token_secret_key", b"token_secret_key", "token_secret_version", b"token_secret_version"]) -> None: ...
 
-global___ListUsersReq = ListUsersReq
+global___TokenConfig = TokenConfig
 
-class ListUsersResp(google.protobuf.message.Message):
+class IntegrationConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    USERS_FIELD_NUMBER: builtins.int
-    NEXT_PAGE_TOKEN_FIELD_NUMBER: builtins.int
+    SLACK_CONFIG_FIELD_NUMBER: builtins.int
+    PAGERDUTY_CONFIG_FIELD_NUMBER: builtins.int
     @property
-    def users(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SettingsUser]: ...
-    next_page_token: builtins.str
-    def __init__(
-        self,
-        *,
-        users: collections.abc.Iterable[global___SettingsUser] | None = ...,
-        next_page_token: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["next_page_token", b"next_page_token", "users", b"users"]) -> None: ...
-
-global___ListUsersResp = ListUsersResp
-
-class SetRolesReq(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    USER_ID_FIELD_NUMBER: builtins.int
-    ROLES_FIELD_NUMBER: builtins.int
-    user_id: builtins.str
+    def slack_config(self) -> global___TokenConfig: ...
     @property
-    def roles(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    def pagerduty_config(self) -> global___TokenConfig: ...
     def __init__(
         self,
         *,
-        user_id: builtins.str = ...,
-        roles: collections.abc.Iterable[builtins.str] | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["roles", b"roles", "user_id", b"user_id"]) -> None: ...
-
-global___SetRolesReq = SetRolesReq
-
-class SetRolesResp(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    def __init__(
-        self,
+        slack_config: global___TokenConfig | None = ...,
+        pagerduty_config: global___TokenConfig | None = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["config_oneof", b"config_oneof", "pagerduty_config", b"pagerduty_config", "slack_config", b"slack_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["config_oneof", b"config_oneof", "pagerduty_config", b"pagerduty_config", "slack_config", b"slack_config"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["slack_config", "pagerduty_config"] | None: ...
 
-global___SetRolesResp = SetRolesResp
+global___IntegrationConfig = IntegrationConfig
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/template/service_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/template/service.proto
+# source: prodvana/common_config/meta.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.object import meta_pb2 as prodvana_dot_object_dot_meta__pb2
-from prodvana.proto.prodvana.service import service_config_pb2 as prodvana_dot_service_dot_service__config__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fprodvana/template/service.proto\x12\x11prodvana.template\x1a\x1aprodvana/object/meta.proto\x1a%prodvana/service/service_config.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\"\xba\x01\n\x0fServiceTemplate\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x39\n\x15last_update_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x0eservice_config\x18\x03 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfigB\x08\xfa\x42\x05\x8a\x01\x02\x08\x01\x42MZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/templateb\x06proto3')
-
-
-
-_SERVICETEMPLATE = DESCRIPTOR.message_types_by_name['ServiceTemplate']
-ServiceTemplate = _reflection.GeneratedProtocolMessageType('ServiceTemplate', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICETEMPLATE,
-  '__module__' : 'prodvana.template.service_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.template.ServiceTemplate)
-  })
-_sym_db.RegisterMessage(ServiceTemplate)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/common_config/meta.proto\x12\x16prodvana.common_config\x1a\x1aprodvana/object/meta.proto\"\x89\x01\n\x19ServiceInstanceObjectMeta\x12\x31\n\x0cservice_meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x39\n\x14release_channel_meta\x18\x02 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\"]\n\x15PipelineRunObjectMeta\x12\x32\n\rpipeline_meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x10\n\x08run_name\x18\x02 \x01(\tBRZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.common_config.meta_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/template'
-  _SERVICETEMPLATE.fields_by_name['service_config']._options = None
-  _SERVICETEMPLATE.fields_by_name['service_config']._serialized_options = b'\372B\005\212\001\002\010\001'
-  _SERVICETEMPLATE._serialized_start=180
-  _SERVICETEMPLATE._serialized_end=366
+  DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
+  _globals['_SERVICEINSTANCEOBJECTMETA']._serialized_start=90
+  _globals['_SERVICEINSTANCEOBJECTMETA']._serialized_end=227
+  _globals['_PIPELINERUNOBJECTMETA']._serialized_start=229
+  _globals['_PIPELINERUNOBJECTMETA']._serialized_end=322
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/users/users.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aprodvana/users/users.proto\x12\x0eprodvana.users\"\\\n\x04User\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x0e\n\x06\x65mails\x18\x05 \x03(\tBJZHgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/usersb\x06proto3')
 
-
-
-_USER = DESCRIPTOR.message_types_by_name['User']
-User = _reflection.GeneratedProtocolMessageType('User', (_message.Message,), {
-  'DESCRIPTOR' : _USER,
-  '__module__' : 'prodvana.users.users_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.users.User)
-  })
-_sym_db.RegisterMessage(User)
-
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.users.users_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZHgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/users'
-  _USER._serialized_start=46
-  _USER._serialized_end=138
+  _globals['_USER']._serialized_start=46
+  _globals['_USER']._serialized_end=138
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -27,26 +27,30 @@
     INTERACTIVE_PVNCTL: _Source.ValueType  # 2
     CONFIG_FILE: _Source.ValueType  # 3
     REPO_FOLLOW: _Source.ValueType  # 4
     PRODVANA: _Source.ValueType  # 5
     """this source indicates this version was provided by Prodvana
     this is used for things like builtin Protections or other first party provided features
     """
+    IAC: _Source.ValueType  # 6
+    """Infra as Code sources like Terraform and Pulumi"""
 
 class Source(_Source, metaclass=_SourceEnumTypeWrapper): ...
 
 UNKNOWN_SOURCE: Source.ValueType  # 0
 WEB: Source.ValueType  # 1
 INTERACTIVE_PVNCTL: Source.ValueType  # 2
 CONFIG_FILE: Source.ValueType  # 3
 REPO_FOLLOW: Source.ValueType  # 4
 PRODVANA: Source.ValueType  # 5
 """this source indicates this version was provided by Prodvana
 this is used for things like builtin Protections or other first party provided features
 """
+IAC: Source.ValueType  # 6
+"""Infra as Code sources like Terraform and Pulumi"""
 global___Source = Source
 
 class SourceMetadata(google.protobuf.message.Message):
     """all of these fields are optional and only set if it makes sense for a given source."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.2.0/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/utils/desired_states.py` & `prodvana-0.2.0/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/utils/service_config.py` & `prodvana-0.2.0/prodvana/utils/service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/prodvana/utils/tests/test_service_config.py` & `prodvana-0.2.0/prodvana/utils/tests/test_service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.9/pyproject.toml` & `prodvana-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.1.9"
+version = "0.2.0"
 description = "Prodvana's client libraries"
 readme = "README.md"
 authors = []
 homepage = "https://prodvana.io"
 documentation = "https://docs.prodvana.io"
 repository = "https://github.com/prodvana/prodvana-public"
 exclude = ["examples"]
```

### Comparing `prodvana-0.1.9/PKG-INFO` & `prodvana-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.1.9
+Version: 0.2.0
 Summary: Prodvana's client libraries
 Home-page: https://prodvana.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
```

