# Comparing `tmp/mimosa-0.1.3.tar.gz` & `tmp/mimosa-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimosa-0.1.3.tar", last modified: Fri Jul 21 11:20:16 2023, max compression
+gzip compressed data, was "mimosa-0.1.4.tar", last modified: Sat Jul 22 12:45:04 2023, max compression
```

## Comparing `mimosa-0.1.3.tar` & `mimosa-0.1.4.tar`

### file list

```diff
@@ -1,188 +1,191 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.101244 mimosa-0.1.3/
--rw-rw-rw-   0        0        0       66 2020-05-27 06:46:03.000000 mimosa-0.1.3/.gitattributes
--rw-rw-rw-   0        0        0     2098 2021-05-12 09:46:36.000000 mimosa-0.1.3/.gitignore
--rw-rw-rw-   0        0        0    35822 2020-05-18 11:44:25.000000 mimosa-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       26 2023-07-21 06:53:35.000000 mimosa-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5603 2023-07-21 11:20:16.101244 mimosa-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5308 2023-07-21 11:18:29.000000 mimosa-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.684654 mimosa-0.1.3/mimosa/
--rw-rw-rw-   0        0        0      108 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.738051 mimosa-0.1.3/mimosa/__pycache__/
--rw-rw-rw-   0        0        0      275 2023-07-21 07:54:49.000000 mimosa-0.1.3/mimosa/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3648 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/__pycache__/abstract_model.cpython-310.pyc
--rw-rw-rw-   0        0        0     6915 2023-07-21 07:41:57.000000 mimosa-0.1.3/mimosa/__pycache__/mimosa.cpython-310.pyc
--rw-rw-rw-   0        0        0     5160 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/abstract_model.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.758571 mimosa-0.1.3/mimosa/common/
--rw-rw-rw-   0        0        0     1206 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.774197 mimosa-0.1.3/mimosa/common/__pycache__/
--rw-rw-rw-   0        0        0     1361 2023-07-21 07:41:57.000000 mimosa-0.1.3/mimosa/common/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1405 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/__pycache__/economics.cpython-310.pyc
--rw-rw-rw-   0        0        0     9297 2023-07-21 07:41:59.000000 mimosa-0.1.3/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     3475 2023-07-21 07:42:42.000000 mimosa-0.1.3/mimosa/common/__pycache__/units.cpython-310.pyc
--rw-rw-rw-   0        0        0     1705 2023-07-21 07:42:41.000000 mimosa-0.1.3/mimosa/common/__pycache__/utils.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.774197 mimosa-0.1.3/mimosa/common/config/
--rw-rw-rw-   0        0        0        0 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.774197 mimosa-0.1.3/mimosa/common/config/__pycache__/
--rw-rw-rw-   0        0        0      191 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/config/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2230 2023-07-21 07:54:51.000000 mimosa-0.1.3/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc
--rw-rw-rw-   0        0        0     2429 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/parseconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.789824 mimosa-0.1.3/mimosa/common/config/utils/
--rw-rw-rw-   0        0        0      112 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.789824 mimosa-0.1.3/mimosa/common/config/utils/__pycache__/
--rw-rw-rw-   0        0        0      352 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/config/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1190 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc
--rw-rw-rw-   0        0        0     9387 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc
--rw-rw-rw-   0        0        0      969 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/utils/nested_dict.py
--rw-rw-rw-   0        0        0     8454 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/utils/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.805445 mimosa-0.1.3/mimosa/common/data/
--rw-rw-rw-   0        0        0       36 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.813051 mimosa-0.1.3/mimosa/common/data/__pycache__/
--rw-rw-rw-   0        0        0      232 2023-07-21 07:42:44.000000 mimosa-0.1.3/mimosa/common/data/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     6111 2023-07-21 07:42:44.000000 mimosa-0.1.3/mimosa/common/data/__pycache__/datastore.cpython-310.pyc
--rw-rw-rw-   0        0        0     1235 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/data/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     6574 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/data/datastore.py
--rw-rw-rw-   0        0        0     1463 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/data/utils.py
--rw-rw-rw-   0        0        0     1419 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/economics.py
--rw-rw-rw-   0        0        0     8234 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/pyomo_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.822557 mimosa-0.1.3/mimosa/common/regional_params/
--rw-rw-rw-   0        0        0       38 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/regional_params/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.838186 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/
--rw-rw-rw-   0        0        0      247 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2765 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc
--rw-rw-rw-   0        0        0     2404 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc
--rw-rw-rw-   0        0        0     1334 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc
--rw-rw-rw-   0        0        0     2754 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/regional_params/main.py
--rw-rw-rw-   0        0        0     2772 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/regional_params/region_mappers.py
--rw-rw-rw-   0        0        0     1340 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/regional_params/regional_param_container.py
--rw-rw-rw-   0        0        0     3579 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/units.py
--rw-rw-rw-   0        0        0     1220 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.838186 mimosa-0.1.3/mimosa/components/
--rw-rw-rw-   0        0        0        0 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.869432 mimosa-0.1.3/mimosa/components/__pycache__/
--rw-rw-rw-   0        0        0      188 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4889 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/abatement.cpython-310.pyc
--rw-rw-rw-   0        0        0     3844 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/burdensharing.cpython-310.pyc
--rw-rw-rw-   0        0        0     3333 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc
--rw-rw-rw-   0        0        0     6923 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/emissions.cpython-310.pyc
--rw-rw-rw-   0        0        0     3700 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc
--rw-rw-rw-   0        0        0     5469 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/abatement.py
--rw-rw-rw-   0        0        0     4025 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/burdensharing.py
--rw-rw-rw-   0        0        0     3697 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/cobbdouglas.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.869432 mimosa-0.1.3/mimosa/components/damages/
--rw-rw-rw-   0        0        0      116 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.900679 mimosa-0.1.3/mimosa/components/damages/__pycache__/
--rw-rw-rw-   0        0        0      364 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4552 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc
--rw-rw-rw-   0        0        0     4166 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc
--rw-rw-rw-   0        0        0     4299 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc
--rw-rw-rw-   0        0        0     3277 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc
--rw-rw-rw-   0        0        0     1274 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc
--rw-rw-rw-   0        0        0     5331 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/ad_rice2010.py
--rw-rw-rw-   0        0        0     4874 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/ad_rice2012.py
--rw-rw-rw-   0        0        0     6688 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/ad_witch.py
--rw-rw-rw-   0        0        0     4260 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/coacch.py
--rw-rw-rw-   0        0        0      971 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/nodamage.py
--rw-rw-rw-   0        0        0    10151 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissions.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.900679 mimosa-0.1.3/mimosa/components/emissiontrade/
--rw-rw-rw-   0        0        0      112 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.922815 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/
--rw-rw-rw-   0        0        0      348 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3898 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc
--rw-rw-rw-   0        0        0     2968 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc
--rw-rw-rw-   0        0        0     1414 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc
--rw-rw-rw-   0        0        0     5274 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissiontrade/emissiontrade.py
--rw-rw-rw-   0        0        0     3276 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissiontrade/globalcostpool.py
--rw-rw-rw-   0        0        0     1131 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissiontrade/notrade.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.922815 mimosa-0.1.3/mimosa/components/financialtransfer/
--rw-rw-rw-   0        0        0      105 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/financialtransfer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.938444 mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/
--rw-rw-rw-   0        0        0      336 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2230 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc
--rw-rw-rw-   0        0        0     1093 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc
--rw-rw-rw-   0        0        0     1968 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/financialtransfer/globaldamagepool.py
--rw-rw-rw-   0        0        0      939 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/financialtransfer/notransfer.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.938444 mimosa-0.1.3/mimosa/components/objective/
--rw-rw-rw-   0        0        0      101 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/objective/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.954082 mimosa-0.1.3/mimosa/components/objective/__pycache__/
--rw-rw-rw-   0        0        0      322 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/objective/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2118 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc
--rw-rw-rw-   0        0        0     1736 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/objective/__pycache__/utility.cpython-310.pyc
--rw-rw-rw-   0        0        0     1558 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/objective/globalcosts.py
--rw-rw-rw-   0        0        0     1713 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/objective/utility.py
--rw-rw-rw-   0        0        0     4213 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/sealevelrise.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.954082 mimosa-0.1.3/mimosa/components/welfare/
--rw-rw-rw-   0        0        0      165 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/welfare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.969690 mimosa-0.1.3/mimosa/components/welfare/__pycache__/
--rw-rw-rw-   0        0        0      391 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/welfare/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1882 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc
--rw-rw-rw-   0        0        0     2368 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc
--rw-rw-rw-   0        0        0     2133 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc
--rw-rw-rw-   0        0        0     1456 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_elasmu.py
--rw-rw-rw-   0        0        0     2048 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_general.py
--rw-rw-rw-   0        0        0     1663 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_zero.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.985317 mimosa-0.1.3/mimosa/concrete_model/
--rw-rw-rw-   0        0        0        0 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.985317 mimosa-0.1.3/mimosa/concrete_model/__pycache__/
--rw-rw-rw-   0        0        0      192 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     8590 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc
--rw-rw-rw-   0        0        0    15078 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/instantiate_params.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.000937 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/
--rw-rw-rw-   0        0        0       39 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.023093 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/
--rw-rw-rw-   0        0        0      256 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      677 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc
--rw-rw-rw-   0        0        0     1046 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc
--rw-rw-rw-   0        0        0     2504 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc
--rw-rw-rw-   0        0        0     2101 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0      493 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/deactivate_constraints.py
--rw-rw-rw-   0        0        0      907 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/main.py
--rw-rw-rw-   0        0        0     3369 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/set_constraints.py
--rw-rw-rw-   0        0        0     1557 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.023093 mimosa-0.1.3/mimosa/export/
--rw-rw-rw-   0        0        0      202 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/export/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.038745 mimosa-0.1.3/mimosa/export/__pycache__/
--rw-rw-rw-   0        0        0      418 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/export/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3355 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/export/__pycache__/plot.cpython-310.pyc
--rw-rw-rw-   0        0        0     2567 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/export/__pycache__/save.cpython-310.pyc
--rw-rw-rw-   0        0        0     5349 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/export/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     5262 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/export/plot.py
--rw-rw-rw-   0        0        0     3110 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/export/save.py
--rw-rw-rw-   0        0        0     5836 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/export/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.653412 mimosa-0.1.3/mimosa/inputdata/
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.054368 mimosa-0.1.3/mimosa/inputdata/config/
--rw-rw-rw-   0        0        0       13 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/config.yaml
--rw-rw-rw-   0        0        0     2296 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/config_R5.yaml
--rw-rw-rw-   0        0        0    13790 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/config_default.yaml
--rw-rw-rw-   0        0        0      154 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/default_units.yaml
--rw-rw-rw-   0        0        0      456 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/extra_units.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.054368 mimosa-0.1.3/mimosa/inputdata/data/
--rw-rw-rw-   0        0        0    89096 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/data/data_IMAGE_SSP.csv
--rw-rw-rw-   0        0        0    89101 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.069998 mimosa-0.1.3/mimosa/inputdata/params/
--rw-rw-rw-   0        0        0      491 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/ADRICE2010.csv
--rw-rw-rw-   0        0        0      593 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/ADRICE2012.csv
--rw-rw-rw-   0        0        0    34077 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/COACCH.csv
--rw-rw-rw-   0        0        0      321 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/economics.csv
--rw-rw-rw-   0        0        0     7044 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/mac.csv
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.101244 mimosa-0.1.3/mimosa/inputdata/regions/
--rw-rw-rw-   0        0        0      286 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_ADRICE2010.csv
--rw-rw-rw-   0        0        0      280 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_ADRICE2012.csv
--rw-rw-rw-   0        0        0      337 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_COACCH.csv
--rw-rw-rw-   0        0        0   167460 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_regions.json
--rw-rw-rw-   0        0        0   123689 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/R5_regions.json
--rw-rw-rw-   0        0        0    21007 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/country_ISO_codes.csv
--rw-rw-rw-   0        0        0     8217 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/mimosa.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.101244 mimosa-0.1.3/mimosa/socialcostofcarbon/
--rw-rw-rw-   0        0        0        0 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/socialcostofcarbon/__init__.py
--rw-rw-rw-   0        0        0     5546 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/socialcostofcarbon/scc.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.738051 mimosa-0.1.3/mimosa.egg-info/
--rw-rw-rw-   0        0        0     5603 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6851 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-21 11:19:19.000000 mimosa-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       61 2023-07-21 06:53:35.000000 mimosa-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0      217 2023-07-21 11:19:19.000000 mimosa-0.1.3/run.py
--rw-rw-rw-   0        0        0       42 2023-07-21 11:20:16.101244 mimosa-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-07-21 11:19:41.000000 mimosa-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:04.078626 mimosa-0.1.4/
+-rw-rw-rw-   0        0        0       66 2020-05-27 06:46:03.000000 mimosa-0.1.4/.gitattributes
+-rw-rw-rw-   0        0        0     2098 2021-05-12 09:46:36.000000 mimosa-0.1.4/.gitignore
+-rw-rw-rw-   0        0        0    35822 2020-05-18 11:44:25.000000 mimosa-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-07-21 06:53:35.000000 mimosa-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    46849 2023-07-22 12:45:04.076627 mimosa-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5308 2023-07-21 11:18:29.000000 mimosa-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.312842 mimosa-0.1.4/mimosa/
+-rw-rw-rw-   0        0        0      108 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.370765 mimosa-0.1.4/mimosa/__pycache__/
+-rw-rw-rw-   0        0        0      275 2023-07-21 15:09:23.000000 mimosa-0.1.4/mimosa/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3643 2023-07-21 19:36:45.000000 mimosa-0.1.4/mimosa/__pycache__/abstract_model.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6915 2023-07-22 10:51:47.000000 mimosa-0.1.4/mimosa/__pycache__/mimosa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5150 2023-07-21 19:35:54.000000 mimosa-0.1.4/mimosa/abstract_model.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.422897 mimosa-0.1.4/mimosa/common/
+-rw-rw-rw-   0        0        0     1206 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.444086 mimosa-0.1.4/mimosa/common/__pycache__/
+-rw-rw-rw-   0        0        0     1361 2023-07-21 15:09:23.000000 mimosa-0.1.4/mimosa/common/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1405 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/__pycache__/economics.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9297 2023-07-21 15:09:24.000000 mimosa-0.1.4/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3475 2023-07-21 15:09:24.000000 mimosa-0.1.4/mimosa/common/__pycache__/units.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1705 2023-07-21 15:09:24.000000 mimosa-0.1.4/mimosa/common/__pycache__/utils.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.449084 mimosa-0.1.4/mimosa/common/config/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.456085 mimosa-0.1.4/mimosa/common/config/__pycache__/
+-rw-rw-rw-   0        0        0      191 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/config/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2230 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2429 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/config/parseconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.502085 mimosa-0.1.4/mimosa/common/config/utils/
+-rw-rw-rw-   0        0        0      112 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/config/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.516085 mimosa-0.1.4/mimosa/common/config/utils/__pycache__/
+-rw-rw-rw-   0        0        0      352 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/config/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1190 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9387 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc
+-rw-rw-rw-   0        0        0      969 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/config/utils/nested_dict.py
+-rw-rw-rw-   0        0        0     8454 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/config/utils/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.561090 mimosa-0.1.4/mimosa/common/data/
+-rw-rw-rw-   0        0        0       36 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.573085 mimosa-0.1.4/mimosa/common/data/__pycache__/
+-rw-rw-rw-   0        0        0      232 2023-07-21 15:09:25.000000 mimosa-0.1.4/mimosa/common/data/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6111 2023-07-21 15:09:25.000000 mimosa-0.1.4/mimosa/common/data/__pycache__/datastore.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1235 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/data/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6574 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/data/datastore.py
+-rw-rw-rw-   0        0        0     1463 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/data/utils.py
+-rw-rw-rw-   0        0        0     1419 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/economics.py
+-rw-rw-rw-   0        0        0     8234 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/pyomo_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.632089 mimosa-0.1.4/mimosa/common/regional_params/
+-rw-rw-rw-   0        0        0       38 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/regional_params/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.649085 mimosa-0.1.4/mimosa/common/regional_params/__pycache__/
+-rw-rw-rw-   0        0        0      247 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/regional_params/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2765 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2404 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1334 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2754 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/regional_params/main.py
+-rw-rw-rw-   0        0        0     2772 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/regional_params/region_mappers.py
+-rw-rw-rw-   0        0        0     1340 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/regional_params/regional_param_container.py
+-rw-rw-rw-   0        0        0     3579 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/units.py
+-rw-rw-rw-   0        0        0     1220 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.757085 mimosa-0.1.4/mimosa/components/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.812085 mimosa-0.1.4/mimosa/components/__pycache__/
+-rw-rw-rw-   0        0        0      188 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/components/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4889 2023-07-21 07:42:48.000000 mimosa-0.1.4/mimosa/components/__pycache__/abatement.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3693 2023-07-22 10:17:11.000000 mimosa-0.1.4/mimosa/components/__pycache__/burdensharing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3334 2023-07-22 10:52:37.000000 mimosa-0.1.4/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6923 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/components/__pycache__/emissions.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4898 2023-07-21 15:14:41.000000 mimosa-0.1.4/mimosa/components/__pycache__/mitigation.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3700 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3785 2023-07-21 20:21:58.000000 mimosa-0.1.4/mimosa/components/burdensharing.py
+-rw-rw-rw-   0        0        0     3698 2023-07-22 10:52:22.000000 mimosa-0.1.4/mimosa/components/cobbdouglas.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.948085 mimosa-0.1.4/mimosa/components/damages/
+-rw-rw-rw-   0        0        0      116 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/damages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.978085 mimosa-0.1.4/mimosa/components/damages/__pycache__/
+-rw-rw-rw-   0        0        0      364 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/damages/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4552 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4166 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4299 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3289 2023-07-21 20:14:15.000000 mimosa-0.1.4/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1274 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5331 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/damages/ad_rice2010.py
+-rw-rw-rw-   0        0        0     4874 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/damages/ad_rice2012.py
+-rw-rw-rw-   0        0        0     6688 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/damages/ad_witch.py
+-rw-rw-rw-   0        0        0     4308 2023-07-21 20:06:17.000000 mimosa-0.1.4/mimosa/components/damages/coacch.py
+-rw-rw-rw-   0        0        0      971 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/damages/nodamage.py
+-rw-rw-rw-   0        0        0    10151 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/emissions.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.051085 mimosa-0.1.4/mimosa/components/emissiontrade/
+-rw-rw-rw-   0        0        0      112 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/emissiontrade/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.073089 mimosa-0.1.4/mimosa/components/emissiontrade/__pycache__/
+-rw-rw-rw-   0        0        0      348 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/components/emissiontrade/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3901 2023-07-21 15:14:41.000000 mimosa-0.1.4/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2971 2023-07-21 15:14:41.000000 mimosa-0.1.4/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1417 2023-07-21 15:14:41.000000 mimosa-0.1.4/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5278 2023-07-21 15:13:06.000000 mimosa-0.1.4/mimosa/components/emissiontrade/emissiontrade.py
+-rw-rw-rw-   0        0        0     3282 2023-07-21 15:13:14.000000 mimosa-0.1.4/mimosa/components/emissiontrade/globalcostpool.py
+-rw-rw-rw-   0        0        0     1135 2023-07-21 15:11:11.000000 mimosa-0.1.4/mimosa/components/emissiontrade/notrade.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.130086 mimosa-0.1.4/mimosa/components/financialtransfer/
+-rw-rw-rw-   0        0        0      105 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/financialtransfer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.144085 mimosa-0.1.4/mimosa/components/financialtransfer/__pycache__/
+-rw-rw-rw-   0        0        0      336 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/financialtransfer/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2230 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1093 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1968 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/financialtransfer/globaldamagepool.py
+-rw-rw-rw-   0        0        0      939 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/financialtransfer/notransfer.py
+-rw-rw-rw-   0        0        0     5488 2023-07-21 15:13:50.000000 mimosa-0.1.4/mimosa/components/mitigation.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.197087 mimosa-0.1.4/mimosa/components/objective/
+-rw-rw-rw-   0        0        0      101 2023-07-21 11:19:18.000000 mimosa-0.1.4/mimosa/components/objective/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.210090 mimosa-0.1.4/mimosa/components/objective/__pycache__/
+-rw-rw-rw-   0        0        0      322 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/objective/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2119 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1736 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/objective/__pycache__/utility.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1559 2023-07-21 15:07:20.000000 mimosa-0.1.4/mimosa/components/objective/globalcosts.py
+-rw-rw-rw-   0        0        0     1713 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/components/objective/utility.py
+-rw-rw-rw-   0        0        0     4213 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/components/sealevelrise.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.275086 mimosa-0.1.4/mimosa/components/welfare/
+-rw-rw-rw-   0        0        0      159 2023-07-21 19:35:35.000000 mimosa-0.1.4/mimosa/components/welfare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.292964 mimosa-0.1.4/mimosa/components/welfare/__pycache__/
+-rw-rw-rw-   0        0        0      385 2023-07-21 19:36:45.000000 mimosa-0.1.4/mimosa/components/welfare/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2127 2023-07-21 20:14:15.000000 mimosa-0.1.4/mimosa/components/welfare/__pycache__/cost_minimising.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1882 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2368 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2133 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1882 2023-07-21 20:14:15.000000 mimosa-0.1.4/mimosa/components/welfare/__pycache__/welfare_loss_minimising.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1663 2023-07-21 20:11:40.000000 mimosa-0.1.4/mimosa/components/welfare/cost_minimising.py
+-rw-rw-rw-   0        0        0     2048 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/components/welfare/inequal_aversion_general.py
+-rw-rw-rw-   0        0        0     1456 2023-07-21 20:11:40.000000 mimosa-0.1.4/mimosa/components/welfare/welfare_loss_minimising.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.322798 mimosa-0.1.4/mimosa/concrete_model/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/concrete_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.333016 mimosa-0.1.4/mimosa/concrete_model/__pycache__/
+-rw-rw-rw-   0        0        0      192 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/concrete_model/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8591 2023-07-21 15:14:41.000000 mimosa-0.1.4/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc
+-rw-rw-rw-   0        0        0    15080 2023-07-21 15:13:22.000000 mimosa-0.1.4/mimosa/concrete_model/instantiate_params.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.451251 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/
+-rw-rw-rw-   0        0        0       39 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.484762 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/
+-rw-rw-rw-   0        0        0      256 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      677 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1046 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2504 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2101 2023-07-21 15:10:56.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0      493 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/deactivate_constraints.py
+-rw-rw-rw-   0        0        0      907 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/main.py
+-rw-rw-rw-   0        0        0     3369 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/set_constraints.py
+-rw-rw-rw-   0        0        0     1557 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/concrete_model/simulation_mode/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.550921 mimosa-0.1.4/mimosa/export/
+-rw-rw-rw-   0        0        0      202 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/export/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.591921 mimosa-0.1.4/mimosa/export/__pycache__/
+-rw-rw-rw-   0        0        0      418 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/export/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3358 2023-07-21 15:14:40.000000 mimosa-0.1.4/mimosa/export/__pycache__/plot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2549 2023-07-22 10:23:47.000000 mimosa-0.1.4/mimosa/export/__pycache__/save.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5402 2023-07-21 15:09:29.000000 mimosa-0.1.4/mimosa/export/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5265 2023-07-21 15:14:02.000000 mimosa-0.1.4/mimosa/export/plot.py
+-rw-rw-rw-   0        0        0     3096 2023-07-22 10:19:04.000000 mimosa-0.1.4/mimosa/export/save.py
+-rw-rw-rw-   0        0        0     5836 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/export/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.248911 mimosa-0.1.4/mimosa/inputdata/
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.778016 mimosa-0.1.4/mimosa/inputdata/config/
+-rw-rw-rw-   0        0        0       13 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/config/config.yaml
+-rw-rw-rw-   0        0        0     2296 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/config/config_R5.yaml
+-rw-rw-rw-   0        0        0    13786 2023-07-21 19:36:17.000000 mimosa-0.1.4/mimosa/inputdata/config/config_default.yaml
+-rw-rw-rw-   0        0        0      154 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/config/default_units.yaml
+-rw-rw-rw-   0        0        0      456 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/config/extra_units.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.862070 mimosa-0.1.4/mimosa/inputdata/data/
+-rw-rw-rw-   0        0        0    89096 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/data/data_IMAGE_SSP.csv
+-rw-rw-rw-   0        0        0    89101 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:03.963355 mimosa-0.1.4/mimosa/inputdata/params/
+-rw-rw-rw-   0        0        0      491 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/params/ADRICE2010.csv
+-rw-rw-rw-   0        0        0      593 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/params/ADRICE2012.csv
+-rw-rw-rw-   0        0        0    34077 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/params/COACCH.csv
+-rw-rw-rw-   0        0        0      321 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/params/economics.csv
+-rw-rw-rw-   0        0        0     7044 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/params/mac.csv
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:04.063627 mimosa-0.1.4/mimosa/inputdata/regions/
+-rw-rw-rw-   0        0        0      286 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/regions/IMAGE26_ADRICE2010.csv
+-rw-rw-rw-   0        0        0      280 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/regions/IMAGE26_ADRICE2012.csv
+-rw-rw-rw-   0        0        0      337 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/regions/IMAGE26_COACCH.csv
+-rw-rw-rw-   0        0        0   167460 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/regions/IMAGE26_regions.json
+-rw-rw-rw-   0        0        0   123689 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/regions/R5_regions.json
+-rw-rw-rw-   0        0        0    21007 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/inputdata/regions/country_ISO_codes.csv
+-rw-rw-rw-   0        0        0     8217 2023-07-22 10:46:10.000000 mimosa-0.1.4/mimosa/mimosa.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:04.070628 mimosa-0.1.4/mimosa/socialcostofcarbon/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/socialcostofcarbon/__init__.py
+-rw-rw-rw-   0        0        0     5546 2023-07-21 11:19:19.000000 mimosa-0.1.4/mimosa/socialcostofcarbon/scc.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:45:02.360767 mimosa-0.1.4/mimosa.egg-info/
+-rw-rw-rw-   0        0        0    46849 2023-07-22 12:45:02.000000 mimosa-0.1.4/mimosa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7051 2023-07-22 12:45:02.000000 mimosa-0.1.4/mimosa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 12:45:02.000000 mimosa-0.1.4/mimosa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-22 12:45:02.000000 mimosa-0.1.4/mimosa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-22 12:45:02.000000 mimosa-0.1.4/mimosa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 11:19:19.000000 mimosa-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       61 2023-07-21 06:53:35.000000 mimosa-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0      217 2023-07-22 10:21:59.000000 mimosa-0.1.4/run.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 12:45:04.079629 mimosa-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-07-22 12:43:29.000000 mimosa-0.1.4/setup.py
```

### Comparing `mimosa-0.1.3/.gitignore` & `mimosa-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/LICENSE` & `mimosa-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/PKG-INFO` & `mimosa-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: mimosa
-Version: 0.1.3
-Summary: MIMOSA: Integrated Assessment Model for Cost-Benefit Analysis
-Author: Kaj-Ivar van der Wijst
-Author-email: k.i.vanderwijst@gmail.com
-License: LICENSE.txt
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MIMOSA: Mathematical Integrated Model for Optimal and Stylised Assessment
 
 MIMOSA is a recent simple IAM based on FAIR, with 26 regions covering the whole world. It is a relatively simple Cost-Benefit IAM but still covers the relevant technological and socio-economic dynamics. Temperature is a linear function of cumulative CO2 emissions. MIMOSA uses the DICE sea-level rise module. The mitigation costs, population, initial capital stock and baseline GDP and CO2 emissions are regional. The direct regional mitigation costs are calculated as area under the Marginal Abatement Cost (MAC) curve, and have been calibrated to the IPCC AR6 WGIII database.
 
 ### General
 
 The model is written in the Python optimisation package [Pyomo](https://www.pyomo.org/). It is mainly an `AbstractModel`
@@ -93,11 +83,11 @@
 ```
 
 ## How to cite
 When using MIMOSA, please cite [[1]](#1) (global version) and [[2]](#2) (regional version).
 
 ## References
 <a id="1">[1]</a> 
-van der Wijst, KI., Hof, A.F. & van Vuuren, D.P. On the optimality of 2Â°C targets and a decomposition of uncertainty. *Nature Communications* **12**, 2575 (2021). https://doi.org/10.1038/s41467-021-22826-5
+van der Wijst, KI., Hof, A.F. & van Vuuren, D.P. On the optimality of 2°C targets and a decomposition of uncertainty. *Nature Communications* **12**, 2575 (2021). https://doi.org/10.1038/s41467-021-22826-5
 
 <a id="2">[2]</a> 
-van der Wijst, KI., Bosello, F., Dasgupta, S. *et al*. New damage curves and multimodel analysis suggest lower optimal temperature. *Nature Climate Change* **13**, 434â€“441 (2023). https://doi.org/10.1038/s41558-023-01636-1
+van der Wijst, KI., Bosello, F., Dasgupta, S. *et al*. New damage curves and multimodel analysis suggest lower optimal temperature. *Nature Climate Change* **13**, 434–441 (2023). https://doi.org/10.1038/s41558-023-01636-1
```

### Comparing `mimosa-0.1.3/mimosa/__pycache__/abstract_model.cpython-310.pyc` & `mimosa-0.1.4/mimosa/__pycache__/abstract_model.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:41 2023 UTC, .py size: 5160 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b536 ba64 2814 0000  o........6.d(...
+00000000: 6f0d 0d0a 0000 0000 1ade ba64 1e14 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6401 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0f 5a0f 6d10 5a10 6d11 5a11 6d12 5a12  m.Z.m.Z.m.Z.m.Z.
@@ -17,212 +17,212 @@
 00000100: 6f6e 7461 696e 7320 616c 6c20 6d6f 6465  ontains all mode
 00000110: 6c20 6571 7561 7469 6f6e 7320 616e 6420  l equations and 
 00000120: 636f 6e73 7472 6169 6e74 730a e900 0000  constraints.....
 00000130: 004e 2904 da05 5061 7261 6dda 0d41 6273  .N)...Param..Abs
 00000140: 7472 6163 744d 6f64 656c da03 5365 74da  tractModel..Set.
 00000150: 0e61 6464 5f63 6f6e 7374 7261 696e 7429  .add_constraint)
 00000160: 0ada 0d62 7572 6465 6e73 6861 7269 6e67  ...burdensharing
-00000170: da09 656d 6973 7369 6f6e 73da 0961 6261  ..emissions..aba
-00000180: 7465 6d65 6e74 da0d 656d 6973 7369 6f6e  tement..emission
-00000190: 7472 6164 65da 1166 696e 616e 6369 616c  trade..financial
-000001a0: 7472 616e 7366 6572 da0b 636f 6262 646f  transfer..cobbdo
-000001b0: 7567 6c61 73da 0764 616d 6167 6573 da09  uglas..damages..
-000001c0: 6f62 6a65 6374 6976 65da 0c73 6561 6c65  objective..seale
-000001d0: 7665 6c72 6973 65da 0777 656c 6661 7265  velrise..welfare
-000001e0: da0d 6461 6d61 6765 5f6d 6f64 756c 65da  ..damage_module.
-000001f0: 1465 6d69 7373 696f 6e74 7261 6465 5f6d  .emissiontrade_m
-00000200: 6f64 756c 65da 1866 696e 616e 6369 616c  odule..financial
-00000210: 7472 616e 7366 6572 5f6d 6f64 756c 65da  transfer_module.
-00000220: 0e77 656c 6661 7265 5f6d 6f64 756c 65da  .welfare_module.
-00000230: 106f 626a 6563 7469 7665 5f6d 6f64 756c  .objective_modul
-00000240: 65da 0672 6574 7572 6e63 0500 0000 0000  e..returnc......
-00000250: 0000 0000 0000 0900 0000 0600 0000 0300  ................
-00000260: 0000 73fc 0200 0074 0083 0089 0167 007d  ..s....t.....g.}
-00000270: 0574 0183 0088 015f 0274 0183 0088 015f  .t....._.t....._
-00000280: 0374 0183 0088 015f 0474 0583 0088 015f  .t....._.t....._
-00000290: 0664 0088 015f 0774 0183 0088 015f 0874  .d..._.t....._.t
-000002a0: 0564 0164 028d 0188 015f 0964 0364 0484  .d.d....._.d.d..
-000002b0: 0088 015f 0a64 0564 0484 0088 015f 0b64  ..._.d.d....._.d
-000002c0: 0664 0484 0088 015f 0c64 0764 0484 0088  .d....._.d.d....
-000002d0: 015f 0d64 0864 0484 0088 015f 0e87 0166  ._.d.d....._...f
-000002e0: 0164 0964 0a84 0889 0088 0088 015f 0f87  .d.d........._..
-000002f0: 0066 0164 0b64 0484 0888 015f 107c 05a0  .f.d.d....._.|..
-00000300: 1174 12a0 1388 01a1 01a1 0101 007c 05a0  .t...........|..
-00000310: 1174 14a0 1388 01a1 01a1 0101 007c 0064  .t...........|.d
-00000320: 0c6b 0272 697c 05a0 1174 156a 16a0 1388  .k.ri|...t.j....
-00000330: 01a1 01a1 0101 006e 3a7c 0064 0d6b 0272  .......n:|.d.k.r
-00000340: 777c 05a0 1174 156a 17a0 1388 01a1 01a1  w|...t.j........
-00000350: 0101 006e 2c7c 0064 0e6b 0272 857c 05a0  ...n,|.d.k.r.|..
-00000360: 1174 156a 18a0 1388 01a1 01a1 0101 006e  .t.j...........n
-00000370: 1e7c 0064 0f6b 0272 937c 05a0 1174 156a  .|.d.k.r.|...t.j
-00000380: 19a0 1388 01a1 01a1 0101 006e 107c 0064  ...........n.|.d
-00000390: 106b 0272 a17c 05a0 1174 156a 1aa0 1388  .k.r.|...t.j....
-000003a0: 01a1 01a1 0101 006e 0274 1b82 017c 05a0  .......n.t...|..
-000003b0: 1174 1ca0 1388 01a1 01a1 0101 007c 0164  .t...........|.d
-000003c0: 116b 0272 b97c 05a0 1174 1d6a 1ea0 1388  .k.r.|...t.j....
-000003d0: 01a1 01a1 0101 006e 247c 0164 126b 0272  .......n$|.d.k.r
-000003e0: c77c 05a0 1174 1d6a 1fa0 1388 01a1 01a1  .|...t.j........
-000003f0: 0101 006e 167c 0164 136b 0272 d57c 05a0  ...n.|.d.k.r.|..
-00000400: 1174 1d6a 1da0 1388 01a1 01a1 0101 006e  .t.j...........n
-00000410: 0874 1b64 147c 019b 0064 159d 0383 0182  .t.d.|...d......
-00000420: 017c 0264 166b 0272 eb7c 05a0 1174 206a  .|.d.k.r.|...t j
-00000430: 21a0 1388 01a1 01a1 0101 006e 167c 0264  !..........n.|.d
-00000440: 176b 0272 f97c 05a0 1174 206a 22a0 1388  .k.r.|...t j"...
-00000450: 01a1 01a1 0101 006e 0874 1b64 187c 029b  .......n.t.d.|..
-00000460: 0064 159d 0383 0182 017c 05a0 1174 23a0  .d.......|...t#.
-00000470: 1388 01a1 01a1 0101 007c 05a0 1174 24a0  .........|...t$.
-00000480: 1388 01a1 01a1 0101 007c 0364 196b 0290  .........|.d.k..
-00000490: 0172 207c 05a0 1174 256a 26a0 1388 01a1  .r |...t%j&.....
-000004a0: 01a1 0101 006e 267c 0364 1a6b 0290 0172  .....n&|.d.k...r
-000004b0: 2f7c 05a0 1174 256a 27a0 1388 01a1 01a1  /|...t%j'.......
-000004c0: 0101 006e 177c 0364 1b6b 0290 0172 3e7c  ...n.|.d.k...r>|
-000004d0: 05a0 1174 256a 28a0 1388 01a1 01a1 0101  ...t%j(.........
-000004e0: 006e 0874 1b64 1c7c 039b 0064 159d 0383  .n.t.d.|...d....
-000004f0: 0182 017c 0464 1d6b 0290 0172 5474 296a  ...|.d.k...rTt)j
-00000500: 2aa0 1388 01a1 015c 027d 067d 076e 107c  *......\.}.}.n.|
-00000510: 0464 1e6b 0290 0172 6274 296a 2ba0 1388  .d.k...rbt)j+...
-00000520: 01a1 015c 027d 067d 076e 0274 1b82 017c  ...\.}.}.n.t...|
-00000530: 05a0 117c 07a1 0101 007c 0544 005d 0d7d  ...|.....|.D.].}
-00000540: 0874 2c88 017c 08a0 2d88 01a1 017c 086a  .t,..|..-....|.j
-00000550: 2e83 0301 0090 0171 6b7c 0688 015f 2f88  .......qk|..._/.
-00000560: 0153 0029 1f4e 5429 01da 076f 7264 6572  .S.).NT)...order
-00000570: 6564 6302 0000 0000 0000 0000 0000 0002  edc.............
-00000580: 0000 0001 0000 0053 0000 00f3 0400 0000  .......S........
-00000590: 6400 5300 a901 4ea9 00a9 02da 0479 6561  d.S...N......yea
-000005a0: 72da 0672 6567 696f 6e72 1900 0000 7219  r..regionr....r.
-000005b0: 0000 00fa 5a63 3a5c 7573 6572 735c 3339  ....Zc:\users\39
-000005c0: 3033 3838 355c 6f6e 6564 7269 7665 202d  03885\onedrive -
-000005d0: 2075 6e69 7665 7273 6974 6569 7420 7574   universiteit ut
-000005e0: 7265 6368 745c 646f 6375 6d65 6e74 735c  recht\documents\
-000005f0: 6d69 6d6f 7361 5c6d 696d 6f73 615c 6162  mimosa\mimosa\ab
-00000600: 7374 7261 6374 5f6d 6f64 656c 2e70 79da  stract_model.py.
-00000610: 083c 6c61 6d62 6461 3e39 0000 00f3 0200  .<lambda>9......
-00000620: 0000 0400 7a27 6372 6561 7465 5f61 6273  ....z'create_abs
-00000630: 7472 6163 745f 6d6f 6465 6c2e 3c6c 6f63  tract_model.<loc
-00000640: 616c 733e 2e3c 6c61 6d62 6461 3e63 0200  als>.<lambda>c..
-00000650: 0000 0000 0000 0000 0000 0200 0000 0100  ................
-00000660: 0000 5300 0000 7217 0000 0072 1800 0000  ..S...r....r....
-00000670: 7219 0000 0072 1a00 0000 7219 0000 0072  r....r....r....r
-00000680: 1900 0000 721d 0000 0072 1e00 0000 3a00  ....r....r....:.
-00000690: 0000 721f 0000 0063 0200 0000 0000 0000  ..r....c........
-000006a0: 0000 0000 0200 0000 0100 0000 5300 0000  ............S...
-000006b0: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-000006c0: 1a00 0000 7219 0000 0072 1900 0000 721d  ....r....r....r.
-000006d0: 0000 0072 1e00 0000 3b00 0000 721f 0000  ...r....;...r...
-000006e0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-000006f0: 0000 0100 0000 5300 0000 7217 0000 0072  ......S...r....r
-00000700: 1800 0000 7219 0000 0072 1a00 0000 7219  ....r....r....r.
-00000710: 0000 0072 1900 0000 721d 0000 0072 1e00  ...r....r....r..
-00000720: 0000 3c00 0000 721f 0000 0063 0200 0000  ..<...r....c....
-00000730: 0000 0000 0000 0000 0200 0000 0100 0000  ................
-00000740: 5300 0000 7217 0000 0072 1800 0000 7219  S...r....r....r.
-00000750: 0000 0072 1a00 0000 7219 0000 0072 1900  ...r....r....r..
-00000760: 0000 721d 0000 0072 1e00 0000 3d00 0000  ..r....r....=...
-00000770: 721f 0000 0063 0300 0000 0000 0000 0000  r....c..........
-00000780: 0000 0400 0000 0500 0000 1300 0000 7324  ..............s$
-00000790: 0000 0074 00a0 017c 007c 0164 01a1 037d  ...t...|.|.d...}
-000007a0: 0374 006a 0288 00a0 037c 037c 02a1 027c  .t.j.....|.|...|
-000007b0: 0364 028d 0253 0029 034e e964 0000 0029  .d...S.).N.d...)
-000007c0: 01da 0178 2904 da02 6e70 da08 6c69 6e73  ...x)...np..lins
-000007d0: 7061 6365 da05 7472 6170 7ada 1262 6173  pace..trapz..bas
-000007e0: 656c 696e 655f 656d 6973 7369 6f6e 7329  eline_emissions)
-000007f0: 04da 0a79 6561 725f 7374 6172 74da 0879  ...year_start..y
-00000800: 6561 725f 656e 6472 1c00 0000 da05 7965  ear_endr......ye
-00000810: 6172 7329 01da 016d 7219 0000 0072 1d00  ars)...mr....r..
-00000820: 0000 da13 6261 7365 6c69 6e65 5f63 756d  ....baseline_cum
-00000830: 756c 6174 6976 653f 0000 0073 0400 0000  ulative?...s....
-00000840: 0e01 1601 7a32 6372 6561 7465 5f61 6273  ....z2create_abs
-00000850: 7472 6163 745f 6d6f 6465 6c2e 3c6c 6f63  tract_model.<loc
-00000860: 616c 733e 2e62 6173 656c 696e 655f 6375  als>.baseline_cu
-00000870: 6d75 6c61 7469 7665 6303 0000 0000 0000  mulativec.......
-00000880: 0000 0000 0003 0000 0004 0000 0013 0000  ................
-00000890: 0073 1c00 0000 7400 8702 8700 8701 6603  .s....t.......f.
-000008a0: 6401 6402 8408 7c00 6a01 4400 8301 8301  d.d...|.j.D.....
-000008b0: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-000008c0: 0000 0200 0000 0500 0000 3300 0000 731c  ..........3...s.
-000008d0: 0000 0081 007c 005d 097d 0188 0088 0288  .....|.].}......
-000008e0: 017c 0183 0356 0001 0071 0264 0053 0072  .|...V...q.d.S.r
-000008f0: 1800 0000 7219 0000 0029 02da 022e 30da  ....r....)....0.
-00000900: 0172 2903 722a 0000 0072 2700 0000 7226  .r).r*...r'...r&
-00000910: 0000 0072 1900 0000 721d 0000 00da 093c  ...r....r......<
-00000920: 6765 6e65 7870 723e 4400 0000 7308 0000  genexpr>D...s...
-00000930: 0002 8004 000c 010a ff7a 3a63 7265 6174  .........z:creat
-00000940: 655f 6162 7374 7261 6374 5f6d 6f64 656c  e_abstract_model
-00000950: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00000960: 613e 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  a>.<locals>.<gen
-00000970: 6578 7072 3e29 02da 0373 756d da07 7265  expr>)...sum..re
-00000980: 6769 6f6e 7329 0372 2900 0000 7226 0000  gions).r)...r&..
-00000990: 0072 2700 0000 2901 722a 0000 0029 0272  .r'...).r*...).r
-000009a0: 2700 0000 7226 0000 0072 1d00 0000 721e  '...r&...r....r.
-000009b0: 0000 0044 0000 0073 0600 0000 1000 0401  ...D...s........
-000009c0: 08ff 5a08 5249 4345 3230 3130 5a05 5749  ..Z.RICE2010Z.WI
-000009d0: 5443 485a 0852 4943 4532 3031 32da 0643  TCHZ.RICE2012..C
-000009e0: 4f41 4343 48da 086e 6f64 616d 6167 65da  OACCH..nodamage.
-000009f0: 076e 6f74 7261 6465 da0e 676c 6f62 616c  .notrade..global
-00000a00: 636f 7374 706f 6f6c 7209 0000 007a 1945  costpoolr....z.E
-00000a10: 6d69 7373 696f 6e20 7472 6164 696e 6720  mission trading 
-00000a20: 6d6f 6475 6c65 2060 7a11 6020 6e6f 7420  module `z.` not 
-00000a30: 696d 706c 656d 656e 7465 64da 0a6e 6f74  implemented..not
-00000a40: 7261 6e73 6665 72da 1067 6c6f 6261 6c64  ransfer..globald
-00000a50: 616d 6167 6570 6f6f 6c7a 1b46 696e 616e  amagepoolz.Finan
-00000a60: 6369 616c 2074 7261 6e73 6665 7220 6d6f  cial transfer mo
-00000a70: 6475 6c65 2060 da17 696e 6571 7561 6c5f  dule `..inequal_
-00000a80: 6176 6572 7369 6f6e 5f65 6c61 736d 75da  aversion_elasmu.
-00000a90: 1569 6e65 7175 616c 5f61 7665 7273 696f  .inequal_aversio
-00000aa0: 6e5f 7a65 726f da18 696e 6571 7561 6c5f  n_zero..inequal_
-00000ab0: 6176 6572 7369 6f6e 5f67 656e 6572 616c  aversion_general
-00000ac0: 7a10 5765 6c66 6172 6520 6d6f 6475 6c65  z.Welfare module
-00000ad0: 2060 da07 7574 696c 6974 79da 0b67 6c6f   `..utility..glo
-00000ae0: 6261 6c63 6f73 7473 2930 7203 0000 0072  balcosts)0r....r
-00000af0: 0200 0000 da09 6265 6769 6e79 6561 72da  ......beginyear.
-00000b00: 0264 74da 0274 6672 0400 0000 da01 7472  .dt..tfr......tr
-00000b10: 1b00 0000 5a08 7965 6172 3231 3030 722f  ....Z.year2100r/
-00000b20: 0000 0072 2500 0000 da0a 706f 7075 6c61  ...r%.....popula
-00000b30: 7469 6f6e da03 5446 50da 0347 4450 da10  tion..TFP..GDP..
-00000b40: 6361 7262 6f6e 5f69 6e74 656e 7369 7479  carbon_intensity
-00000b50: 722a 0000 005a 1a62 6173 656c 696e 655f  r*...Z.baseline_
-00000b60: 6375 6d75 6c61 7469 7665 5f67 6c6f 6261  cumulative_globa
-00000b70: 6cda 0665 7874 656e 6472 0700 0000 5a0f  l..extendr....Z.
-00000b80: 6765 745f 636f 6e73 7472 6169 6e74 7372  get_constraintsr
-00000b90: 0e00 0000 720c 0000 005a 0b61 645f 7269  ....r....Z.ad_ri
-00000ba0: 6365 3230 3130 5a08 6164 5f77 6974 6368  ce2010Z.ad_witch
-00000bb0: 5a0b 6164 5f72 6963 6532 3031 325a 0663  Z.ad_rice2012Z.c
-00000bc0: 6f61 6363 6872 3100 0000 da13 4e6f 7449  oacchr1.....NotI
-00000bd0: 6d70 6c65 6d65 6e74 6564 4572 726f 7272  mplementedErrorr
-00000be0: 0800 0000 7209 0000 0072 3200 0000 7233  ....r....r2...r3
-00000bf0: 0000 0072 0a00 0000 7234 0000 0072 3500  ...r....r4...r5.
-00000c00: 0000 7206 0000 0072 0b00 0000 720f 0000  ..r....r....r...
-00000c10: 0072 3600 0000 7237 0000 0072 3800 0000  .r6...r7...r8...
-00000c20: 720d 0000 0072 3900 0000 723a 0000 0072  r....r9...r:...r
-00000c30: 0500 0000 da13 746f 5f70 796f 6d6f 5f63  ......to_pyomo_c
-00000c40: 6f6e 7374 7261 696e 74da 046e 616d 65da  onstraint..name.
-00000c50: 036f 626a 2909 7210 0000 0072 1100 0000  .obj).r....r....
-00000c60: 7212 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00000c70: 0b63 6f6e 7374 7261 696e 7473 5a0e 6f62  .constraintsZ.ob
-00000c80: 6a65 6374 6976 655f 7275 6c65 5a15 6f62  jective_ruleZ.ob
-00000c90: 6a65 6374 6976 655f 636f 6e73 7472 6169  jective_constrai
-00000ca0: 6e74 73da 0a63 6f6e 7374 7261 696e 7472  nts..constraintr
-00000cb0: 1900 0000 2902 722a 0000 0072 2900 0000  ....).r*...r)...
-00000cc0: 721d 0000 00da 1563 7265 6174 655f 6162  r......create_ab
-00000cd0: 7374 7261 6374 5f6d 6f64 656c 1c00 0000  stract_model....
-00000ce0: 7384 0000 0006 0704 0508 0308 0108 0108  s...............
-00000cf0: 0106 0108 010c 020a 070a 010a 010a 010a  ................
-00000d00: 010c 0206 040e 0110 0910 0308 0314 0108  ................
-00000d10: 0114 0108 0114 0108 0114 0108 0114 0104  ................
-00000d20: 0210 0308 0314 0108 0114 0108 0114 0102  ................
-00000d30: 020a 0104 ff08 0514 0108 0114 0102 020a  ................
-00000d40: 0104 ff10 0510 030a 0314 010a 0114 010a  ................
-00000d50: 0114 0110 020a 0312 010a 0112 0104 020a  ................
-00000d60: 0208 0618 0106 0204 0272 4a00 0000 2915  .........rJ...).
-00000d70: da07 5f5f 646f 635f 5fda 056e 756d 7079  ..__doc__..numpy
-00000d80: 7222 0000 00da 0d6d 696d 6f73 612e 636f  r".....mimosa.co
-00000d90: 6d6d 6f6e 7202 0000 0072 0300 0000 7204  mmonr....r....r.
-00000da0: 0000 0072 0500 0000 5a11 6d69 6d6f 7361  ...r....Z.mimosa
-00000db0: 2e63 6f6d 706f 6e65 6e74 7372 0600 0000  .componentsr....
-00000dc0: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-00000dd0: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
-00000de0: 0000 0072 0e00 0000 720f 0000 00da 0373  ...r....r......s
-00000df0: 7472 724a 0000 0072 1900 0000 7219 0000  trrJ...r....r...
-00000e00: 0072 1900 0000 721d 0000 00da 083c 6d6f  .r....r......<mo
-00000e10: 6475 6c65 3e01 0000 0073 2200 0000 0400  dule>....s".....
-00000e20: 0806 1801 3001 0213 0201 02ff 0202 02fe  ....0...........
-00000e30: 0203 02fd 0204 02fc 0205 02fb 0206 0efa  ................
+00000170: da09 656d 6973 7369 6f6e 73da 0d65 6d69  ..emissions..emi
+00000180: 7373 696f 6e74 7261 6465 da11 6669 6e61  ssiontrade..fina
+00000190: 6e63 6961 6c74 7261 6e73 6665 72da 0b63  ncialtransfer..c
+000001a0: 6f62 6264 6f75 676c 6173 da07 6461 6d61  obbdouglas..dama
+000001b0: 6765 73da 0a6d 6974 6967 6174 696f 6eda  ges..mitigation.
+000001c0: 096f 626a 6563 7469 7665 da0c 7365 616c  .objective..seal
+000001d0: 6576 656c 7269 7365 da07 7765 6c66 6172  evelrise..welfar
+000001e0: 65da 0d64 616d 6167 655f 6d6f 6475 6c65  e..damage_module
+000001f0: da14 656d 6973 7369 6f6e 7472 6164 655f  ..emissiontrade_
+00000200: 6d6f 6475 6c65 da18 6669 6e61 6e63 6961  module..financia
+00000210: 6c74 7261 6e73 6665 725f 6d6f 6475 6c65  ltransfer_module
+00000220: da0e 7765 6c66 6172 655f 6d6f 6475 6c65  ..welfare_module
+00000230: da10 6f62 6a65 6374 6976 655f 6d6f 6475  ..objective_modu
+00000240: 6c65 da06 7265 7475 726e 6305 0000 0000  le..returnc.....
+00000250: 0000 0000 0000 0009 0000 0006 0000 0003  ................
+00000260: 0000 0073 fc02 0000 7400 8300 8901 6700  ...s....t.....g.
+00000270: 7d05 7401 8300 8801 5f02 7401 8300 8801  }.t....._.t.....
+00000280: 5f03 7401 8300 8801 5f04 7405 8300 8801  _.t....._.t.....
+00000290: 5f06 6400 8801 5f07 7401 8300 8801 5f08  _.d..._.t....._.
+000002a0: 7405 6401 6402 8d01 8801 5f09 6403 6404  t.d.d....._.d.d.
+000002b0: 8400 8801 5f0a 6405 6404 8400 8801 5f0b  ...._.d.d....._.
+000002c0: 6406 6404 8400 8801 5f0c 6407 6404 8400  d.d....._.d.d...
+000002d0: 8801 5f0d 6408 6404 8400 8801 5f0e 8701  .._.d.d....._...
+000002e0: 6601 6409 640a 8408 8900 8800 8801 5f0f  f.d.d........._.
+000002f0: 8700 6601 640b 6404 8408 8801 5f10 7c05  ..f.d.d....._.|.
+00000300: a011 7412 a013 8801 a101 a101 0100 7c05  ..t...........|.
+00000310: a011 7414 a013 8801 a101 a101 0100 7c00  ..t...........|.
+00000320: 640c 6b02 7269 7c05 a011 7415 6a16 a013  d.k.ri|...t.j...
+00000330: 8801 a101 a101 0100 6e3a 7c00 640d 6b02  ........n:|.d.k.
+00000340: 7277 7c05 a011 7415 6a17 a013 8801 a101  rw|...t.j.......
+00000350: a101 0100 6e2c 7c00 640e 6b02 7285 7c05  ....n,|.d.k.r.|.
+00000360: a011 7415 6a18 a013 8801 a101 a101 0100  ..t.j...........
+00000370: 6e1e 7c00 640f 6b02 7293 7c05 a011 7415  n.|.d.k.r.|...t.
+00000380: 6a19 a013 8801 a101 a101 0100 6e10 7c00  j...........n.|.
+00000390: 6410 6b02 72a1 7c05 a011 7415 6a1a a013  d.k.r.|...t.j...
+000003a0: 8801 a101 a101 0100 6e02 741b 8201 7c05  ........n.t...|.
+000003b0: a011 741c a013 8801 a101 a101 0100 7c01  ..t...........|.
+000003c0: 6411 6b02 72b9 7c05 a011 741d 6a1e a013  d.k.r.|...t.j...
+000003d0: 8801 a101 a101 0100 6e24 7c01 6412 6b02  ........n$|.d.k.
+000003e0: 72c7 7c05 a011 741d 6a1f a013 8801 a101  r.|...t.j.......
+000003f0: a101 0100 6e16 7c01 6413 6b02 72d5 7c05  ....n.|.d.k.r.|.
+00000400: a011 741d 6a1d a013 8801 a101 a101 0100  ..t.j...........
+00000410: 6e08 741b 6414 7c01 9b00 6415 9d03 8301  n.t.d.|...d.....
+00000420: 8201 7c02 6416 6b02 72eb 7c05 a011 7420  ..|.d.k.r.|...t 
+00000430: 6a21 a013 8801 a101 a101 0100 6e16 7c02  j!..........n.|.
+00000440: 6417 6b02 72f9 7c05 a011 7420 6a22 a013  d.k.r.|...t j"..
+00000450: 8801 a101 a101 0100 6e08 741b 6418 7c02  ........n.t.d.|.
+00000460: 9b00 6415 9d03 8301 8201 7c05 a011 7423  ..d.......|...t#
+00000470: a013 8801 a101 a101 0100 7c05 a011 7424  ..........|...t$
+00000480: a013 8801 a101 a101 0100 7c03 6419 6b02  ..........|.d.k.
+00000490: 9001 7220 7c05 a011 7425 6a26 a013 8801  ..r |...t%j&....
+000004a0: a101 a101 0100 6e26 7c03 641a 6b02 9001  ......n&|.d.k...
+000004b0: 722f 7c05 a011 7425 6a27 a013 8801 a101  r/|...t%j'......
+000004c0: a101 0100 6e17 7c03 641b 6b02 9001 723e  ....n.|.d.k...r>
+000004d0: 7c05 a011 7425 6a28 a013 8801 a101 a101  |...t%j(........
+000004e0: 0100 6e08 741b 641c 7c03 9b00 6415 9d03  ..n.t.d.|...d...
+000004f0: 8301 8201 7c04 641d 6b02 9001 7254 7429  ....|.d.k...rTt)
+00000500: 6a2a a013 8801 a101 5c02 7d06 7d07 6e10  j*......\.}.}.n.
+00000510: 7c04 641e 6b02 9001 7262 7429 6a2b a013  |.d.k...rbt)j+..
+00000520: 8801 a101 5c02 7d06 7d07 6e02 741b 8201  ....\.}.}.n.t...
+00000530: 7c05 a011 7c07 a101 0100 7c05 4400 5d0d  |...|.....|.D.].
+00000540: 7d08 742c 8801 7c08 a02d 8801 a101 7c08  }.t,..|..-....|.
+00000550: 6a2e 8303 0100 9001 716b 7c06 8801 5f2f  j.......qk|..._/
+00000560: 8801 5300 291f 4e54 2901 da07 6f72 6465  ..S.).NT)...orde
+00000570: 7265 6463 0200 0000 0000 0000 0000 0000  redc............
+00000580: 0200 0000 0100 0000 5300 0000 f304 0000  ........S.......
+00000590: 0064 0053 00a9 014e a900 a902 da04 7965  .d.S...N......ye
+000005a0: 6172 da06 7265 6769 6f6e 7219 0000 0072  ar..regionr....r
+000005b0: 1900 0000 fa5a 633a 5c55 7365 7273 5c33  .....Zc:\Users\3
+000005c0: 3930 3338 3835 5c4f 6e65 4472 6976 6520  903885\OneDrive 
+000005d0: 2d20 556e 6976 6572 7369 7465 6974 2055  - Universiteit U
+000005e0: 7472 6563 6874 5c44 6f63 756d 656e 7473  trecht\Documents
+000005f0: 5c4d 494d 4f53 415c 6d69 6d6f 7361 5c61  \MIMOSA\mimosa\a
+00000600: 6273 7472 6163 745f 6d6f 6465 6c2e 7079  bstract_model.py
+00000610: da08 3c6c 616d 6264 613e 3900 0000 f302  ..<lambda>9.....
+00000620: 0000 0004 007a 2763 7265 6174 655f 6162  .....z'create_ab
+00000630: 7374 7261 6374 5f6d 6f64 656c 2e3c 6c6f  stract_model.<lo
+00000640: 6361 6c73 3e2e 3c6c 616d 6264 613e 6302  cals>.<lambda>c.
+00000650: 0000 0000 0000 0000 0000 0002 0000 0001  ................
+00000660: 0000 0053 0000 0072 1700 0000 7218 0000  ...S...r....r...
+00000670: 0072 1900 0000 721a 0000 0072 1900 0000  .r....r....r....
+00000680: 7219 0000 0072 1d00 0000 721e 0000 003a  r....r....r....:
+00000690: 0000 0072 1f00 0000 6302 0000 0000 0000  ...r....c.......
+000006a0: 0000 0000 0002 0000 0001 0000 0053 0000  .............S..
+000006b0: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
+000006c0: 721a 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+000006d0: 1d00 0000 721e 0000 003b 0000 0072 1f00  ....r....;...r..
+000006e0: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+000006f0: 0000 0001 0000 0053 0000 0072 1700 0000  .......S...r....
+00000700: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00000710: 1900 0000 7219 0000 0072 1d00 0000 721e  ....r....r....r.
+00000720: 0000 003c 0000 0072 1f00 0000 6302 0000  ...<...r....c...
+00000730: 0000 0000 0000 0000 0002 0000 0001 0000  ................
+00000740: 0053 0000 0072 1700 0000 7218 0000 0072  .S...r....r....r
+00000750: 1900 0000 721a 0000 0072 1900 0000 7219  ....r....r....r.
+00000760: 0000 0072 1d00 0000 721e 0000 003d 0000  ...r....r....=..
+00000770: 0072 1f00 0000 6303 0000 0000 0000 0000  .r....c.........
+00000780: 0000 0004 0000 0005 0000 0013 0000 0073  ...............s
+00000790: 2400 0000 7400 a001 7c00 7c01 6401 a103  $...t...|.|.d...
+000007a0: 7d03 7400 6a02 8800 a003 7c03 7c02 a102  }.t.j.....|.|...
+000007b0: 7c03 6402 8d02 5300 2903 4ee9 6400 0000  |.d...S.).N.d...
+000007c0: 2901 da01 7829 04da 026e 70da 086c 696e  )...x)...np..lin
+000007d0: 7370 6163 65da 0574 7261 707a da12 6261  space..trapz..ba
+000007e0: 7365 6c69 6e65 5f65 6d69 7373 696f 6e73  seline_emissions
+000007f0: 2904 da0a 7965 6172 5f73 7461 7274 da08  )...year_start..
+00000800: 7965 6172 5f65 6e64 721c 0000 00da 0579  year_endr......y
+00000810: 6561 7273 2901 da01 6d72 1900 0000 721d  ears)...mr....r.
+00000820: 0000 00da 1362 6173 656c 696e 655f 6375  .....baseline_cu
+00000830: 6d75 6c61 7469 7665 3f00 0000 7304 0000  mulative?...s...
+00000840: 000e 0116 017a 3263 7265 6174 655f 6162  .....z2create_ab
+00000850: 7374 7261 6374 5f6d 6f64 656c 2e3c 6c6f  stract_model.<lo
+00000860: 6361 6c73 3e2e 6261 7365 6c69 6e65 5f63  cals>.baseline_c
+00000870: 756d 756c 6174 6976 6563 0300 0000 0000  umulativec......
+00000880: 0000 0000 0000 0300 0000 0400 0000 1300  ................
+00000890: 0000 731c 0000 0074 0087 0287 0087 0166  ..s....t.......f
+000008a0: 0364 0164 0284 087c 006a 0144 0083 0183  .d.d...|.j.D....
+000008b0: 0153 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
+000008c0: 0000 0002 0000 0005 0000 0033 0000 0073  ...........3...s
+000008d0: 1c00 0000 8100 7c00 5d09 7d01 8800 8802  ......|.].}.....
+000008e0: 8801 7c01 8303 5600 0100 7102 6400 5300  ..|...V...q.d.S.
+000008f0: 7218 0000 0072 1900 0000 2902 da02 2e30  r....r....)....0
+00000900: da01 7229 0372 2a00 0000 7227 0000 0072  ..r).r*...r'...r
+00000910: 2600 0000 7219 0000 0072 1d00 0000 da09  &...r....r......
+00000920: 3c67 656e 6578 7072 3e44 0000 0073 0800  <genexpr>D...s..
+00000930: 0000 0280 0400 0c01 0aff 7a3a 6372 6561  ..........z:crea
+00000940: 7465 5f61 6273 7472 6163 745f 6d6f 6465  te_abstract_mode
+00000950: 6c2e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  l.<locals>.<lamb
+00000960: 6461 3e2e 3c6c 6f63 616c 733e 2e3c 6765  da>.<locals>.<ge
+00000970: 6e65 7870 723e 2902 da03 7375 6dda 0772  nexpr>)...sum..r
+00000980: 6567 696f 6e73 2903 7229 0000 0072 2600  egions).r)...r&.
+00000990: 0000 7227 0000 0029 0172 2a00 0000 2902  ..r'...).r*...).
+000009a0: 7227 0000 0072 2600 0000 721d 0000 0072  r'...r&...r....r
+000009b0: 1e00 0000 4400 0000 7306 0000 0010 0004  ....D...s.......
+000009c0: 0108 ff5a 0852 4943 4532 3031 305a 0557  ...Z.RICE2010Z.W
+000009d0: 4954 4348 5a08 5249 4345 3230 3132 da06  ITCHZ.RICE2012..
+000009e0: 434f 4143 4348 da08 6e6f 6461 6d61 6765  COACCH..nodamage
+000009f0: da07 6e6f 7472 6164 65da 0e67 6c6f 6261  ..notrade..globa
+00000a00: 6c63 6f73 7470 6f6f 6c72 0800 0000 7a19  lcostpoolr....z.
+00000a10: 456d 6973 7369 6f6e 2074 7261 6469 6e67  Emission trading
+00000a20: 206d 6f64 756c 6520 607a 1160 206e 6f74   module `z.` not
+00000a30: 2069 6d70 6c65 6d65 6e74 6564 da0a 6e6f   implemented..no
+00000a40: 7472 616e 7366 6572 da10 676c 6f62 616c  transfer..global
+00000a50: 6461 6d61 6765 706f 6f6c 7a1b 4669 6e61  damagepoolz.Fina
+00000a60: 6e63 6961 6c20 7472 616e 7366 6572 206d  ncial transfer m
+00000a70: 6f64 756c 6520 60da 1777 656c 6661 7265  odule `..welfare
+00000a80: 5f6c 6f73 735f 6d69 6e69 6d69 7369 6e67  _loss_minimising
+00000a90: da0f 636f 7374 5f6d 696e 696d 6973 696e  ..cost_minimisin
+00000aa0: 67da 1869 6e65 7175 616c 5f61 7665 7273  g..inequal_avers
+00000ab0: 696f 6e5f 6765 6e65 7261 6c7a 1057 656c  ion_generalz.Wel
+00000ac0: 6661 7265 206d 6f64 756c 6520 60da 0775  fare module `..u
+00000ad0: 7469 6c69 7479 da0b 676c 6f62 616c 636f  tility..globalco
+00000ae0: 7374 7329 3072 0300 0000 7202 0000 00da  sts)0r....r.....
+00000af0: 0962 6567 696e 7965 6172 da02 6474 da02  .beginyear..dt..
+00000b00: 7466 7204 0000 00da 0174 721b 0000 005a  tfr......tr....Z
+00000b10: 0879 6561 7232 3130 3072 2f00 0000 7225  .year2100r/...r%
+00000b20: 0000 00da 0a70 6f70 756c 6174 696f 6eda  .....population.
+00000b30: 0354 4650 da03 4744 50da 1063 6172 626f  .TFP..GDP..carbo
+00000b40: 6e5f 696e 7465 6e73 6974 7972 2a00 0000  n_intensityr*...
+00000b50: 5a1a 6261 7365 6c69 6e65 5f63 756d 756c  Z.baseline_cumul
+00000b60: 6174 6976 655f 676c 6f62 616c da06 6578  ative_global..ex
+00000b70: 7465 6e64 7207 0000 005a 0f67 6574 5f63  tendr....Z.get_c
+00000b80: 6f6e 7374 7261 696e 7473 720e 0000 0072  onstraintsr....r
+00000b90: 0b00 0000 5a0b 6164 5f72 6963 6532 3031  ....Z.ad_rice201
+00000ba0: 305a 0861 645f 7769 7463 685a 0b61 645f  0Z.ad_witchZ.ad_
+00000bb0: 7269 6365 3230 3132 5a06 636f 6163 6368  rice2012Z.coacch
+00000bc0: 7231 0000 00da 134e 6f74 496d 706c 656d  r1.....NotImplem
+00000bd0: 656e 7465 6445 7272 6f72 720c 0000 0072  entedErrorr....r
+00000be0: 0800 0000 7232 0000 0072 3300 0000 7209  ....r2...r3...r.
+00000bf0: 0000 0072 3400 0000 7235 0000 0072 0600  ...r4...r5...r..
+00000c00: 0000 720a 0000 0072 0f00 0000 7236 0000  ..r....r....r6..
+00000c10: 0072 3700 0000 7238 0000 0072 0d00 0000  .r7...r8...r....
+00000c20: 7239 0000 0072 3a00 0000 7205 0000 00da  r9...r:...r.....
+00000c30: 1374 6f5f 7079 6f6d 6f5f 636f 6e73 7472  .to_pyomo_constr
+00000c40: 6169 6e74 da04 6e61 6d65 da03 6f62 6a29  aint..name..obj)
+00000c50: 0972 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000c60: 7213 0000 0072 1400 0000 da0b 636f 6e73  r....r......cons
+00000c70: 7472 6169 6e74 735a 0e6f 626a 6563 7469  traintsZ.objecti
+00000c80: 7665 5f72 756c 655a 156f 626a 6563 7469  ve_ruleZ.objecti
+00000c90: 7665 5f63 6f6e 7374 7261 696e 7473 da0a  ve_constraints..
+00000ca0: 636f 6e73 7472 6169 6e74 7219 0000 0029  constraintr....)
+00000cb0: 0272 2a00 0000 7229 0000 0072 1d00 0000  .r*...r)...r....
+00000cc0: da15 6372 6561 7465 5f61 6273 7472 6163  ..create_abstrac
+00000cd0: 745f 6d6f 6465 6c1c 0000 0073 8400 0000  t_model....s....
+00000ce0: 0607 0405 0803 0801 0801 0801 0601 0801  ................
+00000cf0: 0c02 0a07 0a01 0a01 0a01 0a01 0c02 0604  ................
+00000d00: 0e01 1009 1003 0803 1401 0801 1401 0801  ................
+00000d10: 1401 0801 1401 0801 1401 0402 1003 0803  ................
+00000d20: 1401 0801 1401 0801 1401 0202 0a01 04ff  ................
+00000d30: 0805 1401 0801 1401 0202 0a01 04ff 1005  ................
+00000d40: 1003 0a03 1401 0a01 1401 0a01 1401 1002  ................
+00000d50: 0a03 1201 0a01 1201 0402 0a02 0806 1801  ................
+00000d60: 0602 0402 724a 0000 0029 15da 075f 5f64  ....rJ...)...__d
+00000d70: 6f63 5f5f da05 6e75 6d70 7972 2200 0000  oc__..numpyr"...
+00000d80: da0d 6d69 6d6f 7361 2e63 6f6d 6d6f 6e72  ..mimosa.commonr
+00000d90: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
+00000da0: 0000 005a 116d 696d 6f73 612e 636f 6d70  ...Z.mimosa.comp
+00000db0: 6f6e 656e 7473 7206 0000 0072 0700 0000  onentsr....r....
+00000dc0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000dd0: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
+00000de0: 0000 0072 0f00 0000 da03 7374 7272 4a00  ...r......strrJ.
+00000df0: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
+00000e00: 0072 1d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000e10: 0100 0000 7322 0000 0004 0008 0618 0130  ....s".........0
+00000e20: 0102 1302 0102 ff02 0202 fe02 0302 fd02  ................
+00000e30: 0402 fc02 0502 fb02 060e fa              ...........
```

### Comparing `mimosa-0.1.3/mimosa/__pycache__/mimosa.cpython-310.pyc` & `mimosa-0.1.4/mimosa/__pycache__/mimosa.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:41 2023 UTC, .py size: 8217 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b536 ba64 1920 0000  o........6.d. ..
+00000000: 6f0d 0d0a 0000 0000 72b3 bb64 1920 0000  o.......r..d. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0f 5a0f 0100 6401 6404 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
@@ -111,19 +111,19 @@
 000006e0: 0072 1800 0000 da12 6765 745f 6162 7374  .r......get_abst
 000006f0: 7261 6374 5f6d 6f64 656c da0e 6162 7374  ract_model..abst
 00000700: 7261 6374 5f6d 6f64 656c da0f 6372 6561  ract_model..crea
 00000710: 7465 5f69 6e73 7461 6e63 65da 0e63 6f6e  te_instance..con
 00000720: 6372 6574 655f 6d6f 6465 6cda 0d70 7265  crete_model..pre
 00000730: 7072 6f63 6573 7369 6e67 2902 da04 7365  processing)...se
 00000740: 6c66 7217 0000 00a9 0072 1f00 0000 fa52  lfr......r.....R
-00000750: 633a 5c75 7365 7273 5c33 3930 3338 3835  c:\users\3903885
-00000760: 5c6f 6e65 6472 6976 6520 2d20 756e 6976  \onedrive - univ
-00000770: 6572 7369 7465 6974 2075 7472 6563 6874  ersiteit utrecht
-00000780: 5c64 6f63 756d 656e 7473 5c6d 696d 6f73  \documents\mimos
-00000790: 615c 6d69 6d6f 7361 5c6d 696d 6f73 612e  a\mimosa\mimosa.
+00000750: 633a 5c55 7365 7273 5c33 3930 3338 3835  c:\Users\3903885
+00000760: 5c4f 6e65 4472 6976 6520 2d20 556e 6976  \OneDrive - Univ
+00000770: 6572 7369 7465 6974 2055 7472 6563 6874  ersiteit Utrecht
+00000780: 5c44 6f63 756d 656e 7473 5c4d 494d 4f53  \Documents\MIMOS
+00000790: 415c 6d69 6d6f 7361 5c6d 696d 6f73 612e  A\mimosa\mimosa.
 000007a0: 7079 da08 5f5f 696e 6974 5f5f 3300 0000  py..__init__3...
 000007b0: 730c 0000 0008 0206 010a 010a 020a 010c  s...............
 000007c0: 017a 0f4d 494d 4f53 412e 5f5f 696e 6974  .z.MIMOSA.__init
 000007d0: 5f5f da06 7265 7475 726e 6301 0000 0000  __..returnc.....
 000007e0: 0000 0000 0000 0006 0000 0006 0000 0043  ...............C
 000007f0: 0000 0073 5600 0000 7c00 6a00 6401 1900  ...sV...|.j.d...
 00000800: 6402 1900 7d01 7c00 6a00 6401 1900 6403  d...}.|.j.d...d.
@@ -134,15 +134,15 @@
 00000850: 7a74 0a20 2020 2020 2020 2052 6574 7572  zt.        Retur
 00000860: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
 00000870: 4162 7374 7261 6374 4d6f 6465 6c3a 206d  AbstractModel: m
 00000880: 6f64 656c 2063 6f72 7265 7370 6f6e 6469  odel correspondi
 00000890: 6e67 2074 6f20 7468 6520 6461 6d61 6765  ng to the damage
 000008a0: 2f6f 626a 6563 7469 7665 206d 6f64 756c  /objective modul
 000008b0: 6520 636f 6d62 696e 6174 696f 6e0a 2020  e combination.  
-000008c0: 2020 2020 2020 5a05 6d6f 6465 6c7a 0d64        Z.modelz.d
+000008c0: 2020 2020 2020 da05 6d6f 6465 6c7a 0d64        ..modelz.d
 000008d0: 616d 6167 6520 6d6f 6475 6c65 7a14 656d  amage modulez.em
 000008e0: 6973 7369 6f6e 7472 6164 6520 6d6f 6475  issiontrade modu
 000008f0: 6c65 7a18 6669 6e61 6e63 6961 6c74 7261  lez.financialtra
 00000900: 6e73 6665 7220 6d6f 6475 6c65 7a0e 7765  nsfer modulez.we
 00000910: 6c66 6172 6520 6d6f 6475 6c65 7a10 6f62  lfare modulez.ob
 00000920: 6a65 6374 6976 6520 6d6f 6475 6c65 2902  jective module).
 00000930: 7217 0000 0072 1300 0000 2906 721e 0000  r....r....).r...
@@ -182,16 +182,16 @@
 00000b50: 6f6e 6372 6574 654d 6f64 656c 0a0a 2020  oncreteModel..  
 00000b60: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
 00000b70: 2020 2020 2020 2020 2020 2043 6f6e 6372             Concr
 00000b80: 6574 654d 6f64 656c 3a20 6d6f 6465 6c20  eteModel: model 
 00000b90: 696e 7374 616e 7469 6174 6564 2077 6974  instantiated wit
 00000ba0: 6820 7061 7261 6d65 7465 7220 7661 6c75  h parameter valu
 00000bb0: 6573 2061 6e64 2064 6174 6120 6675 6e63  es and data func
-00000bc0: 7469 6f6e 730a 2020 2020 2020 2020 5a0a  tions.        Z.
-00000bd0: 7369 6d75 6c61 7469 6f6e 4e5a 0e73 696d  simulationNZ.sim
+00000bc0: 7469 6f6e 730a 2020 2020 2020 2020 da0a  tions.        ..
+00000bd0: 7369 6d75 6c61 7469 6f6e 4eda 0e73 696d  simulationN..sim
 00000be0: 756c 6174 696f 6e6d 6f64 6529 0d72 0b00  ulationmode).r..
 00000bf0: 0000 5a12 5265 6769 6f6e 616c 5061 7261  ..Z.RegionalPara
 00000c00: 6d53 746f 7265 7217 0000 005a 1472 6567  mStorer....Z.reg
 00000c10: 696f 6e61 6c5f 7061 7261 6d5f 7374 6f72  ional_param_stor
 00000c20: 6572 0a00 0000 5a09 4461 7461 5374 6f72  er....Z.DataStor
 00000c30: 655a 0a64 6174 615f 7374 6f72 6572 1400  eZ.data_storer..
 00000c40: 0000 721a 0000 0072 1c00 0000 da03 6765  ..r....r......ge
@@ -255,19 +255,19 @@
 00000fe0: 0000 0073 2600 0000 7400 7c00 6a01 8301  ...s&...t.|.j...
 00000ff0: 6401 6b04 7211 7402 6402 8301 a003 7c00  d.k.r.t.d.....|.
 00001000: 6a04 a101 0100 6403 5300 6403 5300 2904  j.....d.S.d.S.).
 00001010: 7a4b 506f 7374 2d70 726f 6365 7373 696e  zKPost-processin
 00001020: 6720 7461 736b 7320 746f 2072 6573 746f  g tasks to resto
 00001030: 7265 2061 6767 7265 6761 7465 2076 6172  re aggregate var
 00001040: 6961 626c 6573 2069 6e20 7072 652d 7072  iables in pre-pr
-00001050: 6f63 6573 7369 6e67 2073 7465 7072 2500  ocessing stepr%.
-00001060: 0000 7226 0000 004e 2905 7227 0000 0072  ..r&...N).r'...r
+00001050: 6f63 6573 7369 6e67 2073 7465 7072 2800  ocessing stepr(.
+00001060: 0000 7229 0000 004e 2905 722a 0000 0072  ..r)...N).r*...r
 00001070: 1800 0000 7204 0000 005a 1075 7064 6174  ....r....Z.updat
 00001080: 655f 7661 7269 6162 6c65 7372 1c00 0000  e_variablesr....
-00001090: 7228 0000 0072 1f00 0000 721f 0000 0072  r(...r....r....r
+00001090: 722b 0000 0072 1f00 0000 721f 0000 0072  r+...r....r....r
 000010a0: 2000 0000 da0e 706f 7374 7072 6f63 6573   .....postproces
 000010b0: 7369 6e67 8800 0000 730a 0000 000e 0208  sing....s.......
 000010c0: 0104 0108 ff04 ff7a 154d 494d 4f53 412e  .......z.MIMOSA.
 000010d0: 706f 7374 7072 6f63 6573 7369 6e67 7a0b  postprocessingz.
 000010e0: 4d6f 6465 6c20 736f 6c76 6554 da02 6e6f  Model solveT..no
 000010f0: 4663 0600 0000 0000 0000 0000 0000 0a00  Fc..............
 00001100: 0000 0700 0000 4300 0000 73f0 0000 007c  ......C...s....|
@@ -340,29 +340,29 @@
 00001530: 636f 6e64 6974 696f 6e3a 207b 7d7a 2253  condition: {}z"S
 00001540: 6f6c 7665 7220 6469 6420 6e6f 7420 6578  olver did not ex
 00001550: 6974 2077 6974 6820 7374 6174 7573 204f  it with status O
 00001560: 4b7a 0d46 696e 616c 204e 5056 3a20 7b7d  Kz.Final NPV: {}
 00001570: 2917 da02 6f73 da07 656e 7669 726f 6e72  )...os..environr
 00001580: 0600 0000 da05 736f 6c76 6572 1c00 0000  ......solver....
 00001590: 7205 0000 005a 076f 7074 696f 6e73 7211  r....Z.optionsr.
-000015a0: 0000 0072 2900 0000 720e 0000 00da 0469  ...r)...r......i
+000015a0: 0000 0072 2c00 0000 720e 0000 00da 0469  ...r,...r......i
 000015b0: 6e66 6fda 0666 6f72 6d61 74da 0673 6f6c  nfo..format..sol
 000015c0: 7665 725a 0673 7461 7475 7372 0700 0000  verZ.statusr....
 000015d0: 5a02 6f6b da05 6572 726f 725a 1574 6572  Z.ok..errorZ.ter
 000015e0: 6d69 6e61 7469 6f6e 5f63 6f6e 6469 7469  mination_conditi
 000015f0: 6f6e 5a07 7761 726e 696e 67da 0f53 6f6c  onZ.warning..Sol
 00001600: 7665 7245 7863 6570 7469 6f6e 7208 0000  verExceptionr...
 00001610: 005a 034e 5056 5a02 7466 290a 721e 0000  .Z.NPVZ.tf).r...
-00001620: 00da 0776 6572 626f 7365 722c 0000 005a  ...verboser,...Z
+00001620: 00da 0776 6572 626f 7365 722f 0000 005a  ...verboser/...Z
 00001630: 0875 7365 5f6e 656f 735a 0a6e 656f 735f  .use_neosZ.neos_
 00001640: 656d 6169 6c5a 1169 706f 7074 5f6f 7574  emailZ.ipopt_out
 00001650: 7075 745f 6669 6c65 5a0e 736f 6c76 6572  put_fileZ.solver
-00001660: 5f6d 616e 6167 6572 7233 0000 005a 0772  _managerr3...Z.r
-00001670: 6573 756c 7473 722b 0000 0072 1f00 0000  esultsr+...r....
-00001680: 721f 0000 0072 2000 0000 7230 0000 008f  r....r ...r0....
+00001660: 5f6d 616e 6167 6572 7236 0000 005a 0772  _managerr6...Z.r
+00001670: 6573 756c 7473 722e 0000 0072 1f00 0000  esultsr....r....
+00001680: 721f 0000 0072 2000 0000 7233 0000 008f  r....r ...r3....
 00001690: 0000 0073 3a00 0000 0416 0a03 0801 0401  ...s:...........
 000016a0: 1201 0803 0a01 0802 0a01 0401 0801 06ff  ................
 000016b0: 0803 0801 0802 1402 0e02 0401 0401 0c01  ................
 000016c0: 02ff 04ff 0e05 0801 0402 0401 1201 02ff  ................
 000016d0: 08ff 7a0c 4d49 4d4f 5341 2e73 6f6c 7665  ..z.MIMOSA.solve
 000016e0: 7a10 506c 6f74 7469 6e67 2072 6573 756c  z.Plotting resul
 000016f0: 7473 da06 7265 7375 6c74 6302 0000 0000  ts..resultc.....
@@ -374,46 +374,46 @@
 00001750: da06 6b77 6172 6773 721f 0000 0072 1f00  ..kwargsr....r..
 00001760: 0000 7220 0000 00da 0470 6c6f 74cc 0000  ..r .....plot...
 00001770: 0073 0200 0000 1802 7a0b 4d49 4d4f 5341  .s......z.MIMOSA
 00001780: 2e70 6c6f 7463 0200 0000 0000 0000 0000  .plotc..........
 00001790: 0000 0300 0000 0400 0000 4b00 0000 731c  ..........K...s.
 000017a0: 0000 0074 007c 006a 017c 006a 027c 0166  ...t.|.j.|.j.|.f
 000017b0: 0369 007c 02a4 018e 0101 0064 0053 0072  .i.|.......d.S.r
-000017c0: 3800 0000 2903 7212 0000 0072 1700 0000  8...).r....r....
+000017c0: 3b00 0000 2903 7212 0000 0072 1700 0000  ;...).r....r....
 000017d0: 721c 0000 0029 0372 1e00 0000 5a0a 6578  r....).r....Z.ex
-000017e0: 7065 7269 6d65 6e74 723a 0000 0072 1f00  perimentr:...r..
+000017e0: 7065 7269 6d65 6e74 723d 0000 0072 1f00  perimentr=...r..
 000017f0: 0000 721f 0000 0072 2000 0000 da04 7361  ..r....r .....sa
 00001800: 7665 d000 0000 7302 0000 001c 017a 0b4d  ve....s......z.M
 00001810: 494d 4f53 412e 7361 7665 2902 7222 0000  IMOSA.save).r"..
-00001820: 004e 2905 5472 2a00 0000 464e 4e29 0172  .N).Tr*...FNN).r
-00001830: 3700 0000 7238 0000 0029 11da 085f 5f6e  7...r8...)...__n
+00001820: 004e 2905 5472 2d00 0000 464e 4e29 0172  .N).Tr-...FNN).r
+00001830: 3a00 0000 723b 0000 0029 11da 085f 5f6e  :...r;...)...__n
 00001840: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
 00001850: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
 00001860: 075f 5f64 6f63 5f5f da04 6469 6374 7221  .__doc__..dictr!
 00001870: 0000 0072 0200 0000 7219 0000 0072 0c00  ...r....r....r..
 00001880: 0000 5a05 7469 6d65 7272 0300 0000 721b  ..Z.timerr....r.
-00001890: 0000 0072 1d00 0000 7229 0000 0072 3000  ...r....r)...r0.
-000018a0: 0000 723b 0000 0072 3c00 0000 721f 0000  ..r;...r<...r...
+00001890: 0000 0072 1d00 0000 722c 0000 0072 3300  ...r....r,...r3.
+000018a0: 0000 723e 0000 0072 3f00 0000 721f 0000  ..r>...r?...r...
 000018b0: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
 000018c0: 7216 0000 0022 0000 0073 2800 0000 0800  r...."...s(.....
 000018d0: 0401 0e10 0e0a 0813 1001 0a20 0a17 0a07  ........... ....
 000018e0: 0203 0201 0201 0201 0201 02fa 0207 0cf9  ................
 000018f0: 083c 0c01 0e03 7216 0000 0063 0000 0000  .<....r....c....
 00001900: 0000 0000 0000 0000 0000 0000 0100 0000  ................
 00001910: 4000 0000 7310 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00001920: 0264 015a 0364 0253 0029 0372 3500 0000  .d.Z.d.S.).r5...
+00001920: 0264 015a 0364 0253 0029 0372 3800 0000  .d.Z.d.S.).r8...
 00001930: 7a35 5261 6973 6564 2077 6865 6e20 5079  z5Raised when Py
 00001940: 6f6d 6f20 736f 6c76 6572 2064 6f65 7320  omo solver does 
 00001950: 6e6f 7420 6578 6974 2077 6974 6820 7374  not exit with st
-00001960: 6174 7573 204f 4b4e 2904 723d 0000 0072  atus OKN).r=...r
-00001970: 3e00 0000 723f 0000 0072 4000 0000 721f  >...r?...r@...r.
+00001960: 6174 7573 204f 4b4e 2904 7240 0000 0072  atus OKN).r@...r
+00001970: 4100 0000 7242 0000 0072 4300 0000 721f  A...rB...rC...r.
 00001980: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
-00001990: 0000 7235 0000 00db 0000 0073 0400 0000  ..r5.......s....
-000019a0: 0800 0801 7235 0000 0029 1f72 4000 0000  ....r5...).r@...
-000019b0: 722e 0000 005a 0d6d 696d 6f73 612e 636f  r....Z.mimosa.co
+00001990: 0000 7238 0000 00db 0000 0073 0400 0000  ..r8.......s....
+000019a0: 0800 0801 7238 0000 0029 1f72 4300 0000  ....r8...).rC...
+000019b0: 7231 0000 005a 0d6d 696d 6f73 612e 636f  r1...Z.mimosa.co
 000019c0: 6d6d 6f6e 7202 0000 0072 0300 0000 7204  mmonr....r....r.
 000019d0: 0000 0072 0500 0000 7206 0000 0072 0700  ...r....r....r..
 000019e0: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
 000019f0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
 00001a00: 720e 0000 005a 206d 696d 6f73 612e 636f  r....Z mimosa.co
 00001a10: 6d6d 6f6e 2e63 6f6e 6669 672e 7061 7273  mmon.config.pars
 00001a20: 6563 6f6e 6669 6772 0f00 0000 5a0d 6d69  econfigr....Z.mi
@@ -422,12 +422,12 @@
 00001a50: 7361 2e61 6273 7472 6163 745f 6d6f 6465  sa.abstract_mode
 00001a60: 6c72 1300 0000 5a28 6d69 6d6f 7361 2e63  lr....Z(mimosa.c
 00001a70: 6f6e 6372 6574 655f 6d6f 6465 6c2e 696e  oncrete_model.in
 00001a80: 7374 616e 7469 6174 655f 7061 7261 6d73  stantiate_params
 00001a90: 7214 0000 005a 156d 696d 6f73 612e 636f  r....Z.mimosa.co
 00001aa0: 6e63 7265 7465 5f6d 6f64 656c 7215 0000  ncrete_modelr...
 00001ab0: 0072 1600 0000 da09 4578 6365 7074 696f  .r......Exceptio
-00001ac0: 6e72 3500 0000 721f 0000 0072 1f00 0000  nr5...r....r....
+00001ac0: 6e72 3800 0000 721f 0000 0072 1f00 0000  nr8...r....r....
 00001ad0: 721f 0000 0072 2000 0000 da08 3c6d 6f64  r....r .....<mod
 00001ae0: 756c 653e 0100 0000 7316 0000 0004 0008  ule>....s.......
 00001af0: 093c 020c 0f14 010c 010c 010c 010e 0300  .<..............
 00001b00: 7f14 3a                                  ..:
```

### Comparing `mimosa-0.1.3/mimosa/abstract_model.py` & `mimosa-0.1.4/mimosa/abstract_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 """
 
 import numpy as np
 from mimosa.common import Param, AbstractModel, Set, add_constraint
 from mimosa.components import (
     burdensharing,
     emissions,
-    abatement,
     emissiontrade,
     financialtransfer,
     cobbdouglas,
     damages,
+    mitigation,
     objective,
     sealevelrise,
     welfare,
 )
 
 
 ######################
@@ -90,15 +90,15 @@
         constraints.extend(damages.coacch.get_constraints(m))
     elif damage_module == "nodamage":
         constraints.extend(damages.nodamage.get_constraints(m))
     else:
         raise NotImplementedError
 
     # Abatement costs
-    constraints.extend(abatement.get_constraints(m))
+    constraints.extend(mitigation.get_constraints(m))
 
     # Emission trading
     if emissiontrade_module == "notrade":
         constraints.extend(emissiontrade.notrade.get_constraints(m))
     elif emissiontrade_module == "globalcostpool":
         constraints.extend(emissiontrade.globalcostpool.get_constraints(m))
     elif emissiontrade_module == "emissiontrade":
@@ -121,18 +121,18 @@
     # Burden sharing regime
     constraints.extend(burdensharing.get_constraints(m))
 
     # Cobb-Douglas and economics
     constraints.extend(cobbdouglas.get_constraints(m))
 
     # Utility and welfare
-    if welfare_module == "inequal_aversion_elasmu":
-        constraints.extend(welfare.inequal_aversion_elasmu.get_constraints(m))
-    elif welfare_module == "inequal_aversion_zero":
-        constraints.extend(welfare.inequal_aversion_zero.get_constraints(m))
+    if welfare_module == "welfare_loss_minimising":
+        constraints.extend(welfare.welfare_loss_minimising.get_constraints(m))
+    elif welfare_module == "cost_minimising":
+        constraints.extend(welfare.cost_minimising.get_constraints(m))
     elif welfare_module == "inequal_aversion_general":
         constraints.extend(welfare.inequal_aversion_general.get_constraints(m))
     else:
         raise NotImplementedError(f"Welfare module `{welfare_module}` not implemented")
 
     # Objective of optimisation
     if objective_module == "utility":
```

### Comparing `mimosa-0.1.3/mimosa/common/__init__.py` & `mimosa-0.1.4/mimosa/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/__pycache__/__init__.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 06:54:00 2023 UTC, .py size: 1206 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 882b ba64 b604 0000  o........+.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 b604 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 6403  Z.d.d.l.Z.e...d.
 00000040: a101 5a03 6401 6404 6c04 6d05 5a05 0100  ..Z.d.d.l.m.Z...
 00000050: 6401 6405 6c06 6d07 5a07 6d08 5a08 6d09  d.d.l.m.Z.m.Z.m.
 00000060: 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11  Z.m.Z.m.Z.m.Z.m.
@@ -71,16 +71,16 @@
 00000460: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
 00000470: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
 00000480: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
 00000490: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
 000004a0: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
 000004b0: 0000 da05 7574 696c 7372 2b00 0000 722c  ....utilsr+...r,
 000004c0: 0000 00a9 0072 3100 0000 7231 0000 00fa  .....r1...r1....
-000004d0: 5b63 3a5c 7573 6572 735c 3339 3033 3838  [c:\users\390388
-000004e0: 355c 6f6e 6564 7269 7665 202d 2075 6e69  5\onedrive - uni
-000004f0: 7665 7273 6974 6569 7420 7574 7265 6368  versiteit utrech
-00000500: 745c 646f 6375 6d65 6e74 735c 6d69 6d6f  t\documents\mimo
-00000510: 7361 5c6d 696d 6f73 615c 636f 6d6d 6f6e  sa\mimosa\common
+000004d0: 5b63 3a5c 5573 6572 735c 3339 3033 3838  [c:\Users\390388
+000004e0: 355c 4f6e 6544 7269 7665 202d 2055 6e69  5\OneDrive - Uni
+000004f0: 7665 7273 6974 6569 7420 5574 7265 6368  versiteit Utrech
+00000500: 745c 446f 6375 6d65 6e74 735c 4d49 4d4f  t\Documents\MIMO
+00000510: 5341 5c6d 696d 6f73 615c 636f 6d6d 6f6e  SA\mimosa\common
 00000520: 5c5f 5f69 6e69 745f 5f2e 7079 da08 3c6d  \__init__.py..<m
 00000530: 6f64 756c 653e 0100 0000 7312 0000 0004  odule>....s.....
 00000540: 0008 050a 020c 0354 030c 1550 030c 1610  .......T...P....
 00000550: 02                                       .
```

### Comparing `mimosa-0.1.3/mimosa/common/__pycache__/economics.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/__pycache__/economics.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:43 2023 UTC, .py size: 1419 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b736 ba64 8b05 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 8b05 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6506 6406 6504 6604 6407 6408  ..d.e.d.e.f.d.d.
 00000060: 8404 5a07 6409 640a 8400 5a08 640b 640c  ..Z.d.d...Z.d.d.
 00000070: 8400 5a09 6402 5300 290d 7a38 0a55 7469  ..Z.d.S.).z8.Uti
@@ -47,18 +47,18 @@
 000002e0: 7372 0400 0000 720a 0000 005a 0374 6670  sr....r....Z.tfp
 000002f0: da02 6474 7209 0000 005a 0864 6570 725f  ..dtr....Z.depr_
 00000300: 6361 705a 0c73 6176 696e 6773 5f72 6174  capZ.savings_rat
 00000310: 655a 0867 6470 5f64 6174 615a 0f70 6f70  eZ.gdp_dataZ.pop
 00000320: 756c 6174 696f 6e5f 6461 7461 5a07 6361  ulation_dataZ.ca
 00000330: 7069 7461 6cda 0367 6470 da03 706f 705a  pital..gdp..popZ
 00000340: 0464 4b64 74a9 0072 1800 0000 fa5c 633a  .dKdt..r.....\c:
-00000350: 5c75 7365 7273 5c33 3930 3338 3835 5c6f  \users\3903885\o
-00000360: 6e65 6472 6976 6520 2d20 756e 6976 6572  nedrive - univer
-00000370: 7369 7465 6974 2075 7472 6563 6874 5c64  siteit utrecht\d
-00000380: 6f63 756d 656e 7473 5c6d 696d 6f73 615c  ocuments\mimosa\
+00000350: 5c55 7365 7273 5c33 3930 3338 3835 5c4f  \Users\3903885\O
+00000360: 6e65 4472 6976 6520 2d20 556e 6976 6572  neDrive - Univer
+00000370: 7369 7465 6974 2055 7472 6563 6874 5c44  siteit Utrecht\D
+00000380: 6f63 756d 656e 7473 5c4d 494d 4f53 415c  ocuments\MIMOSA\
 00000390: 6d69 6d6f 7361 5c63 6f6d 6d6f 6e5c 6563  mimosa\common\ec
 000003a0: 6f6e 6f6d 6963 732e 7079 da07 6765 745f  onomics.py..get_
 000003b0: 5446 500a 0000 0073 2200 0000 0607 0402  TFP....s".......
 000003c0: 1001 1003 1001 1001 0803 0801 0c04 0801  ................
 000003d0: 02ff 02ff 1605 1801 1201 0e01 1202 721a  ..............r.
 000003e0: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
 000003f0: 0400 0000 0200 0000 4300 0000 731c 0000  ........C...s...
```

### Comparing `mimosa-0.1.3/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:43 2023 UTC, .py size: 8234 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b736 ba64 2a20 0000  o........6.d* ..
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 2a20 0000  o........i.d* ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5601 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a06 6400 6403 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6404 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6401 6c09 5a0c 6508 6a0d 6508  ..d.d.l.Z.e.j.e.
@@ -35,19 +35,19 @@
 00000220: a006 7c00 a101 5300 a902 4e29 05da 0653  ..|...S...N)...S
 00000230: 6572 6965 73da 0944 6174 6146 7261 6d65  eries..DataFrame
 00000240: da05 666c 6f61 74da 0369 6e74 da07 6e64  ..float..int..nd
 00000250: 6172 7261 7929 07da 0474 7970 65da 085f  array)...type.._
 00000260: 5f6e 616d 655f 5fda 026e 70da 0661 7263  _name__..np..arc
 00000270: 7461 6eda 0570 796f 6d6f da07 656e 7669  tan..pyomo..envi
 00000280: 726f 6e72 0700 0000 a902 da01 78da 046e  ronr........x..n
-00000290: 616d 65a9 0072 1800 0000 fa5e 633a 5c75  ame..r.....^c:\u
-000002a0: 7365 7273 5c33 3930 3338 3835 5c6f 6e65  sers\3903885\one
-000002b0: 6472 6976 6520 2d20 756e 6976 6572 7369  drive - universi
-000002c0: 7465 6974 2075 7472 6563 6874 5c64 6f63  teit utrecht\doc
-000002d0: 756d 656e 7473 5c6d 696d 6f73 615c 6d69  uments\mimosa\mi
+00000290: 616d 65a9 0072 1800 0000 fa5e 633a 5c55  ame..r.....^c:\U
+000002a0: 7365 7273 5c33 3930 3338 3835 5c4f 6e65  sers\3903885\One
+000002b0: 4472 6976 6520 2d20 556e 6976 6572 7369  Drive - Universi
+000002c0: 7465 6974 2055 7472 6563 6874 5c44 6f63  teit Utrecht\Doc
+000002d0: 756d 656e 7473 5c4d 494d 4f53 415c 6d69  uments\MIMOSA\mi
 000002e0: 6d6f 7361 5c63 6f6d 6d6f 6e5c 7079 6f6d  mosa\common\pyom
 000002f0: 6f5f 7574 696c 732e 7079 7207 0000 0016  o_utils.pyr.....
 00000300: 0000 00f3 0800 0000 0a01 0801 0a01 0c02  ................
 00000310: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 00000320: 0003 0000 0043 0000 0073 2800 0000 7400  .....C...s(...t.
 00000330: 7c00 8301 6a01 7d01 7c01 6401 7600 720e  |...j.}.|.d.v.r.
 00000340: 7402 a003 7c00 a101 5300 7404 6a05 a003  t...|...S.t.j...
```

### Comparing `mimosa-0.1.3/mimosa/common/__pycache__/units.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/__pycache__/units.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:42:29 2023 UTC, .py size: 3579 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e536 ba64 fb0d 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 fb0d 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 6404 6405 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6504 a007 6501 6a08 a009 6501 6a08  ..e...e.j...e.j.
 00000060: a00a 650b a101 6406 6407 a103 a101 0100  ..e...d.d.......
 00000070: 6506 6408 8301 5a0c 4700 6409 640a 8400  e.d...Z.G.d.d...
@@ -45,19 +45,19 @@
 000002c0: da0d 4445 4641 554c 545f 554e 4954 53da  ..DEFAULT_UNITS.
 000002d0: 0d64 6566 6175 6c74 5f75 6e69 7473 da0b  .default_units..
 000002e0: 7079 6f6d 6f5f 756e 6974 73da 0d70 696e  pyomo_units..pin
 000002f0: 745f 7265 6769 7374 7279 da0e 5f70 696e  t_registry.._pin
 00000300: 745f 7265 6769 7374 7279 da16 5f70 796f  t_registry.._pyo
 00000310: 6d6f 5f75 6e69 7473 5f63 6f6e 7461 696e  mo_units_contain
 00000320: 6572 2901 da04 7365 6c66 a900 720e 0000  er)...self..r...
-00000330: 00fa 5863 3a5c 7573 6572 735c 3339 3033  ..Xc:\users\3903
-00000340: 3838 355c 6f6e 6564 7269 7665 202d 2075  885\onedrive - u
-00000350: 6e69 7665 7273 6974 6569 7420 7574 7265  niversiteit utre
-00000360: 6368 745c 646f 6375 6d65 6e74 735c 6d69  cht\documents\mi
-00000370: 6d6f 7361 5c6d 696d 6f73 615c 636f 6d6d  mosa\mimosa\comm
+00000330: 00fa 5863 3a5c 5573 6572 735c 3339 3033  ..Xc:\Users\3903
+00000340: 3838 355c 4f6e 6544 7269 7665 202d 2055  885\OneDrive - U
+00000350: 6e69 7665 7273 6974 6569 7420 5574 7265  niversiteit Utre
+00000360: 6368 745c 446f 6375 6d65 6e74 735c 4d49  cht\Documents\MI
+00000370: 4d4f 5341 5c6d 696d 6f73 615c 636f 6d6d  MOSA\mimosa\comm
 00000380: 6f6e 5c75 6e69 7473 2e70 79da 085f 5f69  on\units.py..__i
 00000390: 6e69 745f 5f1c 0000 0073 0600 0000 0601  nit__....s......
 000003a0: 0801 0a01 7a11 5175 616e 7469 7479 2e5f  ....z.Quantity._
 000003b0: 5f69 6e69 745f 5f54 2902 da0e 6f6e 6c79  _init__T)...only
 000003c0: 5f6d 6167 6e69 7475 6465 da0c 6361 6e5f  _magnitude..can_
 000003d0: 6265 5f66 616c 7365 6301 0000 0000 0000  be_falsec.......
 000003e0: 0002 0000 0009 0000 0006 0000 0047 0000  .............G..
```

### Comparing `mimosa-0.1.3/mimosa/common/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:42:29 2023 UTC, .py size: 1220 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e536 ba64 c404 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 c404 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6404 6405 8400 5a06 6406  m.Z...d.d...Z.d.
 00000060: 6407 8400 5a07 640d 6409 640a 8401 5a08  d...Z.d.d.d...Z.
 00000070: 640b 640c 8400 5a09 6402 5300 290e 7a20  d.d...Z.d.S.).z 
@@ -13,19 +13,19 @@
 000000c0: 0003 0000 0043 0000 0073 1400 0000 7400  .....C...s....t.
 000000d0: 7c00 a001 a100 8301 7d01 7c01 6401 1900  |.......}.|.d...
 000000e0: 5300 2902 7a25 5265 7475 726e 7320 7468  S.).z%Returns th
 000000f0: 6520 6669 7273 7420 6b65 7920 6f66 2061  e first key of a
 00000100: 2064 6963 7469 6f6e 6172 7972 0100 0000   dictionaryr....
 00000110: 2902 da04 6c69 7374 da04 6b65 7973 2902  )...list..keys).
 00000120: da0a 6469 6374 696f 6e61 7279 7204 0000  ..dictionaryr...
-00000130: 00a9 0072 0600 0000 fa58 633a 5c75 7365  ...r.....Xc:\use
-00000140: 7273 5c33 3930 3338 3835 5c6f 6e65 6472  rs\3903885\onedr
-00000150: 6976 6520 2d20 756e 6976 6572 7369 7465  ive - universite
-00000160: 6974 2075 7472 6563 6874 5c64 6f63 756d  it utrecht\docum
-00000170: 656e 7473 5c6d 696d 6f73 615c 6d69 6d6f  ents\mimosa\mimo
+00000130: 00a9 0072 0600 0000 fa58 633a 5c55 7365  ...r.....Xc:\Use
+00000140: 7273 5c33 3930 3338 3835 5c4f 6e65 4472  rs\3903885\OneDr
+00000150: 6976 6520 2d20 556e 6976 6572 7369 7465  ive - Universite
+00000160: 6974 2055 7472 6563 6874 5c44 6f63 756d  it Utrecht\Docum
+00000170: 656e 7473 5c4d 494d 4f53 415c 6d69 6d6f  ents\MIMOSA\mimo
 00000180: 7361 5c63 6f6d 6d6f 6e5c 7574 696c 732e  sa\common\utils.
 00000190: 7079 da06 6669 7273 746b 0b00 0000 7304  py..firstk....s.
 000001a0: 0000 000c 0208 0172 0800 0000 6301 0000  .......r....c...
 000001b0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
 000001c0: 0043 0000 0073 0c00 0000 7c00 7400 7c00  .C...s....|.t.|.
 000001d0: 8301 1900 5300 2901 7a31 5265 7475 726e  ....S.).z1Return
 000001e0: 7320 7468 6520 6669 7273 7420 656c 656d  s the first elem
```

### Comparing `mimosa-0.1.3/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:54:34 2023 UTC, .py size: 2429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ba39 ba64 7d09 0000  o........9.d}...
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 7d09 0000  o........i.d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6404 6405 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6411 6407 6408 8401 5a0a 6409 640a  ..d.d.d...Z.d.d.
 00000070: 8400 5a0b 640b 640c 8400 5a0c 6412 640e  ..Z.d.d...Z.d.d.
@@ -39,19 +39,19 @@
 00000260: 7206 0000 00da 0367 6574 2906 5a09 6375  r......get).Z.cu
 00000270: 7272 5f6b 6579 73da 0673 7562 7365 74da  rr_keys..subset.
 00000280: 036b 6579 da04 6e6f 6465 da04 6b65 7973  .key..node..keys
 00000290: da06 7061 7273 6572 a904 da13 5f72 6563  ..parser...._rec
 000002a0: 7572 7369 7665 5f74 7261 7665 7273 655a  ursive_traverseZ
 000002b0: 0b70 6172 7365 645f 6469 6374 da0b 7061  .parsed_dict..pa
 000002c0: 7273 6572 5f74 7265 65da 0975 7365 725f  rser_tree..user_
-000002d0: 7961 6d6c a900 fa65 633a 5c75 7365 7273  yaml...ec:\users
-000002e0: 5c33 3930 3338 3835 5c6f 6e65 6472 6976  \3903885\onedriv
-000002f0: 6520 2d20 756e 6976 6572 7369 7465 6974  e - universiteit
-00000300: 2075 7472 6563 6874 5c64 6f63 756d 656e   utrecht\documen
-00000310: 7473 5c6d 696d 6f73 615c 6d69 6d6f 7361  ts\mimosa\mimosa
+000002d0: 7961 6d6c a900 fa65 633a 5c55 7365 7273  yaml...ec:\Users
+000002e0: 5c33 3930 3338 3835 5c4f 6e65 4472 6976  \3903885\OneDriv
+000002f0: 6520 2d20 556e 6976 6572 7369 7465 6974  e - Universiteit
+00000300: 2055 7472 6563 6874 5c44 6f63 756d 656e   Utrecht\Documen
+00000310: 7473 5c4d 494d 4f53 415c 6d69 6d6f 7361  ts\MIMOSA\mimosa
 00000320: 5c63 6f6d 6d6f 6e5c 636f 6e66 6967 5c70  \common\config\p
 00000330: 6172 7365 636f 6e66 6967 2e70 7972 1600  arseconfig.pyr..
 00000340: 0000 1000 0000 7310 0000 0010 010e 0112  ......s.........
 00000350: 010c 010c 020c 0316 0304 f57a 2970 6172  ...........z)par
 00000360: 7365 5f70 6172 616d 732e 3c6c 6f63 616c  se_params.<local
 00000370: 733e 2e5f 7265 6375 7273 6976 655f 7472  s>._recursive_tr
 00000380: 6176 6572 7365 7219 0000 0029 03da 0c64  averser....)...d
```

### Comparing `mimosa-0.1.3/mimosa/common/config/parseconfig.py` & `mimosa-0.1.4/mimosa/common/config/parseconfig.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 06:54:00 2023 UTC, .py size: 969 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-00000000: 6f0d 0d0a 0000 0000 882b ba64 c903 0000  o........+.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 c903 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2000 0000 6408  .....@...s ...d.
 00000030: 6401 6402 8401 5a00 6403 6404 8400 5a01  d.d...Z.d.d...Z.
 00000040: 6409 6406 6407 8401 5a02 6405 5300 290a  d.d.d...Z.d.S.).
 00000050: 4663 0300 0000 0000 0000 0000 0000 0400  Fc..............
 00000060: 0000 0400 0000 4300 0000 732a 0000 007c  ......C...s*...|
 00000070: 0144 005d 107d 037c 037c 0076 0172 0e7c  .D.].}.|.|.v.r.|
 00000080: 0272 0e69 007c 007c 033c 007c 007c 0319  .r.i.|.|.<.|.|..
 00000090: 007d 0071 027c 0053 00a9 014e a900 2904  .}.q.|.S...N..).
 000000a0: da0a 6469 6374 696f 6e61 7279 da04 6b65  ..dictionary..ke
 000000b0: 7973 da06 6372 6561 7465 da03 6b65 7972  ys..create..keyr
-000000c0: 0200 0000 7202 0000 00fa 6b63 3a5c 7573  ....r.....kc:\us
-000000d0: 6572 735c 3339 3033 3838 355c 6f6e 6564  ers\3903885\oned
-000000e0: 7269 7665 202d 2075 6e69 7665 7273 6974  rive - universit
-000000f0: 6569 7420 7574 7265 6368 745c 646f 6375  eit utrecht\docu
-00000100: 6d65 6e74 735c 6d69 6d6f 7361 5c6d 696d  ments\mimosa\mim
+000000c0: 0200 0000 7202 0000 00fa 6b63 3a5c 5573  ....r.....kc:\Us
+000000d0: 6572 735c 3339 3033 3838 355c 4f6e 6544  ers\3903885\OneD
+000000e0: 7269 7665 202d 2055 6e69 7665 7273 6974  rive - Universit
+000000f0: 6569 7420 5574 7265 6368 745c 446f 6375  eit Utrecht\Docu
+00000100: 6d65 6e74 735c 4d49 4d4f 5341 5c6d 696d  ments\MIMOSA\mim
 00000110: 6f73 615c 636f 6d6d 6f6e 5c63 6f6e 6669  osa\common\confi
 00000120: 675c 7574 696c 735c 6e65 7374 6564 5f64  g\utils\nested_d
 00000130: 6963 742e 7079 da0a 6765 745f 6e65 7374  ict.py..get_nest
 00000140: 6564 0100 0000 730a 0000 0008 010c 0108  ed....s.........
 00000150: 010a 0104 0172 0800 0000 6303 0000 0000  .....r....c.....
 00000160: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
 00000170: 0000 0073 2400 0000 7400 7c00 7c01 6400  ...s$...t.|.|.d.
```

### Comparing `mimosa-0.1.3/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:43 2023 UTC, .py size: 8454 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b736 ba64 0621 0000  o........6.d.!..
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 0621 0000  o........i.d.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 0100 6401 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6406 6407 6c0e 6d0f 5a0f 0100 4700  ..d.d.l.m.Z...G.
@@ -84,19 +84,19 @@
 00000530: 636f 6e74 6169 6e20 6120 7479 7065 3a20  contain a type: 
 00000540: da05 6465 7363 72da 00da 0764 6566 6175  ..descr....defau
 00000550: 6c74 da0c 6361 6e5f 6265 5f66 616c 7365  lt..can_be_false
 00000560: 4629 0672 0e00 0000 da08 4b65 7945 7272  F).r......KeyErr
 00000570: 6f72 da03 6765 7472 0f00 0000 7211 0000  or..getr....r...
 00000580: 0072 1200 0000 a904 da04 7365 6c66 720d  .r........selfr.
 00000590: 0000 00da 0461 7267 73da 066b 7761 7267  .....args..kwarg
-000005a0: 73a9 0072 1900 0000 fa67 633a 5c75 7365  s..r.....gc:\use
-000005b0: 7273 5c33 3930 3338 3835 5c6f 6e65 6472  rs\3903885\onedr
-000005c0: 6976 6520 2d20 756e 6976 6572 7369 7465  ive - universite
-000005d0: 6974 2075 7472 6563 6874 5c64 6f63 756d  it utrecht\docum
-000005e0: 656e 7473 5c6d 696d 6f73 615c 6d69 6d6f  ents\mimosa\mimo
+000005a0: 73a9 0072 1900 0000 fa67 633a 5c55 7365  s..r.....gc:\Use
+000005b0: 7273 5c33 3930 3338 3835 5c4f 6e65 4472  rs\3903885\OneDr
+000005c0: 6976 6520 2d20 556e 6976 6572 7369 7465  ive - Universite
+000005d0: 6974 2055 7472 6563 6874 5c44 6f63 756d  it Utrecht\Docum
+000005e0: 656e 7473 5c4d 494d 4f53 415c 6d69 6d6f  ents\MIMOSA\mimo
 000005f0: 7361 5c63 6f6d 6d6f 6e5c 636f 6e66 6967  sa\common\config
 00000600: 5c75 7469 6c73 5c70 6172 7365 7273 2e70  \utils\parsers.p
 00000610: 79da 085f 5f69 6e69 745f 5f23 0000 0073  y..__init__#...s
 00000620: 1000 0000 0201 0e01 0c01 0e01 02ff 0e03  ................
 00000630: 0e01 1201 7a16 4765 6e65 7261 6c50 6172  ....z.GeneralPar
 00000640: 7365 722e 5f5f 696e 6974 5f5f 6302 0000  ser.__init__c...
 00000650: 0000 0000 0000 0000 0002 0000 000c 0000  ................
```

### Comparing `mimosa-0.1.3/mimosa/common/config/utils/nested_dict.py` & `mimosa-0.1.4/mimosa/common/config/utils/nested_dict.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/config/utils/parsers.py` & `mimosa-0.1.4/mimosa/common/config/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/data/__pycache__/datastore.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/data/__pycache__/datastore.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:42:30 2023 UTC, .py size: 6574 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e636 ba64 ae19 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 ae19 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6402 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a06 6401 6402 6c07 5a08 6401 6404 6c09  Z.d.d.l.Z.d.d.l.
 00000060: 6d0a 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 6d0d 5a0d 0100 6406 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -69,61 +69,61 @@
 00000440: a100 0100 8804 a002 a100 0100 8804 a003  ................
 00000450: 6401 6402 a102 8900 8804 a003 6403 6404  d.d.........d.d.
 00000460: a102 8902 8804 a003 6405 6406 a102 8901  ........d.d.....
 00000470: 8800 8802 8801 8700 8701 6602 6407 6408  ..........f.d.d.
 00000480: 8408 7c01 6409 1900 4400 8301 8701 8702  ..|.d...D.......
 00000490: 8703 8704 6604 640a 6408 8408 7c01 6409  ....f.d.d...|.d.
 000004a0: 1900 4400 8301 640b 9c05 8804 5f04 6400  ..D...d....._.d.
-000004b0: 5300 290c 4e5a 0965 6d69 7373 696f 6e73  S.).NZ.emissions
+000004b0: 5300 290c 4eda 0965 6d69 7373 696f 6e73  S.).N..emissions
 000004c0: 5a12 656d 6973 7369 6f6e 7372 6174 655f  Z.emissionsrate_
 000004d0: 756e 6974 da0a 706f 7075 6c61 7469 6f6e  unit..population
 000004e0: 5a0f 706f 7075 6c61 7469 6f6e 5f75 6e69  Z.population_uni
 000004f0: 74da 0347 4450 5a0d 6375 7272 656e 6379  t..GDPZ.currency
 00000500: 5f75 6e69 7463 0100 0000 0000 0000 0000  _unitc..........
 00000510: 0000 0200 0000 0800 0000 1300 0000 732e  ..............s.
 00000520: 0000 0069 007c 005d 137d 017c 0174 0088  ...i.|.].}.|.t..
 00000530: 007c 0119 006a 0188 007c 0119 006a 0288  .|...j...|...j..
 00000540: 017c 0119 006a 021b 0083 0293 0271 0253  .|...j.......q.S
 00000550: 00a9 0029 0372 0800 0000 da07 7876 616c  ...).r......xval
 00000560: 7565 73da 0779 7661 6c75 6573 a902 da02  ues..yvalues....
 00000570: 2e30 da01 7229 02da 0862 6173 656c 696e  .0..r)...baselin
-00000580: 65da 0367 6470 720d 0000 00fa 6163 3a5c  e..gdpr.....ac:\
-00000590: 7573 6572 735c 3339 3033 3838 355c 6f6e  users\3903885\on
-000005a0: 6564 7269 7665 202d 2075 6e69 7665 7273  edrive - univers
-000005b0: 6974 6569 7420 7574 7265 6368 745c 646f  iteit utrecht\do
-000005c0: 6375 6d65 6e74 735c 6d69 6d6f 7361 5c6d  cuments\mimosa\m
+00000580: 65da 0367 6470 720e 0000 00fa 6163 3a5c  e..gdpr.....ac:\
+00000590: 5573 6572 735c 3339 3033 3838 355c 4f6e  Users\3903885\On
+000005a0: 6544 7269 7665 202d 2055 6e69 7665 7273  eDrive - Univers
+000005b0: 6974 6569 7420 5574 7265 6368 745c 446f  iteit Utrecht\Do
+000005c0: 6375 6d65 6e74 735c 4d49 4d4f 5341 5c6d  cuments\MIMOSA\m
 000005d0: 696d 6f73 615c 636f 6d6d 6f6e 5c64 6174  imosa\common\dat
 000005e0: 615c 6461 7461 7374 6f72 652e 7079 da0a  a\datastore.py..
 000005f0: 3c64 6963 7463 6f6d 703e 2e00 0000 7308  <dictcomp>....s.
 00000600: 0000 0006 0002 0220 ff06 ff7a 2644 6174  ....... ...z&Dat
 00000610: 6153 746f 7265 2e5f 5f69 6e69 745f 5f2e  aStore.__init__.
 00000620: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
 00000630: 6d70 3eda 0772 6567 696f 6e73 6301 0000  mp>..regionsc...
 00000640: 0000 0000 0000 0000 0002 0000 000a 0000  ................
 00000650: 0013 0000 0073 2200 0000 6900 7c00 5d0d  .....s"...i.|.].
 00000660: 7d01 7c01 7400 a001 7c01 8803 6a02 8800  }.|.t...|...j...
-00000670: 8801 8802 a105 9302 7102 5300 720d 0000  ........q.S.r...
+00000670: 8801 8802 a105 9302 7102 5300 720e 0000  ........q.S.r...
 00000680: 0029 0372 0500 0000 5a07 6765 745f 5446  .).r....Z.get_TF
-00000690: 50da 0a64 6174 615f 7965 6172 7372 1000  P..data_yearsr..
-000006a0: 0000 2904 7214 0000 0072 0b00 0000 da14  ..).r....r......
+00000690: 50da 0a64 6174 615f 7965 6172 7372 1100  P..data_yearsr..
+000006a0: 0000 2904 7215 0000 0072 0c00 0000 da14  ..).r....r......
 000006b0: 7265 6769 6f6e 616c 5f70 6172 616d 5f73  regional_param_s
-000006c0: 746f 7265 da04 7365 6c66 720d 0000 0072  tore..selfr....r
-000006d0: 1500 0000 7216 0000 0032 0000 0073 0c00  ....r....2...s..
+000006c0: 746f 7265 da04 7365 6c66 720e 0000 0072  tore..selfr....r
+000006d0: 1600 0000 7217 0000 0032 0000 0073 0c00  ....r....2...s..
 000006e0: 0000 0600 0204 06fd 0c01 02ff 06ff 2905  ..............).
-000006f0: 7213 0000 0072 0b00 0000 720c 0000 005a  r....r....r....Z
+000006f0: 7214 0000 0072 0c00 0000 720d 0000 005a  r....r....r....Z
 00000700: 1063 6172 626f 6e5f 696e 7465 6e73 6974  .carbon_intensit
 00000710: 795a 0354 4650 2905 da06 7061 7261 6d73  yZ.TFP)...params
 00000720: da10 5f73 656c 6563 745f 6461 7461 6261  .._select_databa
 00000730: 7365 da12 5f63 7265 6174 655f 6461 7461  se.._create_data
 00000740: 5f79 6561 7273 da13 5f63 7265 6174 655f  _years.._create_
 00000750: 6461 7461 5f76 616c 7565 73da 0c5f 6461  data_values.._da
-00000760: 7461 5f76 616c 7565 7329 0372 1a00 0000  ta_values).r....
-00000770: 721b 0000 0072 1900 0000 720d 0000 0029  r....r....r....)
-00000780: 0572 1300 0000 7214 0000 0072 0b00 0000  .r....r....r....
-00000790: 7219 0000 0072 1a00 0000 7215 0000 00da  r....r....r.....
+00000760: 7461 5f76 616c 7565 7329 0372 1b00 0000  ta_values).r....
+00000770: 721c 0000 0072 1a00 0000 720e 0000 0029  r....r....r....)
+00000780: 0572 1400 0000 7215 0000 0072 0c00 0000  .r....r....r....
+00000790: 721a 0000 0072 1b00 0000 7216 0000 00da  r....r....r.....
 000007a0: 085f 5f69 6e69 745f 5f22 0000 0073 2000  .__init__"...s .
 000007b0: 0000 0601 0801 0801 0c02 0c01 0c01 0202  ................
 000007c0: 0201 0201 0c01 0602 04fe 1004 0604 04fc  ................
 000007d0: 0cf8 7a12 4461 7461 5374 6f72 652e 5f5f  ..z.DataStore.__
 000007e0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
 000007f0: 0000 0003 0000 0006 0000 0043 0000 0073  ...........C...s
 00000800: 7a00 0000 7400 6a01 a002 7400 6a01 a003  z...t.j...t.j...
@@ -137,87 +137,87 @@
 00000880: 7a3a 4d61 6b65 7320 7375 7265 2074 6865  z:Makes sure the
 00000890: 2066 696c 6520 646f 6573 6e27 7420 6e65   file doesn't ne
 000008a0: 6564 2074 6f20 6265 2072 6561 6420 6d75  ed to be read mu
 000008b0: 6c74 6970 6c65 2074 696d 6573 7a06 2e2e  ltiple timesz...
 000008c0: 2f2e 2e2f da05 696e 7075 745a 0b64 625f  /../..inputZ.db_
 000008d0: 6669 6c65 6e61 6d65 4e29 11da 026f 73da  filenameN)...os.
 000008e0: 0470 6174 68da 046a 6f69 6eda 0764 6972  .path..join..dir
-000008f0: 6e61 6d65 da08 5f5f 6669 6c65 5f5f 721b  name..__file__r.
+000008f0: 6e61 6d65 da08 5f5f 6669 6c65 5f5f 721c  name..__file__r.
 00000900: 0000 0072 0a00 0000 da09 6461 7461 6261  ...r......databa
 00000910: 7365 73da 0270 645a 0872 6561 645f 6373  ses..pdZ.read_cs
 00000920: 76da 0763 6f6c 756d 6e73 da03 7374 72da  v..columns..str.
 00000930: 056c 6f77 6572 da0b 6361 6368 6564 5f64  .lower..cached_d
 00000940: 6174 61da 0864 6174 6162 6173 65da 0563  ata..database..c
 00000950: 6163 6865 da08 6669 6c65 6e61 6d65 2903  ache..filename).
-00000960: 721a 0000 0072 2f00 0000 722d 0000 0072  r....r/...r-...r
-00000970: 0d00 0000 720d 0000 0072 1500 0000 721c  ....r....r....r.
+00000960: 721b 0000 0072 3000 0000 722e 0000 0072  r....r0...r....r
+00000970: 0e00 0000 720e 0000 0072 1600 0000 721d  ....r....r....r.
 00000980: 0000 003a 0000 0073 1a00 0000 0602 0a01  ...:...s........
 00000990: 0201 0c01 04fd 0a05 0a01 0e01 0a01 0a01  ................
 000009a0: 0c02 0c01 0a01 7a1a 4461 7461 5374 6f72  ......z.DataStor
 000009b0: 652e 5f73 656c 6563 745f 6461 7461 6261  e._select_databa
 000009c0: 7365 6301 0000 0000 0000 0000 0000 0004  sec.............
 000009d0: 0000 0005 0000 0043 0000 0073 4200 0000  .......C...sB...
 000009e0: 7c00 6a00 6401 1900 6402 1900 7d01 7c00  |.j.d...d...}.|.
 000009f0: 6a00 6401 1900 6403 1900 6404 1700 7d02  j.d...d...d...}.
 00000a00: 7c00 6a00 6401 1900 6405 1900 7d03 7401  |.j.d...d...}.t.
 00000a10: a002 7c01 7c02 7c03 a103 7c00 5f03 6400  ..|.|.|...|._.d.
 00000a20: 5300 2906 4eda 0474 696d 65da 0573 7461  S.).N..time..sta
 00000a30: 7274 da03 656e 64e9 3200 0000 da02 6474  rt..end.2.....dt
-00000a40: 2904 721b 0000 00da 026e 70da 0661 7261  ).r......np..ara
-00000a50: 6e67 6572 1800 0000 2904 721a 0000 005a  nger....).r....Z
+00000a40: 2904 721c 0000 00da 026e 70da 0661 7261  ).r......np..ara
+00000a50: 6e67 6572 1900 0000 2904 721b 0000 005a  nger....).r....Z
 00000a60: 0962 6567 696e 7965 6172 5a07 656e 6479  .beginyearZ.endy
-00000a70: 6561 7272 3400 0000 720d 0000 0072 0d00  earr4...r....r..
-00000a80: 0000 7215 0000 0072 1d00 0000 4b00 0000  ..r....r....K...
+00000a70: 6561 7272 3500 0000 720e 0000 0072 0e00  earr5...r....r..
+00000a80: 0000 7216 0000 0072 1e00 0000 4b00 0000  ..r....r....K...
 00000a90: 7308 0000 000e 0112 010e 0114 017a 1c44  s............z.D
 00000aa0: 6174 6153 746f 7265 2e5f 6372 6561 7465  ataStore._create
 00000ab0: 5f64 6174 615f 7965 6172 734e da06 7265  _data_yearsN..re
 00000ac0: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
 00000ad0: 0004 0000 0003 0000 0003 0000 0073 2000  .............s .
 00000ae0: 0000 8800 6a00 6401 1900 7d03 8700 8701  ....j.d...}.....
 00000af0: 8702 6603 6402 6403 8408 7c03 4400 8301  ..f.d.d...|.D...
-00000b00: 5300 2904 4e72 1700 0000 6301 0000 0000  S.).Nr....c.....
+00000b00: 5300 2904 4e72 1800 0000 6301 0000 0000  S.).Nr....c.....
 00000b10: 0000 0000 0000 0002 0000 0009 0000 0013  ................
 00000b20: 0000 0073 2000 0000 6900 7c00 5d0c 7d01  ...s ...i.|.].}.
 00000b30: 7c01 8800 a000 8800 6a01 7c01 8802 8801  |.......j.|.....
-00000b40: a104 9302 7102 5300 720d 0000 0029 02da  ....q.S.r....)..
-00000b50: 095f 6765 745f 6461 7461 7218 0000 0029  ._get_datar....)
-00000b60: 0272 1100 0000 da06 7265 6769 6f6e a903  .r......region..
-00000b70: 721a 0000 00da 0774 6f5f 756e 6974 da08  r......to_unit..
-00000b80: 7661 7269 6162 6c65 720d 0000 0072 1500  variabler....r..
-00000b90: 0000 7216 0000 0053 0000 0073 0800 0000  ..r....S...s....
+00000b40: a104 9302 7102 5300 720e 0000 0029 02da  ....q.S.r....)..
+00000b50: 095f 6765 745f 6461 7461 7219 0000 0029  ._get_datar....)
+00000b60: 0272 1200 0000 da06 7265 6769 6f6e a903  .r......region..
+00000b70: 721b 0000 00da 0774 6f5f 756e 6974 da08  r......to_unit..
+00000b80: 7661 7269 6162 6c65 720e 0000 0072 1600  variabler....r..
+00000b90: 0000 7217 0000 0053 0000 0073 0800 0000  ..r....S...s....
 00000ba0: 0600 0202 12ff 06ff 7a31 4461 7461 5374  ........z1DataSt
 00000bb0: 6f72 652e 5f63 7265 6174 655f 6461 7461  ore._create_data
 00000bc0: 5f76 616c 7565 732e 3c6c 6f63 616c 733e  _values.<locals>
-00000bd0: 2e3c 6469 6374 636f 6d70 3e29 0172 1b00  .<dictcomp>).r..
-00000be0: 0000 2904 721a 0000 0072 3c00 0000 723b  ..).r....r<...r;
-00000bf0: 0000 0072 1700 0000 720d 0000 0072 3a00  ...r....r....r:.
-00000c00: 0000 7215 0000 0072 1e00 0000 5100 0000  ..r....r....Q...
+00000bd0: 2e3c 6469 6374 636f 6d70 3e29 0172 1c00  .<dictcomp>).r..
+00000be0: 0000 2904 721b 0000 0072 3d00 0000 723c  ..).r....r=...r<
+00000bf0: 0000 0072 1800 0000 720e 0000 0072 3b00  ...r....r....r;.
+00000c00: 0000 7216 0000 0072 1f00 0000 5100 0000  ..r....r....Q...
 00000c10: 7308 0000 000a 010e 0102 0206 fe7a 1d44  s............z.D
 00000c20: 6174 6153 746f 7265 2e5f 6372 6561 7465  ataStore._create
 00000c30: 5f64 6174 615f 7661 6c75 6573 6303 0000  _data_valuesc...
 00000c40: 0000 0000 0000 0000 0008 0000 0006 0000  ................
 00000c50: 0043 0000 0073 6e00 0000 7c00 6a00 6401  .C...sn...|.j.d.
 00000c60: 1900 7d03 7c00 6a00 6402 1900 6403 1900  ..}.|.j.d...d...
 00000c70: 7c03 1900 6404 1900 7d04 7c00 6a00 6402  |...d...}.|.j.d.
 00000c80: 1900 6403 1900 7c03 1900 6405 1900 7d05  ..d...|...d...}.
 00000c90: 7c00 6a00 6402 1900 6406 1900 7c02 1900  |.j.d...d...|...
 00000ca0: 7d06 7c00 a001 7c04 7c05 7c01 7c06 a104  }.|...|.|.|.|...
 00000cb0: 7d07 7c07 6407 1900 7c07 6408 1900 7c07  }.|.d...|.d...|.
 00000cc0: 6409 1900 6603 5300 290a 4eda 0353 5350  d...f.S.).N..SSP
-00000cd0: 7221 0000 005a 0962 6173 656c 696e 6573  r!...Z.baselines
+00000cd0: 7222 0000 005a 0962 6173 656c 696e 6573  r"...Z.baselines
 00000ce0: da05 6d6f 6465 6cda 0873 6365 6e61 7269  ..model..scenari
 00000cf0: 6fda 0976 6172 6961 626c 6573 da05 7965  o..variables..ye
 00000d00: 6172 73da 0676 616c 7565 73da 0475 6e69  ars..values..uni
-00000d10: 7429 0272 1b00 0000 da1e 5f67 6574 5f63  t).r......_get_c
+00000d10: 7429 0272 1c00 0000 da1e 5f67 6574 5f63  t).r......_get_c
 00000d20: 6163 6865 645f 6461 7461 5f66 726f 6d5f  ached_data_from_
-00000d30: 6461 7461 6261 7365 2908 721a 0000 0072  database).r....r
-00000d40: 3900 0000 723c 0000 0072 3d00 0000 723e  9...r<...r=...r>
-00000d50: 0000 0072 3f00 0000 da0c 7661 7269 6162  ...r?.....variab
-00000d60: 6c65 6e61 6d65 722c 0000 0072 0d00 0000  lenamer,...r....
-00000d70: 720d 0000 0072 1500 0000 da17 5f67 6574  r....r......_get
+00000d30: 6461 7461 6261 7365 2908 721b 0000 0072  database).r....r
+00000d40: 3a00 0000 723d 0000 0072 3e00 0000 723f  :...r=...r>...r?
+00000d50: 0000 0072 4000 0000 da0c 7661 7269 6162  ...r@.....variab
+00000d60: 6c65 6e61 6d65 722d 0000 0072 0e00 0000  lenamer-...r....
+00000d70: 720e 0000 0072 1600 0000 da17 5f67 6574  r....r......_get
 00000d80: 5f64 6174 615f 6672 6f6d 5f64 6174 6162  _data_from_datab
 00000d90: 6173 6558 0000 0073 1000 0000 0a01 1601  aseX...s........
 00000da0: 1601 1201 0402 0801 04ff 1604 7a21 4461  ............z!Da
 00000db0: 7461 5374 6f72 652e 5f67 6574 5f64 6174  taStore._get_dat
 00000dc0: 615f 6672 6f6d 5f64 6174 6162 6173 6563  a_from_databasec
 00000dd0: 0500 0000 0000 0000 0000 0000 0800 0000  ................
 00000de0: 0800 0000 4300 0000 73ea 0000 007c 017c  ....C...s....|.|
@@ -231,32 +231,32 @@
 00000e60: 0372 4874 0464 08a0 0574 037c 0783 017c  .rHt.d...t.|...|
 00000e70: 017c 027c 037c 04a1 0583 0182 017c 076a  .|.|.|.......|.j
 00000e80: 0264 0064 0085 0264 0964 0085 0266 0219  .d.d...d.d...f..
 00000e90: 006a 066a 07a0 0874 09a1 017c 076a 0264  .j.j...t...|.j.d
 00000ea0: 0064 0085 0264 0964 0085 0266 0219 006a  .d...d.d...f...j
 00000eb0: 0764 0a19 007c 076a 0a64 0a19 0064 0b19  .d...|.j.d...d..
 00000ec0: 0064 0c9c 037c 006a 007c 053c 007c 006a  .d...|.j.|.<.|.j
-00000ed0: 007c 0519 0053 0029 0d4e 723e 0000 0072  .|...S.).Nr>...r
-00000ee0: 3f00 0000 7239 0000 00e9 ffff ffff fa01  ?...r9..........
-00000ef0: 2372 3c00 0000 7207 0000 007a 4046 6f75  #r<...r....z@Fou
+00000ed0: 007c 0519 0053 0029 0d4e 723f 0000 0072  .|...S.).Nr?...r
+00000ee0: 4000 0000 723a 0000 00e9 ffff ffff fa01  @...r:..........
+00000ef0: 2372 3d00 0000 7207 0000 007a 4046 6f75  #r=...r....z@Fou
 00000f00: 6e64 207b 7d20 726f 7773 206d 6174 6368  nd {} rows match
 00000f10: 696e 6720 6372 6974 6572 6961 2028 7b7d  ing criteria ({}
 00000f20: 2c20 7b7d 2c20 7b7d 2c20 7b7d 2920 696e  , {}, {}, {}) in
 00000f30: 7374 6561 6420 6f66 206f 6e65 2e5a 0432  stead of one.Z.2
-00000f40: 3031 3072 0100 0000 7243 0000 0029 0372  010r....rC...).r
-00000f50: 4100 0000 7242 0000 0072 4300 0000 290b  A...rB...rC...).
-00000f60: 722e 0000 0072 2d00 0000 da03 6c6f 63da  r....r-.....loc.
+00000f40: 3031 3072 0100 0000 7244 0000 0029 0372  010r....rD...).r
+00000f50: 4200 0000 7243 0000 0072 4400 0000 290b  B...rC...rD...).
+00000f60: 722f 0000 0072 2e00 0000 da03 6c6f 63da  r/...r......loc.
 00000f70: 036c 656e da09 4578 6365 7074 696f 6eda  .len..Exception.
-00000f80: 0666 6f72 6d61 7472 2900 0000 7242 0000  .formatr)...rB..
+00000f80: 0666 6f72 6d61 7472 2a00 0000 7243 0000  .formatr*...rC..
 00000f90: 00da 0661 7374 7970 65da 0566 6c6f 6174  ...astype..float
-00000fa0: 5a04 696c 6f63 2908 721a 0000 0072 3e00  Z.iloc).r....r>.
-00000fb0: 0000 723f 0000 0072 3900 0000 7245 0000  ..r?...r9...rE..
-00000fc0: 00da 036b 6579 722d 0000 005a 0973 656c  ...keyr-...Z.sel
-00000fd0: 6563 7469 6f6e 720d 0000 0072 0d00 0000  ectionr....r....
-00000fe0: 7215 0000 0072 4400 0000 6400 0000 732e  r....rD...d...s.
+00000fa0: 5a04 696c 6f63 2908 721b 0000 0072 3f00  Z.iloc).r....r?.
+00000fb0: 0000 7240 0000 0072 3a00 0000 7246 0000  ..r@...r:...rF..
+00000fc0: 00da 036b 6579 722e 0000 005a 0973 656c  ...keyr....Z.sel
+00000fd0: 6563 7469 6f6e 720e 0000 0072 0e00 0000  ectionr....r....
+00000fe0: 7216 0000 0072 4500 0000 6400 0000 732e  r....rE...d...s.
 00000ff0: 0000 000c 010a 0106 0104 010a 010a 0102  ................
 00001000: ff22 0202 fe0a 0302 fd04 ff0c 0702 0104  ."..............
 00001010: 010e 0102 ff04 ff1e 071a 010c 010c fd0a  ................
 00001020: 057a 2844 6174 6153 746f 7265 2e5f 6765  .z(DataStore._ge
 00001030: 745f 6361 6368 6564 5f64 6174 615f 6672  t_cached_data_fr
 00001040: 6f6d 5f64 6174 6162 6173 6563 0500 0000  om_databasec....
 00001050: 0000 0000 0000 0000 0d00 0000 0600 0000  ................
@@ -268,42 +268,42 @@
 000010b0: 067c 057c 097c 037c 0267 0283 047d 0a74  .|.|.|.|.g...}.t
 000010c0: 04a0 077c 057c 0967 02a1 017d 0b74 087c  ...|.|.g...}.t.|
 000010d0: 0b7c 0a64 0664 078d 037d 0c74 097c 017c  .|.d.d...}.t.|.|
 000010e0: 0c7c 0183 017c 0783 0353 0029 084e 4629  .|...|...S.).NF)
 000010f0: 01da 0e6f 6e6c 795f 6d61 676e 6974 7564  ...only_magnitud
 00001100: 6569 3e08 0000 69d4 0800 00e9 0a00 0000  ei>...i.........
 00001110: 5a05 6375 6269 6329 01da 046b 696e 6429  Z.cubic)...kind)
-00001120: 0a72 4600 0000 7206 0000 00da 096d 6167  .rF...r......mag
-00001130: 6e69 7475 6465 da05 756e 6974 7372 3500  nitude..unitsr5.
-00001140: 0000 7236 0000 0072 0900 0000 da0b 636f  ..r6...r......co
+00001120: 0a72 4700 0000 7206 0000 00da 096d 6167  .rG...r......mag
+00001130: 6e69 7475 6465 da05 756e 6974 7372 3600  nitude..unitsr6.
+00001140: 0000 7237 0000 0072 0900 0000 da0b 636f  ..r7...r......co
 00001150: 6e63 6174 656e 6174 6572 0400 0000 7208  ncatenater....r.
-00001160: 0000 0029 0d72 1a00 0000 5a0c 6f75 7470  ...).r....Z.outp
-00001170: 7574 5f79 6561 7273 7239 0000 0072 3c00  ut_yearsr9...r<.
-00001180: 0000 723b 0000 0072 4100 0000 7242 0000  ..r;...rA...rB..
-00001190: 0072 4300 0000 da08 7175 616e 7469 7479  .rC.....quantity
+00001160: 0000 0029 0d72 1b00 0000 5a0c 6f75 7470  ...).r....Z.outp
+00001170: 7574 5f79 6561 7273 723a 0000 0072 3d00  ut_yearsr:...r=.
+00001180: 0000 723c 0000 0072 4200 0000 7243 0000  ..r<...rB...rC..
+00001190: 0072 4400 0000 da08 7175 616e 7469 7479  .rD.....quantity
 000011a0: 5a0b 6578 7472 615f 7965 6172 735a 0d65  Z.extra_yearsZ.e
 000011b0: 7874 656e 6465 645f 6461 7461 5a0e 6578  xtended_dataZ.ex
 000011c0: 7465 6e64 6564 5f79 6561 7273 5a0a 696e  tended_yearsZ.in
-000011d0: 7465 7270 5f66 6374 720d 0000 0072 0d00  terp_fctr....r..
-000011e0: 0000 7215 0000 0072 3800 0000 7d00 0000  ..r....r8...}...
+000011d0: 7465 7270 5f66 6374 720e 0000 0072 0e00  terp_fctr....r..
+000011e0: 0000 7216 0000 0072 3900 0000 7d00 0000  ..r....r9...}...
 000011f0: 7314 0000 0012 0208 0210 0106 0106 010e  s...............
 00001200: 0312 010e 010e 0310 017a 1344 6174 6153  .........z.DataS
 00001210: 746f 7265 2e5f 6765 745f 6461 7461 6304  tore._get_datac.
 00001220: 0000 0000 0000 0000 0000 0005 0000 0005  ................
 00001230: 0000 0043 0000 0073 2000 0000 7c00 6a00  ...C...s ...|.j.
 00001240: 7c03 1900 7c02 1900 7d04 7401 a002 7c01  |...|...}.t...|.
 00001250: 7c04 6a03 7c04 6a04 a103 5300 a901 4e29  |.j.|.j...S...N)
-00001260: 0572 1f00 0000 7235 0000 00da 0669 6e74  .r....r5.....int
-00001270: 6572 7072 0e00 0000 720f 0000 0029 0572  erpr....r....).r
-00001280: 1a00 0000 da04 7965 6172 7239 0000 0072  ......yearr9...r
-00001290: 3c00 0000 7242 0000 0072 0d00 0000 720d  <...rB...r....r.
-000012a0: 0000 0072 1500 0000 da0c 5f69 6e74 6572  ...r......_inter
+00001260: 0572 2000 0000 7236 0000 00da 0669 6e74  .r ...r6.....int
+00001270: 6572 7072 0f00 0000 7210 0000 0029 0572  erpr....r....).r
+00001280: 1b00 0000 da04 7965 6172 723a 0000 0072  ......yearr:...r
+00001290: 3d00 0000 7243 0000 0072 0e00 0000 720e  =...rC...r....r.
+000012a0: 0000 0072 1600 0000 da0c 5f69 6e74 6572  ...r......_inter
 000012b0: 705f 6461 7461 8f00 0000 7304 0000 000e  p_data....s.....
 000012c0: 0112 017a 1644 6174 6153 746f 7265 2e5f  ...z.DataStore._
-000012d0: 696e 7465 7270 5f64 6174 6172 3c00 0000  interp_datar<...
+000012d0: 696e 7465 7270 5f64 6174 6172 3d00 0000  interp_datar=...
 000012e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
 000012f0: 0003 0000 0003 0000 0073 0e00 0000 8700  .........s......
 00001300: 8701 6602 6401 6402 8408 5300 2903 6111  ..f.d.d...S.).a.
 00001310: 0100 0043 7265 6174 6573 2061 2066 756e  ...Creates a fun
 00001320: 6374 696f 6e20 6769 7669 6e67 2074 6865  ction giving the
 00001330: 2076 616c 7565 206f 6620 6076 6172 6961   value of `varia
 00001340: 626c 6560 2061 7420 6120 6769 7665 6e20  ble` at a given 
@@ -319,23 +319,23 @@
 000013e0: 7472 5d2c 2066 6c6f 6174 5d3a 2069 6e74  tr], float]: int
 000013f0: 6572 706f 6c61 7469 6e67 2066 756e 6374  erpolating funct
 00001400: 696f 6e20 6f66 2074 7970 6520 6628 7965  ion of type f(ye
 00001410: 6172 2c20 7265 6769 6f6e 290a 2020 2020  ar, region).    
 00001420: 2020 2020 6302 0000 0000 0000 0000 0000      c...........
 00001430: 0002 0000 0005 0000 0013 0000 0073 0e00  .............s..
 00001440: 0000 8800 a000 7c00 7c01 8801 a103 5300  ......|.|.....S.
-00001450: 7257 0000 0029 0172 5a00 0000 2902 7259  rW...).rZ...).rY
-00001460: 0000 0072 3900 0000 a902 721a 0000 0072  ...r9.....r....r
-00001470: 3c00 0000 720d 0000 0072 1500 0000 da08  <...r....r......
+00001450: 7258 0000 0029 0172 5b00 0000 2902 725a  rX...).r[...).rZ
+00001460: 0000 0072 3a00 0000 a902 721b 0000 0072  ...r:.....r....r
+00001470: 3d00 0000 720e 0000 0072 1600 0000 da08  =...r....r......
 00001480: 3c6c 616d 6264 613e 9c00 0000 7302 0000  <lambda>....s...
 00001490: 000e 007a 2744 6174 6153 746f 7265 2e64  ...z'DataStore.d
 000014a0: 6174 615f 6f62 6a65 6374 2e3c 6c6f 6361  ata_object.<loca
-000014b0: 6c73 3e2e 3c6c 616d 6264 613e 720d 0000  ls>.<lambda>r...
-000014c0: 0072 5b00 0000 720d 0000 0072 5b00 0000  .r[...r....r[...
-000014d0: 7215 0000 00da 0b64 6174 615f 6f62 6a65  r......data_obje
+000014b0: 6c73 3e2e 3c6c 616d 6264 613e 720e 0000  ls>.<lambda>r...
+000014c0: 0072 5c00 0000 720e 0000 0072 5c00 0000  .r\...r....r\...
+000014d0: 7216 0000 00da 0b64 6174 615f 6f62 6a65  r......data_obje
 000014e0: 6374 9300 0000 7302 0000 000e 097a 1544  ct....s......z.D
 000014f0: 6174 6153 746f 7265 2e64 6174 615f 6f62  ataStore.data_ob
 00001500: 6a65 6374 6301 0000 0000 0000 0000 0000  jectc...........
 00001510: 0001 0000 0009 0000 0043 0000 0073 4000  .........C...s@.
 00001520: 0000 6401 a000 7401 7c00 6a02 a003 a100  ..d...t.|.j.....
 00001530: 8301 7c00 6a04 6402 1900 7c00 6a04 6403  ..|.j.d...|.j.d.
 00001540: 1900 7c00 6a05 7401 7c00 6a06 6404 1900  ..|.j.t.|.j.d...
@@ -343,40 +343,40 @@
 00001560: 5300 2906 4e7a 6844 6174 6153 746f 7265  S.).NzhDataStore
 00001570: 2077 6974 6820 6461 7461 2076 616c 7565   with data value
 00001580: 7320 7b7d 2063 616c 6375 6c61 7465 6420  s {} calculated 
 00001590: 6f6e 2074 6865 2079 6561 7273 207b 7d2d  on the years {}-
 000015a0: 7b7d 2066 726f 6d20 696e 7075 7420 6669  {} from input fi
 000015b0: 6c65 207b 7d20 666f 7220 7468 6520 7265  le {} for the re
 000015c0: 6769 6f6e 7320 7b7d 2061 6e64 207b 7d72  gions {} and {}r
-000015d0: 0100 0000 7247 0000 0072 1700 0000 723d  ....rG...r....r=
-000015e0: 0000 0029 0772 4c00 0000 da04 6c69 7374  ...).rL.....list
-000015f0: 721f 0000 00da 046b 6579 7372 1800 0000  r......keysr....
-00001600: 722f 0000 0072 1b00 0000 2901 721a 0000  r/...r....).r...
-00001610: 0072 0d00 0000 720d 0000 0072 1500 0000  .r....r....r....
+000015d0: 0100 0000 7248 0000 0072 1800 0000 723e  ....rH...r....r>
+000015e0: 0000 0029 0772 4d00 0000 da04 6c69 7374  ...).rM.....list
+000015f0: 7220 0000 00da 046b 6579 7372 1900 0000  r .....keysr....
+00001600: 7230 0000 0072 1c00 0000 2901 721b 0000  r0...r....).r...
+00001610: 0072 0e00 0000 720e 0000 0072 1600 0000  .r....r....r....
 00001620: da08 5f5f 7265 7072 5f5f 9e00 0000 7310  ..__repr__....s.
 00001630: 0000 0004 010c 0108 0108 0104 0110 0108  ................
 00001640: 0104 fa7a 1244 6174 6153 746f 7265 2e5f  ...z.DataStore._
-00001650: 5f72 6570 725f 5f72 5700 0000 2916 da08  _repr__rW...)...
+00001650: 5f72 6570 725f 5f72 5800 0000 2916 da08  _repr__rX...)...
 00001660: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
 00001670: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00001680: 5f5f da07 5f5f 646f 635f 5f72 2700 0000  __..__doc__r'...
-00001690: 722c 0000 0072 2000 0000 721c 0000 0072  r,...r ...r....r
-000016a0: 1d00 0000 7203 0000 0072 2a00 0000 7208  ....r....r*...r.
-000016b0: 0000 0072 1e00 0000 7246 0000 0072 4400  ...r....rF...rD.
-000016c0: 0000 7238 0000 0072 5a00 0000 7202 0000  ..r8...rZ...r...
-000016d0: 00da 0369 6e74 724e 0000 0072 5d00 0000  ...intrN...r]...
-000016e0: 7260 0000 0072 0d00 0000 720d 0000 0072  r`...r....r....r
-000016f0: 0d00 0000 7215 0000 0072 0a00 0000 1000  ....r....r......
+00001680: 5f5f da07 5f5f 646f 635f 5f72 2800 0000  __..__doc__r(...
+00001690: 722d 0000 0072 2100 0000 721d 0000 0072  r-...r!...r....r
+000016a0: 1e00 0000 7203 0000 0072 2b00 0000 7208  ....r....r+...r.
+000016b0: 0000 0072 1f00 0000 7247 0000 0072 4500  ...r....rG...rE.
+000016c0: 0000 7239 0000 0072 5b00 0000 7202 0000  ..r9...r[...r...
+000016d0: 00da 0369 6e74 724f 0000 0072 5e00 0000  ...intrO...r^...
+000016e0: 7261 0000 0072 0e00 0000 720e 0000 0072  ra...r....r....r
+000016f0: 0e00 0000 7216 0000 0072 0a00 0000 1000  ....r....r......
 00001700: 0000 731c 0000 0008 0004 0104 0e04 0108  ..s.............
 00001710: 0208 1808 1118 0608 0708 0c10 1908 121e  ................
-00001720: 040c 0b72 0a00 0000 2912 7264 0000 0072  ...r....).rd...r
-00001730: 2200 0000 da06 7479 7069 6e67 7202 0000  ".....typingr...
-00001740: 0072 0300 0000 da05 6e75 6d70 7972 3500  .r......numpyr5.
-00001750: 0000 da06 7061 6e64 6173 7228 0000 005a  ....pandasr(...Z
+00001720: 040c 0b72 0a00 0000 2912 7265 0000 0072  ...r....).re...r
+00001730: 2300 0000 da06 7479 7069 6e67 7202 0000  #.....typingr...
+00001740: 0072 0300 0000 da05 6e75 6d70 7972 3600  .r......numpyr6.
+00001750: 0000 da06 7061 6e64 6173 7229 0000 005a  ....pandasr)...Z
 00001760: 1173 6369 7079 2e69 6e74 6572 706f 6c61  .scipy.interpola
 00001770: 7465 7204 0000 00da 0d6d 696d 6f73 612e  ter......mimosa.
 00001780: 636f 6d6d 6f6e 7205 0000 0072 0600 0000  commonr....r....
 00001790: da05 7574 696c 7372 0800 0000 7209 0000  ..utilsr....r...
-000017a0: 0072 0a00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-000017b0: 720d 0000 0072 1500 0000 da08 3c6d 6f64  r....r......<mod
+000017a0: 0072 0a00 0000 720e 0000 0072 0e00 0000  .r....r....r....
+000017b0: 720e 0000 0072 1600 0000 da08 3c6d 6f64  r....r......<mod
 000017c0: 756c 653e 0100 0000 7312 0000 0004 0008  ule>....s.......
 000017d0: 0510 0108 0108 010c 0110 0210 0112 03    ...............
```

### Comparing `mimosa-0.1.3/mimosa/common/data/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/data/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 06:54:00 2023 UTC, .py size: 1463 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 882b ba64 b705 0000  o........+.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 b705 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a05 6501  m.Z...d.d.l.Z.e.
 00000050: 4700 6404 6405 8400 6405 8302 8301 5a06  G.d.d...d.....Z.
 00000060: 6409 6407 6408 8401 5a07 6403 5300 290a  d.d.d...Z.d.S.).
 00000070: e900 0000 0029 01da 0964 6174 6163 6c61  .....)...datacla
@@ -15,19 +15,19 @@
 000000e0: 616c 7565 73da 0778 7661 6c75 6573 da07  alues..xvalues..
 000000f0: 7976 616c 7565 734e da04 756e 6974 2907  yvaluesN..unit).
 00000100: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 00000110: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 00000120: 6d65 5f5f 7203 0000 00da 0f5f 5f61 6e6e  me__r......__ann
 00000130: 6f74 6174 696f 6e73 5f5f 7207 0000 00da  otations__r.....
 00000140: 0373 7472 a900 720d 0000 0072 0d00 0000  .str..r....r....
-00000150: fa5d 633a 5c75 7365 7273 5c33 3930 3338  .]c:\users\39038
-00000160: 3835 5c6f 6e65 6472 6976 6520 2d20 756e  85\onedrive - un
-00000170: 6976 6572 7369 7465 6974 2075 7472 6563  iversiteit utrec
-00000180: 6874 5c64 6f63 756d 656e 7473 5c6d 696d  ht\documents\mim
-00000190: 6f73 615c 6d69 6d6f 7361 5c63 6f6d 6d6f  osa\mimosa\commo
+00000150: fa5d 633a 5c55 7365 7273 5c33 3930 3338  .]c:\Users\39038
+00000160: 3835 5c4f 6e65 4472 6976 6520 2d20 556e  85\OneDrive - Un
+00000170: 6976 6572 7369 7465 6974 2055 7472 6563  iversiteit Utrec
+00000180: 6874 5c44 6f63 756d 656e 7473 5c4d 494d  ht\Documents\MIM
+00000190: 4f53 415c 6d69 6d6f 7361 5c63 6f6d 6d6f  OSA\mimosa\commo
 000001a0: 6e5c 6461 7461 5c75 7469 6c73 2e70 7972  n\data\utils.pyr
 000001b0: 0400 0000 0700 0000 7308 0000 000a 0008  ........s.......
 000001c0: 0208 0110 0172 0400 0000 e932 0000 0063  .....r.....2...c
 000001d0: 0500 0000 0000 0000 0000 0000 0e00 0000  ................
 000001e0: 0700 0000 4300 0000 73ae 0000 0064 017d  ....C...s....d.}
 000001f0: 057c 0064 0219 007c 0064 0319 0018 007c  .|.d...|.d.....|
 00000200: 0164 0219 007c 0164 0319 0018 001b 007d  .d...|.d.......}
```

### Comparing `mimosa-0.1.3/mimosa/common/data/datastore.py` & `mimosa-0.1.4/mimosa/common/data/datastore.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/data/utils.py` & `mimosa-0.1.4/mimosa/common/data/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/economics.py` & `mimosa-0.1.4/mimosa/common/economics.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/pyomo_utils.py` & `mimosa-0.1.4/mimosa/common/pyomo_utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 06:54:00 2023 UTC, .py size: 2754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 882b ba64 c20a 0000  o........+.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 c20a 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 4700  Z.d.d.l.m.Z...G.
 00000040: 6403 6404 8400 6404 8302 5a03 6405 5300  d.d...d...Z.d.S.
 00000050: 2906 6133 0100 000a 4372 6561 7465 2061  ).a3....Create a
 00000060: 2052 6567 696f 6e61 6c50 6172 616d 5374   RegionalParamSt
 00000070: 6f72 6520 6f62 6a65 6374 2077 6869 6368  ore object which
@@ -105,19 +105,19 @@
 00000680: 434f 4143 4348 2e63 7376 da06 434f 4143  COACCH.csv..COAC
 00000690: 4348 2905 da09 6563 6f6e 6f6d 6963 735a  CH)...economicsZ
 000006a0: 034d 4143 7205 0000 0072 0600 0000 7207  .MACr....r....r.
 000006b0: 0000 0029 04da 0670 6172 616d 7372 0400  ...)...paramsr..
 000006c0: 0000 7202 0000 00da 0a63 6174 6567 6f72  ..r......categor
 000006d0: 6965 7329 03da 0473 656c 6672 0900 0000  ies)...selfr....
 000006e0: 5a11 7265 6769 6f6e 7479 7065 5f6f 7574  Z.regiontype_out
-000006f0: 7075 74a9 0072 0c00 0000 fa67 633a 5c75  put..r.....gc:\u
-00000700: 7365 7273 5c33 3930 3338 3835 5c6f 6e65  sers\3903885\one
-00000710: 6472 6976 6520 2d20 756e 6976 6572 7369  drive - universi
-00000720: 7465 6974 2075 7472 6563 6874 5c64 6f63  teit utrecht\doc
-00000730: 756d 656e 7473 5c6d 696d 6f73 615c 6d69  uments\mimosa\mi
+000006f0: 7075 74a9 0072 0c00 0000 fa67 633a 5c55  put..r.....gc:\U
+00000700: 7365 7273 5c33 3930 3338 3835 5c4f 6e65  sers\3903885\One
+00000710: 4472 6976 6520 2d20 556e 6976 6572 7369  Drive - Universi
+00000720: 7465 6974 2055 7472 6563 6874 5c44 6f63  teit Utrecht\Doc
+00000730: 756d 656e 7473 5c4d 494d 4f53 415c 6d69  uments\MIMOSA\mi
 00000740: 6d6f 7361 5c63 6f6d 6d6f 6e5c 7265 6769  mosa\common\regi
 00000750: 6f6e 616c 5f70 6172 616d 735c 6d61 696e  onal_params\main
 00000760: 2e70 79da 085f 5f69 6e69 745f 5f33 0000  .py..__init__3..
 00000770: 0073 1e00 0000 0601 0a01 0802 0203 0601  .s..............
 00000780: 02ff 0a03 0201 0601 02ff 0203 0601 02ff  ................
 00000790: 0a03 0cf5 7a1b 5265 6769 6f6e 616c 5061  ....z.RegionalPa
 000007a0: 7261 6d53 746f 7265 2e5f 5f69 6e69 745f  ramStore.__init_
```

### Comparing `mimosa-0.1.3/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:42:30 2023 UTC, .py size: 2772 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e636 ba64 d40a 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 d40a 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7200 0000 5500  .....@...sr...U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6402 6c03 5a04 4700 6403  l.Z.d.d.l.Z.G.d.
 00000050: 6404 8400 6404 8302 5a05 6900 5a06 6502  d...d...Z.i.Z.e.
 00000060: 6a07 6508 6505 6602 1900 6509 6405 3c00  j.e.e.f...e.d.<.
 00000070: 6406 6407 8400 5a0a 650a 6408 6409 640a  d.d...Z.e.d.d.d.
@@ -53,19 +53,19 @@
 00000340: 0872 6561 645f 6373 76da 076d 6170 7069  .read_csv..mappi
 00000350: 6e67 da07 636f 6c75 6d6e 73da 084b 6579  ng..columns..Key
 00000360: 4572 726f 72da 0666 6f72 6d61 7429 05da  Error..format)..
 00000370: 0473 656c 66da 0b72 6567 696f 6e74 7970  .self..regiontyp
 00000380: 6531 da0b 7265 6769 6f6e 7479 7065 32da  e1..regiontype2.
 00000390: 0c6d 6170 7069 6e67 5f66 696c 65da 0d66  .mapping_file..f
 000003a0: 756c 6c5f 6669 6c65 6e61 6d65 a900 7213  ull_filename..r.
-000003b0: 0000 00fa 7163 3a5c 7573 6572 735c 3339  ....qc:\users\39
-000003c0: 3033 3838 355c 6f6e 6564 7269 7665 202d  03885\onedrive -
-000003d0: 2075 6e69 7665 7273 6974 6569 7420 7574   universiteit ut
-000003e0: 7265 6368 745c 646f 6375 6d65 6e74 735c  recht\documents\
-000003f0: 6d69 6d6f 7361 5c6d 696d 6f73 615c 636f  mimosa\mimosa\co
+000003b0: 0000 00fa 7163 3a5c 5573 6572 735c 3339  ....qc:\Users\39
+000003c0: 3033 3838 355c 4f6e 6544 7269 7665 202d  03885\OneDrive -
+000003d0: 2055 6e69 7665 7273 6974 6569 7420 5574   Universiteit Ut
+000003e0: 7265 6368 745c 446f 6375 6d65 6e74 735c  recht\Documents\
+000003f0: 4d49 4d4f 5341 5c6d 696d 6f73 615c 636f  MIMOSA\mimosa\co
 00000400: 6d6d 6f6e 5c72 6567 696f 6e61 6c5f 7061  mmon\regional_pa
 00000410: 7261 6d73 5c72 6567 696f 6e5f 6d61 7070  rams\region_mapp
 00000420: 6572 732e 7079 da08 5f5f 696e 6974 5f5f  ers.py..__init__
 00000430: 1100 0000 731c 0000 0006 010a 0102 0102  ....s...........
 00000440: 0104 fd0c 060c 040c 0102 0204 0106 0102  ................
 00000450: ff04 ff04 fe7a 1552 6567 696f 6e4d 6170  .....z.RegionMap
 00000460: 7065 722e 5f5f 696e 6974 5f5f da06 7265  per.__init__..re
```

### Comparing `mimosa-0.1.3/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc` & `mimosa-0.1.4/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:42:30 2023 UTC, .py size: 1340 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e636 ba64 3c05 0000  o........6.d<...
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 3c05 0000  o........i.d<...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6403 6404 6c04 6d05 5a05 0100 4700  Z.d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 8302 5a06 6402 5300  d.d...d...Z.d.S.
 00000060: 2907 7a37 5468 6520 7374 6f72 6520 7573  ).z7The store us
 00000070: 6573 2052 6567 696f 6e61 6c50 6172 616d  es RegionalParam
@@ -38,19 +38,19 @@
 00000250: 0b6d 6170 5f72 6567 696f 6e73 2907 da04  .map_regions)...
 00000260: 7365 6c66 da08 6669 6c65 6e61 6d65 5a10  self..filenameZ.
 00000270: 7265 6769 6f6e 7479 7065 5f69 6e70 7574  regiontype_input
 00000280: da11 7265 6769 6f6e 7479 7065 5f6f 7574  ..regiontype_out
 00000290: 7075 74da 0d66 756c 6c5f 6669 6c65 6e61  put..full_filena
 000002a0: 6d65 5a08 6461 7461 5f72 6177 5a0d 7265  meZ.data_rawZ.re
 000002b0: 6769 6f6e 5f6d 6170 7065 72a9 0072 1400  gion_mapper..r..
-000002c0: 0000 fa7b 633a 5c75 7365 7273 5c33 3930  ...{c:\users\390
-000002d0: 3338 3835 5c6f 6e65 6472 6976 6520 2d20  3885\onedrive - 
-000002e0: 756e 6976 6572 7369 7465 6974 2075 7472  universiteit utr
-000002f0: 6563 6874 5c64 6f63 756d 656e 7473 5c6d  echt\documents\m
-00000300: 696d 6f73 615c 6d69 6d6f 7361 5c63 6f6d  imosa\mimosa\com
+000002c0: 0000 fa7b 633a 5c55 7365 7273 5c33 3930  ...{c:\Users\390
+000002d0: 3338 3835 5c4f 6e65 4472 6976 6520 2d20  3885\OneDrive - 
+000002e0: 556e 6976 6572 7369 7465 6974 2055 7472  Universiteit Utr
+000002f0: 6563 6874 5c44 6f63 756d 656e 7473 5c4d  echt\Documents\M
+00000300: 494d 4f53 415c 6d69 6d6f 7361 5c63 6f6d  IMOSA\mimosa\com
 00000310: 6d6f 6e5c 7265 6769 6f6e 616c 5f70 6172  mon\regional_par
 00000320: 616d 735c 7265 6769 6f6e 616c 5f70 6172  ams\regional_par
 00000330: 616d 5f63 6f6e 7461 696e 6572 2e70 79da  am_container.py.
 00000340: 085f 5f69 6e69 745f 5f0a 0000 0073 2800  .__init__....s(.
 00000350: 0000 0601 0a01 0201 0201 04fd 0a05 0802  ................
 00000360: 1001 0203 1001 0c01 0201 0e01 04ff 02ff  ................
 00000370: 0405 0601 02ff 0602 08fe 7a1f 5265 6769  ..........z.Regi
```

### Comparing `mimosa-0.1.3/mimosa/common/regional_params/main.py` & `mimosa-0.1.4/mimosa/common/regional_params/main.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/regional_params/region_mappers.py` & `mimosa-0.1.4/mimosa/common/regional_params/region_mappers.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/regional_params/regional_param_container.py` & `mimosa-0.1.4/mimosa/common/regional_params/regional_param_container.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/units.py` & `mimosa-0.1.4/mimosa/common/units.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/common/utils.py` & `mimosa-0.1.4/mimosa/common/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/__pycache__/abatement.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/__pycache__/abatement.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/__pycache__/burdensharing.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/__pycache__/burdensharing.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 4025 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 b90f 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 e6e8 ba64 c90e 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 0100 6404 6504 6405 6502 6507  m.Z...d.e.d.e.e.
 00000070: 1900 6604 6406 6407 8404 5a0c 6408 6409  ..f.d.d...Z.d.d.
@@ -15,227 +15,217 @@
 000000e0: 0356 6172 da05 5061 7261 6dda 1147 656e  .Var..Param..Gen
 000000f0: 6572 616c 436f 6e73 7472 6169 6e74 da1e  eralConstraint..
 00000100: 5265 6769 6f6e 616c 536f 6674 4571 7561  RegionalSoftEqua
 00000110: 6c69 7479 436f 6e73 7472 6169 6e74 da03  lityConstraint..
 00000120: 416e 79da 0571 7561 6e74 da05 7661 6c75  Any..quant..valu
 00000130: 65da 016d da06 7265 7475 726e 6301 0000  e..m..returnc...
 00000140: 0000 0000 0000 0000 0002 0000 000a 0000  ................
-00000150: 0043 0000 0073 f200 0000 6700 7d01 7400  .C...s....g.}.t.
+00000150: 0043 0000 0073 c800 0000 6700 7d01 7400  .C...s....g.}.t.
 00000160: 7401 6401 8d01 7c00 5f02 7403 7c00 6a04  t.d...|._.t.|.j.
 00000170: 7405 a006 6402 a101 6403 8d02 7c00 5f07  t...d...d...|._.
 00000180: 7c01 a008 7409 6404 6405 8400 6406 6405  |...t.d.d...d.d.
 00000190: 8400 6407 6408 6405 8400 6409 8d04 7409  ..d.d.d...d...t.
 000001a0: 640a 6405 8400 640b 6405 8400 640c 640d  d.d...d.d...d.d.
 000001b0: 6405 8400 6409 8d04 6702 a101 0100 7400  d...d...g.....t.
 000001c0: 7c00 6a0a 640e 6405 8400 640f 8d02 7c00  |.j.d.d...d...|.
 000001d0: 5f0b 7400 6410 640f 8d01 7c00 5f0c 7400  _.t.d.d...|._.t.
 000001e0: 7c00 6a04 7c00 6a0a 6411 6405 8400 640f  |.j.|.j.d.d...d.
-000001f0: 8d03 7c00 5f0d 7403 7c00 6a04 7c00 6a0a  ..|._.t.|.j.|.j.
-00000200: 8302 7c00 5f0e 7403 7c00 6a04 7c00 6a0a  ..|._.t.|.j.|.j.
-00000210: 7405 a006 6412 a101 6403 8d03 7c00 5f0f  t...d...d...|._.
-00000220: 7c01 a008 7409 6413 6405 8400 6414 6405  |...t.d.d...d.d.
-00000230: 8400 6415 6416 6417 6405 8400 6418 6419  ..d.d.d.d...d.d.
-00000240: 8d06 6701 a101 0100 7c01 5300 291a 6113  ..g.....|.S.).a.
-00000250: 0100 0045 6d69 7373 696f 6e73 2061 6e64  ...Emissions and
-00000260: 2074 656d 7065 7261 7475 7265 2065 7175   temperature equ
-00000270: 6174 696f 6e73 2061 6e64 2063 6f6e 7374  ations and const
-00000280: 7261 696e 7473 0a0a 2020 2020 4e65 6365  raints..    Nece
-00000290: 7373 6172 7920 7661 7269 6162 6c65 733a  ssary variables:
-000002a0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-000002b0: 2020 2020 2020 206c 6973 7420 6f66 2063         list of c
-000002c0: 6f6e 7374 7261 696e 7473 2028 616e 7920  onstraints (any 
-000002d0: 6f66 3a0a 2020 2020 2020 2020 2020 202d  of:.           -
-000002e0: 2047 6c6f 6261 6c43 6f6e 7374 7261 696e   GlobalConstrain
-000002f0: 740a 2020 2020 2020 2020 2020 202d 2047  t.           - G
-00000300: 6c6f 6261 6c49 6e69 7443 6f6e 7374 7261  lobalInitConstra
-00000310: 696e 740a 2020 2020 2020 2020 2020 202d  int.           -
-00000320: 2052 6567 696f 6e61 6c43 6f6e 7374 7261   RegionalConstra
-00000330: 696e 740a 2020 2020 2020 2020 2020 202d  int.           -
-00000340: 2052 6567 696f 6e61 6c49 6e69 7443 6f6e   RegionalInitCon
-00000350: 7374 7261 696e 740a 2020 2020 2020 2020  straint.        
-00000360: 290a 2020 2020 2901 da06 7769 7468 696e  ).    )...within
-00000370: 5a0f 6672 6163 7469 6f6e 5f6f 665f 4744  Z.fraction_of_GD
-00000380: 5029 01da 0575 6e69 7473 6303 0000 0000  P)...unitsc.....
-00000390: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
-000003a0: 0000 0073 2a00 0000 7c00 6a00 7c01 7c02  ...s*...|.j.|.|.
-000003b0: 6602 1900 7c00 6a01 7c01 7c02 6602 1900  f...|.j.|.|.f...
-000003c0: 1700 7c00 6a02 7c01 7c02 6602 1900 1700  ..|.j.|.|.f.....
-000003d0: 5300 a901 4e29 03da 1372 656c 5f61 6261  S...N)...rel_aba
-000003e0: 7465 6d65 6e74 5f63 6f73 7473 da0c 6461  tement_costs..da
-000003f0: 6d61 6765 5f63 6f73 7473 5a16 7265 6c5f  mage_costsZ.rel_
-00000400: 6669 6e61 6e63 6961 6c5f 7472 616e 7366  financial_transf
-00000410: 6572 a903 720b 0000 00da 0174 da01 72a9  er..r......t..r.
-00000420: 0072 1500 0000 fa64 633a 5c75 7365 7273  .r.....dc:\users
-00000430: 5c33 3930 3338 3835 5c6f 6e65 6472 6976  \3903885\onedriv
-00000440: 6520 2d20 756e 6976 6572 7369 7465 6974  e - universiteit
-00000450: 2075 7472 6563 6874 5c64 6f63 756d 656e   utrecht\documen
-00000460: 7473 5c6d 696d 6f73 615c 6d69 6d6f 7361  ts\mimosa\mimosa
-00000470: 5c63 6f6d 706f 6e65 6e74 735c 6275 7264  \components\burd
-00000480: 656e 7368 6172 696e 672e 7079 da08 3c6c  ensharing.py..<l
-00000490: 616d 6264 613e 2b00 0000 730a 0000 000c  ambda>+...s.....
-000004a0: 000c 0102 ff0c 0204 fe7a 2167 6574 5f63  .........z!get_c
-000004b0: 6f6e 7374 7261 696e 7473 2e3c 6c6f 6361  onstraints.<loca
-000004c0: 6c73 3e2e 3c6c 616d 6264 613e 6303 0000  ls>.<lambda>c...
-000004d0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-000004e0: 0053 0000 00f3 0a00 0000 7c00 6a00 7c01  .S........|.j.|.
-000004f0: 1900 5300 720f 0000 00a9 01da 1b62 7572  ..S.r........bur
-00000500: 6465 6e5f 7368 6172 696e 675f 636f 6d6d  den_sharing_comm
-00000510: 6f6e 5f6c 6576 656c 7212 0000 0072 1500  on_levelr....r..
-00000520: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000530: 002e 0000 00f3 0200 0000 0a00 5a21 6275  ............Z!bu
-00000540: 7264 656e 5f73 6861 7269 6e67 5f72 6567  rden_sharing_reg
-00000550: 696d 655f 746f 7461 6c5f 636f 7374 7363  ime_total_costsc
-00000560: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000570: 0300 0000 5300 0000 731c 0000 0074 007c  ....S...s....t.|
-00000580: 006a 0183 0164 016b 0370 0d7c 00a0 027c  .j...d.k.p.|...|
-00000590: 01a1 0164 026b 0453 0029 034e 5a11 6571  ...d.k.S.).NZ.eq
-000005a0: 7561 6c5f 746f 7461 6c5f 636f 7374 7369  ual_total_costsi
-000005b0: 3408 0000 2903 720a 0000 00da 1562 7572  4...).r......bur
-000005c0: 6465 6e5f 7368 6172 696e 675f 7265 6769  den_sharing_regi
-000005d0: 6d65 da04 7965 6172 7212 0000 0072 1500  me..yearr....r..
-000005e0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-000005f0: 0030 0000 0073 0800 0000 0800 0201 04ff  .0...s..........
-00000600: 0e02 2901 da09 6967 6e6f 7265 5f69 6663  ..)...ignore_ifc
-00000610: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000620: 0300 0000 5300 0000 730e 0000 007c 006a  ....S...s....|.j
-00000630: 007c 017c 0266 0219 0053 0072 0f00 0000  .|.|.f...S.r....
-00000640: 2901 7210 0000 0072 1200 0000 7215 0000  ).r....r....r...
-00000650: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000660: 3600 0000 7302 0000 000e 0063 0300 0000  6...s......c....
-00000670: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00000680: 5300 0000 7218 0000 0072 0f00 0000 7219  S...r....r....r.
-00000690: 0000 0072 1200 0000 7215 0000 0072 1500  ...r....r....r..
-000006a0: 0000 7216 0000 0072 1700 0000 3700 0000  ..r....r....7...
-000006b0: 721b 0000 005a 2562 7572 6465 6e5f 7368  r....Z%burden_sh
-000006c0: 6172 696e 675f 7265 6769 6d65 5f61 6261  aring_regime_aba
-000006d0: 7465 6d65 6e74 5f63 6f73 7473 6303 0000  tement_costsc...
-000006e0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-000006f0: 0053 0000 0073 0e00 0000 7400 7c00 6a01  .S...s....t.|.j.
-00000700: 8301 6401 6b03 5300 2902 4e5a 1565 7175  ..d.k.S.).NZ.equ
-00000710: 616c 5f61 6261 7465 6d65 6e74 5f63 6f73  al_abatement_cos
-00000720: 7473 a902 720a 0000 0072 1c00 0000 7212  ts..r....r....r.
-00000730: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00000740: 0000 7217 0000 0039 0000 0073 0600 0000  ..r....9...s....
-00000750: 0800 0201 04ff 6302 0000 0000 0000 0000  ......c.........
-00000760: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
-00000770: 2a00 0000 8800 a000 8800 a001 6401 a101  *...........d...
-00000780: 7c01 a102 7402 8700 6601 6402 6403 8408  |...t...f.d.d...
-00000790: 8800 6a03 4400 8301 8301 1b00 5300 2904  ..j.D.......S.).
-000007a0: 4e72 0100 0000 6301 0000 0000 0000 0000  Nr....c.........
-000007b0: 0000 0002 0000 0006 0000 0033 0000 0073  ...........3...s
-000007c0: 2200 0000 8100 7c00 5d0c 7d01 8800 a000  ".....|.].}.....
-000007d0: 8800 a001 6400 a101 7c01 a102 5600 0100  ....d...|...V...
-000007e0: 7102 6401 5300 2902 7201 0000 004e 2902  q.d.S.).r....N).
-000007f0: da12 6261 7365 6c69 6e65 5f65 6d69 7373  ..baseline_emiss
-00000800: 696f 6e73 721d 0000 00a9 02da 022e 30da  ionsr.........0.
-00000810: 0173 a901 720b 0000 0072 1500 0000 7216  .s..r....r....r.
-00000820: 0000 00da 093c 6765 6e65 7870 723e 4700  .....<genexpr>G.
-00000830: 0000 f304 0000 0002 8020 00fa 3467 6574  ......... ..4get
-00000840: 5f63 6f6e 7374 7261 696e 7473 2e3c 6c6f  _constraints.<lo
-00000850: 6361 6c73 3e2e 3c6c 616d 6264 613e 2e3c  cals>.<lambda>.<
-00000860: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
-00000870: 3e29 0472 2000 0000 721d 0000 00da 0373  >).r ...r......s
-00000880: 756d da07 7265 6769 6f6e 7329 0272 0b00  um..regions).r..
-00000890: 0000 7214 0000 0072 1500 0000 7224 0000  ..r....r....r$..
-000008a0: 0072 1600 0000 7217 0000 0046 0000 0073  .r....r....F...s
-000008b0: 0600 0000 1000 1601 04ff 2901 da0a 696e  ..........)...in
-000008c0: 6974 6961 6c69 7a65 6902 0800 0063 0300  itializei....c..
-000008d0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-000008e0: 0000 1300 0000 732c 0000 0088 00a0 0088  ......s,........
-000008f0: 00a0 0188 01a1 017c 02a1 0274 0287 0087  .......|...t....
-00000900: 0166 0264 0164 0284 0888 006a 0344 0083  .f.d.d.....j.D..
-00000910: 0183 011b 0053 0029 034e 6301 0000 0000  .....S.).Nc.....
-00000920: 0000 0000 0000 0002 0000 0006 0000 0033  ...............3
-00000930: 0000 0073 2200 0000 8100 7c00 5d0c 7d01  ...s".....|.].}.
-00000940: 8800 a000 8800 a001 8801 a101 7c01 a102  ............|...
-00000950: 5600 0100 7102 6400 5300 720f 0000 0029  V...q.d.S.r....)
-00000960: 02da 0a70 6f70 756c 6174 696f 6e72 1d00  ...populationr..
-00000970: 0000 7221 0000 00a9 0272 0b00 0000 7213  ..r!.....r....r.
-00000980: 0000 0072 1500 0000 7216 0000 0072 2500  ...r....r....r%.
-00000990: 0000 4e00 0000 7226 0000 0072 2700 0000  ..N...r&...r'...
-000009a0: 2904 722b 0000 0072 1d00 0000 7228 0000  ).r+...r....r(..
-000009b0: 0072 2900 0000 7212 0000 0072 1500 0000  .r)...r....r....
-000009c0: 722c 0000 0072 1600 0000 7217 0000 004d  r,...r....r....M
-000009d0: 0000 0073 0600 0000 1000 1801 04ff da12  ...s............
-000009e0: 656d 6973 7369 6f6e 7372 6174 655f 756e  emissionsrate_un
-000009f0: 6974 6303 0000 0000 0000 0000 0000 0003  itc.............
-00000a00: 0000 0004 0000 0053 0000 0073 1600 0000  .......S...s....
-00000a10: 7400 7c00 7c01 7c02 8303 7c00 6a01 7c01  t.|.|.|...|.j.|.
-00000a20: 1900 1400 5300 720f 0000 0029 02da 1570  ....S.r....)...p
-00000a30: 6572 6361 7063 6f6e 765f 7368 6172 655f  ercapconv_share_
-00000a40: 7275 6c65 da10 676c 6f62 616c 5f65 6d69  rule..global_emi
-00000a50: 7373 696f 6e73 7212 0000 0072 1500 0000  ssionsr....r....
-00000a60: 7215 0000 0072 1600 0000 7217 0000 005a  r....r....r....Z
-00000a70: 0000 0073 0200 0000 1600 6303 0000 0000  ...s......c.....
-00000a80: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
-00000a90: 0000 0073 1c00 0000 7c00 6a00 7c01 7c02  ...s....|.j.|.|.
-00000aa0: 6602 1900 7c00 6a01 7c01 7c02 6602 1900  f...|.j.|.|.f...
-00000ab0: 1800 5300 720f 0000 0029 02da 0862 6173  ..S.r....)...bas
-00000ac0: 656c 696e 655a 1c70 6169 645f 666f 725f  elineZ.paid_for_
-00000ad0: 656d 6973 7369 6f6e 5f72 6564 7563 7469  emission_reducti
-00000ae0: 6f6e 7372 1200 0000 7215 0000 0072 1500  onsr....r....r..
-00000af0: 0000 7216 0000 0072 1700 0000 5b00 0000  ..r....r....[...
-00000b00: 7302 0000 001c 004e 677b 14ae 47e1 7a84  s......Ng{..G.z.
-00000b10: 3f63 0300 0000 0000 0000 0000 0000 0300  ?c..............
-00000b20: 0000 0200 0000 5300 0000 7316 0000 0074  ......S...s....t
-00000b30: 007c 006a 0183 0164 016b 0370 0a7c 0164  .|.j...d.k.p.|.d
-00000b40: 026b 0253 0029 034e 5a13 7065 725f 6361  .k.S.).NZ.per_ca
-00000b50: 705f 636f 6e76 6572 6765 6e63 6572 0100  p_convergencer..
-00000b60: 0000 721f 0000 0072 1200 0000 7215 0000  ..r....r....r...
-00000b70: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000b80: 5e00 0000 7308 0000 0008 0002 0104 ff08  ^...s...........
-00000b90: 025a 0f70 6572 6361 7063 6f6e 765f 7275  .Z.percapconv_ru
-00000ba0: 6c65 2904 da07 6570 7369 6c6f 6eda 1061  le)...epsilon..a
-00000bb0: 6273 6f6c 7574 655f 6570 7369 6c6f 6e72  bsolute_epsilonr
-00000bc0: 1e00 0000 da04 6e61 6d65 2910 7205 0000  ......name).r...
-00000bd0: 0072 0800 0000 721c 0000 0072 0400 0000  .r....r....r....
-00000be0: 7213 0000 0072 0900 0000 da04 756e 6974  r....r......unit
-00000bf0: 721a 0000 00da 0665 7874 656e 6472 0700  r......extendr..
-00000c00: 0000 7229 0000 00da 1570 6572 6361 7063  ..r).....percapc
-00000c10: 6f6e 765f 7368 6172 655f 696e 6974 da0f  onv_share_init..
-00000c20: 7065 7263 6170 636f 6e76 5f79 6561 72da  percapconv_year.
-00000c30: 1470 6572 6361 7063 6f6e 765f 7368 6172  .percapconv_shar
-00000c40: 655f 706f 705a 1970 6572 6361 7063 6f6e  e_popZ.percapcon
-00000c50: 765f 656d 6973 7369 6f6e 5f73 6861 7265  v_emission_share
-00000c60: 5a33 7065 7263 6170 636f 6e76 5f69 6d70  Z3percapconv_imp
-00000c70: 6f72 745f 6578 706f 7274 5f65 6d69 7373  ort_export_emiss
-00000c80: 696f 6e5f 7265 6475 6374 696f 6e5f 6261  ion_reduction_ba
-00000c90: 6c61 6e63 6529 0272 0b00 0000 da0b 636f  lance).r......co
-00000ca0: 6e73 7472 6169 6e74 7372 1500 0000 7215  nstraintsr....r.
-00000cb0: 0000 0072 1600 0000 da0f 6765 745f 636f  ...r......get_co
-00000cc0: 6e73 7472 6169 6e74 7313 0000 0073 5c00  nstraints....s\.
-00000cd0: 0000 040d 0c02 1603 0402 0203 0601 0603  ................
-00000ce0: 0201 0601 04fa 020b 0601 0601 0201 0601  ................
-00000cf0: 04fc 02f3 04ff 021d 0401 0601 08fe 0c05  ................
-00000d00: 0201 0401 0401 0601 08fd 0207 0801 06ff  ................
-00000d10: 0203 1001 08ff 0403 0202 0601 0601 0201  ................
-00000d20: 0201 0601 0203 04f8 02ff 04ff 040f 723a  ..............r:
-00000d30: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00000d40: 0700 0000 0400 0000 4300 0000 7384 0000  ........C...s...
-00000d50: 007c 00a0 0064 01a1 017c 00a0 007c 01a1  .|...d...|...|..
-00000d60: 0102 027d 037d 047c 006a 017d 057c 0564  ...}.}.|.j.}.|.d
-00000d70: 0275 0072 177c 006a 027c 0219 0053 007c  .u.r.|.j.|...S.|
-00000d80: 057c 036b 0272 227c 006a 037c 017c 0266  .|.k.r"|.j.|.|.f
-00000d90: 0219 0053 007c 047c 0318 007c 057c 0318  ...S.|.|...|.|..
-00000da0: 001b 007d 0674 047c 0664 0383 027c 006a  ...}.t.|.d...|.j
-00000db0: 037c 017c 0266 0219 0014 0074 0564 037c  .|.|.f.....t.d.|
-00000dc0: 0618 0064 0183 027c 006a 027c 0219 0014  ...d...|.j.|....
-00000dd0: 0017 0053 0029 044e 7201 0000 0046 e901  ...S.).Nr....F..
-00000de0: 0000 0029 0672 1d00 0000 7237 0000 0072  ...).r....r7...r
-00000df0: 3600 0000 7238 0000 00da 036d 696e da03  6...r8.....min..
-00000e00: 6d61 7829 0772 0b00 0000 7213 0000 0072  max).r....r....r
-00000e10: 1400 0000 5a06 7965 6172 5f30 5a06 7965  ....Z.year_0Z.ye
-00000e20: 6172 5f74 5a09 7965 6172 5f63 6f6e 765a  ar_tZ.year_convZ
-00000e30: 1079 6561 725f 6c69 6e65 6172 5f70 6172  .year_linear_par
-00000e40: 7472 1500 0000 7215 0000 0072 1600 0000  tr....r....r....
-00000e50: 722e 0000 0069 0000 0073 1600 0000 1601  r....i...s......
-00000e60: 0601 0802 0a02 0801 0e02 1002 1603 1601  ................
-00000e70: 02ff 02ff 722e 0000 004e 290e da07 5f5f  ....r....N)...__
-00000e80: 646f 635f 5fda 0674 7970 696e 6772 0200  doc__..typingr..
-00000e90: 0000 da0d 6d69 6d6f 7361 2e63 6f6d 6d6f  ....mimosa.commo
-00000ea0: 6e72 0300 0000 7204 0000 0072 0500 0000  nr....r....r....
-00000eb0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00000ec0: 0900 0000 720a 0000 0072 3a00 0000 722e  ....r....r:...r.
-00000ed0: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
-00000ee0: 0000 7216 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000ef0: 3e01 0000 0073 0a00 0000 0400 0c05 2801  >....s........(.
-00000f00: 160c 0c56                                ...V
+000001f0: 8d03 7c00 5f0d 7c01 a008 7409 6412 6405  ..|._.|...t.d.d.
+00000200: 8400 6413 6405 8400 6414 6415 6416 6405  ..d.d...d.d.d.d.
+00000210: 8400 6417 6418 8d06 6701 a101 0100 7c01  ..d.d...g.....|.
+00000220: 5300 2919 6113 0100 0045 6d69 7373 696f  S.).a....Emissio
+00000230: 6e73 2061 6e64 2074 656d 7065 7261 7475  ns and temperatu
+00000240: 7265 2065 7175 6174 696f 6e73 2061 6e64  re equations and
+00000250: 2063 6f6e 7374 7261 696e 7473 0a0a 2020   constraints..  
+00000260: 2020 4e65 6365 7373 6172 7920 7661 7269    Necessary vari
+00000270: 6162 6c65 733a 0a0a 2020 2020 5265 7475  ables:..    Retu
+00000280: 726e 733a 0a20 2020 2020 2020 206c 6973  rns:.        lis
+00000290: 7420 6f66 2063 6f6e 7374 7261 696e 7473  t of constraints
+000002a0: 2028 616e 7920 6f66 3a0a 2020 2020 2020   (any of:.      
+000002b0: 2020 2020 202d 2047 6c6f 6261 6c43 6f6e       - GlobalCon
+000002c0: 7374 7261 696e 740a 2020 2020 2020 2020  straint.        
+000002d0: 2020 202d 2047 6c6f 6261 6c49 6e69 7443     - GlobalInitC
+000002e0: 6f6e 7374 7261 696e 740a 2020 2020 2020  onstraint.      
+000002f0: 2020 2020 202d 2052 6567 696f 6e61 6c43       - RegionalC
+00000300: 6f6e 7374 7261 696e 740a 2020 2020 2020  onstraint.      
+00000310: 2020 2020 202d 2052 6567 696f 6e61 6c49       - RegionalI
+00000320: 6e69 7443 6f6e 7374 7261 696e 740a 2020  nitConstraint.  
+00000330: 2020 2020 2020 290a 2020 2020 2901 da06        ).    )...
+00000340: 7769 7468 696e 5a0f 6672 6163 7469 6f6e  withinZ.fraction
+00000350: 5f6f 665f 4744 5029 01da 0575 6e69 7473  _of_GDP)...units
+00000360: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00000370: 0004 0000 0053 0000 0073 2a00 0000 7c00  .....S...s*...|.
+00000380: 6a00 7c01 7c02 6602 1900 7c00 6a01 7c01  j.|.|.f...|.j.|.
+00000390: 7c02 6602 1900 1700 7c00 6a02 7c01 7c02  |.f.....|.j.|.|.
+000003a0: 6602 1900 1700 5300 a901 4e29 03da 1472  f.....S...N)...r
+000003b0: 656c 5f6d 6974 6967 6174 696f 6e5f 636f  el_mitigation_co
+000003c0: 7374 73da 0c64 616d 6167 655f 636f 7374  sts..damage_cost
+000003d0: 735a 1672 656c 5f66 696e 616e 6369 616c  sZ.rel_financial
+000003e0: 5f74 7261 6e73 6665 72a9 0372 0b00 0000  _transfer..r....
+000003f0: da01 74da 0172 a900 7215 0000 00fa 6443  ..t..r..r.....dC
+00000400: 3a5c 5573 6572 735c 3339 3033 3838 355c  :\Users\3903885\
+00000410: 4f6e 6544 7269 7665 202d 2055 6e69 7665  OneDrive - Unive
+00000420: 7273 6974 6569 7420 5574 7265 6368 745c  rsiteit Utrecht\
+00000430: 446f 6375 6d65 6e74 735c 4d49 4d4f 5341  Documents\MIMOSA
+00000440: 5c6d 696d 6f73 615c 636f 6d70 6f6e 656e  \mimosa\componen
+00000450: 7473 5c62 7572 6465 6e73 6861 7269 6e67  ts\burdensharing
+00000460: 2e70 79da 083c 6c61 6d62 6461 3e2b 0000  .py..<lambda>+..
+00000470: 0073 0a00 0000 0c00 0c01 02ff 0c02 04fe  .s..............
+00000480: 7a21 6765 745f 636f 6e73 7472 6169 6e74  z!get_constraint
+00000490: 732e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  s.<locals>.<lamb
+000004a0: 6461 3e63 0300 0000 0000 0000 0000 0000  da>c............
+000004b0: 0300 0000 0200 0000 5300 0000 f30a 0000  ........S.......
+000004c0: 007c 006a 007c 0119 0053 0072 0f00 0000  .|.j.|...S.r....
+000004d0: a901 da1b 6275 7264 656e 5f73 6861 7269  ....burden_shari
+000004e0: 6e67 5f63 6f6d 6d6f 6e5f 6c65 7665 6c72  ng_common_levelr
+000004f0: 1200 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000500: 0000 0072 1700 0000 2e00 0000 f302 0000  ...r............
+00000510: 000a 005a 2162 7572 6465 6e5f 7368 6172  ...Z!burden_shar
+00000520: 696e 675f 7265 6769 6d65 5f74 6f74 616c  ing_regime_total
+00000530: 5f63 6f73 7473 6303 0000 0000 0000 0000  _costsc.........
+00000540: 0000 0003 0000 0003 0000 0053 0000 0073  ...........S...s
+00000550: 1c00 0000 7400 7c00 6a01 8301 6401 6b03  ....t.|.j...d.k.
+00000560: 700d 7c00 a002 7c01 a101 6402 6b04 5300  p.|...|...d.k.S.
+00000570: 2903 4e5a 1165 7175 616c 5f74 6f74 616c  ).NZ.equal_total
+00000580: 5f63 6f73 7473 6934 0800 0029 0372 0a00  _costsi4...).r..
+00000590: 0000 da15 6275 7264 656e 5f73 6861 7269  ....burden_shari
+000005a0: 6e67 5f72 6567 696d 65da 0479 6561 7272  ng_regime..yearr
+000005b0: 1200 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+000005c0: 0000 0072 1700 0000 3000 0000 7308 0000  ...r....0...s...
+000005d0: 0008 0002 0104 ff0e 0229 01da 0969 676e  .........)...ign
+000005e0: 6f72 655f 6966 6303 0000 0000 0000 0000  ore_ifc.........
+000005f0: 0000 0003 0000 0003 0000 0053 0000 0073  ...........S...s
+00000600: 0e00 0000 7c00 6a00 7c01 7c02 6602 1900  ....|.j.|.|.f...
+00000610: 5300 720f 0000 0029 0172 1000 0000 7212  S.r....).r....r.
+00000620: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00000630: 0000 7217 0000 0036 0000 0073 0200 0000  ..r....6...s....
+00000640: 0e00 6303 0000 0000 0000 0000 0000 0003  ..c.............
+00000650: 0000 0002 0000 0053 0000 0072 1800 0000  .......S...r....
+00000660: 720f 0000 0072 1900 0000 7212 0000 0072  r....r....r....r
+00000670: 1500 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
+00000680: 0000 0037 0000 0072 1b00 0000 5a26 6275  ...7...r....Z&bu
+00000690: 7264 656e 5f73 6861 7269 6e67 5f72 6567  rden_sharing_reg
+000006a0: 696d 655f 6d69 7469 6761 7469 6f6e 5f63  ime_mitigation_c
+000006b0: 6f73 7473 6303 0000 0000 0000 0000 0000  ostsc...........
+000006c0: 0003 0000 0002 0000 0053 0000 0073 0e00  .........S...s..
+000006d0: 0000 7400 7c00 6a01 8301 6401 6b03 5300  ..t.|.j...d.k.S.
+000006e0: 2902 4e5a 1665 7175 616c 5f6d 6974 6967  ).NZ.equal_mitig
+000006f0: 6174 696f 6e5f 636f 7374 73a9 0272 0a00  ation_costs..r..
+00000700: 0000 721c 0000 0072 1200 0000 7215 0000  ..r....r....r...
+00000710: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000720: 3900 0000 7306 0000 0008 0002 0104 ff63  9...s..........c
+00000730: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000740: 0500 0000 1300 0000 732a 0000 0088 00a0  ........s*......
+00000750: 0088 00a0 0164 01a1 017c 01a1 0274 0287  .....d...|...t..
+00000760: 0066 0164 0264 0384 0888 006a 0344 0083  .f.d.d.....j.D..
+00000770: 0183 011b 0053 0029 044e 7201 0000 0063  .....S.).Nr....c
+00000780: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000790: 0600 0000 3300 0000 7322 0000 0081 007c  ....3...s".....|
+000007a0: 005d 0c7d 0188 00a0 0088 00a0 0164 00a1  .].}.........d..
+000007b0: 017c 01a1 0256 0001 0071 0264 0153 0029  .|...V...q.d.S.)
+000007c0: 0272 0100 0000 4e29 02da 1262 6173 656c  .r....N)...basel
+000007d0: 696e 655f 656d 6973 7369 6f6e 7372 1d00  ine_emissionsr..
+000007e0: 0000 a902 da02 2e30 da01 73a9 0172 0b00  .......0..s..r..
+000007f0: 0000 7215 0000 0072 1600 0000 da09 3c67  ..r....r......<g
+00000800: 656e 6578 7072 3e47 0000 00f3 0400 0000  enexpr>G........
+00000810: 0280 2000 fa34 6765 745f 636f 6e73 7472  .. ..4get_constr
+00000820: 6169 6e74 732e 3c6c 6f63 616c 733e 2e3c  aints.<locals>.<
+00000830: 6c61 6d62 6461 3e2e 3c6c 6f63 616c 733e  lambda>.<locals>
+00000840: 2e3c 6765 6e65 7870 723e 2904 7220 0000  .<genexpr>).r ..
+00000850: 0072 1d00 0000 da03 7375 6dda 0772 6567  .r......sum..reg
+00000860: 696f 6e73 2902 720b 0000 0072 1400 0000  ions).r....r....
+00000870: 7215 0000 0072 2400 0000 7216 0000 0072  r....r$...r....r
+00000880: 1700 0000 4600 0000 7306 0000 0010 0016  ....F...s.......
+00000890: 0104 ff29 01da 0a69 6e69 7469 616c 697a  ...)...initializ
+000008a0: 6569 0208 0000 6303 0000 0000 0000 0000  ei....c.........
+000008b0: 0000 0003 0000 0005 0000 0013 0000 0073  ...............s
+000008c0: 2c00 0000 8800 a000 8800 a001 8801 a101  ,...............
+000008d0: 7c02 a102 7402 8700 8701 6602 6401 6402  |...t.....f.d.d.
+000008e0: 8408 8800 6a03 4400 8301 8301 1b00 5300  ....j.D.......S.
+000008f0: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00000900: 0200 0000 0600 0000 3300 0000 7322 0000  ........3...s"..
+00000910: 0081 007c 005d 0c7d 0188 00a0 0088 00a0  ...|.].}........
+00000920: 0188 01a1 017c 01a1 0256 0001 0071 0264  .....|...V...q.d
+00000930: 0053 0072 0f00 0000 2902 da0a 706f 7075  .S.r....)...popu
+00000940: 6c61 7469 6f6e 721d 0000 0072 2100 0000  lationr....r!...
+00000950: a902 720b 0000 0072 1300 0000 7215 0000  ..r....r....r...
+00000960: 0072 1600 0000 7225 0000 004e 0000 0072  .r....r%...N...r
+00000970: 2600 0000 7227 0000 0029 0472 2b00 0000  &...r'...).r+...
+00000980: 721d 0000 0072 2800 0000 7229 0000 0072  r....r(...r)...r
+00000990: 1200 0000 7215 0000 0072 2c00 0000 7216  ....r....r,...r.
+000009a0: 0000 0072 1700 0000 4d00 0000 7306 0000  ...r....M...s...
+000009b0: 0010 0018 0104 ff63 0300 0000 0000 0000  .......c........
+000009c0: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
+000009d0: 7316 0000 0074 007c 007c 017c 0283 037c  s....t.|.|.|...|
+000009e0: 006a 017c 0119 0014 0053 0072 0f00 0000  .j.|.....S.r....
+000009f0: 2902 da15 7065 7263 6170 636f 6e76 5f73  )...percapconv_s
+00000a00: 6861 7265 5f72 756c 65da 1067 6c6f 6261  hare_rule..globa
+00000a10: 6c5f 656d 6973 7369 6f6e 7372 1200 0000  l_emissionsr....
+00000a20: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000a30: 1700 0000 5400 0000 7302 0000 0016 0063  ....T...s......c
+00000a40: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000a50: 0400 0000 5300 0000 731c 0000 007c 006a  ....S...s....|.j
+00000a60: 007c 017c 0266 0219 007c 006a 017c 017c  .|.|.f...|.j.|.|
+00000a70: 0266 0219 0018 0053 0072 0f00 0000 2902  .f.....S.r....).
+00000a80: da08 6261 7365 6c69 6e65 5a1c 7061 6964  ..baselineZ.paid
+00000a90: 5f66 6f72 5f65 6d69 7373 696f 6e5f 7265  _for_emission_re
+00000aa0: 6475 6374 696f 6e73 7212 0000 0072 1500  ductionsr....r..
+00000ab0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000ac0: 0055 0000 0073 0200 0000 1c00 4e67 7b14  .U...s......Ng{.
+00000ad0: ae47 e17a 843f 6303 0000 0000 0000 0000  .G.z.?c.........
+00000ae0: 0000 0003 0000 0002 0000 0053 0000 0073  ...........S...s
+00000af0: 1600 0000 7400 7c00 6a01 8301 6401 6b03  ....t.|.j...d.k.
+00000b00: 700a 7c01 6402 6b02 5300 2903 4e5a 1370  p.|.d.k.S.).NZ.p
+00000b10: 6572 5f63 6170 5f63 6f6e 7665 7267 656e  er_cap_convergen
+00000b20: 6365 7201 0000 0072 1f00 0000 7212 0000  cer....r....r...
+00000b30: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000b40: 7217 0000 0058 0000 0073 0800 0000 0800  r....X...s......
+00000b50: 0201 04ff 0802 5a0f 7065 7263 6170 636f  ......Z.percapco
+00000b60: 6e76 5f72 756c 6529 04da 0765 7073 696c  nv_rule)...epsil
+00000b70: 6f6e da10 6162 736f 6c75 7465 5f65 7073  on..absolute_eps
+00000b80: 696c 6f6e 721e 0000 00da 046e 616d 6529  ilonr......name)
+00000b90: 0e72 0500 0000 7208 0000 0072 1c00 0000  .r....r....r....
+00000ba0: 7204 0000 0072 1300 0000 7209 0000 00da  r....r....r.....
+00000bb0: 0475 6e69 7472 1a00 0000 da06 6578 7465  .unitr......exte
+00000bc0: 6e64 7207 0000 0072 2900 0000 da15 7065  ndr....r).....pe
+00000bd0: 7263 6170 636f 6e76 5f73 6861 7265 5f69  rcapconv_share_i
+00000be0: 6e69 74da 0f70 6572 6361 7063 6f6e 765f  nit..percapconv_
+00000bf0: 7965 6172 da14 7065 7263 6170 636f 6e76  year..percapconv
+00000c00: 5f73 6861 7265 5f70 6f70 2902 720b 0000  _share_pop).r...
+00000c10: 00da 0b63 6f6e 7374 7261 696e 7473 7215  ...constraintsr.
+00000c20: 0000 0072 1500 0000 7216 0000 00da 0f67  ...r....r......g
+00000c30: 6574 5f63 6f6e 7374 7261 696e 7473 1300  et_constraints..
+00000c40: 0000 7350 0000 0004 0d0c 0216 0304 0202  ..sP............
+00000c50: 0306 0106 0302 0106 0104 fa02 0b06 0106  ................
+00000c60: 0102 0106 0104 fc02 f304 ff02 1d04 0106  ................
+00000c70: 0108 fe0c 0502 0104 0104 0106 0108 fd04  ................
+00000c80: 0702 0206 0106 0102 0102 0106 0102 0304  ................
+00000c90: f802 ff04 ff04 0f72 3900 0000 6303 0000  .......r9...c...
+00000ca0: 0000 0000 0000 0000 0007 0000 0004 0000  ................
+00000cb0: 0043 0000 0073 8400 0000 7c00 a000 6401  .C...s....|...d.
+00000cc0: a101 7c00 a000 7c01 a101 0202 7d03 7d04  ..|...|.....}.}.
+00000cd0: 7c00 6a01 7d05 7c05 6402 7500 7217 7c00  |.j.}.|.d.u.r.|.
+00000ce0: 6a02 7c02 1900 5300 7c05 7c03 6b02 7222  j.|...S.|.|.k.r"
+00000cf0: 7c00 6a03 7c01 7c02 6602 1900 5300 7c04  |.j.|.|.f...S.|.
+00000d00: 7c03 1800 7c05 7c03 1800 1b00 7d06 7404  |...|.|.....}.t.
+00000d10: 7c06 6403 8302 7c00 6a03 7c01 7c02 6602  |.d...|.j.|.|.f.
+00000d20: 1900 1400 7405 6403 7c06 1800 6401 8302  ....t.d.|...d...
+00000d30: 7c00 6a02 7c02 1900 1400 1700 5300 2904  |.j.|.......S.).
+00000d40: 4e72 0100 0000 46e9 0100 0000 2906 721d  Nr....F.....).r.
+00000d50: 0000 0072 3600 0000 7235 0000 0072 3700  ...r6...r5...r7.
+00000d60: 0000 da03 6d69 6eda 036d 6178 2907 720b  ....min..max).r.
+00000d70: 0000 0072 1300 0000 7214 0000 005a 0679  ...r....r....Z.y
+00000d80: 6561 725f 305a 0679 6561 725f 745a 0979  ear_0Z.year_tZ.y
+00000d90: 6561 725f 636f 6e76 5a10 7965 6172 5f6c  ear_convZ.year_l
+00000da0: 696e 6561 725f 7061 7274 7215 0000 0072  inear_partr....r
+00000db0: 1500 0000 7216 0000 0072 2d00 0000 6300  ....r....r-...c.
+00000dc0: 0000 7316 0000 0016 0106 0108 020a 0208  ..s.............
+00000dd0: 010e 0210 0216 0316 0102 ff02 ff72 2d00  .............r-.
+00000de0: 0000 4e29 0eda 075f 5f64 6f63 5f5f da06  ..N)...__doc__..
+00000df0: 7479 7069 6e67 7202 0000 00da 0d6d 696d  typingr......mim
+00000e00: 6f73 612e 636f 6d6d 6f6e 7203 0000 0072  osa.commonr....r
+00000e10: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+00000e20: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+00000e30: 0000 7239 0000 0072 2d00 0000 7215 0000  ..r9...r-...r...
+00000e40: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000e50: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+00000e60: 0000 0004 000c 0528 0116 0c0c 50         .......(....P
```

### Comparing `mimosa-0.1.3/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 3697 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 710e 0000  o........6.dq...
+00000000: 6f0d 0d0a 0000 0000 e6b4 bb64 720e 0000  o..........dr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6404 6504 6405 6502 6507 1900 6604  ..d.e.d.e.e...f.
@@ -68,18 +68,18 @@
 00000430: 0003 0000 0006 0000 0053 0000 0073 1c00  .........S...s..
 00000440: 0000 7c00 6a00 7c02 1900 7c00 a001 7c00  ..|.j.|...|...|.
 00000450: a002 7c01 a101 7c02 a102 1400 5300 a901  ..|...|.....S...
 00000460: 4e29 03da 1869 6e69 745f 6361 7069 7461  N)...init_capita
 00000470: 6c73 746f 636b 5f66 6163 746f 72da 0347  lstock_factor..G
 00000480: 4450 da04 7965 6172 a903 720e 0000 00da  DP..year..r.....
 00000490: 0174 da01 72a9 0072 1900 0000 fa62 633a  .t..r..r.....bc:
-000004a0: 5c75 7365 7273 5c33 3930 3338 3835 5c6f  \users\3903885\o
-000004b0: 6e65 6472 6976 6520 2d20 756e 6976 6572  nedrive - univer
-000004c0: 7369 7465 6974 2075 7472 6563 6874 5c64  siteit utrecht\d
-000004d0: 6f63 756d 656e 7473 5c6d 696d 6f73 615c  ocuments\mimosa\
+000004a0: 5c55 7365 7273 5c33 3930 3338 3835 5c4f  \Users\3903885\O
+000004b0: 6e65 4472 6976 6520 2d20 556e 6976 6572  neDrive - Univer
+000004c0: 7369 7465 6974 2055 7472 6563 6874 5c44  siteit Utrecht\D
+000004d0: 6f63 756d 656e 7473 5c4d 494d 4f53 415c  ocuments\MIMOSA\
 000004e0: 6d69 6d6f 7361 5c63 6f6d 706f 6e65 6e74  mimosa\component
 000004f0: 735c 636f 6262 646f 7567 6c61 732e 7079  s\cobbdouglas.py
 00000500: da08 3c6c 616d 6264 613e 2b00 0000 7302  ..<lambda>+...s.
 00000510: 0000 001c 007a 2167 6574 5f63 6f6e 7374  .....z!get_const
 00000520: 7261 696e 7473 2e3c 6c6f 6361 6c73 3e2e  raints.<locals>.
 00000530: 3c6c 616d 6264 613e 2902 da0a 696e 6974  <lambda>)...init
 00000540: 6961 6c69 7a65 7211 0000 0063 0300 0000  ializer....c....
@@ -128,82 +128,82 @@
 000007f0: 8301 7319 7c00 6a04 7c01 7c02 6602 1900  ..s.|.j.|.|.f...
 00000800: 6e01 6402 1800 1400 7c00 6a05 7c01 7c02  n.d.....|.j.|.|.
 00000810: 6602 1900 1800 7c00 6a06 7c01 7c02 6602  f.....|.j.|.|.f.
 00000820: 1900 1800 6b02 5300 2903 4ee9 0100 0000  ....k.S.).N.....
 00000830: 7201 0000 0029 07da 0747 4450 5f6e 6574  r....)...GDP_net
 00000840: 7223 0000 0072 0a00 0000 da0e 6967 6e6f  r#...r......igno
 00000850: 7265 5f64 616d 6167 6573 da0c 6461 6d61  re_damages..dama
-00000860: 6765 5f63 6f73 7473 da0f 6162 6174 656d  ge_costs..abatem
-00000870: 656e 745f 636f 7374 73da 1266 696e 616e  ent_costs..finan
-00000880: 6369 616c 5f74 7261 6e73 6665 7272 1600  cial_transferr..
-00000890: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-000008a0: 0072 1b00 0000 5800 0000 7312 0000 000c  .r....X...s.....
-000008b0: 000c 011e 0102 ff0c 0202 fe0c 0302 fd04  ................
-000008c0: ff72 2c00 0000 6303 0000 0000 0000 0000  .r,...c.........
-000008d0: 0000 0003 0000 0005 0000 0053 0000 0073  ...........S...s
-000008e0: 2200 0000 7c00 6a00 7c01 7c02 6602 1900  "...|.j.|.|.f...
-000008f0: 7c00 6a01 7c00 6a02 7c01 7c02 6602 1900  |.j.|.j.|.|.f...
-00000900: 1400 6b02 5300 7212 0000 0029 03da 0b69  ..k.S.r....)...i
-00000910: 6e76 6573 746d 656e 7473 da02 7372 722c  nvestments..srr,
-00000920: 0000 0072 1600 0000 7219 0000 0072 1900  ...r....r....r..
-00000930: 0000 721a 0000 0072 1b00 0000 6000 0000  ..r....r....`...
-00000940: 7302 0000 0022 0072 3100 0000 6303 0000  s....".r1...c...
-00000950: 0000 0000 0000 0000 0003 0000 0005 0000  ................
-00000960: 0053 0000 0073 2600 0000 7c00 6a00 7c01  .S...s&...|.j.|.
-00000970: 7c02 6602 1900 6401 7c00 6a01 1800 7c00  |.f...d.|.j...|.
-00000980: 6a02 7c01 7c02 6602 1900 1400 6b02 5300  j.|.|.f.....k.S.
-00000990: 2902 4e72 2b00 0000 2903 da0b 636f 6e73  ).Nr+...)...cons
-000009a0: 756d 7074 696f 6e72 3200 0000 722c 0000  umptionr2...r,..
-000009b0: 0072 1600 0000 7219 0000 0072 1900 0000  .r....r....r....
-000009c0: 721a 0000 0072 1b00 0000 6400 0000 7302  r....r....d...s.
-000009d0: 0000 0026 0072 3300 0000 6303 0000 0000  ...&.r3...c.....
-000009e0: 0000 0000 0000 0003 0000 000a 0000 0053  ...............S
-000009f0: 0000 0073 5c00 0000 7c01 6401 6b04 722b  ...s\...|.d.k.r+
-00000a00: 7c00 6a00 7c01 7c02 6602 1900 7c00 6a00  |.j.|.|.f...|.j.
-00000a10: 7c01 6402 1800 7c02 6602 1900 7c00 6a01  |.d...|.f...|.j.
-00000a20: 7402 a003 7c00 6a00 7c01 7c02 6602 1900  t...|.j.|.|.f...
-00000a30: 7c00 6a04 7c00 6a05 7c01 7c02 6602 1900  |.j.|.j.|.|.f...
-00000a40: 7c00 6a01 a104 1400 1700 6b02 5300 7406  |.j.......k.S.t.
-00000a50: 6a07 5300 2903 4e72 0100 0000 722b 0000  j.S.).Nr....r+..
-00000a60: 0029 0872 2700 0000 da02 6474 720c 0000  .).r'.....dtr...
-00000a70: 00da 0963 616c 635f 644b 6474 da02 646b  ...calc_dKdt..dk
-00000a80: 7231 0000 0072 0900 0000 7229 0000 0072  r1...r....r)...r
-00000a90: 1600 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-00000aa0: 0000 0072 1b00 0000 6800 0000 7316 0000  ...r....h...s...
-00000ab0: 0008 080c f910 0104 0104 0120 0102 ff02  ........... ....
-00000ac0: ff02 ff04 ff06 0872 2700 0000 6302 0000  .......r'...c...
-00000ad0: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-00000ae0: 0053 0000 0073 2a00 0000 7c00 6a00 6401  .S...s*...|.j.d.
-00000af0: 7c01 6602 1900 7c00 6a01 7c01 1900 7c00  |.f...|.j.|...|.
-00000b00: a002 7c00 a003 6401 a101 7c01 a102 1400  ..|...d...|.....
-00000b10: 6b02 5300 721e 0000 0029 0472 2700 0000  k.S.r....).r'...
-00000b20: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00000b30: 2a00 0000 7219 0000 0072 1900 0000 721a  *...r....r....r.
-00000b40: 0000 0072 1b00 0000 7500 0000 7306 0000  ...r....u...s...
-00000b50: 000c 001a 0104 ff29 1372 0400 0000 da07  .......).r......
-00000b60: 7265 6769 6f6e 7372 0d00 0000 da04 756e  regionsr......un
-00000b70: 6974 7213 0000 0072 0500 0000 7217 0000  itr....r....r...
-00000b80: 0072 2700 0000 7228 0000 0072 3600 0000  .r'...r(...r6...
-00000b90: 7232 0000 0072 2300 0000 722c 0000 0072  r2...r#...r,...r
-00000ba0: 3100 0000 7233 0000 0072 2d00 0000 da06  1...r3...r-.....
-00000bb0: 6578 7465 6e64 7207 0000 0072 0800 0000  extendr....r....
-00000bc0: 2902 720e 0000 00da 0b63 6f6e 7374 7261  ).r......constra
-00000bd0: 696e 7473 7219 0000 0072 1900 0000 721a  intsr....r....r.
-00000be0: 0000 00da 0f67 6574 5f63 6f6e 7374 7261  .....get_constra
-00000bf0: 696e 7473 1600 0000 7370 0000 0004 0f16  ints....sp......
-00000c00: 0202 0104 0104 0106 0108 0108 fc08 0808  ................
-00000c10: 0108 0102 0204 0104 0106 0108 0108 fc02  ................
-00000c20: 0604 0104 0108 0106 0108 fc1a 061a 0108  ................
-00000c30: 0204 0302 0206 0102 0902 f602 0c08 0102  ................
-00000c40: ff02 0306 0102 0502 fa02 0806 0102 0102  ................
-00000c50: fe02 0406 0102 0102 fe02 0406 0102 0a02  ................
-00000c60: f502 0d06 0102 ff02 d304 ff04 3572 3b00  ............5r;.
-00000c70: 0000 4e29 10da 075f 5f64 6f63 5f5f da06  ..N)...__doc__..
-00000c80: 7479 7069 6e67 7202 0000 00da 0d6d 696d  typingr......mim
-00000c90: 6f73 612e 636f 6d6d 6f6e 7203 0000 0072  osa.commonr....r
-00000ca0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00000cb0: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00000cc0: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000cd0: 0072 3b00 0000 7219 0000 0072 1900 0000  .r;...r....r....
-00000ce0: 7219 0000 0072 1a00 0000 da08 3c6d 6f64  r....r......<mod
-00000cf0: 756c 653e 0100 0000 7308 0000 0004 000c  ule>....s.......
-00000d00: 0534 011a 0f                             .4...
+00000860: 6765 5f63 6f73 7473 da10 6d69 7469 6761  ge_costs..mitiga
+00000870: 7469 6f6e 5f63 6f73 7473 da12 6669 6e61  tion_costs..fina
+00000880: 6e63 6961 6c5f 7472 616e 7366 6572 7216  ncial_transferr.
+00000890: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+000008a0: 0000 721b 0000 0058 0000 0073 1200 0000  ..r....X...s....
+000008b0: 0c00 0c01 1e01 02ff 0c02 02fe 0c03 02fd  ................
+000008c0: 04ff 722c 0000 0063 0300 0000 0000 0000  ..r,...c........
+000008d0: 0000 0000 0300 0000 0500 0000 5300 0000  ............S...
+000008e0: 7322 0000 007c 006a 007c 017c 0266 0219  s"...|.j.|.|.f..
+000008f0: 007c 006a 017c 006a 027c 017c 0266 0219  .|.j.|.j.|.|.f..
+00000900: 0014 006b 0253 0072 1200 0000 2903 da0b  ...k.S.r....)...
+00000910: 696e 7665 7374 6d65 6e74 73da 0273 7272  investments..srr
+00000920: 2c00 0000 7216 0000 0072 1900 0000 7219  ,...r....r....r.
+00000930: 0000 0072 1a00 0000 721b 0000 0060 0000  ...r....r....`..
+00000940: 0073 0200 0000 2200 7231 0000 0063 0300  .s....".r1...c..
+00000950: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+00000960: 0000 5300 0000 7326 0000 007c 006a 007c  ..S...s&...|.j.|
+00000970: 017c 0266 0219 0064 017c 006a 0118 007c  .|.f...d.|.j...|
+00000980: 006a 027c 017c 0266 0219 0014 006b 0253  .j.|.|.f.....k.S
+00000990: 0029 024e 722b 0000 0029 03da 0b63 6f6e  .).Nr+...)...con
+000009a0: 7375 6d70 7469 6f6e 7232 0000 0072 2c00  sumptionr2...r,.
+000009b0: 0000 7216 0000 0072 1900 0000 7219 0000  ..r....r....r...
+000009c0: 0072 1a00 0000 721b 0000 0064 0000 0073  .r....r....d...s
+000009d0: 0200 0000 2600 7233 0000 0063 0300 0000  ....&.r3...c....
+000009e0: 0000 0000 0000 0000 0300 0000 0a00 0000  ................
+000009f0: 5300 0000 735c 0000 007c 0164 016b 0472  S...s\...|.d.k.r
+00000a00: 2b7c 006a 007c 017c 0266 0219 007c 006a  +|.j.|.|.f...|.j
+00000a10: 007c 0164 0218 007c 0266 0219 007c 006a  .|.d...|.f...|.j
+00000a20: 0174 02a0 037c 006a 007c 017c 0266 0219  .t...|.j.|.|.f..
+00000a30: 007c 006a 047c 006a 057c 017c 0266 0219  .|.j.|.j.|.|.f..
+00000a40: 007c 006a 01a1 0414 0017 006b 0253 0074  .|.j.......k.S.t
+00000a50: 066a 0753 0029 034e 7201 0000 0072 2b00  .j.S.).Nr....r+.
+00000a60: 0000 2908 7227 0000 00da 0264 7472 0c00  ..).r'.....dtr..
+00000a70: 0000 da09 6361 6c63 5f64 4b64 74da 0264  ....calc_dKdt..d
+00000a80: 6b72 3100 0000 7209 0000 0072 2900 0000  kr1...r....r)...
+00000a90: 7216 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000aa0: 1a00 0000 721b 0000 0068 0000 0073 1600  ....r....h...s..
+00000ab0: 0000 0808 0cf9 1001 0401 0401 2001 02ff  ............ ...
+00000ac0: 02ff 02ff 04ff 0608 7227 0000 0063 0200  ........r'...c..
+00000ad0: 0000 0000 0000 0000 0000 0200 0000 0700  ................
+00000ae0: 0000 5300 0000 732a 0000 007c 006a 0064  ..S...s*...|.j.d
+00000af0: 017c 0166 0219 007c 006a 017c 0119 007c  .|.f...|.j.|...|
+00000b00: 00a0 027c 00a0 0364 01a1 017c 01a1 0214  ...|...d...|....
+00000b10: 006b 0253 0072 1e00 0000 2904 7227 0000  .k.S.r....).r'..
+00000b20: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000b30: 722a 0000 0072 1900 0000 7219 0000 0072  r*...r....r....r
+00000b40: 1a00 0000 721b 0000 0075 0000 0073 0600  ....r....u...s..
+00000b50: 0000 0c00 1a01 04ff 2913 7204 0000 00da  ........).r.....
+00000b60: 0772 6567 696f 6e73 720d 0000 00da 0475  .regionsr......u
+00000b70: 6e69 7472 1300 0000 7205 0000 0072 1700  nitr....r....r..
+00000b80: 0000 7227 0000 0072 2800 0000 7236 0000  ..r'...r(...r6..
+00000b90: 0072 3200 0000 7223 0000 0072 2c00 0000  .r2...r#...r,...
+00000ba0: 7231 0000 0072 3300 0000 722d 0000 00da  r1...r3...r-....
+00000bb0: 0665 7874 656e 6472 0700 0000 7208 0000  .extendr....r...
+00000bc0: 0029 0272 0e00 0000 da0b 636f 6e73 7472  .).r......constr
+00000bd0: 6169 6e74 7372 1900 0000 7219 0000 0072  aintsr....r....r
+00000be0: 1a00 0000 da0f 6765 745f 636f 6e73 7472  ......get_constr
+00000bf0: 6169 6e74 7316 0000 0073 7000 0000 040f  aints....sp.....
+00000c00: 1602 0201 0401 0401 0601 0801 08fc 0808  ................
+00000c10: 0801 0801 0202 0401 0401 0601 0801 08fc  ................
+00000c20: 0206 0401 0401 0801 0601 08fc 1a06 1a01  ................
+00000c30: 0802 0403 0202 0601 0209 02f6 020c 0801  ................
+00000c40: 02ff 0203 0601 0205 02fa 0208 0601 0201  ................
+00000c50: 02fe 0204 0601 0201 02fe 0204 0601 020a  ................
+00000c60: 02f5 020d 0601 02ff 02d3 04ff 0435 723b  .............5r;
+00000c70: 0000 004e 2910 da07 5f5f 646f 635f 5fda  ...N)...__doc__.
+00000c80: 0674 7970 696e 6772 0200 0000 da0d 6d69  .typingr......mi
+00000c90: 6d6f 7361 2e63 6f6d 6d6f 6e72 0300 0000  mosa.commonr....
+00000ca0: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00000cb0: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
+00000cc0: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000cd0: 0000 723b 0000 0072 1900 0000 7219 0000  ..r;...r....r...
+00000ce0: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
+00000cf0: 6475 6c65 3e01 0000 0073 0800 0000 0400  dule>....s......
+00000d00: 0c05 3401 1a0f                           ..4...
```

### Comparing `mimosa-0.1.3/mimosa/components/__pycache__/emissions.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/__pycache__/emissions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 10151 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 a727 0000  o........6.d.'..
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 a727 0000  o........i.d.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6404 6504 6405 6502 6507 1900 6604  ..d.e.d.e.e...f.
@@ -91,18 +91,18 @@
 000005a0: 01da 0575 6e69 7473 6303 0000 0000 0000  ...unitsc.......
 000005b0: 0000 0000 0003 0000 0005 0000 0053 0000  .............S..
 000005c0: 0073 1200 0000 7c00 a000 7c00 a001 7c01  .s....|...|...|.
 000005d0: a101 7c02 a102 5300 a901 4ea9 02da 1262  ..|...S...N....b
 000005e0: 6173 656c 696e 655f 656d 6973 7369 6f6e  aseline_emission
 000005f0: 73da 0479 6561 72a9 0372 0e00 0000 da01  s..year..r......
 00000600: 74da 0172 a900 7219 0000 00fa 6063 3a5c  t..r..r.....`c:\
-00000610: 7573 6572 735c 3339 3033 3838 355c 6f6e  users\3903885\on
-00000620: 6564 7269 7665 202d 2075 6e69 7665 7273  edrive - univers
-00000630: 6974 6569 7420 7574 7265 6368 745c 646f  iteit utrecht\do
-00000640: 6375 6d65 6e74 735c 6d69 6d6f 7361 5c6d  cuments\mimosa\m
+00000610: 5573 6572 735c 3339 3033 3838 355c 4f6e  Users\3903885\On
+00000620: 6544 7269 7665 202d 2055 6e69 7665 7273  eDrive - Univers
+00000630: 6974 6569 7420 5574 7265 6368 745c 446f  iteit Utrecht\Do
+00000640: 6375 6d65 6e74 735c 4d49 4d4f 5341 5c6d  cuments\MIMOSA\m
 00000650: 696d 6f73 615c 636f 6d70 6f6e 656e 7473  imosa\components
 00000660: 5c65 6d69 7373 696f 6e73 2e70 79da 083c  \emissions.py..<
 00000670: 6c61 6d62 6461 3e2d 0000 0073 0200 0000  lambda>-...s....
 00000680: 1200 7a21 6765 745f 636f 6e73 7472 6169  ..z!get_constrai
 00000690: 6e74 732e 3c6c 6f63 616c 733e 2e3c 6c61  nts.<locals>.<la
 000006a0: 6d62 6461 3e29 02da 0a69 6e69 7469 616c  mbda>)...initial
 000006b0: 697a 6572 1100 0000 7201 0000 0029 0272  izer....r....).r
```

### Comparing `mimosa-0.1.3/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 4213 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 7510 0000  o........6.du...
+00000000: 6f0d 0d0a 0000 0000 b769 ba64 7510 0000  o........i.du...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6404 6504 6405  m.Z.m.Z...d.e.d.
 00000070: 6502 6507 1900 6604 6406 6407 8404 5a0d  e.e...f.d.d...Z.
@@ -71,19 +71,19 @@
 00000460: 0019 007c 006a 027c 0164 0218 0019 007c  ...|.j.|.d.....|
 00000470: 0083 036b 0253 0074 036a 0453 00a9 034e  ...k.S.t.j.S...N
 00000480: 7201 0000 00e9 0100 0000 2905 da0b 736c  r.........)...sl
 00000490: 725f 7468 6572 6d61 6cda 1573 6c72 5f74  r_thermal..slr_t
 000004a0: 6865 726d 616c 5f65 7870 616e 7369 6f6e  hermal_expansion
 000004b0: da0b 7465 6d70 6572 6174 7572 6572 0900  ..temperaturer..
 000004c0: 0000 da04 536b 6970 a902 720c 0000 00da  ....Skip..r.....
-000004d0: 0174 a900 7219 0000 00fa 6363 3a5c 7573  .t..r.....cc:\us
-000004e0: 6572 735c 3339 3033 3838 355c 6f6e 6564  ers\3903885\oned
-000004f0: 7269 7665 202d 2075 6e69 7665 7273 6974  rive - universit
-00000500: 6569 7420 7574 7265 6368 745c 646f 6375  eit utrecht\docu
-00000510: 6d65 6e74 735c 6d69 6d6f 7361 5c6d 696d  ments\mimosa\mim
+000004d0: 0174 a900 7219 0000 00fa 6363 3a5c 5573  .t..r.....cc:\Us
+000004e0: 6572 735c 3339 3033 3838 355c 4f6e 6544  ers\3903885\OneD
+000004f0: 7269 7665 202d 2055 6e69 7665 7273 6974  rive - Universit
+00000500: 6569 7420 5574 7265 6368 745c 446f 6375  eit Utrecht\Docu
+00000510: 6d65 6e74 735c 4d49 4d4f 5341 5c6d 696d  ments\MIMOSA\mim
 00000520: 6f73 615c 636f 6d70 6f6e 656e 7473 5c73  osa\components\s
 00000530: 6561 6c65 7665 6c72 6973 652e 7079 da08  ealevelrise.py..
 00000540: 3c6c 616d 6264 613e 3a00 0000 f30a 0000  <lambda>:.......
 00000550: 0008 0208 fe1e 0104 ff06 037a 2167 6574  ...........z!get
 00000560: 5f63 6f6e 7374 7261 696e 7473 2e3c 6c6f  _constraints.<lo
 00000570: 6361 6c73 3e2e 3c6c 616d 6264 613e 5a0b  cals>.<lambda>Z.
 00000580: 534c 525f 7468 6572 6d61 6c29 01da 046e  SLR_thermal)...n
```

### Comparing `mimosa-0.1.3/mimosa/components/abatement.py` & `mimosa-0.1.4/mimosa/components/mitigation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Model equations and constraints:
-Abatement costs
+Mitigation costs
 """
 
 from typing import Sequence
 from mimosa.common import (
     AbstractModel,
     Param,
     Var,
@@ -18,18 +18,18 @@
     soft_min,
     NonNegativeReals,
     quant,
 )
 
 
 def get_constraints(m: AbstractModel) -> Sequence[GeneralConstraint]:
-    """Abatement cost equations and constraints
+    """Mitigation cost equations and constraints
 
     Necessary variables:
-        m.abatement_costs
+        m.mitigation_costs
 
     Returns:
         list of constraints (any of:
            - GlobalConstraint
            - GlobalInitConstraint
            - RegionalConstraint
            - RegionalInitConstraint
@@ -73,65 +73,65 @@
                 lambda m, t: m.learning_factor[t]
                 == (m.LBD_factor[t] * m.LOT_factor[t]),
                 "learning",
             ),
         ]
     )
 
-    # Abatement costs and MAC
-    m.abatement_costs = Var(
+    # Mitigation costs and MAC
+    m.mitigation_costs = Var(
         m.t,
         m.regions,
         # within=NonNegativeReals,
         initialize=0,
         units=quant.unit("currency_unit"),
     )
-    m.rel_abatement_costs = Var(m.t, m.regions, units=quant.unit("fraction_of_GDP"))
+    m.rel_mitigation_costs = Var(m.t, m.regions, units=quant.unit("fraction_of_GDP"))
     m.MAC_gamma = Param()
     m.MAC_beta = Param()
     m.MAC_scaling_factor = Param(m.regions)  # Regional scaling of the MAC
     m.carbonprice = Var(
         m.t,
         m.regions,
         bounds=lambda m: (0, 2 * m.MAC_gamma),
         units=quant.unit("currency_unit/emissions_unit"),
     )
-    m.rel_abatement_costs_min_level = Param()
+    m.rel_mitigation_costs_min_level = Param()
     constraints.extend(
         [
             RegionalConstraint(
-                lambda m, t, r: m.rel_abatement_costs[t, r]
-                == m.abatement_costs[t, r] / m.GDP_gross[t, r],
-                "rel_abatement_costs",
+                lambda m, t, r: m.rel_mitigation_costs[t, r]
+                == m.mitigation_costs[t, r] / m.GDP_gross[t, r],
+                "rel_mitigation_costs",
             ),
             RegionalConstraint(
-                lambda m, t, r: m.rel_abatement_costs[t, r]
-                >= (m.rel_abatement_costs_min_level if t > 0 else 0.0),
-                "rel_abatement_costs_non_negative",
+                lambda m, t, r: m.rel_mitigation_costs[t, r]
+                >= (m.rel_mitigation_costs_min_level if t > 0 else 0.0),
+                "rel_mitigation_costs_non_negative",
             ),
             RegionalConstraint(
                 lambda m, t, r: m.carbonprice[t, r]
                 == MAC(m.relative_abatement[t, r], m, t, r),
                 "carbonprice",
             ),
             RegionalInitConstraint(
                 lambda m, r: m.carbonprice[0, r] == 0, "init_carbon_price"
             ),
         ]
     )
 
     # Keep track of relative global costs
-    m.global_rel_abatement_costs = Var(m.t)
+    m.global_rel_mitigation_costs = Var(m.t)
     constraints.extend(
         [
             GlobalConstraint(
-                lambda m, t: m.global_rel_abatement_costs[t]
-                == sum(m.abatement_costs[t, r] for r in m.regions)
+                lambda m, t: m.global_rel_mitigation_costs[t]
+                == sum(m.mitigation_costs[t, r] for r in m.regions)
                 / sum(m.GDP_gross[t, r] for r in m.regions),
-                "global_rel_abatement_costs",
+                "global_rel_mitigation_costs",
             )
         ]
     )
 
     # Calculate average global emission reduction per cost unit
     # and average cost per unit emission reduction
 
@@ -142,22 +142,22 @@
         m.t, units=quant.unit("currency_unit / emissionsrate_unit")
     )
     constraints.extend(
         [
             GlobalConstraint(
                 lambda m, t: m.global_emission_reduction_per_cost_unit[t]
                 == sum(m.regional_emission_reduction[t, r] for r in m.regions)
-                / soft_min(sum(m.abatement_costs[t, r] for r in m.regions))
+                / soft_min(sum(m.mitigation_costs[t, r] for r in m.regions))
                 if t > 0
                 else Constraint.Skip,
                 "global_emission_reduction_per_cost_unit",
             ),
             GlobalConstraint(
                 lambda m, t: m.global_cost_per_emission_reduction_unit[t]
-                == sum(m.abatement_costs[t, r] for r in m.regions)
+                == sum(m.mitigation_costs[t, r] for r in m.regions)
                 / soft_min(sum(m.regional_emission_reduction[t, r] for r in m.regions))
                 if t > 0
                 else Constraint.Skip,
                 "global_cost_per_emission_reduction_unit",
             ),
         ]
     )
```

### Comparing `mimosa-0.1.3/mimosa/components/burdensharing.py` & `mimosa-0.1.4/mimosa/components/burdensharing.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,32 +34,32 @@
     m.burden_sharing_regime = Param(within=Any)
 
     ## Burden sharing scheme:
     m.burden_sharing_common_level = Var(m.t, units=quant.unit("fraction_of_GDP"))
 
     constraints.extend(
         [
-            # Total costs: abatement + damage costs should be equal among regions as % GDP
+            # Total costs: mitigation + damage costs should be equal among regions as % GDP
             RegionalSoftEqualityConstraint(
-                lambda m, t, r: m.rel_abatement_costs[t, r]
+                lambda m, t, r: m.rel_mitigation_costs[t, r]
                 + m.damage_costs[t, r]
                 + m.rel_financial_transfer[t, r],
                 lambda m, t, r: m.burden_sharing_common_level[t],
                 "burden_sharing_regime_total_costs",
                 ignore_if=lambda m, t, r: value(m.burden_sharing_regime)
                 != "equal_total_costs"
                 or m.year(t) > 2100,
             ),
-            # Abatement costs: abatement costs should be equal among regions as % GDP
+            # Mitigation costs: mitigation costs should be equal among regions as % GDP
             RegionalSoftEqualityConstraint(
-                lambda m, t, r: m.rel_abatement_costs[t, r],
+                lambda m, t, r: m.rel_mitigation_costs[t, r],
                 lambda m, t, r: m.burden_sharing_common_level[t],
-                "burden_sharing_regime_abatement_costs",
+                "burden_sharing_regime_mitigation_costs",
                 ignore_if=lambda m, t, r: value(m.burden_sharing_regime)
-                != "equal_abatement_costs"
+                != "equal_mitigation_costs"
                 # or m.year(t) > 2125,
             ),
         ]
     )
 
     ## Per capita convergence:
     # m.regional_per_cap_emissions = Var(
@@ -74,20 +74,14 @@
     m.percapconv_share_pop = Param(
         m.t,
         m.regions,
         initialize=lambda m, t, r: m.population(m.year(t), r)
         / sum(m.population(m.year(t), s) for s in m.regions),
     )
 
-    m.percapconv_emission_share = Var(
-        m.t, m.regions  # , initialize=_percapconv_share_rule
-    )
-    m.percapconv_import_export_emission_reduction_balance = Var(
-        m.t, m.regions, units=quant.unit("emissionsrate_unit")
-    )
     constraints.extend(
         [
             RegionalSoftEqualityConstraint(
                 lambda m, t, r: percapconv_share_rule(m, t, r) * m.global_emissions[t],
                 lambda m, t, r: m.baseline[t, r] - m.paid_for_emission_reductions[t, r],
                 epsilon=None,
                 absolute_epsilon=0.01,
```

### Comparing `mimosa-0.1.3/mimosa/components/cobbdouglas.py` & `mimosa-0.1.4/mimosa/components/cobbdouglas.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             RegionalInitConstraint(
                 lambda m, r: m.GDP_gross[0, r] == m.GDP(m.year(0), r), "GDP_gross_init"
             ),
             RegionalConstraint(
                 lambda m, t, r: m.GDP_net[t, r]
                 == m.GDP_gross[t, r]
                 * (1 - (m.damage_costs[t, r] if not value(m.ignore_damages) else 0))
-                - m.abatement_costs[t, r]
+                - m.mitigation_costs[t, r]
                 - m.financial_transfer[t, r],
                 "GDP_net",
             ),
             RegionalConstraint(
                 lambda m, t, r: m.investments[t, r] == m.sr * m.GDP_net[t, r],
                 "investments",
             ),
```

### Comparing `mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:45 2023 UTC, .py size: 5331 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b936 ba64 d314 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 d314 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6404  m.Z.m.Z.m.Z...d.
 00000070: 6504 6405 6502 6507 1900 6604 6406 6407  e.d.e.e...f.d.d.
@@ -77,19 +77,19 @@
 000004c0: 006a 007c 0119 0074 007c 017c 006a 017c  .j.|...t.|.|.j.|
 000004d0: 006a 027c 006a 0383 046b 0253 00a9 014e  .j.|.j...k.S...N
 000004e0: 2904 da0f 736d 6f6f 7468 6564 5f66 6163  )...smoothed_fac
 000004f0: 746f 72da 0b74 656d 7065 7261 7475 7265  tor..temperature
 00000500: da02 6474 da17 7065 7263 5f72 6576 6572  ..dt..perc_rever
 00000510: 7369 626c 655f 6461 6d61 6765 7329 0272  sible_damages).r
 00000520: 0d00 0000 da01 74a9 0072 1700 0000 fa6a  ......t..r.....j
-00000530: 633a 5c75 7365 7273 5c33 3930 3338 3835  c:\users\3903885
-00000540: 5c6f 6e65 6472 6976 6520 2d20 756e 6976  \onedrive - univ
-00000550: 6572 7369 7465 6974 2075 7472 6563 6874  ersiteit utrecht
-00000560: 5c64 6f63 756d 656e 7473 5c6d 696d 6f73  \documents\mimos
-00000570: 615c 6d69 6d6f 7361 5c63 6f6d 706f 6e65  a\mimosa\compone
+00000530: 633a 5c55 7365 7273 5c33 3930 3338 3835  c:\Users\3903885
+00000540: 5c4f 6e65 4472 6976 6520 2d20 556e 6976  \OneDrive - Univ
+00000550: 6572 7369 7465 6974 2055 7472 6563 6874  ersiteit Utrecht
+00000560: 5c44 6f63 756d 656e 7473 5c4d 494d 4f53  \Documents\MIMOS
+00000570: 415c 6d69 6d6f 7361 5c63 6f6d 706f 6e65  A\mimosa\compone
 00000580: 6e74 735c 6461 6d61 6765 735c 6164 5f72  nts\damages\ad_r
 00000590: 6963 6532 3031 302e 7079 da08 3c6c 616d  ice2010.py..<lam
 000005a0: 6264 613e 3a00 0000 7306 0000 0008 0012  bda>:...s.......
 000005b0: 0104 ff7a 2167 6574 5f63 6f6e 7374 7261  ...z!get_constra
 000005c0: 696e 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c  ints.<locals>.<l
 000005d0: 616d 6264 613e 7212 0000 0029 01da 046e  ambda>r....)...n
 000005e0: 616d 6563 0300 0000 0000 0000 0000 0000  amec............
```

### Comparing `mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:45 2023 UTC, .py size: 4874 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b936 ba64 0a13 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 0a13 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6404 6504 6405  m.Z.m.Z...d.e.d.
 00000070: 6502 6507 1900 6604 6406 6407 8404 5a0d  e.e...f.d.d...Z.
@@ -89,19 +89,19 @@
 00000580: 006a 047c 0219 007c 006a 057c 0219 0083  .j.|...|.j.|....
 00000590: 056b 0253 00a9 024e 7201 0000 0029 06da  .k.S...Nr....)..
 000005a0: 0b53 4c52 5f64 616d 6167 6573 da0b 736c  .SLR_damages..sl
 000005b0: 725f 6461 6d61 6765 73da 0974 6f74 616c  r_damages..total
 000005c0: 5f53 4c52 da09 4744 505f 6772 6f73 73da  _SLR..GDP_gross.
 000005d0: 0753 4c52 6461 6d31 da07 534c 5264 616d  .SLRdam1..SLRdam
 000005e0: 32a9 0372 0c00 0000 da01 74da 0172 a900  2..r......t..r..
-000005f0: 721b 0000 00fa 6a63 3a5c 7573 6572 735c  r.....jc:\users\
-00000600: 3339 3033 3838 355c 6f6e 6564 7269 7665  3903885\onedrive
-00000610: 202d 2075 6e69 7665 7273 6974 6569 7420   - universiteit 
-00000620: 7574 7265 6368 745c 646f 6375 6d65 6e74  utrecht\document
-00000630: 735c 6d69 6d6f 7361 5c6d 696d 6f73 615c  s\mimosa\mimosa\
+000005f0: 721b 0000 00fa 6a63 3a5c 5573 6572 735c  r.....jc:\Users\
+00000600: 3339 3033 3838 355c 4f6e 6544 7269 7665  3903885\OneDrive
+00000610: 202d 2055 6e69 7665 7273 6974 6569 7420   - Universiteit 
+00000620: 5574 7265 6368 745c 446f 6375 6d65 6e74  Utrecht\Document
+00000630: 735c 4d49 4d4f 5341 5c6d 696d 6f73 615c  s\MIMOSA\mimosa\
 00000640: 636f 6d70 6f6e 656e 7473 5c64 616d 6167  components\damag
 00000650: 6573 5c61 645f 7269 6365 3230 3132 2e70  es\ad_rice2012.p
 00000660: 79da 083c 6c61 6d62 6461 3e42 0000 0073  y..<lambda>B...s
 00000670: 1200 0000 0c00 0201 0801 0c01 0c01 0801  ................
 00000680: 0801 02fb 04ff 7a21 6765 745f 636f 6e73  ......z!get_cons
 00000690: 7472 6169 6e74 732e 3c6c 6f63 616c 733e  traints.<locals>
 000006a0: 2e3c 6c61 6d62 6461 3e72 1200 0000 6303  .<lambda>r....c.
```

### Comparing `mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:46 2023 UTC, .py size: 6688 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ba36 ba64 201a 0000  o........6.d ...
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 201a 0000  o........i.d ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6404  m.Z.m.Z.m.Z...d.
 00000060: 6504 6405 6502 6507 1900 6604 6406 6407  e.d.e.e...f.d.d.
 00000070: 8404 5a0a 6408 6409 8400 5a0b 640a 640b  ..Z.d.d...Z.d.d.
@@ -83,18 +83,18 @@
 00000520: 6a04 7c00 7c02 8305 1400 6b02 5300 a902  j.|.|.....k.S...
 00000530: 4e72 0100 0000 2905 da0d 6772 6f73 735f  Nr....)...gross_
 00000540: 6461 6d61 6765 73da 1364 616d 6167 655f  damages..damage_
 00000550: 7363 616c 655f 6661 6374 6f72 da0a 6461  scale_factor..da
 00000560: 6d61 6765 5f66 6374 da0b 7465 6d70 6572  mage_fct..temper
 00000570: 6174 7572 65da 0254 30a9 0372 0900 0000  ature..T0..r....
 00000580: da01 74da 0172 a900 7215 0000 00fa 6763  ..t..r..r.....gc
-00000590: 3a5c 7573 6572 735c 3339 3033 3838 355c  :\users\3903885\
-000005a0: 6f6e 6564 7269 7665 202d 2075 6e69 7665  onedrive - unive
-000005b0: 7273 6974 6569 7420 7574 7265 6368 745c  rsiteit utrecht\
-000005c0: 646f 6375 6d65 6e74 735c 6d69 6d6f 7361  documents\mimosa
+00000590: 3a5c 5573 6572 735c 3339 3033 3838 355c  :\Users\3903885\
+000005a0: 4f6e 6544 7269 7665 202d 2055 6e69 7665  OneDrive - Unive
+000005b0: 7273 6974 6569 7420 5574 7265 6368 745c  rsiteit Utrecht\
+000005c0: 446f 6375 6d65 6e74 735c 4d49 4d4f 5341  Documents\MIMOSA
 000005d0: 5c6d 696d 6f73 615c 636f 6d70 6f6e 656e  \mimosa\componen
 000005e0: 7473 5c64 616d 6167 6573 5c61 645f 7769  ts\damages\ad_wi
 000005f0: 7463 682e 7079 da08 3c6c 616d 6264 613e  tch.py..<lambda>
 00000600: 3900 0000 7306 0000 000c 001c 0104 ff7a  9...s..........z
 00000610: 2167 6574 5f63 6f6e 7374 7261 696e 7473  !get_constraints
 00000620: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
 00000630: 613e 720d 0000 0063 0300 0000 0000 0000  a>r....c........
```

### Comparing `mimosa-0.1.3/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:45 2023 UTC, .py size: 4260 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b936 ba64 a410 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 39e5 ba64 d410 0000  o.......9..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6404  m.Z.m.Z.m.Z...d.
 00000070: 6504 6405 6502 6507 1900 6604 6406 6407  e.d.e.e...f.d.d.
@@ -72,134 +72,135 @@
 00000470: 01da 0677 6974 6869 6e63 0300 0000 0000  ...withinc......
 00000480: 0000 0000 0000 0300 0000 0900 0000 5300  ..............S.
 00000490: 0000 7336 0000 007c 006a 007c 017c 0266  ..s6...|.j.|.|.f
 000004a0: 0219 007c 006a 0174 027c 006a 037c 0119  ...|.j.t.|.j.|..
 000004b0: 0064 0118 007c 006a 0464 0118 007c 007c  .d...|.j.d...|.|
 000004c0: 0264 0264 038d 0514 006b 0253 0029 044e  .d.d.....k.S.).N
 000004d0: 6733 3333 3333 33e3 3f46 a901 da06 6973  g333333.?F....is
-000004e0: 5f73 6c72 2905 da0d 7265 7369 645f 6461  _slr)...resid_da
-000004f0: 6d61 6765 73da 1364 616d 6167 655f 7363  mages..damage_sc
-00000500: 616c 655f 6661 6374 6f72 da0a 6461 6d61  ale_factor..dama
-00000510: 6765 5f66 6374 da0b 7465 6d70 6572 6174  ge_fct..temperat
-00000520: 7572 65da 0254 30a9 0372 0d00 0000 da01  ure..T0..r......
-00000530: 74da 0172 a900 721c 0000 00fa 6563 3a5c  t..r..r.....ec:\
-00000540: 7573 6572 735c 3339 3033 3838 355c 6f6e  users\3903885\on
-00000550: 6564 7269 7665 202d 2075 6e69 7665 7273  edrive - univers
-00000560: 6974 6569 7420 7574 7265 6368 745c 646f  iteit utrecht\do
-00000570: 6375 6d65 6e74 735c 6d69 6d6f 7361 5c6d  cuments\mimosa\m
-00000580: 696d 6f73 615c 636f 6d70 6f6e 656e 7473  imosa\components
-00000590: 5c64 616d 6167 6573 5c63 6f61 6363 682e  \damages\coacch.
-000005a0: 7079 da08 3c6c 616d 6264 613e 3800 0000  py..<lambda>8...
-000005b0: 730a 0000 000c 0004 0120 0102 ff04 ff7a  s........ .....z
-000005c0: 2167 6574 5f63 6f6e 7374 7261 696e 7473  !get_constraints
-000005d0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-000005e0: 613e 7214 0000 0029 0267 0000 0000 0000  a>r....).g......
-000005f0: e0bf 6766 6666 6666 66e6 3f29 02da 0662  ..gffffff.?)...b
-00000600: 6f75 6e64 7372 1000 0000 6303 0000 0000  oundsr....c.....
-00000610: 0000 0000 0000 0003 0000 0009 0000 0053  ...............S
-00000620: 0000 0073 3200 0000 7c00 6a00 7c01 7c02  ...s2...|.j.|.|.
-00000630: 6602 1900 7c00 6a01 7402 7c00 6a03 7c01  f...|.j.t.|.j.|.
-00000640: 1900 7c00 6a03 6401 1900 7c00 7c02 6402  ..|.j.d...|.|.d.
-00000650: 6403 8d05 1400 6b02 5300 2904 4e72 0100  d.....k.S.).Nr..
-00000660: 0000 5472 1200 0000 2904 da0b 534c 525f  ..Tr....)...SLR_
-00000670: 6461 6d61 6765 7372 1500 0000 7216 0000  damagesr....r...
-00000680: 00da 0974 6f74 616c 5f53 4c52 7219 0000  ...total_SLRr...
-00000690: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-000006a0: 721e 0000 0053 0000 0073 0a00 0000 0c00  r....S...s......
-000006b0: 0401 1c01 02ff 04ff 7220 0000 0063 0300  ........r ...c..
-000006c0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-000006d0: 0000 5300 0000 732a 0000 007c 006a 007c  ..S...s*...|.j.|
-000006e0: 017c 0266 0219 007c 006a 017c 017c 0266  .|.f...|.j.|.|.f
-000006f0: 0219 007c 006a 027c 017c 0266 0219 0017  ...|.j.|.|.f....
-00000700: 006b 0253 00a9 014e 2903 da0c 6461 6d61  .k.S...N)...dama
-00000710: 6765 5f63 6f73 7473 7214 0000 0072 2000  ge_costsr....r .
-00000720: 0000 7219 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-00000730: 0072 1d00 0000 721e 0000 005d 0000 0073  .r....r....]...s
-00000740: 0600 0000 0c00 1a01 04ff 7223 0000 0029  ..........r#...)
-00000750: 1772 0500 0000 721a 0000 00da 0772 6567  .r....r......reg
-00000760: 696f 6e73 720c 0000 00da 0475 6e69 7472  ionsr......unitr
-00000770: 2300 0000 7204 0000 0072 1500 0000 7214  #...r....r....r.
-00000780: 0000 0072 0a00 0000 da11 6461 6d61 6765  ...r......damage
-00000790: 5f6e 6f73 6c72 5f66 6f72 6dda 0f64 616d  _noslr_form..dam
-000007a0: 6167 655f 6e6f 736c 725f 6231 da0f 6461  age_noslr_b1..da
-000007b0: 6d61 6765 5f6e 6f73 6c72 5f62 32da 0f64  mage_noslr_b2..d
-000007c0: 616d 6167 655f 6e6f 736c 725f 6233 da0e  amage_noslr_b3..
-000007d0: 6461 6d61 6765 5f6e 6f73 6c72 5f61 da06  damage_noslr_a..
-000007e0: 6170 7065 6e64 7207 0000 0072 2000 0000  appendr....r ...
-000007f0: da0f 6461 6d61 6765 5f73 6c72 5f66 6f72  ..damage_slr_for
-00000800: 6dda 0d64 616d 6167 655f 736c 725f 6231  m..damage_slr_b1
-00000810: da0d 6461 6d61 6765 5f73 6c72 5f62 32da  ..damage_slr_b2.
-00000820: 0d64 616d 6167 655f 736c 725f 6233 da0c  .damage_slr_b3..
-00000830: 6461 6d61 6765 5f73 6c72 5f61 2902 720d  damage_slr_a).r.
-00000840: 0000 00da 0b63 6f6e 7374 7261 696e 7473  .....constraints
-00000850: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
-00000860: 0f67 6574 5f63 6f6e 7374 7261 696e 7473  .get_constraints
-00000870: 1500 0000 7350 0000 0004 0f1a 0208 011a  ....sP..........
-00000880: 0310 020c 010c 0110 010c 0304 0402 0106  ................
-00000890: 0102 0302 fc04 ff02 0a12 0108 ff10 040c  ................
-000008a0: 0102 0106 0108 ff02 0306 0108 ff0c 0504  ................
-000008b0: 0302 0106 0102 0302 fc04 ff04 0a02 0106  ................
-000008c0: 0102 0202 fd04 ff04 0872 3200 0000 4663  .........r2...Fc
-000008d0: 0400 0000 0000 0000 0000 0000 0900 0000  ................
-000008e0: 0600 0000 4300 0000 73dc 0000 007c 0372  ....C...s....|.r
-000008f0: 1e7c 016a 007c 0219 007d 047c 016a 017c  .|.j.|...}.|.j.|
-00000900: 0219 007c 016a 027c 0219 007c 016a 037c  ...|.j.|...|.j.|
-00000910: 0219 0003 0302 037d 057d 067d 077c 016a  .......}.}.}.|.j
-00000920: 047c 0219 007d 086e 1b7c 016a 057c 0219  .|...}.n.|.j.|..
-00000930: 007d 047c 016a 067c 0219 007c 016a 077c  .}.|.j.|...|.j.|
-00000940: 0219 007c 016a 087c 0219 0003 0302 037d  ...|.j.|.......}
-00000950: 057d 067d 077c 016a 097c 0219 007d 0864  .}.}.|.j.|...}.d
-00000960: 0174 0a7c 0483 0176 0072 477c 087c 0514  .t.|...v.rG|.|..
-00000970: 007c 0014 0064 021b 0053 0064 0374 0a7c  .|...d...S.d.t.|
-00000980: 0483 0176 0072 5b7c 087c 057c 0014 007c  ...v.r[|.|.|...|
-00000990: 067c 0064 0413 0014 0017 0014 0064 021b  .|.d.........d..
-000009a0: 0053 0064 0574 0a7c 0483 0176 0072 6c7c  .S.d.t.|...v.rl|
-000009b0: 0874 0b7c 007c 057c 067c 0783 0414 0064  .t.|.|.|.|.....d
-000009c0: 021b 0053 0074 0c82 0129 064e da06 4c69  ...S.t...).N..Li
-000009d0: 6e65 6172 6700 0000 0000 0059 405a 0951  nearg......Y@Z.Q
-000009e0: 7561 6472 6174 6963 e902 0000 005a 084c  uadratic.....Z.L
-000009f0: 6f67 6973 7469 6329 0d72 2c00 0000 722d  ogistic).r,...r-
-00000a00: 0000 0072 2e00 0000 722f 0000 0072 3000  ...r....r/...r0.
-00000a10: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
-00000a20: 0072 2900 0000 722a 0000 0072 0800 0000  .r)...r*...r....
-00000a30: da08 6c6f 6769 7374 6963 da13 4e6f 7449  ..logistic..NotI
-00000a40: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
-00000a50: 09da 0178 720d 0000 0072 1b00 0000 7213  ...xr....r....r.
-00000a60: 0000 00da 0466 6f72 6dda 0262 31da 0262  .....form..b1..b
-00000a70: 32da 0262 33da 0161 721c 0000 0072 1c00  2..b3..ar....r..
-00000a80: 0000 721d 0000 00da 0f66 756e 6374 696f  ..r......functio
-00000a90: 6e61 6c5f 666f 726d 6e00 0000 731c 0000  nal_formn...s...
-00000aa0: 0004 010a 0122 010c 010a 0222 010a 010c  ....."....."....
-00000ab0: 0310 010c 031c 010c 0316 0104 0272 3d00  .............r=.
-00000ac0: 0000 6305 0000 0000 0000 0000 0000 0006  ..c.............
-00000ad0: 0000 0006 0000 0043 0000 0073 2c00 0000  .......C...s,...
-00000ae0: 7400 7c00 7c02 7c03 7c04 8304 7d05 7c01  t.|.|.|.|...}.|.
-00000af0: 6400 7501 7214 7c05 7400 7c01 7c02 7c03  d.u.r.|.t.|.|.|.
-00000b00: 7c04 8304 3800 7d05 7c05 5300 7222 0000  |...8.}.|.S.r"..
-00000b10: 0029 0172 3d00 0000 2906 7237 0000 00da  .).r=...).r7....
-00000b20: 0278 3072 0d00 0000 721b 0000 0072 1300  .x0r....r....r..
-00000b30: 0000 da06 6461 6d61 6765 721c 0000 0072  ....damager....r
-00000b40: 1c00 0000 721d 0000 0072 1600 0000 8700  ....r....r......
-00000b50: 0000 7308 0000 000e 0108 0112 0104 0272  ..s............r
-00000b60: 1600 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00000b70: 0005 0000 0005 0000 0043 0000 0073 3400  .........C...s4.
-00000b80: 0000 7400 7c03 0b00 7c00 1400 6401 6402  ..t.|...|...d.d.
-00000b90: 6403 8d03 7d04 7c01 6404 7c02 7401 7c04  d...}.|.d.|.t.|.
-00000ba0: 8301 1400 1700 1b00 7c01 6404 7c02 1700  ........|.d.|...
-00000bb0: 1b00 1800 5300 2905 4ee9 0a00 0000 679a  ....S.).N.....g.
-00000bc0: 9999 9999 99b9 3f29 01da 0573 6361 6c65  ......?)...scale
-00000bd0: e901 0000 0029 0272 0900 0000 720b 0000  .....).r....r...
-00000be0: 0029 0572 3700 0000 7239 0000 0072 3a00  .).r7...r9...r:.
-00000bf0: 0000 723b 0000 00da 0865 7870 6f6e 656e  ..r;.....exponen
-00000c00: 7472 1c00 0000 721c 0000 0072 1d00 0000  tr....r....r....
-00000c10: 7235 0000 008f 0000 0073 0400 0000 1401  r5.......s......
-00000c20: 2001 7235 0000 004e 2901 4629 12da 075f   .r5...N).F)..._
-00000c30: 5f64 6f63 5f5f da06 7479 7069 6e67 7202  _doc__..typingr.
-00000c40: 0000 00da 0d6d 696d 6f73 612e 636f 6d6d  .....mimosa.comm
-00000c50: 6f6e 7203 0000 0072 0400 0000 7205 0000  onr....r....r...
-00000c60: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
-00000c70: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000c80: 0c00 0000 7232 0000 0072 3d00 0000 7216  ....r2...r=...r.
-00000c90: 0000 0072 3500 0000 721c 0000 0072 1c00  ...r5...r....r..
-00000ca0: 0000 721c 0000 0072 1d00 0000 da08 3c6d  ..r....r......<m
-00000cb0: 6f64 756c 653e 0100 0000 730e 0000 0004  odule>....s.....
-00000cc0: 000c 0530 0116 0e0a 5908 190c 08         ...0....Y....
+000004e0: 5f73 6c72 2905 da14 6461 6d61 6765 5f63  _slr)...damage_c
+000004f0: 6f73 7473 5f6e 6f6e 5f73 6c72 da13 6461  osts_non_slr..da
+00000500: 6d61 6765 5f73 6361 6c65 5f66 6163 746f  mage_scale_facto
+00000510: 72da 0a64 616d 6167 655f 6663 74da 0b74  r..damage_fct..t
+00000520: 656d 7065 7261 7475 7265 da02 5430 a903  emperature..T0..
+00000530: 720d 0000 00da 0174 da01 72a9 0072 1c00  r......t..r..r..
+00000540: 0000 fa65 633a 5c55 7365 7273 5c33 3930  ...ec:\Users\390
+00000550: 3338 3835 5c4f 6e65 4472 6976 6520 2d20  3885\OneDrive - 
+00000560: 556e 6976 6572 7369 7465 6974 2055 7472  Universiteit Utr
+00000570: 6563 6874 5c44 6f63 756d 656e 7473 5c4d  echt\Documents\M
+00000580: 494d 4f53 415c 6d69 6d6f 7361 5c63 6f6d  IMOSA\mimosa\com
+00000590: 706f 6e65 6e74 735c 6461 6d61 6765 735c  ponents\damages\
+000005a0: 636f 6163 6368 2e70 79da 083c 6c61 6d62  coacch.py..<lamb
+000005b0: 6461 3e38 0000 0073 0a00 0000 0c00 0401  da>8...s........
+000005c0: 2001 02ff 04ff 7a21 6765 745f 636f 6e73   .....z!get_cons
+000005d0: 7472 6169 6e74 732e 3c6c 6f63 616c 733e  traints.<locals>
+000005e0: 2e3c 6c61 6d62 6461 3e72 1400 0000 2902  .<lambda>r....).
+000005f0: 6700 0000 0000 00e0 bf67 6666 6666 6666  g........gffffff
+00000600: e63f 2902 da06 626f 756e 6473 7210 0000  .?)...boundsr...
+00000610: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
+00000620: 0000 0900 0000 5300 0000 7332 0000 007c  ......S...s2...|
+00000630: 006a 007c 017c 0266 0219 007c 006a 0174  .j.|.|.f...|.j.t
+00000640: 027c 006a 037c 0119 007c 006a 0364 0119  .|.j.|...|.j.d..
+00000650: 007c 007c 0264 0264 038d 0514 006b 0253  .|.|.d.d.....k.S
+00000660: 0029 044e 7201 0000 0054 7212 0000 0029  .).Nr....Tr....)
+00000670: 04da 1064 616d 6167 655f 636f 7374 735f  ...damage_costs_
+00000680: 736c 7272 1500 0000 7216 0000 00da 0974  slrr....r......t
+00000690: 6f74 616c 5f53 4c52 7219 0000 0072 1c00  otal_SLRr....r..
+000006a0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+000006b0: 0053 0000 0073 0a00 0000 0c00 0401 1c01  .S...s..........
+000006c0: 02ff 04ff 7220 0000 0063 0300 0000 0000  ....r ...c......
+000006d0: 0000 0000 0000 0300 0000 0500 0000 5300  ..............S.
+000006e0: 0000 732a 0000 007c 006a 007c 017c 0266  ..s*...|.j.|.|.f
+000006f0: 0219 007c 006a 017c 017c 0266 0219 007c  ...|.j.|.|.f...|
+00000700: 006a 027c 017c 0266 0219 0017 006b 0253  .j.|.|.f.....k.S
+00000710: 00a9 014e 2903 da0c 6461 6d61 6765 5f63  ...N)...damage_c
+00000720: 6f73 7473 7214 0000 0072 2000 0000 7219  ostsr....r ...r.
+00000730: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
+00000740: 0000 721e 0000 005d 0000 0073 0600 0000  ..r....]...s....
+00000750: 0c00 1a01 04ff 7223 0000 0029 1772 0500  ......r#...).r..
+00000760: 0000 721a 0000 00da 0772 6567 696f 6e73  ..r......regions
+00000770: 720c 0000 00da 0475 6e69 7472 2300 0000  r......unitr#...
+00000780: 7204 0000 0072 1500 0000 7214 0000 0072  r....r....r....r
+00000790: 0a00 0000 da11 6461 6d61 6765 5f6e 6f73  ......damage_nos
+000007a0: 6c72 5f66 6f72 6dda 0f64 616d 6167 655f  lr_form..damage_
+000007b0: 6e6f 736c 725f 6231 da0f 6461 6d61 6765  noslr_b1..damage
+000007c0: 5f6e 6f73 6c72 5f62 32da 0f64 616d 6167  _noslr_b2..damag
+000007d0: 655f 6e6f 736c 725f 6233 da0e 6461 6d61  e_noslr_b3..dama
+000007e0: 6765 5f6e 6f73 6c72 5f61 da06 6170 7065  ge_noslr_a..appe
+000007f0: 6e64 7207 0000 0072 2000 0000 da0f 6461  ndr....r .....da
+00000800: 6d61 6765 5f73 6c72 5f66 6f72 6dda 0d64  mage_slr_form..d
+00000810: 616d 6167 655f 736c 725f 6231 da0d 6461  amage_slr_b1..da
+00000820: 6d61 6765 5f73 6c72 5f62 32da 0d64 616d  mage_slr_b2..dam
+00000830: 6167 655f 736c 725f 6233 da0c 6461 6d61  age_slr_b3..dama
+00000840: 6765 5f73 6c72 5f61 2902 720d 0000 00da  ge_slr_a).r.....
+00000850: 0b63 6f6e 7374 7261 696e 7473 721c 0000  .constraintsr...
+00000860: 0072 1c00 0000 721d 0000 00da 0f67 6574  .r....r......get
+00000870: 5f63 6f6e 7374 7261 696e 7473 1500 0000  _constraints....
+00000880: 7350 0000 0004 0f1a 0208 011a 0310 020c  sP..............
+00000890: 010c 0110 010c 0304 0402 0106 0102 0302  ................
+000008a0: fc04 ff02 0a12 0108 ff10 040c 0102 0106  ................
+000008b0: 0108 ff02 0306 0108 ff0c 0504 0302 0106  ................
+000008c0: 0102 0302 fc04 ff04 0a02 0106 0102 0202  ................
+000008d0: fd04 ff04 0872 3200 0000 4663 0400 0000  .....r2...Fc....
+000008e0: 0000 0000 0000 0000 0900 0000 0600 0000  ................
+000008f0: 4300 0000 73dc 0000 007c 0372 1e7c 016a  C...s....|.r.|.j
+00000900: 007c 0219 007d 047c 016a 017c 0219 007c  .|...}.|.j.|...|
+00000910: 016a 027c 0219 007c 016a 037c 0219 0003  .j.|...|.j.|....
+00000920: 0302 037d 057d 067d 077c 016a 047c 0219  ...}.}.}.|.j.|..
+00000930: 007d 086e 1b7c 016a 057c 0219 007d 047c  .}.n.|.j.|...}.|
+00000940: 016a 067c 0219 007c 016a 077c 0219 007c  .j.|...|.j.|...|
+00000950: 016a 087c 0219 0003 0302 037d 057d 067d  .j.|.......}.}.}
+00000960: 077c 016a 097c 0219 007d 0864 0174 0a7c  .|.j.|...}.d.t.|
+00000970: 0483 0176 0072 477c 087c 0514 007c 0014  ...v.rG|.|...|..
+00000980: 0064 021b 0053 0064 0374 0a7c 0483 0176  .d...S.d.t.|...v
+00000990: 0072 5b7c 087c 057c 0014 007c 067c 0064  .r[|.|.|...|.|.d
+000009a0: 0413 0014 0017 0014 0064 021b 0053 0064  .........d...S.d
+000009b0: 0574 0a7c 0483 0176 0072 6c7c 0874 0b7c  .t.|...v.rl|.t.|
+000009c0: 007c 057c 067c 0783 0414 0064 021b 0053  .|.|.|.....d...S
+000009d0: 0074 0c82 0129 064e da06 4c69 6e65 6172  .t...).N..Linear
+000009e0: 6700 0000 0000 0059 405a 0951 7561 6472  g......Y@Z.Quadr
+000009f0: 6174 6963 e902 0000 005a 084c 6f67 6973  atic.....Z.Logis
+00000a00: 7469 6329 0d72 2c00 0000 722d 0000 0072  tic).r,...r-...r
+00000a10: 2e00 0000 722f 0000 0072 3000 0000 7226  ....r/...r0...r&
+00000a20: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
+00000a30: 0000 722a 0000 0072 0800 0000 da08 6c6f  ..r*...r......lo
+00000a40: 6769 7374 6963 da13 4e6f 7449 6d70 6c65  gistic..NotImple
+00000a50: 6d65 6e74 6564 4572 726f 7229 09da 0178  mentedError)...x
+00000a60: 720d 0000 0072 1b00 0000 7213 0000 00da  r....r....r.....
+00000a70: 0466 6f72 6dda 0262 31da 0262 32da 0262  .form..b1..b2..b
+00000a80: 33da 0161 721c 0000 0072 1c00 0000 721d  3..ar....r....r.
+00000a90: 0000 00da 0f66 756e 6374 696f 6e61 6c5f  .....functional_
+00000aa0: 666f 726d 6e00 0000 731c 0000 0004 010a  formn...s.......
+00000ab0: 0122 010c 010a 0222 010a 010c 0310 010c  ."....."........
+00000ac0: 031c 010c 0316 0104 0272 3d00 0000 6305  .........r=...c.
+00000ad0: 0000 0000 0000 0000 0000 0006 0000 0006  ................
+00000ae0: 0000 0043 0000 0073 2c00 0000 7400 7c00  ...C...s,...t.|.
+00000af0: 7c02 7c03 7c04 8304 7d05 7c01 6400 7501  |.|.|...}.|.d.u.
+00000b00: 7214 7c05 7400 7c01 7c02 7c03 7c04 8304  r.|.t.|.|.|.|...
+00000b10: 3800 7d05 7c05 5300 7222 0000 0029 0172  8.}.|.S.r"...).r
+00000b20: 3d00 0000 2906 7237 0000 00da 0278 3072  =...).r7.....x0r
+00000b30: 0d00 0000 721b 0000 0072 1300 0000 da06  ....r....r......
+00000b40: 6461 6d61 6765 721c 0000 0072 1c00 0000  damager....r....
+00000b50: 721d 0000 0072 1600 0000 8700 0000 7308  r....r........s.
+00000b60: 0000 000e 0108 0112 0104 0272 1600 0000  ...........r....
+00000b70: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
+00000b80: 0005 0000 0043 0000 0073 3400 0000 7400  .....C...s4...t.
+00000b90: 7c03 0b00 7c00 1400 6401 6402 6403 8d03  |...|...d.d.d...
+00000ba0: 7d04 7c01 6404 7c02 7401 7c04 8301 1400  }.|.d.|.t.|.....
+00000bb0: 1700 1b00 7c01 6404 7c02 1700 1b00 1800  ....|.d.|.......
+00000bc0: 5300 2905 4ee9 0a00 0000 679a 9999 9999  S.).N.....g.....
+00000bd0: 99b9 3f29 01da 0573 6361 6c65 e901 0000  ..?)...scale....
+00000be0: 0029 0272 0900 0000 720b 0000 0029 0572  .).r....r....).r
+00000bf0: 3700 0000 7239 0000 0072 3a00 0000 723b  7...r9...r:...r;
+00000c00: 0000 00da 0865 7870 6f6e 656e 7472 1c00  .....exponentr..
+00000c10: 0000 721c 0000 0072 1d00 0000 7235 0000  ..r....r....r5..
+00000c20: 008f 0000 0073 0400 0000 1401 2001 7235  .....s...... .r5
+00000c30: 0000 004e 2901 4629 12da 075f 5f64 6f63  ...N).F)...__doc
+00000c40: 5f5f da06 7479 7069 6e67 7202 0000 00da  __..typingr.....
+00000c50: 0d6d 696d 6f73 612e 636f 6d6d 6f6e 7203  .mimosa.commonr.
+00000c60: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
+00000c70: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00000c80: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00000c90: 7232 0000 0072 3d00 0000 7216 0000 0072  r2...r=...r....r
+00000ca0: 3500 0000 721c 0000 0072 1c00 0000 721c  5...r....r....r.
+00000cb0: 0000 0072 1d00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000cc0: 653e 0100 0000 730e 0000 0004 000c 0530  e>....s........0
+00000cd0: 0116 0e0a 5908 190c 08                   ....Y....
```

### Comparing `mimosa-0.1.3/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:45 2023 UTC, .py size: 971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b936 ba64 cb03 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 cb03 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6404 6504 6405 6502 6506  m.Z...d.e.d.e.e.
 00000060: 1900 6604 6406 6407 8404 5a08 6408 5300  ..f.d.d...Z.d.S.
 00000070: 2909 7a3e 0a4d 6f64 656c 2065 7175 6174  ).z>.Model equat
@@ -48,18 +48,18 @@
 000002f0: 0029 01da 0a69 6e69 7469 616c 697a 6563  .)...initializec
 00000300: 0300 0000 0000 0000 0000 0000 0300 0000  ................
 00000310: 0300 0000 5300 0000 7312 0000 007c 006a  ....S...s....|.j
 00000320: 007c 017c 0266 0219 0064 016b 0253 0029  .|.|.f...d.k.S.)
 00000330: 024e 7209 0000 0029 01da 0c64 616d 6167  .Nr....)...damag
 00000340: 655f 636f 7374 7329 0372 0700 0000 da01  e_costs).r......
 00000350: 74da 0172 a900 720e 0000 00fa 6763 3a5c  t..r..r.....gc:\
-00000360: 7573 6572 735c 3339 3033 3838 355c 6f6e  users\3903885\on
-00000370: 6564 7269 7665 202d 2075 6e69 7665 7273  edrive - univers
-00000380: 6974 6569 7420 7574 7265 6368 745c 646f  iteit utrecht\do
-00000390: 6375 6d65 6e74 735c 6d69 6d6f 7361 5c6d  cuments\mimosa\m
+00000360: 5573 6572 735c 3339 3033 3838 355c 4f6e  Users\3903885\On
+00000370: 6544 7269 7665 202d 2055 6e69 7665 7273  eDrive - Univers
+00000380: 6974 6569 7420 5574 7265 6368 745c 446f  iteit Utrecht\Do
+00000390: 6375 6d65 6e74 735c 4d49 4d4f 5341 5c6d  cuments\MIMOSA\m
 000003a0: 696d 6f73 615c 636f 6d70 6f6e 656e 7473  imosa\components
 000003b0: 5c64 616d 6167 6573 5c6e 6f64 616d 6167  \damages\nodamag
 000003c0: 652e 7079 da08 3c6c 616d 6264 613e 1f00  e.py..<lambda>..
 000003d0: 0000 7302 0000 0012 007a 2167 6574 5f63  ..s......z!get_c
 000003e0: 6f6e 7374 7261 696e 7473 2e3c 6c6f 6361  onstraints.<loca
 000003f0: 6c73 3e2e 3c6c 616d 6264 613e 5a11 7a65  ls>.<lambda>Z.ze
 00000400: 726f 5f64 616d 6167 655f 636f 7374 7329  ro_damage_costs)
```

### Comparing `mimosa-0.1.3/mimosa/components/damages/ad_rice2010.py` & `mimosa-0.1.4/mimosa/components/damages/ad_rice2010.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/damages/ad_rice2012.py` & `mimosa-0.1.4/mimosa/components/damages/ad_rice2012.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/damages/ad_witch.py` & `mimosa-0.1.4/mimosa/components/damages/ad_witch.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/damages/coacch.py` & `mimosa-0.1.4/mimosa/components/damages/coacch.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,37 +35,37 @@
     """
     constraints = []
 
     m.damage_costs = Var(m.t, m.regions, units=quant.unit("fraction_of_GDP"))
     m.damage_scale_factor = Param()
 
     # Damages not related to SLR (dependent on temperature)
-    m.resid_damages = Var(m.t, m.regions, units=quant.unit("fraction_of_GDP"))
+    m.damage_costs_non_slr = Var(m.t, m.regions, units=quant.unit("fraction_of_GDP"))
 
     m.damage_noslr_form = Param(m.regions, within=Any)  # String for functional form
     m.damage_noslr_b1 = Param(m.regions)
     m.damage_noslr_b2 = Param(m.regions)
     m.damage_noslr_b3 = Param(m.regions, within=Any)  # Can be empty
     # (b2 and b3 are only used for some functional forms)
 
     m.damage_noslr_a = Param(m.regions)
 
     # Quadratic damage function for non-SLR damages. Factor `a` represents
     # the damage quantile
     constraints.append(
         RegionalConstraint(
-            lambda m, t, r: m.resid_damages[t, r]
+            lambda m, t, r: m.damage_costs_non_slr[t, r]
             == m.damage_scale_factor
             * damage_fct(m.temperature[t] - 0.6, m.T0 - 0.6, m, r, is_slr=False),
-            "resid_damages",
+            "damage_costs_non_slr",
         )
     )
 
     # SLR damages
-    m.SLR_damages = Var(
+    m.damage_costs_slr = Var(
         m.t, m.regions, bounds=(-0.5, 0.7), units=quant.unit("fraction_of_GDP")
     )
 
     m.damage_slr_form = Param(m.regions, within=Any)  # String for functional form
     m.damage_slr_b1 = Param(m.regions)
     m.damage_slr_b2 = Param(
         m.regions, within=Any
@@ -76,26 +76,26 @@
     # (b2 and b3 are only used for some functional forms)
 
     m.damage_slr_a = Param(m.regions)
 
     # Linear damage function for SLR damages, including adaptation costs
     constraints.append(
         RegionalConstraint(
-            lambda m, t, r: m.SLR_damages[t, r]
+            lambda m, t, r: m.damage_costs_slr[t, r]
             == m.damage_scale_factor
             * damage_fct(m.total_SLR[t], m.total_SLR[0], m, r, is_slr=True),
-            "SLR_damages",
+            "damage_costs_slr",
         )
     )
 
     # Total damages are sum of non-SLR and SLR damages
     constraints.append(
         RegionalConstraint(
             lambda m, t, r: m.damage_costs[t, r]
-            == m.resid_damages[t, r] + m.SLR_damages[t, r],
+            == m.damage_costs_non_slr[t, r] + m.damage_costs_slr[t, r],
             "damage_costs",
         ),
     )
 
     return constraints
```

### Comparing `mimosa-0.1.3/mimosa/components/damages/nodamage.py` & `mimosa-0.1.4/mimosa/components/damages/nodamage.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/emissions.py` & `mimosa-0.1.4/mimosa/components/emissions.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:45 2023 UTC, .py size: 5274 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b936 ba64 9a14 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 82a0 ba64 9e14 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 0100 6401 6404 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6504 6406 6502 6505 1900 6604  ..d.e.d.e.e...f.
@@ -44,201 +44,201 @@
 000002b0: 8400 640a 8302 7410 640b 6407 8400 640c  ..d...t.d.d...d.
 000002c0: 8302 6703 a101 0100 7c01 a00f 7411 640d  ..g.....|...t.d.
 000002d0: 6407 8400 640e 8302 7411 640f 6407 8400  d...d...t.d.d...
 000002e0: 6410 8302 7411 6411 6407 8400 6412 8302  d...t.d.d...d...
 000002f0: 7411 6413 6407 8400 6414 8302 7411 6415  t.d.d...d...t.d.
 00000300: 6407 8400 6416 8302 7411 6417 6407 8400  d...d...t.d.d...
 00000310: 6418 8302 6706 a101 0100 7c01 5300 2919  d...g.....|.S.).
-00000320: 617a 0100 0045 6d69 7373 696f 6e20 7472  az...Emission tr
+00000320: 617b 0100 0045 6d69 7373 696f 6e20 7472  a{...Emission tr
 00000330: 6164 696e 6720 6571 7561 7469 6f6e 7320  ading equations 
 00000340: 616e 6420 636f 6e73 7472 6169 6e74 730a  and constraints.
 00000350: 2020 2020 2874 7261 6469 6e67 206f 6620      (trading of 
 00000360: 656d 6973 7369 6f6e 7320 7370 6563 6966  emissions specif
 00000370: 6963 6174 696f 6e29 0a0a 2020 2020 4e65  ication)..    Ne
 00000380: 6365 7373 6172 7920 7661 7269 6162 6c65  cessary variable
-00000390: 733a 0a20 2020 2020 2020 206d 2e61 6261  s:.        m.aba
-000003a0: 7465 6d65 6e74 5f63 6f73 7473 2028 6162  tement_costs (ab
-000003b0: 6174 656d 656e 7420 636f 7374 7320 6173  atement costs as
-000003c0: 2070 6169 6420 666f 7220 6279 2074 6869   paid for by thi
-000003d0: 7320 7265 6769 6f6e 290a 0a20 2020 2052  s region)..    R
-000003e0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000003f0: 6c69 7374 206f 6620 636f 6e73 7472 6169  list of constrai
-00000400: 6e74 7320 2861 6e79 206f 663a 0a20 2020  nts (any of:.   
-00000410: 2020 2020 2020 2020 2d20 476c 6f62 616c          - Global
-00000420: 436f 6e73 7472 6169 6e74 0a20 2020 2020  Constraint.     
-00000430: 2020 2020 2020 2d20 476c 6f62 616c 496e        - GlobalIn
-00000440: 6974 436f 6e73 7472 6169 6e74 0a20 2020  itConstraint.   
-00000450: 2020 2020 2020 2020 2d20 5265 6769 6f6e          - Region
-00000460: 616c 436f 6e73 7472 6169 6e74 0a20 2020  alConstraint.   
-00000470: 2020 2020 2020 2020 2d20 5265 6769 6f6e          - Region
-00000480: 616c 496e 6974 436f 6e73 7472 6169 6e74  alInitConstraint
-00000490: 0a20 2020 2020 2020 2029 0a20 2020 20da  .        ).    .
-000004a0: 0e65 6d69 7373 696f 6e73 5f75 6e69 7429  .emissions_unit)
-000004b0: 02da 0575 6e69 7473 da06 7769 7468 696e  ...units..within
-000004c0: da0d 6375 7272 656e 6379 5f75 6e69 74da  ..currency_unit.
-000004d0: 0a69 6e69 7469 616c 697a 6567 7b14 ae47  .initializeg{..G
-000004e0: e17a 843f 6302 0000 0000 0000 0000 0000  .z.?c...........
-000004f0: 0002 0000 0005 0000 0013 0000 00f3 2400  ..............$.
-00000500: 0000 8800 6a00 8801 1900 7401 8700 8701  ....j.....t.....
-00000510: 6602 6401 6402 8408 8800 6a02 4400 8301  f.d.d.....j.D...
-00000520: 8301 6b02 5300 2903 4e63 0100 0000 0000  ..k.S.).Nc......
-00000530: 0000 0000 0000 0200 0000 0400 0000 3300  ..............3.
-00000540: 0000 f31e 0000 0081 007c 005d 0a7d 0188  .........|.].}..
-00000550: 006a 0088 017c 0166 0219 0056 0001 0071  .j...|.f...V...q
-00000560: 0264 0053 00a9 014e 2901 da1b 6578 706f  .d.S...N)...expo
-00000570: 7274 6564 5f65 6d69 7373 696f 6e5f 7265  rted_emission_re
-00000580: 6475 6374 696f 6ea9 02da 022e 30da 0172  duction.....0..r
-00000590: a902 720c 0000 00da 0174 a900 fa72 633a  ..r......t...rc:
-000005a0: 5c75 7365 7273 5c33 3930 3338 3835 5c6f  \users\3903885\o
-000005b0: 6e65 6472 6976 6520 2d20 756e 6976 6572  nedrive - univer
-000005c0: 7369 7465 6974 2075 7472 6563 6874 5c64  siteit utrecht\d
-000005d0: 6f63 756d 656e 7473 5c6d 696d 6f73 615c  ocuments\mimosa\
-000005e0: 6d69 6d6f 7361 5c63 6f6d 706f 6e65 6e74  mimosa\component
-000005f0: 735c 656d 6973 7369 6f6e 7472 6164 655c  s\emissiontrade\
-00000600: 656d 6973 7369 6f6e 7472 6164 652e 7079  emissiontrade.py
-00000610: da09 3c67 656e 6578 7072 3e43 0000 00f3  ..<genexpr>C....
-00000620: 0400 0000 0280 1c00 fa34 6765 745f 636f  .........4get_co
-00000630: 6e73 7472 6169 6e74 732e 3c6c 6f63 616c  nstraints.<local
-00000640: 733e 2e3c 6c61 6d62 6461 3e2e 3c6c 6f63  s>.<lambda>.<loc
-00000650: 616c 733e 2e3c 6765 6e65 7870 723e a903  als>.<genexpr>..
-00000660: da19 746f 7461 6c5f 6578 706f 7274 6564  ..total_exported
-00000670: 5f72 6564 7563 7469 6f6e 73da 0373 756d  _reductions..sum
-00000680: da07 7265 6769 6f6e 7372 1a00 0000 721c  ..regionsr....r.
-00000690: 0000 0072 1a00 0000 721d 0000 00da 083c  ...r....r......<
-000006a0: 6c61 6d62 6461 3e42 0000 00f3 0600 0000  lambda>B........
-000006b0: 0800 1801 04ff 7a21 6765 745f 636f 6e73  ......z!get_cons
-000006c0: 7472 6169 6e74 732e 3c6c 6f63 616c 733e  traints.<locals>
-000006d0: 2e3c 6c61 6d62 6461 3e5a 1874 6f74 616c  .<lambda>Z.total
-000006e0: 5f65 7870 6f72 7465 645f 656d 6973 7369  _exported_emissi
-000006f0: 6f6e 7363 0200 0000 0000 0000 0000 0000  onsc............
-00000700: 0200 0000 0500 0000 1300 0000 7213 0000  ............r...
-00000710: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00000720: 0002 0000 0004 0000 0033 0000 0072 1400  .........3...r..
-00000730: 0000 7215 0000 0029 01da 2165 7870 6f72  ..r....)..!expor
-00000740: 7465 645f 656d 6973 7369 6f6e 5f72 6564  ted_emission_red
-00000750: 7563 7469 6f6e 5f63 6f73 7473 7217 0000  uction_costsr...
-00000760: 0072 1a00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000770: 721e 0000 0048 0000 0072 1f00 0000 7220  r....H...r....r 
-00000780: 0000 0029 03da 1e74 6f74 616c 5f65 7870  ...)...total_exp
-00000790: 6f72 7465 645f 7265 6475 6374 696f 6e5f  orted_reduction_
-000007a0: 636f 7374 7372 2300 0000 7224 0000 0072  costsr#...r$...r
-000007b0: 1a00 0000 721c 0000 0072 1a00 0000 721d  ....r....r....r.
-000007c0: 0000 0072 2500 0000 4700 0000 7226 0000  ...r%...G...r&..
-000007d0: 0072 2800 0000 6302 0000 0000 0000 0000  .r(...c.........
-000007e0: 0000 0002 0000 0005 0000 0013 0000 0072  ...............r
-000007f0: 1300 0000 2903 4e63 0100 0000 0000 0000  ....).Nc........
-00000800: 0000 0000 0200 0000 0400 0000 3300 0000  ............3...
-00000810: 7214 0000 0072 1500 0000 2901 da1b 696d  r....r....)...im
-00000820: 706f 7274 6564 5f65 6d69 7373 696f 6e5f  ported_emission_
-00000830: 7265 6475 6374 696f 6e72 1700 0000 721a  reductionr....r.
-00000840: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
-00000850: 0000 4d00 0000 721f 0000 0072 2000 0000  ..M...r....r ...
-00000860: 7221 0000 0072 1a00 0000 721c 0000 0072  r!...r....r....r
-00000870: 1a00 0000 721d 0000 0072 2500 0000 4c00  ....r....r%...L.
-00000880: 0000 7226 0000 005a 3874 6f74 616c 5f69  ..r&...Z8total_i
-00000890: 6d70 6f72 7465 645f 6571 7561 6c73 5f74  mported_equals_t
-000008a0: 6f74 616c 5f65 7870 6f72 7465 645f 656d  otal_exported_em
-000008b0: 6973 7369 6f6e 5f72 6564 7563 7469 6f6e  ission_reduction
-000008c0: 7363 0300 0000 0000 0000 0000 0000 0300  sc..............
-000008d0: 0000 0400 0000 5300 0000 7330 0000 007c  ......S...s0...|
-000008e0: 006a 007c 017c 0266 0219 007c 006a 017c  .j.|.|.f...|.j.|
-000008f0: 017c 0266 0219 007c 006a 027c 0119 0014  .|.f...|.j.|....
-00000900: 007c 006a 037c 0119 001b 006b 0253 0072  .|.j.|.....k.S.r
-00000910: 1500 0000 2904 da21 696d 706f 7274 6564  ....)..!imported
-00000920: 5f65 6d69 7373 696f 6e5f 7265 6475 6374  _emission_reduct
-00000930: 696f 6e5f 636f 7374 7372 2900 0000 7228  ion_costsr)...r(
-00000940: 0000 0072 2200 0000 a903 720c 0000 0072  ...r".....r....r
-00000950: 1b00 0000 7219 0000 0072 1c00 0000 721c  ....r....r....r.
-00000960: 0000 0072 1d00 0000 7225 0000 0057 0000  ...r....r%...W..
-00000970: 0073 0e00 0000 0c00 0c01 0801 02ff 0802  .s..............
-00000980: 02fe 04ff 5a26 636f 7374 735f 666f 725f  ....Z&costs_for_
-00000990: 696d 706f 7274 6564 5f65 6d69 7373 696f  imported_emissio
-000009a0: 6e5f 7265 6475 6374 696f 6e73 6303 0000  n_reductionsc...
-000009b0: 0000 0000 0000 0000 0003 0000 0006 0000  ................
-000009c0: 0053 0000 0073 4200 0000 7c00 6a00 7c01  .S...sB...|.j.|.
-000009d0: 7c02 6602 1900 7401 7c00 6a02 7c01 7c02  |.f...t.|.j.|.|.
-000009e0: 6602 1900 7c00 6a03 7c01 7c02 6602 1900  f...|.j.|.|.f...
-000009f0: 1b00 7c00 7c01 7c02 8304 7c00 6a03 7c01  ..|.|.|...|.j.|.
-00000a00: 7c02 6602 1900 1400 6b02 5300 7215 0000  |.f.....k.S.r...
-00000a10: 0029 04da 1c6f 776e 5f65 6d69 7373 696f  .)...own_emissio
-00000a20: 6e5f 7265 6475 6374 696f 6e5f 636f 7374  n_reduction_cost
-00000a30: 7372 0b00 0000 da16 6f77 6e5f 656d 6973  sr......own_emis
-00000a40: 7369 6f6e 5f72 6564 7563 7469 6f6e da08  sion_reduction..
-00000a50: 6261 7365 6c69 6e65 722b 0000 0072 1c00  baseliner+...r..
-00000a60: 0000 721c 0000 0072 1d00 0000 7225 0000  ..r....r....r%..
-00000a70: 005f 0000 0073 0a00 0000 0c00 2401 0c01  ._...s......$...
-00000a80: 02ff 04ff 5a1d 636f 7374 735f 6f77 6e5f  ....Z.costs_own_
-00000a90: 656d 6973 7369 6f6e 5f72 6564 7563 7469  emission_reducti
-00000aa0: 6f6e 7363 0300 0000 0000 0000 0000 0000  onsc............
-00000ab0: 0300 0000 0500 0000 5300 0000 732a 0000  ........S...s*..
-00000ac0: 007c 006a 007c 017c 0266 0219 007c 006a  .|.j.|.|.f...|.j
-00000ad0: 017c 017c 0266 0219 007c 006a 027c 017c  .|.|.f...|.j.|.|
-00000ae0: 0266 0219 0017 006b 0253 0072 1500 0000  .f.....k.S.r....
-00000af0: 2903 da19 6163 7475 616c 5f65 6d69 7373  )...actual_emiss
-00000b00: 696f 6e5f 7265 6475 6374 696f 6e72 2d00  ion_reductionr-.
-00000b10: 0000 7216 0000 0072 2b00 0000 721c 0000  ..r....r+...r...
-00000b20: 0072 1c00 0000 721d 0000 0072 2500 0000  .r....r....r%...
-00000b30: 6800 0000 f306 0000 000c 001a 0104 ff72  h..............r
-00000b40: 2f00 0000 6303 0000 0000 0000 0000 0000  /...c...........
-00000b50: 0003 0000 0006 0000 0053 0000 0073 5000  .........S...sP.
-00000b60: 0000 7c00 6a00 7c01 7c02 6602 1900 7401  ..|.j.|.|.f...t.
-00000b70: 7c00 6a02 7c01 7c02 6602 1900 7c00 6a03  |.j.|.|.f...|.j.
-00000b80: 7c01 7c02 6602 1900 1b00 7c00 7c01 7c02  |.|.f.....|.|.|.
-00000b90: 8304 7c00 6a03 7c01 7c02 6602 1900 1400  ..|.j.|.|.f.....
-00000ba0: 7c00 6a04 7c01 7c02 6602 1900 1800 6b02  |.j.|.|.f.....k.
-00000bb0: 5300 7215 0000 0029 0572 2700 0000 720b  S.r....).r'...r.
-00000bc0: 0000 0072 2f00 0000 722e 0000 0072 2c00  ...r/...r....r,.
-00000bd0: 0000 722b 0000 0072 1c00 0000 721c 0000  ..r+...r....r...
-00000be0: 0072 1d00 0000 7225 0000 006d 0000 0073  .r....r%...m...s
-00000bf0: 1800 0000 0c00 0201 1a01 0201 0201 0201  ................
-00000c00: 02fc 0c06 02fa 0c07 02f9 04ff 5a22 636f  ............Z"co
-00000c10: 7374 735f 6578 706f 7274 6564 5f65 6d69  sts_exported_emi
-00000c20: 7373 696f 6e5f 7265 6475 6374 696f 6e73  ssion_reductions
-00000c30: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00000c40: 0005 0000 0053 0000 0073 2a00 0000 7c00  .....S...s*...|.
-00000c50: 6a00 7c01 7c02 6602 1900 7c00 6a01 7c01  j.|.|.f...|.j.|.
-00000c60: 7c02 6602 1900 7c00 6a02 7c01 7c02 6602  |.f...|.j.|.|.f.
-00000c70: 1900 1b00 6b02 5300 7215 0000 0029 03da  ....k.S.r....)..
-00000c80: 1272 656c 6174 6976 655f 6162 6174 656d  .relative_abatem
-00000c90: 656e 7472 2f00 0000 722e 0000 0072 2b00  entr/...r....r+.
-00000ca0: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000cb0: 0072 2500 0000 7a00 0000 7230 0000 0072  .r%...z...r0...r
-00000cc0: 3100 0000 6303 0000 0000 0000 0000 0000  1...c...........
-00000cd0: 0003 0000 0006 0000 0053 0000 0073 2e00  .........S...s..
-00000ce0: 0000 7c00 6a00 7c01 7c02 6602 1900 7c00  ..|.j.|.|.f...|.
-00000cf0: 6a01 7c01 7c02 6602 1900 6401 7c00 6a02  j.|.|.f...d.|.j.
-00000d00: 7c01 7c02 6602 1900 1400 1700 6b02 5300  |.|.f.......k.S.
-00000d10: 2902 4e67 52b8 1e85 eb51 f03f 2903 da0f  ).NgR....Q.?)...
-00000d20: 6162 6174 656d 656e 745f 636f 7374 7372  abatement_costsr
-00000d30: 2c00 0000 722a 0000 0072 2b00 0000 721c  ,...r*...r+...r.
-00000d40: 0000 0072 1c00 0000 721d 0000 0072 2500  ...r....r....r%.
-00000d50: 0000 7f00 0000 730a 0000 000c 000c 0110  ......s.........
-00000d60: 0102 ff04 ff72 3200 0000 2912 7209 0000  .....r2...).r...
-00000d70: 00da 0475 6e69 7472 0800 0000 7207 0000  ...unitr....r...
-00000d80: 0072 1b00 0000 7224 0000 0072 2d00 0000  .r....r$...r-...
-00000d90: 722c 0000 0072 2900 0000 722a 0000 0072  r,...r)...r*...r
-00000da0: 1600 0000 7227 0000 0072 2f00 0000 7222  ....r'...r/...r"
-00000db0: 0000 0072 2800 0000 da06 6578 7465 6e64  ...r(.....extend
-00000dc0: 7205 0000 0072 0600 0000 2904 720c 0000  r....r....).r...
-00000dd0: 00da 0b63 6f6e 7374 7261 696e 7473 5a0a  ...constraintsZ.
-00000de0: 6f70 7473 5f65 6d69 7373 5a0a 6f70 7473  opts_emissZ.opts
-00000df0: 5f63 6f73 7473 721c 0000 0072 1c00 0000  _costsr....r....
-00000e00: 721d 0000 00da 0f67 6574 5f63 6f6e 7374  r......get_const
-00000e10: 7261 696e 7473 1700 0000 736e 0000 0004  raints....sn....
-00000e20: 0f10 0310 0118 0318 0118 0318 011c 0318  ................
-00000e30: 0118 0314 0314 0104 0202 0206 0102 0202  ................
-00000e40: fd02 0506 0102 0202 fd02 0506 0102 0202  ................
-00000e50: fd02 f504 ff04 1402 0306 0102 0402 fb02  ................
-00000e60: 0806 0102 0302 fc02 0906 0102 0202 fd02  ................
-00000e70: 0506 0102 0902 f602 0d06 0102 0202 fd02  ................
-00000e80: 0506 0102 0302 fc02 d604 ff04 3472 3600  ............4r6.
-00000e90: 0000 4e29 0fda 075f 5f64 6f63 5f5f da06  ..N)...__doc__..
-00000ea0: 7479 7069 6e67 7202 0000 00da 0d6d 696d  typingr......mim
-00000eb0: 6f73 612e 636f 6d6d 6f6e 7203 0000 0072  osa.commonr....r
-00000ec0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00000ed0: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00000ee0: 0000 5a1b 6d69 6d6f 7361 2e63 6f6d 706f  ..Z.mimosa.compo
-00000ef0: 6e65 6e74 732e 6162 6174 656d 656e 7472  nents.abatementr
-00000f00: 0b00 0000 7236 0000 0072 1c00 0000 721c  ....r6...r....r.
-00000f10: 0000 0072 1c00 0000 721d 0000 00da 083c  ...r....r......<
-00000f20: 6d6f 6475 6c65 3e01 0000 0073 0a00 0000  module>....s....
-00000f30: 0400 0c06 2802 0c0b 1a03                 ....(.....
+00000390: 733a 0a20 2020 2020 2020 206d 2e6d 6974  s:.        m.mit
+000003a0: 6967 6174 696f 6e5f 636f 7374 7320 2861  igation_costs (a
+000003b0: 6261 7465 6d65 6e74 2063 6f73 7473 2061  batement costs a
+000003c0: 7320 7061 6964 2066 6f72 2062 7920 7468  s paid for by th
+000003d0: 6973 2072 6567 696f 6e29 0a0a 2020 2020  is region)..    
+000003e0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000003f0: 206c 6973 7420 6f66 2063 6f6e 7374 7261   list of constra
+00000400: 696e 7473 2028 616e 7920 6f66 3a0a 2020  ints (any of:.  
+00000410: 2020 2020 2020 2020 202d 2047 6c6f 6261           - Globa
+00000420: 6c43 6f6e 7374 7261 696e 740a 2020 2020  lConstraint.    
+00000430: 2020 2020 2020 202d 2047 6c6f 6261 6c49         - GlobalI
+00000440: 6e69 7443 6f6e 7374 7261 696e 740a 2020  nitConstraint.  
+00000450: 2020 2020 2020 2020 202d 2052 6567 696f           - Regio
+00000460: 6e61 6c43 6f6e 7374 7261 696e 740a 2020  nalConstraint.  
+00000470: 2020 2020 2020 2020 202d 2052 6567 696f           - Regio
+00000480: 6e61 6c49 6e69 7443 6f6e 7374 7261 696e  nalInitConstrain
+00000490: 740a 2020 2020 2020 2020 290a 2020 2020  t.        ).    
+000004a0: da0e 656d 6973 7369 6f6e 735f 756e 6974  ..emissions_unit
+000004b0: 2902 da05 756e 6974 73da 0677 6974 6869  )...units..withi
+000004c0: 6eda 0d63 7572 7265 6e63 795f 756e 6974  n..currency_unit
+000004d0: da0a 696e 6974 6961 6c69 7a65 677b 14ae  ..initializeg{..
+000004e0: 47e1 7a84 3f63 0200 0000 0000 0000 0000  G.z.?c..........
+000004f0: 0000 0200 0000 0500 0000 1300 0000 f324  ...............$
+00000500: 0000 0088 006a 0088 0119 0074 0187 0087  .....j.....t....
+00000510: 0166 0264 0164 0284 0888 006a 0244 0083  .f.d.d.....j.D..
+00000520: 0183 016b 0253 0029 034e 6301 0000 0000  ...k.S.).Nc.....
+00000530: 0000 0000 0000 0002 0000 0004 0000 0033  ...............3
+00000540: 0000 00f3 1e00 0000 8100 7c00 5d0a 7d01  ..........|.].}.
+00000550: 8800 6a00 8801 7c01 6602 1900 5600 0100  ..j...|.f...V...
+00000560: 7102 6400 5300 a901 4e29 01da 1b65 7870  q.d.S...N)...exp
+00000570: 6f72 7465 645f 656d 6973 7369 6f6e 5f72  orted_emission_r
+00000580: 6564 7563 7469 6f6e a902 da02 2e30 da01  eduction.....0..
+00000590: 72a9 0272 0c00 0000 da01 74a9 00fa 7263  r..r......t...rc
+000005a0: 3a5c 5573 6572 735c 3339 3033 3838 355c  :\Users\3903885\
+000005b0: 4f6e 6544 7269 7665 202d 2055 6e69 7665  OneDrive - Unive
+000005c0: 7273 6974 6569 7420 5574 7265 6368 745c  rsiteit Utrecht\
+000005d0: 446f 6375 6d65 6e74 735c 4d49 4d4f 5341  Documents\MIMOSA
+000005e0: 5c6d 696d 6f73 615c 636f 6d70 6f6e 656e  \mimosa\componen
+000005f0: 7473 5c65 6d69 7373 696f 6e74 7261 6465  ts\emissiontrade
+00000600: 5c65 6d69 7373 696f 6e74 7261 6465 2e70  \emissiontrade.p
+00000610: 79da 093c 6765 6e65 7870 723e 4300 0000  y..<genexpr>C...
+00000620: f304 0000 0002 801c 00fa 3467 6574 5f63  ..........4get_c
+00000630: 6f6e 7374 7261 696e 7473 2e3c 6c6f 6361  onstraints.<loca
+00000640: 6c73 3e2e 3c6c 616d 6264 613e 2e3c 6c6f  ls>.<lambda>.<lo
+00000650: 6361 6c73 3e2e 3c67 656e 6578 7072 3ea9  cals>.<genexpr>.
+00000660: 03da 1974 6f74 616c 5f65 7870 6f72 7465  ...total_exporte
+00000670: 645f 7265 6475 6374 696f 6e73 da03 7375  d_reductions..su
+00000680: 6dda 0772 6567 696f 6e73 721a 0000 0072  m..regionsr....r
+00000690: 1c00 0000 721a 0000 0072 1d00 0000 da08  ....r....r......
+000006a0: 3c6c 616d 6264 613e 4200 0000 f306 0000  <lambda>B.......
+000006b0: 0008 0018 0104 ff7a 2167 6574 5f63 6f6e  .......z!get_con
+000006c0: 7374 7261 696e 7473 2e3c 6c6f 6361 6c73  straints.<locals
+000006d0: 3e2e 3c6c 616d 6264 613e 5a18 746f 7461  >.<lambda>Z.tota
+000006e0: 6c5f 6578 706f 7274 6564 5f65 6d69 7373  l_exported_emiss
+000006f0: 696f 6e73 6302 0000 0000 0000 0000 0000  ionsc...........
+00000700: 0002 0000 0005 0000 0013 0000 0072 1300  .............r..
+00000710: 0000 2903 4e63 0100 0000 0000 0000 0000  ..).Nc..........
+00000720: 0000 0200 0000 0400 0000 3300 0000 7214  ..........3...r.
+00000730: 0000 0072 1500 0000 2901 da21 6578 706f  ...r....)..!expo
+00000740: 7274 6564 5f65 6d69 7373 696f 6e5f 7265  rted_emission_re
+00000750: 6475 6374 696f 6e5f 636f 7374 7372 1700  duction_costsr..
+00000760: 0000 721a 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000770: 0072 1e00 0000 4800 0000 721f 0000 0072  .r....H...r....r
+00000780: 2000 0000 2903 da1e 746f 7461 6c5f 6578   ...)...total_ex
+00000790: 706f 7274 6564 5f72 6564 7563 7469 6f6e  ported_reduction
+000007a0: 5f63 6f73 7473 7223 0000 0072 2400 0000  _costsr#...r$...
+000007b0: 721a 0000 0072 1c00 0000 721a 0000 0072  r....r....r....r
+000007c0: 1d00 0000 7225 0000 0047 0000 0072 2600  ....r%...G...r&.
+000007d0: 0000 7228 0000 0063 0200 0000 0000 0000  ..r(...c........
+000007e0: 0000 0000 0200 0000 0500 0000 1300 0000  ................
+000007f0: 7213 0000 0029 034e 6301 0000 0000 0000  r....).Nc.......
+00000800: 0000 0000 0002 0000 0004 0000 0033 0000  .............3..
+00000810: 0072 1400 0000 7215 0000 0029 01da 1b69  .r....r....)...i
+00000820: 6d70 6f72 7465 645f 656d 6973 7369 6f6e  mported_emission
+00000830: 5f72 6564 7563 7469 6f6e 7217 0000 0072  _reductionr....r
+00000840: 1a00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
+00000850: 0000 004d 0000 0072 1f00 0000 7220 0000  ...M...r....r ..
+00000860: 0072 2100 0000 721a 0000 0072 1c00 0000  .r!...r....r....
+00000870: 721a 0000 0072 1d00 0000 7225 0000 004c  r....r....r%...L
+00000880: 0000 0072 2600 0000 5a38 746f 7461 6c5f  ...r&...Z8total_
+00000890: 696d 706f 7274 6564 5f65 7175 616c 735f  imported_equals_
+000008a0: 746f 7461 6c5f 6578 706f 7274 6564 5f65  total_exported_e
+000008b0: 6d69 7373 696f 6e5f 7265 6475 6374 696f  mission_reductio
+000008c0: 6e73 6303 0000 0000 0000 0000 0000 0003  nsc.............
+000008d0: 0000 0004 0000 0053 0000 0073 3000 0000  .......S...s0...
+000008e0: 7c00 6a00 7c01 7c02 6602 1900 7c00 6a01  |.j.|.|.f...|.j.
+000008f0: 7c01 7c02 6602 1900 7c00 6a02 7c01 1900  |.|.f...|.j.|...
+00000900: 1400 7c00 6a03 7c01 1900 1b00 6b02 5300  ..|.j.|.....k.S.
+00000910: 7215 0000 0029 04da 2169 6d70 6f72 7465  r....)..!importe
+00000920: 645f 656d 6973 7369 6f6e 5f72 6564 7563  d_emission_reduc
+00000930: 7469 6f6e 5f63 6f73 7473 7229 0000 0072  tion_costsr)...r
+00000940: 2800 0000 7222 0000 00a9 0372 0c00 0000  (...r".....r....
+00000950: 721b 0000 0072 1900 0000 721c 0000 0072  r....r....r....r
+00000960: 1c00 0000 721d 0000 0072 2500 0000 5700  ....r....r%...W.
+00000970: 0000 730e 0000 000c 000c 0108 0102 ff08  ..s.............
+00000980: 0202 fe04 ff5a 2663 6f73 7473 5f66 6f72  .....Z&costs_for
+00000990: 5f69 6d70 6f72 7465 645f 656d 6973 7369  _imported_emissi
+000009a0: 6f6e 5f72 6564 7563 7469 6f6e 7363 0300  on_reductionsc..
+000009b0: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+000009c0: 0000 5300 0000 7342 0000 007c 006a 007c  ..S...sB...|.j.|
+000009d0: 017c 0266 0219 0074 017c 006a 027c 017c  .|.f...t.|.j.|.|
+000009e0: 0266 0219 007c 006a 037c 017c 0266 0219  .f...|.j.|.|.f..
+000009f0: 001b 007c 007c 017c 0283 047c 006a 037c  ...|.|.|...|.j.|
+00000a00: 017c 0266 0219 0014 006b 0253 0072 1500  .|.f.....k.S.r..
+00000a10: 0000 2904 da1c 6f77 6e5f 656d 6973 7369  ..)...own_emissi
+00000a20: 6f6e 5f72 6564 7563 7469 6f6e 5f63 6f73  on_reduction_cos
+00000a30: 7473 720b 0000 00da 166f 776e 5f65 6d69  tsr......own_emi
+00000a40: 7373 696f 6e5f 7265 6475 6374 696f 6eda  ssion_reduction.
+00000a50: 0862 6173 656c 696e 6572 2b00 0000 721c  .baseliner+...r.
+00000a60: 0000 0072 1c00 0000 721d 0000 0072 2500  ...r....r....r%.
+00000a70: 0000 5f00 0000 730a 0000 000c 0024 010c  .._...s......$..
+00000a80: 0102 ff04 ff5a 1d63 6f73 7473 5f6f 776e  .....Z.costs_own
+00000a90: 5f65 6d69 7373 696f 6e5f 7265 6475 6374  _emission_reduct
+00000aa0: 696f 6e73 6303 0000 0000 0000 0000 0000  ionsc...........
+00000ab0: 0003 0000 0005 0000 0053 0000 0073 2a00  .........S...s*.
+00000ac0: 0000 7c00 6a00 7c01 7c02 6602 1900 7c00  ..|.j.|.|.f...|.
+00000ad0: 6a01 7c01 7c02 6602 1900 7c00 6a02 7c01  j.|.|.f...|.j.|.
+00000ae0: 7c02 6602 1900 1700 6b02 5300 7215 0000  |.f.....k.S.r...
+00000af0: 0029 03da 1961 6374 7561 6c5f 656d 6973  .)...actual_emis
+00000b00: 7369 6f6e 5f72 6564 7563 7469 6f6e 722d  sion_reductionr-
+00000b10: 0000 0072 1600 0000 722b 0000 0072 1c00  ...r....r+...r..
+00000b20: 0000 721c 0000 0072 1d00 0000 7225 0000  ..r....r....r%..
+00000b30: 0068 0000 00f3 0600 0000 0c00 1a01 04ff  .h..............
+00000b40: 722f 0000 0063 0300 0000 0000 0000 0000  r/...c..........
+00000b50: 0000 0300 0000 0600 0000 5300 0000 7350  ..........S...sP
+00000b60: 0000 007c 006a 007c 017c 0266 0219 0074  ...|.j.|.|.f...t
+00000b70: 017c 006a 027c 017c 0266 0219 007c 006a  .|.j.|.|.f...|.j
+00000b80: 037c 017c 0266 0219 001b 007c 007c 017c  .|.|.f.....|.|.|
+00000b90: 0283 047c 006a 037c 017c 0266 0219 0014  ...|.j.|.|.f....
+00000ba0: 007c 006a 047c 017c 0266 0219 0018 006b  .|.j.|.|.f.....k
+00000bb0: 0253 0072 1500 0000 2905 7227 0000 0072  .S.r....).r'...r
+00000bc0: 0b00 0000 722f 0000 0072 2e00 0000 722c  ....r/...r....r,
+00000bd0: 0000 0072 2b00 0000 721c 0000 0072 1c00  ...r+...r....r..
+00000be0: 0000 721d 0000 0072 2500 0000 6d00 0000  ..r....r%...m...
+00000bf0: 7318 0000 000c 0002 011a 0102 0102 0102  s...............
+00000c00: 0102 fc0c 0602 fa0c 0702 f904 ff5a 2263  .............Z"c
+00000c10: 6f73 7473 5f65 7870 6f72 7465 645f 656d  osts_exported_em
+00000c20: 6973 7369 6f6e 5f72 6564 7563 7469 6f6e  ission_reduction
+00000c30: 7363 0300 0000 0000 0000 0000 0000 0300  sc..............
+00000c40: 0000 0500 0000 5300 0000 732a 0000 007c  ......S...s*...|
+00000c50: 006a 007c 017c 0266 0219 007c 006a 017c  .j.|.|.f...|.j.|
+00000c60: 017c 0266 0219 007c 006a 027c 017c 0266  .|.f...|.j.|.|.f
+00000c70: 0219 001b 006b 0253 0072 1500 0000 2903  .....k.S.r....).
+00000c80: da12 7265 6c61 7469 7665 5f61 6261 7465  ..relative_abate
+00000c90: 6d65 6e74 722f 0000 0072 2e00 0000 722b  mentr/...r....r+
+00000ca0: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
+00000cb0: 0000 7225 0000 007a 0000 0072 3000 0000  ..r%...z...r0...
+00000cc0: 7231 0000 0063 0300 0000 0000 0000 0000  r1...c..........
+00000cd0: 0000 0300 0000 0600 0000 5300 0000 732e  ..........S...s.
+00000ce0: 0000 007c 006a 007c 017c 0266 0219 007c  ...|.j.|.|.f...|
+00000cf0: 006a 017c 017c 0266 0219 0064 017c 006a  .j.|.|.f...d.|.j
+00000d00: 027c 017c 0266 0219 0014 0017 006b 0253  .|.|.f.......k.S
+00000d10: 0029 024e 6752 b81e 85eb 51f0 3f29 03da  .).NgR....Q.?)..
+00000d20: 106d 6974 6967 6174 696f 6e5f 636f 7374  .mitigation_cost
+00000d30: 7372 2c00 0000 722a 0000 0072 2b00 0000  sr,...r*...r+...
+00000d40: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00000d50: 2500 0000 7f00 0000 730a 0000 000c 000c  %.......s.......
+00000d60: 0110 0102 ff04 ff72 3200 0000 2912 7209  .......r2...).r.
+00000d70: 0000 00da 0475 6e69 7472 0800 0000 7207  .....unitr....r.
+00000d80: 0000 0072 1b00 0000 7224 0000 0072 2d00  ...r....r$...r-.
+00000d90: 0000 722c 0000 0072 2900 0000 722a 0000  ..r,...r)...r*..
+00000da0: 0072 1600 0000 7227 0000 0072 2f00 0000  .r....r'...r/...
+00000db0: 7222 0000 0072 2800 0000 da06 6578 7465  r"...r(.....exte
+00000dc0: 6e64 7205 0000 0072 0600 0000 2904 720c  ndr....r....).r.
+00000dd0: 0000 00da 0b63 6f6e 7374 7261 696e 7473  .....constraints
+00000de0: 5a0a 6f70 7473 5f65 6d69 7373 5a0a 6f70  Z.opts_emissZ.op
+00000df0: 7473 5f63 6f73 7473 721c 0000 0072 1c00  ts_costsr....r..
+00000e00: 0000 721d 0000 00da 0f67 6574 5f63 6f6e  ..r......get_con
+00000e10: 7374 7261 696e 7473 1700 0000 736e 0000  straints....sn..
+00000e20: 0004 0f10 0310 0118 0318 0118 0318 011c  ................
+00000e30: 0318 0118 0314 0314 0104 0202 0206 0102  ................
+00000e40: 0202 fd02 0506 0102 0202 fd02 0506 0102  ................
+00000e50: 0202 fd02 f504 ff04 1402 0306 0102 0402  ................
+00000e60: fb02 0806 0102 0302 fc02 0906 0102 0202  ................
+00000e70: fd02 0506 0102 0902 f602 0d06 0102 0202  ................
+00000e80: fd02 0506 0102 0302 fc02 d604 ff04 3472  ..............4r
+00000e90: 3600 0000 4e29 0fda 075f 5f64 6f63 5f5f  6...N)...__doc__
+00000ea0: da06 7479 7069 6e67 7202 0000 00da 0d6d  ..typingr......m
+00000eb0: 696d 6f73 612e 636f 6d6d 6f6e 7203 0000  imosa.commonr...
+00000ec0: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
+00000ed0: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+00000ee0: 0a00 0000 da1c 6d69 6d6f 7361 2e63 6f6d  ......mimosa.com
+00000ef0: 706f 6e65 6e74 732e 6d69 7469 6761 7469  ponents.mitigati
+00000f00: 6f6e 720b 0000 0072 3600 0000 721c 0000  onr....r6...r...
+00000f10: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+00000f20: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+00000f30: 0000 0004 000c 0628 020c 0b1a 03         .......(.....
```

### Comparing `mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 3276 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 cc0c 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 8aa0 ba64 d20c 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6401 6404 6c0d  m.Z.m.Z...d.d.l.
 00000070: 6d0e 5a0e 0100 6405 6504 6406 6502 6507  m.Z...d.e.d.e.e.
@@ -33,154 +33,154 @@
 00000200: 7c00 6a01 7c00 6a02 7404 a005 6409 a101  |.j.|.j.t...d...
 00000210: 640a 8d03 7c00 5f0b 7400 7c00 6a01 7c00  d...|._.t.|.j.|.
 00000220: 6a02 7404 a005 6402 a101 640a 8d03 7c00  j.t...d...d...|.
 00000230: 5f0c 7c01 a007 7408 640b 6405 8400 640c  _.|...t.d.d...d.
 00000240: 8302 7408 640d 6405 8400 640e 8302 7408  ..t.d.d...d...t.
 00000250: 640f 6405 8400 6410 8302 6703 a101 0100  d.d...d...g.....
 00000260: 740d 8300 7c00 5f0e 740d 8300 7c00 5f0f  t...|._.t...|._.
-00000270: 7c01 5300 2911 6176 0100 0045 6d69 7373  |.S.).av...Emiss
+00000270: 7c01 5300 2911 6177 0100 0045 6d69 7373  |.S.).aw...Emiss
 00000280: 696f 6e20 7472 6164 696e 6720 6571 7561  ion trading equa
 00000290: 7469 6f6e 7320 616e 6420 636f 6e73 7472  tions and constr
 000002a0: 6169 6e74 730a 2020 2020 2867 6c6f 6261  aints.    (globa
 000002b0: 6c20 636f 7374 2070 6f6f 6c20 7370 6563  l cost pool spec
 000002c0: 6966 6963 6174 696f 6e29 0a0a 2020 2020  ification)..    
 000002d0: 4e65 6365 7373 6172 7920 7661 7269 6162  Necessary variab
-000002e0: 6c65 733a 0a20 2020 2020 2020 206d 2e61  les:.        m.a
-000002f0: 6261 7465 6d65 6e74 5f63 6f73 7473 2028  batement_costs (
-00000300: 6162 6174 656d 656e 7420 636f 7374 7320  abatement costs 
-00000310: 6173 2070 6169 6420 666f 7220 6279 2074  as paid for by t
-00000320: 6869 7320 7265 6769 6f6e 290a 0a20 2020  his region)..   
-00000330: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00000340: 2020 6c69 7374 206f 6620 636f 6e73 7472    list of constr
-00000350: 6169 6e74 7320 2861 6e79 206f 663a 0a20  aints (any of:. 
-00000360: 2020 2020 2020 2020 2020 2d20 476c 6f62            - Glob
-00000370: 616c 436f 6e73 7472 6169 6e74 0a20 2020  alConstraint.   
-00000380: 2020 2020 2020 2020 2d20 476c 6f62 616c          - Global
-00000390: 496e 6974 436f 6e73 7472 6169 6e74 0a20  InitConstraint. 
-000003a0: 2020 2020 2020 2020 2020 2d20 5265 6769            - Regi
-000003b0: 6f6e 616c 436f 6e73 7472 6169 6e74 0a20  onalConstraint. 
-000003c0: 2020 2020 2020 2020 2020 2d20 5265 6769            - Regi
-000003d0: 6f6e 616c 496e 6974 436f 6e73 7472 6169  onalInitConstrai
-000003e0: 6e74 0a20 2020 2020 2020 2029 0a20 2020  nt.        ).   
-000003f0: 2072 0100 0000 da0d 6375 7272 656e 6379   r......currency
-00000400: 5f75 6e69 7429 03da 0677 6974 6869 6eda  _unit)...within.
-00000410: 0a69 6e69 7469 616c 697a 65da 0575 6e69  .initialize..uni
-00000420: 7473 6303 0000 0000 0000 0000 0000 0003  tsc.............
-00000430: 0000 0006 0000 0053 0000 0073 3400 0000  .......S...s4...
-00000440: 7c00 6a00 7c01 7c02 6602 1900 7401 7c00  |.j.|.|.f...t.|.
-00000450: 6a02 7c01 7c02 6602 1900 7c00 7c01 7c02  j.|.|.f...|.|.|.
-00000460: 8304 7c00 6a03 7c01 7c02 6602 1900 1400  ..|.j.|.|.f.....
-00000470: 6b02 5300 a901 4e29 04da 0e61 7265 615f  k.S...N)...area_
-00000480: 756e 6465 725f 4d41 4372 0c00 0000 da12  under_MACr......
-00000490: 7265 6c61 7469 7665 5f61 6261 7465 6d65  relative_abateme
-000004a0: 6e74 da08 6261 7365 6c69 6e65 a903 720d  nt..baseline..r.
-000004b0: 0000 00da 0174 da01 72a9 0072 1a00 0000  .....t..r..r....
-000004c0: fa73 633a 5c75 7365 7273 5c33 3930 3338  .sc:\users\39038
-000004d0: 3835 5c6f 6e65 6472 6976 6520 2d20 756e  85\onedrive - un
-000004e0: 6976 6572 7369 7465 6974 2075 7472 6563  iversiteit utrec
-000004f0: 6874 5c64 6f63 756d 656e 7473 5c6d 696d  ht\documents\mim
-00000500: 6f73 615c 6d69 6d6f 7361 5c63 6f6d 706f  osa\mimosa\compo
-00000510: 6e65 6e74 735c 656d 6973 7369 6f6e 7472  nents\emissiontr
-00000520: 6164 655c 676c 6f62 616c 636f 7374 706f  ade\globalcostpo
-00000530: 6f6c 2e70 79da 083c 6c61 6d62 6461 3e34  ol.py..<lambda>4
-00000540: 0000 0073 0600 0000 0c00 2401 04ff 7a21  ...s......$...z!
-00000550: 6765 745f 636f 6e73 7472 6169 6e74 732e  get_constraints.
-00000560: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00000570: 3eda 0f61 6261 7465 6d65 6e74 5f63 6f73  >..abatement_cos
-00000580: 7473 6302 0000 0000 0000 0000 0000 0002  tsc.............
-00000590: 0000 0005 0000 0013 0000 0073 3400 0000  ...........s4...
-000005a0: 7400 8700 8701 6602 6401 6402 8408 8800  t.....f.d.d.....
-000005b0: 6a01 4400 8301 8301 7400 8700 8701 6602  j.D.....t.....f.
-000005c0: 6403 6402 8408 8800 6a01 4400 8301 8301  d.d.....j.D.....
-000005d0: 6b02 5300 2904 4e63 0100 0000 0000 0000  k.S.).Nc........
-000005e0: 0000 0000 0200 0000 0400 0000 3300 0000  ............3...
-000005f0: f31e 0000 0081 007c 005d 0a7d 0188 006a  .......|.].}...j
-00000600: 0088 017c 0166 0219 0056 0001 0071 0264  ...|.f...V...q.d
-00000610: 0053 0072 1300 0000 2901 721d 0000 00a9  .S.r....).r.....
-00000620: 02da 022e 3072 1900 0000 a902 720d 0000  ....0r......r...
-00000630: 0072 1800 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000640: da09 3c67 656e 6578 7072 3e39 0000 00f3  ..<genexpr>9....
-00000650: 0400 0000 0280 1c00 7a34 6765 745f 636f  ........z4get_co
-00000660: 6e73 7472 6169 6e74 732e 3c6c 6f63 616c  nstraints.<local
-00000670: 733e 2e3c 6c61 6d62 6461 3e2e 3c6c 6f63  s>.<lambda>.<loc
-00000680: 616c 733e 2e3c 6765 6e65 7870 723e 6301  als>.<genexpr>c.
-00000690: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000006a0: 0000 0033 0000 0072 1e00 0000 7213 0000  ...3...r....r...
-000006b0: 0029 0172 1400 0000 721f 0000 0072 2100  .).r....r....r!.
-000006c0: 0000 721a 0000 0072 1b00 0000 7222 0000  ..r....r....r"..
-000006d0: 003a 0000 0072 2300 0000 2902 da03 7375  .:...r#...)...su
-000006e0: 6dda 0772 6567 696f 6e73 7221 0000 0072  m..regionsr!...r
-000006f0: 1a00 0000 7221 0000 0072 1b00 0000 721c  ....r!...r....r.
-00000700: 0000 0039 0000 0073 0600 0000 1800 1801  ...9...s........
-00000710: 04ff 5a27 7375 6d5f 6162 6174 656d 656e  ..Z'sum_abatemen
-00000720: 745f 6571 7561 6c73 5f73 756d 5f61 7265  t_equals_sum_are
-00000730: 615f 756e 6465 725f 6d61 63da 1265 6d69  a_under_mac..emi
-00000740: 7373 696f 6e73 7261 7465 5f75 6e69 7429  ssionsrate_unit)
-00000750: 0172 1200 0000 6303 0000 0000 0000 0000  .r....c.........
-00000760: 0000 0003 0000 0004 0000 0053 0000 0073  ...........S...s
-00000770: 3400 0000 7c01 6401 6b04 7217 7c00 6a00  4...|.d.k.r.|.j.
-00000780: 7c01 7c02 6602 1900 7c00 6a01 7c01 7c02  |.|.f...|.j.|.|.
-00000790: 6602 1900 7c00 6a02 7c01 1900 1400 6b02  f...|.j.|.....k.
-000007a0: 5300 7403 6a04 5300 a902 4e72 0100 0000  S.t.j.S...Nr....
-000007b0: 2905 da1c 7061 6964 5f66 6f72 5f65 6d69  )...paid_for_emi
-000007c0: 7373 696f 6e5f 7265 6475 6374 696f 6e73  ssion_reductions
-000007d0: 721d 0000 00da 2767 6c6f 6261 6c5f 656d  r.....'global_em
-000007e0: 6973 7369 6f6e 5f72 6564 7563 7469 6f6e  ission_reduction
-000007f0: 5f70 6572 5f63 6f73 745f 756e 6974 7209  _per_cost_unitr.
-00000800: 0000 00da 0453 6b69 7072 1700 0000 721a  .....Skipr....r.
-00000810: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000820: 0000 4e00 0000 730e 0000 0008 030c fd0c  ..N...s.........
-00000830: 0108 0102 ff04 ff06 0472 2800 0000 6303  .........r(...c.
-00000840: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00000850: 0000 0053 0000 0073 3800 0000 7c01 6401  ...S...s8...|.d.
-00000860: 6b04 7219 7c00 6a00 7c01 7c02 6602 1900  k.r.|.j.|.|.f...
-00000870: 7c00 6a01 7c01 7c02 6602 1900 7c00 6a02  |.j.|.|.f...|.j.
-00000880: 7c01 7c02 6602 1900 1800 6b02 5300 7403  |.|.f.....k.S.t.
-00000890: 6a04 5300 7227 0000 0029 05da 2869 6d70  j.S.r'...)..(imp
-000008a0: 6f72 745f 6578 706f 7274 5f65 6d69 7373  ort_export_emiss
-000008b0: 696f 6e5f 7265 6475 6374 696f 6e5f 6261  ion_reduction_ba
-000008c0: 6c61 6e63 6572 2800 0000 da1b 7265 6769  lancer(.....regi
-000008d0: 6f6e 616c 5f65 6d69 7373 696f 6e5f 7265  onal_emission_re
-000008e0: 6475 6374 696f 6e72 0900 0000 722a 0000  ductionr....r*..
-000008f0: 0072 1700 0000 721a 0000 0072 1a00 0000  .r....r....r....
-00000900: 721b 0000 0072 1c00 0000 5700 0000 730e  r....r....W...s.
-00000910: 0000 0008 030c fd0c 010c 0102 ff04 ff06  ................
-00000920: 0472 2b00 0000 6303 0000 0000 0000 0000  .r+...c.........
-00000930: 0000 0003 0000 0005 0000 0053 0000 0073  ...........S...s
-00000940: 2a00 0000 7c00 6a00 7c01 7c02 6602 1900  *...|.j.|.|.f...
-00000950: 7c00 6a01 7c01 7c02 6602 1900 7c00 6a02  |.j.|.|.f...|.j.
-00000960: 7c01 7c02 6602 1900 1800 6b02 5300 7213  |.|.f.....k.S.r.
-00000970: 0000 0029 03da 2569 6d70 6f72 745f 6578  ...)..%import_ex
-00000980: 706f 7274 5f6d 6974 6967 6174 696f 6e5f  port_mitigation_
-00000990: 636f 7374 5f62 616c 616e 6365 721d 0000  cost_balancer...
-000009a0: 0072 1400 0000 7217 0000 0072 1a00 0000  .r....r....r....
-000009b0: 721a 0000 0072 1b00 0000 721c 0000 005f  r....r....r...._
-000009c0: 0000 0073 0600 0000 0c00 1a01 04ff 722d  ...s..........r-
-000009d0: 0000 0029 1072 0400 0000 7218 0000 0072  ...).r....r....r
-000009e0: 2500 0000 720a 0000 0072 0b00 0000 da04  %...r....r......
-000009f0: 756e 6974 7214 0000 00da 0665 7874 656e  unitr......exten
-00000a00: 6472 0800 0000 7207 0000 0072 2800 0000  dr....r....r(...
-00000a10: 722b 0000 0072 2d00 0000 7205 0000 005a  r+...r-...r....Z
-00000a20: 156d 696e 5f72 656c 5f70 6179 6d65 6e74  .min_rel_payment
-00000a30: 5f6c 6576 656c 5a15 6d61 785f 7265 6c5f  _levelZ.max_rel_
-00000a40: 7061 796d 656e 745f 6c65 7665 6c29 0272  payment_level).r
-00000a50: 0d00 0000 da0b 636f 6e73 7472 6169 6e74  ......constraint
-00000a60: 7372 1a00 0000 721a 0000 0072 1b00 0000  sr....r....r....
-00000a70: da0f 6765 745f 636f 6e73 7472 6169 6e74  ..get_constraint
-00000a80: 7317 0000 0073 5c00 0000 040f 0202 0401  s....s\.........
-00000a90: 0401 0201 0201 0801 08fb 0409 0202 0601  ................
-00000aa0: 0202 02fd 0205 0601 0202 02fd 02fa 04ff  ................
-00000ab0: 0211 1001 08ff 0203 1001 08ff 0203 1001  ................
-00000ac0: 08ff 0403 0202 0601 0205 02fa 0209 0601  ................
-00000ad0: 0205 02fa 0208 0601 0202 02fd 02ee 04ff  ................
-00000ae0: 081c 0801 0402 7231 0000 004e 2910 da07  ......r1...N)...
-00000af0: 5f5f 646f 635f 5fda 0674 7970 696e 6772  __doc__..typingr
-00000b00: 0200 0000 da0d 6d69 6d6f 7361 2e63 6f6d  ......mimosa.com
-00000b10: 6d6f 6e72 0300 0000 7204 0000 0072 0500  monr....r....r..
-00000b20: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-00000b30: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000b40: 5a1b 6d69 6d6f 7361 2e63 6f6d 706f 6e65  Z.mimosa.compone
-00000b50: 6e74 732e 6162 6174 656d 656e 7472 0c00  nts.abatementr..
-00000b60: 0000 7231 0000 0072 1a00 0000 721a 0000  ..r1...r....r...
-00000b70: 0072 1a00 0000 721b 0000 00da 083c 6d6f  .r....r......<mo
-00000b80: 6475 6c65 3e01 0000 0073 0a00 0000 0400  dule>....s......
-00000b90: 0c06 2c01 0c0c 1a03                      ..,.....
+000002e0: 6c65 733a 0a20 2020 2020 2020 206d 2e6d  les:.        m.m
+000002f0: 6974 6967 6174 696f 6e5f 636f 7374 7320  itigation_costs 
+00000300: 2861 6261 7465 6d65 6e74 2063 6f73 7473  (abatement costs
+00000310: 2061 7320 7061 6964 2066 6f72 2062 7920   as paid for by 
+00000320: 7468 6973 2072 6567 696f 6e29 0a0a 2020  this region)..  
+00000330: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00000340: 2020 206c 6973 7420 6f66 2063 6f6e 7374     list of const
+00000350: 7261 696e 7473 2028 616e 7920 6f66 3a0a  raints (any of:.
+00000360: 2020 2020 2020 2020 2020 202d 2047 6c6f             - Glo
+00000370: 6261 6c43 6f6e 7374 7261 696e 740a 2020  balConstraint.  
+00000380: 2020 2020 2020 2020 202d 2047 6c6f 6261           - Globa
+00000390: 6c49 6e69 7443 6f6e 7374 7261 696e 740a  lInitConstraint.
+000003a0: 2020 2020 2020 2020 2020 202d 2052 6567             - Reg
+000003b0: 696f 6e61 6c43 6f6e 7374 7261 696e 740a  ionalConstraint.
+000003c0: 2020 2020 2020 2020 2020 202d 2052 6567             - Reg
+000003d0: 696f 6e61 6c49 6e69 7443 6f6e 7374 7261  ionalInitConstra
+000003e0: 696e 740a 2020 2020 2020 2020 290a 2020  int.        ).  
+000003f0: 2020 7201 0000 00da 0d63 7572 7265 6e63    r......currenc
+00000400: 795f 756e 6974 2903 da06 7769 7468 696e  y_unit)...within
+00000410: da0a 696e 6974 6961 6c69 7a65 da05 756e  ..initialize..un
+00000420: 6974 7363 0300 0000 0000 0000 0000 0000  itsc............
+00000430: 0300 0000 0600 0000 5300 0000 7334 0000  ........S...s4..
+00000440: 007c 006a 007c 017c 0266 0219 0074 017c  .|.j.|.|.f...t.|
+00000450: 006a 027c 017c 0266 0219 007c 007c 017c  .j.|.|.f...|.|.|
+00000460: 0283 047c 006a 037c 017c 0266 0219 0014  ...|.j.|.|.f....
+00000470: 006b 0253 00a9 014e 2904 da0e 6172 6561  .k.S...N)...area
+00000480: 5f75 6e64 6572 5f4d 4143 720c 0000 00da  _under_MACr.....
+00000490: 1272 656c 6174 6976 655f 6162 6174 656d  .relative_abatem
+000004a0: 656e 74da 0862 6173 656c 696e 65a9 0372  ent..baseline..r
+000004b0: 0d00 0000 da01 74da 0172 a900 721a 0000  ......t..r..r...
+000004c0: 00fa 7363 3a5c 5573 6572 735c 3339 3033  ..sc:\Users\3903
+000004d0: 3838 355c 4f6e 6544 7269 7665 202d 2055  885\OneDrive - U
+000004e0: 6e69 7665 7273 6974 6569 7420 5574 7265  niversiteit Utre
+000004f0: 6368 745c 446f 6375 6d65 6e74 735c 4d49  cht\Documents\MI
+00000500: 4d4f 5341 5c6d 696d 6f73 615c 636f 6d70  MOSA\mimosa\comp
+00000510: 6f6e 656e 7473 5c65 6d69 7373 696f 6e74  onents\emissiont
+00000520: 7261 6465 5c67 6c6f 6261 6c63 6f73 7470  rade\globalcostp
+00000530: 6f6f 6c2e 7079 da08 3c6c 616d 6264 613e  ool.py..<lambda>
+00000540: 3400 0000 7306 0000 000c 0024 0104 ff7a  4...s......$...z
+00000550: 2167 6574 5f63 6f6e 7374 7261 696e 7473  !get_constraints
+00000560: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00000570: 613e da10 6d69 7469 6761 7469 6f6e 5f63  a>..mitigation_c
+00000580: 6f73 7473 6302 0000 0000 0000 0000 0000  ostsc...........
+00000590: 0002 0000 0005 0000 0013 0000 0073 3400  .............s4.
+000005a0: 0000 7400 8700 8701 6602 6401 6402 8408  ..t.....f.d.d...
+000005b0: 8800 6a01 4400 8301 8301 7400 8700 8701  ..j.D.....t.....
+000005c0: 6602 6403 6402 8408 8800 6a01 4400 8301  f.d.d.....j.D...
+000005d0: 8301 6b02 5300 2904 4e63 0100 0000 0000  ..k.S.).Nc......
+000005e0: 0000 0000 0000 0200 0000 0400 0000 3300  ..............3.
+000005f0: 0000 f31e 0000 0081 007c 005d 0a7d 0188  .........|.].}..
+00000600: 006a 0088 017c 0166 0219 0056 0001 0071  .j...|.f...V...q
+00000610: 0264 0053 0072 1300 0000 2901 721d 0000  .d.S.r....).r...
+00000620: 00a9 02da 022e 3072 1900 0000 a902 720d  ......0r......r.
+00000630: 0000 0072 1800 0000 721a 0000 0072 1b00  ...r....r....r..
+00000640: 0000 da09 3c67 656e 6578 7072 3e39 0000  ....<genexpr>9..
+00000650: 00f3 0400 0000 0280 1c00 7a34 6765 745f  ..........z4get_
+00000660: 636f 6e73 7472 6169 6e74 732e 3c6c 6f63  constraints.<loc
+00000670: 616c 733e 2e3c 6c61 6d62 6461 3e2e 3c6c  als>.<lambda>.<l
+00000680: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+00000690: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000006a0: 0004 0000 0033 0000 0072 1e00 0000 7213  .....3...r....r.
+000006b0: 0000 0029 0172 1400 0000 721f 0000 0072  ...).r....r....r
+000006c0: 2100 0000 721a 0000 0072 1b00 0000 7222  !...r....r....r"
+000006d0: 0000 003a 0000 0072 2300 0000 2902 da03  ...:...r#...)...
+000006e0: 7375 6dda 0772 6567 696f 6e73 7221 0000  sum..regionsr!..
+000006f0: 0072 1a00 0000 7221 0000 0072 1b00 0000  .r....r!...r....
+00000700: 721c 0000 0039 0000 0073 0600 0000 1800  r....9...s......
+00000710: 1801 04ff 5a27 7375 6d5f 6162 6174 656d  ....Z'sum_abatem
+00000720: 656e 745f 6571 7561 6c73 5f73 756d 5f61  ent_equals_sum_a
+00000730: 7265 615f 756e 6465 725f 6d61 63da 1265  rea_under_mac..e
+00000740: 6d69 7373 696f 6e73 7261 7465 5f75 6e69  missionsrate_uni
+00000750: 7429 0172 1200 0000 6303 0000 0000 0000  t).r....c.......
+00000760: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
+00000770: 0073 3400 0000 7c01 6401 6b04 7217 7c00  .s4...|.d.k.r.|.
+00000780: 6a00 7c01 7c02 6602 1900 7c00 6a01 7c01  j.|.|.f...|.j.|.
+00000790: 7c02 6602 1900 7c00 6a02 7c01 1900 1400  |.f...|.j.|.....
+000007a0: 6b02 5300 7403 6a04 5300 a902 4e72 0100  k.S.t.j.S...Nr..
+000007b0: 0000 2905 da1c 7061 6964 5f66 6f72 5f65  ..)...paid_for_e
+000007c0: 6d69 7373 696f 6e5f 7265 6475 6374 696f  mission_reductio
+000007d0: 6e73 721d 0000 005a 2767 6c6f 6261 6c5f  nsr....Z'global_
+000007e0: 656d 6973 7369 6f6e 5f72 6564 7563 7469  emission_reducti
+000007f0: 6f6e 5f70 6572 5f63 6f73 745f 756e 6974  on_per_cost_unit
+00000800: 7209 0000 00da 0453 6b69 7072 1700 0000  r......Skipr....
+00000810: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00000820: 1c00 0000 4e00 0000 730e 0000 0008 030c  ....N...s.......
+00000830: fd0c 0108 0102 ff04 ff06 0472 2800 0000  ...........r(...
+00000840: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00000850: 0005 0000 0053 0000 0073 3800 0000 7c01  .....S...s8...|.
+00000860: 6401 6b04 7219 7c00 6a00 7c01 7c02 6602  d.k.r.|.j.|.|.f.
+00000870: 1900 7c00 6a01 7c01 7c02 6602 1900 7c00  ..|.j.|.|.f...|.
+00000880: 6a02 7c01 7c02 6602 1900 1800 6b02 5300  j.|.|.f.....k.S.
+00000890: 7403 6a04 5300 7227 0000 0029 05da 2869  t.j.S.r'...)..(i
+000008a0: 6d70 6f72 745f 6578 706f 7274 5f65 6d69  mport_export_emi
+000008b0: 7373 696f 6e5f 7265 6475 6374 696f 6e5f  ssion_reduction_
+000008c0: 6261 6c61 6e63 6572 2800 0000 da1b 7265  balancer(.....re
+000008d0: 6769 6f6e 616c 5f65 6d69 7373 696f 6e5f  gional_emission_
+000008e0: 7265 6475 6374 696f 6e72 0900 0000 7229  reductionr....r)
+000008f0: 0000 0072 1700 0000 721a 0000 0072 1a00  ...r....r....r..
+00000900: 0000 721b 0000 0072 1c00 0000 5700 0000  ..r....r....W...
+00000910: 730e 0000 0008 030c fd0c 010c 0102 ff04  s...............
+00000920: ff06 0472 2a00 0000 6303 0000 0000 0000  ...r*...c.......
+00000930: 0000 0000 0003 0000 0005 0000 0053 0000  .............S..
+00000940: 0073 2a00 0000 7c00 6a00 7c01 7c02 6602  .s*...|.j.|.|.f.
+00000950: 1900 7c00 6a01 7c01 7c02 6602 1900 7c00  ..|.j.|.|.f...|.
+00000960: 6a02 7c01 7c02 6602 1900 1800 6b02 5300  j.|.|.f.....k.S.
+00000970: 7213 0000 0029 03da 2569 6d70 6f72 745f  r....)..%import_
+00000980: 6578 706f 7274 5f6d 6974 6967 6174 696f  export_mitigatio
+00000990: 6e5f 636f 7374 5f62 616c 616e 6365 721d  n_cost_balancer.
+000009a0: 0000 0072 1400 0000 7217 0000 0072 1a00  ...r....r....r..
+000009b0: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+000009c0: 005f 0000 0073 0600 0000 0c00 1a01 04ff  ._...s..........
+000009d0: 722c 0000 0029 1072 0400 0000 7218 0000  r,...).r....r...
+000009e0: 0072 2500 0000 720a 0000 0072 0b00 0000  .r%...r....r....
+000009f0: da04 756e 6974 7214 0000 00da 0665 7874  ..unitr......ext
+00000a00: 656e 6472 0800 0000 7207 0000 0072 2800  endr....r....r(.
+00000a10: 0000 722a 0000 0072 2c00 0000 7205 0000  ..r*...r,...r...
+00000a20: 005a 156d 696e 5f72 656c 5f70 6179 6d65  .Z.min_rel_payme
+00000a30: 6e74 5f6c 6576 656c 5a15 6d61 785f 7265  nt_levelZ.max_re
+00000a40: 6c5f 7061 796d 656e 745f 6c65 7665 6c29  l_payment_level)
+00000a50: 0272 0d00 0000 da0b 636f 6e73 7472 6169  .r......constrai
+00000a60: 6e74 7372 1a00 0000 721a 0000 0072 1b00  ntsr....r....r..
+00000a70: 0000 da0f 6765 745f 636f 6e73 7472 6169  ....get_constrai
+00000a80: 6e74 7317 0000 0073 5c00 0000 040f 0202  nts....s\.......
+00000a90: 0401 0401 0201 0201 0801 08fb 0409 0202  ................
+00000aa0: 0601 0202 02fd 0205 0601 0202 02fd 02fa  ................
+00000ab0: 04ff 0211 1001 08ff 0203 1001 08ff 0203  ................
+00000ac0: 1001 08ff 0403 0202 0601 0205 02fa 0209  ................
+00000ad0: 0601 0205 02fa 0208 0601 0202 02fd 02ee  ................
+00000ae0: 04ff 081c 0801 0402 7230 0000 004e 2910  ........r0...N).
+00000af0: da07 5f5f 646f 635f 5fda 0674 7970 696e  ..__doc__..typin
+00000b00: 6772 0200 0000 da0d 6d69 6d6f 7361 2e63  gr......mimosa.c
+00000b10: 6f6d 6d6f 6e72 0300 0000 7204 0000 0072  ommonr....r....r
+00000b20: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
+00000b30: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
+00000b40: 0000 5a1c 6d69 6d6f 7361 2e63 6f6d 706f  ..Z.mimosa.compo
+00000b50: 6e65 6e74 732e 6d69 7469 6761 7469 6f6e  nents.mitigation
+00000b60: 720c 0000 0072 3000 0000 721a 0000 0072  r....r0...r....r
+00000b70: 1a00 0000 721a 0000 0072 1b00 0000 da08  ....r....r......
+00000b80: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+00000b90: 0004 000c 062c 010c 0c1a 03              .....,.....
```

### Comparing `mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 1131 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 6b04 0000  o........6.dk...
+00000000: 6f0d 0d0a 0000 0000 0fa0 ba64 6f04 0000  o..........do...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6504 6406 6502 6505 1900 6604  ..d.e.d.e.e...f.
 00000070: 6407 6408 8404 5a0a 6409 5300 290a 7a49  d.d...Z.d.S.).zI
@@ -17,73 +17,73 @@
 00000100: 5265 6769 6f6e 616c 436f 6e73 7472 6169  RegionalConstrai
 00000110: 6e74 da05 5061 7261 6d29 01da 0241 43da  nt..Param)...AC.
 00000120: 016d da06 7265 7475 726e 6301 0000 0000  .m..returnc.....
 00000130: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
 00000140: 0000 0073 3200 0000 6700 7d01 7400 7c00  ...s2...g.}.t.|.
 00000150: 6a01 7c00 6a02 6401 6402 8d03 7c00 5f03  j.|.j.d.d...|._.
 00000160: 7c01 a004 7405 6403 6404 8400 6405 8302  |...t.d.d...d...
-00000170: 6701 a101 0100 7c01 5300 2906 616e 0100  g.....|.S.).an..
+00000170: 6701 a101 0100 7c01 5300 2906 616f 0100  g.....|.S.).ao..
 00000180: 0045 6d69 7373 696f 6e20 7472 6164 696e  .Emission tradin
 00000190: 6720 6571 7561 7469 6f6e 7320 616e 6420  g equations and 
 000001a0: 636f 6e73 7472 6169 6e74 730a 2020 2020  constraints.    
 000001b0: 286e 6f2d 7472 6164 6520 7370 6563 6966  (no-trade specif
 000001c0: 6963 6174 696f 6e29 0a0a 2020 2020 4e65  ication)..    Ne
 000001d0: 6365 7373 6172 7920 7661 7269 6162 6c65  cessary variable
-000001e0: 733a 0a20 2020 2020 2020 206d 2e61 6261  s:.        m.aba
-000001f0: 7465 6d65 6e74 5f63 6f73 7473 2028 6162  tement_costs (ab
-00000200: 6174 656d 656e 7420 636f 7374 7320 6173  atement costs as
-00000210: 2070 6169 6420 666f 7220 6279 2074 6869   paid for by thi
-00000220: 7320 7265 6769 6f6e 290a 0a20 2020 2052  s region)..    R
-00000230: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00000240: 6c69 7374 206f 6620 636f 6e73 7472 6169  list of constrai
-00000250: 6e74 7320 2861 6e79 206f 663a 0a20 2020  nts (any of:.   
-00000260: 2020 2020 2020 2020 2d20 476c 6f62 616c          - Global
-00000270: 436f 6e73 7472 6169 6e74 0a20 2020 2020  Constraint.     
-00000280: 2020 2020 2020 2d20 476c 6f62 616c 496e        - GlobalIn
-00000290: 6974 436f 6e73 7472 6169 6e74 0a20 2020  itConstraint.   
-000002a0: 2020 2020 2020 2020 2d20 5265 6769 6f6e          - Region
-000002b0: 616c 436f 6e73 7472 6169 6e74 0a20 2020  alConstraint.   
-000002c0: 2020 2020 2020 2020 2d20 5265 6769 6f6e          - Region
-000002d0: 616c 496e 6974 436f 6e73 7472 6169 6e74  alInitConstraint
-000002e0: 0a20 2020 2020 2020 2029 0a20 2020 2072  .        ).    r
-000002f0: 0100 0000 2901 da0a 696e 6974 6961 6c69  ....)...initiali
-00000300: 7a65 6303 0000 0000 0000 0000 0000 0003  zec.............
-00000310: 0000 0006 0000 0053 0000 0073 3400 0000  .......S...s4...
-00000320: 7c00 6a00 7c01 7c02 6602 1900 7401 7c00  |.j.|.|.f...t.|.
-00000330: 6a02 7c01 7c02 6602 1900 7c00 7c01 7c02  j.|.|.f...|.|.|.
-00000340: 8304 7c00 6a03 7c01 7c02 6602 1900 1400  ..|.j.|.|.f.....
-00000350: 6b02 5300 2901 4e29 04da 0f61 6261 7465  k.S.).N)...abate
-00000360: 6d65 6e74 5f63 6f73 7473 7207 0000 00da  ment_costsr.....
-00000370: 1272 656c 6174 6976 655f 6162 6174 656d  .relative_abatem
-00000380: 656e 74da 0862 6173 656c 696e 6529 0372  ent..baseline).r
-00000390: 0800 0000 da01 74da 0172 a900 7210 0000  ......t..r..r...
-000003a0: 00fa 6c63 3a5c 7573 6572 735c 3339 3033  ..lc:\users\3903
-000003b0: 3838 355c 6f6e 6564 7269 7665 202d 2075  885\onedrive - u
-000003c0: 6e69 7665 7273 6974 6569 7420 7574 7265  niversiteit utre
-000003d0: 6368 745c 646f 6375 6d65 6e74 735c 6d69  cht\documents\mi
-000003e0: 6d6f 7361 5c6d 696d 6f73 615c 636f 6d70  mosa\mimosa\comp
-000003f0: 6f6e 656e 7473 5c65 6d69 7373 696f 6e74  onents\emissiont
-00000400: 7261 6465 5c6e 6f74 7261 6465 2e70 79da  rade\notrade.py.
-00000410: 083c 6c61 6d62 6461 3e23 0000 0073 0600  .<lambda>#...s..
-00000420: 0000 0c00 2401 04ff 7a21 6765 745f 636f  ....$...z!get_co
-00000430: 6e73 7472 6169 6e74 732e 3c6c 6f63 616c  nstraints.<local
-00000440: 733e 2e3c 6c61 6d62 6461 3e72 0b00 0000  s>.<lambda>r....
-00000450: 2906 7206 0000 0072 0e00 0000 da07 7265  ).r....r......re
-00000460: 6769 6f6e 73da 2869 6d70 6f72 745f 6578  gions.(import_ex
-00000470: 706f 7274 5f65 6d69 7373 696f 6e5f 7265  port_emission_re
-00000480: 6475 6374 696f 6e5f 6261 6c61 6e63 65da  duction_balance.
-00000490: 0665 7874 656e 6472 0500 0000 2902 7208  .extendr....).r.
-000004a0: 0000 00da 0b63 6f6e 7374 7261 696e 7473  .....constraints
-000004b0: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-000004c0: 0f67 6574 5f63 6f6e 7374 7261 696e 7473  .get_constraints
-000004d0: 0d00 0000 7314 0000 0004 0f14 0204 0202  ....s...........
-000004e0: 0206 0102 0202 fd02 ff04 ff04 0a72 1700  .............r..
-000004f0: 0000 4e29 0bda 075f 5f64 6f63 5f5f da06  ..N)...__doc__..
-00000500: 7479 7069 6e67 7202 0000 00da 0d6d 696d  typingr......mim
-00000510: 6f73 612e 636f 6d6d 6f6e 7203 0000 0072  osa.commonr....r
-00000520: 0400 0000 7205 0000 0072 0600 0000 5a1b  ....r....r....Z.
-00000530: 6d69 6d6f 7361 2e63 6f6d 706f 6e65 6e74  mimosa.component
-00000540: 732e 6162 6174 656d 656e 7472 0700 0000  s.abatementr....
-00000550: 7217 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000560: 1000 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
-00000570: 6c65 3e01 0000 0073 0a00 0000 0400 0c06  le>....s........
-00000580: 1801 0c02 1a03                           ......
+000001e0: 733a 0a20 2020 2020 2020 206d 2e6d 6974  s:.        m.mit
+000001f0: 6967 6174 696f 6e5f 636f 7374 7320 2861  igation_costs (a
+00000200: 6261 7465 6d65 6e74 2063 6f73 7473 2061  batement costs a
+00000210: 7320 7061 6964 2066 6f72 2062 7920 7468  s paid for by th
+00000220: 6973 2072 6567 696f 6e29 0a0a 2020 2020  is region)..    
+00000230: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00000240: 206c 6973 7420 6f66 2063 6f6e 7374 7261   list of constra
+00000250: 696e 7473 2028 616e 7920 6f66 3a0a 2020  ints (any of:.  
+00000260: 2020 2020 2020 2020 202d 2047 6c6f 6261           - Globa
+00000270: 6c43 6f6e 7374 7261 696e 740a 2020 2020  lConstraint.    
+00000280: 2020 2020 2020 202d 2047 6c6f 6261 6c49         - GlobalI
+00000290: 6e69 7443 6f6e 7374 7261 696e 740a 2020  nitConstraint.  
+000002a0: 2020 2020 2020 2020 202d 2052 6567 696f           - Regio
+000002b0: 6e61 6c43 6f6e 7374 7261 696e 740a 2020  nalConstraint.  
+000002c0: 2020 2020 2020 2020 202d 2052 6567 696f           - Regio
+000002d0: 6e61 6c49 6e69 7443 6f6e 7374 7261 696e  nalInitConstrain
+000002e0: 740a 2020 2020 2020 2020 290a 2020 2020  t.        ).    
+000002f0: 7201 0000 0029 01da 0a69 6e69 7469 616c  r....)...initial
+00000300: 697a 6563 0300 0000 0000 0000 0000 0000  izec............
+00000310: 0300 0000 0600 0000 5300 0000 7334 0000  ........S...s4..
+00000320: 007c 006a 007c 017c 0266 0219 0074 017c  .|.j.|.|.f...t.|
+00000330: 006a 027c 017c 0266 0219 007c 007c 017c  .j.|.|.f...|.|.|
+00000340: 0283 047c 006a 037c 017c 0266 0219 0014  ...|.j.|.|.f....
+00000350: 006b 0253 0029 014e 2904 da10 6d69 7469  .k.S.).N)...miti
+00000360: 6761 7469 6f6e 5f63 6f73 7473 7207 0000  gation_costsr...
+00000370: 00da 1272 656c 6174 6976 655f 6162 6174  ...relative_abat
+00000380: 656d 656e 74da 0862 6173 656c 696e 6529  ement..baseline)
+00000390: 0372 0800 0000 da01 74da 0172 a900 7210  .r......t..r..r.
+000003a0: 0000 00fa 6c63 3a5c 5573 6572 735c 3339  ....lc:\Users\39
+000003b0: 3033 3838 355c 4f6e 6544 7269 7665 202d  03885\OneDrive -
+000003c0: 2055 6e69 7665 7273 6974 6569 7420 5574   Universiteit Ut
+000003d0: 7265 6368 745c 446f 6375 6d65 6e74 735c  recht\Documents\
+000003e0: 4d49 4d4f 5341 5c6d 696d 6f73 615c 636f  MIMOSA\mimosa\co
+000003f0: 6d70 6f6e 656e 7473 5c65 6d69 7373 696f  mponents\emissio
+00000400: 6e74 7261 6465 5c6e 6f74 7261 6465 2e70  ntrade\notrade.p
+00000410: 79da 083c 6c61 6d62 6461 3e23 0000 0073  y..<lambda>#...s
+00000420: 0600 0000 0c00 2401 04ff 7a21 6765 745f  ......$...z!get_
+00000430: 636f 6e73 7472 6169 6e74 732e 3c6c 6f63  constraints.<loc
+00000440: 616c 733e 2e3c 6c61 6d62 6461 3e72 0b00  als>.<lambda>r..
+00000450: 0000 2906 7206 0000 0072 0e00 0000 da07  ..).r....r......
+00000460: 7265 6769 6f6e 73da 2869 6d70 6f72 745f  regions.(import_
+00000470: 6578 706f 7274 5f65 6d69 7373 696f 6e5f  export_emission_
+00000480: 7265 6475 6374 696f 6e5f 6261 6c61 6e63  reduction_balanc
+00000490: 65da 0665 7874 656e 6472 0500 0000 2902  e..extendr....).
+000004a0: 7208 0000 00da 0b63 6f6e 7374 7261 696e  r......constrain
+000004b0: 7473 7210 0000 0072 1000 0000 7211 0000  tsr....r....r...
+000004c0: 00da 0f67 6574 5f63 6f6e 7374 7261 696e  ...get_constrain
+000004d0: 7473 0d00 0000 7314 0000 0004 0f14 0204  ts....s.........
+000004e0: 0202 0206 0102 0202 fd02 ff04 ff04 0a72  ...............r
+000004f0: 1700 0000 4e29 0bda 075f 5f64 6f63 5f5f  ....N)...__doc__
+00000500: da06 7479 7069 6e67 7202 0000 00da 0d6d  ..typingr......m
+00000510: 696d 6f73 612e 636f 6d6d 6f6e 7203 0000  imosa.commonr...
+00000520: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
+00000530: da1c 6d69 6d6f 7361 2e63 6f6d 706f 6e65  ..mimosa.compone
+00000540: 6e74 732e 6d69 7469 6761 7469 6f6e 7207  nts.mitigationr.
+00000550: 0000 0072 1700 0000 7210 0000 0072 1000  ...r....r....r..
+00000560: 0000 7210 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
+00000570: 6f64 756c 653e 0100 0000 730a 0000 0004  odule>....s.....
+00000580: 000c 0618 010c 021a 03                   .........
```

### Comparing `mimosa-0.1.3/mimosa/components/emissiontrade/emissiontrade.py` & `mimosa-0.1.4/mimosa/components/emissiontrade/emissiontrade.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     RegionalConstraint,
     Var,
     NonNegativeReals,
     quant,
     sqrt,
 )
 
-from mimosa.components.abatement import AC
+from mimosa.components.mitigation import AC
 
 
 def get_constraints(m: AbstractModel) -> Sequence[GeneralConstraint]:
     """Emission trading equations and constraints
     (trading of emissions specification)
 
     Necessary variables:
-        m.abatement_costs (abatement costs as paid for by this region)
+        m.mitigation_costs (abatement costs as paid for by this region)
 
     Returns:
         list of constraints (any of:
            - GlobalConstraint
            - GlobalInitConstraint
            - RegionalConstraint
            - RegionalInitConstraint
@@ -120,16 +120,16 @@
             # Actual reductions and actual abatement costs:
             RegionalConstraint(
                 lambda m, t, r: m.relative_abatement[t, r]
                 == m.actual_emission_reduction[t, r] / m.baseline[t, r],
                 "relative_abatement",
             ),
             RegionalConstraint(
-                lambda m, t, r: m.abatement_costs[t, r]
+                lambda m, t, r: m.mitigation_costs[t, r]
                 == m.own_emission_reduction_costs[t, r]
                 + 1.02 * m.imported_emission_reduction_costs[t, r],
-                "abatement_costs",
+                "mitigation_costs",
             ),
         ]
     )
 
     return constraints
```

### Comparing `mimosa-0.1.3/mimosa/components/emissiontrade/globalcostpool.py` & `mimosa-0.1.4/mimosa/components/emissiontrade/globalcostpool.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     GlobalConstraint,
     RegionalConstraint,
     Constraint,
     NonNegativeReals,
     quant,
 )
 
-from mimosa.components.abatement import AC
+from mimosa.components.mitigation import AC
 
 
 def get_constraints(m: AbstractModel) -> Sequence[GeneralConstraint]:
     """Emission trading equations and constraints
     (global cost pool specification)
 
     Necessary variables:
-        m.abatement_costs (abatement costs as paid for by this region)
+        m.mitigation_costs (abatement costs as paid for by this region)
 
     Returns:
         list of constraints (any of:
            - GlobalConstraint
            - GlobalInitConstraint
            - RegionalConstraint
            - RegionalInitConstraint
@@ -47,18 +47,18 @@
 
     # The global mitigation cost pool:
     constraints.extend(
         [
             RegionalConstraint(
                 lambda m, t, r: m.area_under_MAC[t, r]
                 == AC(m.relative_abatement[t, r], m, t, r) * m.baseline[t, r],
-                "abatement_costs",
+                "mitigation_costs",
             ),
             GlobalConstraint(
-                lambda m, t: sum(m.abatement_costs[t, r] for r in m.regions)
+                lambda m, t: sum(m.mitigation_costs[t, r] for r in m.regions)
                 == sum(m.area_under_MAC[t, r] for r in m.regions),
                 "sum_abatement_equals_sum_area_under_mac",
             ),
         ]
     )
 
     ## Extra reporting variables:
@@ -72,15 +72,15 @@
     m.import_export_mitigation_cost_balance = Var(
         m.t, m.regions, units=quant.unit("currency_unit")
     )
     constraints.extend(
         [
             RegionalConstraint(
                 lambda m, t, r: m.paid_for_emission_reductions[t, r]
-                == m.abatement_costs[t, r]
+                == m.mitigation_costs[t, r]
                 * m.global_emission_reduction_per_cost_unit[t]
                 if t > 0
                 else Constraint.Skip,
                 "paid_for_emission_reductions",
             ),
             # Import export of emission reduction balance: if positive: , if negative:
             RegionalConstraint(
@@ -89,15 +89,15 @@
                 - m.regional_emission_reduction[t, r]
                 if t > 0
                 else Constraint.Skip,
                 "import_export_emission_reduction_balance",
             ),
             RegionalConstraint(
                 lambda m, t, r: m.import_export_mitigation_cost_balance[t, r]
-                == m.abatement_costs[t, r] - m.area_under_MAC[t, r],
+                == m.mitigation_costs[t, r] - m.area_under_MAC[t, r],
                 "import_export_mitigation_cost_balance",
             ),
         ]
     )
 
     # How are mitigation costs distributed over regions?
     m.min_rel_payment_level = Param()
```

### Comparing `mimosa-0.1.3/mimosa/components/emissiontrade/notrade.py` & `mimosa-0.1.4/mimosa/components/emissiontrade/notrade.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 Emission trading module
 Type: no trade
 """
 
 from typing import Sequence
 from mimosa.common import AbstractModel, GeneralConstraint, RegionalConstraint, Param
 
-from mimosa.components.abatement import AC
+from mimosa.components.mitigation import AC
 
 
 def get_constraints(m: AbstractModel) -> Sequence[GeneralConstraint]:
     """Emission trading equations and constraints
     (no-trade specification)
 
     Necessary variables:
-        m.abatement_costs (abatement costs as paid for by this region)
+        m.mitigation_costs (abatement costs as paid for by this region)
 
     Returns:
         list of constraints (any of:
            - GlobalConstraint
            - GlobalInitConstraint
            - RegionalConstraint
            - RegionalInitConstraint
@@ -28,15 +28,15 @@
     constraints = []
 
     m.import_export_emission_reduction_balance = Param(m.t, m.regions, initialize=0)
 
     constraints.extend(
         [
             RegionalConstraint(
-                lambda m, t, r: (m.abatement_costs[t, r])
+                lambda m, t, r: (m.mitigation_costs[t, r])
                 == AC(m.relative_abatement[t, r], m, t, r) * m.baseline[t, r],
-                "abatement_costs",
+                "mitigation_costs",
             ),
         ]
     )
 
     return constraints
```

### Comparing `mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 1968 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 b007 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 b007 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6404 6504 6405 6502 6505 1900 6604  ..d.e.d.e.e...f.
 00000070: 6406 6407 8404 5a0b 6408 5300 2909 7a6b  d.d...Z.d.S.).zk
@@ -60,19 +60,19 @@
 000003b0: 054e 7201 0000 0063 0100 0000 0000 0000  .Nr....c........
 000003c0: 0000 0000 0200 0000 0400 0000 3300 0000  ............3...
 000003d0: 731e 0000 0081 007c 005d 0a7d 0188 006a  s......|.].}...j
 000003e0: 0088 017c 0166 0219 0056 0001 0071 0264  ...|.f...V...q.d
 000003f0: 0053 00a9 014e a901 da12 6669 6e61 6e63  .S...N....financ
 00000400: 6961 6c5f 7472 616e 7366 6572 2902 da02  ial_transfer)...
 00000410: 2e30 da01 72a9 0272 0a00 0000 da01 74a9  .0..r..r......t.
-00000420: 00fa 7963 3a5c 7573 6572 735c 3339 3033  ..yc:\users\3903
-00000430: 3838 355c 6f6e 6564 7269 7665 202d 2075  885\onedrive - u
-00000440: 6e69 7665 7273 6974 6569 7420 7574 7265  niversiteit utre
-00000450: 6368 745c 646f 6375 6d65 6e74 735c 6d69  cht\documents\mi
-00000460: 6d6f 7361 5c6d 696d 6f73 615c 636f 6d70  mosa\mimosa\comp
+00000420: 00fa 7963 3a5c 5573 6572 735c 3339 3033  ..yc:\Users\3903
+00000430: 3838 355c 4f6e 6544 7269 7665 202d 2055  885\OneDrive - U
+00000440: 6e69 7665 7273 6974 6569 7420 5574 7265  niversiteit Utre
+00000450: 6368 745c 446f 6375 6d65 6e74 735c 4d49  cht\Documents\MI
+00000460: 4d4f 5341 5c6d 696d 6f73 615c 636f 6d70  MOSA\mimosa\comp
 00000470: 6f6e 656e 7473 5c66 696e 616e 6369 616c  onents\financial
 00000480: 7472 616e 7366 6572 5c67 6c6f 6261 6c64  transfer\globald
 00000490: 616d 6167 6570 6f6f 6c2e 7079 da09 3c67  amagepool.py..<g
 000004a0: 656e 6578 7072 3e2b 0000 0073 0400 0000  enexpr>+...s....
 000004b0: 0280 1c00 7a34 6765 745f 636f 6e73 7472  ....z4get_constr
 000004c0: 6169 6e74 732e 3c6c 6f63 616c 733e 2e3c  aints.<locals>.<
 000004d0: 6c61 6d62 6461 3e2e 3c6c 6f63 616c 733e  lambda>.<locals>
```

### Comparing `mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 939 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 ab03 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b669 ba64 ab03 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6404 6504 6405 6502 6505  m.Z...d.e.d.e.e.
 00000060: 1900 6604 6406 6407 8404 5a08 6408 5300  ..f.d.d...Z.d.S.
 00000070: 2909 7a5f 0a4d 6f64 656c 2065 7175 6174  ).z_.Model equat
@@ -45,19 +45,19 @@
 000002c0: 2020 2020 2020 290a 2020 2020 7201 0000        ).    r...
 000002d0: 0029 01da 0a69 6e69 7469 616c 697a 6529  .)...initialize)
 000002e0: 0572 0600 0000 da01 74da 0772 6567 696f  .r......t..regio
 000002f0: 6e73 5a12 6669 6e61 6e63 6961 6c5f 7472  nsZ.financial_tr
 00000300: 616e 7366 6572 da16 7265 6c5f 6669 6e61  ansfer..rel_fina
 00000310: 6e63 6961 6c5f 7472 616e 7366 6572 2902  ncial_transfer).
 00000320: 7207 0000 00da 0b63 6f6e 7374 7261 696e  r......constrain
-00000330: 7473 a900 720e 0000 00fa 7363 3a5c 7573  ts..r.....sc:\us
-00000340: 6572 735c 3339 3033 3838 355c 6f6e 6564  ers\3903885\oned
-00000350: 7269 7665 202d 2075 6e69 7665 7273 6974  rive - universit
-00000360: 6569 7420 7574 7265 6368 745c 646f 6375  eit utrecht\docu
-00000370: 6d65 6e74 735c 6d69 6d6f 7361 5c6d 696d  ments\mimosa\mim
+00000330: 7473 a900 720e 0000 00fa 7363 3a5c 5573  ts..r.....sc:\Us
+00000340: 6572 735c 3339 3033 3838 355c 4f6e 6544  ers\3903885\OneD
+00000350: 7269 7665 202d 2055 6e69 7665 7273 6974  rive - Universit
+00000360: 6569 7420 5574 7265 6368 745c 446f 6375  eit Utrecht\Docu
+00000370: 6d65 6e74 735c 4d49 4d4f 5341 5c6d 696d  ments\MIMOSA\mim
 00000380: 6f73 615c 636f 6d70 6f6e 656e 7473 5c66  osa\components\f
 00000390: 696e 616e 6369 616c 7472 616e 7366 6572  inancialtransfer
 000003a0: 5c6e 6f74 7261 6e73 6665 722e 7079 da0f  \notransfer.py..
 000003b0: 6765 745f 636f 6e73 7472 6169 6e74 730b  get_constraints.
 000003c0: 0000 0073 0800 0000 040f 1403 1401 0402  ...s............
 000003d0: 7210 0000 004e 2909 da07 5f5f 646f 635f  r....N)...__doc_
 000003e0: 5fda 0674 7970 696e 6772 0200 0000 da0d  _..typingr......
```

### Comparing `mimosa-0.1.3/mimosa/components/financialtransfer/globaldamagepool.py` & `mimosa-0.1.4/mimosa/components/financialtransfer/globaldamagepool.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/financialtransfer/notransfer.py` & `mimosa-0.1.4/mimosa/components/financialtransfer/notransfer.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 1558 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 1606 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 289f ba64 1706 0000  o.......(..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6404 6505 6405 6503 650a 6502 6507  ..d.e.d.e.e.e.e.
@@ -60,74 +60,74 @@
 000003b0: 8700 8701 6602 6405 6404 8408 8800 6a07  ....f.d.d.....j.
 000003c0: 4400 8301 8301 1700 1400 1700 6b02 5300  D...........k.S.
 000003d0: 7408 6a09 5300 2906 4e72 0100 0000 e901  t.j.S.).Nr......
 000003e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
 000003f0: 0200 0000 0400 0000 3300 0000 731e 0000  ........3...s...
 00000400: 0081 007c 005d 0a7d 0188 006a 0088 017c  ...|.].}...j...|
 00000410: 0166 0219 0056 0001 0071 0264 0053 00a9  .f...V...q.d.S..
-00000420: 014e 2901 da0f 6162 6174 656d 656e 745f  .N)...abatement_
-00000430: 636f 7374 73a9 02da 022e 30da 0172 a902  costs.....0..r..
-00000440: 720e 0000 00da 0174 a900 fa6c 633a 5c75  r......t...lc:\u
-00000450: 7365 7273 5c33 3930 3338 3835 5c6f 6e65  sers\3903885\one
-00000460: 6472 6976 6520 2d20 756e 6976 6572 7369  drive - universi
-00000470: 7465 6974 2075 7472 6563 6874 5c64 6f63  teit utrecht\doc
-00000480: 756d 656e 7473 5c6d 696d 6f73 615c 6d69  uments\mimosa\mi
-00000490: 6d6f 7361 5c63 6f6d 706f 6e65 6e74 735c  mosa\components\
-000004a0: 6f62 6a65 6374 6976 655c 676c 6f62 616c  objective\global
-000004b0: 636f 7374 732e 7079 da09 3c67 656e 6578  costs.py..<genex
-000004c0: 7072 3e32 0000 0073 0400 0000 0280 1c00  pr>2...s........
-000004d0: 7a34 6765 745f 636f 6e73 7472 6169 6e74  z4get_constraint
-000004e0: 732e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  s.<locals>.<lamb
-000004f0: 6461 3e2e 3c6c 6f63 616c 733e 2e3c 6765  da>.<locals>.<ge
-00000500: 6e65 7870 723e 6301 0000 0000 0000 0000  nexpr>c.........
-00000510: 0000 0002 0000 0005 0000 0033 0000 0073  ...........3...s
-00000520: 2c00 0000 8100 7c00 5d11 7d01 8800 6a00  ,.....|.].}...j.
-00000530: 8801 7c01 6602 1900 8800 6a01 8801 7c01  ..|.f.....j...|.
-00000540: 6602 1900 1400 5600 0100 7102 6400 5300  f.....V...q.d.S.
-00000550: 7211 0000 0029 02da 0c64 616d 6167 655f  r....)...damage_
-00000560: 636f 7374 73da 0947 4450 5f67 726f 7373  costs..GDP_gross
-00000570: 7213 0000 0072 1600 0000 7218 0000 0072  r....r....r....r
-00000580: 1900 0000 721a 0000 0033 0000 0073 0400  ....r....3...s..
-00000590: 0000 0280 2a00 290a da03 4e50 56da 0264  ....*.)...NPV..d
-000005a0: 7472 0c00 0000 da04 5052 5450 da04 7965  tr......PRTP..ye
-000005b0: 6172 da09 6265 6769 6e79 6561 72da 0373  ar..beginyear..s
-000005c0: 756d da07 7265 6769 6f6e 7372 0500 0000  um..regionsr....
-000005d0: da04 536b 6970 7216 0000 0072 1800 0000  ..Skipr....r....
-000005e0: 7216 0000 0072 1900 0000 da08 3c6c 616d  r....r......<lam
-000005f0: 6264 613e 2d00 0000 731a 0000 0008 0808  bda>-...s.......
-00000600: f80c 0104 011a 0102 ff18 0318 0102 ff02  ................
-00000610: fd02 ff04 ff06 097a 2167 6574 5f63 6f6e  .......z!get_con
-00000620: 7374 7261 696e 7473 2e3c 6c6f 6361 6c73  straints.<locals
-00000630: 3e2e 3c6c 616d 6264 613e 721d 0000 0029  >.<lambda>r....)
-00000640: 01da 046e 616d 6563 0100 0000 0000 0000  ...namec........
-00000650: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
-00000660: 730e 0000 007c 006a 0064 0119 0064 016b  s....|.j.d...d.k
-00000670: 0253 0029 024e 7201 0000 0029 0172 1d00  .S.).Nr....).r..
-00000680: 0000 a901 720e 0000 0072 1800 0000 7218  ....r....r....r.
-00000690: 0000 0072 1900 0000 7225 0000 0039 0000  ...r....r%...9..
-000006a0: 0073 0200 0000 0e00 6301 0000 0000 0000  .s......c.......
-000006b0: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
-000006c0: 0073 0c00 0000 7c00 6a00 7c00 6a01 1900  .s....|.j.|.j...
-000006d0: 5300 7211 0000 0029 0272 1d00 0000 da02  S.r....).r......
-000006e0: 7466 7227 0000 0072 1800 0000 7218 0000  tfr'...r....r...
-000006f0: 0072 1900 0000 7225 0000 003d 0000 0073  .r....r%...=...s
-00000700: 0200 0000 0c00 2902 da04 7275 6c65 da05  ......)...rule..
-00000710: 7365 6e73 6529 0a72 0b00 0000 7217 0000  sense).r....r...
-00000720: 0072 1d00 0000 720a 0000 0072 1f00 0000  .r....r....r....
-00000730: da06 6578 7465 6e64 7207 0000 0072 0800  ..extendr....r..
-00000740: 0000 7209 0000 0072 0d00 0000 2903 720e  ..r....r....).r.
-00000750: 0000 00da 0b63 6f6e 7374 7261 696e 7473  .....constraints
-00000760: da09 6f62 6a65 6374 6976 6572 1800 0000  ..objectiver....
-00000770: 7218 0000 0072 1900 0000 da0f 6765 745f  r....r......get_
-00000780: 636f 6e73 7472 6169 6e74 7316 0000 0073  constraints....s
-00000790: 1a00 0000 0410 0c02 0801 0401 0202 0601  ................
-000007a0: 020a 04f5 0a0d 02f2 04ff 1013 0802 722e  ..............r.
-000007b0: 0000 004e 2910 da07 5f5f 646f 635f 5fda  ...N)...__doc__.
-000007c0: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-000007d0: 00da 0d6d 696d 6f73 612e 636f 6d6d 6f6e  ...mimosa.common
-000007e0: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-000007f0: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
-00000800: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000810: 0000 722e 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00000820: 0072 1800 0000 7219 0000 00da 083c 6d6f  .r....r......<mo
-00000830: 6475 6c65 3e01 0000 0073 0800 0000 0400  dule>....s......
-00000840: 1005 3002 220e                           ..0.".
+00000420: 014e 2901 da10 6d69 7469 6761 7469 6f6e  .N)...mitigation
+00000430: 5f63 6f73 7473 a902 da02 2e30 da01 72a9  _costs.....0..r.
+00000440: 0272 0e00 0000 da01 74a9 00fa 6c63 3a5c  .r......t...lc:\
+00000450: 5573 6572 735c 3339 3033 3838 355c 4f6e  Users\3903885\On
+00000460: 6544 7269 7665 202d 2055 6e69 7665 7273  eDrive - Univers
+00000470: 6974 6569 7420 5574 7265 6368 745c 446f  iteit Utrecht\Do
+00000480: 6375 6d65 6e74 735c 4d49 4d4f 5341 5c6d  cuments\MIMOSA\m
+00000490: 696d 6f73 615c 636f 6d70 6f6e 656e 7473  imosa\components
+000004a0: 5c6f 626a 6563 7469 7665 5c67 6c6f 6261  \objective\globa
+000004b0: 6c63 6f73 7473 2e70 79da 093c 6765 6e65  lcosts.py..<gene
+000004c0: 7870 723e 3200 0000 7304 0000 0002 801c  xpr>2...s.......
+000004d0: 007a 3467 6574 5f63 6f6e 7374 7261 696e  .z4get_constrain
+000004e0: 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ts.<locals>.<lam
+000004f0: 6264 613e 2e3c 6c6f 6361 6c73 3e2e 3c67  bda>.<locals>.<g
+00000500: 656e 6578 7072 3e63 0100 0000 0000 0000  enexpr>c........
+00000510: 0000 0000 0200 0000 0500 0000 3300 0000  ............3...
+00000520: 732c 0000 0081 007c 005d 117d 0188 006a  s,.....|.].}...j
+00000530: 0088 017c 0166 0219 0088 006a 0188 017c  ...|.f.....j...|
+00000540: 0166 0219 0014 0056 0001 0071 0264 0053  .f.....V...q.d.S
+00000550: 0072 1100 0000 2902 da0c 6461 6d61 6765  .r....)...damage
+00000560: 5f63 6f73 7473 da09 4744 505f 6772 6f73  _costs..GDP_gros
+00000570: 7372 1300 0000 7216 0000 0072 1800 0000  sr....r....r....
+00000580: 7219 0000 0072 1a00 0000 3300 0000 7304  r....r....3...s.
+00000590: 0000 0002 802a 0029 0ada 034e 5056 da02  .....*.)...NPV..
+000005a0: 6474 720c 0000 00da 0450 5254 50da 0479  dtr......PRTP..y
+000005b0: 6561 72da 0962 6567 696e 7965 6172 da03  ear..beginyear..
+000005c0: 7375 6dda 0772 6567 696f 6e73 7205 0000  sum..regionsr...
+000005d0: 00da 0453 6b69 7072 1600 0000 7218 0000  ...Skipr....r...
+000005e0: 0072 1600 0000 7219 0000 00da 083c 6c61  .r....r......<la
+000005f0: 6d62 6461 3e2d 0000 0073 1a00 0000 0808  mbda>-...s......
+00000600: 08f8 0c01 0401 1a01 02ff 1803 1801 02ff  ................
+00000610: 02fd 02ff 04ff 0609 7a21 6765 745f 636f  ........z!get_co
+00000620: 6e73 7472 6169 6e74 732e 3c6c 6f63 616c  nstraints.<local
+00000630: 733e 2e3c 6c61 6d62 6461 3e72 1d00 0000  s>.<lambda>r....
+00000640: 2901 da04 6e61 6d65 6301 0000 0000 0000  )...namec.......
+00000650: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
+00000660: 0073 0e00 0000 7c00 6a00 6401 1900 6401  .s....|.j.d...d.
+00000670: 6b02 5300 2902 4e72 0100 0000 2901 721d  k.S.).Nr....).r.
+00000680: 0000 00a9 0172 0e00 0000 7218 0000 0072  .....r....r....r
+00000690: 1800 0000 7219 0000 0072 2500 0000 3900  ....r....r%...9.
+000006a0: 0000 7302 0000 000e 0063 0100 0000 0000  ..s......c......
+000006b0: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
+000006c0: 0000 730c 0000 007c 006a 007c 006a 0119  ..s....|.j.|.j..
+000006d0: 0053 0072 1100 0000 2902 721d 0000 00da  .S.r....).r.....
+000006e0: 0274 6672 2700 0000 7218 0000 0072 1800  .tfr'...r....r..
+000006f0: 0000 7219 0000 0072 2500 0000 3d00 0000  ..r....r%...=...
+00000700: 7302 0000 000c 0029 02da 0472 756c 65da  s......)...rule.
+00000710: 0573 656e 7365 290a 720b 0000 0072 1700  .sense).r....r..
+00000720: 0000 721d 0000 0072 0a00 0000 721f 0000  ..r....r....r...
+00000730: 00da 0665 7874 656e 6472 0700 0000 7208  ...extendr....r.
+00000740: 0000 0072 0900 0000 720d 0000 0029 0372  ...r....r....).r
+00000750: 0e00 0000 da0b 636f 6e73 7472 6169 6e74  ......constraint
+00000760: 73da 096f 626a 6563 7469 7665 7218 0000  s..objectiver...
+00000770: 0072 1800 0000 7219 0000 00da 0f67 6574  .r....r......get
+00000780: 5f63 6f6e 7374 7261 696e 7473 1600 0000  _constraints....
+00000790: 731a 0000 0004 100c 0208 0104 0102 0206  s...............
+000007a0: 0102 0a04 f50a 0d02 f204 ff10 1308 0272  ...............r
+000007b0: 2e00 0000 4e29 10da 075f 5f64 6f63 5f5f  ....N)...__doc__
+000007c0: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
+000007d0: 0000 da0d 6d69 6d6f 7361 2e63 6f6d 6d6f  ....mimosa.commo
+000007e0: 6e72 0400 0000 7205 0000 0072 0600 0000  nr....r....r....
+000007f0: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+00000800: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
+00000810: 0000 0072 2e00 0000 7218 0000 0072 1800  ...r....r....r..
+00000820: 0000 7218 0000 0072 1900 0000 da08 3c6d  ..r....r......<m
+00000830: 6f64 756c 653e 0100 0000 7308 0000 0004  odule>....s.....
+00000840: 0010 0530 0222 0e                        ...0.".
```

### Comparing `mimosa-0.1.3/mimosa/components/objective/__pycache__/utility.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/objective/__pycache__/utility.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 1713 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 b106 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b769 ba64 b106 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6404 6505 6405 6503 650c 6502 6508  ..d.e.d.e.e.e.e.
@@ -59,19 +59,19 @@
 000003a0: 1900 1400 1700 6b02 5300 7407 6a08 5300  ......k.S.t.j.S.
 000003b0: 2903 4e72 0100 0000 e901 0000 0029 09da  ).Nr.........)..
 000003c0: 034e 5056 da02 6474 720c 0000 00da 0450  .NPV..dtr......P
 000003d0: 5254 50da 0479 6561 72da 0962 6567 696e  RTP..year..begin
 000003e0: 7965 6172 5a0e 7965 6172 6c79 5f77 656c  yearZ.yearly_wel
 000003f0: 6661 7265 720a 0000 00da 0453 6b69 7029  farer......Skip)
 00000400: 0272 0e00 0000 da01 74a9 0072 1800 0000  .r......t..r....
-00000410: fa68 633a 5c75 7365 7273 5c33 3930 3338  .hc:\users\39038
-00000420: 3835 5c6f 6e65 6472 6976 6520 2d20 756e  85\onedrive - un
-00000430: 6976 6572 7369 7465 6974 2075 7472 6563  iversiteit utrec
-00000440: 6874 5c64 6f63 756d 656e 7473 5c6d 696d  ht\documents\mim
-00000450: 6f73 615c 6d69 6d6f 7361 5c63 6f6d 706f  osa\mimosa\compo
+00000410: fa68 633a 5c55 7365 7273 5c33 3930 3338  .hc:\Users\39038
+00000420: 3835 5c4f 6e65 4472 6976 6520 2d20 556e  85\OneDrive - Un
+00000430: 6976 6572 7369 7465 6974 2055 7472 6563  iversiteit Utrec
+00000440: 6874 5c44 6f63 756d 656e 7473 5c4d 494d  ht\Documents\MIM
+00000450: 4f53 415c 6d69 6d6f 7361 5c63 6f6d 706f  OSA\mimosa\compo
 00000460: 6e65 6e74 735c 6f62 6a65 6374 6976 655c  nents\objective\
 00000470: 7574 696c 6974 792e 7079 da08 3c6c 616d  utility.py..<lam
 00000480: 6264 613e 2c00 0000 730e 0000 0008 0308  bda>,...s.......
 00000490: fd0c 012a 0102 ff04 ff06 047a 2167 6574  ...*.......z!get
 000004a0: 5f63 6f6e 7374 7261 696e 7473 2e3c 6c6f  _constraints.<lo
 000004b0: 6361 6c73 3e2e 3c6c 616d 6264 613e 7211  cals>.<lambda>r.
 000004c0: 0000 0029 01da 046e 616d 6563 0100 0000  ...)...namec....
```

### Comparing `mimosa-0.1.3/mimosa/components/objective/globalcosts.py` & `mimosa-0.1.4/mimosa/components/objective/globalcosts.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         [
             GlobalConstraint(
                 lambda m, t: m.NPV[t]
                 == m.NPV[t - 1]
                 + m.dt
                 * exp(-m.PRTP * (m.year(t) - m.beginyear))
                 * (
-                    sum(m.abatement_costs[t, r] for r in m.regions)
+                    sum(m.mitigation_costs[t, r] for r in m.regions)
                     + sum(m.damage_costs[t, r] * m.GDP_gross[t, r] for r in m.regions)
                 )
                 if t > 0
                 else Constraint.Skip,
                 name="NPV",
             ),
             GlobalInitConstraint(lambda m: m.NPV[0] == 0),
```

### Comparing `mimosa-0.1.3/mimosa/components/objective/utility.py` & `mimosa-0.1.4/mimosa/components/objective/utility.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/sealevelrise.py` & `mimosa-0.1.4/mimosa/components/sealevelrise.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 1456 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 b005 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b769 ba64 b005 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6404 6504 6405 6502 6507 1900 6604  ..d.e.d.e.e...f.
 00000070: 6406 6407 8404 5a0b 6408 6409 8400 5a0c  d.d...Z.d.d...Z.
@@ -51,19 +51,19 @@
 00000320: 7c01 7c02 6602 1900 7c00 a003 7c00 a004  |.|.f...|...|...
 00000330: 7c01 a101 7c02 a102 7c00 6a05 8303 6b02  |...|...|.j...k.
 00000340: 5300 a901 4e29 06da 0775 7469 6c69 7479  S...N)...utility
 00000350: da0c 6361 6c63 5f75 7469 6c69 7479 da0b  ..calc_utility..
 00000360: 636f 6e73 756d 7074 696f 6eda 014c da04  consumption..L..
 00000370: 7965 6172 da06 656c 6173 6d75 2903 720a  year..elasmu).r.
 00000380: 0000 00da 0174 da01 72a9 0072 1600 0000  .....t..r..r....
-00000390: fa76 633a 5c75 7365 7273 5c33 3930 3338  .vc:\users\39038
-000003a0: 3835 5c6f 6e65 6472 6976 6520 2d20 756e  85\onedrive - un
-000003b0: 6976 6572 7369 7465 6974 2075 7472 6563  iversiteit utrec
-000003c0: 6874 5c64 6f63 756d 656e 7473 5c6d 696d  ht\documents\mim
-000003d0: 6f73 615c 6d69 6d6f 7361 5c63 6f6d 706f  osa\mimosa\compo
+00000390: fa76 633a 5c55 7365 7273 5c33 3930 3338  .vc:\Users\39038
+000003a0: 3835 5c4f 6e65 4472 6976 6520 2d20 556e  85\OneDrive - Un
+000003b0: 6976 6572 7369 7465 6974 2055 7472 6563  iversiteit Utrec
+000003c0: 6874 5c44 6f63 756d 656e 7473 5c4d 494d  ht\Documents\MIM
+000003d0: 4f53 415c 6d69 6d6f 7361 5c63 6f6d 706f  OSA\mimosa\compo
 000003e0: 6e65 6e74 735c 7765 6c66 6172 655c 696e  nents\welfare\in
 000003f0: 6571 7561 6c5f 6176 6572 7369 6f6e 5f65  equal_aversion_e
 00000400: 6c61 736d 752e 7079 da08 3c6c 616d 6264  lasmu.py..<lambd
 00000410: 613e 2c00 0000 7306 0000 000c 0024 0104  a>,...s......$..
 00000420: ff7a 2167 6574 5f63 6f6e 7374 7261 696e  .z!get_constrain
 00000430: 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ts.<locals>.<lam
 00000440: 6264 613e 720e 0000 0063 0200 0000 0000  bda>r....c......
```

### Comparing `mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 2048 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 0008 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b769 ba64 0008 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6404 6504 6405 6502 6507 1900 6604  ..d.e.d.e.e...f.
 00000070: 6406 6407 8404 5a0b 6408 6409 8400 5a0c  d.d...Z.d.d...Z.
@@ -53,19 +53,19 @@
 00000340: 7c02 a102 7c00 6a05 8303 6b02 5300 a901  |...|.j...k.S...
 00000350: 4e29 06da 0775 7469 6c69 7479 da15 6361  N)...utility..ca
 00000360: 6c63 5f72 6567 696f 6e61 6c5f 7574 696c  lc_regional_util
 00000370: 6974 79da 0b63 6f6e 7375 6d70 7469 6f6e  ity..consumption
 00000380: da01 4cda 0479 6561 72da 1069 6e65 7175  ..L..year..inequ
 00000390: 616c 5f61 7665 7273 696f 6e29 0372 0a00  al_aversion).r..
 000003a0: 0000 da01 74da 0172 a900 7217 0000 00fa  ....t..r..r.....
-000003b0: 7763 3a5c 7573 6572 735c 3339 3033 3838  wc:\users\390388
-000003c0: 355c 6f6e 6564 7269 7665 202d 2075 6e69  5\onedrive - uni
-000003d0: 7665 7273 6974 6569 7420 7574 7265 6368  versiteit utrech
-000003e0: 745c 646f 6375 6d65 6e74 735c 6d69 6d6f  t\documents\mimo
-000003f0: 7361 5c6d 696d 6f73 615c 636f 6d70 6f6e  sa\mimosa\compon
+000003b0: 7763 3a5c 5573 6572 735c 3339 3033 3838  wc:\Users\390388
+000003c0: 355c 4f6e 6544 7269 7665 202d 2055 6e69  5\OneDrive - Uni
+000003d0: 7665 7273 6974 6569 7420 5574 7265 6368  versiteit Utrech
+000003e0: 745c 446f 6375 6d65 6e74 735c 4d49 4d4f  t\Documents\MIMO
+000003f0: 5341 5c6d 696d 6f73 615c 636f 6d70 6f6e  SA\mimosa\compon
 00000400: 656e 7473 5c77 656c 6661 7265 5c69 6e65  ents\welfare\ine
 00000410: 7175 616c 5f61 7665 7273 696f 6e5f 6765  qual_aversion_ge
 00000420: 6e65 7261 6c2e 7079 da08 3c6c 616d 6264  neral.py..<lambd
 00000430: 613e 2e00 0000 730a 0000 000c 0002 0120  a>....s........ 
 00000440: 0102 ff04 ff7a 2167 6574 5f63 6f6e 7374  .....z!get_const
 00000450: 7261 696e 7473 2e3c 6c6f 6361 6c73 3e2e  raints.<locals>.
 00000460: 3c6c 616d 6264 613e 720f 0000 0063 0200  <lambda>r....c..
```

### Comparing `mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc` & `mimosa-0.1.4/mimosa/components/welfare/__pycache__/cost_minimising.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:44 2023 UTC, .py size: 1663 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b836 ba64 7f06 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 7ce6 ba64 7f06 0000  o.......|..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6404 6504 6405 6502 6507 1900 6604  ..d.e.d.e.e...f.
 00000070: 6406 6407 8404 5a0b 6408 6409 8400 5a0c  d.d...Z.d.d...Z.
@@ -49,86 +49,85 @@
 00000300: 0003 0000 0007 0000 0053 0000 0073 2e00  .........S...s..
 00000310: 0000 7c00 6a00 7c01 7c02 6602 1900 7c00  ..|.j.|.|.f...|.
 00000320: 6a01 7c01 7c02 6602 1900 7c00 a002 7c00  j.|.|.f...|...|.
 00000330: a003 7c01 a101 7c02 a102 1b00 6b02 5300  ..|...|.....k.S.
 00000340: a901 4e29 04da 0775 7469 6c69 7479 da0b  ..N)...utility..
 00000350: 636f 6e73 756d 7074 696f 6eda 014c da04  consumption..L..
 00000360: 7965 6172 2903 720a 0000 00da 0174 da01  year).r......t..
-00000370: 72a9 0072 1500 0000 fa74 633a 5c75 7365  r..r.....tc:\use
-00000380: 7273 5c33 3930 3338 3835 5c6f 6e65 6472  rs\3903885\onedr
-00000390: 6976 6520 2d20 756e 6976 6572 7369 7465  ive - universite
-000003a0: 6974 2075 7472 6563 6874 5c64 6f63 756d  it utrecht\docum
-000003b0: 656e 7473 5c6d 696d 6f73 615c 6d69 6d6f  ents\mimosa\mimo
+00000370: 72a9 0072 1500 0000 fa6e 633a 5c55 7365  r..r.....nc:\Use
+00000380: 7273 5c33 3930 3338 3835 5c4f 6e65 4472  rs\3903885\OneDr
+00000390: 6976 6520 2d20 556e 6976 6572 7369 7465  ive - Universite
+000003a0: 6974 2055 7472 6563 6874 5c44 6f63 756d  it Utrecht\Docum
+000003b0: 656e 7473 5c4d 494d 4f53 415c 6d69 6d6f  ents\MIMOSA\mimo
 000003c0: 7361 5c63 6f6d 706f 6e65 6e74 735c 7765  sa\components\we
-000003d0: 6c66 6172 655c 696e 6571 7561 6c5f 6176  lfare\inequal_av
-000003e0: 6572 7369 6f6e 5f7a 6572 6f2e 7079 da08  ersion_zero.py..
-000003f0: 3c6c 616d 6264 613e 2e00 0000 7306 0000  <lambda>....s...
-00000400: 000c 001e 0104 ff7a 2167 6574 5f63 6f6e  .......z!get_con
-00000410: 7374 7261 696e 7473 2e3c 6c6f 6361 6c73  straints.<locals
-00000420: 3e2e 3c6c 616d 6264 613e 720f 0000 0063  >.<lambda>r....c
-00000430: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000440: 0800 0000 1300 0000 735e 0000 0088 006a  ........s^.....j
-00000450: 0088 0119 0074 0187 0087 0166 0264 0164  .....t.....f.d.d
-00000460: 0284 0888 006a 0244 0083 0183 0174 0374  .....j.D.....t.t
-00000470: 0187 0087 0166 0264 0364 0284 0888 006a  .....f.d.d.....j
-00000480: 0244 0083 0183 0174 0187 0087 0166 0264  .D.....t.....f.d
-00000490: 0464 0284 0888 006a 0244 0083 0183 0188  .d.....j.D......
-000004a0: 006a 0483 0314 006b 0253 0029 054e 6301  .j.....k.S.).Nc.
-000004b0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-000004c0: 0000 0033 0000 00f3 2200 0000 8100 7c00  ...3....".....|.
-000004d0: 5d0c 7d01 8800 a000 8800 a001 8801 a101  ].}.............
-000004e0: 7c01 a102 5600 0100 7102 6400 5300 720e  |...V...q.d.S.r.
-000004f0: 0000 00a9 0272 1100 0000 7212 0000 00a9  .....r....r.....
-00000500: 02da 022e 3072 1400 0000 a902 720a 0000  ....0r......r...
-00000510: 0072 1300 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000520: da09 3c67 656e 6578 7072 3e34 0000 00f3  ..<genexpr>4....
-00000530: 0400 0000 0280 2000 7a34 6765 745f 636f  ...... .z4get_co
-00000540: 6e73 7472 6169 6e74 732e 3c6c 6f63 616c  nstraints.<local
-00000550: 733e 2e3c 6c61 6d62 6461 3e2e 3c6c 6f63  s>.<lambda>.<loc
-00000560: 616c 733e 2e3c 6765 6e65 7870 723e 6301  als>.<genexpr>c.
-00000570: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000580: 0000 0033 0000 0073 1e00 0000 8100 7c00  ...3...s......|.
-00000590: 5d0a 7d01 8800 6a00 8801 7c01 6602 1900  ].}...j...|.f...
-000005a0: 5600 0100 7102 6400 5300 720e 0000 0029  V...q.d.S.r....)
-000005b0: 0172 1000 0000 721a 0000 0072 1c00 0000  .r....r....r....
-000005c0: 7215 0000 0072 1600 0000 721d 0000 0036  r....r....r....6
-000005d0: 0000 0073 0400 0000 0280 1c00 6301 0000  ...s........c...
-000005e0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-000005f0: 0033 0000 0072 1800 0000 720e 0000 0072  .3...r....r....r
-00000600: 1900 0000 721a 0000 0072 1c00 0000 7215  ....r....r....r.
-00000610: 0000 0072 1600 0000 721d 0000 0037 0000  ...r....r....7..
-00000620: 0072 1e00 0000 2905 da0e 7965 6172 6c79  .r....)...yearly
-00000630: 5f77 656c 6661 7265 da03 7375 6dda 0772  _welfare..sum..r
-00000640: 6567 696f 6e73 da0c 6361 6c63 5f75 7469  egions..calc_uti
-00000650: 6c69 7479 da06 656c 6173 6d75 721c 0000  lity..elasmur...
-00000660: 0072 1500 0000 721c 0000 0072 1600 0000  .r....r....r....
-00000670: 7217 0000 0033 0000 0073 1200 0000 0800  r....3...s......
-00000680: 1801 0201 1801 1801 0401 02fd 02ff 04ff  ................
-00000690: 721f 0000 0029 0b72 0400 0000 7223 0000  r....).r....r#..
-000006a0: 005a 1069 6e65 7175 616c 5f61 7665 7273  .Z.inequal_avers
-000006b0: 696f 6e72 0500 0000 7213 0000 0072 2100  ionr....r....r!.
-000006c0: 0000 720f 0000 0072 1f00 0000 da06 6578  ..r....r......ex
-000006d0: 7465 6e64 7207 0000 0072 0800 0000 2902  tendr....r....).
-000006e0: 720a 0000 00da 0b63 6f6e 7374 7261 696e  r......constrain
-000006f0: 7473 7215 0000 0072 1500 0000 7216 0000  tsr....r....r...
-00000700: 00da 0f67 6574 5f63 6f6e 7374 7261 696e  ...get_constrain
-00000710: 7473 1300 0000 7322 0000 0004 0f08 0308  ts....s"........
-00000720: 0114 020c 0104 0202 0206 0102 0202 fd02  ................
-00000730: 0506 0102 0702 f802 fa04 ff04 1472 2600  .............r&.
-00000740: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00000750: 0000 0003 0000 0043 0000 0073 2400 0000  .......C...s$...
-00000760: 7400 7c00 7c01 1b00 8301 6401 7c02 1800  t.|.|.....d.|...
-00000770: 1300 6401 1800 6401 7c02 1800 1b00 6401  ..d...d.|.....d.
-00000780: 1800 5300 2902 4ee9 0100 0000 2901 7209  ..S.).N.....).r.
-00000790: 0000 0029 0372 1000 0000 da0a 706f 7075  ...).r......popu
-000007a0: 6c61 7469 6f6e 7223 0000 0072 1500 0000  lationr#...r....
-000007b0: 7215 0000 0072 1600 0000 7222 0000 0042  r....r....r"...B
-000007c0: 0000 0073 0200 0000 2401 7222 0000 004e  ...s....$.r"...N
-000007d0: 290d da07 5f5f 646f 635f 5fda 0674 7970  )...__doc__..typ
-000007e0: 696e 6772 0200 0000 da0d 6d69 6d6f 7361  ingr......mimosa
-000007f0: 2e63 6f6d 6d6f 6e72 0300 0000 7204 0000  .commonr....r...
-00000800: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
-00000810: 7208 0000 0072 0900 0000 7226 0000 0072  r....r....r&...r
-00000820: 2200 0000 7215 0000 0072 1500 0000 7215  "...r....r....r.
-00000830: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000840: 653e 0100 0000 730a 0000 0004 000c 0524  e>....s........$
-00000850: 0216 0b0c 2f                             ..../
+000003d0: 6c66 6172 655c 636f 7374 5f6d 696e 696d  lfare\cost_minim
+000003e0: 6973 696e 672e 7079 da08 3c6c 616d 6264  ising.py..<lambd
+000003f0: 613e 2e00 0000 7306 0000 000c 001e 0104  a>....s.........
+00000400: ff7a 2167 6574 5f63 6f6e 7374 7261 696e  .z!get_constrain
+00000410: 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ts.<locals>.<lam
+00000420: 6264 613e 720f 0000 0063 0200 0000 0000  bda>r....c......
+00000430: 0000 0000 0000 0200 0000 0800 0000 1300  ................
+00000440: 0000 735e 0000 0088 006a 0088 0119 0074  ..s^.....j.....t
+00000450: 0187 0087 0166 0264 0164 0284 0888 006a  .....f.d.d.....j
+00000460: 0244 0083 0183 0174 0374 0187 0087 0166  .D.....t.t.....f
+00000470: 0264 0364 0284 0888 006a 0244 0083 0183  .d.d.....j.D....
+00000480: 0174 0187 0087 0166 0264 0464 0284 0888  .t.....f.d.d....
+00000490: 006a 0244 0083 0183 0188 006a 0483 0314  .j.D.......j....
+000004a0: 006b 0253 0029 054e 6301 0000 0000 0000  .k.S.).Nc.......
+000004b0: 0000 0000 0002 0000 0006 0000 0033 0000  .............3..
+000004c0: 00f3 2200 0000 8100 7c00 5d0c 7d01 8800  ..".....|.].}...
+000004d0: a000 8800 a001 8801 a101 7c01 a102 5600  ..........|...V.
+000004e0: 0100 7102 6400 5300 720e 0000 00a9 0272  ..q.d.S.r......r
+000004f0: 1100 0000 7212 0000 00a9 02da 022e 3072  ....r.........0r
+00000500: 1400 0000 a902 720a 0000 0072 1300 0000  ......r....r....
+00000510: 7215 0000 0072 1600 0000 da09 3c67 656e  r....r......<gen
+00000520: 6578 7072 3e34 0000 00f3 0400 0000 0280  expr>4..........
+00000530: 2000 7a34 6765 745f 636f 6e73 7472 6169   .z4get_constrai
+00000540: 6e74 732e 3c6c 6f63 616c 733e 2e3c 6c61  nts.<locals>.<la
+00000550: 6d62 6461 3e2e 3c6c 6f63 616c 733e 2e3c  mbda>.<locals>.<
+00000560: 6765 6e65 7870 723e 6301 0000 0000 0000  genexpr>c.......
+00000570: 0000 0000 0002 0000 0004 0000 0033 0000  .............3..
+00000580: 0073 1e00 0000 8100 7c00 5d0a 7d01 8800  .s......|.].}...
+00000590: 6a00 8801 7c01 6602 1900 5600 0100 7102  j...|.f...V...q.
+000005a0: 6400 5300 720e 0000 0029 0172 1000 0000  d.S.r....).r....
+000005b0: 721a 0000 0072 1c00 0000 7215 0000 0072  r....r....r....r
+000005c0: 1600 0000 721d 0000 0036 0000 0073 0400  ....r....6...s..
+000005d0: 0000 0280 1c00 6301 0000 0000 0000 0000  ......c.........
+000005e0: 0000 0002 0000 0006 0000 0033 0000 0072  ...........3...r
+000005f0: 1800 0000 720e 0000 0072 1900 0000 721a  ....r....r....r.
+00000600: 0000 0072 1c00 0000 7215 0000 0072 1600  ...r....r....r..
+00000610: 0000 721d 0000 0037 0000 0072 1e00 0000  ..r....7...r....
+00000620: 2905 da0e 7965 6172 6c79 5f77 656c 6661  )...yearly_welfa
+00000630: 7265 da03 7375 6dda 0772 6567 696f 6e73  re..sum..regions
+00000640: da0c 6361 6c63 5f75 7469 6c69 7479 da06  ..calc_utility..
+00000650: 656c 6173 6d75 721c 0000 0072 1500 0000  elasmur....r....
+00000660: 721c 0000 0072 1600 0000 7217 0000 0033  r....r....r....3
+00000670: 0000 0073 1200 0000 0800 1801 0201 1801  ...s............
+00000680: 1801 0401 02fd 02ff 04ff 721f 0000 0029  ..........r....)
+00000690: 0b72 0400 0000 7223 0000 005a 1069 6e65  .r....r#...Z.ine
+000006a0: 7175 616c 5f61 7665 7273 696f 6e72 0500  qual_aversionr..
+000006b0: 0000 7213 0000 0072 2100 0000 720f 0000  ..r....r!...r...
+000006c0: 0072 1f00 0000 da06 6578 7465 6e64 7207  .r......extendr.
+000006d0: 0000 0072 0800 0000 2902 720a 0000 00da  ...r....).r.....
+000006e0: 0b63 6f6e 7374 7261 696e 7473 7215 0000  .constraintsr...
+000006f0: 0072 1500 0000 7216 0000 00da 0f67 6574  .r....r......get
+00000700: 5f63 6f6e 7374 7261 696e 7473 1300 0000  _constraints....
+00000710: 7322 0000 0004 0f08 0308 0114 020c 0104  s"..............
+00000720: 0202 0206 0102 0202 fd02 0506 0102 0702  ................
+00000730: f802 fa04 ff04 1472 2600 0000 6303 0000  .......r&...c...
+00000740: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00000750: 0043 0000 0073 2400 0000 7400 7c00 7c01  .C...s$...t.|.|.
+00000760: 1b00 8301 6401 7c02 1800 1300 6401 1800  ....d.|.....d...
+00000770: 6401 7c02 1800 1b00 6401 1800 5300 2902  d.|.....d...S.).
+00000780: 4ee9 0100 0000 2901 7209 0000 0029 0372  N.....).r....).r
+00000790: 1000 0000 da0a 706f 7075 6c61 7469 6f6e  ......population
+000007a0: 7223 0000 0072 1500 0000 7215 0000 0072  r#...r....r....r
+000007b0: 1600 0000 7222 0000 0042 0000 0073 0200  ....r"...B...s..
+000007c0: 0000 2401 7222 0000 004e 290d da07 5f5f  ..$.r"...N)...__
+000007d0: 646f 635f 5fda 0674 7970 696e 6772 0200  doc__..typingr..
+000007e0: 0000 da0d 6d69 6d6f 7361 2e63 6f6d 6d6f  ....mimosa.commo
+000007f0: 6e72 0300 0000 7204 0000 0072 0500 0000  nr....r....r....
+00000800: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
+00000810: 0900 0000 7226 0000 0072 2200 0000 7215  ....r&...r"...r.
+00000820: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00000830: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000840: 730a 0000 0004 000c 0524 0216 0b0c 2f    s........$..../
```

### Comparing `mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_elasmu.py` & `mimosa-0.1.4/mimosa/components/welfare/welfare_loss_minimising.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_general.py` & `mimosa-0.1.4/mimosa/components/welfare/inequal_aversion_general.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_zero.py` & `mimosa-0.1.4/mimosa/components/welfare/cost_minimising.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc` & `mimosa-0.1.4/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:42 2023 UTC, .py size: 15078 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-00000000: 6f0d 0d0a 0000 0000 b636 ba64 e63a 0000  o........6.d.:..
+00000000: 6f0d 0d0a 0000 0000 92a0 ba64 e83a 0000  o..........d.:..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6400 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c07 6d08 5a08 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 8400 5a09 4700 6407 6408 8400 6408  d...Z.G.d.d...d.
 00000070: 8302 5a0a 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
 00000080: 2902 da0d 4162 7374 7261 6374 4d6f 6465  )...AbstractMode
 00000090: 6cda 0571 7561 6e74 2901 da09 4461 7461  l..quant)...Data
 000000a0: 5374 6f72 6529 01da 1252 6567 696f 6e61  Store)...Regiona
 000000b0: 6c50 6172 616d 5374 6f72 6563 0100 0000  lParamStorec....
 000000c0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
 000000d0: 4300 0000 7308 0000 0064 007c 0069 0153  C...s....d.|.i.S
 000000e0: 00a9 014e a900 2901 da03 7661 6c72 0700  ...N..)...valr..
-000000f0: 0000 7207 0000 00fa 6d63 3a5c 7573 6572  ..r.....mc:\user
-00000100: 735c 3339 3033 3838 355c 6f6e 6564 7269  s\3903885\onedri
-00000110: 7665 202d 2075 6e69 7665 7273 6974 6569  ve - universitei
-00000120: 7420 7574 7265 6368 745c 646f 6375 6d65  t utrecht\docume
-00000130: 6e74 735c 6d69 6d6f 7361 5c6d 696d 6f73  nts\mimosa\mimos
+000000f0: 0000 7207 0000 00fa 6d63 3a5c 5573 6572  ..r.....mc:\User
+00000100: 735c 3339 3033 3838 355c 4f6e 6544 7269  s\3903885\OneDri
+00000110: 7665 202d 2055 6e69 7665 7273 6974 6569  ve - Universitei
+00000120: 7420 5574 7265 6368 745c 446f 6375 6d65  t Utrecht\Docume
+00000130: 6e74 735c 4d49 4d4f 5341 5c6d 696d 6f73  nts\MIMOSA\mimos
 00000140: 615c 636f 6e63 7265 7465 5f6d 6f64 656c  a\concrete_model
 00000150: 5c69 6e73 7461 6e74 6961 7465 5f70 6172  \instantiate_par
 00000160: 616d 732e 7079 da08 3c6c 616d 6264 613e  ams.py..<lambda>
 00000170: 0800 0000 7302 0000 0008 0072 0a00 0000  ....s......r....
 00000180: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000190: 0009 0000 0040 0000 0073 7e00 0000 6500  .....@...s~...e.
 000001a0: 5a01 6400 5a02 0901 641c 6402 6503 6403  Z.d.Z...d.d.e.d.
@@ -208,15 +208,15 @@
 00000cf0: 6461 3e69 3408 0000 da09 6265 6769 6e79  da>i4.....beginy
 00000d00: 6561 72da 0274 6672 3800 0000 da08 7965  ear..tfr8.....ye
 00000d10: 6172 3231 3030 da07 7265 6769 6f6e 73da  ar2100..regions.
 00000d20: 1962 6173 656c 696e 655f 6361 7262 6f6e  .baseline_carbon
 00000d30: 5f69 6e74 656e 7369 7479 da09 656d 6973  _intensity..emis
 00000d40: 7369 6f6e 737a 1962 6173 656c 696e 6520  sionsz.baseline 
 00000d50: 6361 7262 6f6e 2069 6e74 656e 7369 7479  carbon intensity
-00000d60: da06 6275 6467 6574 5a0c 6361 7262 6f6e  ..budgetZ.carbon
+00000d60: da06 6275 6467 6574 da0c 6361 7262 6f6e  ..budget..carbon
 00000d70: 6275 6467 6574 da0e 656d 6973 7369 6f6e  budget..emission
 00000d80: 735f 756e 6974 da10 696e 6572 7469 615f  s_unit..inertia_
 00000d90: 7265 6769 6f6e 616c 5a07 696e 6572 7469  regionalZ.inerti
 00000da0: 615a 0872 6567 696f 6e61 6cda 0e69 6e65  aZ.regional..ine
 00000db0: 7274 6961 5f67 6c6f 6261 6cda 0667 6c6f  rtia_global..glo
 00000dc0: 6261 6cda 1067 6c6f 6261 6c5f 6d69 6e5f  bal..global_min_
 00000dd0: 6c65 7665 6c7a 1067 6c6f 6261 6c20 6d69  levelz.global mi
@@ -262,276 +262,276 @@
 00001050: 6761 6d6d 61da 0567 616d 6d61 7a20 6375  gamma..gammaz cu
 00001060: 7272 656e 6379 5f75 6e69 742f 656d 6973  rrency_unit/emis
 00001070: 7369 6f6e 7372 6174 655f 756e 6974 da08  sionsrate_unit..
 00001080: 4d41 435f 6265 7461 da04 6265 7461 da12  MAC_beta..beta..
 00001090: 4d41 435f 7363 616c 696e 675f 6661 6374  MAC_scaling_fact
 000010a0: 6f72 7a1b 7265 6769 6f6e 616c 2063 616c  orz.regional cal
 000010b0: 6962 7261 7469 6f6e 2066 6163 746f 72da  ibration factor.
-000010c0: 1d72 656c 5f61 6261 7465 6d65 6e74 5f63  .rel_abatement_c
-000010d0: 6f73 7473 5f6d 696e 5f6c 6576 656c da18  osts_min_level..
-000010e0: 696e 6974 5f63 6170 6974 616c 7374 6f63  init_capitalstoc
-000010f0: 6b5f 6661 6374 6f72 da13 696e 6974 5f63  k_factor..init_c
-00001100: 6170 6974 616c 5f66 6163 746f 72da 0561  apital_factor..a
-00001110: 6c70 6861 721a 0000 00da 0264 6b7a 1764  lphar......dkz.d
-00001120: 6570 7265 6369 6174 696f 6e20 6f66 2063  epreciation of c
-00001130: 6170 6974 616c 7a0c 7361 7669 6e67 7320  apitalz.savings 
-00001140: 7261 7465 da06 656c 6173 6d75 da10 696e  rate..elasmu..in
-00001150: 6571 7561 6c5f 6176 6572 7369 6f6e da04  equal_aversion..
-00001160: 5052 5450 2904 da02 7372 7268 0000 0072  PRTP)...srrh...r
-00001170: 6900 0000 726a 0000 005a 0e63 7573 746f  i...rj...Z.custo
-00001180: 6d5f 6d61 7070 696e 67da 0a73 696d 756c  m_mapping..simul
-00001190: 6174 696f 6e29 0e72 1000 0000 da03 696e  ation).r......in
-000011a0: 74da 026e 70da 0463 6569 6c72 0c00 0000  t..np..ceilr....
-000011b0: da04 7965 6172 da01 56da 0572 616e 6765  ..year..V..range
-000011c0: da04 6b65 7973 7203 0000 0072 0d00 0000  ..keysr....r....
-000011d0: da03 6765 74da 0675 7064 6174 65da 165f  ..get..update.._
-000011e0: 7365 745f 696e 7374 616e 6365 5f64 6174  set_instance_dat
-000011f0: 615f 736c 7229 0772 1600 0000 7213 0000  a_slr).r....r...
-00001200: 0072 1000 0000 5a05 745f 656e 645a 096e  .r....Z.t_endZ.n
-00001210: 756d 5f79 6561 7273 723c 0000 00da 1170  um_yearsr<.....p
-00001220: 6172 616d 6574 6572 5f6d 6170 7069 6e67  arameter_mapping
-00001230: 7207 0000 0072 3900 0000 7209 0000 0072  r....r9...r....r
-00001240: 2a00 0000 6600 0000 73ea 0000 0006 010c  *...f...s.......
-00001250: 010c 010c 011a 0112 0110 0102 0208 0102  ................
-00001260: ff08 0202 fe0c 0302 fd0c 0402 fc08 0502  ................
-00001270: fb10 0602 fa04 070a 0102 ff02 f916 0a02  ................
-00001280: f614 0b02 f514 0c02 f404 0d10 0102 ff02  ................
-00001290: f304 1010 0102 ff02 f004 130a 0102 ff02  ................
-000012a0: ed04 160a 0102 ff02 ea04 190a 0102 ff02  ................
-000012b0: e710 1c02 e410 1d04 e316 1e02 e204 1f10  ................
-000012c0: 0102 ff02 e104 2202 010a 0102 0102 fe02  ......".........
-000012d0: ff02 de14 2802 d80e 2902 d708 2a02 d614  ....(...)...*...
-000012e0: 2b02 d514 2c02 d404 2d0e 0102 ff02 d314  +...,...-.......
-000012f0: 3002 d004 3102 010e 0102 0102 fe02 ff02  0...1...........
-00001300: cf14 3702 c908 3810 0102 ff02 c804 3b0e  ..7...8.......;.
-00001310: 0102 ff02 c508 3e04 0102 ff02 c214 4102  ......>.......A.
-00001320: bf14 4204 be12 430e 010e 010e 0108 ba0e  ..B...C.........
-00001330: 4912 010e 020e 037a 2949 6e73 7461 6e74  I......z)Instant
-00001340: 6961 7465 644d 6f64 656c 2e5f 7365 745f  iatedModel._set_
-00001350: 696e 7374 616e 6365 5f64 6174 615f 6d61  instance_data_ma
-00001360: 696e 6302 0000 0000 0000 0000 0000 0003  inc.............
-00001370: 0000 000a 0000 0043 0000 0073 4e00 0000  .......C...sN...
-00001380: 7400 6401 8301 7400 6402 8301 7400 6403  t.d...t.d...t.d.
-00001390: 8301 7400 6404 8301 7400 6405 8301 7400  ..t.d...t.d...t.
-000013a0: 6406 8301 7400 6407 8301 7400 6408 8301  d...t.d...t.d...
-000013b0: 7400 6409 8301 640a 9c09 7d02 7c01 6400  t.d...d...}.|.d.
-000013c0: 1900 a001 7c02 a101 0100 6400 5300 290b  ....|.....d.S.).
-000013d0: 4ee7 0000 0000 0000 e03f 67cc ad56 ceae  N........?g..V..
-000013e0: 91b7 3f67 c4c7 6c7b 6aa7 983f 672d 431c  ..?g..l{j..?g-C.
-000013f0: ebe2 364a 3f67 a470 3d0a d7a3 d03f e9ff  ..6J?g.p=....?..
-00001400: ffff ff67 4bdc 32f9 c9e5 f13f 6733 3333  ...gK.2....?g333
-00001410: 3333 33e3 3f67 3333 3333 3333 1d40 2909  333.?g333333.@).
-00001420: da11 736c 725f 7468 6572 6d61 6c5f 6571  ..slr_thermal_eq
-00001430: 7569 6cda 1073 6c72 5f74 6865 726d 616c  uil..slr_thermal
-00001440: 5f69 6e69 74da 1773 6c72 5f74 6865 726d  _init..slr_therm
-00001450: 616c 5f61 646a 7573 745f 7261 7465 da12  al_adjust_rate..
-00001460: 736c 725f 6773 6963 5f6d 656c 745f 7261  slr_gsic_melt_ra
-00001470: 7465 da12 736c 725f 6773 6963 5f74 6f74  te..slr_gsic_tot
-00001480: 616c 5f69 6365 da13 736c 725f 6773 6963  al_ice..slr_gsic
-00001490: 5f65 7175 696c 5f74 656d 70da 1e73 6c72  _equil_temp..slr
-000014a0: 5f67 6973 5f6d 656c 745f 7261 7465 5f61  _gis_melt_rate_a
-000014b0: 626f 7665 5f74 6872 6573 68da 1673 6c72  bove_thresh..slr
-000014c0: 5f67 6973 5f69 6e69 745f 6d65 6c74 5f72  _gis_init_melt_r
-000014d0: 6174 65da 1473 6c72 5f67 6973 5f69 6e69  ate..slr_gis_ini
-000014e0: 745f 6963 655f 766f 6c29 0272 7100 0000  t_ice_vol).rq...
-000014f0: 7275 0000 00a9 0372 1600 0000 7213 0000  ru.....r....r...
-00001500: 0072 7700 0000 7207 0000 0072 0700 0000  .rw...r....r....
-00001510: 7209 0000 0072 7600 0000 c000 0000 7316  r....rv.......s.
-00001520: 0000 0006 0306 0106 0106 0106 0106 0106  ................
-00001530: 0106 0106 0106 f612 0d7a 2849 6e73 7461  .........z(Insta
-00001540: 6e74 6961 7465 644d 6f64 656c 2e5f 7365  ntiatedModel._se
-00001550: 745f 696e 7374 616e 6365 5f64 6174 615f  t_instance_data_
-00001560: 736c 7263 0200 0000 0000 0000 0000 0000  slrc............
-00001570: 0400 0000 0400 0000 4300 0000 7342 0000  ........C...sB..
-00001580: 007c 006a 007d 0274 017c 0264 0119 0064  .|.j.}.t.|.d...d
-00001590: 0219 0064 0319 0083 0174 017c 0264 0119  ...d.....t.|.d..
-000015a0: 0064 0219 0064 0419 0083 0164 059c 027d  .d...d.....d...}
-000015b0: 037c 0164 0019 00a0 027c 03a1 0101 0064  .|.d.....|.....d
-000015c0: 0053 0029 064e 7226 0000 007a 0e65 6d69  .S.).Nr&...z.emi
-000015d0: 7373 696f 6e20 7472 6164 657a 156d 696e  ssion tradez.min
-000015e0: 2072 656c 2070 6179 6d65 6e74 206c 6576   rel payment lev
-000015f0: 656c 7a15 6d61 7820 7265 6c20 7061 796d  elz.max rel paym
-00001600: 656e 7420 6c65 7665 6c29 02da 156d 696e  ent level)...min
-00001610: 5f72 656c 5f70 6179 6d65 6e74 5f6c 6576  _rel_payment_lev
-00001620: 656c da15 6d61 785f 7265 6c5f 7061 796d  el..max_rel_paym
-00001630: 656e 745f 6c65 7665 6c29 0372 1000 0000  ent_level).r....
-00001640: 7271 0000 0072 7500 0000 a904 7216 0000  rq...ru.....r...
-00001650: 0072 1300 0000 7210 0000 0072 7700 0000  .r....r....rw...
-00001660: 7207 0000 0072 0700 0000 7209 0000 0072  r....r....r....r
-00001670: 2b00 0000 d000 0000 7312 0000 0006 0102  +.......s.......
-00001680: 020e 0102 ff02 030e 0102 ff06 fc12 097a  ...............z
-00001690: 4149 6e73 7461 6e74 6961 7465 644d 6f64  AInstantiatedMod
-000016a0: 656c 2e5f 7365 745f 696e 7374 616e 6365  el._set_instance
-000016b0: 5f64 6174 615f 656d 6973 7369 6f6e 7472  _data_emissiontr
-000016c0: 6164 655f 676c 6f62 616c 636f 7374 706f  ade_globalcostpo
-000016d0: 6f6c 6302 0000 0000 0000 0000 0000 0004  olc.............
-000016e0: 0000 0009 0000 0043 0000 0073 6c00 0000  .......C...sl...
-000016f0: 7c00 6a00 7d02 7401 7c02 6401 1900 6402  |.j.}.t.|.d...d.
-00001700: 1900 6403 1900 8301 7c00 6a02 a003 6404  ..d.....|.j...d.
-00001710: 6405 a102 7c00 6a02 a003 6404 6406 a102  d...|.j...d.d...
-00001720: 7c00 6a02 a003 6404 6407 a102 7c00 6a02  |.j...d.d...|.j.
-00001730: a003 6404 6408 a102 7c00 6a02 a003 6404  ..d.d...|.j...d.
-00001740: 6409 a102 640a 9c06 7d03 7c01 6400 1900  d...d...}.|.d...
-00001750: a004 7c03 a101 0100 6400 5300 290b 4e72  ..|.....d.S.).Nr
-00001760: 2600 0000 725a 0000 005a 0a63 7572 725f  &...rZ...Z.curr_
-00001770: 6c65 7665 6cda 0a41 4452 4943 4532 3031  level..ADRICE201
-00001780: 30da 0261 31da 0261 32da 0261 33da 0267  0..a1..a2..a3..g
-00001790: 31da 0267 3229 06da 1061 6461 7074 5f63  1..g2)...adapt_c
-000017a0: 7572 725f 6c65 7665 6cda 0964 616d 6167  urr_level..damag
-000017b0: 655f 6131 da09 6461 6d61 6765 5f61 32da  e_a1..damage_a2.
-000017c0: 0964 616d 6167 655f 6133 da08 6164 6170  .damage_a3..adap
-000017d0: 745f 6731 da08 6164 6170 745f 6732 2905  t_g1..adapt_g2).
-000017e0: 7210 0000 0072 7100 0000 720d 0000 0072  r....rq...r....r
-000017f0: 7400 0000 7275 0000 0072 8600 0000 7207  t...ru...r....r.
-00001800: 0000 0072 0700 0000 7209 0000 0072 2c00  ...r....r....r,.
-00001810: 0000 dd00 0000 7312 0000 0006 0112 020c  ......s.........
-00001820: 010c 010c 010c 010c 0106 fa12 097a 2d49  .............z-I
-00001830: 6e73 7461 6e74 6961 7465 644d 6f64 656c  nstantiatedModel
-00001840: 2e5f 7365 745f 696e 7374 616e 6365 5f64  ._set_instance_d
-00001850: 6174 615f 7269 6365 3230 3130 6302 0000  ata_rice2010c...
-00001860: 0000 0000 0000 0000 0003 0000 000c 0000  ................
-00001870: 0043 0000 0073 7e00 0000 7c00 6a00 a001  .C...s~...|.j...
-00001880: 6401 6402 a102 7c00 6a00 a001 6401 6403  d.d...|.j...d.d.
-00001890: a102 7c00 6a00 a001 6401 6404 a102 7c00  ..|.j...d.d...|.
-000018a0: 6a00 a001 6401 6405 a102 7c00 6a00 a001  j...d.d...|.j...
-000018b0: 6401 6406 a102 7c00 6a00 a001 6401 6407  d.d...|.j...d.d.
-000018c0: a102 7402 6408 8301 7c00 6a00 a001 6401  ..t.d...|.j...d.
-000018d0: 6409 a102 7c00 6a00 a001 6401 640a a102  d...|.j...d.d...
-000018e0: 640b 9c09 7d02 7c01 6400 1900 a003 7c02  d...}.|.d.....|.
-000018f0: a101 0100 6400 5300 290c 4eda 0a41 4452  ....d.S.).N..ADR
-00001900: 4943 4532 3031 3272 8800 0000 7289 0000  ICE2012r....r...
-00001910: 0072 8a00 0000 5a03 6e75 315a 036e 7532  .r....Z.nu1Z.nu2
-00001920: 5a03 6e75 3372 7800 0000 5a07 736c 7264  Z.nu3rx...Z.slrd
-00001930: 616d 315a 0773 6c72 6461 6d32 2909 728e  am1Z.slrdam2).r.
-00001940: 0000 0072 8f00 0000 7290 0000 00da 0561  ...r....r......a
-00001950: 6461 7031 da05 6164 6170 32da 0561 6461  dap1..adap2..ada
-00001960: 7033 da09 6164 6170 745f 7268 6fda 0753  p3..adapt_rho..S
-00001970: 4c52 6461 6d31 da07 534c 5264 616d 3229  LRdam1..SLRdam2)
-00001980: 0472 0d00 0000 7274 0000 0072 7100 0000  .r....rt...rq...
-00001990: 7275 0000 0072 8300 0000 7207 0000 0072  ru...r....r....r
-000019a0: 0700 0000 7209 0000 0072 2d00 0000 ea00  ....r....r-.....
-000019b0: 0000 7316 0000 000c 020c 010c 010c 010c  ..s.............
-000019c0: 010c 0106 010c 010c 0106 f712 0c7a 2d49  .............z-I
-000019d0: 6e73 7461 6e74 6961 7465 644d 6f64 656c  nstantiatedModel
-000019e0: 2e5f 7365 745f 696e 7374 616e 6365 5f64  ._set_instance_d
-000019f0: 6174 615f 7269 6365 3230 3132 6302 0000  ata_rice2012c...
-00001a00: 0000 0000 0000 0000 000b 0000 000d 0000  ................
-00001a10: 0003 0000 0073 a401 0000 7a0b 8800 6a00  .....s....z...j.
-00001a20: 6401 1900 6402 1900 6403 1900 7d02 5700  d...d...d...}.W.
-00001a30: 6e0b 0400 7401 7916 0100 0100 0100 6404  n...t.y.......d.
-00001a40: 7d02 5900 6e01 7700 8800 6a00 6401 1900  }.Y.n.w...j.d...
-00001a50: 6402 1900 6405 1900 7d03 8800 6a00 6401  d...d...}...j.d.
-00001a60: 1900 6402 1900 6406 1900 7d04 7c04 722d  ..d...d...}.|.r-
-00001a70: 6407 6e01 6408 7d05 6409 7c05 9b00 9d02  d.n.d.}.d.|.....
-00001a80: 7d06 8700 6601 640a 640b 8408 7d07 7c03  }...f.d.d...}.|.
-00001a90: 7270 7c07 640c 8301 8800 6a02 a003 640d  rp|.d.....j...d.
-00001aa0: 640e 7c05 9b00 640f 7c02 9b00 9d04 a102  d.|...d.|.......
-00001ab0: 8800 6a02 a003 640d 6410 7c05 9b00 640f  ..j...d.d.|...d.
-00001ac0: 7c02 9b00 9d04 a102 7c07 6411 8301 7c07  |.......|.d...|.
-00001ad0: 6412 8301 7c07 6413 8301 7c07 6411 8301  d...|.d...|.d...
-00001ae0: 7c07 6411 8301 7c07 6411 8301 7c07 6411  |.d...|.d...|.d.
-00001af0: 8301 6414 9c0a 7d08 6e59 6415 7c02 9b00  ..d...}.nYd.|...
-00001b00: 6416 9d03 7d09 7c06 9b00 6417 7c02 9b00  d...}.|...d.|...
-00001b10: 6416 9d04 7d0a 8800 6a02 a003 640d 6418  d...}...j...d.d.
-00001b20: a102 8800 6a02 a003 640d 6419 a102 8800  ....j...d.d.....
-00001b30: 6a02 a003 640d 641a a102 8800 6a02 a003  j...d.d.....j...
-00001b40: 640d 641b a102 8800 6a02 a003 640d 7c09  d.d.....j...d.|.
-00001b50: a102 8800 6a02 a003 640d 7c06 9b00 641c  ....j...d.|...d.
-00001b60: 9d02 a102 8800 6a02 a003 640d 7c06 9b00  ......j...d.|...
-00001b70: 641d 9d02 a102 8800 6a02 a003 640d 7c06  d.......j...d.|.
-00001b80: 9b00 641e 9d02 a102 8800 6a02 a003 640d  ..d.......j...d.
-00001b90: 7c06 9b00 641f 9d02 a102 8800 6a02 a003  |...d.......j...
-00001ba0: 640d 7c0a a102 6414 9c0a 7d08 7c01 6400  d.|...d...}.|.d.
-00001bb0: 1900 a004 7c08 a101 0100 6400 5300 2920  ....|.....d.S.) 
-00001bc0: 4e72 2600 0000 7227 0000 00da 0871 7561  Nr&...r'.....qua
-00001bd0: 6e74 696c 6572 7800 0000 5a22 636f 6163  ntilerx...Z"coac
-00001be0: 6368 5f63 6f6d 6269 6e65 645f 736c 725f  ch_combined_slr_
-00001bf0: 6e6f 6e73 6c72 5f64 616d 6167 6573 5a14  nonslr_damagesZ.
-00001c00: 636f 6163 6368 5f73 6c72 5f77 6974 6861  coacch_slr_witha
-00001c10: 6461 7074 5a02 4164 5a04 4e6f 4164 7a04  daptZ.AdZ.NoAdz.
-00001c20: 534c 522d 6301 0000 0000 0000 0000 0000  SLR-c...........
-00001c30: 0001 0000 0003 0000 0013 0000 0073 1800  .............s..
-00001c40: 0000 8700 6601 6401 6402 8408 8801 6a00  ....f.d.d.....j.
-00001c50: 6403 1900 4400 8301 5300 2904 4e63 0100  d...D...S.).Nc..
-00001c60: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001c70: 0000 1300 0000 7312 0000 0069 007c 005d  ......s....i.|.]
-00001c80: 057d 017c 0188 0093 0271 0253 0072 0700  .}.|.....q.S.r..
-00001c90: 0000 7207 0000 0029 02da 022e 30da 0672  ..r....)....0..r
-00001ca0: 6567 696f 6ea9 01da 0178 7207 0000 0072  egion....xr....r
-00001cb0: 0900 0000 da0a 3c64 6963 7463 6f6d 703e  ......<dictcomp>
-00001cc0: 0601 0000 7302 0000 0012 007a 5149 6e73  ....s......zQIns
-00001cd0: 7461 6e74 6961 7465 644d 6f64 656c 2e5f  tantiatedModel._
-00001ce0: 7365 745f 696e 7374 616e 6365 5f64 6174  set_instance_dat
-00001cf0: 615f 636f 6163 6368 2e3c 6c6f 6361 6c73  a_coacch.<locals
-00001d00: 3e2e 3c6c 616d 6264 613e 2e3c 6c6f 6361  >.<lambda>.<loca
-00001d10: 6c73 3e2e 3c64 6963 7463 6f6d 703e 723d  ls>.<dictcomp>r=
-00001d20: 0000 0029 0172 1000 0000 729d 0000 0072  ...).r....r....r
-00001d30: 2000 0000 729d 0000 0072 0900 0000 720a   ...r....r....r.
-00001d40: 0000 0006 0100 0073 0200 0000 1800 7a3d  .......s......z=
-00001d50: 496e 7374 616e 7469 6174 6564 4d6f 6465  InstantiatedMode
-00001d60: 6c2e 5f73 6574 5f69 6e73 7461 6e63 655f  l._set_instance_
-00001d70: 6461 7461 5f63 6f61 6363 682e 3c6c 6f63  data_coacch.<loc
-00001d80: 616c 733e 2e3c 6c61 6d62 6461 3e7a 1052  als>.<lambda>z.R
-00001d90: 6f62 7573 742d 5175 6164 7261 7469 6372  obust-Quadraticr
-00001da0: 2500 0000 5a0c 636f 6d62 696e 6564 5f62  %...Z.combined_b
-00001db0: 315f 7a02 2d71 5a0c 636f 6d62 696e 6564  1_z.-qZ.combined
-00001dc0: 5f62 325f 7201 0000 0072 2900 0000 7a0d  _b2_r....r)...z.
-00001dd0: 526f 6275 7374 2d4c 696e 6561 7229 0ada  Robust-Linear)..
-00001de0: 1164 616d 6167 655f 6e6f 736c 725f 666f  .damage_noslr_fo
-00001df0: 726d da0f 6461 6d61 6765 5f6e 6f73 6c72  rm..damage_noslr
-00001e00: 5f62 31da 0f64 616d 6167 655f 6e6f 736c  _b1..damage_nosl
-00001e10: 725f 6232 da0f 6461 6d61 6765 5f6e 6f73  r_b2..damage_nos
-00001e20: 6c72 5f62 33da 0e64 616d 6167 655f 6e6f  lr_b3..damage_no
-00001e30: 736c 725f 61da 0f64 616d 6167 655f 736c  slr_a..damage_sl
-00001e40: 725f 666f 726d da0d 6461 6d61 6765 5f73  r_form..damage_s
-00001e50: 6c72 5f62 31da 0d64 616d 6167 655f 736c  lr_b1..damage_sl
-00001e60: 725f 6232 da0d 6461 6d61 6765 5f73 6c72  r_b2..damage_slr
-00001e70: 5f62 33da 0c64 616d 6167 655f 736c 725f  _b3..damage_slr_
-00001e80: 617a 0b4e 6f53 4c52 5f61 2028 713d fa01  az.NoSLR_a (q=..
-00001e90: 297a 065f 6120 2871 3d5a 0a4e 6f53 4c52  )z._a (q=Z.NoSLR
-00001ea0: 5f66 6f72 6d5a 084e 6f53 4c52 5f62 315a  _formZ.NoSLR_b1Z
-00001eb0: 084e 6f53 4c52 5f62 325a 084e 6f53 4c52  .NoSLR_b2Z.NoSLR
-00001ec0: 5f62 335a 055f 666f 726d 5a03 5f62 315a  _b3Z._formZ._b1Z
-00001ed0: 035f 6232 5a03 5f62 3329 0572 1000 0000  ._b2Z._b3).r....
-00001ee0: da08 4b65 7945 7272 6f72 720d 0000 0072  ..KeyErrorr....r
-00001ef0: 7400 0000 7275 0000 0029 0b72 1600 0000  t...ru...).r....
-00001f00: 7213 0000 005a 0f64 616d 6167 655f 7175  r....Z.damage_qu
-00001f10: 616e 7469 6c65 5a1b 636f 6d62 696e 6564  antileZ.combined
-00001f20: 5f73 6c72 5f6e 6f6e 736c 725f 6461 6d61  _slr_nonslr_dama
-00001f30: 6765 735a 0d73 6c72 5f77 6974 6861 6461  gesZ.slr_withada
-00001f40: 7074 5a0a 6164 6170 745f 7072 6678 5a04  ptZ.adapt_prfxZ.
-00001f50: 7072 6678 5a08 565f 7265 6769 6f6e 7277  prfxZ.V_regionrw
-00001f60: 0000 005a 0c66 6163 746f 725f 6e6f 736c  ...Z.factor_nosl
-00001f70: 725a 0d66 6163 746f 725f 736c 725f 6164  rZ.factor_slr_ad
-00001f80: 7207 0000 0072 2000 0000 7209 0000 0072  r....r ...r....r
-00001f90: 2e00 0000 f900 0000 735c 0000 0002 0116  ........s\......
-00001fa0: 010c 0108 0102 ff0c 0302 0104 ff12 030c  ................
-00001fb0: 010a 010c 0204 0206 0306 0110 0102 ff06  ................
-00001fc0: 0310 0102 ff06 0306 0106 0206 0106 0106  ................
-00001fd0: 0106 0108 f00c 1410 0106 0404 0102 ff0c  ................
-00001fe0: 030c 010c 010c 0106 020a 0102 ff12 0312  ................
-00001ff0: 0112 010c 0106 f012 137a 2b49 6e73 7461  .........z+Insta
-00002000: 6e74 6961 7465 644d 6f64 656c 2e5f 7365  ntiatedModel._se
-00002010: 745f 696e 7374 616e 6365 5f64 6174 615f  t_instance_data_
-00002020: 636f 6163 6368 2901 5429 0272 3300 0000  coacch).T).r3...
-00002030: 4e29 11da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00002040: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00002050: 6c6e 616d 655f 5f72 0200 0000 7205 0000  lname__r....r...
-00002060: 0072 0400 0000 da04 626f 6f6c 7217 0000  .r......boolr...
-00002070: 0072 1100 0000 7214 0000 0072 1200 0000  .r....r....r....
-00002080: 722a 0000 0072 7600 0000 722b 0000 0072  r*...rv...r+...r
-00002090: 2c00 0000 722d 0000 0072 2e00 0000 7207  ,...r-...r....r.
-000020a0: 0000 0072 0700 0000 7207 0000 0072 0900  ...r....r....r..
-000020b0: 0000 720b 0000 000b 0000 0073 2800 0000  ..r........s(...
-000020c0: 0800 0206 04fb 0202 02fe 0203 02fd 0204  ................
-000020d0: 02fc 0205 0afb 0816 080d 0803 0a34 0a5a  .............4.Z
-000020e0: 0a10 0a0d 0a0d 0e0f 720b 0000 0029 0bda  ........r....)..
-000020f0: 056e 756d 7079 726e 0000 00da 0d6d 696d  .numpyrn.....mim
-00002100: 6f73 612e 636f 6d6d 6f6e 7202 0000 0072  osa.commonr....r
-00002110: 0300 0000 5a12 6d69 6d6f 7361 2e63 6f6d  ....Z.mimosa.com
-00002120: 6d6f 6e2e 6461 7461 7204 0000 00da 1d6d  mon.datar......m
-00002130: 696d 6f73 612e 636f 6d6d 6f6e 2e72 6567  imosa.common.reg
-00002140: 696f 6e61 6c5f 7061 7261 6d73 7205 0000  ional_paramsr...
-00002150: 0072 7100 0000 720b 0000 0072 0700 0000  .rq...r....r....
-00002160: 7207 0000 0072 0700 0000 7209 0000 00da  r....r....r.....
-00002170: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
-00002180: 0000 0800 1001 0c01 0c01 0804 1203       ..............
+000010c0: 1e72 656c 5f6d 6974 6967 6174 696f 6e5f  .rel_mitigation_
+000010d0: 636f 7374 735f 6d69 6e5f 6c65 7665 6cda  costs_min_level.
+000010e0: 1869 6e69 745f 6361 7069 7461 6c73 746f  .init_capitalsto
+000010f0: 636b 5f66 6163 746f 72da 1369 6e69 745f  ck_factor..init_
+00001100: 6361 7069 7461 6c5f 6661 6374 6f72 da05  capital_factor..
+00001110: 616c 7068 6172 1a00 0000 da02 646b 7a17  alphar......dkz.
+00001120: 6465 7072 6563 6961 7469 6f6e 206f 6620  depreciation of 
+00001130: 6361 7069 7461 6c7a 0c73 6176 696e 6773  capitalz.savings
+00001140: 2072 6174 65da 0665 6c61 736d 75da 1069   rate..elasmu..i
+00001150: 6e65 7175 616c 5f61 7665 7273 696f 6eda  nequal_aversion.
+00001160: 0450 5254 5029 04da 0273 7272 6900 0000  .PRTP)...srri...
+00001170: 726a 0000 0072 6b00 0000 5a0e 6375 7374  rj...rk...Z.cust
+00001180: 6f6d 5f6d 6170 7069 6e67 da0a 7369 6d75  om_mapping..simu
+00001190: 6c61 7469 6f6e 290e 7210 0000 00da 0369  lation).r......i
+000011a0: 6e74 da02 6e70 da04 6365 696c 720c 0000  nt..np..ceilr...
+000011b0: 00da 0479 6561 72da 0156 da05 7261 6e67  ...year..V..rang
+000011c0: 65da 046b 6579 7372 0300 0000 720d 0000  e..keysr....r...
+000011d0: 00da 0367 6574 da06 7570 6461 7465 da16  ...get..update..
+000011e0: 5f73 6574 5f69 6e73 7461 6e63 655f 6461  _set_instance_da
+000011f0: 7461 5f73 6c72 2907 7216 0000 0072 1300  ta_slr).r....r..
+00001200: 0000 7210 0000 005a 0574 5f65 6e64 5a09  ..r....Z.t_endZ.
+00001210: 6e75 6d5f 7965 6172 7372 3c00 0000 da11  num_yearsr<.....
+00001220: 7061 7261 6d65 7465 725f 6d61 7070 696e  parameter_mappin
+00001230: 6772 0700 0000 7239 0000 0072 0900 0000  gr....r9...r....
+00001240: 722a 0000 0066 0000 0073 ea00 0000 0601  r*...f...s......
+00001250: 0c01 0c01 0c01 1a01 1201 1001 0202 0801  ................
+00001260: 02ff 0802 02fe 0c03 02fd 0c04 02fc 0805  ................
+00001270: 02fb 1006 02fa 0407 0a01 02ff 02f9 160a  ................
+00001280: 02f6 140b 02f5 140c 02f4 040d 1001 02ff  ................
+00001290: 02f3 0410 1001 02ff 02f0 0413 0a01 02ff  ................
+000012a0: 02ed 0416 0a01 02ff 02ea 0419 0a01 02ff  ................
+000012b0: 02e7 101c 02e4 101d 04e3 161e 02e2 041f  ................
+000012c0: 1001 02ff 02e1 0422 0201 0a01 0201 02fe  ......."........
+000012d0: 02ff 02de 1428 02d8 0e29 02d7 082a 02d6  .....(...)...*..
+000012e0: 142b 02d5 142c 02d4 042d 0e01 02ff 02d3  .+...,...-......
+000012f0: 1430 02d0 0431 0201 0e01 0201 02fe 02ff  .0...1..........
+00001300: 02cf 1437 02c9 0838 1001 02ff 02c8 043b  ...7...8.......;
+00001310: 0e01 02ff 02c5 083e 0401 02ff 02c2 1441  .......>.......A
+00001320: 02bf 1442 04be 1243 0e01 0e01 0e01 08ba  ...B...C........
+00001330: 0e49 1201 0e02 0e03 7a29 496e 7374 616e  .I......z)Instan
+00001340: 7469 6174 6564 4d6f 6465 6c2e 5f73 6574  tiatedModel._set
+00001350: 5f69 6e73 7461 6e63 655f 6461 7461 5f6d  _instance_data_m
+00001360: 6169 6e63 0200 0000 0000 0000 0000 0000  ainc............
+00001370: 0300 0000 0a00 0000 4300 0000 734e 0000  ........C...sN..
+00001380: 0074 0064 0183 0174 0064 0283 0174 0064  .t.d...t.d...t.d
+00001390: 0383 0174 0064 0483 0174 0064 0583 0174  ...t.d...t.d...t
+000013a0: 0064 0683 0174 0064 0783 0174 0064 0883  .d...t.d...t.d..
+000013b0: 0174 0064 0983 0164 0a9c 097d 027c 0164  .t.d...d...}.|.d
+000013c0: 0019 00a0 017c 02a1 0101 0064 0053 0029  .....|.....d.S.)
+000013d0: 0b4e e700 0000 0000 00e0 3f67 ccad 56ce  .N........?g..V.
+000013e0: ae91 b73f 67c4 c76c 7b6a a798 3f67 2d43  ...?g..l{j..?g-C
+000013f0: 1ceb e236 4a3f 67a4 703d 0ad7 a3d0 3fe9  ...6J?g.p=....?.
+00001400: ffff ffff 674b dc32 f9c9 e5f1 3f67 3333  ....gK.2....?g33
+00001410: 3333 3333 e33f 6733 3333 3333 331d 4029  3333.?g333333.@)
+00001420: 09da 1173 6c72 5f74 6865 726d 616c 5f65  ...slr_thermal_e
+00001430: 7175 696c da10 736c 725f 7468 6572 6d61  quil..slr_therma
+00001440: 6c5f 696e 6974 da17 736c 725f 7468 6572  l_init..slr_ther
+00001450: 6d61 6c5f 6164 6a75 7374 5f72 6174 65da  mal_adjust_rate.
+00001460: 1273 6c72 5f67 7369 635f 6d65 6c74 5f72  .slr_gsic_melt_r
+00001470: 6174 65da 1273 6c72 5f67 7369 635f 746f  ate..slr_gsic_to
+00001480: 7461 6c5f 6963 65da 1373 6c72 5f67 7369  tal_ice..slr_gsi
+00001490: 635f 6571 7569 6c5f 7465 6d70 da1e 736c  c_equil_temp..sl
+000014a0: 725f 6769 735f 6d65 6c74 5f72 6174 655f  r_gis_melt_rate_
+000014b0: 6162 6f76 655f 7468 7265 7368 da16 736c  above_thresh..sl
+000014c0: 725f 6769 735f 696e 6974 5f6d 656c 745f  r_gis_init_melt_
+000014d0: 7261 7465 da14 736c 725f 6769 735f 696e  rate..slr_gis_in
+000014e0: 6974 5f69 6365 5f76 6f6c 2902 7272 0000  it_ice_vol).rr..
+000014f0: 0072 7600 0000 a903 7216 0000 0072 1300  .rv.....r....r..
+00001500: 0000 7278 0000 0072 0700 0000 7207 0000  ..rx...r....r...
+00001510: 0072 0900 0000 7277 0000 00c0 0000 0073  .r....rw.......s
+00001520: 1600 0000 0603 0601 0601 0601 0601 0601  ................
+00001530: 0601 0601 0601 06f6 120d 7a28 496e 7374  ..........z(Inst
+00001540: 616e 7469 6174 6564 4d6f 6465 6c2e 5f73  antiatedModel._s
+00001550: 6574 5f69 6e73 7461 6e63 655f 6461 7461  et_instance_data
+00001560: 5f73 6c72 6302 0000 0000 0000 0000 0000  _slrc...........
+00001570: 0004 0000 0004 0000 0043 0000 0073 4200  .........C...sB.
+00001580: 0000 7c00 6a00 7d02 7401 7c02 6401 1900  ..|.j.}.t.|.d...
+00001590: 6402 1900 6403 1900 8301 7401 7c02 6401  d...d.....t.|.d.
+000015a0: 1900 6402 1900 6404 1900 8301 6405 9c02  ..d...d.....d...
+000015b0: 7d03 7c01 6400 1900 a002 7c03 a101 0100  }.|.d.....|.....
+000015c0: 6400 5300 2906 4e72 2600 0000 7a0e 656d  d.S.).Nr&...z.em
+000015d0: 6973 7369 6f6e 2074 7261 6465 7a15 6d69  ission tradez.mi
+000015e0: 6e20 7265 6c20 7061 796d 656e 7420 6c65  n rel payment le
+000015f0: 7665 6c7a 156d 6178 2072 656c 2070 6179  velz.max rel pay
+00001600: 6d65 6e74 206c 6576 656c 2902 da15 6d69  ment level)...mi
+00001610: 6e5f 7265 6c5f 7061 796d 656e 745f 6c65  n_rel_payment_le
+00001620: 7665 6cda 156d 6178 5f72 656c 5f70 6179  vel..max_rel_pay
+00001630: 6d65 6e74 5f6c 6576 656c 2903 7210 0000  ment_level).r...
+00001640: 0072 7200 0000 7276 0000 00a9 0472 1600  .rr...rv.....r..
+00001650: 0000 7213 0000 0072 1000 0000 7278 0000  ..r....r....rx..
+00001660: 0072 0700 0000 7207 0000 0072 0900 0000  .r....r....r....
+00001670: 722b 0000 00d0 0000 0073 1200 0000 0601  r+.......s......
+00001680: 0202 0e01 02ff 0203 0e01 02ff 06fc 1209  ................
+00001690: 7a41 496e 7374 616e 7469 6174 6564 4d6f  zAInstantiatedMo
+000016a0: 6465 6c2e 5f73 6574 5f69 6e73 7461 6e63  del._set_instanc
+000016b0: 655f 6461 7461 5f65 6d69 7373 696f 6e74  e_data_emissiont
+000016c0: 7261 6465 5f67 6c6f 6261 6c63 6f73 7470  rade_globalcostp
+000016d0: 6f6f 6c63 0200 0000 0000 0000 0000 0000  oolc............
+000016e0: 0400 0000 0900 0000 4300 0000 736c 0000  ........C...sl..
+000016f0: 007c 006a 007d 0274 017c 0264 0119 0064  .|.j.}.t.|.d...d
+00001700: 0219 0064 0319 0083 017c 006a 02a0 0364  ...d.....|.j...d
+00001710: 0464 05a1 027c 006a 02a0 0364 0464 06a1  .d...|.j...d.d..
+00001720: 027c 006a 02a0 0364 0464 07a1 027c 006a  .|.j...d.d...|.j
+00001730: 02a0 0364 0464 08a1 027c 006a 02a0 0364  ...d.d...|.j...d
+00001740: 0464 09a1 0264 0a9c 067d 037c 0164 0019  .d...d...}.|.d..
+00001750: 00a0 047c 03a1 0101 0064 0053 0029 0b4e  ...|.....d.S.).N
+00001760: 7226 0000 0072 5b00 0000 5a0a 6375 7272  r&...r[...Z.curr
+00001770: 5f6c 6576 656c da0a 4144 5249 4345 3230  _level..ADRICE20
+00001780: 3130 da02 6131 da02 6132 da02 6133 da02  10..a1..a2..a3..
+00001790: 6731 da02 6732 2906 da10 6164 6170 745f  g1..g2)...adapt_
+000017a0: 6375 7272 5f6c 6576 656c da09 6461 6d61  curr_level..dama
+000017b0: 6765 5f61 31da 0964 616d 6167 655f 6132  ge_a1..damage_a2
+000017c0: da09 6461 6d61 6765 5f61 33da 0861 6461  ..damage_a3..ada
+000017d0: 7074 5f67 31da 0861 6461 7074 5f67 3229  pt_g1..adapt_g2)
+000017e0: 0572 1000 0000 7272 0000 0072 0d00 0000  .r....rr...r....
+000017f0: 7275 0000 0072 7600 0000 7287 0000 0072  ru...rv...r....r
+00001800: 0700 0000 7207 0000 0072 0900 0000 722c  ....r....r....r,
+00001810: 0000 00dd 0000 0073 1200 0000 0601 1202  .......s........
+00001820: 0c01 0c01 0c01 0c01 0c01 06fa 1209 7a2d  ..............z-
+00001830: 496e 7374 616e 7469 6174 6564 4d6f 6465  InstantiatedMode
+00001840: 6c2e 5f73 6574 5f69 6e73 7461 6e63 655f  l._set_instance_
+00001850: 6461 7461 5f72 6963 6532 3031 3063 0200  data_rice2010c..
+00001860: 0000 0000 0000 0000 0000 0300 0000 0c00  ................
+00001870: 0000 4300 0000 737e 0000 007c 006a 00a0  ..C...s~...|.j..
+00001880: 0164 0164 02a1 027c 006a 00a0 0164 0164  .d.d...|.j...d.d
+00001890: 03a1 027c 006a 00a0 0164 0164 04a1 027c  ...|.j...d.d...|
+000018a0: 006a 00a0 0164 0164 05a1 027c 006a 00a0  .j...d.d...|.j..
+000018b0: 0164 0164 06a1 027c 006a 00a0 0164 0164  .d.d...|.j...d.d
+000018c0: 07a1 0274 0264 0883 017c 006a 00a0 0164  ...t.d...|.j...d
+000018d0: 0164 09a1 027c 006a 00a0 0164 0164 0aa1  .d...|.j...d.d..
+000018e0: 0264 0b9c 097d 027c 0164 0019 00a0 037c  .d...}.|.d.....|
+000018f0: 02a1 0101 0064 0053 0029 0c4e da0a 4144  .....d.S.).N..AD
+00001900: 5249 4345 3230 3132 7289 0000 0072 8a00  RICE2012r....r..
+00001910: 0000 728b 0000 005a 036e 7531 5a03 6e75  ..r....Z.nu1Z.nu
+00001920: 325a 036e 7533 7279 0000 005a 0773 6c72  2Z.nu3ry...Z.slr
+00001930: 6461 6d31 5a07 736c 7264 616d 3229 0972  dam1Z.slrdam2).r
+00001940: 8f00 0000 7290 0000 0072 9100 0000 da05  ....r....r......
+00001950: 6164 6170 31da 0561 6461 7032 da05 6164  adap1..adap2..ad
+00001960: 6170 33da 0961 6461 7074 5f72 686f da07  ap3..adapt_rho..
+00001970: 534c 5264 616d 31da 0753 4c52 6461 6d32  SLRdam1..SLRdam2
+00001980: 2904 720d 0000 0072 7500 0000 7272 0000  ).r....ru...rr..
+00001990: 0072 7600 0000 7284 0000 0072 0700 0000  .rv...r....r....
+000019a0: 7207 0000 0072 0900 0000 722d 0000 00ea  r....r....r-....
+000019b0: 0000 0073 1600 0000 0c02 0c01 0c01 0c01  ...s............
+000019c0: 0c01 0c01 0601 0c01 0c01 06f7 120c 7a2d  ..............z-
+000019d0: 496e 7374 616e 7469 6174 6564 4d6f 6465  InstantiatedMode
+000019e0: 6c2e 5f73 6574 5f69 6e73 7461 6e63 655f  l._set_instance_
+000019f0: 6461 7461 5f72 6963 6532 3031 3263 0200  data_rice2012c..
+00001a00: 0000 0000 0000 0000 0000 0b00 0000 0d00  ................
+00001a10: 0000 0300 0000 73a4 0100 007a 0b88 006a  ......s....z...j
+00001a20: 0064 0119 0064 0219 0064 0319 007d 0257  .d...d...d...}.W
+00001a30: 006e 0b04 0074 0179 1601 0001 0001 0064  .n...t.y.......d
+00001a40: 047d 0259 006e 0177 0088 006a 0064 0119  .}.Y.n.w...j.d..
+00001a50: 0064 0219 0064 0519 007d 0388 006a 0064  .d...d...}...j.d
+00001a60: 0119 0064 0219 0064 0619 007d 047c 0472  ...d...d...}.|.r
+00001a70: 2d64 076e 0164 087d 0564 097c 059b 009d  -d.n.d.}.d.|....
+00001a80: 027d 0687 0066 0164 0a64 0b84 087d 077c  .}...f.d.d...}.|
+00001a90: 0372 707c 0764 0c83 0188 006a 02a0 0364  .rp|.d.....j...d
+00001aa0: 0d64 0e7c 059b 0064 0f7c 029b 009d 04a1  .d.|...d.|......
+00001ab0: 0288 006a 02a0 0364 0d64 107c 059b 0064  ...j...d.d.|...d
+00001ac0: 0f7c 029b 009d 04a1 027c 0764 1183 017c  .|.......|.d...|
+00001ad0: 0764 1283 017c 0764 1383 017c 0764 1183  .d...|.d...|.d..
+00001ae0: 017c 0764 1183 017c 0764 1183 017c 0764  .|.d...|.d...|.d
+00001af0: 1183 0164 149c 0a7d 086e 5964 157c 029b  ...d...}.nYd.|..
+00001b00: 0064 169d 037d 097c 069b 0064 177c 029b  .d...}.|...d.|..
+00001b10: 0064 169d 047d 0a88 006a 02a0 0364 0d64  .d...}...j...d.d
+00001b20: 18a1 0288 006a 02a0 0364 0d64 19a1 0288  .....j...d.d....
+00001b30: 006a 02a0 0364 0d64 1aa1 0288 006a 02a0  .j...d.d.....j..
+00001b40: 0364 0d64 1ba1 0288 006a 02a0 0364 0d7c  .d.d.....j...d.|
+00001b50: 09a1 0288 006a 02a0 0364 0d7c 069b 0064  .....j...d.|...d
+00001b60: 1c9d 02a1 0288 006a 02a0 0364 0d7c 069b  .......j...d.|..
+00001b70: 0064 1d9d 02a1 0288 006a 02a0 0364 0d7c  .d.......j...d.|
+00001b80: 069b 0064 1e9d 02a1 0288 006a 02a0 0364  ...d.......j...d
+00001b90: 0d7c 069b 0064 1f9d 02a1 0288 006a 02a0  .|...d.......j..
+00001ba0: 0364 0d7c 0aa1 0264 149c 0a7d 087c 0164  .d.|...d...}.|.d
+00001bb0: 0019 00a0 047c 08a1 0101 0064 0053 0029  .....|.....d.S.)
+00001bc0: 204e 7226 0000 0072 2700 0000 da08 7175   Nr&...r'.....qu
+00001bd0: 616e 7469 6c65 7279 0000 005a 2263 6f61  antilery...Z"coa
+00001be0: 6363 685f 636f 6d62 696e 6564 5f73 6c72  cch_combined_slr
+00001bf0: 5f6e 6f6e 736c 725f 6461 6d61 6765 735a  _nonslr_damagesZ
+00001c00: 1463 6f61 6363 685f 736c 725f 7769 7468  .coacch_slr_with
+00001c10: 6164 6170 745a 0241 645a 044e 6f41 647a  adaptZ.AdZ.NoAdz
+00001c20: 0453 4c52 2d63 0100 0000 0000 0000 0000  .SLR-c..........
+00001c30: 0000 0100 0000 0300 0000 1300 0000 7318  ..............s.
+00001c40: 0000 0087 0066 0164 0164 0284 0888 016a  .....f.d.d.....j
+00001c50: 0064 0319 0044 0083 0153 0029 044e 6301  .d...D...S.).Nc.
+00001c60: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001c70: 0000 0013 0000 0073 1200 0000 6900 7c00  .......s....i.|.
+00001c80: 5d05 7d01 7c01 8800 9302 7102 5300 7207  ].}.|.....q.S.r.
+00001c90: 0000 0072 0700 0000 2902 da02 2e30 da06  ...r....)....0..
+00001ca0: 7265 6769 6f6e a901 da01 7872 0700 0000  region....xr....
+00001cb0: 7209 0000 00da 0a3c 6469 6374 636f 6d70  r......<dictcomp
+00001cc0: 3e06 0100 0073 0200 0000 1200 7a51 496e  >....s......zQIn
+00001cd0: 7374 616e 7469 6174 6564 4d6f 6465 6c2e  stantiatedModel.
+00001ce0: 5f73 6574 5f69 6e73 7461 6e63 655f 6461  _set_instance_da
+00001cf0: 7461 5f63 6f61 6363 682e 3c6c 6f63 616c  ta_coacch.<local
+00001d00: 733e 2e3c 6c61 6d62 6461 3e2e 3c6c 6f63  s>.<lambda>.<loc
+00001d10: 616c 733e 2e3c 6469 6374 636f 6d70 3e72  als>.<dictcomp>r
+00001d20: 3d00 0000 2901 7210 0000 0072 9e00 0000  =...).r....r....
+00001d30: 7220 0000 0072 9e00 0000 7209 0000 0072  r ...r....r....r
+00001d40: 0a00 0000 0601 0000 7302 0000 0018 007a  ........s......z
+00001d50: 3d49 6e73 7461 6e74 6961 7465 644d 6f64  =InstantiatedMod
+00001d60: 656c 2e5f 7365 745f 696e 7374 616e 6365  el._set_instance
+00001d70: 5f64 6174 615f 636f 6163 6368 2e3c 6c6f  _data_coacch.<lo
+00001d80: 6361 6c73 3e2e 3c6c 616d 6264 613e 7a10  cals>.<lambda>z.
+00001d90: 526f 6275 7374 2d51 7561 6472 6174 6963  Robust-Quadratic
+00001da0: 7225 0000 005a 0c63 6f6d 6269 6e65 645f  r%...Z.combined_
+00001db0: 6231 5f7a 022d 715a 0c63 6f6d 6269 6e65  b1_z.-qZ.combine
+00001dc0: 645f 6232 5f72 0100 0000 7229 0000 007a  d_b2_r....r)...z
+00001dd0: 0d52 6f62 7573 742d 4c69 6e65 6172 290a  .Robust-Linear).
+00001de0: da11 6461 6d61 6765 5f6e 6f73 6c72 5f66  ..damage_noslr_f
+00001df0: 6f72 6dda 0f64 616d 6167 655f 6e6f 736c  orm..damage_nosl
+00001e00: 725f 6231 da0f 6461 6d61 6765 5f6e 6f73  r_b1..damage_nos
+00001e10: 6c72 5f62 32da 0f64 616d 6167 655f 6e6f  lr_b2..damage_no
+00001e20: 736c 725f 6233 da0e 6461 6d61 6765 5f6e  slr_b3..damage_n
+00001e30: 6f73 6c72 5f61 da0f 6461 6d61 6765 5f73  oslr_a..damage_s
+00001e40: 6c72 5f66 6f72 6dda 0d64 616d 6167 655f  lr_form..damage_
+00001e50: 736c 725f 6231 da0d 6461 6d61 6765 5f73  slr_b1..damage_s
+00001e60: 6c72 5f62 32da 0d64 616d 6167 655f 736c  lr_b2..damage_sl
+00001e70: 725f 6233 da0c 6461 6d61 6765 5f73 6c72  r_b3..damage_slr
+00001e80: 5f61 7a0b 4e6f 534c 525f 6120 2871 3dfa  _az.NoSLR_a (q=.
+00001e90: 0129 7a06 5f61 2028 713d 5a0a 4e6f 534c  .)z._a (q=Z.NoSL
+00001ea0: 525f 666f 726d 5a08 4e6f 534c 525f 6231  R_formZ.NoSLR_b1
+00001eb0: 5a08 4e6f 534c 525f 6232 5a08 4e6f 534c  Z.NoSLR_b2Z.NoSL
+00001ec0: 525f 6233 5a05 5f66 6f72 6d5a 035f 6231  R_b3Z._formZ._b1
+00001ed0: 5a03 5f62 325a 035f 6233 2905 7210 0000  Z._b2Z._b3).r...
+00001ee0: 00da 084b 6579 4572 726f 7272 0d00 0000  ...KeyErrorr....
+00001ef0: 7275 0000 0072 7600 0000 290b 7216 0000  ru...rv...).r...
+00001f00: 0072 1300 0000 5a0f 6461 6d61 6765 5f71  .r....Z.damage_q
+00001f10: 7561 6e74 696c 655a 1b63 6f6d 6269 6e65  uantileZ.combine
+00001f20: 645f 736c 725f 6e6f 6e73 6c72 5f64 616d  d_slr_nonslr_dam
+00001f30: 6167 6573 5a0d 736c 725f 7769 7468 6164  agesZ.slr_withad
+00001f40: 6170 745a 0a61 6461 7074 5f70 7266 785a  aptZ.adapt_prfxZ
+00001f50: 0470 7266 785a 0856 5f72 6567 696f 6e72  .prfxZ.V_regionr
+00001f60: 7800 0000 5a0c 6661 6374 6f72 5f6e 6f73  x...Z.factor_nos
+00001f70: 6c72 5a0d 6661 6374 6f72 5f73 6c72 5f61  lrZ.factor_slr_a
+00001f80: 6472 0700 0000 7220 0000 0072 0900 0000  dr....r ...r....
+00001f90: 722e 0000 00f9 0000 0073 5c00 0000 0201  r........s\.....
+00001fa0: 1601 0c01 0801 02ff 0c03 0201 04ff 1203  ................
+00001fb0: 0c01 0a01 0c02 0402 0603 0601 1001 02ff  ................
+00001fc0: 0603 1001 02ff 0603 0601 0602 0601 0601  ................
+00001fd0: 0601 0601 08f0 0c14 1001 0604 0401 02ff  ................
+00001fe0: 0c03 0c01 0c01 0c01 0602 0a01 02ff 1203  ................
+00001ff0: 1201 1201 0c01 06f0 1213 7a2b 496e 7374  ..........z+Inst
+00002000: 616e 7469 6174 6564 4d6f 6465 6c2e 5f73  antiatedModel._s
+00002010: 6574 5f69 6e73 7461 6e63 655f 6461 7461  et_instance_data
+00002020: 5f63 6f61 6363 6829 0154 2902 7233 0000  _coacch).T).r3..
+00002030: 004e 2911 da08 5f5f 6e61 6d65 5f5f da0a  .N)...__name__..
+00002040: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00002050: 616c 6e61 6d65 5f5f 7202 0000 0072 0500  alname__r....r..
+00002060: 0000 7204 0000 00da 0462 6f6f 6c72 1700  ..r......boolr..
+00002070: 0000 7211 0000 0072 1400 0000 7212 0000  ..r....r....r...
+00002080: 0072 2a00 0000 7277 0000 0072 2b00 0000  .r*...rw...r+...
+00002090: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
+000020a0: 0700 0000 7207 0000 0072 0700 0000 7209  ....r....r....r.
+000020b0: 0000 0072 0b00 0000 0b00 0000 7328 0000  ...r........s(..
+000020c0: 0008 0002 0604 fb02 0202 fe02 0302 fd02  ................
+000020d0: 0402 fc02 050a fb08 1608 0d08 030a 340a  ..............4.
+000020e0: 5a0a 100a 0d0a 0d0e 0f72 0b00 0000 290b  Z........r....).
+000020f0: da05 6e75 6d70 7972 6f00 0000 da0d 6d69  ..numpyro.....mi
+00002100: 6d6f 7361 2e63 6f6d 6d6f 6e72 0200 0000  mosa.commonr....
+00002110: 7203 0000 005a 126d 696d 6f73 612e 636f  r....Z.mimosa.co
+00002120: 6d6d 6f6e 2e64 6174 6172 0400 0000 da1d  mmon.datar......
+00002130: 6d69 6d6f 7361 2e63 6f6d 6d6f 6e2e 7265  mimosa.common.re
+00002140: 6769 6f6e 616c 5f70 6172 616d 7372 0500  gional_paramsr..
+00002150: 0000 7272 0000 0072 0b00 0000 7207 0000  ..rr...r....r...
+00002160: 0072 0700 0000 7207 0000 0072 0900 0000  .r....r....r....
+00002170: da08 3c6d 6f64 756c 653e 0100 0000 730c  ..<module>....s.
+00002180: 0000 0008 0010 010c 010c 0108 0412 03    ...............
```

### Comparing `mimosa-0.1.3/mimosa/concrete_model/instantiate_params.py` & `mimosa-0.1.4/mimosa/concrete_model/instantiate_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,16 @@
                     "currency_unit/emissionsrate_unit",
                 )
             ),
             "MAC_beta": V(params["economics"]["MAC"]["beta"]),
             "MAC_scaling_factor": self.regional_param_store.get(
                 "MAC", params["economics"]["MAC"]["regional calibration factor"]
             ),
-            "rel_abatement_costs_min_level": V(
-                params["economics"]["MAC"]["rel_abatement_costs_min_level"]
+            "rel_mitigation_costs_min_level": V(
+                params["economics"]["MAC"]["rel_mitigation_costs_min_level"]
             ),
             "init_capitalstock_factor": self.regional_param_store.get(
                 "economics", "init_capital_factor"
             ),
             "alpha": V(params["economics"]["GDP"]["alpha"]),
             "dk": V(params["economics"]["GDP"]["depreciation of capital"]),
             "sr": V(params["economics"]["GDP"]["savings rate"]),
```

### Comparing `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc` & `mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 06:54:00 2023 UTC, .py size: 493 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 882b ba64 ed01 0000  o........+.d....
+00000000: 6f0d 0d0a 0000 0000 b769 ba64 ed01 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 8400 5a01 6403 5300 2904  Z.d.d...Z.d.S.).
 00000040: 7a89 0a43 6572 7461 696e 2063 6f6e 7374  z..Certain const
 00000050: 7261 696e 7473 2063 616e 2062 6520 6465  raints can be de
 00000060: 6163 7469 7661 7465 642e 2054 6865 7365  activated. These
 00000070: 2061 7265 2064 6566 696e 6564 2069 6e3a   are defined in:
@@ -21,19 +21,19 @@
 00000140: 6f6e 5a17 6465 6163 7469 7661 7465 645f  onZ.deactivated_
 00000150: 636f 6e73 7472 6169 6e74 73da 0b63 6f6e  constraints..con
 00000160: 7374 7261 696e 745f 2902 da07 6765 7461  straint_)...geta
 00000170: 7474 72da 0a64 6561 6374 6976 6174 6529  ttr..deactivate)
 00000180: 04da 016d da06 7061 7261 6d73 da0f 636f  ...m..params..co
 00000190: 6e73 7472 6169 6e74 5f6e 616d 65da 0a63  nstraint_name..c
 000001a0: 6f6e 7374 7261 696e 74a9 0072 0900 0000  onstraint..r....
-000001b0: fa81 633a 5c75 7365 7273 5c33 3930 3338  ..c:\users\39038
-000001c0: 3835 5c6f 6e65 6472 6976 6520 2d20 756e  85\onedrive - un
-000001d0: 6976 6572 7369 7465 6974 2075 7472 6563  iversiteit utrec
-000001e0: 6874 5c64 6f63 756d 656e 7473 5c6d 696d  ht\documents\mim
-000001f0: 6f73 615c 6d69 6d6f 7361 5c63 6f6e 6372  osa\mimosa\concr
+000001b0: fa81 633a 5c55 7365 7273 5c33 3930 3338  ..c:\Users\39038
+000001c0: 3835 5c4f 6e65 4472 6976 6520 2d20 556e  85\OneDrive - Un
+000001d0: 6976 6572 7369 7465 6974 2055 7472 6563  iversiteit Utrec
+000001e0: 6874 5c44 6f63 756d 656e 7473 5c4d 494d  ht\Documents\MIM
+000001f0: 4f53 415c 6d69 6d6f 7361 5c63 6f6e 6372  OSA\mimosa\concr
 00000200: 6574 655f 6d6f 6465 6c5c 7369 6d75 6c61  ete_model\simula
 00000210: 7469 6f6e 5f6d 6f64 655c 6465 6163 7469  tion_mode\deacti
 00000220: 7661 7465 5f63 6f6e 7374 7261 696e 7473  vate_constraints
 00000230: 2e70 79da 1664 6561 6374 6976 6174 655f  .py..deactivate_
 00000240: 636f 6e73 7472 6169 6e74 7307 0000 0073  constraints....s
 00000250: 1000 0000 1001 1001 1001 0801 0801 0280  ................
 00000260: 04fc 0401 720b 0000 004e 2902 da07 5f5f  ....r....N)...__
```

### Comparing `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc` & `mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:42 2023 UTC, .py size: 907 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b636 ba64 8b03 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b769 ba64 8b03 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
 00000040: 6404 6c03 6d03 5a03 0100 6403 6405 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6406 6502 6407 6506 6408  m.Z...d.e.d.e.d.
 00000060: 6409 6606 640a 640b 8404 5a07 6409 5300  d.f.d.d...Z.d.S.
 00000070: 290c 61cd 0100 000a 5468 6520 7369 6d75  ).a.....The simu
@@ -42,19 +42,19 @@
 00000290: 6564 5f76 6172 6961 626c 6573 da01 6dda  ed_variables..m.
 000002a0: 0670 6172 616d 73da 0672 6574 7572 6e4e  .params..returnN
 000002b0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
 000002c0: 0003 0000 0043 0000 0073 1800 0000 7400  .....C...s....t.
 000002d0: 7c00 7c01 8302 0100 7401 7c00 7c01 8302  |.|.....t.|.|...
 000002e0: 0100 6400 5300 2901 4e29 0272 0500 0000  ..d.S.).N).r....
 000002f0: 7204 0000 0029 0272 0600 0000 7207 0000  r....).r....r...
-00000300: 00a9 0072 0900 0000 fa6f 633a 5c75 7365  ...r.....oc:\use
-00000310: 7273 5c33 3930 3338 3835 5c6f 6e65 6472  rs\3903885\onedr
-00000320: 6976 6520 2d20 756e 6976 6572 7369 7465  ive - universite
-00000330: 6974 2075 7472 6563 6874 5c64 6f63 756d  it utrecht\docum
-00000340: 656e 7473 5c6d 696d 6f73 615c 6d69 6d6f  ents\mimosa\mimo
+00000300: 00a9 0072 0900 0000 fa6f 633a 5c55 7365  ...r.....oc:\Use
+00000310: 7273 5c33 3930 3338 3835 5c4f 6e65 4472  rs\3903885\OneDr
+00000320: 6976 6520 2d20 556e 6976 6572 7369 7465  ive - Universite
+00000330: 6974 2055 7472 6563 6874 5c44 6f63 756d  it Utrecht\Docum
+00000340: 656e 7473 5c4d 494d 4f53 415c 6d69 6d6f  ents\MIMOSA\mimo
 00000350: 7361 5c63 6f6e 6372 6574 655f 6d6f 6465  sa\concrete_mode
 00000360: 6c5c 7369 6d75 6c61 7469 6f6e 5f6d 6f64  l\simulation_mod
 00000370: 655c 6d61 696e 2e70 79da 1373 6574 5f73  e\main.py..set_s
 00000380: 696d 756c 6174 696f 6e5f 6d6f 6465 1500  imulation_mode..
 00000390: 0000 7304 0000 000a 020e 0372 0b00 0000  ..s........r....
 000003a0: 2908 da07 5f5f 646f 635f 5fda 0d6d 696d  )...__doc__..mim
 000003b0: 6f73 612e 636f 6d6d 6f6e 7202 0000 0072  osa.commonr....r
```

### Comparing `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc` & `mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:42 2023 UTC, .py size: 3369 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b636 ba64 290d 0000  o........6.d)...
+00000000: 6f0d 0d0a 0000 0000 b769 ba64 290d 0000  o........i.d)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6404 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6406 6407 8400 5a0b 6408 6409 8400  ..d.d...Z.d.d...
 00000070: 5a0c 640a 640b 8400 5a0d 640c 640d 8400  Z.d.d...Z.d.d...
@@ -36,18 +36,18 @@
 00000230: 2908 da01 6dda 0670 6172 616d 73da 0a64  )...m..params..d
 00000240: 6174 615f 6361 6368 65da 1165 7874 7261  ata_cache..extra
 00000250: 5f63 6f6e 7374 7261 696e 7473 da0d 7661  _constraints..va
 00000260: 7269 6162 6c65 5f6e 616d 65da 1066 696c  riable_name..fil
 00000270: 6570 6174 685f 6f72 5f64 6174 61da 0b69  epath_or_data..i
 00000280: 6e74 6572 705f 6461 7461 da0a 636f 6e73  nterp_data..cons
 00000290: 7472 6169 6e74 a900 7218 0000 00fa 7a63  traint..r.....zc
-000002a0: 3a5c 7573 6572 735c 3339 3033 3838 355c  :\users\3903885\
-000002b0: 6f6e 6564 7269 7665 202d 2075 6e69 7665  onedrive - unive
-000002c0: 7273 6974 6569 7420 7574 7265 6368 745c  rsiteit utrecht\
-000002d0: 646f 6375 6d65 6e74 735c 6d69 6d6f 7361  documents\mimosa
+000002a0: 3a5c 5573 6572 735c 3339 3033 3838 355c  :\Users\3903885\
+000002b0: 4f6e 6544 7269 7665 202d 2055 6e69 7665  OneDrive - Unive
+000002c0: 7273 6974 6569 7420 5574 7265 6368 745c  rsiteit Utrecht\
+000002d0: 446f 6375 6d65 6e74 735c 4d49 4d4f 5341  Documents\MIMOSA
 000002e0: 5c6d 696d 6f73 615c 636f 6e63 7265 7465  \mimosa\concrete
 000002f0: 5f6d 6f64 656c 5c73 696d 756c 6174 696f  _model\simulatio
 00000300: 6e5f 6d6f 6465 5c73 6574 5f63 6f6e 7374  n_mode\set_const
 00000310: 7261 696e 7473 2e70 79da 1f73 6574 5f63  raints.py..set_c
 00000320: 6f6e 7374 7261 696e 7473 5f66 6978 6564  onstraints_fixed
 00000330: 5f76 6172 6961 626c 6573 0f00 0000 7318  _variables....s.
 00000340: 0000 0004 0104 0106 0202 0102 ff04 020a  ................
```

### Comparing `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.4/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:42 2023 UTC, .py size: 1557 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b636 ba64 1506 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 b769 ba64 1506 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6403 6c06 5a07 6401 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6407 6408 8400 5a0c 4700 6409 640a  ..d.d...Z.G.d.d.
@@ -23,19 +23,19 @@
 00000160: 6420 7b7d 2066 696c 6573 2069 6e73 7465  d {} files inste
 00000170: 6164 206f 6620 3120 666f 7220 6669 6c65  ad of 1 for file
 00000180: 2070 6174 7465 726e 207b 7d72 0100 0000   pattern {}r....
 00000190: 2907 7202 0000 00da 036c 656e 7205 0000  ).r......lenr...
 000001a0: 00da 0777 6172 6e69 6e67 da06 666f 726d  ...warning..form
 000001b0: 6174 da02 7064 da08 7265 6164 5f63 7376  at..pd..read_csv
 000001c0: 2902 da04 7061 7468 da05 7061 7468 73a9  )...path..paths.
-000001d0: 0072 0f00 0000 fa70 633a 5c75 7365 7273  .r.....pc:\users
-000001e0: 5c33 3930 3338 3835 5c6f 6e65 6472 6976  \3903885\onedriv
-000001f0: 6520 2d20 756e 6976 6572 7369 7465 6974  e - universiteit
-00000200: 2075 7472 6563 6874 5c64 6f63 756d 656e   utrecht\documen
-00000210: 7473 5c6d 696d 6f73 615c 6d69 6d6f 7361  ts\mimosa\mimosa
+000001d0: 0072 0f00 0000 fa70 633a 5c55 7365 7273  .r.....pc:\Users
+000001e0: 5c33 3930 3338 3835 5c4f 6e65 4472 6976  \3903885\OneDriv
+000001f0: 6520 2d20 556e 6976 6572 7369 7465 6974  e - Universiteit
+00000200: 2055 7472 6563 6874 5c44 6f63 756d 656e   Utrecht\Documen
+00000210: 7473 5c4d 494d 4f53 415c 6d69 6d6f 7361  ts\MIMOSA\mimosa
 00000220: 5c63 6f6e 6372 6574 655f 6d6f 6465 6c5c  \concrete_model\
 00000230: 7369 6d75 6c61 7469 6f6e 5f6d 6f64 655c  simulation_mode\
 00000240: 7574 696c 732e 7079 720c 0000 000f 0000  utils.pyr.......
 00000250: 0073 1400 0000 0801 0801 0c01 0401 0401  .s..............
 00000260: 0801 02ff 04ff 0c05 0a01 720c 0000 0063  ..........r....c
 00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000280: 0300 0000 4000 0000 732c 0000 0065 005a  ....@...s,...e.Z
```

### Comparing `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/main.py` & `mimosa-0.1.4/mimosa/concrete_model/simulation_mode/main.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/set_constraints.py` & `mimosa-0.1.4/mimosa/concrete_model/simulation_mode/set_constraints.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/utils.py` & `mimosa-0.1.4/mimosa/concrete_model/simulation_mode/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/export/__pycache__/plot.cpython-310.pyc` & `mimosa-0.1.4/mimosa/export/__pycache__/plot.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:42 2023 UTC, .py size: 5262 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b636 ba64 8e14 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 baa0 ba64 9114 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6407 6405 6406 8401 5a04  m.Z...d.d.d...Z.
 00000050: 6402 5300 2908 6132 0100 000a 4372 6561  d.S.).a2....Crea
 00000060: 7465 7320 6120 6269 6720 506c 6f74 6c79  tes a big Plotly
 00000070: 2066 6967 7572 6520 7769 7468 2065 6163   figure with eac
@@ -132,79 +132,79 @@
 00000830: da08 6261 7365 6c69 6e65 da0e 4174 7472  ..baseline..Attr
 00000840: 6962 7574 6545 7272 6f72 5a12 7265 6769  ibuteErrorZ.regi
 00000850: 6f6e 616c 5f65 6d69 7373 696f 6e73 5a0b  onal_emissionsZ.
 00000860: 6361 7262 6f6e 7072 6963 655a 0b61 6461  carbonpriceZ.ada
 00000870: 7074 5f63 6f73 7473 5a0d 7265 7369 645f  pt_costsZ.resid_
 00000880: 6461 6d61 6765 735a 0d67 726f 7373 5f64  damagesZ.gross_d
 00000890: 616d 6167 6573 5a0c 6461 6d61 6765 5f63  amagesZ.damage_c
-000008a0: 6f73 7473 5a13 7265 6c5f 6162 6174 656d  ostsZ.rel_abatem
-000008b0: 656e 745f 636f 7374 735a 0d63 6170 6974  ent_costsZ.capit
-000008c0: 616c 5f73 746f 636b 5a09 4744 505f 6772  al_stockZ.GDP_gr
-000008d0: 6f73 735a 0747 4450 5f6e 6574 5a0b 636f  ossZ.GDP_netZ.co
-000008e0: 6e73 756d 7074 696f 6e5a 0775 7469 6c69  nsumptionZ.utili
-000008f0: 7479 5a0f 6162 6174 656d 656e 745f 636f  tyZ.abatement_co
-00000900: 7374 735a 1067 6c6f 6261 6c5f 656d 6973  stsZ.global_emis
-00000910: 7369 6f6e 73da 0b74 656d 7065 7261 7475  sions..temperatu
-00000920: 7265 5a14 6375 6d75 6c61 7469 7665 5f65  reZ.cumulative_e
-00000930: 6d69 7373 696f 6e73 5a1a 676c 6f62 616c  missionsZ.global
-00000940: 5f72 656c 5f61 6261 7465 6d65 6e74 5f63  _rel_abatement_c
-00000950: 6f73 7473 5a1c 656d 6973 7369 6f6e 5f72  ostsZ.emission_r
-00000960: 656c 6174 6976 655f 6375 6d75 6c61 7469  elative_cumulati
-00000970: 7665 5a10 636f 6e73 756d 7074 696f 6e5f  veZ.consumption_
-00000980: 6c6f 7373 5a0f 736d 6f6f 7468 6564 5f66  lossZ.smoothed_f
-00000990: 6163 746f 725a 156e 6574 6e65 6761 7469  actorZ.netnegati
-000009a0: 7665 5f65 6d69 7373 696f 6e73 5a09 6f76  ve_emissionsZ.ov
-000009b0: 6572 7368 6f6f 745a 0b61 6461 7074 5f6c  ershootZ.adapt_l
-000009c0: 6576 656c 5a09 6164 6170 745f 4641 445a  evelZ.adapt_FADZ
-000009d0: 0961 6461 7074 5f53 4144 5a09 6164 6170  .adapt_SADZ.adap
-000009e0: 745f 4941 445a 0b53 4c52 5f64 616d 6167  t_IADZ.SLR_damag
-000009f0: 6573 5a09 746f 7461 6c5f 534c 52da 0353  esZ.total_SLR..S
-00000a00: 4c52 5a07 4355 4d47 5349 435a 0643 554d  LRZ.CUMGSICZ.CUM
-00000a10: 4749 535a 0a4c 4244 5f66 6163 746f 72da  GISZ.LBD_factor.
-00000a20: 0474 6573 745a 1461 6461 7074 5f63 6f73  .testZ.adapt_cos
-00000a30: 7473 5f72 6561 6374 6976 655a 1561 6461  ts_reactiveZ.ada
-00000a40: 7074 5f63 6f73 7473 5f70 726f 6163 7469  pt_costs_proacti
-00000a50: 7665 5a13 6164 6170 745f 636f 7374 735f  veZ.adapt_costs_
-00000a60: 7370 6563 6361 705a 0b61 6461 7074 5f51  speccapZ.adapt_Q
-00000a70: 5f63 6170 5a11 6164 6170 745f 4b5f 7072  _capZ.adapt_K_pr
-00000a80: 6f61 6374 6976 655a 1073 6574 5f79 6178  oactiveZ.set_yax
-00000a90: 6573 5f74 6974 6c65 73da 0366 6967 5a0c  es_titles..figZ.
-00000aa0: 7570 6461 7465 5f79 6178 6573 da03 6c65  update_yaxes..le
-00000ab0: 6eda 0772 6567 696f 6e73 5a0a 7365 745f  n..regionsZ.set_
-00000ac0: 6c61 796f 7574 5a0d 7570 6461 7465 5f6c  layoutZ.update_l
-00000ad0: 6179 6f75 74da 026f 73da 086d 616b 6564  ayout..os..maked
-00000ae0: 6972 73da 0666 6f72 6d61 74da 0570 7269  irs..format..pri
-00000af0: 6e74 5a0a 7772 6974 655f 6874 6d6c 2907  ntZ.write_html).
-00000b00: da01 6dda 0866 696c 656e 616d 6572 1300  ..m..filenamer..
-00000b10: 0000 5a0d 6375 7374 6f6d 5f6c 6179 6f75  ..Z.custom_layou
-00000b20: 74da 0470 6c6f 74da 096f 7574 7075 7464  t..plot..outputd
-00000b30: 6972 5a0a 6f75 7470 7574 6669 6c65 a900  irZ.outputfile..
-00000b40: 7225 0000 00fa 5763 3a5c 7573 6572 735c  r%....Wc:\users\
-00000b50: 3339 3033 3838 355c 6f6e 6564 7269 7665  3903885\onedrive
-00000b60: 202d 2075 6e69 7665 7273 6974 6569 7420   - universiteit 
-00000b70: 7574 7265 6368 745c 646f 6375 6d65 6e74  utrecht\document
-00000b80: 735c 6d69 6d6f 7361 5c6d 696d 6f73 615c  s\mimosa\mimosa\
-00000b90: 6578 706f 7274 5c70 6c6f 742e 7079 da09  export\plot.py..
-00000ba0: 6675 6c6c 5f70 6c6f 740d 0000 0073 0201  full_plot....s..
-00000bb0: 0000 0801 0401 0e02 1402 0201 1401 0c01  ................
-00000bc0: 0401 02ff 1002 1201 0201 1201 1201 1401  ................
-00000bd0: 0c01 1601 02ff 1202 1002 1001 1001 1201  ................
-00000be0: 1401 1201 1201 1401 1401 0202 0401 0401  ................
-00000bf0: 0201 0201 0201 0201 0afb 0c07 0401 02ff  ................
-00000c00: 0205 0401 0401 0201 0201 0201 0201 06fb  ................
-00000c10: 0407 0401 0201 0201 0201 0201 06fb 0407  ................
-00000c20: 0401 0201 0201 0201 0201 06fb 0407 0a01  ................
-00000c30: 06ff 1803 0e01 0401 02ff 0203 1402 1401  ................
-00000c40: 1401 1401 1201 0401 0401 0201 0201 0201  ................
-00000c50: 0201 06fb 0407 0c01 06ff 0403 0c01 06ff  ................
-00000c60: 0403 0c01 06ff 0403 0401 0201 0201 0201  ................
-00000c70: 0201 06fb 0407 0c01 0aff 0e03 0401 02ff  ................
-00000c80: 0203 1402 1401 1401 1401 1801 0e01 0401  ................
-00000c90: 02ff 0403 0601 04ff 0603 0e01 06ff 0603  ................
-00000ca0: 0e01 06ff 1003 0801 0c01 0402 1201 0c01  ................
-00000cb0: 0e01 1401 7227 0000 0029 0254 4e29 05da  ....r'...).TN)..
-00000cc0: 075f 5f64 6f63 5f5f 721d 0000 005a 136d  .__doc__r....Z.m
-00000cd0: 696d 6f73 612e 6578 706f 7274 2e75 7469  imosa.export.uti
-00000ce0: 6c73 7202 0000 0072 2700 0000 7225 0000  lsr....r'...r%..
-00000cf0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00000d00: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
-00000d10: 0000 0004 0008 080c 010e 03              ...........
+000008a0: 6f73 7473 5a14 7265 6c5f 6d69 7469 6761  ostsZ.rel_mitiga
+000008b0: 7469 6f6e 5f63 6f73 7473 5a0d 6361 7069  tion_costsZ.capi
+000008c0: 7461 6c5f 7374 6f63 6b5a 0947 4450 5f67  tal_stockZ.GDP_g
+000008d0: 726f 7373 5a07 4744 505f 6e65 745a 0b63  rossZ.GDP_netZ.c
+000008e0: 6f6e 7375 6d70 7469 6f6e 5a07 7574 696c  onsumptionZ.util
+000008f0: 6974 795a 106d 6974 6967 6174 696f 6e5f  ityZ.mitigation_
+00000900: 636f 7374 735a 1067 6c6f 6261 6c5f 656d  costsZ.global_em
+00000910: 6973 7369 6f6e 73da 0b74 656d 7065 7261  issions..tempera
+00000920: 7475 7265 5a14 6375 6d75 6c61 7469 7665  tureZ.cumulative
+00000930: 5f65 6d69 7373 696f 6e73 5a1b 676c 6f62  _emissionsZ.glob
+00000940: 616c 5f72 656c 5f6d 6974 6967 6174 696f  al_rel_mitigatio
+00000950: 6e5f 636f 7374 735a 1c65 6d69 7373 696f  n_costsZ.emissio
+00000960: 6e5f 7265 6c61 7469 7665 5f63 756d 756c  n_relative_cumul
+00000970: 6174 6976 655a 1063 6f6e 7375 6d70 7469  ativeZ.consumpti
+00000980: 6f6e 5f6c 6f73 735a 0f73 6d6f 6f74 6865  on_lossZ.smoothe
+00000990: 645f 6661 6374 6f72 5a15 6e65 746e 6567  d_factorZ.netneg
+000009a0: 6174 6976 655f 656d 6973 7369 6f6e 735a  ative_emissionsZ
+000009b0: 096f 7665 7273 686f 6f74 5a0b 6164 6170  .overshootZ.adap
+000009c0: 745f 6c65 7665 6c5a 0961 6461 7074 5f46  t_levelZ.adapt_F
+000009d0: 4144 5a09 6164 6170 745f 5341 445a 0961  ADZ.adapt_SADZ.a
+000009e0: 6461 7074 5f49 4144 5a0b 534c 525f 6461  dapt_IADZ.SLR_da
+000009f0: 6d61 6765 735a 0974 6f74 616c 5f53 4c52  magesZ.total_SLR
+00000a00: da03 534c 525a 0743 554d 4753 4943 5a06  ..SLRZ.CUMGSICZ.
+00000a10: 4355 4d47 4953 5a0a 4c42 445f 6661 6374  CUMGISZ.LBD_fact
+00000a20: 6f72 da04 7465 7374 5a14 6164 6170 745f  or..testZ.adapt_
+00000a30: 636f 7374 735f 7265 6163 7469 7665 5a15  costs_reactiveZ.
+00000a40: 6164 6170 745f 636f 7374 735f 7072 6f61  adapt_costs_proa
+00000a50: 6374 6976 655a 1361 6461 7074 5f63 6f73  ctiveZ.adapt_cos
+00000a60: 7473 5f73 7065 6363 6170 5a0b 6164 6170  ts_speccapZ.adap
+00000a70: 745f 515f 6361 705a 1161 6461 7074 5f4b  t_Q_capZ.adapt_K
+00000a80: 5f70 726f 6163 7469 7665 5a10 7365 745f  _proactiveZ.set_
+00000a90: 7961 7865 735f 7469 746c 6573 da03 6669  yaxes_titles..fi
+00000aa0: 675a 0c75 7064 6174 655f 7961 7865 73da  gZ.update_yaxes.
+00000ab0: 036c 656e da07 7265 6769 6f6e 735a 0a73  .len..regionsZ.s
+00000ac0: 6574 5f6c 6179 6f75 745a 0d75 7064 6174  et_layoutZ.updat
+00000ad0: 655f 6c61 796f 7574 da02 6f73 da08 6d61  e_layout..os..ma
+00000ae0: 6b65 6469 7273 da06 666f 726d 6174 da05  kedirs..format..
+00000af0: 7072 696e 745a 0a77 7269 7465 5f68 746d  printZ.write_htm
+00000b00: 6c29 07da 016d da08 6669 6c65 6e61 6d65  l)...m..filename
+00000b10: 7213 0000 005a 0d63 7573 746f 6d5f 6c61  r....Z.custom_la
+00000b20: 796f 7574 da04 706c 6f74 da09 6f75 7470  yout..plot..outp
+00000b30: 7574 6469 725a 0a6f 7574 7075 7466 696c  utdirZ.outputfil
+00000b40: 65a9 0072 2500 0000 fa57 633a 5c55 7365  e..r%....Wc:\Use
+00000b50: 7273 5c33 3930 3338 3835 5c4f 6e65 4472  rs\3903885\OneDr
+00000b60: 6976 6520 2d20 556e 6976 6572 7369 7465  ive - Universite
+00000b70: 6974 2055 7472 6563 6874 5c44 6f63 756d  it Utrecht\Docum
+00000b80: 656e 7473 5c4d 494d 4f53 415c 6d69 6d6f  ents\MIMOSA\mimo
+00000b90: 7361 5c65 7870 6f72 745c 706c 6f74 2e70  sa\export\plot.p
+00000ba0: 79da 0966 756c 6c5f 706c 6f74 0d00 0000  y..full_plot....
+00000bb0: 7302 0100 0008 0104 010e 0214 0202 0114  s...............
+00000bc0: 010c 0104 0102 ff10 0212 0102 0112 0112  ................
+00000bd0: 0114 010c 0116 0102 ff12 0210 0210 0110  ................
+00000be0: 0112 0114 0112 0112 0114 0114 0102 0204  ................
+00000bf0: 0104 0102 0102 0102 0102 010a fb0c 0704  ................
+00000c00: 0102 ff02 0504 0104 0102 0102 0102 0102  ................
+00000c10: 0106 fb04 0704 0102 0102 0102 0102 0106  ................
+00000c20: fb04 0704 0102 0102 0102 0102 0106 fb04  ................
+00000c30: 070a 0106 ff18 030e 0104 0102 ff02 0314  ................
+00000c40: 0214 0114 0114 0112 0104 0104 0102 0102  ................
+00000c50: 0102 0102 0106 fb04 070c 0106 ff04 030c  ................
+00000c60: 0106 ff04 030c 0106 ff04 0304 0102 0102  ................
+00000c70: 0102 0102 0106 fb04 070c 010a ff0e 0304  ................
+00000c80: 0102 ff02 0314 0214 0114 0114 0118 010e  ................
+00000c90: 0104 0102 ff04 0306 0104 ff06 030e 0106  ................
+00000ca0: ff06 030e 0106 ff10 0308 010c 0104 0212  ................
+00000cb0: 010c 010e 0114 0172 2700 0000 2902 544e  .......r'...).TN
+00000cc0: 2905 da07 5f5f 646f 635f 5f72 1d00 0000  )...__doc__r....
+00000cd0: 5a13 6d69 6d6f 7361 2e65 7870 6f72 742e  Z.mimosa.export.
+00000ce0: 7574 696c 7372 0200 0000 7227 0000 0072  utilsr....r'...r
+00000cf0: 2500 0000 7225 0000 0072 2500 0000 7226  %...r%...r%...r&
+00000d00: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000d10: 0073 0800 0000 0400 0808 0c01 0e03       .s............
```

### Comparing `mimosa-0.1.3/mimosa/export/__pycache__/save.cpython-310.pyc` & `mimosa-0.1.4/mimosa/export/__pycache__/save.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 07:41:42 2023 UTC, .py size: 3110 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,161 +1,160 @@
-00000000: 6f0d 0d0a 0000 0000 b636 ba64 260c 0000  o........6.d&...
+00000000: 6f0d 0d0a 0000 0000 18ad bb64 180c 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
+00000020: 0003 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 5a04 6401 6402 6c05 5a06 6401 6402 6c07  Z.d.d.l.Z.d.d.l.
-00000060: 5a08 6401 6403 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
-00000070: 0100 640c 6406 6407 8401 5a0c 6408 6409  ..d.d.d...Z.d.d.
-00000080: 8400 5a0d 640a 640b 8400 5a0e 6402 5300  ..Z.d.d...Z.d.S.
-00000090: 290d 7a55 0a47 656e 6572 6174 6573 2061  ).zU.Generates a
-000000a0: 2043 5356 2066 696c 6520 7769 7468 2061   CSV file with a
-000000b0: 2072 6f77 2066 6f72 2065 6163 6820 7661   row for each va
-000000c0: 7269 6162 6c65 2028 6056 6172 6029 0a69  riable (`Var`).i
-000000d0: 6e20 7468 6520 436f 6e63 7265 7465 4d6f  n the ConcreteMo
-000000e0: 6465 6c20 606d 602e 0ae9 0000 0000 4e29  del `m`.......N)
-000000f0: 02da 1167 6574 5f61 6c6c 5f76 6172 6961  ...get_all_varia
-00000100: 626c 6573 da05 7661 6c75 6554 da06 6f75  bles..valueT..ou
-00000110: 7470 7574 6305 0000 0000 0000 0000 0000  tputc...........
-00000120: 000e 0000 0008 0000 0043 0000 0073 1201  .........C...s..
-00000130: 0000 7c03 7213 7400 a001 7402 a003 7c00  ..|.r.t...t...|.
-00000140: a101 a004 a100 a101 a005 a100 6400 6401  ............d.d.
-00000150: 8502 1900 7d05 6e02 6402 7d05 7406 7c01  ....}.n.d.}.t.|.
-00000160: 8301 7d06 7c01 6a07 6403 6702 6701 7d07  ..}.|.j.d.g.g.}.
-00000170: 6700 7d08 7c07 4400 5d0a 7d09 7408 7c08  g.}.|.D.].}.t.|.
-00000180: 7c01 7c09 6404 6400 8305 0100 7123 7c06  |.|.d.d.....q#|.
-00000190: 4400 5d0d 7d0a 7408 7c08 7c01 7c0a 6a09  D.].}.t.|.|.|.j.
-000001a0: 7c0a 6a0a 7c0a 6a0b 8305 0100 7130 740c  |.j.|.j.....q0t.
-000001b0: 7c08 7c01 8302 7d0b 740d 6a0e 7c04 6405  |.|...}.t.j.|.d.
-000001c0: 1700 6404 6406 8d02 0100 7c03 7255 7c02  ..d.d.....|.rU|.
-000001d0: 9b00 6407 7c05 9b00 9d03 6e01 7c02 7d0c  ..d.|.....n.|.}.
-000001e0: 7c0b 6a0f 7c04 9b00 6405 7c0c 9b00 6408  |.j.|...d.|...d.
-000001f0: 9d04 6409 640a 640b 8d03 0100 7410 7c04  ..d.d.d.....t.|.
-00000200: 9b00 6405 7c0c 9b00 640c 9d04 640d 8302  ..d.|...d...d...
-00000210: 8f0f 7d0d 7402 a011 7c00 7c0d a102 0100  ..}.t...|.|.....
-00000220: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
-00000230: 3100 7382 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
-00000240: 6400 5300 290e 4ee9 0900 0000 da00 da0a  d.S.).N.........
-00000250: 706f 7075 6c61 7469 6f6e 54fa 012f 2901  populationT../).
-00000260: da08 6578 6973 745f 6f6b da01 5f7a 042e  ..exist_ok.._z..
-00000270: 6373 767a 0425 2e36 6746 2902 da0c 666c  csvz.%.6gF)...fl
-00000280: 6f61 745f 666f 726d 6174 da05 696e 6465  oat_format..inde
-00000290: 787a 102e 6373 762e 7061 7261 6d73 2e6a  xz..csv.params.j
-000002a0: 736f 6eda 0177 2912 da07 6861 7368 6c69  son..w)...hashli
-000002b0: 62da 036d 6435 da04 6a73 6f6e da05 6475  b..md5..json..du
-000002c0: 6d70 73da 0665 6e63 6f64 65da 0968 6578  mps..encode..hex
-000002d0: 6469 6765 7374 7202 0000 0072 0700 0000  digestr....r....
-000002e0: da0a 7661 725f 746f 5f72 6f77 da03 7661  ..var_to_row..va
-000002f0: 72da 0b69 735f 7265 6769 6f6e 616c da04  r..is_regional..
-00000300: 756e 6974 da11 726f 7773 5f74 6f5f 6461  unit..rows_to_da
-00000310: 7461 6672 616d 65da 026f 73da 086d 616b  taframe..os..mak
-00000320: 6564 6972 73da 0674 6f5f 6373 76da 046f  edirs..to_csv..o
-00000330: 7065 6eda 0464 756d 7029 0eda 0670 6172  pen..dump)...par
-00000340: 616d 73da 016d da0a 6578 7065 7269 6d65  ams..m..experime
-00000350: 6e74 5a0b 6861 7368 5f73 7566 6669 78da  ntZ.hash_suffix.
-00000360: 0666 6f6c 6465 725a 0d73 6574 7469 6e67  .folderZ.setting
-00000370: 735f 6861 7368 da0d 616c 6c5f 7661 7269  s_hash..all_vari
-00000380: 6162 6c65 735a 0d61 6c6c 5f66 756e 6374  ablesZ.all_funct
-00000390: 696f 6e73 da04 726f 7773 7215 0000 005a  ions..rowsr....Z
-000003a0: 0a75 7365 6675 6c5f 7661 72da 0964 6174  .useful_var..dat
-000003b0: 6166 7261 6d65 da08 6669 6c65 6e61 6d65  aframe..filename
-000003c0: da02 6668 a900 7227 0000 00fa 5763 3a5c  ..fh..r'....Wc:\
-000003d0: 7573 6572 735c 3339 3033 3838 355c 6f6e  users\3903885\on
-000003e0: 6564 7269 7665 202d 2075 6e69 7665 7273  edrive - univers
-000003f0: 6974 6569 7420 7574 7265 6368 745c 646f  iteit utrecht\do
-00000400: 6375 6d65 6e74 735c 6d69 6d6f 7361 5c6d  cuments\mimosa\m
-00000410: 696d 6f73 615c 6578 706f 7274 5c73 6176  imosa\export\sav
-00000420: 652e 7079 da0b 7361 7665 5f6f 7574 7075  e.py..save_outpu
-00000430: 7410 0000 0073 2200 0000 0402 2201 0402  t....s"....."...
-00000440: 0803 0c02 0402 0801 1201 0801 1801 0a01  ................
-00000450: 1205 1601 1c02 1803 0e01 22ff 7229 0000  ..........".r)..
-00000460: 0063 0500 0000 0000 0000 0000 0000 0600  .c..............
-00000470: 0000 0700 0000 0300 0000 73a0 0000 0074  ..........s....t
-00000480: 0088 0374 0183 0272 0e88 0364 0119 007d  ...t...r...d...}
-00000490: 0588 0364 0219 0089 036e 0388 036a 027d  ...d.....n...j.}
-000004a0: 057c 0372 3587 0187 0366 0264 0364 0484  .|.r5....f.d.d..
-000004b0: 0889 0088 016a 0344 005d 1589 027c 00a0  .....j.D.]...|..
-000004c0: 047c 0588 027c 0467 0387 0087 0266 0264  .|...|.g.....f.d
-000004d0: 0564 0684 0888 016a 0544 0083 0117 00a1  .d.....j.D......
-000004e0: 0101 0071 1d64 0053 0087 0187 0366 0264  ...q.d.S.....f.d
-000004f0: 0764 0484 0889 007c 00a0 047c 0564 087c  .d.....|...|.d.|
-00000500: 0467 0387 0066 0164 0964 0684 0888 016a  .g...f.d.d.....j
-00000510: 0544 0083 0117 00a1 0101 0064 0053 0029  .D.........d.S.)
-00000520: 0a4e e901 0000 0072 0100 0000 6302 0000  .N.....r....c...
-00000530: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000540: 0013 0000 0073 2800 0000 7400 8801 8301  .....s(...t.....
-00000550: 720c 8801 8800 a001 7c00 a101 7c01 8302  r.......|...|...
-00000560: 5300 7402 8801 7c00 7c01 6602 1900 8301  S.t...|.|.f.....
-00000570: 5300 a901 4ea9 03da 0863 616c 6c61 626c  S...N....callabl
-00000580: 65da 0479 6561 7272 0300 0000 2902 da01  e..yearr....)...
-00000590: 74da 0172 a902 721f 0000 0072 1500 0000  t..r..r....r....
-000005a0: 7227 0000 0072 2800 0000 da08 3c6c 616d  r'...r(.....<lam
-000005b0: 6264 613e 3a00 0000 7302 0000 0028 007a  bda>:...s....(.z
-000005c0: 1c76 6172 5f74 6f5f 726f 772e 3c6c 6f63  .var_to_row.<loc
-000005d0: 616c 733e 2e3c 6c61 6d62 6461 3e63 0100  als>.<lambda>c..
-000005e0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-000005f0: 0000 1300 0000 7316 0000 0067 007c 005d  ......s....g.|.]
-00000600: 077d 0188 007c 0188 0183 0291 0271 0253  .}...|.......q.S
-00000610: 0072 2700 0000 7227 0000 00a9 02da 022e  .r'...r'........
-00000620: 3072 2f00 0000 2902 da03 6663 7472 3000  0r/...)...fctr0.
-00000630: 0000 7227 0000 0072 2800 0000 da0a 3c6c  ..r'...r(.....<l
-00000640: 6973 7463 6f6d 703e 3c00 0000 f302 0000  istcomp><.......
-00000650: 0016 007a 1e76 6172 5f74 6f5f 726f 772e  ...z.var_to_row.
-00000660: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000670: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-00000680: 0100 0000 0400 0000 1300 0000 7322 0000  ............s"..
-00000690: 0074 0088 0183 0172 0b88 0188 00a0 017c  .t.....r.......|
-000006a0: 00a1 0183 0153 0074 0288 017c 0019 0083  .....S.t...|....
-000006b0: 0153 0072 2b00 0000 722c 0000 0029 0172  .S.r+...r,...).r
-000006c0: 2f00 0000 7231 0000 0072 2700 0000 7228  /...r1...r'...r(
-000006d0: 0000 0072 3200 0000 3e00 0000 7302 0000  ...r2...>...s...
-000006e0: 0022 00da 0647 6c6f 6261 6c63 0100 0000  ."...Globalc....
-000006f0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000700: 1300 0000 7314 0000 0067 007c 005d 067d  ....s....g.|.].}
-00000710: 0188 007c 0183 0191 0271 0253 0072 2700  ...|.....q.S.r'.
-00000720: 0000 7227 0000 0072 3300 0000 2901 7235  ..r'...r3...).r5
-00000730: 0000 0072 2700 0000 7228 0000 0072 3600  ...r'...r(...r6.
-00000740: 0000 3f00 0000 7302 0000 0014 0029 06da  ..?...s......)..
-00000750: 0a69 7369 6e73 7461 6e63 65da 046c 6973  .isinstance..lis
-00000760: 74da 046e 616d 65da 0772 6567 696f 6e73  t..name..regions
-00000770: da06 6170 7065 6e64 722f 0000 0029 0672  ..appendr/...).r
-00000780: 2300 0000 721f 0000 0072 1500 0000 7216  #...r....r....r.
-00000790: 0000 0072 1700 0000 723b 0000 0072 2700  ...r....r;...r'.
-000007a0: 0000 2904 7235 0000 0072 1f00 0000 7230  ..).r5...r....r0
-000007b0: 0000 0072 1500 0000 7228 0000 0072 1400  ...r....r(...r..
-000007c0: 0000 3000 0000 7316 0000 000a 0208 010a  ..0...s.........
-000007d0: 0106 0204 030e 010a 0128 0104 ff0e 0328  .........(.....(
-000007e0: 0172 1400 0000 6302 0000 0000 0000 0000  .r....c.........
-000007f0: 0000 0004 0000 0006 0000 0043 0000 0073  ...........C...s
-00000800: 3600 0000 6401 6402 8400 7c01 a000 7401  6...d.d...|...t.
-00000810: a002 7c01 6a03 a101 a101 4400 8301 7d02  ..|.j.....D...}.
-00000820: 6700 6403 a201 7c02 1700 7d03 7404 6a05  g.d...|...}.t.j.
-00000830: 7c00 7c03 6404 8d02 5300 2905 4e63 0100  |.|.d...S.).Nc..
-00000840: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00000850: 0000 5300 0000 7316 0000 0067 007c 005d  ..S...s....g.|.]
-00000860: 077d 0164 00a0 007c 01a1 0191 0271 0253  .}.d...|.....q.S
-00000870: 0029 017a 047b 3a67 7d29 01da 0666 6f72  .).z.{:g})...for
-00000880: 6d61 7429 0272 3400 0000 722e 0000 0072  mat).r4...r....r
-00000890: 2700 0000 7227 0000 0072 2800 0000 7236  '...r'...r(...r6
-000008a0: 0000 0043 0000 0072 3700 0000 7a25 726f  ...C...r7...z%ro
-000008b0: 7773 5f74 6f5f 6461 7461 6672 616d 652e  ws_to_dataframe.
-000008c0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000008d0: 6d70 3e29 03da 0856 6172 6961 626c 655a  mp>)...VariableZ
-000008e0: 0652 6567 696f 6eda 0455 6e69 7429 01da  .Region..Unit)..
-000008f0: 0763 6f6c 756d 6e73 2906 722e 0000 00da  .columns).r.....
-00000900: 026e 70da 0561 7272 6179 722f 0000 00da  .np..arrayr/....
-00000910: 0270 64da 0944 6174 6146 7261 6d65 2904  .pd..DataFrame).
-00000920: 7223 0000 0072 1f00 0000 da05 7965 6172  r#...r......year
-00000930: 7372 4100 0000 7227 0000 0072 2700 0000  srA...r'...r'...
-00000940: 7228 0000 0072 1800 0000 4200 0000 7306  r(...r....B...s.
-00000950: 0000 001c 010c 010e 0172 1800 0000 2903  .........r....).
-00000960: 4e54 7204 0000 0029 0fda 075f 5f64 6f63  NTr....)...__doc
-00000970: 5f5f 7210 0000 0072 1900 0000 da06 7261  __r....r......ra
-00000980: 6e64 6f6d 720e 0000 00da 056e 756d 7079  ndomr......numpy
-00000990: 7242 0000 00da 0670 616e 6461 7372 4400  rB.....pandasrD.
-000009a0: 0000 da0d 6d69 6d6f 7361 2e63 6f6d 6d6f  ....mimosa.commo
-000009b0: 6e72 0200 0000 7203 0000 0072 2900 0000  nr....r....r)...
-000009c0: 7214 0000 0072 1800 0000 7227 0000 0072  r....r....r'...r
-000009d0: 2700 0000 7227 0000 0072 2800 0000 da08  '...r'...r(.....
-000009e0: 3c6d 6f64 756c 653e 0100 0000 7316 0000  <module>....s...
-000009f0: 0004 0008 0508 0108 0108 0108 0108 0110  ................
-00000a00: 020a 0308 200c 12                        .... ..
+00000050: 5a05 6401 6402 6c06 5a07 6401 6403 6c08  Z.d.d.l.Z.d.d.l.
+00000060: 6d09 5a09 6d0a 5a0a 0100 640c 6406 6407  m.Z.m.Z...d.d.d.
+00000070: 8401 5a0b 6408 6409 8400 5a0c 640a 640b  ..Z.d.d...Z.d.d.
+00000080: 8400 5a0d 6402 5300 290d 7a55 0a47 656e  ..Z.d.S.).zU.Gen
+00000090: 6572 6174 6573 2061 2043 5356 2066 696c  erates a CSV fil
+000000a0: 6520 7769 7468 2061 2072 6f77 2066 6f72  e with a row for
+000000b0: 2065 6163 6820 7661 7269 6162 6c65 2028   each variable (
+000000c0: 6056 6172 6029 0a69 6e20 7468 6520 436f  `Var`).in the Co
+000000d0: 6e63 7265 7465 4d6f 6465 6c20 606d 602e  ncreteModel `m`.
+000000e0: 0ae9 0000 0000 4e29 02da 1167 6574 5f61  ......N)...get_a
+000000f0: 6c6c 5f76 6172 6961 626c 6573 da05 7661  ll_variables..va
+00000100: 6c75 6546 da06 6f75 7470 7574 6305 0000  lueF..outputc...
+00000110: 0000 0000 0000 0000 000e 0000 0008 0000  ................
+00000120: 0043 0000 0073 1201 0000 7c03 7213 7400  .C...s....|.r.t.
+00000130: a001 7402 a003 7c00 a101 a004 a100 a101  ..t...|.........
+00000140: a005 a100 6400 6401 8502 1900 7d05 6e02  ....d.d.....}.n.
+00000150: 6402 7d05 7406 7c01 8301 7d06 7c01 6a07  d.}.t.|...}.|.j.
+00000160: 6403 6702 6701 7d07 6700 7d08 7c07 4400  d.g.g.}.g.}.|.D.
+00000170: 5d0a 7d09 7408 7c08 7c01 7c09 6404 6400  ].}.t.|.|.|.d.d.
+00000180: 8305 0100 7123 7c06 4400 5d0d 7d0a 7408  ....q#|.D.].}.t.
+00000190: 7c08 7c01 7c0a 6a09 7c0a 6a0a 7c0a 6a0b  |.|.|.j.|.j.|.j.
+000001a0: 8305 0100 7130 740c 7c08 7c01 8302 7d0b  ....q0t.|.|...}.
+000001b0: 740d 6a0e 7c04 6405 1700 6404 6406 8d02  t.j.|.d...d.d...
+000001c0: 0100 7c03 7255 7c02 9b00 6407 7c05 9b00  ..|.rU|...d.|...
+000001d0: 9d03 6e01 7c02 7d0c 7c0b 6a0f 7c04 9b00  ..n.|.}.|.j.|...
+000001e0: 6405 7c0c 9b00 6408 9d04 6409 640a 640b  d.|...d...d.d.d.
+000001f0: 8d03 0100 7410 7c04 9b00 6405 7c0c 9b00  ....t.|...d.|...
+00000200: 640c 9d04 640d 8302 8f0f 7d0d 7402 a011  d...d.....}.t...
+00000210: 7c00 7c0d a102 0100 5700 6400 0400 0400  |.|.....W.d.....
+00000220: 8303 0100 6400 5300 3100 7382 7701 0100  ....d.S.1.s.w...
+00000230: 0100 0100 5900 0100 6400 5300 290e 4ee9  ....Y...d.S.).N.
+00000240: 0900 0000 da00 da0a 706f 7075 6c61 7469  ........populati
+00000250: 6f6e 54fa 012f 2901 da08 6578 6973 745f  onT../)...exist_
+00000260: 6f6b da01 5f7a 042e 6373 767a 0425 2e36  ok.._z..csvz.%.6
+00000270: 6746 2902 da0c 666c 6f61 745f 666f 726d  gF)...float_form
+00000280: 6174 da05 696e 6465 787a 102e 6373 762e  at..indexz..csv.
+00000290: 7061 7261 6d73 2e6a 736f 6eda 0177 2912  params.json..w).
+000002a0: da07 6861 7368 6c69 62da 036d 6435 da04  ..hashlib..md5..
+000002b0: 6a73 6f6e da05 6475 6d70 73da 0665 6e63  json..dumps..enc
+000002c0: 6f64 65da 0968 6578 6469 6765 7374 7202  ode..hexdigestr.
+000002d0: 0000 0072 0700 0000 da0a 7661 725f 746f  ...r......var_to
+000002e0: 5f72 6f77 da03 7661 72da 0b69 735f 7265  _row..var..is_re
+000002f0: 6769 6f6e 616c da04 756e 6974 da11 726f  gional..unit..ro
+00000300: 7773 5f74 6f5f 6461 7461 6672 616d 65da  ws_to_dataframe.
+00000310: 026f 73da 086d 616b 6564 6972 73da 0674  .os..makedirs..t
+00000320: 6f5f 6373 76da 046f 7065 6eda 0464 756d  o_csv..open..dum
+00000330: 7029 0eda 0670 6172 616d 73da 016d da0a  p)...params..m..
+00000340: 6578 7065 7269 6d65 6e74 5a0b 6861 7368  experimentZ.hash
+00000350: 5f73 7566 6669 78da 0666 6f6c 6465 725a  _suffix..folderZ
+00000360: 0d73 6574 7469 6e67 735f 6861 7368 da0d  .settings_hash..
+00000370: 616c 6c5f 7661 7269 6162 6c65 735a 0d61  all_variablesZ.a
+00000380: 6c6c 5f66 756e 6374 696f 6e73 da04 726f  ll_functions..ro
+00000390: 7773 7215 0000 005a 0a75 7365 6675 6c5f  wsr....Z.useful_
+000003a0: 7661 72da 0964 6174 6166 7261 6d65 da08  var..dataframe..
+000003b0: 6669 6c65 6e61 6d65 da02 6668 a900 7227  filename..fh..r'
+000003c0: 0000 00fa 5763 3a5c 5573 6572 735c 3339  ....Wc:\Users\39
+000003d0: 3033 3838 355c 4f6e 6544 7269 7665 202d  03885\OneDrive -
+000003e0: 2055 6e69 7665 7273 6974 6569 7420 5574   Universiteit Ut
+000003f0: 7265 6368 745c 446f 6375 6d65 6e74 735c  recht\Documents\
+00000400: 4d49 4d4f 5341 5c6d 696d 6f73 615c 6578  MIMOSA\mimosa\ex
+00000410: 706f 7274 5c73 6176 652e 7079 da0b 7361  port\save.py..sa
+00000420: 7665 5f6f 7574 7075 740f 0000 0073 2200  ve_output....s".
+00000430: 0000 0402 2201 0402 0803 0c02 0402 0801  ...."...........
+00000440: 1201 0801 1801 0a01 1205 1601 1c02 1803  ................
+00000450: 0e01 22ff 7229 0000 0063 0500 0000 0000  ..".r)...c......
+00000460: 0000 0000 0000 0600 0000 0700 0000 0300  ................
+00000470: 0000 73a0 0000 0074 0088 0374 0183 0272  ..s....t...t...r
+00000480: 0e88 0364 0119 007d 0588 0364 0219 0089  ...d...}...d....
+00000490: 036e 0388 036a 027d 057c 0372 3587 0187  .n...j.}.|.r5...
+000004a0: 0366 0264 0364 0484 0889 0088 016a 0344  .f.d.d.......j.D
+000004b0: 005d 1589 027c 00a0 047c 0588 027c 0467  .]...|...|...|.g
+000004c0: 0387 0087 0266 0264 0564 0684 0888 016a  .....f.d.d.....j
+000004d0: 0544 0083 0117 00a1 0101 0071 1d64 0053  .D.........q.d.S
+000004e0: 0087 0187 0366 0264 0764 0484 0889 007c  .....f.d.d.....|
+000004f0: 00a0 047c 0564 087c 0467 0387 0066 0164  ...|.d.|.g...f.d
+00000500: 0964 0684 0888 016a 0544 0083 0117 00a1  .d.....j.D......
+00000510: 0101 0064 0053 0029 0a4e e901 0000 0072  ...d.S.).N.....r
+00000520: 0100 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000530: 0002 0000 0004 0000 0013 0000 0073 2800  .............s(.
+00000540: 0000 7400 8801 8301 720c 8801 8800 a001  ..t.....r.......
+00000550: 7c00 a101 7c01 8302 5300 7402 8801 7c00  |...|...S.t...|.
+00000560: 7c01 6602 1900 8301 5300 a901 4ea9 03da  |.f.....S...N...
+00000570: 0863 616c 6c61 626c 65da 0479 6561 7272  .callable..yearr
+00000580: 0300 0000 2902 da01 74da 0172 a902 721f  ....)...t..r..r.
+00000590: 0000 0072 1500 0000 7227 0000 0072 2800  ...r....r'...r(.
+000005a0: 0000 da08 3c6c 616d 6264 613e 3900 0000  ....<lambda>9...
+000005b0: 7302 0000 0028 007a 1c76 6172 5f74 6f5f  s....(.z.var_to_
+000005c0: 726f 772e 3c6c 6f63 616c 733e 2e3c 6c61  row.<locals>.<la
+000005d0: 6d62 6461 3e63 0100 0000 0000 0000 0000  mbda>c..........
+000005e0: 0000 0200 0000 0500 0000 1300 0000 7316  ..............s.
+000005f0: 0000 0067 007c 005d 077d 0188 007c 0188  ...g.|.].}...|..
+00000600: 0183 0291 0271 0253 0072 2700 0000 7227  .....q.S.r'...r'
+00000610: 0000 00a9 02da 022e 3072 2f00 0000 2902  ........0r/...).
+00000620: da03 6663 7472 3000 0000 7227 0000 0072  ..fctr0...r'...r
+00000630: 2800 0000 da0a 3c6c 6973 7463 6f6d 703e  (.....<listcomp>
+00000640: 3b00 0000 f302 0000 0016 007a 1e76 6172  ;..........z.var
+00000650: 5f74 6f5f 726f 772e 3c6c 6f63 616c 733e  _to_row.<locals>
+00000660: 2e3c 6c69 7374 636f 6d70 3e63 0100 0000  .<listcomp>c....
+00000670: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000680: 1300 0000 7322 0000 0074 0088 0183 0172  ....s"...t.....r
+00000690: 0b88 0188 00a0 017c 00a1 0183 0153 0074  .......|.....S.t
+000006a0: 0288 017c 0019 0083 0153 0072 2b00 0000  ...|.....S.r+...
+000006b0: 722c 0000 0029 0172 2f00 0000 7231 0000  r,...).r/...r1..
+000006c0: 0072 2700 0000 7228 0000 0072 3200 0000  .r'...r(...r2...
+000006d0: 3d00 0000 7302 0000 0022 00da 0647 6c6f  =...s...."...Glo
+000006e0: 6261 6c63 0100 0000 0000 0000 0000 0000  balc............
+000006f0: 0200 0000 0400 0000 1300 0000 7314 0000  ............s...
+00000700: 0067 007c 005d 067d 0188 007c 0183 0191  .g.|.].}...|....
+00000710: 0271 0253 0072 2700 0000 7227 0000 0072  .q.S.r'...r'...r
+00000720: 3300 0000 2901 7235 0000 0072 2700 0000  3...).r5...r'...
+00000730: 7228 0000 0072 3600 0000 3e00 0000 7302  r(...r6...>...s.
+00000740: 0000 0014 0029 06da 0a69 7369 6e73 7461  .....)...isinsta
+00000750: 6e63 65da 046c 6973 74da 046e 616d 65da  nce..list..name.
+00000760: 0772 6567 696f 6e73 da06 6170 7065 6e64  .regions..append
+00000770: 722f 0000 0029 0672 2300 0000 721f 0000  r/...).r#...r...
+00000780: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000790: 723b 0000 0072 2700 0000 2904 7235 0000  r;...r'...).r5..
+000007a0: 0072 1f00 0000 7230 0000 0072 1500 0000  .r....r0...r....
+000007b0: 7228 0000 0072 1400 0000 2f00 0000 7316  r(...r..../...s.
+000007c0: 0000 000a 0208 010a 0106 0204 030e 010a  ................
+000007d0: 0128 0104 ff0e 0328 0172 1400 0000 6302  .(.....(.r....c.
+000007e0: 0000 0000 0000 0000 0000 0004 0000 0006  ................
+000007f0: 0000 0043 0000 0073 3600 0000 6401 6402  ...C...s6...d.d.
+00000800: 8400 7c01 a000 7401 a002 7c01 6a03 a101  ..|...t...|.j...
+00000810: a101 4400 8301 7d02 6700 6403 a201 7c02  ..D...}.g.d...|.
+00000820: 1700 7d03 7404 6a05 7c00 7c03 6404 8d02  ..}.t.j.|.|.d...
+00000830: 5300 2905 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000840: 0000 0200 0000 0500 0000 5300 0000 7316  ..........S...s.
+00000850: 0000 0067 007c 005d 077d 0164 00a0 007c  ...g.|.].}.d...|
+00000860: 01a1 0191 0271 0253 0029 017a 047b 3a67  .....q.S.).z.{:g
+00000870: 7d29 01da 0666 6f72 6d61 7429 0272 3400  })...format).r4.
+00000880: 0000 722e 0000 0072 2700 0000 7227 0000  ..r....r'...r'..
+00000890: 0072 2800 0000 7236 0000 0042 0000 0072  .r(...r6...B...r
+000008a0: 3700 0000 7a25 726f 7773 5f74 6f5f 6461  7...z%rows_to_da
+000008b0: 7461 6672 616d 652e 3c6c 6f63 616c 733e  taframe.<locals>
+000008c0: 2e3c 6c69 7374 636f 6d70 3e29 03da 0856  .<listcomp>)...V
+000008d0: 6172 6961 626c 655a 0652 6567 696f 6eda  ariableZ.Region.
+000008e0: 0455 6e69 7429 01da 0763 6f6c 756d 6e73  .Unit)...columns
+000008f0: 2906 722e 0000 00da 026e 70da 0561 7272  ).r......np..arr
+00000900: 6179 722f 0000 00da 0270 64da 0944 6174  ayr/.....pd..Dat
+00000910: 6146 7261 6d65 2904 7223 0000 0072 1f00  aFrame).r#...r..
+00000920: 0000 da05 7965 6172 7372 4100 0000 7227  ....yearsrA...r'
+00000930: 0000 0072 2700 0000 7228 0000 0072 1800  ...r'...r(...r..
+00000940: 0000 4100 0000 7306 0000 001c 010c 010e  ..A...s.........
+00000950: 0172 1800 0000 2903 4e46 7204 0000 0029  .r....).NFr....)
+00000960: 0eda 075f 5f64 6f63 5f5f 7210 0000 0072  ...__doc__r....r
+00000970: 1900 0000 720e 0000 00da 056e 756d 7079  ....r......numpy
+00000980: 7242 0000 00da 0670 616e 6461 7372 4400  rB.....pandasrD.
+00000990: 0000 da0d 6d69 6d6f 7361 2e63 6f6d 6d6f  ....mimosa.commo
+000009a0: 6e72 0200 0000 7203 0000 0072 2900 0000  nr....r....r)...
+000009b0: 7214 0000 0072 1800 0000 7227 0000 0072  r....r....r'...r
+000009c0: 2700 0000 7227 0000 0072 2800 0000 da08  '...r'...r(.....
+000009d0: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
+000009e0: 0004 0008 0508 0108 0108 0108 0110 020a  ................
+000009f0: 0308 200c 12                             .. ..
```

### Comparing `mimosa-0.1.3/mimosa/export/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.4/mimosa/export/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 21 06:54:00 2023 UTC, .py size: 5783 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,335 +1,338 @@
-00000000: 6f0d 0d0a 0000 0000 882b ba64 9716 0000  o........+.d....
+00000000: 6f0d 0d0a 0000 0000 b769 ba64 cc16 0000  o........i.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
+00000020: 0008 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
-00000040: 5a04 6401 6402 6c05 6d06 5a07 0100 6401  Z.d.d.l.m.Z...d.
-00000050: 6403 6c08 6d09 5a09 0100 6401 6404 6c0a  d.l.m.Z...d.d.l.
-00000060: 6d0b 5a0b 0100 6700 6405 a201 5a0c 4700  m.Z...g.d...Z.G.
-00000070: 6406 6407 8400 6407 8302 5a0d 6408 6409  d.d...d...Z.d.d.
-00000080: 8400 5a0e 6402 5300 290a 7a35 0a50 6c6f  ..Z.d.S.).z5.Plo
-00000090: 7420 6675 6e63 7469 6f6e 732e 204e 6f74  t functions. Not
-000000a0: 206e 6563 6573 7361 7279 2069 6620 6461   necessary if da
-000000b0: 7368 626f 6172 6420 6973 2075 7365 642e  shboard is used.
-000000c0: 0ae9 0000 0000 4e29 01da 0d6d 616b 655f  ......N)...make_
-000000d0: 7375 6270 6c6f 7473 a901 da05 7661 6c75  subplots....valu
-000000e0: 6529 107a 0723 3030 4145 4546 7a07 2338  e).z.#00AEEFz.#8
-000000f0: 3038 4431 447a 0723 4236 3033 3643 7a07  08D1Dz.#B6036Cz.
-00000100: 2346 4141 4431 457a 0723 3346 3134 3634  #FAAD1Ez.#3F1464
-00000110: 7a07 2337 4343 4646 327a 0723 4631 3938  z.#7CCFF2z.#F198
-00000120: 4331 7a07 2334 3242 3634 397a 0723 4545  C1z.#42B649z.#EE
-00000130: 3241 3233 7a07 2330 3034 3031 397a 0723  2A23z.#004019z.#
-00000140: 4634 3733 3231 7a07 2335 3131 3630 377a  F47321z.#511607z
-00000150: 0723 4241 3839 3132 7a07 2337 3843 4242  .#BA8912z.#78CBB
-00000160: 467a 0723 4646 4632 3239 7a07 2330 3037  Fz.#FFF229z.#007
-00000170: 3142 4263 0000 0000 0000 0000 0000 0000  1BBc............
-00000180: 0000 0000 0300 0000 4000 0000 7354 0000  ........@...sT..
-00000190: 0065 005a 0164 005a 0264 015a 0364 1764  .e.Z.d.Z.d.Z.d.d
-000001a0: 0464 0584 015a 0464 0664 0784 005a 0564  .d...Z.d.d...Z.d
-000001b0: 0864 0984 005a 0664 0a64 0b84 005a 0764  .d...Z.d.d...Z.d
-000001c0: 1864 0f64 1084 015a 0864 1164 1284 005a  .d.d...Z.d.d...Z
-000001d0: 0964 1364 1484 005a 0a64 1564 1684 005a  .d.d...Z.d.d...Z
-000001e0: 0b64 0353 0029 19da 0450 6c6f 747a 9e0a  .d.S.)...Plotz..
-000001f0: 2020 2020 5772 6170 7065 7220 666f 7220      Wrapper for 
-00000200: 6120 506c 6f74 6c79 2066 6967 7572 652e  a Plotly figure.
-00000210: 0a0a 2020 2020 4669 7273 7420 6974 2063  ..    First it c
-00000220: 7265 6174 6573 2061 2073 7562 706c 6f74  reates a subplot
-00000230: 2066 6967 7572 652c 2074 6865 6e20 7573   figure, then us
-00000240: 696e 6720 7468 6520 6675 6e63 7469 6f6e  ing the function
-00000250: 2060 6164 6460 2c0a 2020 2020 6120 7472   `add`,.    a tr
-00000260: 6163 6520 6361 6e20 6265 2061 6464 6564  ace can be added
-00000270: 2067 6976 656e 2061 2050 796f 6d6f 2076   given a Pyomo v
-00000280: 6172 6961 626c 652e 0a20 2020 20e9 0400  ariable..    ...
-00000290: 0000 4e63 0500 0000 0000 0000 0000 0000  ..Nc............
-000002a0: 0c00 0000 0700 0000 0b00 0000 7314 0100  ............s...
-000002b0: 007c 0364 0075 0072 0764 0167 017d 037c  .|.d.u.r.d.g.}.|
-000002c0: 017c 005f 007c 016a 017c 005f 017c 01a0  .|._.|.j.|._.|..
-000002d0: 0274 03a0 047c 016a 05a1 01a1 017c 005f  .t...|.j.....|._
-000002e0: 067c 016a 057c 005f 0574 077c 016a 0183  .|.j.|._.t.|.j..
-000002f0: 0189 0087 0066 0164 0264 0384 0874 087c  .....f.d.d...t.|
-00000300: 0283 0144 0083 017d 067c 0344 005d 137d  ...D...}.|.D.].}
-00000310: 0788 0064 0464 059c 0267 0164 0067 0188  ...d.d...g.d.g..
-00000320: 0064 0618 0014 0017 007c 067c 0764 0618  .d.......|.|.d..
-00000330: 003c 0071 2e74 097c 0288 0066 0264 0464  .<.q.t.|...f.d.d
-00000340: 077c 067c 0464 0075 0172 4f7c 046e 0474  .|.|.d.u.rO|.n.t
-00000350: 0a7c 016a 0183 0164 089c 047c 05a4 018e  .|.j...d...|....
-00000360: 017c 005f 0b74 087c 0283 0144 005d 267d  .|._.t.|...D.]&}
-00000370: 0874 0c7c 006a 0b6a 0d7c 0864 0617 0064  .t.|.j.j.|.d...d
-00000380: 0664 0464 098d 0383 017d 097c 096a 0ea0  .d.d.....}.|.j..
-00000390: 0f64 0a64 0ba1 027d 0a7c 006a 0b6a 0d7c  .d.d...}.|.j.j.|
-000003a0: 0864 0617 0064 0464 0c8d 0244 005d 057d  .d...d.d...D.].}
-000003b0: 0b7c 0a7c 0b5f 1071 7e71 5e69 007c 005f  .|.|._.q~q^i.|._
-000003c0: 1164 0053 0029 0d4e 7206 0000 0063 0100  .d.S.).Nr....c..
-000003d0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000003e0: 0000 1300 0000 731a 0000 0067 007c 005d  ......s....g.|.]
-000003f0: 097d 0164 0064 0169 0167 0188 0014 0091  .}.d.d.i.g......
-00000400: 0271 0253 0029 02da 0b73 6563 6f6e 6461  .q.S.)...seconda
-00000410: 7279 5f79 54a9 0029 02da 022e 30da 015f  ry_yT..)....0.._
-00000420: a901 da01 6e72 0800 0000 fa58 633a 5c75  ....nr.....Xc:\u
-00000430: 7365 7273 5c33 3930 3338 3835 5c6f 6e65  sers\3903885\one
-00000440: 6472 6976 6520 2d20 756e 6976 6572 7369  drive - universi
-00000450: 7465 6974 2075 7472 6563 6874 5c64 6f63  teit utrecht\doc
-00000460: 756d 656e 7473 5c6d 696d 6f73 615c 6d69  uments\mimosa\mi
-00000470: 6d6f 7361 5c65 7870 6f72 745c 7574 696c  mosa\export\util
-00000480: 732e 7079 da0a 3c6c 6973 7463 6f6d 703e  s.py..<listcomp>
-00000490: 2f00 0000 7302 0000 001a 007a 2150 6c6f  /...s......z!Plo
-000004a0: 742e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  t.__init__.<loca
-000004b0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 5429  ls>.<listcomp>T)
-000004c0: 02da 0763 6f6c 7370 616e 7207 0000 00e9  ...colspanr.....
-000004d0: 0100 0000 da04 726f 7773 2904 5a0c 7368  ......rows).Z.sh
-000004e0: 6172 6564 5f79 6178 6573 5a0c 7368 6172  ared_yaxesZ.shar
-000004f0: 6564 5f78 6178 6573 da05 7370 6563 735a  ed_xaxes..specsZ
-00000500: 0e73 7562 706c 6f74 5f74 6974 6c65 7329  .subplot_titles)
-00000510: 03da 0372 6f77 da03 636f 6c72 0700 0000  ...row..colr....
-00000520: da04 6178 6973 da00 2902 7213 0000 0072  ..axis..).r....r
-00000530: 0700 0000 2912 da01 6dda 0772 6567 696f  ....)...m..regio
-00000540: 6e73 da04 7965 6172 da02 6e70 da05 6172  ns..year..np..ar
-00000550: 7261 79da 0174 da05 7965 6172 73da 036c  ray..t..years..l
-00000560: 656e da05 7261 6e67 6572 0200 0000 da04  en..ranger......
-00000570: 6c69 7374 da03 6669 67da 046e 6578 745a  list..fig..nextZ
-00000580: 0c73 656c 6563 745f 7961 7865 735a 0b70  .select_yaxesZ.p
-00000590: 6c6f 746c 795f 6e61 6d65 da07 7265 706c  lotly_name..repl
-000005a0: 6163 65da 076d 6174 6368 6573 da0b 6375  ace..matches..cu
-000005b0: 7272 5f76 616c 7565 7329 0cda 0473 656c  rr_values)...sel
-000005c0: 6672 1700 0000 5a07 6e75 6d72 6f77 735a  fr....Z.numrowsZ
-000005d0: 0a67 6c6f 6261 6c72 6f77 735a 0963 6f6c  .globalrowsZ.col
-000005e0: 7469 746c 6573 da06 6b77 6172 6773 7212  titles..kwargsr.
-000005f0: 0000 0072 1300 0000 da01 69da 0372 6566  ...r......i..ref
-00000600: 5a08 7265 665f 6e61 6d65 7215 0000 0072  Z.ref_namer....r
-00000610: 0800 0000 720b 0000 0072 0d00 0000 da08  ....r....r......
-00000620: 5f5f 696e 6974 5f5f 2600 0000 7338 0000  __init__&...s8..
-00000630: 0008 0106 0106 0108 0114 0108 010a 0216  ................
-00000640: 0108 0124 0102 0202 0102 0102 fe02 0302  ...$............
-00000650: 0102 0114 0104 fa02 0708 f90c 0b1a 010e  ................
-00000660: 0118 0108 0102 ff0a 037a 0d50 6c6f 742e  .........z.Plot.
-00000670: 5f5f 696e 6974 5f5f 6304 0000 0000 0000  __init__c.......
-00000680: 0000 0000 0004 0000 0003 0000 0003 0000  ................
-00000690: 0073 3000 0000 7c03 720d 8700 8701 6602  .s0...|.r.....f.
-000006a0: 6401 6402 8408 7c00 6a00 4400 8301 5300  d.d...|.j.D...S.
-000006b0: 8700 8701 6602 6403 6402 8408 7c00 6a01  ....f.d.d...|.j.
-000006c0: 4400 8301 5300 2904 4e63 0100 0000 0000  D...S.).Nc......
-000006d0: 0000 0000 0000 0200 0000 0500 0000 1300  ................
-000006e0: 0000 7316 0000 0067 007c 005d 077d 0188  ..s....g.|.].}..
-000006f0: 017c 0188 0083 0291 0271 0253 0072 0800  .|.......q.S.r..
-00000700: 0000 7208 0000 00a9 0272 0900 0000 721c  ..r......r....r.
-00000710: 0000 00a9 02da 0672 6567 696f 6eda 0376  .......region..v
-00000720: 6172 7208 0000 0072 0d00 0000 720e 0000  arr....r....r...
-00000730: 0048 0000 0073 0200 0000 1600 7a1f 506c  .H...s......z.Pl
-00000740: 6f74 2e5f 7661 6c75 652e 3c6c 6f63 616c  ot._value.<local
-00000750: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
-00000760: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00000770: 0000 1300 0000 731c 0000 0067 007c 005d  ......s....g.|.]
-00000780: 0a7d 0174 0088 017c 0188 0066 0219 0083  .}.t...|...f....
-00000790: 0191 0271 0253 0072 0800 0000 7203 0000  ...q.S.r....r...
-000007a0: 0072 2b00 0000 722c 0000 0072 0800 0000  .r+...r,...r....
-000007b0: 720d 0000 0072 0e00 0000 4a00 0000 7302  r....r....J...s.
-000007c0: 0000 001c 0029 0272 1d00 0000 721c 0000  .....).r....r...
-000007d0: 0029 0472 2600 0000 722e 0000 0072 2d00  .).r&...r....r-.
-000007e0: 0000 da06 6973 5f66 6374 7208 0000 0072  ....is_fctr....r
-000007f0: 2c00 0000 720d 0000 00da 065f 7661 6c75  ,...r......_valu
-00000800: 6546 0000 0073 0600 0000 0401 1601 1602  eF...s..........
-00000810: 7a0b 506c 6f74 2e5f 7661 6c75 6563 0300  z.Plot._valuec..
-00000820: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00000830: 0000 0300 0000 732c 0000 007c 0272 0c87  ......s,...|.r..
-00000840: 0066 0164 0164 0284 087c 006a 0044 0083  .f.d.d...|.j.D..
-00000850: 0153 0087 0066 0164 0364 0284 087c 006a  .S...f.d.d...|.j
-00000860: 0044 0083 0153 0029 044e 6301 0000 0000  .D...S.).Nc.....
-00000870: 0000 0000 0000 0002 0000 0004 0000 0013  ................
-00000880: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
-00000890: 8800 7c01 8301 9102 7102 5300 7208 0000  ..|.....q.S.r...
-000008a0: 0072 0800 0000 722b 0000 00a9 0172 2e00  .r....r+.....r..
-000008b0: 0000 7208 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-000008c0: 004e 0000 0073 0200 0000 1400 7a26 506c  .N...s......z&Pl
-000008d0: 6f74 2e5f 7661 6c75 655f 676c 6f62 616c  ot._value_global
-000008e0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000008f0: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
-00000900: 0002 0000 0005 0000 0013 0000 0073 1800  .............s..
-00000910: 0000 6700 7c00 5d08 7d01 7400 8800 7c01  ..g.|.].}.t...|.
-00000920: 1900 8301 9102 7102 5300 7208 0000 0072  ......q.S.r....r
-00000930: 0300 0000 722b 0000 0072 3100 0000 7208  ....r+...r1...r.
-00000940: 0000 0072 0d00 0000 720e 0000 0050 0000  ...r....r....P..
-00000950: 0073 0200 0000 1800 2901 721c 0000 0029  .s......).r....)
-00000960: 0372 2600 0000 722e 0000 0072 2f00 0000  .r&...r....r/...
-00000970: 7208 0000 0072 3100 0000 720d 0000 00da  r....r1...r.....
-00000980: 0d5f 7661 6c75 655f 676c 6f62 616c 4c00  ._value_globalL.
-00000990: 0000 7306 0000 0004 0114 0114 027a 1250  ..s..........z.P
-000009a0: 6c6f 742e 5f76 616c 7565 5f67 6c6f 6261  lot._value_globa
-000009b0: 6c63 0700 0000 0000 0000 0000 0000 0800  lc..............
-000009c0: 0000 0b00 0000 4b00 0000 734e 0000 007c  ......K...sN...|
-000009d0: 006a 006a 0164 077c 006a 027c 017c 027c  .j.j.d.|.j.|.|.|
-000009e0: 027c 037c 047c 057c 0664 019c 0864 027c  .|.|.|.|.d...d.|
-000009f0: 0776 0172 1f64 027c 07a0 0364 0364 04a1  .v.r.d.|...d.d..
-00000a00: 0272 1c64 056e 0164 0669 016e 0169 00a4  .r.d.n.d.i.n.i..
-00000a10: 017c 07a4 018e 0101 0064 0053 0029 084e  .|.......d.S.).N
-00000a20: 2908 da01 78da 0179 da04 6e61 6d65 5a0b  )...x..y..nameZ.
-00000a30: 6c65 6765 6e64 6772 6f75 705a 0a6c 696e  legendgroupZ.lin
-00000a40: 655f 636f 6c6f 7272 1300 0000 7214 0000  e_colorr....r...
-00000a50: 00da 0a73 686f 776c 6567 656e 645a 096c  ...showlegendZ.l
-00000a60: 696e 655f 6461 7368 7207 0000 0046 da03  ine_dashr....F..
-00000a70: 646f 74da 0573 6f6c 6964 7208 0000 0029  dot..solidr....)
-00000a80: 0472 2100 0000 da0b 6164 645f 7363 6174  .r!.....add_scat
-00000a90: 7465 7272 1d00 0000 da03 6765 7429 0872  terr......get).r
-00000aa0: 2600 0000 da06 7661 6c75 6573 7235 0000  &.....valuesr5..
-00000ab0: 00da 0563 6f6c 6f72 7213 0000 0072 1400  ...colorr....r..
-00000ac0: 0000 7236 0000 0072 2700 0000 7208 0000  ..r6...r'...r...
-00000ad0: 0072 0800 0000 720d 0000 0072 3900 0000  .r....r....r9...
-00000ae0: 5200 0000 7320 0000 0008 0104 0102 0102  R...s ..........
-00000af0: 0102 0102 0102 0102 0102 0104 f808 0b18  ................
-00000b00: ff02 0202 f402 0e0a f27a 1050 6c6f 742e  .........z.Plot.
-00000b10: 6164 645f 7363 6174 7465 7254 4672 1000  add_scatterTFr..
-00000b20: 0000 6306 0000 0000 0000 0000 0000 000b  ..c.............
-00000b30: 0000 0007 0000 004b 0000 0073 c000 0000  .......K...s....
-00000b40: 7c03 7309 7c04 6400 7500 7209 7c01 6a00  |.s.|.d.u.r.|.j.
-00000b50: 7d04 7c04 7c00 6a01 7601 7d07 7c07 7218  }.|.|.j.v.}.|.r.
-00000b60: 7402 7c00 6a01 8301 7c00 6a01 7c04 3c00  t.|.j...|.j.|.<.
-00000b70: 7403 7c00 6a01 7c04 1900 7402 7403 8301  t.|.j.|...t.t...
-00000b80: 1600 1900 7d08 7c02 724b 7404 7c00 6a05  ....}.|.rKt.|.j.
-00000b90: 8301 4400 5d1e 5c02 7d09 7d0a 7c00 6a06  ..D.].\.}.}.|.j.
-00000ba0: 7c00 a007 7c01 7c0a 7c03 a103 7c04 7c08  |...|.|.|...|.|.
-00000bb0: 7c05 6604 7c09 6401 1700 7c07 6f42 7c09  |.f.|.d...|.oB|.
-00000bc0: 6402 6b02 6403 9c02 7c06 a401 8e01 0100  d.k.d...|.......
-00000bd0: 712a 6400 5300 7c00 6a06 7c00 a008 7c01  q*d.S.|.j.|...|.
-00000be0: 7c03 a102 7c04 7c08 7c05 6604 6401 7c07  |...|.|.|.f.d.|.
-00000bf0: 6403 9c02 7c06 a401 8e01 0100 6400 5300  d...|.......d.S.
-00000c00: 2904 4e72 1000 0000 7201 0000 0029 0272  ).Nr....r....).r
-00000c10: 1400 0000 7236 0000 0029 0972 3500 0000  ....r6...).r5...
-00000c20: 7225 0000 0072 1e00 0000 da0a 434f 4c4f  r%...r......COLO
-00000c30: 5253 5f50 424c da09 656e 756d 6572 6174  RS_PBL..enumerat
-00000c40: 6572 1800 0000 7239 0000 0072 3000 0000  er....r9...r0...
-00000c50: 7232 0000 0029 0b72 2600 0000 722e 0000  r2...).r&...r...
-00000c60: 00da 0b69 735f 7265 6769 6f6e 616c 722f  ...is_regionalr/
-00000c70: 0000 0072 3500 0000 7213 0000 0072 2700  ...r5...r....r'.
-00000c80: 0000 da03 6e65 7772 3c00 0000 7228 0000  ....newr<...r(..
-00000c90: 00da 0172 7208 0000 0072 0800 0000 720d  ...rr....r....r.
-00000ca0: 0000 00da 0361 6464 6400 0000 733e 0000  .....addd...s>..
-00000cb0: 000c 0206 010a 0104 0210 0116 0104 0212  ................
-00000cc0: 0104 010c 0102 0102 0102 0102 fc06 050a  ................
-00000cd0: 0104 fa02 0708 f904 ff04 0b0a 0102 0102  ................
-00000ce0: 0102 0102 fc02 0502 0104 fa02 070a f97a  ...............z
-00000cf0: 0850 6c6f 742e 6164 6463 0100 0000 0000  .Plot.addc......
-00000d00: 0000 0000 0000 0200 0000 0600 0000 4300  ..............C.
-00000d10: 0000 7372 0000 007c 006a 006a 017c 006a  ..sr...|.j.j.|.j
-00000d20: 0264 0119 0064 0267 0264 038d 0101 0074  .d...d.g.d.....t
-00000d30: 0364 0474 047c 006a 0583 0183 0244 005d  .d.t.|.j.....D.]
-00000d40: 0b7d 017c 006a 006a 0664 0564 067c 0164  .}.|.j.j.d.d.|.d
-00000d50: 078d 0301 0071 147c 006a 006a 0764 0864  .....q.|.j.j.d.d
-00000d60: 098d 0101 007c 006a 006a 0864 0a64 0a64  .....|.j.j.d.d.d
-00000d70: 0a64 0a64 0b9c 0464 0c64 0d64 0e9c 0264  .d.d...d.d.d...d
-00000d80: 0f8d 0201 0064 0053 0029 104e 7201 0000  .....d.S.).Nr...
-00000d90: 0069 3408 0000 2901 721f 0000 0072 1000  .i4...).r....r..
-00000da0: 0000 5446 2903 7207 0000 005a 0e73 686f  ..TF).r....Z.sho
-00000db0: 7774 6963 6b6c 6162 656c 7372 1400 0000  wticklabelsr....
-00000dc0: da05 6c69 6e65 7329 01da 046d 6f64 65e9  ..lines)...mode.
-00000dd0: 3200 0000 2904 721c 0000 00da 016c 7241  2...).r......lrA
-00000de0: 0000 00da 0162 da06 6d69 6464 6c65 6700  .....b..middleg.
-00000df0: 0000 0000 00e0 3f29 025a 0779 616e 6368  ......?).Z.yanch
-00000e00: 6f72 7234 0000 0029 02da 066d 6172 6769  orr4...)...margi
-00000e10: 6eda 066c 6567 656e 6429 0972 2100 0000  n..legend).r!...
-00000e20: 5a0c 7570 6461 7465 5f78 6178 6573 721d  Z.update_xaxesr.
-00000e30: 0000 0072 1f00 0000 721e 0000 0072 1800  ...r....r....r..
-00000e40: 0000 da0c 7570 6461 7465 5f79 6178 6573  ....update_yaxes
-00000e50: 5a0d 7570 6461 7465 5f74 7261 6365 73da  Z.update_traces.
-00000e60: 0d75 7064 6174 655f 6c61 796f 7574 2902  .update_layout).
-00000e70: 7226 0000 0072 2800 0000 7208 0000 0072  r&...r(...r....r
-00000e80: 0800 0000 720d 0000 00da 0a73 6574 5f6c  ....r......set_l
-00000e90: 6179 6f75 7484 0000 0073 1000 0000 1801  ayout....s......
-00000ea0: 1401 1401 0e01 0601 0c01 0801 0afe 7a0f  ..............z.
-00000eb0: 506c 6f74 2e73 6574 5f6c 6179 6f75 7463  Plot.set_layoutc
-00000ec0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000ed0: 0700 0000 4300 0000 732e 0000 0074 007c  ....C...s....t.|
-00000ee0: 0183 0144 005d 105c 027d 027d 037c 006a  ...D.].\.}.}.|.j
-00000ef0: 016a 027c 037c 0264 0117 0064 0164 0264  .j.|.|.d...d.d.d
-00000f00: 038d 0401 0071 0464 0053 0029 044e 7210  .....q.d.S.).Nr.
-00000f10: 0000 0046 2904 da05 7469 746c 6572 1300  ...F)...titler..
-00000f20: 0000 7214 0000 0072 0700 0000 2903 723e  ..r....r....).r>
-00000f30: 0000 0072 2100 0000 724b 0000 0029 0472  ...r!...rK...).r
-00000f40: 2600 0000 da06 7469 746c 6573 7228 0000  &.....titlesr(..
-00000f50: 0072 4e00 0000 7208 0000 0072 0800 0000  .rN...r....r....
-00000f60: 720d 0000 00da 1073 6574 5f79 6178 6573  r......set_yaxes
-00000f70: 5f74 6974 6c65 738e 0000 0073 0600 0000  _titles....s....
-00000f80: 1001 1a01 04ff 7a15 506c 6f74 2e73 6574  ......z.Plot.set
-00000f90: 5f79 6178 6573 5f74 6974 6c65 7363 0100  _yaxes_titlesc..
-00000fa0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000fb0: 0000 4300 0000 730e 0000 007c 00a0 00a1  ..C...s....|....
-00000fc0: 0001 007c 006a 0153 0029 014e 2902 724d  ...|.j.S.).N).rM
-00000fd0: 0000 0072 2100 0000 2901 7226 0000 0072  ...r!...).r&...r
-00000fe0: 0800 0000 7208 0000 0072 0d00 0000 da04  ....r....r......
-00000ff0: 7368 6f77 9200 0000 7304 0000 0008 0106  show....s.......
-00001000: 017a 0950 6c6f 742e 7368 6f77 2903 7206  .z.Plot.show).r.
-00001010: 0000 004e 4e29 0454 464e 7210 0000 0029  ...NN).TFNr....)
-00001020: 0cda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00001030: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001040: 616d 655f 5fda 075f 5f64 6f63 5f5f 722a  ame__..__doc__r*
-00001050: 0000 0072 3000 0000 7232 0000 0072 3900  ...r0...r2...r9.
-00001060: 0000 7242 0000 0072 4d00 0000 7250 0000  ..rB...rM...rP..
-00001070: 0072 5100 0000 7208 0000 0072 0800 0000  .rQ...r....r....
-00001080: 7208 0000 0072 0d00 0000 7205 0000 001e  r....r....r.....
-00001090: 0000 0073 1400 0000 0800 0401 0a07 0820  ...s........... 
-000010a0: 0806 0806 0a12 0820 080a 0c04 7205 0000  ....... ....r...
-000010b0: 0063 0100 0000 0000 0000 0000 0000 0900  .c..............
-000010c0: 0000 0700 0000 4300 0000 7318 0100 0074  ......C...s....t
-000010d0: 007c 0064 0183 027d 0164 027d 0267 007d  .|.d...}.d.}.g.}
-000010e0: 037c 0144 005d 437d 047c 04a0 0164 03a1  .|.D.]C}.|...d..
-000010f0: 0172 1464 047d 027c 04a0 02a1 0064 056b  .r.d.}.|.....d.k
-00001100: 0272 1c64 027d 027c 0272 4e7c 04a0 0164  .r.d.}.|.rN|...d
-00001110: 06a1 0172 4e7c 04a0 02a1 00a0 0364 06a1  ...rN|.......d..
-00001120: 0164 0064 0785 0219 007d 0564 017c 0564  .d.d.....}.d.|.d
-00001130: 0819 0076 0072 4464 047d 067c 0564 0819  ...v.rDd.}.|.d..
-00001140: 00a0 0364 01a1 017c 0564 0964 0a85 0219  ...d...|.d.d....
-00001150: 0017 007d 056e 0264 027d 067c 03a0 047c  ...}.n.d.}.|...|
-00001160: 057c 0667 0117 00a1 0101 0071 0b74 056a  .|.g.......q.t.j
-00001170: 067c 0367 0064 0ba2 0164 0c8d 027d 077c  .|.g.d...d...}.|
-00001180: 07a0 0774 0874 0974 0974 0964 0d9c 04a1  ...t.t.t.t.d....
-00001190: 017d 077c 01a0 0aa1 0001 0074 0b6a 0c7c  .}.|.......t.j.|
-000011a0: 0764 0e67 0064 0fa2 0164 1064 1164 128d  .d.g.d...d.d.d..
-000011b0: 056a 0d64 0064 1364 148d 026a 0d64 1564  .j.d.d.d...j.d.d
-000011c0: 1664 178d 027d 087c 086a 0e7c 00a0 0364  .d...}.|.j.|...d
-000011d0: 18a1 0164 0819 0064 1917 0064 1a64 1b8d  ...d...d...d.d..
-000011e0: 0201 0064 0053 0029 1c4e 7241 0000 0046  ...d.S.).NrA...F
-000011f0: 7a05 6974 6572 2054 7216 0000 00fa 0120  z.iter Tr...... 
-00001200: 7206 0000 0072 0100 0000 7210 0000 00e9  r....r....r.....
-00001210: ffff ffff 2905 da04 6974 6572 da09 6f62  ....)...iter..ob
-00001220: 6a65 6374 6976 65da 0669 6e66 5f70 72da  jective..inf_pr.
-00001230: 0669 6e66 5f64 75da 0972 6563 6f76 6572  .inf_du..recover
-00001240: 6564 2901 da07 636f 6c75 6d6e 7329 0472  ed)...columns).r
-00001250: 5800 0000 7259 0000 0072 5a00 0000 725b  X...rY...rZ...r[
-00001260: 0000 0072 5800 0000 2903 7259 0000 0072  ...rX...).rY...r
-00001270: 5a00 0000 725b 0000 00da 0876 6172 6961  Z...r[.....varia
-00001280: 626c 6572 5c00 0000 2904 7233 0000 0072  bler\...).r3...r
-00001290: 3400 0000 5a09 6661 6365 745f 726f 7772  4...Z.facet_rowr
-000012a0: 3c00 0000 da03 6c6f 6729 0272 2400 0000  <.....log).r$...
-000012b0: da04 7479 7065 e903 0000 00da 066c 696e  ..type.......lin
-000012c0: 6561 7229 0272 1300 0000 7260 0000 00da  ear).r....r`....
-000012d0: 012e 7a05 2e68 746d 6c5a 0363 646e 2901  ..z..htmlZ.cdn).
-000012e0: da10 696e 636c 7564 655f 706c 6f74 6c79  ..include_plotly
-000012f0: 6a73 290f da04 6f70 656e da0a 7374 6172  js)...open..star
-00001300: 7473 7769 7468 da05 7374 7269 70da 0573  tswith..strip..s
-00001310: 706c 6974 da06 6170 7065 6e64 da02 7064  plit..append..pd
-00001320: da09 4461 7461 4672 616d 65da 0661 7374  ..DataFrame..ast
-00001330: 7970 65da 0369 6e74 da05 666c 6f61 74da  ype..int..float.
-00001340: 0563 6c6f 7365 da02 7078 da07 7363 6174  .close..px..scat
-00001350: 7465 7272 4b00 0000 da0a 7772 6974 655f  terrK.....write_
-00001360: 6874 6d6c 2909 da0b 6f75 7470 7574 5f66  html)...output_f
-00001370: 696c 65da 0466 696c 655a 0d69 6e5f 6974  ile..fileZ.in_it
-00001380: 6572 6174 696f 6e73 da0a 6974 6572 6174  erations..iterat
-00001390: 696f 6e73 da04 6c69 6e65 7268 0000 0072  ions..linerh...r
-000013a0: 5c00 0000 5a0d 6974 6572 6174 696f 6e73  \...Z.iterations
-000013b0: 5f64 6672 2100 0000 7208 0000 0072 0800  _dfr!...r....r..
-000013c0: 0000 720d 0000 00da 1676 6973 7561 6c69  ..r......visuali
-000013d0: 7365 5f69 706f 7074 5f6f 7574 7075 7497  se_ipopt_output.
-000013e0: 0000 0073 4800 0000 0a01 0401 0402 0802  ...sH...........
-000013f0: 0a01 0401 0c01 0401 0e02 1601 0c03 0401  ................
-00001400: 1c01 0402 1001 0280 0402 0801 06ff 0403  ................
-00001410: 0c01 04ff 0804 0403 0201 0201 0601 0201  ................
-00001420: 0201 04fb 0607 04f9 0608 04f8 02ff 200c  .............. .
-00001430: 7277 0000 0029 0f72 5500 0000 da05 6e75  rw...).rU.....nu
-00001440: 6d70 7972 1a00 0000 da06 7061 6e64 6173  mpyr......pandas
-00001450: 726a 0000 005a 0e70 6c6f 746c 792e 6578  rj...Z.plotly.ex
-00001460: 7072 6573 735a 0765 7870 7265 7373 7270  pressZ.expressrp
-00001470: 0000 005a 0f70 6c6f 746c 792e 7375 6270  ...Z.plotly.subp
-00001480: 6c6f 7473 7202 0000 00da 0d70 796f 6d6f  lotsr......pyomo
-00001490: 2e65 6e76 6972 6f6e 7204 0000 0072 3d00  .environr....r=.
-000014a0: 0000 7205 0000 0072 7700 0000 7208 0000  ..r....rw...r...
-000014b0: 0072 0800 0000 7208 0000 0072 0d00 0000  .r....r....r....
-000014c0: da08 3c6d 6f64 756c 653e 0100 0000 7312  ..<module>....s.
-000014d0: 0000 0004 0008 0308 010c 010c 010c 0108  ................
-000014e0: 020e 140c 79                             ....y
+00000040: 5a04 6401 6403 6c05 6d06 5a06 0100 7a0e  Z.d.d.l.m.Z...z.
+00000050: 6401 6402 6c07 6d08 5a09 0100 6401 6404  d.d.l.m.Z...d.d.
+00000060: 6c0a 6d0b 5a0b 0100 5700 6e09 0400 650c  l.m.Z...W.n...e.
+00000070: 7927 0100 0100 0100 5900 6e01 7700 6700  y'......Y.n.w.g.
+00000080: 6405 a201 5a0d 4700 6406 6407 8400 6407  d...Z.G.d.d...d.
+00000090: 8302 5a0e 6408 6409 8400 5a0f 6402 5300  ..Z.d.d...Z.d.S.
+000000a0: 290a 7a35 0a50 6c6f 7420 6675 6e63 7469  ).z5.Plot functi
+000000b0: 6f6e 732e 204e 6f74 206e 6563 6573 7361  ons. Not necessa
+000000c0: 7279 2069 6620 6461 7368 626f 6172 6420  ry if dashboard 
+000000d0: 6973 2075 7365 642e 0ae9 0000 0000 4ea9  is used.......N.
+000000e0: 01da 0576 616c 7565 2901 da0d 6d61 6b65  ...value)...make
+000000f0: 5f73 7562 706c 6f74 7329 107a 0723 3030  _subplots).z.#00
+00000100: 4145 4546 7a07 2338 3038 4431 447a 0723  AEEFz.#808D1Dz.#
+00000110: 4236 3033 3643 7a07 2346 4141 4431 457a  B6036Cz.#FAAD1Ez
+00000120: 0723 3346 3134 3634 7a07 2337 4343 4646  .#3F1464z.#7CCFF
+00000130: 327a 0723 4631 3938 4331 7a07 2334 3242  2z.#F198C1z.#42B
+00000140: 3634 397a 0723 4545 3241 3233 7a07 2330  649z.#EE2A23z.#0
+00000150: 3034 3031 397a 0723 4634 3733 3231 7a07  04019z.#F47321z.
+00000160: 2335 3131 3630 377a 0723 4241 3839 3132  #511607z.#BA8912
+00000170: 7a07 2337 3843 4242 467a 0723 4646 4632  z.#78CBBFz.#FFF2
+00000180: 3239 7a07 2330 3037 3142 4263 0000 0000  29z.#0071BBc....
+00000190: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+000001a0: 4000 0000 7354 0000 0065 005a 0164 005a  @...sT...e.Z.d.Z
+000001b0: 0264 015a 0364 1764 0464 0584 015a 0464  .d.Z.d.d.d...Z.d
+000001c0: 0664 0784 005a 0564 0864 0984 005a 0664  .d...Z.d.d...Z.d
+000001d0: 0a64 0b84 005a 0764 1864 0f64 1084 015a  .d...Z.d.d.d...Z
+000001e0: 0864 1164 1284 005a 0964 1364 1484 005a  .d.d...Z.d.d...Z
+000001f0: 0a64 1564 1684 005a 0b64 0353 0029 19da  .d.d...Z.d.S.)..
+00000200: 0450 6c6f 747a 9e0a 2020 2020 5772 6170  .Plotz..    Wrap
+00000210: 7065 7220 666f 7220 6120 506c 6f74 6c79  per for a Plotly
+00000220: 2066 6967 7572 652e 0a0a 2020 2020 4669   figure...    Fi
+00000230: 7273 7420 6974 2063 7265 6174 6573 2061  rst it creates a
+00000240: 2073 7562 706c 6f74 2066 6967 7572 652c   subplot figure,
+00000250: 2074 6865 6e20 7573 696e 6720 7468 6520   then using the 
+00000260: 6675 6e63 7469 6f6e 2060 6164 6460 2c0a  function `add`,.
+00000270: 2020 2020 6120 7472 6163 6520 6361 6e20      a trace can 
+00000280: 6265 2061 6464 6564 2067 6976 656e 2061  be added given a
+00000290: 2050 796f 6d6f 2076 6172 6961 626c 652e   Pyomo variable.
+000002a0: 0a20 2020 20e9 0400 0000 4e63 0500 0000  .    .....Nc....
+000002b0: 0000 0000 0000 0000 0c00 0000 0700 0000  ................
+000002c0: 0b00 0000 7314 0100 007c 0364 0075 0072  ....s....|.d.u.r
+000002d0: 0764 0167 017d 037c 017c 005f 007c 016a  .d.g.}.|.|._.|.j
+000002e0: 017c 005f 017c 01a0 0274 03a0 047c 016a  .|._.|...t...|.j
+000002f0: 05a1 01a1 017c 005f 067c 016a 057c 005f  .....|._.|.j.|._
+00000300: 0574 077c 016a 0183 0189 0087 0066 0164  .t.|.j.......f.d
+00000310: 0264 0384 0874 087c 0283 0144 0083 017d  .d...t.|...D...}
+00000320: 067c 0344 005d 137d 0788 0064 0464 059c  .|.D.].}...d.d..
+00000330: 0267 0164 0067 0188 0064 0618 0014 0017  .g.d.g...d......
+00000340: 007c 067c 0764 0618 003c 0071 2e74 097c  .|.|.d...<.q.t.|
+00000350: 0288 0066 0264 0464 077c 067c 0464 0075  ...f.d.d.|.|.d.u
+00000360: 0172 4f7c 046e 0474 0a7c 016a 0183 0164  .rO|.n.t.|.j...d
+00000370: 089c 047c 05a4 018e 017c 005f 0b74 087c  ...|.....|._.t.|
+00000380: 0283 0144 005d 267d 0874 0c7c 006a 0b6a  ...D.]&}.t.|.j.j
+00000390: 0d7c 0864 0617 0064 0664 0464 098d 0383  .|.d...d.d.d....
+000003a0: 017d 097c 096a 0ea0 0f64 0a64 0ba1 027d  .}.|.j...d.d...}
+000003b0: 0a7c 006a 0b6a 0d7c 0864 0617 0064 0464  .|.j.j.|.d...d.d
+000003c0: 0c8d 0244 005d 057d 0b7c 0a7c 0b5f 1071  ...D.].}.|.|._.q
+000003d0: 7e71 5e69 007c 005f 1164 0053 0029 0d4e  ~q^i.|._.d.S.).N
+000003e0: 7206 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000003f0: 0000 0200 0000 0400 0000 1300 0000 731a  ..............s.
+00000400: 0000 0067 007c 005d 097d 0164 0064 0169  ...g.|.].}.d.d.i
+00000410: 0167 0188 0014 0091 0271 0253 0029 02da  .g.......q.S.)..
+00000420: 0b73 6563 6f6e 6461 7279 5f79 54a9 0029  .secondary_yT..)
+00000430: 02da 022e 30da 015f a901 da01 6e72 0800  ....0.._....nr..
+00000440: 0000 fa58 633a 5c55 7365 7273 5c33 3930  ...Xc:\Users\390
+00000450: 3338 3835 5c4f 6e65 4472 6976 6520 2d20  3885\OneDrive - 
+00000460: 556e 6976 6572 7369 7465 6974 2055 7472  Universiteit Utr
+00000470: 6563 6874 5c44 6f63 756d 656e 7473 5c4d  echt\Documents\M
+00000480: 494d 4f53 415c 6d69 6d6f 7361 5c65 7870  IMOSA\mimosa\exp
+00000490: 6f72 745c 7574 696c 732e 7079 da0a 3c6c  ort\utils.py..<l
+000004a0: 6973 7463 6f6d 703e 3300 0000 7302 0000  istcomp>3...s...
+000004b0: 001a 007a 2150 6c6f 742e 5f5f 696e 6974  ...z!Plot.__init
+000004c0: 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  __.<locals>.<lis
+000004d0: 7463 6f6d 703e 5429 02da 0763 6f6c 7370  tcomp>T)...colsp
+000004e0: 616e 7207 0000 00e9 0100 0000 da04 726f  anr...........ro
+000004f0: 7773 2904 5a0c 7368 6172 6564 5f79 6178  ws).Z.shared_yax
+00000500: 6573 5a0c 7368 6172 6564 5f78 6178 6573  esZ.shared_xaxes
+00000510: da05 7370 6563 735a 0e73 7562 706c 6f74  ..specsZ.subplot
+00000520: 5f74 6974 6c65 7329 03da 0372 6f77 da03  _titles)...row..
+00000530: 636f 6c72 0700 0000 da04 6178 6973 da00  colr......axis..
+00000540: 2902 7213 0000 0072 0700 0000 2912 da01  ).r....r....)...
+00000550: 6dda 0772 6567 696f 6e73 da04 7965 6172  m..regions..year
+00000560: da02 6e70 da05 6172 7261 79da 0174 da05  ..np..array..t..
+00000570: 7965 6172 73da 036c 656e da05 7261 6e67  years..len..rang
+00000580: 6572 0400 0000 da04 6c69 7374 da03 6669  er......list..fi
+00000590: 67da 046e 6578 745a 0c73 656c 6563 745f  g..nextZ.select_
+000005a0: 7961 7865 735a 0b70 6c6f 746c 795f 6e61  yaxesZ.plotly_na
+000005b0: 6d65 da07 7265 706c 6163 65da 076d 6174  me..replace..mat
+000005c0: 6368 6573 da0b 6375 7272 5f76 616c 7565  ches..curr_value
+000005d0: 7329 0cda 0473 656c 6672 1700 0000 5a07  s)...selfr....Z.
+000005e0: 6e75 6d72 6f77 735a 0a67 6c6f 6261 6c72  numrowsZ.globalr
+000005f0: 6f77 735a 0963 6f6c 7469 746c 6573 da06  owsZ.coltitles..
+00000600: 6b77 6172 6773 7212 0000 0072 1300 0000  kwargsr....r....
+00000610: da01 69da 0372 6566 5a08 7265 665f 6e61  ..i..refZ.ref_na
+00000620: 6d65 7215 0000 0072 0800 0000 720b 0000  mer....r....r...
+00000630: 0072 0d00 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
+00000640: 2a00 0000 7338 0000 0008 0106 0106 0108  *...s8..........
+00000650: 0114 0108 010a 0216 0108 0124 0102 0202  ...........$....
+00000660: 0102 0102 fe02 0302 0102 0114 0104 fa02  ................
+00000670: 0708 f90c 0b1a 010e 0118 0108 0102 ff0a  ................
+00000680: 037a 0d50 6c6f 742e 5f5f 696e 6974 5f5f  .z.Plot.__init__
+00000690: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
+000006a0: 0003 0000 0003 0000 0073 3000 0000 7c03  .........s0...|.
+000006b0: 720d 8700 8701 6602 6401 6402 8408 7c00  r.....f.d.d...|.
+000006c0: 6a00 4400 8301 5300 8700 8701 6602 6403  j.D...S.....f.d.
+000006d0: 6402 8408 7c00 6a01 4400 8301 5300 2904  d...|.j.D...S.).
+000006e0: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+000006f0: 0000 0500 0000 1300 0000 7316 0000 0067  ..........s....g
+00000700: 007c 005d 077d 0188 017c 0188 0083 0291  .|.].}...|......
+00000710: 0271 0253 0072 0800 0000 7208 0000 00a9  .q.S.r....r.....
+00000720: 0272 0900 0000 721c 0000 00a9 02da 0672  .r....r........r
+00000730: 6567 696f 6eda 0376 6172 7208 0000 0072  egion..varr....r
+00000740: 0d00 0000 720e 0000 004c 0000 0073 0200  ....r....L...s..
+00000750: 0000 1600 7a1f 506c 6f74 2e5f 7661 6c75  ....z.Plot._valu
+00000760: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
+00000770: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
+00000780: 0000 0200 0000 0600 0000 1300 0000 731c  ..............s.
+00000790: 0000 0067 007c 005d 0a7d 0174 0088 017c  ...g.|.].}.t...|
+000007a0: 0188 0066 0219 0083 0191 0271 0253 0072  ...f.......q.S.r
+000007b0: 0800 0000 7202 0000 0072 2b00 0000 722c  ....r....r+...r,
+000007c0: 0000 0072 0800 0000 720d 0000 0072 0e00  ...r....r....r..
+000007d0: 0000 4e00 0000 7302 0000 001c 0029 0272  ..N...s......).r
+000007e0: 1d00 0000 721c 0000 0029 0472 2600 0000  ....r....).r&...
+000007f0: 722e 0000 0072 2d00 0000 da06 6973 5f66  r....r-.....is_f
+00000800: 6374 7208 0000 0072 2c00 0000 720d 0000  ctr....r,...r...
+00000810: 00da 065f 7661 6c75 654a 0000 0073 0600  ..._valueJ...s..
+00000820: 0000 0401 1601 1602 7a0b 506c 6f74 2e5f  ........z.Plot._
+00000830: 7661 6c75 6563 0300 0000 0000 0000 0000  valuec..........
+00000840: 0000 0300 0000 0300 0000 0300 0000 732c  ..............s,
+00000850: 0000 007c 0272 0c87 0066 0164 0164 0284  ...|.r...f.d.d..
+00000860: 087c 006a 0044 0083 0153 0087 0066 0164  .|.j.D...S...f.d
+00000870: 0364 0284 087c 006a 0044 0083 0153 0029  .d...|.j.D...S.)
+00000880: 044e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
+00000890: 0000 0004 0000 0013 0000 0073 1400 0000  ...........s....
+000008a0: 6700 7c00 5d06 7d01 8800 7c01 8301 9102  g.|.].}...|.....
+000008b0: 7102 5300 7208 0000 0072 0800 0000 722b  q.S.r....r....r+
+000008c0: 0000 00a9 0172 2e00 0000 7208 0000 0072  .....r....r....r
+000008d0: 0d00 0000 720e 0000 0052 0000 0073 0200  ....r....R...s..
+000008e0: 0000 1400 7a26 506c 6f74 2e5f 7661 6c75  ....z&Plot._valu
+000008f0: 655f 676c 6f62 616c 2e3c 6c6f 6361 6c73  e_global.<locals
+00000900: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
+00000910: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00000920: 0013 0000 0073 1800 0000 6700 7c00 5d08  .....s....g.|.].
+00000930: 7d01 7400 8800 7c01 1900 8301 9102 7102  }.t...|.......q.
+00000940: 5300 7208 0000 0072 0200 0000 722b 0000  S.r....r....r+..
+00000950: 0072 3100 0000 7208 0000 0072 0d00 0000  .r1...r....r....
+00000960: 720e 0000 0054 0000 0073 0200 0000 1800  r....T...s......
+00000970: 2901 721c 0000 0029 0372 2600 0000 722e  ).r....).r&...r.
+00000980: 0000 0072 2f00 0000 7208 0000 0072 3100  ...r/...r....r1.
+00000990: 0000 720d 0000 00da 0d5f 7661 6c75 655f  ..r......_value_
+000009a0: 676c 6f62 616c 5000 0000 7306 0000 0004  globalP...s.....
+000009b0: 0114 0114 027a 1250 6c6f 742e 5f76 616c  .....z.Plot._val
+000009c0: 7565 5f67 6c6f 6261 6c63 0700 0000 0000  ue_globalc......
+000009d0: 0000 0000 0000 0800 0000 0b00 0000 4b00  ..............K.
+000009e0: 0000 734e 0000 007c 006a 006a 0164 077c  ..sN...|.j.j.d.|
+000009f0: 006a 027c 017c 027c 027c 037c 047c 057c  .j.|.|.|.|.|.|.|
+00000a00: 0664 019c 0864 027c 0776 0172 1f64 027c  .d...d.|.v.r.d.|
+00000a10: 07a0 0364 0364 04a1 0272 1c64 056e 0164  ...d.d...r.d.n.d
+00000a20: 0669 016e 0169 00a4 017c 07a4 018e 0101  .i.n.i...|......
+00000a30: 0064 0053 0029 084e 2908 da01 78da 0179  .d.S.).N)...x..y
+00000a40: da04 6e61 6d65 5a0b 6c65 6765 6e64 6772  ..nameZ.legendgr
+00000a50: 6f75 705a 0a6c 696e 655f 636f 6c6f 7272  oupZ.line_colorr
+00000a60: 1300 0000 7214 0000 00da 0a73 686f 776c  ....r......showl
+00000a70: 6567 656e 645a 096c 696e 655f 6461 7368  egendZ.line_dash
+00000a80: 7207 0000 0046 da03 646f 74da 0573 6f6c  r....F..dot..sol
+00000a90: 6964 7208 0000 0029 0472 2100 0000 da0b  idr....).r!.....
+00000aa0: 6164 645f 7363 6174 7465 7272 1d00 0000  add_scatterr....
+00000ab0: da03 6765 7429 0872 2600 0000 da06 7661  ..get).r&.....va
+00000ac0: 6c75 6573 7235 0000 00da 0563 6f6c 6f72  luesr5.....color
+00000ad0: 7213 0000 0072 1400 0000 7236 0000 0072  r....r....r6...r
+00000ae0: 2700 0000 7208 0000 0072 0800 0000 720d  '...r....r....r.
+00000af0: 0000 0072 3900 0000 5600 0000 7320 0000  ...r9...V...s ..
+00000b00: 0008 0104 0102 0102 0102 0102 0102 0102  ................
+00000b10: 0102 0104 f808 0b18 ff02 0202 f402 0e0a  ................
+00000b20: f27a 1050 6c6f 742e 6164 645f 7363 6174  .z.Plot.add_scat
+00000b30: 7465 7254 4672 1000 0000 6306 0000 0000  terTFr....c.....
+00000b40: 0000 0000 0000 000b 0000 0007 0000 004b  ...............K
+00000b50: 0000 0073 c000 0000 7c03 7309 7c04 6400  ...s....|.s.|.d.
+00000b60: 7500 7209 7c01 6a00 7d04 7c04 7c00 6a01  u.r.|.j.}.|.|.j.
+00000b70: 7601 7d07 7c07 7218 7402 7c00 6a01 8301  v.}.|.r.t.|.j...
+00000b80: 7c00 6a01 7c04 3c00 7403 7c00 6a01 7c04  |.j.|.<.t.|.j.|.
+00000b90: 1900 7402 7403 8301 1600 1900 7d08 7c02  ..t.t.......}.|.
+00000ba0: 724b 7404 7c00 6a05 8301 4400 5d1e 5c02  rKt.|.j...D.].\.
+00000bb0: 7d09 7d0a 7c00 6a06 7c00 a007 7c01 7c0a  }.}.|.j.|...|.|.
+00000bc0: 7c03 a103 7c04 7c08 7c05 6604 7c09 6401  |...|.|.|.f.|.d.
+00000bd0: 1700 7c07 6f42 7c09 6402 6b02 6403 9c02  ..|.oB|.d.k.d...
+00000be0: 7c06 a401 8e01 0100 712a 6400 5300 7c00  |.......q*d.S.|.
+00000bf0: 6a06 7c00 a008 7c01 7c03 a102 7c04 7c08  j.|...|.|...|.|.
+00000c00: 7c05 6604 6401 7c07 6403 9c02 7c06 a401  |.f.d.|.d...|...
+00000c10: 8e01 0100 6400 5300 2904 4e72 1000 0000  ....d.S.).Nr....
+00000c20: 7201 0000 0029 0272 1400 0000 7236 0000  r....).r....r6..
+00000c30: 0029 0972 3500 0000 7225 0000 0072 1e00  .).r5...r%...r..
+00000c40: 0000 da0a 434f 4c4f 5253 5f50 424c da09  ....COLORS_PBL..
+00000c50: 656e 756d 6572 6174 6572 1800 0000 7239  enumerater....r9
+00000c60: 0000 0072 3000 0000 7232 0000 0029 0b72  ...r0...r2...).r
+00000c70: 2600 0000 722e 0000 00da 0b69 735f 7265  &...r......is_re
+00000c80: 6769 6f6e 616c 722f 0000 0072 3500 0000  gionalr/...r5...
+00000c90: 7213 0000 0072 2700 0000 da03 6e65 7772  r....r'.....newr
+00000ca0: 3c00 0000 7228 0000 00da 0172 7208 0000  <...r(.....rr...
+00000cb0: 0072 0800 0000 720d 0000 00da 0361 6464  .r....r......add
+00000cc0: 6800 0000 733e 0000 000c 0106 010a 0104  h...s>..........
+00000cd0: 0210 0116 0104 0212 0104 010c 0102 0102  ................
+00000ce0: 0102 0102 fc06 050a 0104 fa02 0708 f904  ................
+00000cf0: ff04 0b0a 0102 0102 0102 0102 fc02 0502  ................
+00000d00: 0104 fa02 070a f97a 0850 6c6f 742e 6164  .......z.Plot.ad
+00000d10: 6463 0100 0000 0000 0000 0000 0000 0200  dc..............
+00000d20: 0000 0600 0000 4300 0000 7372 0000 007c  ......C...sr...|
+00000d30: 006a 006a 017c 006a 0264 0119 0064 0267  .j.j.|.j.d...d.g
+00000d40: 0264 038d 0101 0074 0364 0474 047c 006a  .d.....t.d.t.|.j
+00000d50: 0583 0183 0244 005d 0b7d 017c 006a 006a  .....D.].}.|.j.j
+00000d60: 0664 0564 067c 0164 078d 0301 0071 147c  .d.d.|.d.....q.|
+00000d70: 006a 006a 0764 0864 098d 0101 007c 006a  .j.j.d.d.....|.j
+00000d80: 006a 0864 0a64 0a64 0a64 0a64 0b9c 0464  .j.d.d.d.d.d...d
+00000d90: 0c64 0d64 0e9c 0264 0f8d 0201 0064 0053  .d.d...d.....d.S
+00000da0: 0029 104e 7201 0000 0069 3408 0000 2901  .).Nr....i4...).
+00000db0: 721f 0000 0072 1000 0000 5446 2903 7207  r....r....TF).r.
+00000dc0: 0000 005a 0e73 686f 7774 6963 6b6c 6162  ...Z.showticklab
+00000dd0: 656c 7372 1400 0000 da05 6c69 6e65 7329  elsr......lines)
+00000de0: 01da 046d 6f64 65e9 3200 0000 2904 721c  ...mode.2...).r.
+00000df0: 0000 00da 016c 7241 0000 00da 0162 da06  .....lrA.....b..
+00000e00: 6d69 6464 6c65 6700 0000 0000 00e0 3f29  middleg.......?)
+00000e10: 025a 0779 616e 6368 6f72 7234 0000 0029  .Z.yanchorr4...)
+00000e20: 02da 066d 6172 6769 6eda 066c 6567 656e  ...margin..legen
+00000e30: 6429 0972 2100 0000 5a0c 7570 6461 7465  d).r!...Z.update
+00000e40: 5f78 6178 6573 721d 0000 0072 1f00 0000  _xaxesr....r....
+00000e50: 721e 0000 0072 1800 0000 da0c 7570 6461  r....r......upda
+00000e60: 7465 5f79 6178 6573 5a0d 7570 6461 7465  te_yaxesZ.update
+00000e70: 5f74 7261 6365 73da 0d75 7064 6174 655f  _traces..update_
+00000e80: 6c61 796f 7574 2902 7226 0000 0072 2800  layout).r&...r(.
+00000e90: 0000 7208 0000 0072 0800 0000 720d 0000  ..r....r....r...
+00000ea0: 00da 0a73 6574 5f6c 6179 6f75 7487 0000  ...set_layout...
+00000eb0: 0073 1000 0000 1801 1401 1401 0e01 0601  .s..............
+00000ec0: 0c01 0801 0afe 7a0f 506c 6f74 2e73 6574  ......z.Plot.set
+00000ed0: 5f6c 6179 6f75 7463 0200 0000 0000 0000  _layoutc........
+00000ee0: 0000 0000 0400 0000 0700 0000 4300 0000  ............C...
+00000ef0: 732e 0000 0074 007c 0183 0144 005d 105c  s....t.|...D.].\
+00000f00: 027d 027d 037c 006a 016a 027c 037c 0264  .}.}.|.j.j.|.|.d
+00000f10: 0117 0064 0164 0264 038d 0401 0071 0464  ...d.d.d.....q.d
+00000f20: 0053 0029 044e 7210 0000 0046 2904 da05  .S.).Nr....F)...
+00000f30: 7469 746c 6572 1300 0000 7214 0000 0072  titler....r....r
+00000f40: 0700 0000 2903 723e 0000 0072 2100 0000  ....).r>...r!...
+00000f50: 724b 0000 0029 0472 2600 0000 da06 7469  rK...).r&.....ti
+00000f60: 746c 6573 7228 0000 0072 4e00 0000 7208  tlesr(...rN...r.
+00000f70: 0000 0072 0800 0000 720d 0000 00da 1073  ...r....r......s
+00000f80: 6574 5f79 6178 6573 5f74 6974 6c65 7391  et_yaxes_titles.
+00000f90: 0000 0073 0600 0000 1001 1a01 04ff 7a15  ...s..........z.
+00000fa0: 506c 6f74 2e73 6574 5f79 6178 6573 5f74  Plot.set_yaxes_t
+00000fb0: 6974 6c65 7363 0100 0000 0000 0000 0000  itlesc..........
+00000fc0: 0000 0100 0000 0200 0000 4300 0000 730e  ..........C...s.
+00000fd0: 0000 007c 00a0 00a1 0001 007c 006a 0153  ...|.......|.j.S
+00000fe0: 0029 014e 2902 724d 0000 0072 2100 0000  .).N).rM...r!...
+00000ff0: 2901 7226 0000 0072 0800 0000 7208 0000  ).r&...r....r...
+00001000: 0072 0d00 0000 da04 7368 6f77 9500 0000  .r......show....
+00001010: 7304 0000 0008 0106 017a 0950 6c6f 742e  s........z.Plot.
+00001020: 7368 6f77 2903 7206 0000 004e 4e29 0454  show).r....NN).T
+00001030: 464e 7210 0000 0029 0cda 085f 5f6e 616d  FNr....)...__nam
+00001040: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00001050: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00001060: 5f64 6f63 5f5f 722a 0000 0072 3000 0000  _doc__r*...r0...
+00001070: 7232 0000 0072 3900 0000 7242 0000 0072  r2...r9...rB...r
+00001080: 4d00 0000 7250 0000 0072 5100 0000 7208  M...rP...rQ...r.
+00001090: 0000 0072 0800 0000 7208 0000 0072 0d00  ...r....r....r..
+000010a0: 0000 7205 0000 0022 0000 0073 1400 0000  ..r...."...s....
+000010b0: 0800 0401 0a07 0820 0806 0806 0a12 081f  ....... ........
+000010c0: 080a 0c04 7205 0000 0063 0100 0000 0000  ....r....c......
+000010d0: 0000 0000 0000 0900 0000 0700 0000 4300  ..............C.
+000010e0: 0000 7318 0100 0074 007c 0064 0183 027d  ..s....t.|.d...}
+000010f0: 0164 027d 0267 007d 037c 0144 005d 437d  .d.}.g.}.|.D.]C}
+00001100: 047c 04a0 0164 03a1 0172 1464 047d 027c  .|...d...r.d.}.|
+00001110: 04a0 02a1 0064 056b 0272 1c64 027d 027c  .....d.k.r.d.}.|
+00001120: 0272 4e7c 04a0 0164 06a1 0172 4e7c 04a0  .rN|...d...rN|..
+00001130: 02a1 00a0 0364 06a1 0164 0064 0785 0219  .....d...d.d....
+00001140: 007d 0564 017c 0564 0819 0076 0072 4464  .}.d.|.d...v.rDd
+00001150: 047d 067c 0564 0819 00a0 0364 01a1 017c  .}.|.d.....d...|
+00001160: 0564 0964 0a85 0219 0017 007d 056e 0264  .d.d.......}.n.d
+00001170: 027d 067c 03a0 047c 057c 0667 0117 00a1  .}.|...|.|.g....
+00001180: 0101 0071 0b74 056a 067c 0367 0064 0ba2  ...q.t.j.|.g.d..
+00001190: 0164 0c8d 027d 077c 07a0 0774 0874 0974  .d...}.|...t.t.t
+000011a0: 0974 0964 0d9c 04a1 017d 077c 01a0 0aa1  .t.d.....}.|....
+000011b0: 0001 0074 0b6a 0c7c 0764 0e67 0064 0fa2  ...t.j.|.d.g.d..
+000011c0: 0164 1064 1164 128d 056a 0d64 0064 1364  .d.d.d...j.d.d.d
+000011d0: 148d 026a 0d64 1564 1664 178d 027d 087c  ...j.d.d.d...}.|
+000011e0: 086a 0e7c 00a0 0364 18a1 0164 0819 0064  .j.|...d...d...d
+000011f0: 1917 0064 1a64 1b8d 0201 0064 0053 0029  ...d.d.....d.S.)
+00001200: 1c4e 7241 0000 0046 7a05 6974 6572 2054  .NrA...Fz.iter T
+00001210: 7216 0000 00fa 0120 7206 0000 0072 0100  r...... r....r..
+00001220: 0000 7210 0000 00e9 ffff ffff 2905 da04  ..r.........)...
+00001230: 6974 6572 da09 6f62 6a65 6374 6976 65da  iter..objective.
+00001240: 0669 6e66 5f70 72da 0669 6e66 5f64 75da  .inf_pr..inf_du.
+00001250: 0972 6563 6f76 6572 6564 2901 da07 636f  .recovered)...co
+00001260: 6c75 6d6e 7329 0472 5800 0000 7259 0000  lumns).rX...rY..
+00001270: 0072 5a00 0000 725b 0000 0072 5800 0000  .rZ...r[...rX...
+00001280: 2903 7259 0000 0072 5a00 0000 725b 0000  ).rY...rZ...r[..
+00001290: 00da 0876 6172 6961 626c 6572 5c00 0000  ...variabler\...
+000012a0: 2904 7233 0000 0072 3400 0000 5a09 6661  ).r3...r4...Z.fa
+000012b0: 6365 745f 726f 7772 3c00 0000 da03 6c6f  cet_rowr<.....lo
+000012c0: 6729 0272 2400 0000 da04 7479 7065 e903  g).r$.....type..
+000012d0: 0000 00da 066c 696e 6561 7229 0272 1300  .....linear).r..
+000012e0: 0000 7260 0000 00da 012e 7a05 2e68 746d  ..r`......z..htm
+000012f0: 6c5a 0363 646e 2901 da10 696e 636c 7564  lZ.cdn)...includ
+00001300: 655f 706c 6f74 6c79 6a73 290f da04 6f70  e_plotlyjs)...op
+00001310: 656e da0a 7374 6172 7473 7769 7468 da05  en..startswith..
+00001320: 7374 7269 70da 0573 706c 6974 da06 6170  strip..split..ap
+00001330: 7065 6e64 da02 7064 da09 4461 7461 4672  pend..pd..DataFr
+00001340: 616d 65da 0661 7374 7970 65da 0369 6e74  ame..astype..int
+00001350: da05 666c 6f61 74da 0563 6c6f 7365 da02  ..float..close..
+00001360: 7078 da07 7363 6174 7465 7272 4b00 0000  px..scatterrK...
+00001370: da0a 7772 6974 655f 6874 6d6c 2909 da0b  ..write_html)...
+00001380: 6f75 7470 7574 5f66 696c 65da 0466 696c  output_file..fil
+00001390: 655a 0d69 6e5f 6974 6572 6174 696f 6e73  eZ.in_iterations
+000013a0: da0a 6974 6572 6174 696f 6e73 da04 6c69  ..iterations..li
+000013b0: 6e65 7268 0000 0072 5c00 0000 5a0d 6974  nerh...r\...Z.it
+000013c0: 6572 6174 696f 6e73 5f64 6672 2100 0000  erations_dfr!...
+000013d0: 7208 0000 0072 0800 0000 720d 0000 00da  r....r....r.....
+000013e0: 1676 6973 7561 6c69 7365 5f69 706f 7074  .visualise_ipopt
+000013f0: 5f6f 7574 7075 749a 0000 0073 4800 0000  _output....sH...
+00001400: 0a01 0401 0402 0802 0a01 0401 0c01 0401  ................
+00001410: 0e02 1601 0c03 0401 1c01 0402 1001 0280  ................
+00001420: 0402 0801 06ff 0403 0c01 04ff 0804 0403  ................
+00001430: 0201 0201 0601 0201 0201 04fb 0607 04f9  ................
+00001440: 0608 04f8 02ff 200c 7277 0000 0029 1072  ...... .rw...).r
+00001450: 5500 0000 da05 6e75 6d70 7972 1a00 0000  U.....numpyr....
+00001460: da06 7061 6e64 6173 726a 0000 00da 0d70  ..pandasrj.....p
+00001470: 796f 6d6f 2e65 6e76 6972 6f6e 7203 0000  yomo.environr...
+00001480: 005a 0e70 6c6f 746c 792e 6578 7072 6573  .Z.plotly.expres
+00001490: 735a 0765 7870 7265 7373 7270 0000 005a  sZ.expressrp...Z
+000014a0: 0f70 6c6f 746c 792e 7375 6270 6c6f 7473  .plotly.subplots
+000014b0: 7204 0000 00da 134d 6f64 756c 654e 6f74  r......ModuleNot
+000014c0: 466f 756e 6445 7272 6f72 723d 0000 0072  FoundErrorr=...r
+000014d0: 0500 0000 7277 0000 0072 0800 0000 7208  ....rw...r....r.
+000014e0: 0000 0072 0800 0000 720d 0000 00da 083c  ...r....r......<
+000014f0: 6d6f 6475 6c65 3e01 0000 0073 1a00 0000  module>....s....
+00001500: 0400 0803 0801 0c01 0202 0c01 1001 0c01  ................
+00001510: 0401 02ff 0803 0e14 0c78                 .........x
```

### Comparing `mimosa-0.1.3/mimosa/export/plot.py` & `mimosa-0.1.4/mimosa/export/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,29 @@
     plot.add(m.carbonprice, row=1, secondary_y=True)
     try:
         plot.add(m.adapt_costs, row=2, stackgroup="costs")
         plot.add(m.resid_damages, row=2, stackgroup="costs")
         plot.add(m.gross_damages, row=2)
     except AttributeError:
         plot.add(m.damage_costs, row=2, stackgroup="costs")
-    plot.add(m.rel_abatement_costs, row=2, stackgroup="costs")
+    plot.add(m.rel_mitigation_costs, row=2, stackgroup="costs")
 
     plot.add(m.capital_stock, row=3)
     plot.add(m.GDP_gross, row=3)
     plot.add(m.GDP_net, row=3)
     plot.add(m.consumption, row=3, visible="legendonly")
     plot.add(m.utility, row=3, secondary_y=True, visible="legendonly")
-    plot.add(m.abatement_costs, row=3, visible="legendonly")
+    plot.add(m.mitigation_costs, row=3, visible="legendonly")
     plot.add(m.global_emissions, is_regional=False, row=4)
     plot.add(m.temperature, is_regional=False, row=4, secondary_y=True)
     plot.add(m.cumulative_emissions, is_regional=False, row=4, visible="legendonly")
 
     try:
         plot.add(
-            m.global_rel_abatement_costs,
+            m.global_rel_mitigation_costs,
             is_regional=False,
             row=4,
             secondary_y=True,
             visible="legendonly",
         )
     except AttributeError:
         pass
```

### Comparing `mimosa-0.1.3/mimosa/export/save.py` & `mimosa-0.1.4/mimosa/export/save.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Generates a CSV file with a row for each variable (`Var`)
 in the ConcreteModel `m`.
 """
 
 import json
 import os
-import random
 import hashlib
 import numpy as np
 import pandas as pd
 
 from mimosa.common import get_all_variables, value
 
 
-def save_output(params, m, experiment=None, hash_suffix=True, folder="output"):
+def save_output(params, m, experiment=None, hash_suffix=False, folder="output"):
     # 1. Create a unique identifier
     if hash_suffix:
         settings_hash = hashlib.md5(json.dumps(params).encode()).hexdigest()[:9]
     else:
         settings_hash = ""
 
     # 2. Save the Pyomo variables and data functions
```

### Comparing `mimosa-0.1.3/mimosa/export/utils.py` & `mimosa-0.1.4/mimosa/export/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/inputdata/config/config_R5.yaml` & `mimosa-0.1.4/mimosa/inputdata/config/config_R5.yaml`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/inputdata/config/config_default.yaml` & `mimosa-0.1.4/mimosa/inputdata/config/config_default.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         - kappa_rel_abatement_0.5_2070
         - kappa_rel_abatement_0.5_2100
         - kappa_rel_abatement_0.75_2050
         - kappa_rel_abatement_0.75_2070
         - kappa_rel_abatement_0.75_2100
       default: kappa_rel_abatement_0.75_2050
 
-    rel_abatement_costs_min_level:
+    rel_mitigation_costs_min_level:
       descr: >-
         Minimum level of mitigation costs (rel to GDP). By default, this is 0:
         no negative abatement costs are allowed. For certain burden sharing regimes,
         this value can become negative to allow certain (small) financial transfers.
       type: float
       min: -2
       max: 0
@@ -423,15 +423,15 @@
 
 burden sharing:
   regime:
     descr: Type of burden sharing to be used
     type: enum
     values:
       - noregime
-      - equal_abatement_costs
+      - equal_mitigation_costs
       - equal_total_costs
       - per_cap_convergence
       - per_cap_convergence_fake # Per cap convergence performed in post-processing
     default: noregime
   percapconv_year:
     descr: >-
       Year of convergence to per capita emission allowance 
@@ -496,18 +496,18 @@
       - globaldamagepool
     default: notransfer
 
   welfare module:
     descr: Welfare and utility module to be used
     type: enum
     values:
-      - inequal_aversion_elasmu
-      - inequal_aversion_zero
+      - welfare_loss_minimising
+      - cost_minimising
       - inequal_aversion_general
-    default: inequal_aversion_elasmu
+    default: welfare_loss_minimising
 
   objective module:
     descr: Objective module to be used
     type: enum
     values:
       - utility
       - globalcosts
```

### Comparing `mimosa-0.1.3/mimosa/inputdata/data/data_IMAGE_SSP.csv` & `mimosa-0.1.4/mimosa/inputdata/data/data_IMAGE_SSP.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv` & `mimosa-0.1.4/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/inputdata/params/ADRICE2012.csv` & `mimosa-0.1.4/mimosa/inputdata/params/ADRICE2012.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/inputdata/params/COACCH.csv` & `mimosa-0.1.4/mimosa/inputdata/params/COACCH.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/inputdata/params/mac.csv` & `mimosa-0.1.4/mimosa/inputdata/params/mac.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_regions.json` & `mimosa-0.1.4/mimosa/inputdata/regions/IMAGE26_regions.json`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/inputdata/regions/R5_regions.json` & `mimosa-0.1.4/mimosa/inputdata/regions/R5_regions.json`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/inputdata/regions/country_ISO_codes.csv` & `mimosa-0.1.4/mimosa/inputdata/regions/country_ISO_codes.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/mimosa.py` & `mimosa-0.1.4/mimosa/mimosa.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa/socialcostofcarbon/scc.py` & `mimosa-0.1.4/mimosa/socialcostofcarbon/scc.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.3/mimosa.egg-info/SOURCES.txt` & `mimosa-0.1.4/mimosa.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,25 @@
 mimosa/common/regional_params/region_mappers.py
 mimosa/common/regional_params/regional_param_container.py
 mimosa/common/regional_params/__pycache__/__init__.cpython-310.pyc
 mimosa/common/regional_params/__pycache__/main.cpython-310.pyc
 mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc
 mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc
 mimosa/components/__init__.py
-mimosa/components/abatement.py
 mimosa/components/burdensharing.py
 mimosa/components/cobbdouglas.py
 mimosa/components/emissions.py
+mimosa/components/mitigation.py
 mimosa/components/sealevelrise.py
 mimosa/components/__pycache__/__init__.cpython-310.pyc
 mimosa/components/__pycache__/abatement.cpython-310.pyc
 mimosa/components/__pycache__/burdensharing.cpython-310.pyc
 mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc
 mimosa/components/__pycache__/emissions.cpython-310.pyc
+mimosa/components/__pycache__/mitigation.cpython-310.pyc
 mimosa/components/__pycache__/sealevelrise.cpython-310.pyc
 mimosa/components/damages/__init__.py
 mimosa/components/damages/ad_rice2010.py
 mimosa/components/damages/ad_rice2012.py
 mimosa/components/damages/ad_witch.py
 mimosa/components/damages/coacch.py
 mimosa/components/damages/nodamage.py
@@ -93,21 +94,23 @@
 mimosa/components/objective/__init__.py
 mimosa/components/objective/globalcosts.py
 mimosa/components/objective/utility.py
 mimosa/components/objective/__pycache__/__init__.cpython-310.pyc
 mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc
 mimosa/components/objective/__pycache__/utility.cpython-310.pyc
 mimosa/components/welfare/__init__.py
-mimosa/components/welfare/inequal_aversion_elasmu.py
+mimosa/components/welfare/cost_minimising.py
 mimosa/components/welfare/inequal_aversion_general.py
-mimosa/components/welfare/inequal_aversion_zero.py
+mimosa/components/welfare/welfare_loss_minimising.py
 mimosa/components/welfare/__pycache__/__init__.cpython-310.pyc
+mimosa/components/welfare/__pycache__/cost_minimising.cpython-310.pyc
 mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc
 mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc
 mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc
+mimosa/components/welfare/__pycache__/welfare_loss_minimising.cpython-310.pyc
 mimosa/concrete_model/__init__.py
 mimosa/concrete_model/instantiate_params.py
 mimosa/concrete_model/__pycache__/__init__.cpython-310.pyc
 mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc
 mimosa/concrete_model/simulation_mode/__init__.py
 mimosa/concrete_model/simulation_mode/deactivate_constraints.py
 mimosa/concrete_model/simulation_mode/main.py
```

### Comparing `mimosa-0.1.3/setup.py` & `mimosa-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from setuptools import setup
 
 with open("README.md") as fh:
     description = fh.read()
 
+with open("LICENSE") as fh:
+    license_txt = fh.read()
+
 setup(
     name="mimosa",
-    version="0.1.3",
+    version="0.1.4",
     author="Kaj-Ivar van der Wijst",
     author_email="k.i.vanderwijst@gmail.com",
     packages=["mimosa"],
-    # url="http://pypi.python.org/pypi/PackageName/",
-    license="LICENSE.txt",
+    url="https://github.com/kvanderwijst/MIMOSA",
+    license=license_txt,
     description="MIMOSA: Integrated Assessment Model for Cost-Benefit Analysis",
     long_description=description,
     long_description_content_type="text/markdown",
     install_requires=["numpy", "pandas", "pyomo", "pint", "pyyaml", "scipy"],
     include_package_data=True,
 )
```

