# Comparing `tmp/resotocore-3.6.1.tar.gz` & `tmp/resotocore-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotocore-3.6.1.tar", last modified: Fri Jul 14 17:01:36 2023, max compression
+gzip compressed data, was "resotocore-3.6.2.tar", last modified: Fri Jul 21 22:10:27 2023, max compression
```

## Comparing `resotocore-3.6.1.tar` & `resotocore-3.6.2.tar`

### file list

```diff
@@ -1,806 +1,808 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.377378 resotocore-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 16:55:53.000000 resotocore-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-14 16:55:53.000000 resotocore-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-07-14 17:01:36.377378 resotocore-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-14 16:55:53.000000 resotocore-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-14 16:55:53.000000 resotocore-3.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.149377 resotocore-3.6.1/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.153377 resotocore-3.6.1/resotocore/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/action_handlers/merge_outer_edge_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.153377 resotocore-3.6.1/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/analytics/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/analytics/recurrent_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/async_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.153377 resotocore-3.6.1/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31097 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   241878 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/tip_of_the_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.157377 resotocore-3.6.1/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/config/config_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/config/config_override_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/config/core_config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/console_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/core_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.161377 resotocore-3.6.1/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34739 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/arango_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/arangodb_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/configdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/db_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/deferred_edge_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    65689 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/graphdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/packagedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/runningtaskdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/subscriberdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/system_data_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/templatedb.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/usagedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.161377 resotocore-3.6.1/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/graph_manager/graph_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.161377 resotocore-3.6.1/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/local_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.165377 resotocore-3.6.1/resotocore/jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.133377 resotocore-3.6.1/resotocore/jupyterlite/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.165377 resotocore-3.6.1/resotocore/jupyterlite/api/contents/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-14 17:01:30.000000 resotocore-3.6.1/resotocore/jupyterlite/api/contents/all.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.165377 resotocore-3.6.1/resotocore/jupyterlite/api/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 17:01:30.000000 resotocore-3.6.1/resotocore/jupyterlite/api/translations/all.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 17:01:30.000000 resotocore-3.6.1/resotocore/jupyterlite/api/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/bootstrap.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.285378 resotocore-3.6.1/resotocore/jupyterlite/build/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1037.51967a2.js
--rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1079.cdbaf67.js
--rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1084.4cd1c89.js
--rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1113.23c9417.js
--rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1125.129d070.js
--rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1163.ac28297.js
--rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1221.c51249a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1245.be46619.js
--rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1261.199fc1d.js
--rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1272.f334098.js
--rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1278.0524a4a.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1290.3981211.js
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1295.46e72b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1310.23bbe67.js
--rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1320.21effe3.js
--rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1325.f76267c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1408.7461890.js
--rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1440.a9e7ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1483.616d9ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1489.e50b6d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1507.5705605.js
--rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/152.525d460.js
--rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1520.4e2eb21.js
--rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1555.e188f3f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1559.7c89925.js
--rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/160.5f28731.js
--rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1603.370a2a6.js
--rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1644.0e49167.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1667.f0afb2b.js
--rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1687.27f1ad6.js
--rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1725.f151c33.js
--rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1767.c8c2f26.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1806.1aaf66b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1838.1202b16.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1909.28a2def.js
--rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1989.88d258f.js
--rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2030.1562cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2047.baed97b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2099.f4b6fcd.js
--rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2118.5b65f70.js
--rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/213.5769e57.js
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2161.dcb27b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2169.635c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/217.90d10e2.js
--rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2212.72be094.js
--rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2287.997c38e.js
--rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2303.9ff8710.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2319.6b4cbb7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2329.4c5ca6d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2351.fbd96d8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2358.d5cf7c8.js
--rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2359.6451c3e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/237.f765e77.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2384.71782be.js
--rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/240.cddc46b.js
--rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2431.648d237.js
--rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2546.1f48267.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2557.75e9da2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/261.5f53c0e.js
--rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2629.c0e1cd6.js
--rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2788.46acc8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2834.942acc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2887.47ba752.js
--rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2956.8880209.js
--rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2973.2a51dc4.js
--rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3004.255e79c.js
--rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/302.8bcc38f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3037.70ee38d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3042.7cfad84.js
--rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3051.34fac68.js
--rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3122.2289fca.js
--rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3151.10ef4de.js
--rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/316.c850a76.js
--rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3196.4e35a17.js
--rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3265.a80440a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3277.9c04e75.js
--rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/330.126fa98.js
--rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3392.29fe6b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3413.480a49d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3444.47d5ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3469.7d14d0b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3546.fee1bd7.js
--rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/362.6716970.js
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3708.410d087.js
--rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3752.8735345.js
--rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3850.903abc2.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3880.bd39dce.js
--rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3970.236586f.js
--rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3976.58893b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3979.385527e.js
--rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/400.d72234b.js
--rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4018.1a35967.js
--rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/406.9b7af92.js
--rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4117.a8107fd.js
--rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4182.e2430f9.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4191.02bbea8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4197.53ab10b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4206.a5f8bb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4207.0d0580b.js
--rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4262.bb73457.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4298.5ee510c.js
--rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/44.0cfa785.js
--rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4410.e4a25d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4466.64d23d1.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4507.8b41ef4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/451.d9683ad.js
--rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4535.34b060a.js
--rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4565.43bdb91.js
--rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4569.f374f9d.js
--rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4615.eb5d40a.js
--rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4658.090d4a9.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4665.aa19a41.js
--rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4668.f65690b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4690.3dd4096.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4715.e7690b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4749.46ebbb2.js
--rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4750.56c06ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4856.2d7415f.js
--rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4875.375150e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/489.b981dea.js
--rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/490.c2624d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4905.667bf33.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4931.430433b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4942.b96c164.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5016.dd2fe83.js
--rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5072.733a1b5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/509.6448878.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5096.8ed0d8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5126.eecad7a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5129.1ba4763.js
--rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5153.763d8fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5155.06b4ea9.js
--rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5193.e9f6866.js
--rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5213.3e1a360.js
--rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5227.8c8acd8.js
--rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5238.1751cc3.js
--rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/528.2262cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5292.79d4aba.js
--rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5437.31236f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5489.848a8cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5508.317fca3.js
--rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/554.ac98303.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/555.2cd31dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5573.ebcdb93.js
--rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5666.c5e5324.js
--rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5710.70d0b1d.js
--rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5747.94ad626.js
--rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/582.21b8e7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5823.5045bdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5851.30b7b2a.js
--rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5878.32d92fa.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5880.68f975b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5955.88508f7.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5971.88c5642.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6080.aa0ff24.js
--rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/61.2808a0d.js
--rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6136.b8ba2b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6141.9831d58.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6475.6037fbb.js
--rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6493.d796aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6556.b3d9293.js
--rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6571.2c8884e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6576.3ea568e.js
--rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6591.94ed352.js
--rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6612.1632879.js
--rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6623.ae3b3cc.js
--rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6664.2160109.js
--rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6747.47be7f5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6748.be68f5f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6870.7940288.js
--rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6879.c8367a5.js
--rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6898.9bbc12a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6952.f68b818.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6985.321ad92.js
--rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6993.32cf9a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6997.b06fe71.js
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7041.d4f561e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7058.805c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7174.6c45206.js
--rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7334.8859b1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7359.6ee65ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7364.195178b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7380.58a4413.js
--rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7427.f9c2017.js
--rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7463.18fd278.js
--rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7509.1e0189e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7526.1a303e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7537.1323a15.js
--rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7692.33d5169.js
--rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7746.5908d29.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7808.1d582a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/783.c156751.js
--rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7858.2386e4d.js
--rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7941.01ea680.js
--rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8005.c5ad7b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8028.39e2fa1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8061.cc62561.js
--rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8101.cf46d02.js
--rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/812.9b0e86e.js
--rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/816.c8050f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8165.b2c3285.js
--rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8232.a578bf9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/824.8678196.js
--rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8270.89fe7e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/833.9cc6653.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8370.8f855e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8373.96b0b3a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8389.ffe031f.js
--rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8412.1528057.js
--rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8427.4923f43.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8542.027afdc.js
--rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8594.0112f03.js
--rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8656.d5b8e92.js
--rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8685.d78bdab.js
--rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8698.9817d75.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8732.9320f73.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8741.b138cb8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8785.cf4fe95.js
--rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8828.77c71d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8883.80c7b63.js
--rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8976.3816942.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8981.99a4275.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8990.2a453cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9035.1e45c1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9053.45b77fc.js
--rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9077.fefb6ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9128.b8fa6f0.js
--rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9156.0cefbd3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9170.0023587.js
--rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9196.315f9f9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9198.9971d70.js
--rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/920.d15c177.js
--rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9253.0b31caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9266.bacd0dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9307.c3a00ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9321.869e413.js
--rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9344.ba0abcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9382.9014799.js
--rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9440.1b10b8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9464.79e6ac5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9502.9a24831.js
--rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9507.1e6cc5d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9602.62bf0f1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9621.e2e8b5d.js
--rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9622.ccab065.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9626.a178bd0.js
--rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9647.ed91993.js
--rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9657.bc5c60e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/97.ad126b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9712.796a0a1.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9733.a3b2a7f.js
--rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9737.7dc8f98.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9777.0b8a504.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9793.6d63a85.js
--rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9806.652c162.js
--rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9865.2e3db6f.js
--rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/989.bcca86a.js
--rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9943.f3f35c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9958.25c8c06.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9960.64cd61e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/add-above.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/add-below.svg
--rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/add.svg
--rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/bug-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/bug.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/build.svg
--rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-down-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-down-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-up-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/case-sensitive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/circle-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/clear.svg
--rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/copyright.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/cut.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/duplicate.svg
--rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/ellipses.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/extension.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fast-forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/file-upload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/filter-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/folder-favorite.svg
--rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/html5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/inspector.svg
--rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/json.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/julia.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/jupyter-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/jupyter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/keyboard.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/lab/
--rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/lab/bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/launch.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/launcher.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/line-form.svg
--rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/list.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/listings-info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/markdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/move-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/move-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/new-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/not-trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/numbering.svg
--rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/offline-bolt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/palette.svg
--rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/paste.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/python.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/r-kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/react.svg
--rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/regex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/run.svg
--rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/running.svg
--rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.137377 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
--rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.297378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.297378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.297378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
--rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
--rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.137377 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
--rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/all.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/service-worker-b2fb40a.js
--rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/spreadsheet.svg
--rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/table-rows.svg
--rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/tag.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/text-editor.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.137377 resotocore-3.6.1/resotocore/jupyterlite/build/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.137377 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/toc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/tree-view.svg
--rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/vega.svg
--rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/yaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/config-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.141377 resotocore-3.6.1/resotocore/jupyterlite/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/doc/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/doc/workspaces/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.141377 resotocore-3.6.1/resotocore/jupyterlite/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.141377 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.313378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.313378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.317378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
--rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.317378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.321378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
--rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.321378 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.329378 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
--rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.329378 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/
--rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.329378 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/jupyterlite/files/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-14 17:01:30.000000 resotocore-3.6.1/resotocore/jupyterlite/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/jupyterlite.schema.v0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/kernelspecs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/kernelspecs/javascript.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/lab/
--rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/lab/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/lab/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/workspaces/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/service-worker-b2fb40a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/tree/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.337378 resotocore-3.6.1/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/adjust_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/db_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/graph_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    58798 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/resolve_in_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/transform_kind_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/typed_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.341378 resotocore-3.6.1/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50309 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/query_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/template_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/template_expander_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.341378 resotocore-3.6.1/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/report/benchmark_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/report/inspector_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/report/report_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.341378 resotocore-3.6.1/resotocore/static/
--rw-r--r--   0 runner    (1001) docker     (123)   130266 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/api-doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/ck-unicode-truecolor.ans
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.341378 resotocore-3.6.1/resotocore/static/report/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.141377 resotocore-3.6.1/resotocore/static/report/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.345378 resotocore-3.6.1/resotocore/static/report/benchmark/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/benchmark_template.json
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/check_template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.145377 resotocore-3.6.1/resotocore/static/report/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.345378 resotocore-3.6.1/resotocore/static/report/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_apigateway.json
--rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_cloudtrail.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_ec2.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_efs.json
--rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_iam.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_kms.json
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_lambda.json
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_rds.json
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_s3.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/resoto.css
--rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/resoto_logo_and_text.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/system_start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.349378 resotocore-3.6.1/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/job_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/start_workflow_on_first_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/subscribers.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/task_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    32516 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    29621 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.349378 resotocore-3.6.1/resotocore/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/templates/create_first_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.349378 resotocore-3.6.1/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/user/user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.353378 resotocore-3.6.1/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65625 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/certificate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/content_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/worker_task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.153377 resotocore-3.6.1/resotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34535 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:01:35.000000 resotocore-3.6.1/resotocore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-14 17:01:36.377378 resotocore-3.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.353378 resotocore-3.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.357378 resotocore-3.6.1/tests/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.357378 resotocore-3.6.1/tests/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/analytics/posthog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/analytics/recurrent_events_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.357378 resotocore-3.6.1/tests/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/cli/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    59406 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/cli/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/cli/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.361378 resotocore-3.6.1/tests/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/config/config_handler_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/config/config_override_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/config/core_config_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29325 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/console_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/core_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.365378 resotocore-3.6.1/tests/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/arango_query_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/arangodb_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/async_arangodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/configdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/db_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    31108 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/graphdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/jobdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/modeldb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/runningtaskdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/subscriberdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/system_data_db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/templatedb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/dependencies_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.365378 resotocore-3.6.1/tests/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/graph_manager/graph_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/hypothesis_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.369378 resotocore-3.6.1/tests/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/infra_apps/local_runtime_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/infra_apps/package_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/message_bus_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.369378 resotocore-3.6.1/tests/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/adjust_node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/db_updater_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/graph_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/json_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/model_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/resolve_in_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/typed_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.373378 resotocore-3.6.1/tests/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/query/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/query/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/query/template_expander_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.373378 resotocore-3.6.1/tests/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/report/benchnmark_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/report/inspector_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.373378 resotocore-3.6.1/tests/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/job_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/subscribers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/task_description_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/task_handler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.373378 resotocore-3.6.1/tests/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/user/user_management_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/validator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.377378 resotocore-3.6.1/tests/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/certificate_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/content_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/worker_task_queue_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.942369 resotocore-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 22:06:18.000000 resotocore-3.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-21 22:06:18.000000 resotocore-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-07-21 22:10:27.942369 resotocore-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-21 22:06:18.000000 resotocore-3.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-21 22:06:18.000000 resotocore-3.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.842367 resotocore-3.6.2/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.842367 resotocore-3.6.2/resotocore/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/action_handlers/merge_outer_edge_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.842367 resotocore-3.6.2/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/analytics/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/analytics/recurrent_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/async_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.842367 resotocore-3.6.2/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31057 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   242914 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/cli/tip_of_the_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.842367 resotocore-3.6.2/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/config/config_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/config/config_override_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/config/core_config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/console_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/core_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.846367 resotocore-3.6.2/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34739 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/arango_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/arangodb_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/configdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/deferredouteredgedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65689 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/graphdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/packagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/runningtaskdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/subscriberdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/system_data_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/templatedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/db/usagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.846367 resotocore-3.6.2/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/graph_manager/graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.846367 resotocore-3.6.2/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/infra_apps/local_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/infra_apps/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/infra_apps/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/infra_apps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.850367 resotocore-3.6.2/resotocore/jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.830367 resotocore-3.6.2/resotocore/jupyterlite/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.850367 resotocore-3.6.2/resotocore/jupyterlite/api/contents/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-21 22:10:23.000000 resotocore-3.6.2/resotocore/jupyterlite/api/contents/all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.850367 resotocore-3.6.2/resotocore/jupyterlite/api/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 22:10:23.000000 resotocore-3.6.2/resotocore/jupyterlite/api/translations/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 22:10:23.000000 resotocore-3.6.2/resotocore/jupyterlite/api/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/bootstrap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.906368 resotocore-3.6.2/resotocore/jupyterlite/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1037.51967a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1079.cdbaf67.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1084.4cd1c89.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1113.23c9417.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1125.129d070.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1163.ac28297.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1221.c51249a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1245.be46619.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1261.199fc1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1272.f334098.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1278.0524a4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1290.3981211.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1295.46e72b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1310.23bbe67.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1320.21effe3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1325.f76267c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1408.7461890.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1440.a9e7ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1483.616d9ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1489.e50b6d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1507.5705605.js
+-rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/152.525d460.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1520.4e2eb21.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1555.e188f3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1559.7c89925.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/160.5f28731.js
+-rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1603.370a2a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1644.0e49167.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1667.f0afb2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1687.27f1ad6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1725.f151c33.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1767.c8c2f26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1806.1aaf66b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1838.1202b16.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1909.28a2def.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/1989.88d258f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2030.1562cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2047.baed97b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2099.f4b6fcd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2118.5b65f70.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/213.5769e57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2161.dcb27b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2169.635c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/217.90d10e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2212.72be094.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2287.997c38e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2303.9ff8710.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2319.6b4cbb7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2329.4c5ca6d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2351.fbd96d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2358.d5cf7c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2359.6451c3e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/237.f765e77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2384.71782be.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/240.cddc46b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2431.648d237.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2546.1f48267.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2557.75e9da2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/261.5f53c0e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2629.c0e1cd6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2788.46acc8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2834.942acc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2887.47ba752.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2956.8880209.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/2973.2a51dc4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3004.255e79c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/302.8bcc38f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3037.70ee38d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3042.7cfad84.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3051.34fac68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3122.2289fca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3151.10ef4de.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/316.c850a76.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3196.4e35a17.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3265.a80440a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3277.9c04e75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/330.126fa98.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3392.29fe6b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3413.480a49d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3444.47d5ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3469.7d14d0b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3546.fee1bd7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/362.6716970.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3708.410d087.js
+-rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3752.8735345.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3850.903abc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3880.bd39dce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3970.236586f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3976.58893b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/3979.385527e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/400.d72234b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4018.1a35967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/406.9b7af92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4117.a8107fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4182.e2430f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4191.02bbea8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4197.53ab10b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4206.a5f8bb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4207.0d0580b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4262.bb73457.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4298.5ee510c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/44.0cfa785.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4410.e4a25d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4466.64d23d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4507.8b41ef4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/451.d9683ad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4535.34b060a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4565.43bdb91.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4569.f374f9d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4615.eb5d40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4658.090d4a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4665.aa19a41.js
+-rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4668.f65690b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4690.3dd4096.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4715.e7690b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4749.46ebbb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4750.56c06ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4856.2d7415f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4875.375150e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/489.b981dea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/490.c2624d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4905.667bf33.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4931.430433b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/4942.b96c164.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5016.dd2fe83.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5072.733a1b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/509.6448878.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5096.8ed0d8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5126.eecad7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5129.1ba4763.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5153.763d8fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5155.06b4ea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5193.e9f6866.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5213.3e1a360.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5227.8c8acd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5238.1751cc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/528.2262cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5292.79d4aba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5437.31236f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5489.848a8cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5508.317fca3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/554.ac98303.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/555.2cd31dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5573.ebcdb93.js
+-rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5666.c5e5324.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5710.70d0b1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5747.94ad626.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/582.21b8e7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5823.5045bdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5851.30b7b2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5878.32d92fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5880.68f975b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5955.88508f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/5971.88c5642.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6080.aa0ff24.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/61.2808a0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6136.b8ba2b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6141.9831d58.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6475.6037fbb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6493.d796aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6556.b3d9293.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6571.2c8884e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6576.3ea568e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6591.94ed352.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6612.1632879.js
+-rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6623.ae3b3cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6664.2160109.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6747.47be7f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6748.be68f5f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6870.7940288.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6879.c8367a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6898.9bbc12a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6952.f68b818.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6985.321ad92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6993.32cf9a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/6997.b06fe71.js
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7041.d4f561e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7058.805c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7174.6c45206.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7334.8859b1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7359.6ee65ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7364.195178b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7380.58a4413.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7427.f9c2017.js
+-rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7463.18fd278.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7509.1e0189e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7526.1a303e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7537.1323a15.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7692.33d5169.js
+-rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7746.5908d29.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7808.1d582a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/783.c156751.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7858.2386e4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/7941.01ea680.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8005.c5ad7b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8028.39e2fa1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8061.cc62561.js
+-rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8101.cf46d02.js
+-rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/812.9b0e86e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/816.c8050f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8165.b2c3285.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8232.a578bf9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/824.8678196.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8270.89fe7e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/833.9cc6653.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8370.8f855e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8373.96b0b3a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8389.ffe031f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8412.1528057.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8427.4923f43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8542.027afdc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8594.0112f03.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8656.d5b8e92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8685.d78bdab.js
+-rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8698.9817d75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8732.9320f73.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8741.b138cb8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8785.cf4fe95.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8828.77c71d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8883.80c7b63.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8976.3816942.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8981.99a4275.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/8990.2a453cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9035.1e45c1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9053.45b77fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9077.fefb6ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9128.b8fa6f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9156.0cefbd3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9170.0023587.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9196.315f9f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9198.9971d70.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/920.d15c177.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9253.0b31caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9266.bacd0dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9307.c3a00ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9321.869e413.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9344.ba0abcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9382.9014799.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9440.1b10b8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9464.79e6ac5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9502.9a24831.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9507.1e6cc5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9602.62bf0f1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9621.e2e8b5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9622.ccab065.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9626.a178bd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9647.ed91993.js
+-rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9657.bc5c60e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/97.ad126b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9712.796a0a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9733.a3b2a7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9737.7dc8f98.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9777.0b8a504.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9793.6d63a85.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9806.652c162.js
+-rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9865.2e3db6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/989.bcca86a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9943.f3f35c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9958.25c8c06.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/9960.64cd61e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/add-above.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/add-below.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/bug-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/bug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/build.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/caret-down-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/caret-down-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/caret-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/caret-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/caret-up-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/caret-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/case-sensitive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/circle-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/clear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/copyright.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/cut.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/duplicate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/ellipses.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/extension.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/fast-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/file-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/filter-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/folder-favorite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/html5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/inspector.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/json.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/julia.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/jupyter-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/jupyter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/keyboard.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.906368 resotocore-3.6.2/resotocore/jupyterlite/build/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/lab/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/launch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/launcher.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/line-form.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/listings-info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/markdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/move-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/move-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/new-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/not-trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/numbering.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/offline-bolt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/palette.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/r-kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/react.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/regex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/run.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/running.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.906368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.834367 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.906368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.906368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.906368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.906368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.910368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.834367 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@retrolab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/schemas/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/service-worker-b2fb40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/spreadsheet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/table-rows.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/tag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/text-editor.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.834367 resotocore-3.6.2/resotocore/jupyterlite/build/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.834367 resotocore-3.6.2/resotocore/jupyterlite/build/themes/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/toc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/tree-view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/vega.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/build/yaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/config-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.834367 resotocore-3.6.2/resotocore/jupyterlite/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/doc/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/doc/workspaces/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.834367 resotocore-3.6.2/resotocore/jupyterlite/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.834367 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.914368 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.918368 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.918368 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.918368 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-07-21 22:10:20.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.918368 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.922368 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-07-21 22:10:11.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.922368 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.926369 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-07-21 22:10:17.000000 resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.926369 resotocore-3.6.2/resotocore/jupyterlite/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/jupyterlite/files/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-21 22:10:23.000000 resotocore-3.6.2/resotocore/jupyterlite/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/jupyterlite.schema.v0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.926369 resotocore-3.6.2/resotocore/jupyterlite/kernelspecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/kernelspecs/javascript.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.926369 resotocore-3.6.2/resotocore/jupyterlite/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/lab/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/lab/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/lab/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/lab/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/lab/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.926369 resotocore-3.6.2/resotocore/jupyterlite/lab/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/lab/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.926369 resotocore-3.6.2/resotocore/jupyterlite/lab/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/lab/workspaces/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/service-worker-b2fb40a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.926369 resotocore-3.6.2/resotocore/jupyterlite/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.6.2/resotocore/jupyterlite/tree/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.926369 resotocore-3.6.2/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/adjust_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/db_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26960 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/graph_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58697 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/resolve_in_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/transform_kind_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/model/typed_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.930369 resotocore-3.6.2/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50309 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/query/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/query/query_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/query/template_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/query/template_expander_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.930369 resotocore-3.6.2/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/report/benchmark_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/report/inspector_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/report/report_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.930369 resotocore-3.6.2/resotocore/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   130266 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/api-doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/ck-unicode-truecolor.ans
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.930369 resotocore-3.6.2/resotocore/static/report/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.838367 resotocore-3.6.2/resotocore/static/report/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.930369 resotocore-3.6.2/resotocore/static/report/benchmark/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/benchmark_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/check_template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.838367 resotocore-3.6.2/resotocore/static/report/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.930369 resotocore-3.6.2/resotocore/static/report/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_apigateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_cloudtrail.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_ec2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_efs.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_iam.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_kms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_lambda.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_rds.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/report/checks/aws/aws_s3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/resoto.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/static/resoto_logo_and_text.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/system_start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.934369 resotocore-3.6.2/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/task/job_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/task/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/task/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/task/start_workflow_on_first_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/task/subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/task/task_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/task/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30387 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/task/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.934369 resotocore-3.6.2/resotocore/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/templates/create_first_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.934369 resotocore-3.6.2/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/user/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.934369 resotocore-3.6.2/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65625 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/web/certificate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/web/content_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/web/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/web/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-07-21 22:06:18.000000 resotocore-3.6.2/resotocore/worker_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.842367 resotocore-3.6.2/resotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-07-21 22:10:27.000000 resotocore-3.6.2/resotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-07-21 22:10:27.000000 resotocore-3.6.2/resotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:10:27.000000 resotocore-3.6.2/resotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 22:10:27.000000 resotocore-3.6.2/resotocore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:10:27.000000 resotocore-3.6.2/resotocore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 22:10:27.000000 resotocore-3.6.2/resotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 22:10:27.000000 resotocore-3.6.2/resotocore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-21 22:10:27.942369 resotocore-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.934369 resotocore-3.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.934369 resotocore-3.6.2/tests/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.934369 resotocore-3.6.2/tests/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/analytics/posthog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/analytics/recurrent_events_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.938369 resotocore-3.6.2/tests/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/cli/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59677 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/cli/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/cli/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.938369 resotocore-3.6.2/tests/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/config/config_handler_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/config/config_override_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/config/core_config_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29372 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/console_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/core_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.938369 resotocore-3.6.2/tests/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/arango_query_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/arangodb_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/async_arangodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/configdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/db_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/deferredouteredgedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31337 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/graphdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/jobdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/modeldb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/runningtaskdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/subscriberdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/system_data_db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/db/templatedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/dependencies_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.938369 resotocore-3.6.2/tests/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/graph_manager/graph_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/hypothesis_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.938369 resotocore-3.6.2/tests/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/infra_apps/local_runtime_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/infra_apps/package_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/message_bus_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.942369 resotocore-3.6.2/tests/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/model/adjust_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/model/db_updater_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/model/graph_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/model/json_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/model/model_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/model/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/model/resolve_in_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/model/typed_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.942369 resotocore-3.6.2/tests/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/query/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/query/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/query/template_expander_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.942369 resotocore-3.6.2/tests/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/report/benchnmark_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/report/inspector_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.942369 resotocore-3.6.2/tests/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/task/job_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/task/subscribers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/task/task_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/task/task_handler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.942369 resotocore-3.6.2/tests/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/user/user_management_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/validator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:27.942369 resotocore-3.6.2/tests/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/web/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/web/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/web/certificate_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/web/content_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-21 22:06:18.000000 resotocore-3.6.2/tests/resotocore/worker_task_queue_test.py
```

### Comparing `resotocore-3.6.1/LICENSE` & `resotocore-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/PKG-INFO` & `resotocore-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.6.1
+Version: 3.6.2
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotocore-3.6.1/README.md` & `resotocore-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/pyproject.toml` & `resotocore-3.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotocore"
-version = "3.6.1"
+version = "3.6.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Keeps all the things."
 license = {file="LICENSE"}
 urls = {"Homepage" = "https://resoto.com"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
```

### Comparing `resotocore-3.6.1/resotocore/__main__.py` & `resotocore-3.6.2/resotocore/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from resotocore.infra_apps.package_manager import PackageManager
 from resotocore.message_bus import MessageBus
 from resotocore.model.db_updater import GraphMerger
 from resotocore.model.model_handler import ModelHandlerDB
 from resotocore.model.typed_model import to_json, class_fqn
 from resotocore.query.template_expander_service import TemplateExpanderService
 from resotocore.report.inspector_service import InspectorService
-from resotocore.task.scheduler import Scheduler
+from resotocore.task.scheduler import APScheduler, NoScheduler
 from resotocore.task.subscribers import SubscriptionHandler
 from resotocore.task.task_handler import TaskHandlerService
 from resotocore.user.user_management import UserManagementService
 from resotocore.util import shutdown_process, utc
 from resotocore.web.api import Api
 from resotocore.web.certificate_handler import CertificateHandler
 from resotocore.worker_task_queue import WorkerTaskQueue
@@ -144,15 +144,15 @@
         ServiceNames.event_sender, PostHogEventSender(system_data) if config.runtime.usage_metrics else NoEventSender()
     )
     db = deps.add(ServiceNames.db_access, db_access(config, sdb, event_sender))
     api = deps.add("api", Api(deps))
 
     async def on_start() -> None:
         message_bus = deps.add(ServiceNames.message_bus, MessageBus())
-        scheduler = deps.add(ServiceNames.scheduler, Scheduler())
+        scheduler = deps.add(ServiceNames.scheduler, APScheduler() if not config.args.no_scheduling else NoScheduler())
         model = deps.add(ServiceNames.model_handler, ModelHandlerDB(db, config.runtime.plantuml_server))
 
         worker_task_queue = deps.add(ServiceNames.worker_task_queue, WorkerTaskQueue())
         # a "real" config override deps.add, unlike the one used for core config
         config_override_service = deps.add(
             ServiceNames.config_override,
             ConfigOverrideService(config_overrides_paths, partial(model_from_db, db.configs_model_db)),
@@ -217,16 +217,17 @@
                 message_bus,
                 timedelta(hours=1),
                 timedelta(hours=1),
             ),
         )
         # queue must be created inside an async function!
         deps.add(ServiceNames.forked_tasks, Queue())
-        for srv in deps.services:
-            await srv.start()
+
+        # start all dependencies
+        await deps.start()
 
         if created:
             docker = inside_docker()
             kubernetes = inside_kubernetes()
             helm = helm_installation()
             await event_sender.core_event(
                 CoreEvent.SystemInstalled,
@@ -250,16 +251,15 @@
             mem_total=info.mem_total,
             mem_available=info.mem_available,
         )
 
     async def on_stop() -> None:
         duration = utc() - info.started_at
         await event_sender.core_event(CoreEvent.SystemStopped, total_seconds=int(duration.total_seconds()))
-        for srv in reversed(deps.services):
-            await srv.stop()
+        await deps.stop()
 
     async def async_initializer() -> Application:
         async def clean_all_tasks() -> None:
             log.info("Clean up all running tasks.")
             for task in asyncio.all_tasks():
                 with suppress(asyncio.CancelledError):
                     if not task.done() or not task.cancelled():
```

### Comparing `resotocore-3.6.1/resotocore/action_handlers/merge_outer_edge_handler.py` & `resotocore-3.6.2/resotocore/action_handlers/merge_outer_edge_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,19 +38,20 @@
         self.subscription_handler = subscription_handler
         self.subscriber: Optional[Subscriber] = None
         self.task_handler_service = task_handler_service
         self.db_access = db_access
         self.model_handler = model_handler
 
     async def merge_outer_edges(self, task_id: TaskId) -> Tuple[int, int]:
-        pending_outer_edge_db = self.db_access.pending_deferred_edge_db
-        pending_edges = await pending_outer_edge_db.get(task_id)
+        deferred_outer_edge_db = self.db_access.deferred_outer_edge_db
+        pending_edges = await deferred_outer_edge_db.all_for_task(task_id)
         if pending_edges:
-            graph_db = self.db_access.get_graph_db(pending_edges.graph)
-            model = await self.model_handler.load_model(pending_edges.graph)
+            first = pending_edges[0]
+            graph_db = self.db_access.get_graph_db(first.graph)
+            model = await self.model_handler.load_model(first.graph)
 
             async def find_node_id(selector: NodeSelector) -> Optional[NodeId]:
                 try:
                     if isinstance(selector, ByNodeId):
                         node = await graph_db.get_node(model, selector.value)
                         return node.get("id") if node else None
                     else:
@@ -66,36 +67,37 @@
 
                         return next(iter(results), {}).get("id", None)  # type: ignore
                 except Exception as e:
                     log.warning(f"task_id: {task_id}: Error {e} when finding node {selector}")
                     return None
 
             edges: List[Tuple[NodeId, NodeId, str]] = []
-            for edge in pending_edges.edges:
-                from_id = await find_node_id(edge.from_node)
-                to_id = await find_node_id(edge.to_node)
-                if from_id and to_id:
-                    edges.append((from_id, to_id, edge.edge_type))
+            for pending_edge in pending_edges:
+                for edge in pending_edge.edges:
+                    from_id = await find_node_id(edge.from_node)
+                    to_id = await find_node_id(edge.to_node)
+                    if from_id and to_id:
+                        edges.append((from_id, to_id, edge.edge_type))
 
-            updated, deleted = await graph_db.update_deferred_edges(edges, pending_edges.created_at)
+            updated, deleted = await graph_db.update_deferred_edges(edges, first.created_at)
 
             log.info(
-                f"MergeOuterEdgesHandler: updated {updated}/{len(pending_edges.edges)},"
+                f"MergeOuterEdgesHandler: updated {updated}/{len(edges)},"
                 f"  deleted {deleted} edges in task id {task_id}"
             )
 
-            return (updated, deleted)
+            return updated, deleted
         else:
             log.info(f"MergeOuterEdgesHandler: no pending edges for task id {task_id} found.")
 
-            return (0, 0)
+            return 0, 0
 
     async def mark_done(self, task_id: TaskId) -> None:
-        pending_outer_edge_db = self.db_access.pending_deferred_edge_db
-        await pending_outer_edge_db.delete(task_id)
+        deferred_outer_edge_db = self.db_access.deferred_outer_edge_db
+        await deferred_outer_edge_db.delete_for_task(task_id)
 
     async def __handle_events(self, subscription_done: Future[None]) -> None:
         async with self.message_bus.subscribe(subscriber_id, [merge_outer_edges]) as events:
             subscription_done.set_result(None)
             while True:
                 event = await events.get()
                 if isinstance(event, Action) and event.message_type == merge_outer_edges:
```

### Comparing `resotocore-3.6.1/resotocore/analytics/__init__.py` & `resotocore-3.6.2/resotocore/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/analytics/posthog.py` & `resotocore-3.6.2/resotocore/analytics/posthog.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/analytics/recurrent_events.py` & `resotocore-3.6.2/resotocore/analytics/recurrent_events.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/async_extensions.py` & `resotocore-3.6.2/resotocore/async_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/cli/__init__.py` & `resotocore-3.6.2/resotocore/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/cli/cli.py` & `resotocore-3.6.2/resotocore/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,16 +324,14 @@
             task, _ = self.dependencies.forked_tasks.get_nowait()
             loop = asyncio.get_event_loop()
             with suppress(asyncio.CancelledError):
                 if not task.done() or not task.cancelled():
                     task.cancel()
                 loop.run_until_complete(task)
 
-        await self.dependencies.stop()
-
     async def reap_tasks(self) -> None:
         while True:
             try:
                 task, info = await self.dependencies.forked_tasks.get()
                 try:
                     res = await task
                     log.info(f"Spawned task {info} completed with: {res}")
```

### Comparing `resotocore-3.6.1/resotocore/cli/command.py` & `resotocore-3.6.2/resotocore/cli/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -4025,23 +4025,25 @@
 
 class WorkflowsCommand(CLICommand):
     """
     ```shell
     workflows list
     workflows show <id>
     workflows run <id>
+    workflows stop <task_id>
     workflows running
     workflows history
     workflows history <id> --started-before <date> --started-after <date> --has-errors --limit <num>
     workflows log <workflow-run-id>
     ```
 
     - `workflows list`: get the list of all workflows in the system
     - `workflows show <id>`: show the current definition of the workflow defined by given identifier.
     - `workflows run <id>`: run the workflow as if the trigger would be triggered.
+    - `workflows stop <task_id>`: stop a running workflow execution.
     - `workflows running`: show all currently running workflows.
     - `workflows history`: aggregated history of all workflows.
     - `workflows history <id>`: show all runs of this workflow based on defined filter criteria.
     - `workflows log <workflow-run-id>`: show the log of the workflow run.
 
     The workflows that currently available are all hard-wired into resotocore.
     We will support user defined workflows in the future.
@@ -4164,14 +4166,15 @@
         return "Manage all workflows."
 
     def args_info(self) -> ArgsInfo:
         return {
             "show": [ArgInfo(None, help_text="<workflow-id>")],
             "list": [],
             "run": [ArgInfo(None, help_text="<workflow-id>")],
+            "stop": [ArgInfo(None, help_text="<task-id>")],
             "running": [],
             "history": [
                 ArgInfo(None, help_text="<workflow-id>"),
                 ArgInfo("--started-before", help_text="<date>", value_hint="date", expects_value=True),
                 ArgInfo("--started-after", help_text="<date>", value_hint="date", expects_value=True),
                 ArgInfo("--limit", help_text="<number of entries>", expects_value=True),
                 ArgInfo("--has-errors"),
@@ -4278,25 +4281,33 @@
             )
             cursor: AsyncCursor = context.cursor
             try:
                 return cursor.count() or 0, stream.map(cursor, running_task_data)
             finally:
                 cursor.close()
 
+        async def stop_workflow(task_id: TaskId) -> AsyncIterator[str]:
+            if await self.dependencies.task_handler.stop_task(task_id) is not None:
+                yield f"Workflow Task {task_id} stopped."
+            else:
+                yield "No running workflow with this id."
+
         args = re.split("\\s+", arg, maxsplit=1) if arg else []
         if arg and len(args) == 2 and args[0] == "show":
             return CLISource.single(partial(show_workflow, args[1].strip()))
         elif arg and len(args) == 1 and args[0] == "history":
             return CLISource.single(history_aggregation)
         elif arg and len(args) == 2 and args[0] == "history":
             return CLISource(partial(history_of, re.split("\\s+", args[1])))
         elif arg and len(args) == 2 and args[0] == "log":
             return CLISource(partial(show_log, args[1].strip()))
         elif arg and len(args) == 2 and args[0] == "run":
             return CLISource.single(partial(run_workflow, args[1].strip()))
+        elif arg and len(args) == 2 and args[0] == "stop":
+            return CLISource.single(partial(stop_workflow, args[1].strip()))
         elif arg and len(args) == 1 and args[0] == "running":
             return CLISource(running_workflows)
         elif arg and len(args) == 1 and args[0] == "list":
             return CLISource(list_workflows)
         else:
             return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
 
@@ -5696,15 +5707,19 @@
                     query = Query(parts=[Part(term=IsTerm(["graph_root"]), navigation=NavigateUntilLeaf)])
                     graph_db = self.dependencies.db_access.get_graph_db(ctx.graph_name)
                     async with await graph_db.search_graph_gen(
                         QueryModel(query, resoto_model), timeout=timedelta(weeks=200000)
                     ) as cursor:
                         await sync_fn(query=query, in_stream=stream.iterate(cursor))
 
-                yield FilePath.user_local(p.database, file_output).json() if file_output else "Database synchronized."
+                if file_output is not None:
+                    assert p.database, "No database name provided. Use the --database <name> argument."
+                    yield FilePath.user_local(p.database, file_output).json()
+                else:
+                    yield "Database synchronized."
 
         async def database_synchronize(
             engine_config: EngineConfig,
             complete_model: bool,
             drop_existing_tables: bool,
             query: Optional[Query],
             in_stream: Stream,
@@ -5766,15 +5781,20 @@
             parser.add_argument("--port", type=int)
             parser.add_argument("--user", type=str)
             parser.add_argument("--password", type=str)
             parser.add_argument("--database", type=str)
             parser.add_argument("--arg", type=key_value_parser.parse, nargs="+", action="append", default=[])
             parser.add_argument("--complete-schema", action="store_true")
             parser.add_argument("--drop-existing-tables", action="store_true")
-            parser.add_argument("--batch-size", type=int, default=1000)
+            # Batch Size Restrictions:
+            # SQLite before 3.32.0: 999
+            # MySQL/MariaDB: 16MB batch size
+            # Postgres/Snowflake: no limit other than available memory
+            # --> we use 999 as a safe default
+            parser.add_argument("--batch-size", type=int, default=999)
             parsed_args = parser.parse_args(args_parts_unquoted_parser.parse(args[1]))
             produces = MediaType.FilePath if parsed_args.db == "sqlite" else MediaType.Json
             if in_source_position:
                 # in this position we fall back to exporting the whole graph
                 return CLISource.single(
                     fn=partial(sync_database_result, parsed_args, None),
                     envelope={CLIEnvelope.no_history: "yes"},
@@ -5784,15 +5804,15 @@
                 # sync = partial(database_synchronize, db_config, p.complete_schema, p.drop_existing_tables, ctx.query)
                 return CLIFlow(
                     fn=partial(sync_database_result, parsed_args),
                     envelope={CLIEnvelope.no_history: "yes"},
                     produces=produces,
                 )
         else:
-            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+            raise AttributeError("Wrong or insufficient arguments. Execute `help db` to get more information.")
 
 
 def all_commands(d: Dependencies) -> List[CLICommand]:
     commands = [
         AggregateCommand(d, "search"),
         AggregateToCountCommand(d, "search"),
         AncestorsPart(d, "search"),
```

### Comparing `resotocore-3.6.1/resotocore/cli/model.py` & `resotocore-3.6.2/resotocore/cli/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/cli/tip_of_the_day.py` & `resotocore-3.6.2/resotocore/cli/tip_of_the_day.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/config/__init__.py` & `resotocore-3.6.2/resotocore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/config/config_handler_service.py` & `resotocore-3.6.2/resotocore/config/config_handler_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/config/config_override_service.py` & `resotocore-3.6.2/resotocore/config/config_override_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/config/core_config_handler.py` & `resotocore-3.6.2/resotocore/config/core_config_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/console_renderer.py` & `resotocore-3.6.2/resotocore/console_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/constants.py` & `resotocore-3.6.2/resotocore/constants.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/core_config.py` & `resotocore-3.6.2/resotocore/core_config.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/__init__.py` & `resotocore-3.6.2/resotocore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/arango_query.py` & `resotocore-3.6.2/resotocore/db/arango_query.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/arangodb_extensions.py` & `resotocore-3.6.2/resotocore/db/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/arangodb_functions.py` & `resotocore-3.6.2/resotocore/db/arangodb_functions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/async_arangodb.py` & `resotocore-3.6.2/resotocore/db/async_arangodb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/configdb.py` & `resotocore-3.6.2/resotocore/db/configdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/db_access.py` & `resotocore-3.6.2/resotocore/db/db_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from resotocore.analytics import AnalyticsEventSender
 from resotocore.async_extensions import run_async
 from resotocore.core_config import CoreConfig
 from resotocore.db import SystemData
 from resotocore.db.arangodb_extensions import ArangoHTTPClient
 from resotocore.db.async_arangodb import AsyncArangoDB
 from resotocore.db.configdb import config_entity_db, config_validation_entity_db
-from resotocore.db.deferred_edge_db import pending_deferred_edge_db
+from resotocore.db.deferredouteredgedb import deferred_outer_edge_db
 from resotocore.db.entitydb import EventEntityDb
 from resotocore.db.graphdb import ArangoGraphDB, GraphDB, EventGraphDB
 from resotocore.db.jobdb import job_db
 from resotocore.db.modeldb import ModelDb, model_db
 from resotocore.db.packagedb import app_package_entity_db
 from resotocore.db.runningtaskdb import running_task_db
 from resotocore.db.subscriberdb import subscriber_db
@@ -45,30 +45,30 @@
         arango_database: StandardDatabase,
         event_sender: AnalyticsEventSender,
         adjust_node: AdjustNode,
         config: CoreConfig,
         subscriber_name: str = "subscribers",
         running_task_name: str = "running_tasks",
         job_name: str = "jobs",
-        deferred_edge_name: str = "deferred_outer_edges",
+        deferred_outer_edge_name: str = "deferred_outer_edges",
         config_entity: str = "configs",
         config_validation_entity: str = "config_validation",
         configs_model: str = "configs_model",
         template_entity: str = "templates",
         infra_app_packages: str = "infra_app_packages",
     ):
         self.event_sender = event_sender
         self.database = arango_database
         self.db = AsyncArangoDB(arango_database)
         self.adjust_node = adjust_node
         self.graph_model_dbs: Dict[GraphName, ModelDb] = {}
         self.subscribers_db = EventEntityDb(subscriber_db(self.db, subscriber_name), event_sender, subscriber_name)
         self.system_data_db = SystemDataDb(self.db)
         self.running_task_db = running_task_db(self.db, running_task_name)
-        self.pending_deferred_edge_db = pending_deferred_edge_db(self.db, deferred_edge_name)
+        self.deferred_outer_edge_db = deferred_outer_edge_db(self.db, deferred_outer_edge_name)
         self.job_db = job_db(self.db, job_name)
         self.config_entity_db = config_entity_db(self.db, config_entity)
         self.config_validation_entity_db = config_validation_entity_db(self.db, config_validation_entity)
         self.configs_model_db = model_db(self.db, configs_model)
         self.template_entity_db = template_entity_db(self.db, template_entity)
         self.package_entity_db = app_package_entity_db(self.db, infra_app_packages)
         self.graph_dbs: Dict[str, GraphDB] = {}
@@ -79,15 +79,15 @@
         await self.subscribers_db.create_update_schema()
         await self.running_task_db.create_update_schema()
         await self.job_db.create_update_schema()
         await self.config_entity_db.create_update_schema()
         await self.config_validation_entity_db.create_update_schema()
         await self.configs_model_db.create_update_schema()
         await self.template_entity_db.create_update_schema()
-        await self.pending_deferred_edge_db.create_update_schema()
+        await self.deferred_outer_edge_db.create_update_schema()
         await self.package_entity_db.create_update_schema()
         for graph in cast(List[Json], self.database.graphs()):
             graph_name = GraphName(graph["name"])
 
             # snapshot graphs do not need any schema migrations,
             # we can skip them
             if str(graph_name).startswith("snapshot"):
```

### Comparing `resotocore-3.6.1/resotocore/db/deferred_edge_db.py` & `resotocore-3.6.2/resotocore/db/deferredouteredgedb.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,37 +3,58 @@
 from resotocore.db.async_arangodb import AsyncArangoDB
 from resotocore.db.entitydb import ArangoEntityDb
 from resotocore.model.graph_access import DeferredEdge
 from resotocore.ids import TaskId
 from typing import List, cast
 import logging
 
+from resotocore.model.typed_model import from_js
 from resotocore.types import Json
 from resotocore.ids import GraphName
 
 
 @define
-class PendingDeferredEdges:
+class DeferredOuterEdges:
+    id: str
+    change_id: str
     task_id: TaskId
     created_at: datetime  # update the corresponding TTL index when changing this name
     graph: GraphName
     edges: List[DeferredEdge]
 
 
 TWO_HOURS = 7200
 
 
 log = logging.getLogger(__name__)
 
 
-class PendingDeferredEdgeDb(ArangoEntityDb[TaskId, PendingDeferredEdges]):
+class DeferredOuterEdgeDb(ArangoEntityDb[str, DeferredOuterEdges]):
+    async def all_for_task(self, task_id: TaskId) -> List[DeferredOuterEdges]:
+        result = []
+        async with await self.db.aql_cursor(
+            f"FOR e IN `{self.collection_name}` FILTER e.task_id == @task_id RETURN e", bind_vars={"task_id": task_id}
+        ) as cursor:
+            async for doc in cursor:
+                edges = from_js(doc, DeferredOuterEdges)
+                result.append(edges)
+        return result
+
+    async def delete_for_task(self, task_id: TaskId) -> None:
+        async with await self.db.aql_cursor(
+            f"FOR e IN `{self.collection_name}` FILTER e.task_id == @task_id REMOVE e IN `{self.collection_name}`",
+            bind_vars={"task_id": task_id},
+        ) as cursor:
+            async for _ in cursor:
+                pass
+
     async def create_update_schema(self) -> None:
         await super().create_update_schema()
         ttl_index_name = "deferred_edges_expiration_index"
         collection = self.db.collection(self.collection_name)
         if ttl_index_name not in {idx["name"] for idx in cast(List[Json], collection.indexes())}:
             log.info(f"Add index {ttl_index_name} on {collection.name}")
             collection.add_ttl_index(["created_at"], TWO_HOURS, "deferred_edges_expiration_index")
 
 
-def pending_deferred_edge_db(db: AsyncArangoDB, collection: str) -> ArangoEntityDb[TaskId, PendingDeferredEdges]:
-    return PendingDeferredEdgeDb(db, collection, PendingDeferredEdges, lambda k: k.task_id)
+def deferred_outer_edge_db(db: AsyncArangoDB, collection: str) -> DeferredOuterEdgeDb:
+    return DeferredOuterEdgeDb(db, collection, DeferredOuterEdges, lambda k: k.id)
```

### Comparing `resotocore-3.6.1/resotocore/db/entitydb.py` & `resotocore-3.6.2/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/graphdb.py` & `resotocore-3.6.2/resotocore/db/graphdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/model.py` & `resotocore-3.6.2/resotocore/db/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/packagedb.py` & `resotocore-3.6.2/resotocore/db/packagedb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/runningtaskdb.py` & `resotocore-3.6.2/resotocore/db/runningtaskdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                 ["task_started_at"],
                 expiry_time=int(timedelta(days=60).total_seconds()),
                 in_background=True,
                 name=ttl_idx,
             )
 
     async def all_running(self) -> AsyncGenerator[RunningTaskData, None]:
-        aql = f"""FOR doc IN {self.collection_name} FILTER doc.done == false RETURN doc"""
+        aql = f"""FOR doc IN {self.collection_name} FILTER doc.done==false SORT doc.task_started_at DESC  RETURN doc"""
         async with await self.db.aql_cursor(aql) as cursor:
             async for element in cursor:
                 try:
                     yield from_js(element, RunningTaskData)
                 except JsonsError:
                     log.warning(f"Not able to parse {element} into RunningTaskData. Ignore.")
```

### Comparing `resotocore-3.6.1/resotocore/db/system_data_db.py` & `resotocore-3.6.2/resotocore/db/system_data_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/db/usagedb.py` & `resotocore-3.6.2/resotocore/db/usagedb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/error.py` & `resotocore-3.6.2/resotocore/error.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/graph_manager/graph_manager.py` & `resotocore-3.6.2/resotocore/graph_manager/graph_manager.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/infra_apps/local_runtime.py` & `resotocore-3.6.2/resotocore/infra_apps/local_runtime.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/infra_apps/manifest.py` & `resotocore-3.6.2/resotocore/infra_apps/manifest.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/infra_apps/package_manager.py` & `resotocore-3.6.2/resotocore/infra_apps/package_manager.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/infra_apps/runtime.py` & `resotocore-3.6.2/resotocore/infra_apps/runtime.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/bootstrap.js` & `resotocore-3.6.2/resotocore/jupyterlite/bootstrap.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1037.51967a2.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1037.51967a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1079.cdbaf67.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1079.cdbaf67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1084.4cd1c89.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1084.4cd1c89.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1113.23c9417.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1113.23c9417.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1125.129d070.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1125.129d070.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1163.ac28297.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1163.ac28297.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1221.c51249a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1221.c51249a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1245.be46619.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1245.be46619.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1261.199fc1d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1261.199fc1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1272.f334098.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1272.f334098.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1278.0524a4a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1278.0524a4a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt` & `resotocore-3.6.2/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1290.3981211.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1290.3981211.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1295.46e72b8.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1295.46e72b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1310.23bbe67.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1310.23bbe67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1320.21effe3.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1320.21effe3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1325.f76267c.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1325.f76267c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1408.7461890.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1408.7461890.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1440.a9e7ea1.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1440.a9e7ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1483.616d9ab.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1483.616d9ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1489.e50b6d4.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1489.e50b6d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1507.5705605.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1507.5705605.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/152.525d460.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/152.525d460.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1520.4e2eb21.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1520.4e2eb21.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1555.e188f3f.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1555.e188f3f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1559.7c89925.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1559.7c89925.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/160.5f28731.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/160.5f28731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1603.370a2a6.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1603.370a2a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1644.0e49167.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1644.0e49167.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1667.f0afb2b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1667.f0afb2b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1687.27f1ad6.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1687.27f1ad6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1725.f151c33.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1725.f151c33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1767.c8c2f26.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1767.c8c2f26.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1806.1aaf66b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1806.1aaf66b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1838.1202b16.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1838.1202b16.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1909.28a2def.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1909.28a2def.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/1989.88d258f.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/1989.88d258f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2030.1562cc6.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2030.1562cc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2047.baed97b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2047.baed97b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2099.f4b6fcd.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2099.f4b6fcd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2118.5b65f70.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2118.5b65f70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/213.5769e57.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/213.5769e57.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2161.dcb27b8.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2161.dcb27b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2169.635c88e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2169.635c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/217.90d10e2.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/217.90d10e2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2212.72be094.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2212.72be094.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2287.997c38e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2287.997c38e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt` & `resotocore-3.6.2/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2303.9ff8710.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2303.9ff8710.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2319.6b4cbb7.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2319.6b4cbb7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2329.4c5ca6d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2329.4c5ca6d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2351.fbd96d8.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2351.fbd96d8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2358.d5cf7c8.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2358.d5cf7c8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2359.6451c3e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2359.6451c3e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/237.f765e77.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/237.f765e77.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2384.71782be.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2384.71782be.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/240.cddc46b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/240.cddc46b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2431.648d237.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2431.648d237.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2546.1f48267.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2546.1f48267.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2557.75e9da2.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2557.75e9da2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/261.5f53c0e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/261.5f53c0e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2629.c0e1cd6.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2629.c0e1cd6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2788.46acc8a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2788.46acc8a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2834.942acc6.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2834.942acc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2887.47ba752.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2887.47ba752.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2956.8880209.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2956.8880209.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/2973.2a51dc4.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/2973.2a51dc4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3004.255e79c.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3004.255e79c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/302.8bcc38f.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/302.8bcc38f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3037.70ee38d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3037.70ee38d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3042.7cfad84.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3042.7cfad84.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3051.34fac68.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3051.34fac68.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3122.2289fca.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3122.2289fca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3151.10ef4de.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3151.10ef4de.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/316.c850a76.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/316.c850a76.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3196.4e35a17.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3196.4e35a17.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3265.a80440a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3265.a80440a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3277.9c04e75.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3277.9c04e75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/330.126fa98.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/330.126fa98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3392.29fe6b9.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3392.29fe6b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3413.480a49d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3413.480a49d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3444.47d5ea1.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3444.47d5ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3469.7d14d0b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3469.7d14d0b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3546.fee1bd7.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3546.fee1bd7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/362.6716970.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/362.6716970.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3708.410d087.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3708.410d087.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3850.903abc2.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3850.903abc2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt` & `resotocore-3.6.2/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3880.bd39dce.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3880.bd39dce.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3970.236586f.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3970.236586f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3976.58893b9.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3976.58893b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt` & `resotocore-3.6.2/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/3979.385527e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/3979.385527e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/400.d72234b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/400.d72234b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4018.1a35967.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4018.1a35967.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/406.9b7af92.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/406.9b7af92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4117.a8107fd.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4117.a8107fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4182.e2430f9.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4182.e2430f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4191.02bbea8.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4191.02bbea8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4197.53ab10b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4197.53ab10b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4206.a5f8bb0.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4206.a5f8bb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4207.0d0580b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4207.0d0580b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4262.bb73457.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4262.bb73457.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4298.5ee510c.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4298.5ee510c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/44.0cfa785.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/44.0cfa785.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt` & `resotocore-3.6.2/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4410.e4a25d3.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4410.e4a25d3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4466.64d23d1.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4466.64d23d1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/451.d9683ad.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/451.d9683ad.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4535.34b060a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4535.34b060a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4565.43bdb91.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4565.43bdb91.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4569.f374f9d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4569.f374f9d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4615.eb5d40a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4615.eb5d40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4658.090d4a9.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4658.090d4a9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4690.3dd4096.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4690.3dd4096.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4715.e7690b9.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4715.e7690b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4749.46ebbb2.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4749.46ebbb2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4750.56c06ab.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4750.56c06ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4856.2d7415f.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4856.2d7415f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4875.375150e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4875.375150e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/489.b981dea.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/489.b981dea.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/490.c2624d4.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/490.c2624d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4905.667bf33.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4905.667bf33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4931.430433b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4931.430433b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/4942.b96c164.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/4942.b96c164.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5016.dd2fe83.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5016.dd2fe83.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5072.733a1b5.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5072.733a1b5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/509.6448878.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/509.6448878.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5096.8ed0d8e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5096.8ed0d8e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5126.eecad7a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5126.eecad7a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5129.1ba4763.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5129.1ba4763.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5153.763d8fa.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5153.763d8fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5155.06b4ea9.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5155.06b4ea9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5193.e9f6866.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5193.e9f6866.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5213.3e1a360.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5213.3e1a360.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5227.8c8acd8.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5227.8c8acd8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5238.1751cc3.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5238.1751cc3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/528.2262cb0.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/528.2262cb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5292.79d4aba.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5292.79d4aba.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5437.31236f7.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5437.31236f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5489.848a8cf.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5489.848a8cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5508.317fca3.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5508.317fca3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/554.ac98303.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/554.ac98303.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/555.2cd31dd.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/555.2cd31dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5573.ebcdb93.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5573.ebcdb93.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5666.c5e5324.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5666.c5e5324.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5710.70d0b1d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5710.70d0b1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5747.94ad626.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5747.94ad626.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/582.21b8e7d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/582.21b8e7d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5823.5045bdb.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5823.5045bdb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5851.30b7b2a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5851.30b7b2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5878.32d92fa.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5878.32d92fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5880.68f975b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5880.68f975b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5955.88508f7.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5955.88508f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/5971.88c5642.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/5971.88c5642.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6080.aa0ff24.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6080.aa0ff24.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/61.2808a0d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/61.2808a0d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6136.b8ba2b2.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6136.b8ba2b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6141.9831d58.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6141.9831d58.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6475.6037fbb.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6475.6037fbb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6493.d796aa5.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6493.d796aa5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6556.b3d9293.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6556.b3d9293.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6571.2c8884e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6571.2c8884e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6576.3ea568e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6576.3ea568e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6591.94ed352.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6591.94ed352.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6612.1632879.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6612.1632879.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6623.ae3b3cc.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6623.ae3b3cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6664.2160109.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6664.2160109.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6747.47be7f5.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6747.47be7f5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6748.be68f5f.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6748.be68f5f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6870.7940288.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6870.7940288.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6879.c8367a5.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6879.c8367a5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6898.9bbc12a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6898.9bbc12a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6952.f68b818.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6952.f68b818.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6985.321ad92.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6985.321ad92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6993.32cf9a6.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6993.32cf9a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/6997.b06fe71.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/6997.b06fe71.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7041.d4f561e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7041.d4f561e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7058.805c88e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7058.805c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7174.6c45206.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7174.6c45206.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7334.8859b1b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7334.8859b1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7359.6ee65ec.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7359.6ee65ec.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7364.195178b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7364.195178b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7380.58a4413.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7380.58a4413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7427.f9c2017.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7427.f9c2017.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7463.18fd278.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7463.18fd278.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7509.1e0189e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7509.1e0189e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7526.1a303e5.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7526.1a303e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7537.1323a15.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7537.1323a15.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7692.33d5169.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7692.33d5169.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7746.5908d29.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7746.5908d29.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7808.1d582a2.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7808.1d582a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/783.c156751.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/783.c156751.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7858.2386e4d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7858.2386e4d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/7941.01ea680.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/7941.01ea680.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8005.c5ad7b2.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8005.c5ad7b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8028.39e2fa1.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8028.39e2fa1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8061.cc62561.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8061.cc62561.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8101.cf46d02.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8101.cf46d02.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/812.9b0e86e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/812.9b0e86e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/816.c8050f2.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/816.c8050f2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8165.b2c3285.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8165.b2c3285.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8232.a578bf9.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8232.a578bf9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/824.8678196.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/824.8678196.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8270.89fe7e1.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8270.89fe7e1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/833.9cc6653.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/833.9cc6653.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8370.8f855e5.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8370.8f855e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8373.96b0b3a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8373.96b0b3a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8389.ffe031f.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8389.ffe031f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8412.1528057.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8412.1528057.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8427.4923f43.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8427.4923f43.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8542.027afdc.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8542.027afdc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8594.0112f03.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8594.0112f03.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8656.d5b8e92.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8656.d5b8e92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8685.d78bdab.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8685.d78bdab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8698.9817d75.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8698.9817d75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8732.9320f73.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8732.9320f73.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8785.cf4fe95.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8785.cf4fe95.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8828.77c71d0.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8828.77c71d0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8883.80c7b63.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8883.80c7b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8976.3816942.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8976.3816942.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/8990.2a453cf.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/8990.2a453cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9035.1e45c1b.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9035.1e45c1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9053.45b77fc.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9053.45b77fc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9077.fefb6ca.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9077.fefb6ca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9128.b8fa6f0.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9128.b8fa6f0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9156.0cefbd3.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9156.0cefbd3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9170.0023587.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9170.0023587.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9196.315f9f9.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9196.315f9f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9198.9971d70.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9198.9971d70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/920.d15c177.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/920.d15c177.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9253.0b31caa.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9253.0b31caa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9266.bacd0dd.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9266.bacd0dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9307.c3a00ed.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9307.c3a00ed.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9321.869e413.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9321.869e413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9344.ba0abcf.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9344.ba0abcf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9382.9014799.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9382.9014799.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9440.1b10b8f.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9440.1b10b8f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9464.79e6ac5.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9464.79e6ac5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9502.9a24831.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9502.9a24831.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9507.1e6cc5d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9507.1e6cc5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9602.62bf0f1.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9602.62bf0f1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9621.e2e8b5d.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9621.e2e8b5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9622.ccab065.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9622.ccab065.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9626.a178bd0.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9626.a178bd0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9647.ed91993.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9647.ed91993.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9657.bc5c60e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9657.bc5c60e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/97.ad126b0.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/97.ad126b0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9712.796a0a1.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9712.796a0a1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9737.7dc8f98.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9737.7dc8f98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9777.0b8a504.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9777.0b8a504.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9793.6d63a85.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9793.6d63a85.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9806.652c162.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9806.652c162.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9865.2e3db6f.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9865.2e3db6f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/989.bcca86a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/989.bcca86a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9943.f3f35c7.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9943.f3f35c7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9958.25c8c06.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9958.25c8c06.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/9960.64cd61e.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/9960.64cd61e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/add-above.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/add-above.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/add-below.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/add-below.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/bug-dot.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/bug-dot.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/bug.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/bug.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/build.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/build.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/case-sensitive.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/case-sensitive.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/close.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/close.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/copyright.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/copyright.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/cut.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/cut.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/duplicate.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/duplicate.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.woff2` & `resotocore-3.6.2/resotocore/jupyterlite/build/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.woff2` & `resotocore-3.6.2/resotocore/jupyterlite/build/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.woff2` & `resotocore-3.6.2/resotocore/jupyterlite/build/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/html5.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/html5.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/json.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/json.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/julia.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/julia.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/jupyter-favicon.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/jupyter-favicon.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/jupyter.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/jupyter.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/jupyterlab-wordmark.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/jupyterlab-wordmark.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/lab/bundle.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/lab/bundle.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/listings-info.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/listings-info.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/move-down.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/move-down.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/move-up.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/move-up.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/not-trusted.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/not-trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/palette.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/palette.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/pdf.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/pdf.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/python.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/python.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/react.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/react.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/regex.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/regex.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/all.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/schemas/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/service-worker-b2fb40a.js` & `resotocore-3.6.2/resotocore/jupyterlite/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/settings.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/settings.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/tag.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/tag.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/terminal.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/terminal.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css` & `resotocore-3.6.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css` & `resotocore-3.6.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/third-party-licenses.json` & `resotocore-3.6.2/resotocore/jupyterlite/build/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/toc.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/toc.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/build/trusted.svg` & `resotocore-3.6.2/resotocore/jupyterlite/build/trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/config-utils.js` & `resotocore-3.6.2/resotocore/jupyterlite/config-utils.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json` & `resotocore-3.6.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/files/example.ipynb` & `resotocore-3.6.2/resotocore/jupyterlite/files/example.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/icon-120x120.png` & `resotocore-3.6.2/resotocore/jupyterlite/icon-120x120.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/icon-512x512.png` & `resotocore-3.6.2/resotocore/jupyterlite/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/index.html` & `resotocore-3.6.2/resotocore/jupyterlite/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/jupyter-lite.ipynb` & `resotocore-3.6.2/resotocore/jupyterlite/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/jupyter-lite.json` & `resotocore-3.6.2/resotocore/jupyterlite/jupyter-lite.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/jupyterlite.schema.v0.json` & `resotocore-3.6.2/resotocore/jupyterlite/jupyterlite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/kernelspecs/javascript.svg` & `resotocore-3.6.2/resotocore/jupyterlite/kernelspecs/javascript.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/lab/favicon.ico` & `resotocore-3.6.2/resotocore/jupyterlite/lab/favicon.ico`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/lab/index.html` & `resotocore-3.6.2/resotocore/jupyterlite/lab/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/lab/jupyter-lite.ipynb` & `resotocore-3.6.2/resotocore/jupyterlite/lab/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/lab/package.json` & `resotocore-3.6.2/resotocore/jupyterlite/lab/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/manifest.webmanifest` & `resotocore-3.6.2/resotocore/jupyterlite/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/package.json` & `resotocore-3.6.2/resotocore/jupyterlite/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/jupyterlite/service-worker-b2fb40a.js` & `resotocore-3.6.2/resotocore/jupyterlite/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/message_bus.py` & `resotocore-3.6.2/resotocore/message_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,17 @@
         data: Json = json.get("data", {})
         if kind == "event":
             res_data = pop_keys(data, ["subscriber_id"])
             return Event(message_type, res_data)
         elif kind == "action":
             res_data = pop_keys(data, ["task", "step", "subscriber_id"])
             return Action(message_type, data["task"], data["step"], res_data)
+        elif kind == "action_abort":
+            res_data = pop_keys(data, ["task", "step", "subscriber_id"])
+            return ActionAbort(message_type, data["task"], data["step"], res_data)
         elif kind == "action_done":
             res_data = pop_keys(data, ["task", "step", "subscriber_id"])
             return ActionDone(message_type, data["task"], data["step"], data["subscriber_id"], res_data)
         elif kind == "action_info":
             return ActionInfo(
                 message_type, data["task"], data["step"], data["subscriber_id"], data["level"], data["message"]
             )
@@ -106,14 +109,21 @@
         elif isinstance(o, Action):
             extra_data = {"task": o.task_id, "step": o.step_name}
             return {
                 "kind": "action",
                 "message_type": o.message_type,
                 "data": {**o.data, **extra_data},
             }
+        elif isinstance(o, ActionAbort):
+            extra_data = {"task": o.task_id, "step": o.step_name}
+            return {
+                "kind": "action_abort",
+                "message_type": o.message_type,
+                "data": {**o.data, **extra_data},
+            }
         elif isinstance(o, ActionDone):
             extra_data = {"task": o.task_id, "step": o.step_name, "subscriber_id": o.subscriber_id}
             return {"kind": "action_done", "message_type": o.message_type, "data": {**o.data, **extra_data}}
         elif isinstance(o, ActionProgress):
             extra_data = {"task": o.task_id, "step": o.step_name, "subscriber_id": o.subscriber_id}
             return {
                 "kind": "action_progress",
@@ -156,14 +166,18 @@
 
 
 class Action(ActionMessage):
     def done(self, subscriber_id: SubscriberId) -> ActionDone:
         return ActionDone(self.message_type, self.task_id, self.step_name, subscriber_id, dict(self.data))
 
 
+class ActionAbort(ActionMessage):
+    pass
+
+
 class ActionDone(ActionMessage):
     def __init__(
         self,
         message_type: str,
         task_id: TaskId,
         step_name: str,
         subscriber_id: SubscriberId,
```

### Comparing `resotocore-3.6.1/resotocore/metrics.py` & `resotocore-3.6.2/resotocore/metrics.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/model/adjust_node.py` & `resotocore-3.6.2/resotocore/model/adjust_node.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/model/db_updater.py` & `resotocore-3.6.2/resotocore/model/db_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aiostream.core import Stream
 from attrs import define
 
 from resotocore.analytics import AnalyticsEventSender, InMemoryEventSender, AnalyticsEvent
 from resotocore.async_extensions import run_async
 from resotocore.core_config import CoreConfig
 from resotocore.db.db_access import DbAccess
-from resotocore.db.deferred_edge_db import PendingDeferredEdges
+from resotocore.db.deferredouteredgedb import DeferredOuterEdges
 from resotocore.db.graphdb import GraphDB
 from resotocore.db.model import GraphUpdate
 from resotocore.error import ImportAborted
 from resotocore.ids import TaskId, GraphName
 from resotocore.message_bus import MessageBus, CoreMessage
 from resotocore.model.graph_access import GraphBuilder
 from resotocore.model.model_handler import ModelHandlerDB, ModelHandler
@@ -180,21 +180,23 @@
         if isinstance(nxt, PoisonPill):
             log.debug("Got poison pill - going to die.")
             shutdown_process(0)
         elif isinstance(nxt, MergeGraph):
             log.debug("Graph read into memory")
             builder.check_complete()
             graphdb = db.get_graph_db(nxt.graph)
-            outer_edge_db = db.pending_deferred_edge_db
+            outer_edge_db = db.deferred_outer_edge_db
             await graphdb.insert_usage_data(builder.usage)
             _, result = await graphdb.merge_graph(builder.graph, model, nxt.change_id, nxt.is_batch)
             # sizes of model entries have been adjusted during the merge. Update the model in the db.
             await model_handler.update_model(graphdb.name, list(model.kinds.values()))
             if nxt.task_id and builder.deferred_edges:
-                await outer_edge_db.update(PendingDeferredEdges(nxt.task_id, utc(), nxt.graph, builder.deferred_edges))
+                await outer_edge_db.update(
+                    DeferredOuterEdges(uuid_str(), nxt.change_id, nxt.task_id, utc(), nxt.graph, builder.deferred_edges)
+                )
                 log.debug(f"Updated {len(builder.deferred_edges)} pending outer edges for collect task {nxt.task_id}")
             return result
 
     async def setup_and_merge(self) -> GraphUpdate:
         sender = InMemoryEventSender()
         _, _, sdb = DbAccess.connect(self.config.args, timedelta(seconds=3), verify=self.config.run.verify)
         db = db_access(self.config, sdb, sender)
```

### Comparing `resotocore-3.6.1/resotocore/model/graph_access.py` & `resotocore-3.6.2/resotocore/model/graph_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     DictionaryKind,
     StringKind,
     Property,
     SimpleKind,
     DateKind,
     DurationKind,
     UsageDatapoint,
-    UsageMetricValues,
 )
 from resotocore.model.resolve_in_graph import GraphResolver, NodePath, ResolveProp
 from resotocore.model.typed_model import from_js
 from resotocore.types import Json, EdgeType, JsonElement
 from resotocore.util import utc, utc_str, value_in_path, set_value_in_path, value_in_path_get
 
 log = logging.getLogger(__name__)
@@ -162,27 +161,19 @@
                 reported=js[Section.reported],
                 desired=js.get(Section.desired, None),
                 metadata=js.get(Section.metadata, None),
                 search=js.get("search", None),
                 replace=js.get("replace", False) is True,
             )
             if usage_json:
-                values = {
-                    k: UsageMetricValues(
-                        min=v.get("min", v["avg"]),
-                        avg=v["avg"],
-                        max=v.get("max", v["avg"]),
-                    )
-                    for k, v in usage_json.items()
-                }
                 usage = UsageDatapoint(
                     id=js["id"],
                     change_id=self.change_id,
                     at=self.at,
-                    v=values,
+                    v=usage_json,
                 )
                 self.usage.append(usage)
         elif "from" in js and "to" in js:
             self.add_edge(js["from"], js["to"], js.get("edge_type", EdgeTypes.default))
         elif "from_selector" in js and "to_selector" in js:
 
             def parse_selector(js: Json) -> NodeSelector:
```

### Comparing `resotocore-3.6.1/resotocore/model/json_schema.py` & `resotocore-3.6.2/resotocore/model/json_schema.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/model/model.py` & `resotocore-3.6.2/resotocore/model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     Dict,
     List,
     Set,
     cast,
     Tuple,
     Iterable,
     TypeVar,
-    NamedTuple,
 )
 
 import yaml
 from attrs import define, frozen
 from dateutil.parser import parse
 from jsons import set_deserializer, set_serializer
 from networkx import MultiDiGraph
@@ -1456,20 +1455,14 @@
                     )
                 )
             else:
                 result.append(kind)
         return result
 
 
-class UsageMetricValues(NamedTuple):
-    min: float
-    avg: float
-    max: float
-
-
 @frozen
 class UsageDatapoint:
     """
     A single datapoint of resource usage.
 
     id: `str`
         Identifier of the resource as named by the cloud.
@@ -1482,13 +1475,13 @@
         Dictionary of metric names to lists of values. The values are `min`, `avg` and `max`.
 
     """
 
     id: str
     at: int
     change_id: str
-    v: Dict[str, UsageMetricValues]
+    v: Dict[str, Dict[str, float]]
 
 
 # register serializer for this class
 set_deserializer(Kind.from_json, Kind)
 set_serializer(SimpleKind.to_json, SimpleKind)
```

### Comparing `resotocore-3.6.1/resotocore/model/model_handler.py` & `resotocore-3.6.2/resotocore/model/model_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/model/resolve_in_graph.py` & `resotocore-3.6.2/resotocore/model/resolve_in_graph.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/model/transform_kind_convert.py` & `resotocore-3.6.2/resotocore/model/transform_kind_convert.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/model/typed_model.py` & `resotocore-3.6.2/resotocore/model/typed_model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/query/__init__.py` & `resotocore-3.6.2/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/query/model.py` & `resotocore-3.6.2/resotocore/query/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/query/query_parser.py` & `resotocore-3.6.2/resotocore/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/query/template_expander.py` & `resotocore-3.6.2/resotocore/query/template_expander.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/query/template_expander_service.py` & `resotocore-3.6.2/resotocore/query/template_expander_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/report/__init__.py` & `resotocore-3.6.2/resotocore/report/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/report/benchmark_renderer.py` & `resotocore-3.6.2/resotocore/report/benchmark_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/report/inspector_service.py` & `resotocore-3.6.2/resotocore/report/inspector_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/report/report_config.py` & `resotocore-3.6.2/resotocore/report/report_config.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/api-doc.yaml` & `resotocore-3.6.2/resotocore/static/api-doc.yaml`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/ck-unicode-truecolor.ans` & `resotocore-3.6.2/resotocore/static/ck-unicode-truecolor.ans`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/benchmark/aws/aws_cis_1_5.json` & `resotocore-3.6.2/resotocore/static/report/benchmark/aws/aws_cis_1_5.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/check_template.json` & `resotocore-3.6.2/resotocore/static/report/check_template.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_apigateway.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_apigateway.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_cloudtrail.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_cloudtrail.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_config.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_config.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_ec2.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_ec2.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_efs.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_efs.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_iam.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_iam.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_kms.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_kms.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_lambda.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_lambda.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_rds.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_rds.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_s3.json` & `resotocore-3.6.2/resotocore/static/report/checks/aws/aws_s3.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/static/resoto_logo_and_text.svg` & `resotocore-3.6.2/resotocore/static/resoto_logo_and_text.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/system_start.py` & `resotocore-3.6.2/resotocore/system_start.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,23 @@
         "--verbose", "-v", dest="verbose", default=False, action="store_true", help="Enable verbose logging."
     )
     parser.add_argument(  # No default here on purpose: it can be reconfigured!
         "--debug", default=None, action="store_true", help="Enable debug mode. If not defined use configuration."
     )
     parser.add_argument("--ui-path", help=argparse.SUPPRESS)  # no effect any longer, only here to not break anything
     parser.add_argument("--analytics-opt-out", default=None, action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument(
+        "--no-scheduling", default=False, action="store_true", help="Disable scheduling of jobs and workflows."
+    )
+    parser.add_argument(
+        "--ignore-interrupted-tasks",
+        default=False,
+        action="store_true",
+        help="Do not load and continue interrupted tasks.",
+    )
 
     parsed: Namespace = parser.parse_args(args if args else [])
 
     if parsed.version:
         # print here on purpose, since logging is not set up yet.
         print(f"resotocore {version()}")
         sys.exit(0)
```

### Comparing `resotocore-3.6.1/resotocore/task/__init__.py` & `resotocore-3.6.2/resotocore/task/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Optional, List
 
 from attr import define
 
 from resotocore.task.task_description import Job, RunningTask, Workflow
-from resotocore.ids import TaskDescriptorId
+from resotocore.ids import TaskDescriptorId, TaskId
 
 
 @define(frozen=True)
 class RunningTaskInfo:
     running_task: RunningTask
     scheduled_next: bool = False
 
@@ -44,7 +44,11 @@
     @abstractmethod
     async def start_task_by_descriptor_id(self, uid: TaskDescriptorId) -> Optional[RunningTaskInfo]:
         pass
 
     @abstractmethod
     async def running_tasks(self) -> List[RunningTask]:
         pass
+
+    @abstractmethod
+    async def stop_task(self, uid: TaskId) -> Optional[RunningTask]:
+        pass
```

### Comparing `resotocore-3.6.1/resotocore/task/model.py` & `resotocore-3.6.2/resotocore/task/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/task/scheduler.py` & `resotocore-3.6.2/resotocore/task/scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,44 @@
+import logging
 import warnings
+from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import Callable, Any, List
 
 from apscheduler.executors.asyncio import AsyncIOExecutor
 from apscheduler.job import Job
 from apscheduler.jobstores.memory import MemoryJobStore
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 from apscheduler.triggers.cron import CronTrigger
 
 from resotocore.service import Service
 from resotolib.utils import get_local_tzinfo
 
+log = logging.getLogger("resotocore")
+
 
 warnings.filterwarnings(
     "ignore",
     message="The localize method is no longer necessary, as this time zone supports the fold attribute",
 )
 
 
-class Scheduler(Service):
+class Scheduler(Service, ABC):
+    @abstractmethod
+    def cron(
+        self, job_id: str, name: str, cron_string: str, func: Callable[..., Any], *args: Any, **kwargs: Any
+    ) -> None:
+        pass
+
+    @abstractmethod
+    def list_jobs(self) -> List[Job]:
+        pass
+
+
+class APScheduler(Scheduler):
     def __init__(self) -> None:
         self.scheduler = AsyncIOScheduler(
             jobstores={"default": MemoryJobStore()},
             executors={"default": AsyncIOExecutor()},
             # coalesce: run once instead of many times if the job should be run more than once in succession
             # max_instances: allowed parallel instances for one job
             # misfire_grace_time: seconds after the designated runtime that the job is still allowed to be run
@@ -48,7 +64,24 @@
     def interval(
         self, job_id: str, name: str, every_second: int, func: Callable[..., Any], *args: Any, **kwargs: Any
     ) -> Job:
         return self.scheduler.add_job(func, "interval", args, kwargs, job_id, name, seconds=every_second)
 
     def list_jobs(self) -> List[Job]:
         return self.scheduler.get_jobs(jobstore="default")  # type: ignore
+
+
+class NoScheduler(Scheduler):
+    """
+    A scheduler that does not schedule anything.
+    """
+
+    def __init__(self) -> None:
+        log.info("Scheduling disabled")
+
+    def cron(
+        self, job_id: str, name: str, cron_string: str, func: Callable[..., Any], *args: Any, **kwargs: Any
+    ) -> None:
+        pass
+
+    def list_jobs(self) -> List[Job]:
+        return []
```

### Comparing `resotocore-3.6.1/resotocore/task/start_workflow_on_first_subscriber.py` & `resotocore-3.6.2/resotocore/task/start_workflow_on_first_subscriber.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/task/subscribers.py` & `resotocore-3.6.2/resotocore/task/subscribers.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/task/task_description.py` & `resotocore-3.6.2/resotocore/task/task_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     Action,
     ActionDone,
     Message,
     ActionError,
     ActionInfo,
     ActionProgress,
     CoreMessage,
+    ActionAbort,
 )
 from resotocore.model.typed_model import to_json, from_js, to_js
 from resotocore.task.model import Subscriber
 from resotocore.types import Json
 from resotocore.util import first, interleave, empty, exist, identity, utc, utc_str
 from resotolib.core.progress import ProgressTree, Progress, ProgressDone
 from resotolib.utils import freeze
@@ -406,14 +407,20 @@
 
     def initial_progress(self, progress: ProgressTree) -> None:
         """
         Override this method in deriving classes to define initial progress.
         :param progress: the progress tree to update.
         """
 
+    def abort(self) -> Sequence[TaskCommand]:
+        """
+        Override this method in deriving classes to define behaviour when the task is aborted.
+        """
+        return []
+
     @staticmethod
     def from_step(step: Step, instance: RunningTask) -> StepState:
         """
         Create the related state based on the given step and task description.
         """
         if isinstance(step.action, PerformAction):
             return PerformActionState(step.action, step, instance)
@@ -529,14 +536,19 @@
         self._wait_for = list(filter(identity, (existing.get(sid) for sid in wait_for)))  # type: ignore
 
     def initial_progress(self, progress: ProgressTree) -> None:
         super().initial_progress(progress)
         if self.wait_for():
             progress.add_progress(ProgressDone(self.step.name, 0, 1))
 
+    def abort(self) -> Sequence[TaskCommand]:
+        result = list(super().abort())
+        result.append(SendMessage(ActionAbort(self.perform.message_type, self.instance.id, self.step.name)))
+        return result
+
 
 class WaitForEventState(StepState):
     def __init__(self, perform: WaitForEvent, step: Step, instance: RunningTask):
         super().__init__(step, instance)
         self.perform = perform
 
     def current_step_done(self) -> bool:
@@ -624,28 +636,28 @@
 
     def commands_to_execute(self) -> Sequence[TaskCommand]:
         return [SendMessage(self.emit.event)]
 
 
 class StartState(StepState):
     def __init__(self, instance: RunningTask):
-        self.event = Event("task_start")
+        self.event = Event("task_start", {"task_id": instance.id, "descriptor_id": instance.descriptor.id})
         super().__init__(Step("task_start", EmitEvent(self.event)), instance)
 
     def commands_to_execute(self) -> Sequence[TaskCommand]:
         return [SendMessage(self.event)]
 
 
 class EndState(StepState):
     """
     This state marks the end of the task.
     """
 
     def __init__(self, instance: RunningTask):
-        self.event = Event("task_end")
+        self.event = Event("task_end", {"task_id": instance.id, "descriptor_id": instance.descriptor.id})
         super().__init__(Step("task_end", EmitEvent(self.event)), instance)
 
     def is_error(self) -> bool:
         return self.instance.is_error
 
     def current_step_done(self) -> bool:
         return False
```

### Comparing `resotocore-3.6.1/resotocore/task/task_handler.py` & `resotocore-3.6.2/resotocore/task/task_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from attrs import evolve
 
 from resotocore.analytics import AnalyticsEventSender, CoreEvent
 from resotocore.cli.model import CLIContext, CLI
 from resotocore.core_config import CoreConfig
 from resotocore.db.jobdb import JobDb
 from resotocore.db.runningtaskdb import RunningTaskData, RunningTaskDb
-from resotocore.ids import SubscriberId, TaskDescriptorId
+from resotocore.ids import SubscriberId, TaskDescriptorId, TaskId
 from resotocore.message_bus import (
     MessageBus,
     Event,
     Action,
     ActionDone,
     Message,
     ActionError,
@@ -86,15 +86,15 @@
         self.cli_context = CLIContext(source="task_handler")
         self.config = config
         # note: the waiting queue is kept in memory and lost when the service is restarted.
         self.start_when_done: Dict[str, TaskDescription] = {}
 
         # Step1: define all workflows and jobs in code: later it will be persisted and read from database
         self.task_descriptions: Sequence[TaskDescription] = [*self.known_workflows(config), *self.known_jobs()]
-        self.tasks: Dict[str, RunningTask] = {}
+        self.tasks: Dict[TaskId, RunningTask] = {}
         self.message_bus_watcher: Optional[Task[None]] = None
         self.initial_start_workflow_task: Optional[Task[None]] = None
         self.timeout_watcher = Periodic("task_watcher", self.check_running_tasks, timedelta(seconds=10))
         self.registered_event_trigger: List[Tuple[EventTrigger, TaskDescription]] = []
         self.registered_event_trigger_by_message_type: Dict[str, List[Tuple[EventTrigger, TaskDescription]]] = {}
         self.task_dependencies = TaskDependencies(graph_merger, subscription_handler.subscribers_by_event)
 
@@ -221,31 +221,36 @@
                     step_state.timed_out = si.timed_out
             # reset times
             wi.task_started_at = task_data.task_started_at
             # ignore all messages that would be emitted
             wi.move_to_next_state()
             return wi
 
-        instances: List[RunningTask] = []
+        started_instances: Dict[TaskDescriptorId, RunningTask] = {}
         async for data in self.running_task_db.all_running():
             descriptor = descriptions.get(data.task_descriptor_id)
-            if descriptor:
-                # we have captured the timestamp when the task has been started
-                updated = self.evaluate_task_definition(descriptor, now=utc_str(data.task_started_at))
-                rt = RunningTask(data.id, updated, self.task_dependencies)
-                instance = reset_state(rt, data)
-                if isinstance(instance.current_step.action, RestartAgainStepAction):
-                    log.info(f"Restart interrupted action: {instance.current_step.action}")
-                    await self.execute_task_commands(instance, instance.current_state.commands_to_execute())
-                instances.append(instance)
-
-            else:
+            if descriptor is None:
                 log.warning(f"No task description with this id found: {data.task_descriptor_id}. Remove instance data.")
                 await self.running_task_db.delete(data.id)
-        return instances
+                continue
+
+            if descriptor.id in started_instances and descriptor.on_surpass != TaskSurpassBehaviour.Parallel:
+                log.warning(f"Already started task for: {data.task_descriptor_id}: {data.id}. Remove instance data.")
+                await self.running_task_db.delete(data.id)
+                continue
+
+            # we have captured the timestamp when the task has been started
+            updated = self.evaluate_task_definition(descriptor, now=utc_str(data.task_started_at))
+            rt = RunningTask(data.id, updated, self.task_dependencies)
+            instance = reset_state(rt, data)
+            if isinstance(instance.current_step.action, RestartAgainStepAction):
+                log.info(f"Restart interrupted action: {instance.current_step.action}")
+                await self.execute_task_commands(instance, instance.current_state.commands_to_execute())
+            started_instances[descriptor.id] = instance
+        return list(started_instances.values())
 
     async def __aenter__(self) -> TaskHandlerService:
         return await self.start()
 
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         return await self.stop()
 
@@ -253,15 +258,16 @@
         log.debug("TaskHandlerService is starting up!")
 
         # load job descriptions from database
         db_jobs = [job async for job in self.job_db.all()]
         self.task_descriptions = [*self.task_descriptions, *db_jobs]
 
         # load and restore all tasks
-        self.tasks = {wi.id: wi for wi in await self.start_interrupted_tasks()}
+        if not self.config.args.ignore_interrupted_tasks:
+            self.tasks = {wi.id: wi for wi in await self.start_interrupted_tasks()}
 
         await self.timeout_watcher.start()
 
         for descriptor in self.task_descriptions:
             await self.update_trigger(descriptor)
 
         if self.config.runtime.start_collect_on_subscriber_connect:
@@ -354,14 +360,22 @@
             descriptions.remove(existing)
         # store in database
         await self.job_db.update(job)
         descriptions.append(job)
         self.task_descriptions = descriptions
         await self.update_trigger(job)
 
+    async def stop_task(self, uid: TaskId) -> Optional[RunningTask]:
+        if task := self.tasks.get(uid):
+            commands = task.current_state.abort()  # abort current step
+            task.end()  # mark task as done
+            await self.execute_task_commands(task, commands)
+            return task
+        return None
+
     async def delete_running_task(self, task: RunningTask) -> None:
         # send analytics event
         await self.event_sender.core_event(
             CoreEvent.TaskCompleted,
             {
                 "task_descriptor_id": task.descriptor.id,
                 "task_descriptor_name": task.descriptor.name,
```

### Comparing `resotocore-3.6.1/resotocore/templates/base.html` & `resotocore-3.6.2/resotocore/templates/base.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/templates/create_first_user.html` & `resotocore-3.6.2/resotocore/templates/create_first_user.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/templates/login.html` & `resotocore-3.6.2/resotocore/templates/login.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/types.py` & `resotocore-3.6.2/resotocore/types.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/user/__init__.py` & `resotocore-3.6.2/resotocore/user/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/user/user_management.py` & `resotocore-3.6.2/resotocore/user/user_management.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/util.py` & `resotocore-3.6.2/resotocore/util.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/validator.py` & `resotocore-3.6.2/resotocore/validator.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/web/api.py` & `resotocore-3.6.2/resotocore/web/api.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/web/auth.py` & `resotocore-3.6.2/resotocore/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/web/certificate_handler.py` & `resotocore-3.6.2/resotocore/web/certificate_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/web/content_renderer.py` & `resotocore-3.6.2/resotocore/web/content_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/web/directives.py` & `resotocore-3.6.2/resotocore/web/directives.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/web/tsdb.py` & `resotocore-3.6.2/resotocore/web/tsdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore/worker_task_queue.py` & `resotocore-3.6.2/resotocore/worker_task_queue.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/resotocore.egg-info/PKG-INFO` & `resotocore-3.6.2/resotocore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.6.1
+Version: 3.6.2
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotocore-3.6.1/resotocore.egg-info/SOURCES.txt` & `resotocore-3.6.2/resotocore.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 resotocore/db/__init__.py
 resotocore/db/arango_query.py
 resotocore/db/arangodb_extensions.py
 resotocore/db/arangodb_functions.py
 resotocore/db/async_arangodb.py
 resotocore/db/configdb.py
 resotocore/db/db_access.py
-resotocore/db/deferred_edge_db.py
+resotocore/db/deferredouteredgedb.py
 resotocore/db/entitydb.py
 resotocore/db/graphdb.py
 resotocore/db/jobdb.py
 resotocore/db/model.py
 resotocore/db/modeldb.py
 resotocore/db/packagedb.py
 resotocore/db/runningtaskdb.py
@@ -640,14 +640,15 @@
 tests/resotocore/conftest.py
 tests/resotocore/console_renderer_test.py
 tests/resotocore/core_config_test.py
 tests/resotocore/dependencies_test.py
 tests/resotocore/hypothesis_extension.py
 tests/resotocore/message_bus_test.py
 tests/resotocore/util_test.py
+tests/resotocore/utils.py
 tests/resotocore/validator_test.py
 tests/resotocore/worker_task_queue_test.py
 tests/resotocore/analytics/__init__.py
 tests/resotocore/analytics/posthog_test.py
 tests/resotocore/analytics/recurrent_events_test.py
 tests/resotocore/cli/__init__.py
 tests/resotocore/cli/cli_test.py
@@ -659,14 +660,15 @@
 tests/resotocore/config/core_config_handler_test.py
 tests/resotocore/db/__init__.py
 tests/resotocore/db/arango_query_test.py
 tests/resotocore/db/arangodb_functions_test.py
 tests/resotocore/db/async_arangodb_test.py
 tests/resotocore/db/configdb_test.py
 tests/resotocore/db/db_access_test.py
+tests/resotocore/db/deferredouteredgedb_test.py
 tests/resotocore/db/entitydb.py
 tests/resotocore/db/graphdb_test.py
 tests/resotocore/db/jobdb_test.py
 tests/resotocore/db/modeldb_test.py
 tests/resotocore/db/runningtaskdb_test.py
 tests/resotocore/db/subscriberdb_test.py
 tests/resotocore/db/system_data_db_test.py
```

### Comparing `resotocore-3.6.1/tests/resotocore/__init__.py` & `resotocore-3.6.2/tests/resotocore/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/analytics/posthog_test.py` & `resotocore-3.6.2/tests/resotocore/analytics/posthog_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/analytics/recurrent_events_test.py` & `resotocore-3.6.2/tests/resotocore/analytics/recurrent_events_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/cli/cli_test.py` & `resotocore-3.6.2/tests/resotocore/cli/cli_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/cli/command_test.py` & `resotocore-3.6.2/tests/resotocore/cli/command_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,21 +314,27 @@
         ctx = CLIContext(cli.cli_env)
         return (await cli.execute_cli_command(cmd, stream.list, ctx))[0]  # type: ignore
 
     assert await execute("workflows list") == ["sleep_workflow", "wait_for_collect_done", "test_workflow"]
     assert await execute("workflows show test_workflow") == [to_js(test_workflow)]
     wf = await execute("workflows run test_workflow")
     assert wf[0].startswith("Workflow test_workflow started with id")  # type: ignore
-    assert len(await execute("workflows running")) == 1
+    running = await execute("workflows running")
+    assert len(running) == 1
 
     # executing an already running workflow will give a specific message
     await execute("workflows run sleep_workflow")
     sf = await execute("workflows run sleep_workflow")
     assert sf[0].startswith("Workflow sleep_workflow already running with id ")  # type: ignore
 
+    # a workflow task can be stopped
+    task_id = running[0]["task-id"]  # type: ignore
+    af = await execute(f"workflows stop {task_id}")
+    assert af[0] == f"Workflow Task {task_id} stopped."
+
     # make sure to wait for all tasks to finish
     for rt in await task_handler.running_tasks():
         await task_handler.delete_running_task(rt)
 
     # access the history of all workflows
     history = AccessJson.wrap_list(await execute("workflows history"))
     assert len(history) == 1
@@ -1332,13 +1338,14 @@
         await sync_and_check(
             f"db sync sqlite --database db --host bla --port 1234 --user test --password check --arg foo=bla foo2=bla2",
             expected_table_count=11,
         )
     assert "sqlite://test:check@bla:1234" in str(ex.value)
     assert "?foo=bla&foo2=bla2" in str(ex.value)
 
-    # calling db without command will print the help
-    db_res = await cli.execute_cli_command("db", stream.list)
-    assert "Synchronizes data to an SQL database." in db_res[0][0]
+    # calling db without command will yield an error
+    with pytest.raises(Exception) as ex:
+        db_res = await cli.execute_cli_command("db", stream.list)
+    assert "Execute `help db` to get more information." in str(ex.value)
 
     # make sure argsinfo is available
     assert "sync" in cli.direct_commands["db"].args_info()
```

### Comparing `resotocore-3.6.1/tests/resotocore/cli/model_test.py` & `resotocore-3.6.2/tests/resotocore/cli/model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/config/config_handler_service_test.py` & `resotocore-3.6.2/tests/resotocore/config/config_handler_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/config/config_override_service_test.py` & `resotocore-3.6.2/tests/resotocore/config/config_override_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/config/core_config_handler_test.py` & `resotocore-3.6.2/tests/resotocore/config/core_config_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/conftest.py` & `resotocore-3.6.2/tests/resotocore/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from asyncio import Queue
 from collections import defaultdict
 from contextlib import suppress
 from datetime import timedelta
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from types import SimpleNamespace
-from typing import AsyncGenerator, Iterator, Dict, Any, Generator, Callable
+from typing import AsyncGenerator, Iterator, Dict, Any, Generator
 from typing import List, Optional
 from typing import Tuple, AsyncIterator, cast
 
 from aiohttp import ClientSession
 from aiohttp.hdrs import METH_ANY
 from aiohttp.test_utils import TestServer
 from aiohttp.web import Request, Response, Application, route
@@ -25,14 +25,15 @@
 from resotocore.action_handlers.merge_outer_edge_handler import MergeOuterEdgesHandler
 from resotocore.analytics import AnalyticsEventSender, InMemoryEventSender, NoEventSender
 from resotocore.cli.cli import CLIService
 from resotocore.cli.command import (
     alias_names,
     all_commands,
 )
+from resotocore.db.deferredouteredgedb import DeferredOuterEdgeDb
 from resotocore.dependencies import Dependencies
 from resotocore.config import ConfigHandler, ConfigEntity, ConfigValidation, ConfigOverride
 from resotocore.config.config_handler_service import ConfigHandlerService
 from resotocore.config.core_config_handler import CoreConfigHandler
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
 from resotocore.core_config import (
     GraphUpdateConfig,
@@ -40,15 +41,15 @@
     EditableConfig,
     DatabaseConfig,
     RuntimeConfig,
     CustomCommandsConfig,
     SnapshotsScheduleConfig,
     RunConfig,
 )
-from resotocore.db import runningtaskdb, SystemData
+from resotocore.db import runningtaskdb, SystemData, deferredouteredgedb
 from resotocore.db.async_arangodb import AsyncArangoDB
 from resotocore.db.db_access import DbAccess
 from resotocore.db.graphdb import ArangoGraphDB, EventGraphDB
 from resotocore.db.jobdb import JobDb
 from resotocore.db.packagedb import PackageEntityDb, app_package_entity_db
 from resotocore.db.runningtaskdb import RunningTaskDb
 from resotocore.db.system_data_db import SystemDataDb
@@ -73,15 +74,15 @@
 from resotocore.model.typed_model import to_js
 from resotocore.query.template_expander import TemplateExpander
 from resotocore.report import BenchmarkConfigPrefix, CheckConfigPrefix, Benchmark
 from resotocore.report.inspector_service import InspectorService
 from resotocore.report.report_config import BenchmarkConfig
 from resotocore.task.task_dependencies import TaskDependencies
 from resotocore.task.model import Subscriber, Subscription
-from resotocore.task.scheduler import Scheduler
+from resotocore.task.scheduler import APScheduler
 from resotocore.task.subscribers import SubscriptionHandler
 from resotocore.task.task_description import (
     Step,
     PerformAction,
     WaitForEvent,
     EmitEvent,
     StepErrorBehaviour,
@@ -196,14 +197,22 @@
 async def running_task_db(async_db: AsyncArangoDB) -> RunningTaskDb:
     task_db = runningtaskdb.running_task_db(async_db, "running_tasks")
     await task_db.create_update_schema()
     await task_db.wipe()
     return task_db
 
 
+@fixture
+async def pending_deferred_edge_db(async_db: AsyncArangoDB) -> DeferredOuterEdgeDb:
+    edges_db = deferredouteredgedb.deferred_outer_edge_db(async_db, "pending_deferred_edge")
+    await edges_db.create_update_schema()
+    await edges_db.wipe()
+    return edges_db
+
+
 @fixture()
 def db_access(graph_db: ArangoGraphDB) -> DbAccess:
     access = DbAccess(graph_db.db.db, NoEventSender(), NoAdjust(), empty_config())
     return access
 
 
 @fixture
@@ -729,15 +738,23 @@
     graph_merger: GraphMerger,
     cli: CLIService,
     test_workflow: Workflow,
     additional_workflows: List[Workflow],
 ) -> AsyncGenerator[TaskHandlerService, None]:
     config = empty_config()
     task_handler = TaskHandlerService(
-        running_task_db, job_db, message_bus, event_sender, subscription_handler, graph_merger, Scheduler(), cli, config
+        running_task_db,
+        job_db,
+        message_bus,
+        event_sender,
+        subscription_handler,
+        graph_merger,
+        APScheduler(),
+        cli,
+        config,
     )
     task_handler.task_descriptions = additional_workflows + [test_workflow]
     cli.dependencies.lookup["task_handler"] = task_handler
     async with task_handler:
         yield task_handler
 
 
@@ -805,19 +822,7 @@
     with suppress(Exception):
         test_db.insert_document(
             "system_data", {"_key": "ca", "key": "private_key", "certificate": "some cert"}, overwrite=False
         )
     async_db = AsyncArangoDB(test_db)
     yield SystemDataDb(async_db)
     test_db.collection("system_data").delete({"_key": "ca"})
-
-
-async def eventually(
-    predicate: Callable[[], bool],
-    timeout: timedelta = timedelta(seconds=5),
-    interval: timedelta = timedelta(seconds=0.1),
-) -> None:
-    async def wait_for_condition() -> None:
-        while not predicate():
-            await asyncio.sleep(interval.total_seconds())
-
-    await asyncio.wait_for(wait_for_condition(), timeout.total_seconds())
```

### Comparing `resotocore-3.6.1/tests/resotocore/console_renderer_test.py` & `resotocore-3.6.2/tests/resotocore/console_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/core_config_test.py` & `resotocore-3.6.2/tests/resotocore/core_config_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/arango_query_test.py` & `resotocore-3.6.2/tests/resotocore/db/arango_query_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/arangodb_functions_test.py` & `resotocore-3.6.2/tests/resotocore/db/arangodb_functions_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/async_arangodb_test.py` & `resotocore-3.6.2/tests/resotocore/db/async_arangodb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/configdb_test.py` & `resotocore-3.6.2/tests/resotocore/db/configdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/db_access_test.py` & `resotocore-3.6.2/tests/resotocore/db/db_access_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/entitydb.py` & `resotocore-3.6.2/tests/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/graphdb_test.py` & `resotocore-3.6.2/tests/resotocore/db/graphdb_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import asyncio
 import string
 from abc import ABC, abstractmethod
 from datetime import date, datetime, timedelta
 from random import SystemRandom
-from typing import List, Optional, Any, cast
+from typing import List, Optional, Any, Dict, cast
 
 from arango.database import StandardDatabase
 from arango.typings import Json
 from attrs import define
 from networkx import MultiDiGraph
 from pytest import mark, raises
 
 from resotocore.analytics import CoreEvent, InMemoryEventSender
 from resotocore.db.graphdb import ArangoGraphDB, GraphDB, EventGraphDB, HistoryChange
 from resotocore.db.model import QueryModel, GraphUpdate
 from resotocore.db.db_access import DbAccess
 from resotocore.error import ConflictingChangeInProgress, NoSuchChangeError, InvalidBatchUpdate
 from resotocore.ids import NodeId, GraphName
 from resotocore.model.graph_access import GraphAccess, EdgeTypes, Section
-from resotocore.model.model import Model, UsageDatapoint, UsageMetricValues
+from resotocore.model.model import Model, UsageDatapoint
 from resotocore.model.typed_model import from_js, to_js
 from resotocore.query.model import Query, P, Navigation
 from resotocore.query.query_parser import parse_query
 from resotocore.types import JsonElement, EdgeType
 from resotocore.util import AccessJson, utc, value_in_path, AccessNone
+from tests.resotocore.utils import eventually
 
 
 class BaseResource(ABC):
     def __init__(
         self,
         identifier: str,
     ) -> None:
@@ -177,16 +178,16 @@
 async def test_update_merge_batched(graph_db: ArangoGraphDB, foo_model: Model, test_db: StandardDatabase) -> None:
     md = foo_model
     await graph_db.wipe()
     batch_id = "".join(SystemRandom().choice(string.ascii_letters) for _ in range(12))
     g = create_graph("yes or no")
     await graph_db.insert_usage_data(
         [
-            UsageDatapoint("0", at=100, v={"cpu": UsageMetricValues(42, 42, 42)}, change_id=batch_id),
-            UsageDatapoint("0", at=101, v={"cpu": UsageMetricValues(43, 43, 43)}, change_id="foo"),
+            UsageDatapoint("0", at=100, v={"cpu": {"min": 42, "avg": 42, "max": 42}}, change_id=batch_id),
+            UsageDatapoint("0", at=101, v={"cpu": {"min": 0.42, "avg": 0.42, "max": 0.42}}, change_id="foo"),
         ]
     )
 
     # empty database: all changes are written to a temp table
     assert await graph_db.merge_graph(g, foo_model, batch_id, True) == (
         ["collector"],
         GraphUpdate(112, 1, 0, 212, 0, 0),
@@ -216,28 +217,35 @@
     await graph_db.wipe()
 
     def create(txt: str, width: int = 10) -> MultiDiGraph:
         return create_graph(txt, width=width)
 
     await graph_db.insert_usage_data(
         [
-            UsageDatapoint("0", at=100, v={"cpu": UsageMetricValues(42, 42, 42)}, change_id="foo"),
-            UsageDatapoint("0", at=101, v={"cpu": UsageMetricValues(43, 43, 43)}, change_id="bar"),
+            UsageDatapoint("0", at=100, v={"cpu": {"min": 42, "avg": 42, "max": 42}}, change_id="foo"),
+            UsageDatapoint("0", at=101, v={"cpu": {"min": 0.42, "avg": 0.42, "max": 0.42}}, change_id="bar"),
         ]
     )
 
     p = ["collector"]
     # empty database: all nodes and all edges have to be inserted, the root node is updated and the link to root added
     assert await graph_db.merge_graph(create("yes or no"), foo_model, maybe_change_id="foo") == (
         p,
         GraphUpdate(112, 1, 0, 212, 0, 0),
     )
+
     # check the usage
-    n = await graph_db.get_node(foo_model, NodeId("0")) or {}
-    assert n.get("usage", {}).get("cpu") == {"min": 42, "avg": 42, "max": 42}
+    async def check_usage() -> bool:
+        n = await graph_db.get_node(foo_model, NodeId("0")) or {}
+        node_usage: Dict[str, float] = n.get("usage", {}).get("cpu", {})
+        expected = {"min": 42, "avg": 42, "max": 42}
+        return node_usage == expected
+
+    await eventually(check_usage)
+
     # exactly the same graph is updated: expect no changes
     assert await graph_db.merge_graph(create("yes or no"), foo_model) == (p, GraphUpdate(0, 0, 0, 0, 0, 0))
     # all bla entries have different content: expect 100 node updates, but no inserts or deletions
     assert await graph_db.merge_graph(create("maybe"), foo_model) == (p, GraphUpdate(0, 100, 0, 0, 0, 0))
     # the width of the graph is reduced: expect nodes and edges to be removed
     assert await graph_db.merge_graph(create("maybe", width=5), foo_model) == (p, GraphUpdate(0, 0, 80, 0, 0, 155))
     # going back to the previous graph: the same amount of nodes and edges is inserted
@@ -661,15 +669,15 @@
     await db_access.delete_graph(GraphName("snapshot-" + graph_db.name))
 
     snapshot_db_name = GraphName("snapshot-" + graph_db.name)
     snapshot_db = await graph_db.copy_graph(snapshot_db_name, to_snapshot=True)
 
     with raises(ValueError) as ex:
         await snapshot_db.insert_usage_data(
-            [UsageDatapoint("foo", 42, "foo", {"cpu": UsageMetricValues(0.42, 0.42, 0.42)})]
+            [UsageDatapoint("foo", 42, "foo", {"cpu": {"min": 0.42, "avg": 0.42, "max": 0.42}})]
         )
 
     assert str(ex.value) == "Cannot insert usage data into a snapshot graph"
 
     # clean up
     await snapshot_db.wipe()
```

### Comparing `resotocore-3.6.1/tests/resotocore/db/jobdb_test.py` & `resotocore-3.6.2/tests/resotocore/db/jobdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/modeldb_test.py` & `resotocore-3.6.2/tests/resotocore/db/modeldb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/runningtaskdb_test.py` & `resotocore-3.6.2/tests/resotocore/db/runningtaskdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/subscriberdb_test.py` & `resotocore-3.6.2/tests/resotocore/db/subscriberdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/system_data_db_test.py` & `resotocore-3.6.2/tests/resotocore/db/system_data_db_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/db/templatedb_test.py` & `resotocore-3.6.2/tests/resotocore/db/templatedb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/dependencies_test.py` & `resotocore-3.6.2/tests/resotocore/dependencies_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/graph_manager/graph_manager_test.py` & `resotocore-3.6.2/tests/resotocore/graph_manager/graph_manager_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/hypothesis_extension.py` & `resotocore-3.6.2/tests/resotocore/hypothesis_extension.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/infra_apps/local_runtime_test.py` & `resotocore-3.6.2/tests/resotocore/infra_apps/local_runtime_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/infra_apps/package_manager_test.py` & `resotocore-3.6.2/tests/resotocore/infra_apps/package_manager_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/message_bus_test.py` & `resotocore-3.6.2/tests/resotocore/message_bus_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Message,
     Event,
     Action,
     ActionDone,
     ActionError,
     ActionInfo,
     ActionProgress,
+    ActionAbort,
 )
 from resotocore.model.typed_model import to_js, from_js
 from resotocore.util import AnyT, utc, first
 from resotolib.core.progress import ProgressDone, Progress
 
 
 async def wait_for_message(
@@ -81,14 +82,15 @@
     roundtrip(Action("test", task_id, "step_name", {"test": 1}))
     roundtrip(ActionDone("test", task_id, "step_name", subsctiber_id))
     roundtrip(ActionDone("test", task_id, "step_name", subsctiber_id, {"test": 1}))
     roundtrip(ActionError("test", task_id, "step_name", subsctiber_id, "oops"))
     roundtrip(ActionError("test", task_id, "step_name", subsctiber_id, "oops", {"test": 23}))
     roundtrip(ActionInfo("test", task_id, "step_name", subsctiber_id, "error", "Error message"))
     roundtrip(ActionProgress("test", task_id, "step_name", subsctiber_id, ProgressDone("region", 1, 2), now))
+    roundtrip(ActionAbort("test", task_id, "step_name", {"test": 1}))
     nested = Progress.from_progresses("account1", [ProgressDone("region", 1, 2)])
     pg = ActionProgress("test", task_id, "step_name", subsctiber_id, nested, now)
     assert to_js(pg) == to_js(from_js(to_js(pg), ActionProgress))
 
 
 def roundtrip(obj: Any) -> None:
     js = to_js(obj)
```

### Comparing `resotocore-3.6.1/tests/resotocore/model/__init__.py` & `resotocore-3.6.2/tests/resotocore/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/model/adjust_node_test.py` & `resotocore-3.6.2/tests/resotocore/model/adjust_node_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/model/db_updater_test.py` & `resotocore-3.6.2/tests/resotocore/model/db_updater_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from datetime import timedelta
 from multiprocessing import set_start_method
 from typing import List, AsyncGenerator, Any
 
 import pytest
 
 from resotocore.analytics import AnalyticsEventSender
-from resotocore.db.deferred_edge_db import pending_deferred_edge_db
+from resotocore.db.deferredouteredgedb import deferred_outer_edge_db
 from resotocore.db.graphdb import ArangoGraphDB
 from resotocore.db.model import GraphUpdate
+from resotocore.model.graph_access import DeferredEdge, ByNodeId
 from resotocore.system_start import empty_config
-from resotocore.ids import TaskId
+from resotocore.ids import TaskId, NodeId
 from resotocore.message_bus import MessageBus
 from resotocore.model.db_updater import GraphMerger
 from resotocore.model.model import Kind, Model
 from resotocore.model.typed_model import to_js
-from resotocore.types import Json
 from tests.resotocore.db.graphdb_test import create_graph
 from tests.resotocore.model import ModelHandlerStatic
 
 
 @pytest.mark.asyncio
 async def test_merge_process(
     event_sender: AnalyticsEventSender, graph_db: ArangoGraphDB, foo_kinds: List[Kind], message_bus: MessageBus
@@ -32,16 +32,17 @@
     await graph_db.wipe()
     # store the model in db, so it can be loaded by the sub process
     graph_db.db.collection(f"{graph_db.name}_model").insert_many([to_js(a) for a in foo_kinds])
     # define args to parse for the sub process
     config = empty_config(["--graphdb-username", "test", "--graphdb-password", "test", "--graphdb-database", "test"])
     # create sample graph data to insert
     graph = create_graph("test")
-
-    await pending_deferred_edge_db(graph_db.db, "deferred_outer_edges").create_update_schema()
+    outer_edge_db = deferred_outer_edge_db(graph_db.db, "deferred_outer_edges")
+    await outer_edge_db.create_update_schema()
+    await outer_edge_db.wipe()
 
     async def iterator() -> AsyncGenerator[bytes, None]:
         def to_b(a: Any) -> bytes:
             return bytes(json.dumps(a) + "\n", "utf-8")
 
         for node in graph.nodes():
             yield to_b(graph.nodes[node])
@@ -49,26 +50,24 @@
             yield to_b({"from": from_node, "to": to_node, "edge_type": data["edge_type"]})
         yield to_b(
             {"from_selector": {"node_id": "id_123"}, "to_selector": {"node_id": "id_456"}, "edge_type": "delete"}
         )
 
     model_handler = ModelHandlerStatic(Model.from_kinds(foo_kinds))
     async with GraphMerger(model_handler, event_sender, config, message_bus) as merger:
+        task_id = TaskId("test_task_123")
         result = await merger.merge_graph(
-            graph_db, iterator(), timedelta(seconds=30), None, TaskId("test_task_123"), wait_for_result=True
+            graph_db, iterator(), timedelta(seconds=30), None, task_id, wait_for_result=True
         )
         assert result == GraphUpdate(112, 1, 0, 212, 0, 0)
-        elem: Json = graph_db.db.collection("deferred_outer_edges").get("test_task_123")  # type: ignore
-        assert elem["_key"] == "test_task_123"
-        assert elem["task_id"] == "test_task_123"
-        assert elem["edges"][0] == {
-            "from_node": {"value": "id_123"},
-            "to_node": {"value": "id_456"},
-            "edge_type": "delete",
-        }
+        edges = await outer_edge_db.all_for_task(task_id)
+        assert len(edges) == 1
+        elem = edges[0]
+        assert elem.task_id == "test_task_123"
+        assert elem.edges[0] == DeferredEdge(ByNodeId(NodeId("id_123")), ByNodeId(NodeId("id_456")), "delete")
 
         # make another update without wait
         current_count = graph_db.db.collection("ns").count()
         graph = create_graph("test2", width=1)
         no_result = await merger.merge_graph(
             graph_db, iterator(), timedelta(seconds=30), None, TaskId("test_task_124"), wait_for_result=False
         )
```

### Comparing `resotocore-3.6.1/tests/resotocore/model/graph_access_test.py` & `resotocore-3.6.2/tests/resotocore/model/graph_access_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/model/json_schema_test.py` & `resotocore-3.6.2/tests/resotocore/model/json_schema_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/model/model_handler_test.py` & `resotocore-3.6.2/tests/resotocore/model/model_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/model/model_test.py` & `resotocore-3.6.2/tests/resotocore/model/model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/model/typed_model_test.py` & `resotocore-3.6.2/tests/resotocore/model/typed_model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/query/__init__.py` & `resotocore-3.6.2/tests/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/query/model_test.py` & `resotocore-3.6.2/tests/resotocore/query/model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/query/query_parser_test.py` & `resotocore-3.6.2/tests/resotocore/query/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/query/template_expander_test.py` & `resotocore-3.6.2/tests/resotocore/query/template_expander_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/report/benchnmark_renderer_test.py` & `resotocore-3.6.2/tests/resotocore/report/benchnmark_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/report/inspector_service_test.py` & `resotocore-3.6.2/tests/resotocore/report/inspector_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/task/job_handler_test.py` & `resotocore-3.6.2/tests/resotocore/task/job_handler_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from typing import List, Optional, Dict
 
 from resotocore.task import TaskHandler, RunningTaskInfo
 from resotocore.task.task_description import RunningTask, Job, Workflow
-from resotocore.ids import TaskDescriptorId
+from resotocore.ids import TaskDescriptorId, TaskId
 from resotocore.util import first
 
 
 class InMemJobHandler(TaskHandler):
     def __init__(self) -> None:
         self.jobs: List[Job] = []
         self.started_tasks: List[TaskDescriptorId] = []
 
+    async def stop_task(self, uid: TaskId) -> Optional[RunningTask]:
+        return None
+
     async def list_jobs(self) -> List[Job]:
         return self.jobs
 
     async def list_workflows(self) -> List[Workflow]:
         return []
 
     async def add_job(
```

### Comparing `resotocore-3.6.1/tests/resotocore/task/start_workflow_on_first_subscriber_test.py` & `resotocore-3.6.2/tests/resotocore/task/start_workflow_on_first_subscriber_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/task/subscribers_test.py` & `resotocore-3.6.2/tests/resotocore/task/subscribers_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/task/task_description_test.py` & `resotocore-3.6.2/tests/resotocore/task/task_description_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, List, Dict, Tuple, Callable
 
 from attr import evolve
 from deepdiff import DeepDiff
 from frozendict import frozendict
 
 from resotocore.ids import SubscriberId, TaskDescriptorId
-from resotocore.message_bus import Action, ActionDone, ActionError, Event, ActionProgress, ActionInfo
+from resotocore.message_bus import Action, ActionDone, ActionError, Event, ActionProgress, ActionInfo, ActionAbort
 from resotocore.model.typed_model import from_js, to_js
 from resotocore.task.task_dependencies import TaskDependencies
 from resotocore.task.model import Subscriber, Subscription
 from resotocore.task.task_description import (
     Workflow,
     Step,
     RunningTask,
@@ -237,7 +237,16 @@
     assert task.not_emitted_progress() is None
     # add progress updates
     task.handle_progress(ActionProgress("collect", task.id, "collect", sub.id, ProgressDone("collect", 0, 100), utc()))
     assert task.not_emitted_progress() is not None
     # no progress update, nothing to emit
     assert task.not_emitted_progress() is None
     assert task.not_emitted_progress() is None
+
+
+def test_abort(workflow_instance: Tuple[RunningTask, Subscriber, Subscriber, Dict[str, List[Subscriber]]]) -> None:
+    task, _, _, _ = workflow_instance
+    result = task.current_state.abort()
+    assert len(result) == 1
+    assert isinstance(result[0], SendMessage)
+    # noinspection PyUnresolvedReferences
+    assert isinstance(result[0].message, ActionAbort)
```

### Comparing `resotocore-3.6.1/tests/resotocore/task/task_handler_test.py` & `resotocore-3.6.2/tests/resotocore/task/task_handler_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from typing import List
 
 import pytest
 from pytest import LogCaptureFixture
 
 from resotocore.analytics import AnalyticsEventSender, InMemoryEventSender
 from resotocore.cli.cli import CLIService
-from tests.resotocore.conftest import eventually
+from tests.resotocore.utils import eventually
 from resotocore.db.jobdb import JobDb
 from resotocore.db.runningtaskdb import RunningTaskDb
 from resotocore.system_start import empty_config
 from resotocore.ids import SubscriberId, TaskDescriptorId
 from resotocore.message_bus import MessageBus, Event, Message, ActionDone, Action, ActionInfo, ActionError, CoreMessage
 from resotocore.model.db_updater import GraphMerger
-from resotocore.task.scheduler import Scheduler
+from resotocore.task.scheduler import APScheduler
 from resotocore.task.subscribers import SubscriptionHandler
 from resotocore.task.task_description import (
     Workflow,
     EventTrigger,
     TimeTrigger,
     Job,
     TaskSurpassBehaviour,
@@ -54,15 +54,15 @@
         th = TaskHandlerService(
             running_task_db,
             job_db,
             message_bus,
             event_sender,
             subscription_handler,
             graph_merger,
-            Scheduler(),
+            APScheduler(),
             cli,
             empty_config(),
         )
         th.task_descriptions = [test_workflow]
         return th
 
     await subscription_handler.add_subscription(SubscriberId("sub_1"), "start_collect", True, timedelta(seconds=30))
```

### Comparing `resotocore-3.6.1/tests/resotocore/user/user_management_service_test.py` & `resotocore-3.6.2/tests/resotocore/user/user_management_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/util_test.py` & `resotocore-3.6.2/tests/resotocore/util_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/validator_test.py` & `resotocore-3.6.2/tests/resotocore/validator_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/web/api_client.py` & `resotocore-3.6.2/tests/resotocore/web/api_client.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/web/api_test.py` & `resotocore-3.6.2/tests/resotocore/web/api_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 import pytest
 from _pytest.fixtures import fixture
 from aiohttp import ClientSession, MultipartReader
 from networkx import MultiDiGraph
 from datetime import timedelta
 from resotoclient import models as rc
 from resotoclient.async_client import ResotoClient
+from resotoclient.json_utils import json_loadb
+from resotoclient.models import JsObject
 
 from resotolib.utils import get_free_port
 from tests.resotocore import create_graph
 from resotocore.__main__ import run
 from resotocore.analytics import AnalyticsEvent
 from resotocore.db.db_access import DbAccess
 from resotocore.model.model import predefined_kinds, Kind
 from resotocore.model.typed_model import to_js
 from resotocore.util import rnd_str, AccessJson, utc, utc_str
 from resotocore.ids import GraphName
-from resotoclient.json_utils import json_loadb
-from resotoclient.models import JsObject
 
 
 def graph_to_json(graph: MultiDiGraph) -> List[rc.JsObject]:
     ga: List[rc.JsValue] = [{**node, "type": "node"} for _, node in graph.nodes(data=True)]
     for from_node, to_node, data in graph.edges(data=True):
         ga.append({"type": "edge", "from": from_node, "to": to_node, "edge_type": data["edge_type"]})
     return ga
@@ -93,14 +93,16 @@
                 "test",
                 "--graphdb-username",
                 "test",
                 "--graphdb-password",
                 "test",
                 "--debug",
                 "--analytics-opt-out",
+                "--no-scheduling",
+                "--ignore-interrupted-tasks",
                 "--override",
                 f"resotocore.api.https_port=null",
                 f"resotocore.api.http_port={http_port}",
                 "resotocore.api.web_hosts=0.0.0.0",
                 "--override-path",
                 str(config_path),
                 *additional_args,
```

### Comparing `resotocore-3.6.1/tests/resotocore/web/certificate_handler_test.py` & `resotocore-3.6.2/tests/resotocore/web/certificate_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/web/content_renderer_test.py` & `resotocore-3.6.2/tests/resotocore/web/content_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.1/tests/resotocore/worker_task_queue_test.py` & `resotocore-3.6.2/tests/resotocore/worker_task_queue_test.py`

 * *Files identical despite different names*

