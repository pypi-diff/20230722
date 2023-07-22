# Comparing `tmp/omni-pro-0.1.18.tar.gz` & `tmp/omni-pro-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omni-pro-0.1.18.tar", last modified: Wed Jul 19 20:32:14 2023, max compression
+gzip compressed data, was "omni-pro-0.1.19.tar", last modified: Fri Jul 21 16:17:57 2023, max compression
```

## Comparing `omni-pro-0.1.18.tar` & `omni-pro-0.1.19.tar`

### file list

```diff
@@ -1,347 +1,344 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.214300 omni-pro-0.1.18/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-19 20:31:42.000000 omni-pro-0.1.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-19 20:32:14.210300 omni-pro-0.1.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-19 20:31:42.000000 omni-pro-0.1.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.122300 omni-pro-0.1.18/omni/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.122300 omni-pro-0.1.18/omni/pro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/cloudmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.126300 omni-pro-0.1.18/omni/pro/data/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/data/models.user.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.126300 omni-pro-0.1.18/omni/pro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.126300 omni-pro-0.1.18/omni/pro/models/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/common/ms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.126300 omni-pro-0.1.18/omni/pro/models/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.126300 omni-pro-0.1.18/omni/pro/models/sql/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/catalog/category.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.126300 omni-pro-0.1.18/omni/pro/models/sql/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/common/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.130300 omni-pro-0.1.18/omni/pro/models/sql/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_category_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_locality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_method_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_method_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/schedule_work.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/rules/warehouse_hierarchy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.130300 omni-pro-0.1.18/omni/pro/models/sql/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/stock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.130300 omni-pro-0.1.18/omni/pro/models/sql/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/utilities/country.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/utilities/territory_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/sql/utilities/territory_matrix_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.134300 omni-pro-0.1.18/omni/pro/models/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/carrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/picking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/picking_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/procurement_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/uom.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/stock/warehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.134300 omni-pro-0.1.18/omni/pro/models/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/models/utilities/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.134300 omni-pro-0.1.18/omni/pro/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.134300 omni-pro-0.1.18/omni/pro/protos/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/common/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/common/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/common/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/grpc_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.134300 omni-pro-0.1.18/omni/pro/protos/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.138300 omni-pro-0.1.18/omni/pro/protos/v1/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/catalogs/family_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/catalogs/family_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/catalogs/template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/catalogs/template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.138300 omni-pro-0.1.18/omni/pro/protos/v1/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/clients/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/clients/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/clients/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/clients/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/clients/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/clients/client_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.166300 omni-pro-0.1.18/omni/pro/protos/v1/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/calendar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/calendar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/location_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/location_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/location_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.182300 omni-pro-0.1.18/omni/pro/protos/v1/sales/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/carrier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/carrier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/channel_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/client_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/order_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/order_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/product_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/product_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/product_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/sale_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/sale_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/sale_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.198300 omni-pro-0.1.18/omni/pro/protos/v1/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/attachment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/attachment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/attachment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/carrier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/carrier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/carrier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/location_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/location_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/location_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/procurement_group_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/procurement_group_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/product_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/product_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/product_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/quant_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/quant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/quant_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/route_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/route_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/route_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/rule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/rule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/rule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.198300 omni-pro-0.1.18/omni/pro/protos/v1/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20954 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/users/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27451 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/users/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    33602 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/users/user_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.210300 omni-pro-0.1.18/omni/pro/protos/v1/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/document_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/document_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/language_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/language_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/language_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/model_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/timezone_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/timezone_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/protos/v1/utilities/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.210300 omni-pro-0.1.18/omni/pro/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/user/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-19 20:31:42.000000 omni-pro-0.1.18/omni/pro/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 20:32:14.210300 omni-pro-0.1.18/omni_pro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-19 20:32:14.000000 omni-pro-0.1.18/omni_pro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-07-19 20:32:14.000000 omni-pro-0.1.18/omni_pro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 20:32:14.000000 omni-pro-0.1.18/omni_pro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-19 20:32:14.000000 omni-pro-0.1.18/omni_pro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 20:32:14.000000 omni-pro-0.1.18/omni_pro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 20:32:14.214300 omni-pro-0.1.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-19 20:32:05.000000 omni-pro-0.1.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:57.000070 omni-pro-0.1.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-21 16:17:23.000000 omni-pro-0.1.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-21 16:17:57.000070 omni-pro-0.1.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-21 16:17:23.000000 omni-pro-0.1.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.896067 omni-pro-0.1.19/omni/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.896067 omni-pro-0.1.19/omni/pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/cloudmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.900068 omni-pro-0.1.19/omni/pro/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/data/models.user.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.900068 omni-pro-0.1.19/omni/pro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.900068 omni-pro-0.1.19/omni/pro/models/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/common/ms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.900068 omni-pro-0.1.19/omni/pro/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.900068 omni-pro-0.1.19/omni/pro/models/sql/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/catalog/category.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.900068 omni-pro-0.1.19/omni/pro/models/sql/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/common/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.904068 omni-pro-0.1.19/omni/pro/models/sql/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_category_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_locality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_method_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_method_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/schedule_work.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/rules/warehouse_hierarchy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.904068 omni-pro-0.1.19/omni/pro/models/sql/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/stock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.904068 omni-pro-0.1.19/omni/pro/models/sql/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/utilities/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/utilities/territory_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/sql/utilities/territory_matrix_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.908068 omni-pro-0.1.19/omni/pro/models/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/carrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/picking_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/procurement_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/uom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/stock/warehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.908068 omni-pro-0.1.19/omni/pro/models/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/models/utilities/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.908068 omni-pro-0.1.19/omni/pro/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.912068 omni-pro-0.1.19/omni/pro/protos/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/common/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/common/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/common/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/grpc_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.912068 omni-pro-0.1.19/omni/pro/protos/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.912068 omni-pro-0.1.19/omni/pro/protos/v1/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/catalogs/family_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/catalogs/family_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/catalogs/template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/catalogs/template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.912068 omni-pro-0.1.19/omni/pro/protos/v1/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/clients/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/clients/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/clients/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/clients/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/clients/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/clients/client_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.936069 omni-pro-0.1.19/omni/pro/protos/v1/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/calendar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/calendar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/location_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/location_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/location_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.952069 omni-pro-0.1.19/omni/pro/protos/v1/sales/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/carrier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/carrier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/channel_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/client_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/order_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/order_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/product_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/product_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/product_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/sale_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/sale_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/sale_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.976070 omni-pro-0.1.19/omni/pro/protos/v1/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/attachment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/attachment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/attachment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/carrier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/carrier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/carrier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/location_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/location_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/location_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/procurement_group_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/procurement_group_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/product_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/product_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/product_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/quant_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/quant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/quant_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/route_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/route_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/route_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/rule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/rule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/rule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.980070 omni-pro-0.1.19/omni/pro/protos/v1/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/users/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27451 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/users/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    33602 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/users/user_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.996070 omni-pro-0.1.19/omni/pro/protos/v1/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/document_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/document_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/language_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/language_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/language_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/model_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/timezone_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/timezone_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/protos/v1/utilities/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.996070 omni-pro-0.1.19/omni/pro/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/user/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-21 16:17:23.000000 omni-pro-0.1.19/omni/pro/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:17:56.996070 omni-pro-0.1.19/omni_pro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-21 16:17:56.000000 omni-pro-0.1.19/omni_pro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-07-21 16:17:56.000000 omni-pro-0.1.19/omni_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:17:56.000000 omni-pro-0.1.19/omni_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 16:17:56.000000 omni-pro-0.1.19/omni_pro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 16:17:56.000000 omni-pro-0.1.19/omni_pro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:17:57.000070 omni-pro-0.1.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-21 16:17:48.000000 omni-pro-0.1.19/setup.py
```

### Comparing `omni-pro-0.1.18/LICENSE` & `omni-pro-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/PKG-INFO` & `omni-pro-0.1.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.1.18
+Version: 0.1.19
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.1.18/README.md` & `omni-pro-0.1.19/README.md`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/aws.py` & `omni-pro-0.1.19/omni/pro/aws.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/cloudmap.py` & `omni-pro-0.1.19/omni/pro/cloudmap.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/config.py` & `omni-pro-0.1.19/omni/pro/config.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/database.py` & `omni-pro-0.1.19/omni/pro/database.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/decorators.py` & `omni-pro-0.1.19/omni/pro/decorators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/initial.py` & `omni-pro-0.1.19/omni/pro/initial.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/logger.py` & `omni-pro-0.1.19/omni/pro/logger.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/base.py` & `omni-pro-0.1.19/omni/pro/models/base.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/common/country.py` & `omni-pro-0.1.19/omni/pro/models/sql/common/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_category.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_category_category.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_category_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_locality.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_locality.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_method.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_method.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_method_ref.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_method_ref.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_method_warehouse.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_method_warehouse.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/delivery_schedule.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/delivery_schedule.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/schedule_work.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/schedule_work.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/schedule_work_line.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/sql/rules/warehouse_hierarchy.py` & `omni-pro-0.1.19/omni/pro/models/sql/rules/warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/stock/attachment.py` & `omni-pro-0.1.19/omni/pro/models/stock/attachment.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/stock/location.py` & `omni-pro-0.1.19/omni/pro/models/stock/location.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/stock/picking.py` & `omni-pro-0.1.19/omni/pro/models/stock/picking.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/stock/picking_type.py` & `omni-pro-0.1.19/omni/pro/models/stock/picking_type.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/stock/procurement_group.py` & `omni-pro-0.1.19/omni/pro/models/stock/procurement_group.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/stock/product.py` & `omni-pro-0.1.19/omni/pro/models/stock/product.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/stock/uom.py` & `omni-pro-0.1.19/omni/pro/models/stock/uom.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/stock/user.py` & `omni-pro-0.1.19/omni/pro/models/stock/user.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/stock/warehouse.py` & `omni-pro-0.1.19/omni/pro/models/stock/warehouse.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/models/utilities/country.py` & `omni-pro-0.1.19/omni/pro/models/utilities/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/common/base_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/common/base_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/common/base_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/common/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/grpc_connector.py` & `omni-pro-0.1.19/omni/pro/protos/grpc_connector.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/response.py` & `omni-pro-0.1.19/omni/pro/protos/response.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/util.py` & `omni-pro-0.1.19/omni/pro/protos/util.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/catalogs/family_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/catalogs/family_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/catalogs/family_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/catalogs/family_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/catalogs/family_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/catalogs/family_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/catalogs/template_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/catalogs/template_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/catalogs/template_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/catalogs/template_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from common import base_pb2 as _base_pb2
-from v1.catalogs import family_pb2 as _family_pb2
+from typing import ClassVar as _ClassVar
+from typing import Iterable as _Iterable
+from typing import Mapping as _Mapping
+from typing import Optional as _Optional
+from typing import Union as _Union
+
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
 from google.protobuf import struct_pb2 as _struct_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from omni.pro.protos.common import base_pb2 as _base_pb2
+from omni.pro.protos.v1.catalogs import family_pb2 as _family_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ProductTemplate(_message.Message):
     __slots__ = ["id", "code", "name", "family", "attribute_values", "active"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
@@ -19,37 +24,56 @@
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     id: str
     code: str
     name: str
     family: _family_pb2.Family
     attribute_values: _struct_pb2.Struct
     active: _wrappers_pb2.BoolValue
-    def __init__(self, id: _Optional[str] = ..., code: _Optional[str] = ..., name: _Optional[str] = ..., family: _Optional[_Union[_family_pb2.Family, _Mapping]] = ..., attribute_values: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        id: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        family: _Optional[_Union[_family_pb2.Family, _Mapping]] = ...,
+        attribute_values: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductTemplateCreateRequest(_message.Message):
     __slots__ = ["code", "name", "family_id", "attribute_values", "context"]
     CODE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     FAMILY_ID_FIELD_NUMBER: _ClassVar[int]
     ATTRIBUTE_VALUES_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     code: str
     name: str
     family_id: str
     attribute_values: _struct_pb2.Struct
     context: _base_pb2.Context
-    def __init__(self, code: _Optional[str] = ..., name: _Optional[str] = ..., family_id: _Optional[str] = ..., attribute_values: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        code: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        family_id: _Optional[str] = ...,
+        attribute_values: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductTemplateCreateResponse(_message.Message):
     __slots__ = ["response_standard", "product_template"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_TEMPLATE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     product_template: ProductTemplate
-    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ..., product_template: _Optional[_Union[ProductTemplate, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        product_template: _Optional[_Union[ProductTemplate, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductTemplateReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
@@ -59,49 +83,73 @@
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
     id: str
     context: _base_pb2.Context
-    def __init__(self, group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ..., sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ..., fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ..., filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ..., paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ..., id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
+        sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
+        fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
+        filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
+        paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
+        id: _Optional[str] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductTemplateReadResponse(_message.Message):
     __slots__ = ["response_standard", "product_templates", "meta_data"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_TEMPLATES_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     product_templates: _containers.RepeatedCompositeFieldContainer[ProductTemplate]
     meta_data: _base_pb2.MetaData
-    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ..., product_templates: _Optional[_Iterable[_Union[ProductTemplate, _Mapping]]] = ..., meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        product_templates: _Optional[_Iterable[_Union[ProductTemplate, _Mapping]]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductTemplateUpdateRequest(_message.Message):
     __slots__ = ["product_template", "context"]
     PRODUCT_TEMPLATE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     product_template: ProductTemplate
     context: _base_pb2.Context
-    def __init__(self, product_template: _Optional[_Union[ProductTemplate, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        product_template: _Optional[_Union[ProductTemplate, _Mapping]] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductTemplateUpdateResponse(_message.Message):
     __slots__ = ["response_standard", "product_template"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_TEMPLATE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     product_template: ProductTemplate
-    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ..., product_template: _Optional[_Union[ProductTemplate, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        product_template: _Optional[_Union[ProductTemplate, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductTemplateDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
-    def __init__(self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+    ) -> None: ...
 
 class ProductTemplateDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
 
@@ -115,37 +163,56 @@
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     id: str
     code: str
     name: str
     product_template_id: str
     attribute_values: _struct_pb2.Struct
     active: _wrappers_pb2.BoolValue
-    def __init__(self, id: _Optional[str] = ..., code: _Optional[str] = ..., name: _Optional[str] = ..., product_template_id: _Optional[str] = ..., attribute_values: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        id: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        product_template_id: _Optional[str] = ...,
+        attribute_values: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductCreateRequest(_message.Message):
     __slots__ = ["code", "name", "product_template_id", "attribute_values", "context"]
     CODE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_TEMPLATE_ID_FIELD_NUMBER: _ClassVar[int]
     ATTRIBUTE_VALUES_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     code: str
     name: str
     product_template_id: str
     attribute_values: _struct_pb2.Struct
     context: _base_pb2.Context
-    def __init__(self, code: _Optional[str] = ..., name: _Optional[str] = ..., product_template_id: _Optional[str] = ..., attribute_values: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        code: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        product_template_id: _Optional[str] = ...,
+        attribute_values: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductCreateResponse(_message.Message):
     __slots__ = ["response_standard", "product"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     product: Product
-    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ..., product: _Optional[_Union[Product, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        product: _Optional[_Union[Product, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
@@ -155,49 +222,73 @@
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
     id: str
     context: _base_pb2.Context
-    def __init__(self, group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ..., sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ..., fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ..., filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ..., paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ..., id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
+        sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
+        fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
+        filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
+        paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
+        id: _Optional[str] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductReadResponse(_message.Message):
     __slots__ = ["response_standard", "products", "meta_data"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     PRODUCTS_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     products: _containers.RepeatedCompositeFieldContainer[Product]
     meta_data: _base_pb2.MetaData
-    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ..., products: _Optional[_Iterable[_Union[Product, _Mapping]]] = ..., meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        products: _Optional[_Iterable[_Union[Product, _Mapping]]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductUpdateRequest(_message.Message):
     __slots__ = ["product", "context"]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     product: Product
     context: _base_pb2.Context
-    def __init__(self, product: _Optional[_Union[Product, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        product: _Optional[_Union[Product, _Mapping]] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductUpdateResponse(_message.Message):
     __slots__ = ["response_standard", "product"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     product: Product
-    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ..., product: _Optional[_Union[Product, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        product: _Optional[_Union[Product, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
-    def __init__(self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+    ) -> None: ...
 
 class ProductDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
 
@@ -213,15 +304,24 @@
     id: str
     code: str
     name: str
     type: str
     img_url: str
     product_template_id: str
     product_id: str
-    def __init__(self, id: _Optional[str] = ..., code: _Optional[str] = ..., name: _Optional[str] = ..., type: _Optional[str] = ..., img_url: _Optional[str] = ..., product_template_id: _Optional[str] = ..., product_id: _Optional[str] = ...) -> None: ...
+    def __init__(
+        self,
+        id: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        type: _Optional[str] = ...,
+        img_url: _Optional[str] = ...,
+        product_template_id: _Optional[str] = ...,
+        product_id: _Optional[str] = ...,
+    ) -> None: ...
 
 class ProductAllReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
@@ -229,18 +329,31 @@
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
     context: _base_pb2.Context
-    def __init__(self, group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ..., sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ..., fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ..., filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ..., paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
+        sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
+        fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
+        filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
+        paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+    ) -> None: ...
 
 class ProductAllReadResponse(_message.Message):
     __slots__ = ["response_standard", "product_all", "meta_data"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_ALL_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     product_all: _containers.RepeatedCompositeFieldContainer[ProductAll]
     meta_data: _base_pb2.MetaData
-    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ..., product_all: _Optional[_Iterable[_Union[ProductAll, _Mapping]]] = ..., meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...) -> None: ...
+    def __init__(
+        self,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        product_all: _Optional[_Iterable[_Union[ProductAll, _Mapping]]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+    ) -> None: ...
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/catalogs/template_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/catalogs/template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/clients/address_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/clients/address_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/clients/address_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/clients/address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/clients/address_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/clients/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/clients/client_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/clients/client_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/clients/client_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/clients/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/clients/client_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/clients/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/calendar_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/calendar_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/calendar_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/calendar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/calendar_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/calendar_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/category_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/category_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/category_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_category_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,41 +11,40 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 from omni.pro.protos.v1.rules import delivery_method_pb2 as v1_dot_rules_dot_delivery__method__pb2
 from omni.pro.protos.v1.rules import warehouse_pb2 as v1_dot_rules_dot_warehouse__pb2
-from omni.pro.protos.v1.stock import stock_pb2 as v1_dot_stock_dot_stock__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1dv1/rules/delivery_price.proto\x12(pro.omni.oms.api.v1.rules.delivery_price\x1a\x11\x63ommon/base.proto\x1a\x1ev1/rules/delivery_method.proto\x1a\x14v1/stock/stock.proto\x1a\x18v1/rules/warehouse.proto"\xb8\x03\n\rDeliveryPrice\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12V\n\x13\x64\x65livery_method_ids\x18\x03 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x45\n\rwarehouse_ids\x18\x04 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x1d\n\x15locality_available_id\x18\x05 \x01(\t\x12\x45\n\ttime_type\x18\x06 \x01(\x0e\x32\x32.pro.omni.oms.api.v1.rules.delivery_price.TimeType\x12\x11\n\tvalue_min\x18\x07 \x01(\t\x12\x11\n\tvalue_max\x18\x08 \x01(\t\x12\x11\n\tinversely\x18\t \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12?\n\x0cobject_audit\x18\x0b \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x81\x02\n\x1a\x44\x65liveryPriceCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\x15locality_available_id\x18\x02 \x01(\t\x12\x45\n\ttime_type\x18\x03 \x01(\x0e\x32\x32.pro.omni.oms.api.v1.rules.delivery_price.TimeType\x12\x11\n\tvalue_min\x18\x04 \x01(\t\x12\x11\n\tvalue_max\x18\x05 \x01(\t\x12\x11\n\tinversely\x18\x06 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb9\x01\n\x1b\x44\x65liveryPriceCreateResponse\x12O\n\x0e\x64\x65livery_price\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPrice\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf6\x02\n\x18\x44\x65liveryPriceReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf3\x01\n\x19\x44\x65liveryPriceReadResponse\x12P\n\x0f\x64\x65livery_prices\x18\x01 \x03(\x0b\x32\x37.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPrice\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa5\x01\n\x1a\x44\x65liveryPriceUpdateRequest\x12O\n\x0e\x64\x65livery_price\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPrice\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb9\x01\n\x1b\x44\x65liveryPriceUpdateResponse\x12O\n\x0e\x64\x65livery_price\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPrice\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"`\n\x1a\x44\x65liveryPriceDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1b\x44\x65liveryPriceDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*9\n\x08TimeType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MINUTES\x10\x01\x12\t\n\x05HOURS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x32\xac\x05\n\x14\x44\x65liveryPriceService\x12\xa4\x01\n\x13\x44\x65liveryPriceCreate\x12\x44.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceCreateRequest\x1a\x45.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceCreateResponse"\x00\x12\x9e\x01\n\x11\x44\x65liveryPriceRead\x12\x42.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceReadRequest\x1a\x43.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceReadResponse"\x00\x12\xa4\x01\n\x13\x44\x65liveryPriceUpdate\x12\x44.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceUpdateRequest\x1a\x45.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceUpdateResponse"\x00\x12\xa4\x01\n\x13\x44\x65liveryPriceDelete\x12\x44.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceDeleteRequest\x1a\x45.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1dv1/rules/delivery_price.proto\x12(pro.omni.oms.api.v1.rules.delivery_price\x1a\x11\x63ommon/base.proto\x1a\x1ev1/rules/delivery_method.proto\x1a\x18v1/rules/warehouse.proto"\xb8\x03\n\rDeliveryPrice\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12V\n\x13\x64\x65livery_method_ids\x18\x03 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x45\n\rwarehouse_ids\x18\x04 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x1d\n\x15locality_available_id\x18\x05 \x01(\t\x12\x45\n\ttime_type\x18\x06 \x01(\x0e\x32\x32.pro.omni.oms.api.v1.rules.delivery_price.TimeType\x12\x11\n\tvalue_min\x18\x07 \x01(\t\x12\x11\n\tvalue_max\x18\x08 \x01(\t\x12\x11\n\tinversely\x18\t \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12?\n\x0cobject_audit\x18\x0b \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x81\x02\n\x1a\x44\x65liveryPriceCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\x15locality_available_id\x18\x02 \x01(\t\x12\x45\n\ttime_type\x18\x03 \x01(\x0e\x32\x32.pro.omni.oms.api.v1.rules.delivery_price.TimeType\x12\x11\n\tvalue_min\x18\x04 \x01(\t\x12\x11\n\tvalue_max\x18\x05 \x01(\t\x12\x11\n\tinversely\x18\x06 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb9\x01\n\x1b\x44\x65liveryPriceCreateResponse\x12O\n\x0e\x64\x65livery_price\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPrice\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf6\x02\n\x18\x44\x65liveryPriceReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf3\x01\n\x19\x44\x65liveryPriceReadResponse\x12P\n\x0f\x64\x65livery_prices\x18\x01 \x03(\x0b\x32\x37.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPrice\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa5\x01\n\x1a\x44\x65liveryPriceUpdateRequest\x12O\n\x0e\x64\x65livery_price\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPrice\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb9\x01\n\x1b\x44\x65liveryPriceUpdateResponse\x12O\n\x0e\x64\x65livery_price\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPrice\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"`\n\x1a\x44\x65liveryPriceDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1b\x44\x65liveryPriceDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*9\n\x08TimeType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MINUTES\x10\x01\x12\t\n\x05HOURS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x32\xac\x05\n\x14\x44\x65liveryPriceService\x12\xa4\x01\n\x13\x44\x65liveryPriceCreate\x12\x44.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceCreateRequest\x1a\x45.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceCreateResponse"\x00\x12\x9e\x01\n\x11\x44\x65liveryPriceRead\x12\x42.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceReadRequest\x1a\x43.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceReadResponse"\x00\x12\xa4\x01\n\x13\x44\x65liveryPriceUpdate\x12\x44.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceUpdateRequest\x1a\x45.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceUpdateResponse"\x00\x12\xa4\x01\n\x13\x44\x65liveryPriceDelete\x12\x44.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceDeleteRequest\x1a\x45.pro.omni.oms.api.v1.rules.delivery_price.DeliveryPriceDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_price_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TIMETYPE"]._serialized_start = 2248
-    _globals["_TIMETYPE"]._serialized_end = 2305
-    _globals["_DELIVERYPRICE"]._serialized_start = 175
-    _globals["_DELIVERYPRICE"]._serialized_end = 615
-    _globals["_DELIVERYPRICECREATEREQUEST"]._serialized_start = 618
-    _globals["_DELIVERYPRICECREATEREQUEST"]._serialized_end = 875
-    _globals["_DELIVERYPRICECREATERESPONSE"]._serialized_start = 878
-    _globals["_DELIVERYPRICECREATERESPONSE"]._serialized_end = 1063
-    _globals["_DELIVERYPRICEREADREQUEST"]._serialized_start = 1066
-    _globals["_DELIVERYPRICEREADREQUEST"]._serialized_end = 1440
-    _globals["_DELIVERYPRICEREADRESPONSE"]._serialized_start = 1443
-    _globals["_DELIVERYPRICEREADRESPONSE"]._serialized_end = 1686
-    _globals["_DELIVERYPRICEUPDATEREQUEST"]._serialized_start = 1689
-    _globals["_DELIVERYPRICEUPDATEREQUEST"]._serialized_end = 1854
-    _globals["_DELIVERYPRICEUPDATERESPONSE"]._serialized_start = 1857
-    _globals["_DELIVERYPRICEUPDATERESPONSE"]._serialized_end = 2042
-    _globals["_DELIVERYPRICEDELETEREQUEST"]._serialized_start = 2044
-    _globals["_DELIVERYPRICEDELETEREQUEST"]._serialized_end = 2140
-    _globals["_DELIVERYPRICEDELETERESPONSE"]._serialized_start = 2142
-    _globals["_DELIVERYPRICEDELETERESPONSE"]._serialized_end = 2246
-    _globals["_DELIVERYPRICESERVICE"]._serialized_start = 2308
-    _globals["_DELIVERYPRICESERVICE"]._serialized_end = 2992
+    _globals["_TIMETYPE"]._serialized_start = 2226
+    _globals["_TIMETYPE"]._serialized_end = 2283
+    _globals["_DELIVERYPRICE"]._serialized_start = 153
+    _globals["_DELIVERYPRICE"]._serialized_end = 593
+    _globals["_DELIVERYPRICECREATEREQUEST"]._serialized_start = 596
+    _globals["_DELIVERYPRICECREATEREQUEST"]._serialized_end = 853
+    _globals["_DELIVERYPRICECREATERESPONSE"]._serialized_start = 856
+    _globals["_DELIVERYPRICECREATERESPONSE"]._serialized_end = 1041
+    _globals["_DELIVERYPRICEREADREQUEST"]._serialized_start = 1044
+    _globals["_DELIVERYPRICEREADREQUEST"]._serialized_end = 1418
+    _globals["_DELIVERYPRICEREADRESPONSE"]._serialized_start = 1421
+    _globals["_DELIVERYPRICEREADRESPONSE"]._serialized_end = 1664
+    _globals["_DELIVERYPRICEUPDATEREQUEST"]._serialized_start = 1667
+    _globals["_DELIVERYPRICEUPDATEREQUEST"]._serialized_end = 1832
+    _globals["_DELIVERYPRICEUPDATERESPONSE"]._serialized_start = 1835
+    _globals["_DELIVERYPRICEUPDATERESPONSE"]._serialized_end = 2020
+    _globals["_DELIVERYPRICEDELETEREQUEST"]._serialized_start = 2022
+    _globals["_DELIVERYPRICEDELETEREQUEST"]._serialized_end = 2118
+    _globals["_DELIVERYPRICEDELETERESPONSE"]._serialized_start = 2120
+    _globals["_DELIVERYPRICEDELETERESPONSE"]._serialized_end = 2224
+    _globals["_DELIVERYPRICESERVICE"]._serialized_start = 2286
+    _globals["_DELIVERYPRICESERVICE"]._serialized_end = 2970
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from omni.pro.protos.common import base_pb2 as _base_pb2
 from omni.pro.protos.v1.rules import delivery_method_pb2 as _delivery_method_pb2
 from omni.pro.protos.v1.rules import warehouse_pb2 as _warehouse_pb2
-from omni.pro.protos.v1.stock import stock_pb2 as _stock_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class TimeType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
     UNKNOWN: _ClassVar[TimeType]
     MINUTES: _ClassVar[TimeType]
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,40 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 from omni.pro.protos.v1.rules import delivery_method_pb2 as v1_dot_rules_dot_delivery__method__pb2
 from omni.pro.protos.v1.rules import warehouse_pb2 as v1_dot_rules_dot_warehouse__pb2
-from omni.pro.protos.v1.stock import stock_pb2 as v1_dot_stock_dot_stock__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1fv1/rules/delivery_shipper.proto\x12*pro.omni.oms.api.v1.rules.delivery_shipper\x1a\x11\x63ommon/base.proto\x1a\x1ev1/rules/delivery_method.proto\x1a\x14v1/stock/stock.proto\x1a\x18v1/rules/warehouse.proto"\xbc\x03\n\x0f\x44\x65liveryShipper\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12V\n\x13\x64\x65livery_method_ids\x18\x03 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x45\n\rwarehouse_ids\x18\x04 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x1d\n\x15locality_available_id\x18\x05 \x01(\t\x12G\n\ttime_type\x18\x06 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_shipper.TimeType\x12\x11\n\tvalue_min\x18\x07 \x01(\t\x12\x11\n\tvalue_max\x18\x08 \x01(\t\x12\x11\n\tinversely\x18\t \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12?\n\x0cobject_audit\x18\x0b \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x85\x02\n\x1c\x44\x65liveryShipperCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\x15locality_available_id\x18\x02 \x01(\t\x12G\n\ttime_type\x18\x03 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_shipper.TimeType\x12\x11\n\tvalue_min\x18\x04 \x01(\t\x12\x11\n\tvalue_max\x18\x05 \x01(\t\x12\x11\n\tinversely\x18\x06 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc1\x01\n\x1d\x44\x65liveryShipperCreateResponse\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf8\x02\n\x1a\x44\x65liveryShipperReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xfb\x01\n\x1b\x44\x65liveryShipperReadResponse\x12V\n\x11\x64\x65livery_shippers\x18\x01 \x03(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xad\x01\n\x1c\x44\x65liveryShipperUpdateRequest\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc1\x01\n\x1d\x44\x65liveryShipperUpdateResponse\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"b\n\x1c\x44\x65liveryShipperDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"j\n\x1d\x44\x65liveryShipperDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*9\n\x08TimeType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MINUTES\x10\x01\x12\t\n\x05HOURS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x32\xd6\x05\n\x16\x44\x65liveryShipperService\x12\xae\x01\n\x15\x44\x65liveryShipperCreate\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperCreateRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperCreateResponse"\x00\x12\xa8\x01\n\x13\x44\x65liveryShipperRead\x12\x46.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperReadRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperReadResponse"\x00\x12\xae\x01\n\x15\x44\x65liveryShipperUpdate\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperUpdateRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperUpdateResponse"\x00\x12\xae\x01\n\x15\x44\x65liveryShipperDelete\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperDeleteRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1fv1/rules/delivery_shipper.proto\x12*pro.omni.oms.api.v1.rules.delivery_shipper\x1a\x11\x63ommon/base.proto\x1a\x1ev1/rules/delivery_method.proto\x1a\x18v1/rules/warehouse.proto"\xbc\x03\n\x0f\x44\x65liveryShipper\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12V\n\x13\x64\x65livery_method_ids\x18\x03 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x45\n\rwarehouse_ids\x18\x04 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x1d\n\x15locality_available_id\x18\x05 \x01(\t\x12G\n\ttime_type\x18\x06 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_shipper.TimeType\x12\x11\n\tvalue_min\x18\x07 \x01(\t\x12\x11\n\tvalue_max\x18\x08 \x01(\t\x12\x11\n\tinversely\x18\t \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12?\n\x0cobject_audit\x18\x0b \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x85\x02\n\x1c\x44\x65liveryShipperCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\x15locality_available_id\x18\x02 \x01(\t\x12G\n\ttime_type\x18\x03 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_shipper.TimeType\x12\x11\n\tvalue_min\x18\x04 \x01(\t\x12\x11\n\tvalue_max\x18\x05 \x01(\t\x12\x11\n\tinversely\x18\x06 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc1\x01\n\x1d\x44\x65liveryShipperCreateResponse\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf8\x02\n\x1a\x44\x65liveryShipperReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xfb\x01\n\x1b\x44\x65liveryShipperReadResponse\x12V\n\x11\x64\x65livery_shippers\x18\x01 \x03(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xad\x01\n\x1c\x44\x65liveryShipperUpdateRequest\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc1\x01\n\x1d\x44\x65liveryShipperUpdateResponse\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"b\n\x1c\x44\x65liveryShipperDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"j\n\x1d\x44\x65liveryShipperDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*9\n\x08TimeType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MINUTES\x10\x01\x12\t\n\x05HOURS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x32\xd6\x05\n\x16\x44\x65liveryShipperService\x12\xae\x01\n\x15\x44\x65liveryShipperCreate\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperCreateRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperCreateResponse"\x00\x12\xa8\x01\n\x13\x44\x65liveryShipperRead\x12\x46.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperReadRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperReadResponse"\x00\x12\xae\x01\n\x15\x44\x65liveryShipperUpdate\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperUpdateRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperUpdateResponse"\x00\x12\xae\x01\n\x15\x44\x65liveryShipperDelete\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperDeleteRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_shipper_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TIMETYPE"]._serialized_start = 2298
-    _globals["_TIMETYPE"]._serialized_end = 2355
-    _globals["_DELIVERYSHIPPER"]._serialized_start = 179
-    _globals["_DELIVERYSHIPPER"]._serialized_end = 623
-    _globals["_DELIVERYSHIPPERCREATEREQUEST"]._serialized_start = 626
-    _globals["_DELIVERYSHIPPERCREATEREQUEST"]._serialized_end = 887
-    _globals["_DELIVERYSHIPPERCREATERESPONSE"]._serialized_start = 890
-    _globals["_DELIVERYSHIPPERCREATERESPONSE"]._serialized_end = 1083
-    _globals["_DELIVERYSHIPPERREADREQUEST"]._serialized_start = 1086
-    _globals["_DELIVERYSHIPPERREADREQUEST"]._serialized_end = 1462
-    _globals["_DELIVERYSHIPPERREADRESPONSE"]._serialized_start = 1465
-    _globals["_DELIVERYSHIPPERREADRESPONSE"]._serialized_end = 1716
-    _globals["_DELIVERYSHIPPERUPDATEREQUEST"]._serialized_start = 1719
-    _globals["_DELIVERYSHIPPERUPDATEREQUEST"]._serialized_end = 1892
-    _globals["_DELIVERYSHIPPERUPDATERESPONSE"]._serialized_start = 1895
-    _globals["_DELIVERYSHIPPERUPDATERESPONSE"]._serialized_end = 2088
-    _globals["_DELIVERYSHIPPERDELETEREQUEST"]._serialized_start = 2090
-    _globals["_DELIVERYSHIPPERDELETEREQUEST"]._serialized_end = 2188
-    _globals["_DELIVERYSHIPPERDELETERESPONSE"]._serialized_start = 2190
-    _globals["_DELIVERYSHIPPERDELETERESPONSE"]._serialized_end = 2296
-    _globals["_DELIVERYSHIPPERSERVICE"]._serialized_start = 2358
-    _globals["_DELIVERYSHIPPERSERVICE"]._serialized_end = 3084
+    _globals["_TIMETYPE"]._serialized_start = 2276
+    _globals["_TIMETYPE"]._serialized_end = 2333
+    _globals["_DELIVERYSHIPPER"]._serialized_start = 157
+    _globals["_DELIVERYSHIPPER"]._serialized_end = 601
+    _globals["_DELIVERYSHIPPERCREATEREQUEST"]._serialized_start = 604
+    _globals["_DELIVERYSHIPPERCREATEREQUEST"]._serialized_end = 865
+    _globals["_DELIVERYSHIPPERCREATERESPONSE"]._serialized_start = 868
+    _globals["_DELIVERYSHIPPERCREATERESPONSE"]._serialized_end = 1061
+    _globals["_DELIVERYSHIPPERREADREQUEST"]._serialized_start = 1064
+    _globals["_DELIVERYSHIPPERREADREQUEST"]._serialized_end = 1440
+    _globals["_DELIVERYSHIPPERREADRESPONSE"]._serialized_start = 1443
+    _globals["_DELIVERYSHIPPERREADRESPONSE"]._serialized_end = 1694
+    _globals["_DELIVERYSHIPPERUPDATEREQUEST"]._serialized_start = 1697
+    _globals["_DELIVERYSHIPPERUPDATEREQUEST"]._serialized_end = 1870
+    _globals["_DELIVERYSHIPPERUPDATERESPONSE"]._serialized_start = 1873
+    _globals["_DELIVERYSHIPPERUPDATERESPONSE"]._serialized_end = 2066
+    _globals["_DELIVERYSHIPPERDELETEREQUEST"]._serialized_start = 2068
+    _globals["_DELIVERYSHIPPERDELETEREQUEST"]._serialized_end = 2166
+    _globals["_DELIVERYSHIPPERDELETERESPONSE"]._serialized_start = 2168
+    _globals["_DELIVERYSHIPPERDELETERESPONSE"]._serialized_end = 2274
+    _globals["_DELIVERYSHIPPERSERVICE"]._serialized_start = 2336
+    _globals["_DELIVERYSHIPPERSERVICE"]._serialized_end = 3062
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from omni.pro.protos.common import base_pb2 as _base_pb2
 from omni.pro.protos.v1.rules import delivery_method_pb2 as _delivery_method_pb2
 from omni.pro.protos.v1.rules import warehouse_pb2 as _warehouse_pb2
-from omni.pro.protos.v1.stock import stock_pb2 as _stock_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class TimeType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
     UNKNOWN: _ClassVar[TimeType]
     MINUTES: _ClassVar[TimeType]
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/location_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/location_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/location_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/location_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/location_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/location_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_line_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/address_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/address_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/address_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/address_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/carrier_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/carrier_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/carrier_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/carrier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/carrier_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/carrier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/channel_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/channel_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/channel_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/client_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/client_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/client_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/client_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/country_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/country_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/country_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/currency_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/currency_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/currency_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/currency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/currency_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/delivery_method_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/delivery_method_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/order_line_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/order_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/order_line_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/order_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/order_line_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/order_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/order_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/order_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/order_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/order_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/order_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/payment_method_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/payment_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/payment_method_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/payment_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_order_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_order_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_order_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_order_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/picking_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/product_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/product_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/product_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/product_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/product_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/sale_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/sale_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/sale_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/sale_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/sale_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/sale_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/tax_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/tax_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/tax_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/tax_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/tax_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/uom_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/uom_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/uom_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/uom_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/uom_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/user_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/user_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/user_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/warehouse_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/warehouse_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/attachment_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/attachment_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/attachment_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/carrier_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/carrier_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/carrier_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/carrier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/carrier_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/carrier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/country_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/country_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/country_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/location_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/location_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/location_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/location_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/location_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/location_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_type_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_type_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_type_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/procurement_group_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/procurement_group_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/procurement_group_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/procurement_group_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/product_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/product_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/product_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/product_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/product_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/quant_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/quant_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/quant_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/quant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/quant_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/quant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/route_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/route_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/route_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/route_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/route_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/route_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/rule_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/rule_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/rule_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/rule_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/rule_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/rule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_line_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/warehouse_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/stock/stock.proto
+# source: v1/stock/warehouse.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -13,36 +13,36 @@
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x14v1/stock/stock.proto\x12\x18pro.omni.oms.api.v1.rule\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb6\x02\n\x04Rule\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x04 \x01(\x05\x12\x17\n\x0flocation_src_id\x18\x05 \x01(\x05\x12\x13\n\x0blocation_id\x18\x06 \x01(\x05\x12\x16\n\x0eprocure_method\x18\x07 \x01(\t\x12\x10\n\x08route_id\x18\x08 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\t \x01(\x05\x12\x10\n\x08sequence\x18\n \x01(\x05\x12*\n\x06\x61\x63tive\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0c \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x82\x02\n\x11RuleCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x03 \x01(\x05\x12\x17\n\x0flocation_src_id\x18\x04 \x01(\x05\x12\x13\n\x0blocation_id\x18\x05 \x01(\x05\x12\x16\n\x0eprocure_method\x18\x06 \x01(\t\x12\x10\n\x08route_id\x18\x07 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x08 \x01(\x05\x12\x10\n\x08sequence\x18\t \x01(\x05\x12\x36\n\x07\x63ontext\x18\n \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8d\x01\n\x12RuleCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12,\n\x04rule\x18\x02 \x01(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule"\xed\x02\n\x0fRuleReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc7\x01\n\x10RuleReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12-\n\x05rules\x18\x03 \x03(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule"y\n\x11RuleUpdateRequest\x12,\n\x04rule\x18\x01 \x01(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8d\x01\n\x12RuleUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12,\n\x04rule\x18\x02 \x01(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule"W\n\x11RuleDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"_\n\x12RuleDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xb3\x03\n\x0bRuleService\x12i\n\nRuleCreate\x12+.pro.omni.oms.api.v1.rule.RuleCreateRequest\x1a,.pro.omni.oms.api.v1.rule.RuleCreateResponse"\x00\x12\x63\n\x08RuleRead\x12).pro.omni.oms.api.v1.rule.RuleReadRequest\x1a*.pro.omni.oms.api.v1.rule.RuleReadResponse"\x00\x12i\n\nRuleUpdate\x12+.pro.omni.oms.api.v1.rule.RuleUpdateRequest\x1a,.pro.omni.oms.api.v1.rule.RuleUpdateResponse"\x00\x12i\n\nRuleDelete\x12+.pro.omni.oms.api.v1.rule.RuleDeleteRequest\x1a,.pro.omni.oms.api.v1.rule.RuleDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x18v1/stock/warehouse.proto\x12#pro.omni.oms.api.v1.stock.warehouse\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\x92\x02\n\tWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x12\n\ncountry_id\x18\x04 \x01(\x05\x12\x37\n\x16territory_matrix_value\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x06 \x01(\t\x12\x12\n\ncomplement\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\t \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xde\x01\n\x16WarehouseCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x12\n\ncountry_id\x18\x03 \x01(\x05\x12\x37\n\x16territory_matrix_value\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x05 \x01(\t\x12\x12\n\ncomplement\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\xf2\x02\n\x14WarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe1\x01\n\x15WarehouseReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x42\n\nwarehouses\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\x93\x01\n\x16WarehouseUpdateRequest\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\\\n\x16WarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17WarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd0\x04\n\x10WarehouseService\x12\x8e\x01\n\x0fWarehouseCreate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateResponse"\x00\x12\x88\x01\n\rWarehouseRead\x12\x39.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadRequest\x1a:.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadResponse"\x00\x12\x8e\x01\n\x0fWarehouseUpdate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateResponse"\x00\x12\x8e\x01\n\x0fWarehouseDelete\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.stock_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.warehouse_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_RULE"]._serialized_start = 132
-    _globals["_RULE"]._serialized_end = 442
-    _globals["_RULECREATEREQUEST"]._serialized_start = 445
-    _globals["_RULECREATEREQUEST"]._serialized_end = 703
-    _globals["_RULECREATERESPONSE"]._serialized_start = 706
-    _globals["_RULECREATERESPONSE"]._serialized_end = 847
-    _globals["_RULEREADREQUEST"]._serialized_start = 850
-    _globals["_RULEREADREQUEST"]._serialized_end = 1215
-    _globals["_RULEREADRESPONSE"]._serialized_start = 1218
-    _globals["_RULEREADRESPONSE"]._serialized_end = 1417
-    _globals["_RULEUPDATEREQUEST"]._serialized_start = 1419
-    _globals["_RULEUPDATEREQUEST"]._serialized_end = 1540
-    _globals["_RULEUPDATERESPONSE"]._serialized_start = 1543
-    _globals["_RULEUPDATERESPONSE"]._serialized_end = 1684
-    _globals["_RULEDELETEREQUEST"]._serialized_start = 1686
-    _globals["_RULEDELETEREQUEST"]._serialized_end = 1773
-    _globals["_RULEDELETERESPONSE"]._serialized_start = 1775
-    _globals["_RULEDELETERESPONSE"]._serialized_end = 1870
-    _globals["_RULESERVICE"]._serialized_start = 1873
-    _globals["_RULESERVICE"]._serialized_end = 2308
+    _globals["_WAREHOUSE"]._serialized_start = 147
+    _globals["_WAREHOUSE"]._serialized_end = 421
+    _globals["_WAREHOUSECREATEREQUEST"]._serialized_start = 424
+    _globals["_WAREHOUSECREATEREQUEST"]._serialized_end = 646
+    _globals["_WAREHOUSECREATERESPONSE"]._serialized_start = 649
+    _globals["_WAREHOUSECREATERESPONSE"]._serialized_end = 816
+    _globals["_WAREHOUSEREADREQUEST"]._serialized_start = 819
+    _globals["_WAREHOUSEREADREQUEST"]._serialized_end = 1189
+    _globals["_WAREHOUSEREADRESPONSE"]._serialized_start = 1192
+    _globals["_WAREHOUSEREADRESPONSE"]._serialized_end = 1417
+    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_start = 1420
+    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_end = 1567
+    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_start = 1570
+    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_end = 1737
+    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_start = 1739
+    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_end = 1831
+    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_start = 1833
+    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_end = 1933
+    _globals["_WAREHOUSESERVICE"]._serialized_start = 1936
+    _globals["_WAREHOUSESERVICE"]._serialized_end = 2528
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/currency_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,209 +2,212 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf import struct_pb2 as _struct_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Rule(_message.Message):
+class Currency(_message.Message):
     __slots__ = [
         "id",
         "name",
-        "action",
-        "picking_type_id",
-        "location_src_id",
-        "location_id",
-        "procure_method",
-        "route_id",
-        "warehouse_id",
-        "sequence",
+        "code",
+        "currency_unit_label",
+        "currency_subunit_label",
+        "rate",
+        "rounding",
+        "decimal_places",
+        "symbol",
+        "position",
         "active",
         "object_audit",
     ]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    ACTION_FIELD_NUMBER: _ClassVar[int]
-    PICKING_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_SRC_ID_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_ID_FIELD_NUMBER: _ClassVar[int]
-    PROCURE_METHOD_FIELD_NUMBER: _ClassVar[int]
-    ROUTE_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    CURRENCY_UNIT_LABEL_FIELD_NUMBER: _ClassVar[int]
+    CURRENCY_SUBUNIT_LABEL_FIELD_NUMBER: _ClassVar[int]
+    RATE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
+    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
+    SYMBOL_FIELD_NUMBER: _ClassVar[int]
+    POSITION_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     name: str
-    action: str
-    picking_type_id: int
-    location_src_id: int
-    location_id: int
-    procure_method: str
-    route_id: int
-    warehouse_id: int
-    sequence: int
+    code: str
+    currency_unit_label: str
+    currency_subunit_label: str
+    rate: int
+    rounding: float
+    decimal_places: int
+    symbol: str
+    position: str
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        action: _Optional[str] = ...,
-        picking_type_id: _Optional[int] = ...,
-        location_src_id: _Optional[int] = ...,
-        location_id: _Optional[int] = ...,
-        procure_method: _Optional[str] = ...,
-        route_id: _Optional[int] = ...,
-        warehouse_id: _Optional[int] = ...,
-        sequence: _Optional[int] = ...,
+        code: _Optional[str] = ...,
+        currency_unit_label: _Optional[str] = ...,
+        currency_subunit_label: _Optional[str] = ...,
+        rate: _Optional[int] = ...,
+        rounding: _Optional[float] = ...,
+        decimal_places: _Optional[int] = ...,
+        symbol: _Optional[str] = ...,
+        position: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class RuleCreateRequest(_message.Message):
+class CurrencyAddRequest(_message.Message):
     __slots__ = [
         "name",
-        "action",
-        "picking_type_id",
-        "location_src_id",
-        "location_id",
-        "procure_method",
-        "route_id",
-        "warehouse_id",
-        "sequence",
+        "code",
+        "currency_unit_label",
+        "currency_subunit_label",
+        "rate",
+        "rounding",
+        "decimal_places",
+        "symbol",
+        "position",
+        "active",
         "context",
     ]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    ACTION_FIELD_NUMBER: _ClassVar[int]
-    PICKING_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_SRC_ID_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_ID_FIELD_NUMBER: _ClassVar[int]
-    PROCURE_METHOD_FIELD_NUMBER: _ClassVar[int]
-    ROUTE_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    CURRENCY_UNIT_LABEL_FIELD_NUMBER: _ClassVar[int]
+    CURRENCY_SUBUNIT_LABEL_FIELD_NUMBER: _ClassVar[int]
+    RATE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
+    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
+    SYMBOL_FIELD_NUMBER: _ClassVar[int]
+    POSITION_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
-    action: str
-    picking_type_id: int
-    location_src_id: int
-    location_id: int
-    procure_method: str
-    route_id: int
-    warehouse_id: int
-    sequence: int
+    code: str
+    currency_unit_label: str
+    currency_subunit_label: str
+    rate: int
+    rounding: float
+    decimal_places: int
+    symbol: str
+    position: str
+    active: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
-        action: _Optional[str] = ...,
-        picking_type_id: _Optional[int] = ...,
-        location_src_id: _Optional[int] = ...,
-        location_id: _Optional[int] = ...,
-        procure_method: _Optional[str] = ...,
-        route_id: _Optional[int] = ...,
-        warehouse_id: _Optional[int] = ...,
-        sequence: _Optional[int] = ...,
+        code: _Optional[str] = ...,
+        currency_unit_label: _Optional[str] = ...,
+        currency_subunit_label: _Optional[str] = ...,
+        rate: _Optional[int] = ...,
+        rounding: _Optional[float] = ...,
+        decimal_places: _Optional[int] = ...,
+        symbol: _Optional[str] = ...,
+        position: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class RuleCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "rule"]
+class CurrencyAddResponse(_message.Message):
+    __slots__ = ["response_standard", "currency"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    RULE_FIELD_NUMBER: _ClassVar[int]
+    CURRENCY_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    rule: Rule
+    currency: Currency
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        rule: _Optional[_Union[Rule, _Mapping]] = ...,
+        currency: _Optional[_Union[Currency, _Mapping]] = ...,
     ) -> None: ...
 
-class RuleReadRequest(_message.Message):
+class CurrencyReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class RuleReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "rules"]
+class CurrencyReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "currencies"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    RULES_FIELD_NUMBER: _ClassVar[int]
+    CURRENCIES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    rules: _containers.RepeatedCompositeFieldContainer[Rule]
+    currencies: _containers.RepeatedCompositeFieldContainer[Currency]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        rules: _Optional[_Iterable[_Union[Rule, _Mapping]]] = ...,
+        currencies: _Optional[_Iterable[_Union[Currency, _Mapping]]] = ...,
     ) -> None: ...
 
-class RuleUpdateRequest(_message.Message):
-    __slots__ = ["rule", "context"]
-    RULE_FIELD_NUMBER: _ClassVar[int]
+class CurrencyUpdateRequest(_message.Message):
+    __slots__ = ["currency", "context"]
+    CURRENCY_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    rule: Rule
+    currency: Currency
     context: _base_pb2.Context
     def __init__(
         self,
-        rule: _Optional[_Union[Rule, _Mapping]] = ...,
+        currency: _Optional[_Union[Currency, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class RuleUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "rule"]
+class CurrencyUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "currency"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    RULE_FIELD_NUMBER: _ClassVar[int]
+    CURRENCY_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    rule: Rule
+    currency: Currency
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        rule: _Optional[_Union[Rule, _Mapping]] = ...,
+        currency: _Optional[_Union[Currency, _Mapping]] = ...,
     ) -> None: ...
 
-class RuleDeleteRequest(_message.Message):
+class CurrencyDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class RuleDeleteResponse(_message.Message):
+class CurrencyDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/stock_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/uom_pb2_grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,209 +1,211 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.stock import stock_pb2 as v1_dot_stock_dot_stock__pb2
+from omni.pro.protos.v1.stock import uom_pb2 as v1_dot_stock_dot_uom__pb2
 
 
-class RuleServiceStub(object):
+class ProductServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.RuleCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rule.RuleService/RuleCreate",
-            request_serializer=v1_dot_stock_dot_stock__pb2.RuleCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_stock__pb2.RuleCreateResponse.FromString,
+        self.UomCreate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomCreate",
+            request_serializer=v1_dot_stock_dot_uom__pb2.UomCreateRequest.SerializeToString,
+            response_deserializer=v1_dot_stock_dot_uom__pb2.UomCreateResponse.FromString,
         )
-        self.RuleRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rule.RuleService/RuleRead",
-            request_serializer=v1_dot_stock_dot_stock__pb2.RuleReadRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_stock__pb2.RuleReadResponse.FromString,
+        self.UomRead = channel.unary_unary(
+            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomRead",
+            request_serializer=v1_dot_stock_dot_uom__pb2.UomReadRequest.SerializeToString,
+            response_deserializer=v1_dot_stock_dot_uom__pb2.UomReadResponse.FromString,
         )
-        self.RuleUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rule.RuleService/RuleUpdate",
-            request_serializer=v1_dot_stock_dot_stock__pb2.RuleUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_stock__pb2.RuleUpdateResponse.FromString,
+        self.UomUpdate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomUpdate",
+            request_serializer=v1_dot_stock_dot_uom__pb2.UomUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_stock_dot_uom__pb2.UomUpdateResponse.FromString,
         )
-        self.RuleDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rule.RuleService/RuleDelete",
-            request_serializer=v1_dot_stock_dot_stock__pb2.RuleDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_stock__pb2.RuleDeleteResponse.FromString,
+        self.UomDelete = channel.unary_unary(
+            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomDelete",
+            request_serializer=v1_dot_stock_dot_uom__pb2.UomDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_stock_dot_uom__pb2.UomDeleteResponse.FromString,
         )
 
 
-class RuleServiceServicer(object):
+class ProductServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def RuleCreate(self, request, context):
+    def UomCreate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def RuleRead(self, request, context):
+    def UomRead(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def RuleUpdate(self, request, context):
+    def UomUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def RuleDelete(self, request, context):
+    def UomDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_RuleServiceServicer_to_server(servicer, server):
+def add_ProductServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "RuleCreate": grpc.unary_unary_rpc_method_handler(
-            servicer.RuleCreate,
-            request_deserializer=v1_dot_stock_dot_stock__pb2.RuleCreateRequest.FromString,
-            response_serializer=v1_dot_stock_dot_stock__pb2.RuleCreateResponse.SerializeToString,
+        "UomCreate": grpc.unary_unary_rpc_method_handler(
+            servicer.UomCreate,
+            request_deserializer=v1_dot_stock_dot_uom__pb2.UomCreateRequest.FromString,
+            response_serializer=v1_dot_stock_dot_uom__pb2.UomCreateResponse.SerializeToString,
         ),
-        "RuleRead": grpc.unary_unary_rpc_method_handler(
-            servicer.RuleRead,
-            request_deserializer=v1_dot_stock_dot_stock__pb2.RuleReadRequest.FromString,
-            response_serializer=v1_dot_stock_dot_stock__pb2.RuleReadResponse.SerializeToString,
+        "UomRead": grpc.unary_unary_rpc_method_handler(
+            servicer.UomRead,
+            request_deserializer=v1_dot_stock_dot_uom__pb2.UomReadRequest.FromString,
+            response_serializer=v1_dot_stock_dot_uom__pb2.UomReadResponse.SerializeToString,
         ),
-        "RuleUpdate": grpc.unary_unary_rpc_method_handler(
-            servicer.RuleUpdate,
-            request_deserializer=v1_dot_stock_dot_stock__pb2.RuleUpdateRequest.FromString,
-            response_serializer=v1_dot_stock_dot_stock__pb2.RuleUpdateResponse.SerializeToString,
+        "UomUpdate": grpc.unary_unary_rpc_method_handler(
+            servicer.UomUpdate,
+            request_deserializer=v1_dot_stock_dot_uom__pb2.UomUpdateRequest.FromString,
+            response_serializer=v1_dot_stock_dot_uom__pb2.UomUpdateResponse.SerializeToString,
         ),
-        "RuleDelete": grpc.unary_unary_rpc_method_handler(
-            servicer.RuleDelete,
-            request_deserializer=v1_dot_stock_dot_stock__pb2.RuleDeleteRequest.FromString,
-            response_serializer=v1_dot_stock_dot_stock__pb2.RuleDeleteResponse.SerializeToString,
+        "UomDelete": grpc.unary_unary_rpc_method_handler(
+            servicer.UomDelete,
+            request_deserializer=v1_dot_stock_dot_uom__pb2.UomDeleteRequest.FromString,
+            response_serializer=v1_dot_stock_dot_uom__pb2.UomDeleteResponse.SerializeToString,
         ),
     }
-    generic_handler = grpc.method_handlers_generic_handler("pro.omni.oms.api.v1.rule.RuleService", rpc_method_handlers)
+    generic_handler = grpc.method_handlers_generic_handler(
+        "pro.omni.oms.api.v1.stock.uom.ProductService", rpc_method_handlers
+    )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class RuleService(object):
+class ProductService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def RuleCreate(
+    def UomCreate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rule.RuleService/RuleCreate",
-            v1_dot_stock_dot_stock__pb2.RuleCreateRequest.SerializeToString,
-            v1_dot_stock_dot_stock__pb2.RuleCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomCreate",
+            v1_dot_stock_dot_uom__pb2.UomCreateRequest.SerializeToString,
+            v1_dot_stock_dot_uom__pb2.UomCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def RuleRead(
+    def UomRead(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rule.RuleService/RuleRead",
-            v1_dot_stock_dot_stock__pb2.RuleReadRequest.SerializeToString,
-            v1_dot_stock_dot_stock__pb2.RuleReadResponse.FromString,
+            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomRead",
+            v1_dot_stock_dot_uom__pb2.UomReadRequest.SerializeToString,
+            v1_dot_stock_dot_uom__pb2.UomReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def RuleUpdate(
+    def UomUpdate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rule.RuleService/RuleUpdate",
-            v1_dot_stock_dot_stock__pb2.RuleUpdateRequest.SerializeToString,
-            v1_dot_stock_dot_stock__pb2.RuleUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomUpdate",
+            v1_dot_stock_dot_uom__pb2.UomUpdateRequest.SerializeToString,
+            v1_dot_stock_dot_uom__pb2.UomUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def RuleDelete(
+    def UomDelete(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rule.RuleService/RuleDelete",
-            v1_dot_stock_dot_stock__pb2.RuleDeleteRequest.SerializeToString,
-            v1_dot_stock_dot_stock__pb2.RuleDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomDelete",
+            v1_dot_stock_dot_uom__pb2.UomDeleteRequest.SerializeToString,
+            v1_dot_stock_dot_uom__pb2.UomDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/uom_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/uom_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/uom_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/uom_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/uom_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/uom_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.stock import uom_pb2 as v1_dot_stock_dot_uom__pb2
+from omni.pro.protos.v1.utilities import uom_pb2 as v1_dot_utilities_dot_uom__pb2
 
 
-class ProductServiceStub(object):
+class UomServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.UomCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomCreate",
-            request_serializer=v1_dot_stock_dot_uom__pb2.UomCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_uom__pb2.UomCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomCreate",
+            request_serializer=v1_dot_utilities_dot_uom__pb2.UomCreateRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomCreateResponse.FromString,
         )
         self.UomRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomRead",
-            request_serializer=v1_dot_stock_dot_uom__pb2.UomReadRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_uom__pb2.UomReadResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomRead",
+            request_serializer=v1_dot_utilities_dot_uom__pb2.UomReadRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomReadResponse.FromString,
         )
         self.UomUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomUpdate",
-            request_serializer=v1_dot_stock_dot_uom__pb2.UomUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_uom__pb2.UomUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomUpdate",
+            request_serializer=v1_dot_utilities_dot_uom__pb2.UomUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomUpdateResponse.FromString,
         )
         self.UomDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomDelete",
-            request_serializer=v1_dot_stock_dot_uom__pb2.UomDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_uom__pb2.UomDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomDelete",
+            request_serializer=v1_dot_utilities_dot_uom__pb2.UomDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomDeleteResponse.FromString,
         )
 
 
-class ProductServiceServicer(object):
+class UomServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def UomCreate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
@@ -59,45 +59,45 @@
     def UomDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_ProductServiceServicer_to_server(servicer, server):
+def add_UomServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "UomCreate": grpc.unary_unary_rpc_method_handler(
             servicer.UomCreate,
-            request_deserializer=v1_dot_stock_dot_uom__pb2.UomCreateRequest.FromString,
-            response_serializer=v1_dot_stock_dot_uom__pb2.UomCreateResponse.SerializeToString,
+            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomCreateRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_uom__pb2.UomCreateResponse.SerializeToString,
         ),
         "UomRead": grpc.unary_unary_rpc_method_handler(
             servicer.UomRead,
-            request_deserializer=v1_dot_stock_dot_uom__pb2.UomReadRequest.FromString,
-            response_serializer=v1_dot_stock_dot_uom__pb2.UomReadResponse.SerializeToString,
+            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomReadRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_uom__pb2.UomReadResponse.SerializeToString,
         ),
         "UomUpdate": grpc.unary_unary_rpc_method_handler(
             servicer.UomUpdate,
-            request_deserializer=v1_dot_stock_dot_uom__pb2.UomUpdateRequest.FromString,
-            response_serializer=v1_dot_stock_dot_uom__pb2.UomUpdateResponse.SerializeToString,
+            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomUpdateRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_uom__pb2.UomUpdateResponse.SerializeToString,
         ),
         "UomDelete": grpc.unary_unary_rpc_method_handler(
             servicer.UomDelete,
-            request_deserializer=v1_dot_stock_dot_uom__pb2.UomDeleteRequest.FromString,
-            response_serializer=v1_dot_stock_dot_uom__pb2.UomDeleteResponse.SerializeToString,
+            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomDeleteRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_uom__pb2.UomDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.stock.uom.ProductService", rpc_method_handlers
+        "pro.omni.oms.api.v1.utilities.uom.UomService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class ProductService(object):
+class UomService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def UomCreate(
         request,
         target,
         options=(),
@@ -108,17 +108,17 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomCreate",
-            v1_dot_stock_dot_uom__pb2.UomCreateRequest.SerializeToString,
-            v1_dot_stock_dot_uom__pb2.UomCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomCreate",
+            v1_dot_utilities_dot_uom__pb2.UomCreateRequest.SerializeToString,
+            v1_dot_utilities_dot_uom__pb2.UomCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -137,17 +137,17 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomRead",
-            v1_dot_stock_dot_uom__pb2.UomReadRequest.SerializeToString,
-            v1_dot_stock_dot_uom__pb2.UomReadResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomRead",
+            v1_dot_utilities_dot_uom__pb2.UomReadRequest.SerializeToString,
+            v1_dot_utilities_dot_uom__pb2.UomReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -166,17 +166,17 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomUpdate",
-            v1_dot_stock_dot_uom__pb2.UomUpdateRequest.SerializeToString,
-            v1_dot_stock_dot_uom__pb2.UomUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomUpdate",
+            v1_dot_utilities_dot_uom__pb2.UomUpdateRequest.SerializeToString,
+            v1_dot_utilities_dot_uom__pb2.UomUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -195,17 +195,17 @@
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.uom.ProductService/UomDelete",
-            v1_dot_stock_dot_uom__pb2.UomDeleteRequest.SerializeToString,
-            v1_dot_stock_dot_uom__pb2.UomDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomDelete",
+            v1_dot_utilities_dot_uom__pb2.UomDeleteRequest.SerializeToString,
+            v1_dot_utilities_dot_uom__pb2.UomDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/user_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/user_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/user_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/warehouse_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/country_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/stock/warehouse.proto
+# source: v1/utilities/country.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -13,36 +13,36 @@
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x18v1/stock/warehouse.proto\x12#pro.omni.oms.api.v1.stock.warehouse\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\x92\x02\n\tWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x12\n\ncountry_id\x18\x04 \x01(\x05\x12\x37\n\x16territory_matrix_value\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x06 \x01(\t\x12\x12\n\ncomplement\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\t \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xde\x01\n\x16WarehouseCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x12\n\ncountry_id\x18\x03 \x01(\x05\x12\x37\n\x16territory_matrix_value\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x05 \x01(\t\x12\x12\n\ncomplement\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\xf2\x02\n\x14WarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe1\x01\n\x15WarehouseReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x42\n\nwarehouses\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\x93\x01\n\x16WarehouseUpdateRequest\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\\\n\x16WarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17WarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd0\x04\n\x10WarehouseService\x12\x8e\x01\n\x0fWarehouseCreate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateResponse"\x00\x12\x88\x01\n\rWarehouseRead\x12\x39.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadRequest\x1a:.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadResponse"\x00\x12\x8e\x01\n\x0fWarehouseUpdate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateResponse"\x00\x12\x8e\x01\n\x0fWarehouseDelete\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1av1/utilities/country.proto\x12%pro.omni.oms.api.v1.utilities.country\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xbd\x04\n\x07\x43ountry\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x19\n\x11phone_number_size\x18\x04 \x01(\x05\x12\x14\n\x0cphone_prefix\x18\x05 \x01(\t\x12\x33\n\x0frequire_zipcode\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\ncurrencies\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x32\n\x0e\x64ocument_types\x18\t \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x36\n\x12territory_matrixes\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\tmeta_data\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12-\n\ttimezones\x18\r \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12-\n\tlanguages\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x11\n\tlow_level\x18\x0f \x01(\t\x12*\n\x06\x61\x63tive\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x11 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x9d\x04\n\x14\x43ountryCreateRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x19\n\x11phone_number_size\x18\x03 \x01(\x05\x12\x14\n\x0cphone_prefix\x18\x04 \x01(\t\x12\x33\n\x0frequire_zipcode\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0e\x63urrencies_ids\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x36\n\x12\x64ocument_types_ids\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12:\n\x16territory_matrixes_ids\x18\n \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\tmeta_data\x18\x0b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x31\n\rtimezones_ids\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x31\n\rlanguages_ids\x18\r \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x11\n\tlow_level\x18\x0e \x01(\t\x12\x36\n\x07\x63ontext\x18\x0f \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x15\x43ountryCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12?\n\x07\x63ountry\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"\xf0\x02\n\x12\x43ountryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xde\x01\n\x13\x43ountryReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x41\n\tcountries\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"\x8f\x01\n\x14\x43ountryUpdateRequest\x12?\n\x07\x63ountry\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x15\x43ountryUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12?\n\x07\x63ountry\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"Z\n\x14\x43ountryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43ountryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc6\x04\n\x0e\x43ountryService\x12\x8c\x01\n\rCountryCreate\x12;.pro.omni.oms.api.v1.utilities.country.CountryCreateRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryCreateResponse"\x00\x12\x86\x01\n\x0b\x43ountryRead\x12\x39.pro.omni.oms.api.v1.utilities.country.CountryReadRequest\x1a:.pro.omni.oms.api.v1.utilities.country.CountryReadResponse"\x00\x12\x8c\x01\n\rCountryUpdate\x12;.pro.omni.oms.api.v1.utilities.country.CountryUpdateRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryUpdateResponse"\x00\x12\x8c\x01\n\rCountryDelete\x12;.pro.omni.oms.api.v1.utilities.country.CountryDeleteRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.warehouse_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.country_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_WAREHOUSE"]._serialized_start = 147
-    _globals["_WAREHOUSE"]._serialized_end = 421
-    _globals["_WAREHOUSECREATEREQUEST"]._serialized_start = 424
-    _globals["_WAREHOUSECREATEREQUEST"]._serialized_end = 646
-    _globals["_WAREHOUSECREATERESPONSE"]._serialized_start = 649
-    _globals["_WAREHOUSECREATERESPONSE"]._serialized_end = 816
-    _globals["_WAREHOUSEREADREQUEST"]._serialized_start = 819
-    _globals["_WAREHOUSEREADREQUEST"]._serialized_end = 1189
-    _globals["_WAREHOUSEREADRESPONSE"]._serialized_start = 1192
-    _globals["_WAREHOUSEREADRESPONSE"]._serialized_end = 1417
-    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_start = 1420
-    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_end = 1567
-    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_start = 1570
-    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_end = 1737
-    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_start = 1739
-    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_end = 1831
-    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_start = 1833
-    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_end = 1933
-    _globals["_WAREHOUSESERVICE"]._serialized_start = 1936
-    _globals["_WAREHOUSESERVICE"]._serialized_end = 2528
+    _globals["_COUNTRY"]._serialized_start = 151
+    _globals["_COUNTRY"]._serialized_end = 724
+    _globals["_COUNTRYCREATEREQUEST"]._serialized_start = 727
+    _globals["_COUNTRYCREATEREQUEST"]._serialized_end = 1268
+    _globals["_COUNTRYCREATERESPONSE"]._serialized_start = 1271
+    _globals["_COUNTRYCREATERESPONSE"]._serialized_end = 1434
+    _globals["_COUNTRYREADREQUEST"]._serialized_start = 1437
+    _globals["_COUNTRYREADREQUEST"]._serialized_end = 1805
+    _globals["_COUNTRYREADRESPONSE"]._serialized_start = 1808
+    _globals["_COUNTRYREADRESPONSE"]._serialized_end = 2030
+    _globals["_COUNTRYUPDATEREQUEST"]._serialized_start = 2033
+    _globals["_COUNTRYUPDATEREQUEST"]._serialized_end = 2176
+    _globals["_COUNTRYUPDATERESPONSE"]._serialized_start = 2179
+    _globals["_COUNTRYUPDATERESPONSE"]._serialized_end = 2342
+    _globals["_COUNTRYDELETEREQUEST"]._serialized_start = 2344
+    _globals["_COUNTRYDELETEREQUEST"]._serialized_end = 2434
+    _globals["_COUNTRYDELETERESPONSE"]._serialized_start = 2436
+    _globals["_COUNTRYDELETERESPONSE"]._serialized_end = 2534
+    _globals["_COUNTRYSERVICE"]._serialized_start = 2537
+    _globals["_COUNTRYSERVICE"]._serialized_end = 3119
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/warehouse_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/users/user_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/users/user_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/users/user_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/users/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/country_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/tax_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/utilities/country.proto
+# source: v1/utilities/tax.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1av1/utilities/country.proto\x12%pro.omni.oms.api.v1.utilities.country\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xbd\x04\n\x07\x43ountry\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x19\n\x11phone_number_size\x18\x04 \x01(\x05\x12\x14\n\x0cphone_prefix\x18\x05 \x01(\t\x12\x33\n\x0frequire_zipcode\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\ncurrencies\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x32\n\x0e\x64ocument_types\x18\t \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x36\n\x12territory_matrixes\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\tmeta_data\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12-\n\ttimezones\x18\r \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12-\n\tlanguages\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x11\n\tlow_level\x18\x0f \x01(\t\x12*\n\x06\x61\x63tive\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x11 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x9d\x04\n\x14\x43ountryCreateRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x19\n\x11phone_number_size\x18\x03 \x01(\x05\x12\x14\n\x0cphone_prefix\x18\x04 \x01(\t\x12\x33\n\x0frequire_zipcode\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0e\x63urrencies_ids\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x36\n\x12\x64ocument_types_ids\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12:\n\x16territory_matrixes_ids\x18\n \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\tmeta_data\x18\x0b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x31\n\rtimezones_ids\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x31\n\rlanguages_ids\x18\r \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x11\n\tlow_level\x18\x0e \x01(\t\x12\x36\n\x07\x63ontext\x18\x0f \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x15\x43ountryCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12?\n\x07\x63ountry\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"\xf0\x02\n\x12\x43ountryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xde\x01\n\x13\x43ountryReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x41\n\tcountries\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"\x8f\x01\n\x14\x43ountryUpdateRequest\x12?\n\x07\x63ountry\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x15\x43ountryUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12?\n\x07\x63ountry\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.utilities.country.Country"Z\n\x14\x43ountryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43ountryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc6\x04\n\x0e\x43ountryService\x12\x8c\x01\n\rCountryCreate\x12;.pro.omni.oms.api.v1.utilities.country.CountryCreateRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryCreateResponse"\x00\x12\x86\x01\n\x0b\x43ountryRead\x12\x39.pro.omni.oms.api.v1.utilities.country.CountryReadRequest\x1a:.pro.omni.oms.api.v1.utilities.country.CountryReadResponse"\x00\x12\x8c\x01\n\rCountryUpdate\x12;.pro.omni.oms.api.v1.utilities.country.CountryUpdateRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryUpdateResponse"\x00\x12\x8c\x01\n\rCountryDelete\x12;.pro.omni.oms.api.v1.utilities.country.CountryDeleteRequest\x1a<.pro.omni.oms.api.v1.utilities.country.CountryDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/utilities/tax.proto\x12!pro.omni.oms.api.v1.utilities.tax\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xe4\x01\n\x03Tax\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04rate\x18\x04 \x01(\x02\x12\x10\n\x08rounding\x18\x05 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x06 \x01(\x05\x12\x10\n\x08position\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\t \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xad\x01\n\rTaxAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04rate\x18\x03 \x01(\x02\x12\x10\n\x08rounding\x18\x04 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x05 \x01(\x05\x12\x10\n\x08position\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x90\x01\n\x0eTaxAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\xec\x02\n\x0eTaxReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xce\x01\n\x0fTaxReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x35\n\x05taxes\x18\x03 \x03(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\x7f\n\x10TaxUpdateRequest\x12\x33\n\x03tax\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11TaxUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"V\n\x10TaxDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11TaxDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xe5\x03\n\nTaxService\x12o\n\x06TaxAdd\x12\x30.pro.omni.oms.api.v1.utilities.tax.TaxAddRequest\x1a\x31.pro.omni.oms.api.v1.utilities.tax.TaxAddResponse"\x00\x12r\n\x07TaxRead\x12\x31.pro.omni.oms.api.v1.utilities.tax.TaxReadRequest\x1a\x32.pro.omni.oms.api.v1.utilities.tax.TaxReadResponse"\x00\x12x\n\tTaxUpdate\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxUpdateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxUpdateResponse"\x00\x12x\n\tTaxDelete\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxDeleteRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.country_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.tax_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_COUNTRY"]._serialized_start = 151
-    _globals["_COUNTRY"]._serialized_end = 724
-    _globals["_COUNTRYCREATEREQUEST"]._serialized_start = 727
-    _globals["_COUNTRYCREATEREQUEST"]._serialized_end = 1268
-    _globals["_COUNTRYCREATERESPONSE"]._serialized_start = 1271
-    _globals["_COUNTRYCREATERESPONSE"]._serialized_end = 1434
-    _globals["_COUNTRYREADREQUEST"]._serialized_start = 1437
-    _globals["_COUNTRYREADREQUEST"]._serialized_end = 1805
-    _globals["_COUNTRYREADRESPONSE"]._serialized_start = 1808
-    _globals["_COUNTRYREADRESPONSE"]._serialized_end = 2030
-    _globals["_COUNTRYUPDATEREQUEST"]._serialized_start = 2033
-    _globals["_COUNTRYUPDATEREQUEST"]._serialized_end = 2176
-    _globals["_COUNTRYUPDATERESPONSE"]._serialized_start = 2179
-    _globals["_COUNTRYUPDATERESPONSE"]._serialized_end = 2342
-    _globals["_COUNTRYDELETEREQUEST"]._serialized_start = 2344
-    _globals["_COUNTRYDELETEREQUEST"]._serialized_end = 2434
-    _globals["_COUNTRYDELETERESPONSE"]._serialized_start = 2436
-    _globals["_COUNTRYDELETERESPONSE"]._serialized_end = 2534
-    _globals["_COUNTRYSERVICE"]._serialized_start = 2537
-    _globals["_COUNTRYSERVICE"]._serialized_end = 3119
+    _globals["_TAX"]._serialized_start = 113
+    _globals["_TAX"]._serialized_end = 341
+    _globals["_TAXADDREQUEST"]._serialized_start = 344
+    _globals["_TAXADDREQUEST"]._serialized_end = 517
+    _globals["_TAXADDRESPONSE"]._serialized_start = 520
+    _globals["_TAXADDRESPONSE"]._serialized_end = 664
+    _globals["_TAXREADREQUEST"]._serialized_start = 667
+    _globals["_TAXREADREQUEST"]._serialized_end = 1031
+    _globals["_TAXREADRESPONSE"]._serialized_start = 1034
+    _globals["_TAXREADRESPONSE"]._serialized_end = 1240
+    _globals["_TAXUPDATEREQUEST"]._serialized_start = 1242
+    _globals["_TAXUPDATEREQUEST"]._serialized_end = 1369
+    _globals["_TAXUPDATERESPONSE"]._serialized_start = 1372
+    _globals["_TAXUPDATERESPONSE"]._serialized_end = 1519
+    _globals["_TAXDELETEREQUEST"]._serialized_start = 1521
+    _globals["_TAXDELETEREQUEST"]._serialized_end = 1607
+    _globals["_TAXDELETERESPONSE"]._serialized_start = 1609
+    _globals["_TAXDELETERESPONSE"]._serialized_end = 1703
+    _globals["_TAXSERVICE"]._serialized_start = 1706
+    _globals["_TAXSERVICE"]._serialized_end = 2191
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/country_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/country_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/currency_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/currency_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/currency_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/language_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -8,133 +8,141 @@
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Currency(_message.Message):
+class Language(_message.Message):
     __slots__ = [
         "id",
         "name",
         "code",
-        "currency_unit_label",
-        "currency_subunit_label",
-        "rate",
-        "rounding",
-        "decimal_places",
-        "symbol",
-        "position",
+        "code_iso",
+        "direction",
+        "date_format",
+        "time_format",
+        "decimal_point",
+        "thousands_separator",
+        "grouping",
+        "week_start",
         "active",
         "object_audit",
     ]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CURRENCY_UNIT_LABEL_FIELD_NUMBER: _ClassVar[int]
-    CURRENCY_SUBUNIT_LABEL_FIELD_NUMBER: _ClassVar[int]
-    RATE_FIELD_NUMBER: _ClassVar[int]
-    ROUNDING_FIELD_NUMBER: _ClassVar[int]
-    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
-    SYMBOL_FIELD_NUMBER: _ClassVar[int]
-    POSITION_FIELD_NUMBER: _ClassVar[int]
+    CODE_ISO_FIELD_NUMBER: _ClassVar[int]
+    DIRECTION_FIELD_NUMBER: _ClassVar[int]
+    DATE_FORMAT_FIELD_NUMBER: _ClassVar[int]
+    TIME_FORMAT_FIELD_NUMBER: _ClassVar[int]
+    DECIMAL_POINT_FIELD_NUMBER: _ClassVar[int]
+    THOUSANDS_SEPARATOR_FIELD_NUMBER: _ClassVar[int]
+    GROUPING_FIELD_NUMBER: _ClassVar[int]
+    WEEK_START_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     code: str
-    currency_unit_label: str
-    currency_subunit_label: str
-    rate: int
-    rounding: float
-    decimal_places: int
-    symbol: str
-    position: str
+    code_iso: str
+    direction: str
+    date_format: str
+    time_format: str
+    decimal_point: str
+    thousands_separator: str
+    grouping: str
+    week_start: str
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        currency_unit_label: _Optional[str] = ...,
-        currency_subunit_label: _Optional[str] = ...,
-        rate: _Optional[int] = ...,
-        rounding: _Optional[float] = ...,
-        decimal_places: _Optional[int] = ...,
-        symbol: _Optional[str] = ...,
-        position: _Optional[str] = ...,
+        code_iso: _Optional[str] = ...,
+        direction: _Optional[str] = ...,
+        date_format: _Optional[str] = ...,
+        time_format: _Optional[str] = ...,
+        decimal_point: _Optional[str] = ...,
+        thousands_separator: _Optional[str] = ...,
+        grouping: _Optional[str] = ...,
+        week_start: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class CurrencyAddRequest(_message.Message):
+class LanguageAddRequest(_message.Message):
     __slots__ = [
         "name",
         "code",
-        "currency_unit_label",
-        "currency_subunit_label",
-        "rate",
-        "rounding",
-        "decimal_places",
-        "symbol",
-        "position",
+        "code_iso",
+        "direction",
+        "date_format",
+        "time_format",
+        "decimal_point",
+        "thousands_separator",
+        "grouping",
+        "week_start",
         "active",
         "context",
     ]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CURRENCY_UNIT_LABEL_FIELD_NUMBER: _ClassVar[int]
-    CURRENCY_SUBUNIT_LABEL_FIELD_NUMBER: _ClassVar[int]
-    RATE_FIELD_NUMBER: _ClassVar[int]
-    ROUNDING_FIELD_NUMBER: _ClassVar[int]
-    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
-    SYMBOL_FIELD_NUMBER: _ClassVar[int]
-    POSITION_FIELD_NUMBER: _ClassVar[int]
+    CODE_ISO_FIELD_NUMBER: _ClassVar[int]
+    DIRECTION_FIELD_NUMBER: _ClassVar[int]
+    DATE_FORMAT_FIELD_NUMBER: _ClassVar[int]
+    TIME_FORMAT_FIELD_NUMBER: _ClassVar[int]
+    DECIMAL_POINT_FIELD_NUMBER: _ClassVar[int]
+    THOUSANDS_SEPARATOR_FIELD_NUMBER: _ClassVar[int]
+    GROUPING_FIELD_NUMBER: _ClassVar[int]
+    WEEK_START_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     code: str
-    currency_unit_label: str
-    currency_subunit_label: str
-    rate: int
-    rounding: float
-    decimal_places: int
-    symbol: str
-    position: str
+    code_iso: str
+    direction: str
+    date_format: str
+    time_format: str
+    decimal_point: str
+    thousands_separator: str
+    grouping: str
+    week_start: str
     active: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        currency_unit_label: _Optional[str] = ...,
-        currency_subunit_label: _Optional[str] = ...,
-        rate: _Optional[int] = ...,
-        rounding: _Optional[float] = ...,
-        decimal_places: _Optional[int] = ...,
-        symbol: _Optional[str] = ...,
-        position: _Optional[str] = ...,
+        code_iso: _Optional[str] = ...,
+        direction: _Optional[str] = ...,
+        date_format: _Optional[str] = ...,
+        time_format: _Optional[str] = ...,
+        decimal_point: _Optional[str] = ...,
+        thousands_separator: _Optional[str] = ...,
+        grouping: _Optional[str] = ...,
+        week_start: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class CurrencyAddResponse(_message.Message):
-    __slots__ = ["response_standard", "currency"]
+class LanguageAddResponse(_message.Message):
+    __slots__ = ["response_standard", "language"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    CURRENCY_FIELD_NUMBER: _ClassVar[int]
+    LANGUAGE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    currency: Currency
+    language: Language
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        currency: _Optional[_Union[Currency, _Mapping]] = ...,
+        language: _Optional[_Union[Language, _Mapping]] = ...,
     ) -> None: ...
 
-class CurrencyReadRequest(_message.Message):
+class LanguageReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -153,61 +161,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class CurrencyReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "currencies"]
+class LanguageReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "languages"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    CURRENCIES_FIELD_NUMBER: _ClassVar[int]
+    LANGUAGES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    currencies: _containers.RepeatedCompositeFieldContainer[Currency]
+    languages: _containers.RepeatedCompositeFieldContainer[Language]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        currencies: _Optional[_Iterable[_Union[Currency, _Mapping]]] = ...,
+        languages: _Optional[_Iterable[_Union[Language, _Mapping]]] = ...,
     ) -> None: ...
 
-class CurrencyUpdateRequest(_message.Message):
-    __slots__ = ["currency", "context"]
-    CURRENCY_FIELD_NUMBER: _ClassVar[int]
+class LanguageUpdateRequest(_message.Message):
+    __slots__ = ["language", "context"]
+    LANGUAGE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    currency: Currency
+    language: Language
     context: _base_pb2.Context
     def __init__(
         self,
-        currency: _Optional[_Union[Currency, _Mapping]] = ...,
+        language: _Optional[_Union[Language, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class CurrencyUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "currency"]
+class LanguageUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "language"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    CURRENCY_FIELD_NUMBER: _ClassVar[int]
+    LANGUAGE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    currency: Currency
+    language: Language
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        currency: _Optional[_Union[Currency, _Mapping]] = ...,
+        language: _Optional[_Union[Language, _Mapping]] = ...,
     ) -> None: ...
 
-class CurrencyDeleteRequest(_message.Message):
+class LanguageDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class CurrencyDeleteResponse(_message.Message):
+class LanguageDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/currency_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/document_type_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/document_type_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/document_type_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/document_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/language_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/language_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/language_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/timezone_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -8,141 +8,78 @@
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Language(_message.Message):
-    __slots__ = [
-        "id",
-        "name",
-        "code",
-        "code_iso",
-        "direction",
-        "date_format",
-        "time_format",
-        "decimal_point",
-        "thousands_separator",
-        "grouping",
-        "week_start",
-        "active",
-        "object_audit",
-    ]
+class Timezone(_message.Message):
+    __slots__ = ["id", "name", "code", "offset", "offset_dst", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CODE_ISO_FIELD_NUMBER: _ClassVar[int]
-    DIRECTION_FIELD_NUMBER: _ClassVar[int]
-    DATE_FORMAT_FIELD_NUMBER: _ClassVar[int]
-    TIME_FORMAT_FIELD_NUMBER: _ClassVar[int]
-    DECIMAL_POINT_FIELD_NUMBER: _ClassVar[int]
-    THOUSANDS_SEPARATOR_FIELD_NUMBER: _ClassVar[int]
-    GROUPING_FIELD_NUMBER: _ClassVar[int]
-    WEEK_START_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     code: str
-    code_iso: str
-    direction: str
-    date_format: str
-    time_format: str
-    decimal_point: str
-    thousands_separator: str
-    grouping: str
-    week_start: str
+    offset: int
+    offset_dst: int
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        code_iso: _Optional[str] = ...,
-        direction: _Optional[str] = ...,
-        date_format: _Optional[str] = ...,
-        time_format: _Optional[str] = ...,
-        decimal_point: _Optional[str] = ...,
-        thousands_separator: _Optional[str] = ...,
-        grouping: _Optional[str] = ...,
-        week_start: _Optional[str] = ...,
+        offset: _Optional[int] = ...,
+        offset_dst: _Optional[int] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class LanguageAddRequest(_message.Message):
-    __slots__ = [
-        "name",
-        "code",
-        "code_iso",
-        "direction",
-        "date_format",
-        "time_format",
-        "decimal_point",
-        "thousands_separator",
-        "grouping",
-        "week_start",
-        "active",
-        "context",
-    ]
+class TimezoneAddRequest(_message.Message):
+    __slots__ = ["name", "code", "offset", "offset_dst", "active", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CODE_ISO_FIELD_NUMBER: _ClassVar[int]
-    DIRECTION_FIELD_NUMBER: _ClassVar[int]
-    DATE_FORMAT_FIELD_NUMBER: _ClassVar[int]
-    TIME_FORMAT_FIELD_NUMBER: _ClassVar[int]
-    DECIMAL_POINT_FIELD_NUMBER: _ClassVar[int]
-    THOUSANDS_SEPARATOR_FIELD_NUMBER: _ClassVar[int]
-    GROUPING_FIELD_NUMBER: _ClassVar[int]
-    WEEK_START_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     code: str
-    code_iso: str
-    direction: str
-    date_format: str
-    time_format: str
-    decimal_point: str
-    thousands_separator: str
-    grouping: str
-    week_start: str
+    offset: int
+    offset_dst: int
     active: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        code_iso: _Optional[str] = ...,
-        direction: _Optional[str] = ...,
-        date_format: _Optional[str] = ...,
-        time_format: _Optional[str] = ...,
-        decimal_point: _Optional[str] = ...,
-        thousands_separator: _Optional[str] = ...,
-        grouping: _Optional[str] = ...,
-        week_start: _Optional[str] = ...,
+        offset: _Optional[int] = ...,
+        offset_dst: _Optional[int] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class LanguageAddResponse(_message.Message):
-    __slots__ = ["response_standard", "language"]
+class TimezoneAddResponse(_message.Message):
+    __slots__ = ["response_standard", "timezone"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    LANGUAGE_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    language: Language
+    timezone: Timezone
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        language: _Optional[_Union[Language, _Mapping]] = ...,
+        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
     ) -> None: ...
 
-class LanguageReadRequest(_message.Message):
+class TimezoneReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -161,61 +98,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class LanguageReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "languages"]
+class TimezoneReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "timezones"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    LANGUAGES_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    languages: _containers.RepeatedCompositeFieldContainer[Language]
+    timezones: _containers.RepeatedCompositeFieldContainer[Timezone]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        languages: _Optional[_Iterable[_Union[Language, _Mapping]]] = ...,
+        timezones: _Optional[_Iterable[_Union[Timezone, _Mapping]]] = ...,
     ) -> None: ...
 
-class LanguageUpdateRequest(_message.Message):
-    __slots__ = ["language", "context"]
-    LANGUAGE_FIELD_NUMBER: _ClassVar[int]
+class TimezoneUpdateRequest(_message.Message):
+    __slots__ = ["timezone", "context"]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    language: Language
+    timezone: Timezone
     context: _base_pb2.Context
     def __init__(
         self,
-        language: _Optional[_Union[Language, _Mapping]] = ...,
+        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class LanguageUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "language"]
+class TimezoneUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "timezone"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    LANGUAGE_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    language: Language
+    timezone: Timezone
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        language: _Optional[_Union[Language, _Mapping]] = ...,
+        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
     ) -> None: ...
 
-class LanguageDeleteRequest(_message.Message):
+class TimezoneDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class LanguageDeleteResponse(_message.Message):
+class TimezoneDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/language_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/language_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/model_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/model_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/model_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/model_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/payment_method_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/payment_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/payment_method_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/payment_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/tax_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/uom_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/utilities/tax.proto
+# source: v1/utilities/uom.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -12,36 +12,36 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/utilities/tax.proto\x12!pro.omni.oms.api.v1.utilities.tax\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xe4\x01\n\x03Tax\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04rate\x18\x04 \x01(\x02\x12\x10\n\x08rounding\x18\x05 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x06 \x01(\x05\x12\x10\n\x08position\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\t \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xad\x01\n\rTaxAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04rate\x18\x03 \x01(\x02\x12\x10\n\x08rounding\x18\x04 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x05 \x01(\x05\x12\x10\n\x08position\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x90\x01\n\x0eTaxAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\xec\x02\n\x0eTaxReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xce\x01\n\x0fTaxReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x35\n\x05taxes\x18\x03 \x03(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\x7f\n\x10TaxUpdateRequest\x12\x33\n\x03tax\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11TaxUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"V\n\x10TaxDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11TaxDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xe5\x03\n\nTaxService\x12o\n\x06TaxAdd\x12\x30.pro.omni.oms.api.v1.utilities.tax.TaxAddRequest\x1a\x31.pro.omni.oms.api.v1.utilities.tax.TaxAddResponse"\x00\x12r\n\x07TaxRead\x12\x31.pro.omni.oms.api.v1.utilities.tax.TaxReadRequest\x1a\x32.pro.omni.oms.api.v1.utilities.tax.TaxReadResponse"\x00\x12x\n\tTaxUpdate\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxUpdateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxUpdateResponse"\x00\x12x\n\tTaxDelete\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxDeleteRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/utilities/uom.proto\x12!pro.omni.oms.api.v1.utilities.uom\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xcc\x01\n\x03Uom\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x10\n\x08rounding\x18\x06 \x01(\x01\x12*\n\x06\x61\x63tive\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x08 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x98\x01\n\x10UomCreateRequest\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x10\n\x08rounding\x18\x05 \x01(\x01\x12\x36\n\x07\x63ontext\x18\x06 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11UomCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03uom\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"\xec\x02\n\x0eUomReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcd\x01\n\x0fUomReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x34\n\x04uoms\x18\x03 \x03(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"\x7f\n\x10UomUpdateRequest\x12\x33\n\x03uom\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11UomUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03uom\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"V\n\x10UomDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11UomDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xee\x03\n\nUomService\x12x\n\tUomCreate\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomCreateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomCreateResponse"\x00\x12r\n\x07UomRead\x12\x31.pro.omni.oms.api.v1.utilities.uom.UomReadRequest\x1a\x32.pro.omni.oms.api.v1.utilities.uom.UomReadResponse"\x00\x12x\n\tUomUpdate\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomUpdateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomUpdateResponse"\x00\x12x\n\tUomDelete\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomDeleteRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.tax_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.uom_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TAX"]._serialized_start = 113
-    _globals["_TAX"]._serialized_end = 341
-    _globals["_TAXADDREQUEST"]._serialized_start = 344
-    _globals["_TAXADDREQUEST"]._serialized_end = 517
-    _globals["_TAXADDRESPONSE"]._serialized_start = 520
-    _globals["_TAXADDRESPONSE"]._serialized_end = 664
-    _globals["_TAXREADREQUEST"]._serialized_start = 667
-    _globals["_TAXREADREQUEST"]._serialized_end = 1031
-    _globals["_TAXREADRESPONSE"]._serialized_start = 1034
-    _globals["_TAXREADRESPONSE"]._serialized_end = 1240
-    _globals["_TAXUPDATEREQUEST"]._serialized_start = 1242
-    _globals["_TAXUPDATEREQUEST"]._serialized_end = 1369
-    _globals["_TAXUPDATERESPONSE"]._serialized_start = 1372
-    _globals["_TAXUPDATERESPONSE"]._serialized_end = 1519
-    _globals["_TAXDELETEREQUEST"]._serialized_start = 1521
-    _globals["_TAXDELETEREQUEST"]._serialized_end = 1607
-    _globals["_TAXDELETERESPONSE"]._serialized_start = 1609
-    _globals["_TAXDELETERESPONSE"]._serialized_end = 1703
-    _globals["_TAXSERVICE"]._serialized_start = 1706
-    _globals["_TAXSERVICE"]._serialized_end = 2191
+    _globals["_UOM"]._serialized_start = 113
+    _globals["_UOM"]._serialized_end = 317
+    _globals["_UOMCREATEREQUEST"]._serialized_start = 320
+    _globals["_UOMCREATEREQUEST"]._serialized_end = 472
+    _globals["_UOMCREATERESPONSE"]._serialized_start = 475
+    _globals["_UOMCREATERESPONSE"]._serialized_end = 622
+    _globals["_UOMREADREQUEST"]._serialized_start = 625
+    _globals["_UOMREADREQUEST"]._serialized_end = 989
+    _globals["_UOMREADRESPONSE"]._serialized_start = 992
+    _globals["_UOMREADRESPONSE"]._serialized_end = 1197
+    _globals["_UOMUPDATEREQUEST"]._serialized_start = 1199
+    _globals["_UOMUPDATEREQUEST"]._serialized_end = 1326
+    _globals["_UOMUPDATERESPONSE"]._serialized_start = 1329
+    _globals["_UOMUPDATERESPONSE"]._serialized_end = 1476
+    _globals["_UOMDELETEREQUEST"]._serialized_start = 1478
+    _globals["_UOMDELETEREQUEST"]._serialized_end = 1564
+    _globals["_UOMDELETERESPONSE"]._serialized_start = 1566
+    _globals["_UOMDELETERESPONSE"]._serialized_end = 1660
+    _globals["_UOMSERVICE"]._serialized_start = 1663
+    _globals["_UOMSERVICE"]._serialized_end = 2157
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/tax_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/tax_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/tax_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/timezone_pb2.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/timezone_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/timezone_pb2.pyi` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/uom_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -8,151 +8,152 @@
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Timezone(_message.Message):
-    __slots__ = ["id", "name", "code", "offset", "offset_dst", "active", "object_audit"]
+class Uom(_message.Message):
+    __slots__ = ["id", "category", "code", "name", "type", "rounding", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+    CATEGORY_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    OFFSET_FIELD_NUMBER: _ClassVar[int]
-    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
-    name: str
+    category: str
     code: str
-    offset: int
-    offset_dst: int
+    name: str
+    type: str
+    rounding: float
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
-        name: _Optional[str] = ...,
+        category: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        offset: _Optional[int] = ...,
-        offset_dst: _Optional[int] = ...,
+        name: _Optional[str] = ...,
+        type: _Optional[str] = ...,
+        rounding: _Optional[float] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneAddRequest(_message.Message):
-    __slots__ = ["name", "code", "offset", "offset_dst", "active", "context"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+class UomCreateRequest(_message.Message):
+    __slots__ = ["category", "code", "name", "type", "rounding", "context"]
+    CATEGORY_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    OFFSET_FIELD_NUMBER: _ClassVar[int]
-    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
-    ACTIVE_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    name: str
+    category: str
     code: str
-    offset: int
-    offset_dst: int
-    active: _wrappers_pb2.BoolValue
+    name: str
+    type: str
+    rounding: float
     context: _base_pb2.Context
     def __init__(
         self,
-        name: _Optional[str] = ...,
+        category: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        offset: _Optional[int] = ...,
-        offset_dst: _Optional[int] = ...,
-        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
+        name: _Optional[str] = ...,
+        type: _Optional[str] = ...,
+        rounding: _Optional[float] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneAddResponse(_message.Message):
-    __slots__ = ["response_standard", "timezone"]
+class UomCreateResponse(_message.Message):
+    __slots__ = ["response_standard", "uom"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    timezone: Timezone
+    uom: Uom
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
+        uom: _Optional[_Union[Uom, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneReadRequest(_message.Message):
+class UomReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[str] = ...,
+        id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "timezones"]
+class UomReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "uoms"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    TIMEZONES_FIELD_NUMBER: _ClassVar[int]
+    UOMS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    timezones: _containers.RepeatedCompositeFieldContainer[Timezone]
+    uoms: _containers.RepeatedCompositeFieldContainer[Uom]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        timezones: _Optional[_Iterable[_Union[Timezone, _Mapping]]] = ...,
+        uoms: _Optional[_Iterable[_Union[Uom, _Mapping]]] = ...,
     ) -> None: ...
 
-class TimezoneUpdateRequest(_message.Message):
-    __slots__ = ["timezone", "context"]
-    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
+class UomUpdateRequest(_message.Message):
+    __slots__ = ["uom", "context"]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    timezone: Timezone
+    uom: Uom
     context: _base_pb2.Context
     def __init__(
-        self,
-        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
-        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+        self, uom: _Optional[_Union[Uom, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class TimezoneUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "timezone"]
+class UomUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "uom"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    timezone: Timezone
+    uom: Uom
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
+        uom: _Optional[_Union[Uom, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneDeleteRequest(_message.Message):
+class UomDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class TimezoneDeleteResponse(_message.Message):
+class UomDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.18/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py` & `omni-pro-0.1.19/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/stack.py` & `omni-pro-0.1.19/omni/pro/stack.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/user/access.py` & `omni-pro-0.1.19/omni/pro/user/access.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/util.py` & `omni-pro-0.1.19/omni/pro/util.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni/pro/validators.py` & `omni-pro-0.1.19/omni/pro/validators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.18/omni_pro.egg-info/PKG-INFO` & `omni-pro-0.1.19/omni_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.1.18
+Version: 0.1.19
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.1.18/omni_pro.egg-info/SOURCES.txt` & `omni-pro-0.1.19/omni_pro.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -256,17 +256,14 @@
 omni/pro/protos/v1/stock/rule_pb2_grpc.py
 omni/pro/protos/v1/stock/stock_move_line_pb2.py
 omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
 omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
 omni/pro/protos/v1/stock/stock_move_pb2.py
 omni/pro/protos/v1/stock/stock_move_pb2.pyi
 omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
-omni/pro/protos/v1/stock/stock_pb2.py
-omni/pro/protos/v1/stock/stock_pb2.pyi
-omni/pro/protos/v1/stock/stock_pb2_grpc.py
 omni/pro/protos/v1/stock/uom_pb2.py
 omni/pro/protos/v1/stock/uom_pb2.pyi
 omni/pro/protos/v1/stock/uom_pb2_grpc.py
 omni/pro/protos/v1/stock/user_pb2.py
 omni/pro/protos/v1/stock/user_pb2.pyi
 omni/pro/protos/v1/stock/user_pb2_grpc.py
 omni/pro/protos/v1/stock/warehouse_pb2.py
```

### Comparing `omni-pro-0.1.18/setup.py` & `omni-pro-0.1.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 DESCRIPTION = "Python library designed to be a utility for OMS microservices"
-VERSION = "0.1.18"
+VERSION = "0.1.19"
 PACKAGE_NAME = "omni-pro"
 AUTHOR = "OMNI.PRO"
 AUTHOR_EMAIL = "development@omni.pro"
 URL = "https://github.com/Omnipro-Solutions/saas-ms-library"
 
 INSTALL_REQUIRES = [
     "protobuf==4.23.4",
```

