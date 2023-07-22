# Comparing `tmp/emlvp-0.0.5.tar.gz` & `tmp/emlvp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emlvp-0.0.5.tar", last modified: Tue Feb  7 02:52:42 2023, max compression
+gzip compressed data, was "emlvp-0.0.6.tar", last modified: Sat Jul 22 01:52:34 2023, max compression
```

## Comparing `emlvp-0.0.5.tar` & `emlvp-0.0.6.tar`

### file list

```diff
@@ -1,112 +1,116 @@
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-02-07 02:52:42.045295 emlvp-0.0.5/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    11357 2023-01-21 18:45:39.000000 emlvp-0.0.5/LICENSE
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      130 2023-02-01 23:07:16.000000 emlvp-0.0.5/MANIFEST.in
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    20771 2023-02-07 02:52:42.045295 emlvp-0.0.5/PKG-INFO
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7490 2023-02-02 20:38:58.000000 emlvp-0.0.5/README.md
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      766 2023-02-07 02:52:42.045295 emlvp-0.0.5/setup.cfg
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1252 2023-02-01 23:40:10.000000 emlvp-0.0.5/setup.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-02-07 02:52:42.013295 emlvp-0.0.5/src/
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-02-07 02:52:42.013295 emlvp-0.0.5/src/emlvp/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2023-02-06 20:44:52.000000 emlvp-0.0.5/src/emlvp/VERSION.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      128 2023-01-21 19:41:00.000000 emlvp-0.0.5/src/emlvp/__init__.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      637 2023-02-07 02:51:01.000000 emlvp-0.0.5/src/emlvp/changelog.md
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1658 2023-02-06 20:43:54.000000 emlvp-0.0.5/src/emlvp/dereferencer.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     5461 2023-02-06 20:52:18.000000 emlvp-0.0.5/src/emlvp/emlvp_cli.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1121 2023-01-27 21:12:55.000000 emlvp-0.0.5/src/emlvp/exceptions.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8209 2023-02-06 20:39:02.000000 emlvp-0.0.5/src/emlvp/parser.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-02-07 02:52:42.013295 emlvp-0.0.5/src/emlvp/schemas/
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-02-07 02:52:42.025295 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    18447 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-access.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-entity.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-literature.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-methods.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29487 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-party.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-physical.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-project.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    58886 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-resource.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-software.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    18745 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-text.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-view.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    19139 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:00.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/stmml.xsd
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-02-07 02:52:42.037295 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    20356 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-access.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-entity.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-literature.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-methods.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29531 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-party.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-physical.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-project.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    60720 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-resource.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-software.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21204 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-text.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-view.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    19379 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:17.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/stmml.xsd
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-02-07 02:52:42.041295 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493311 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   102174 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-02-07 02:52:42.045295 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    11830 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    86976 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    27152 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    72264 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7693 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    28001 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2899 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    14949 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    58814 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21970 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    28924 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    76821 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29309 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     4952 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    68327 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    15511 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21403 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    46367 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   167250 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    13021 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    10334 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    32155 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    23090 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7008 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22368 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   133761 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      579 2023-01-31 04:06:28.000000 emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1978 2023-02-06 20:13:41.000000 emlvp-0.0.5/src/emlvp/validator.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-02-07 02:52:42.013295 emlvp-0.0.5/src/emlvp.egg-info/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    20771 2023-02-07 02:52:42.000000 emlvp-0.0.5/src/emlvp.egg-info/PKG-INFO
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     4294 2023-02-07 02:52:42.000000 emlvp-0.0.5/src/emlvp.egg-info/SOURCES.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        1 2023-02-07 02:52:42.000000 emlvp-0.0.5/src/emlvp.egg-info/dependency_links.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)       47 2023-02-07 02:52:42.000000 emlvp-0.0.5/src/emlvp.egg-info/entry_points.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)       41 2023-02-07 02:52:42.000000 emlvp-0.0.5/src/emlvp.egg-info/requires.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2023-02-07 02:52:42.000000 emlvp-0.0.5/src/emlvp.egg-info/top_level.txt
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.124358 emlvp-0.0.6/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    11357 2023-01-21 18:45:39.000000 emlvp-0.0.6/LICENSE
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      130 2023-02-01 23:07:16.000000 emlvp-0.0.6/MANIFEST.in
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    20856 2023-07-22 01:52:34.124358 emlvp-0.0.6/PKG-INFO
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7575 2023-02-18 19:31:04.000000 emlvp-0.0.6/README.md
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      766 2023-07-22 01:52:34.124358 emlvp-0.0.6/setup.cfg
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1252 2023-02-01 23:40:10.000000 emlvp-0.0.6/setup.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.108358 emlvp-0.0.6/src/
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.108358 emlvp-0.0.6/src/emlvp/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2023-07-22 01:48:47.000000 emlvp-0.0.6/src/emlvp/VERSION.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      128 2023-01-21 19:41:00.000000 emlvp-0.0.6/src/emlvp/__init__.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      773 2023-07-22 01:48:47.000000 emlvp-0.0.6/src/emlvp/changelog.md
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1658 2023-02-06 20:43:54.000000 emlvp-0.0.6/src/emlvp/dereferencer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     5467 2023-07-22 01:39:02.000000 emlvp-0.0.6/src/emlvp/emlvp_cli.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1121 2023-01-27 21:12:55.000000 emlvp-0.0.6/src/emlvp/exceptions.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8209 2023-02-06 20:39:02.000000 emlvp-0.0.6/src/emlvp/parser.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.108358 emlvp-0.0.6/src/emlvp/schemas/
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.112357 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    18447 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-access.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-entity.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-literature.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-methods.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    29487 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-party.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-physical.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-project.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    58886 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-resource.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-software.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    18745 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-text.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-view.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    19139 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:00.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/stmml.xsd
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.116357 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    20356 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-access.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-entity.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-literature.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-methods.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    29531 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-party.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-physical.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-project.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    60720 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-resource.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-software.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21204 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-text.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-view.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    19379 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:17.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/stmml.xsd
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.120357 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493311 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   102174 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.124358 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    11830 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    86976 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    27152 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    72264 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7693 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    28001 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2899 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    14949 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    58814 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21970 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    28924 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    76821 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    29309 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     4952 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    68327 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    15511 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21403 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    46367 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   167250 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    13021 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    10334 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    32155 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    23090 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7008 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22368 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   133761 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      579 2023-01-31 04:06:28.000000 emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1978 2023-02-06 20:13:41.000000 emlvp-0.0.6/src/emlvp/validator.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.108358 emlvp-0.0.6/src/emlvp.egg-info/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    20856 2023-07-22 01:52:34.000000 emlvp-0.0.6/src/emlvp.egg-info/PKG-INFO
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     4366 2023-07-22 01:52:34.000000 emlvp-0.0.6/src/emlvp.egg-info/SOURCES.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        1 2023-07-22 01:52:34.000000 emlvp-0.0.6/src/emlvp.egg-info/dependency_links.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)       47 2023-07-22 01:52:34.000000 emlvp-0.0.6/src/emlvp.egg-info/entry_points.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)       41 2023-07-22 01:52:34.000000 emlvp-0.0.6/src/emlvp.egg-info/requires.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2023-07-22 01:52:34.000000 emlvp-0.0.6/src/emlvp.egg-info/top_level.txt
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2023-07-22 01:52:34.124358 emlvp-0.0.6/tests/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      689 2023-07-22 01:19:36.000000 emlvp-0.0.6/tests/test_dereferencer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2896 2023-07-22 01:19:36.000000 emlvp-0.0.6/tests/test_parser.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2065 2023-07-22 01:19:36.000000 emlvp-0.0.6/tests/test_validator.py
```

### Comparing `emlvp-0.0.5/LICENSE` & `emlvp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/PKG-INFO` & `emlvp-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlvp
-Version: 0.0.5
+Version: 0.0.6
 Summary: EMLvp (validator and parser)
 Home-page: https://github.com/servilla/EMLvp
 Author: Mark Servilla
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -215,38 +215,44 @@
 
 ![EMLvp](https://github.com/PASTAplus/EMLvp/actions/workflows/python-package-conda.yml/badge.svg) ![RTD](https://readthedocs.org/projects/emlvp/badge/?version=latest)
 
 See [this documentation](https://emlvp.readthedocs.io/en/latest/) on "Read the Docs".
 
 ## Introduction
 
-**EMLvp** is a Python 3 library to validate and parse Ecological Metadata Language XML documents for compliance with
-the EML metadata standard. See the
-[EML normative documentation](https://eml.ecoinformatics.org/validation-and-content-references.html) for reference.
-
-The **EMLvp** package is both a command line interface (CLI) application that can be used in a local environment and an
-EML validation and parsing API that may be imported into other Python modules. The CLI application, `emlvp`, is also
-used as a reference implementation for the emlvp API. The EMLvp package API provides three object classes that 1)
-perform XML schema validation - `Validator`, 2) EML compliance parsing - `Parser`, and 3) dereference EML 
+**EMLvp** is a Python 3 library to validate and parse Ecological Metadata
+Language XML documents for compliance with the EML metadata standard,
+including XML schema validation and ensuring that references resolve to
+existing ids. See the [EML normative documentation](https://eml.ecoinformatics.org/validation-and-content-references.html)
+for reference.
+
+The **EMLvp** package is both a command line interface (CLI) application that
+can be used in a local environment and an EML validation and parsing API that
+may be imported into other Python modules. The CLI application, `emlvp`, is
+also used as a reference implementation for the emlvp API. The EMLvp package
+API provides three object classes that 1) perform XML schema validation -
+`Validator`, 2) EML compliance parsing - `Parser`, and 3) dereference EML
 `<references>` elements into their normalized structures  - `Derefencer`.
 
 Compliance includes the following inspections:
  1.  `id` attributes in all elements are unique,
  2.  `references` elements for subject `id`,
  3.  for circular `references` (`references` parent elements with `id` attributes),
  4.  for `system` attribute consistency,
  5.  `customUnit` for STMML definitions,
  6.  parents of `annotation` elements for subject `id` (sans the annotations element),
  7.  `references` attribute of annotation(s) for subject id, and
  8.  `additionalMetadata` `describes` attribute for subject id.
 
-The `emlvp` application accepts an Ecological Metadata Language XML document file as input or a directory containing
-EML XML document files with a “.xml” file extension. Once an EML XML document is identified, the application will
-immediately perform a schema validation inspection followed by EML compliance parsing that verifies the
-document is compliant with rules that go beyond what is possible with XML schema validation (see above).
+The `emlvp` application accepts an Ecological Metadata Language XML document
+file as input or a directory containing EML XML document files with a “.xml”
+file extension. Once an EML XML document is identified, the application will
+immediately perform a schema validation inspection followed by EML compliance
+parsing that verifies the document is compliant with rules that go beyond what
+is possible with XML schema validation (see above).
 
 ## Installation
 
 **EMLvp** may be install using pip: `pip install emlvp`. You may also install from GitHub by cloning the repository
 and then using pip to install **EMLvp** with `setup.py`. The `emlvp` command line application is installed as part
 of the pip installation, as are the XML schema files for EML 2.1.0, 2.1.1, and 2.2.0. **EMPvp** is dependent on the
 following Python packages: `Python` >= 3.10, `lxml` >= 4.9.2, `click` >= 8.1.3, and `daiquiri` >= 3.0.0.
```

### Comparing `emlvp-0.0.5/README.md` & `emlvp-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,44 @@
 
 ![EMLvp](https://github.com/PASTAplus/EMLvp/actions/workflows/python-package-conda.yml/badge.svg) ![RTD](https://readthedocs.org/projects/emlvp/badge/?version=latest)
 
 See [this documentation](https://emlvp.readthedocs.io/en/latest/) on "Read the Docs".
 
 ## Introduction
 
-**EMLvp** is a Python 3 library to validate and parse Ecological Metadata Language XML documents for compliance with
-the EML metadata standard. See the
-[EML normative documentation](https://eml.ecoinformatics.org/validation-and-content-references.html) for reference.
-
-The **EMLvp** package is both a command line interface (CLI) application that can be used in a local environment and an
-EML validation and parsing API that may be imported into other Python modules. The CLI application, `emlvp`, is also
-used as a reference implementation for the emlvp API. The EMLvp package API provides three object classes that 1)
-perform XML schema validation - `Validator`, 2) EML compliance parsing - `Parser`, and 3) dereference EML 
+**EMLvp** is a Python 3 library to validate and parse Ecological Metadata
+Language XML documents for compliance with the EML metadata standard,
+including XML schema validation and ensuring that references resolve to
+existing ids. See the [EML normative documentation](https://eml.ecoinformatics.org/validation-and-content-references.html)
+for reference.
+
+The **EMLvp** package is both a command line interface (CLI) application that
+can be used in a local environment and an EML validation and parsing API that
+may be imported into other Python modules. The CLI application, `emlvp`, is
+also used as a reference implementation for the emlvp API. The EMLvp package
+API provides three object classes that 1) perform XML schema validation -
+`Validator`, 2) EML compliance parsing - `Parser`, and 3) dereference EML
 `<references>` elements into their normalized structures  - `Derefencer`.
 
 Compliance includes the following inspections:
  1.  `id` attributes in all elements are unique,
  2.  `references` elements for subject `id`,
  3.  for circular `references` (`references` parent elements with `id` attributes),
  4.  for `system` attribute consistency,
  5.  `customUnit` for STMML definitions,
  6.  parents of `annotation` elements for subject `id` (sans the annotations element),
  7.  `references` attribute of annotation(s) for subject id, and
  8.  `additionalMetadata` `describes` attribute for subject id.
 
-The `emlvp` application accepts an Ecological Metadata Language XML document file as input or a directory containing
-EML XML document files with a “.xml” file extension. Once an EML XML document is identified, the application will
-immediately perform a schema validation inspection followed by EML compliance parsing that verifies the
-document is compliant with rules that go beyond what is possible with XML schema validation (see above).
+The `emlvp` application accepts an Ecological Metadata Language XML document
+file as input or a directory containing EML XML document files with a “.xml”
+file extension. Once an EML XML document is identified, the application will
+immediately perform a schema validation inspection followed by EML compliance
+parsing that verifies the document is compliant with rules that go beyond what
+is possible with XML schema validation (see above).
 
 ## Installation
 
 **EMLvp** may be install using pip: `pip install emlvp`. You may also install from GitHub by cloning the repository
 and then using pip to install **EMLvp** with `setup.py`. The `emlvp` command line application is installed as part
 of the pip installation, as are the XML schema files for EML 2.1.0, 2.1.1, and 2.2.0. **EMPvp** is dependent on the
 following Python packages: `Python` >= 3.10, `lxml` >= 4.9.2, `click` >= 8.1.3, and `daiquiri` >= 3.0.0.
```

### Comparing `emlvp-0.0.5/setup.cfg` & `emlvp-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/setup.py` & `emlvp-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/changelog.md` & `emlvp-0.0.6/src/emlvp/changelog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # EMLvp change log
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## (0.0.6) 2023-07-21
+### Changed/Fixed
+- Force opening all files as UTF-8 to support Windows
+- Fix scope of summary statistics output
+
 ## (0.0.5) 2023-02-06
 ### Changed/Fixed
 - Apply "black" formatting and "pylint" refactors
 
 ## (0.0.4) 2023-02-02
 ### Changed/Fixed
 - Add version option to emlvp CLI application
```

### Comparing `emlvp-0.0.5/src/emlvp/dereferencer.py` & `emlvp-0.0.6/src/emlvp/dereferencer.py`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/emlvp_cli.py` & `emlvp-0.0.6/src/emlvp/emlvp_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     return xml
 
 
 def process_one_document(
     doc: str, dereference: bool, fail_fast: bool, pretty_print: bool, verbose: int
 ):
-    with open(doc, "r") as f:
+    with open(doc, "r", encoding="utf-8") as f:
         xml = f.read()
         try:
             xml = vpd(xml, dereference, fail_fast, pretty_print)
             if verbose >= 1:
                 print(f"{doc}\n")
                 if verbose >= 2:
                     print(xml)
@@ -173,16 +173,16 @@
                     )
                 except EMLVPError:
                     docs_with_exceptions += 1
         else:
             logger.error(f"Target {t} is not a file or directory")
             sys.exit(1)
 
-        if statistics:
-            print(f"Total documents validated: {docs_processed}")
-            print(f"Documents that failed validation: {docs_with_exceptions}")
+    if statistics:
+        print(f"Total documents validated: {docs_processed}")
+        print(f"Documents that failed validation: {docs_with_exceptions}")
 
     return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `emlvp-0.0.5/src/emlvp/exceptions.py` & `emlvp-0.0.6/src/emlvp/exceptions.py`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/parser.py` & `emlvp-0.0.6/src/emlvp/parser.py`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-access.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-access.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-entity.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-entity.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-literature.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-literature.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-methods.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-methods.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-party.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-party.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-physical.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-physical.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-project.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-project.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-resource.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-resource.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-software.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-software.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-text.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-text.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml-view.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml-view.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/eml.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/eml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.0/stmml.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.0/stmml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-access.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-access.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-entity.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-entity.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-literature.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-literature.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-methods.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-methods.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-party.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-party.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-physical.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-physical.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-project.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-project.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-resource.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-resource.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-software.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-software.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-text.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-text.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml-view.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml-view.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/eml.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/eml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.1.1/stmml.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.1.1/stmml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd` & `emlvp-0.0.6/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp/validator.py` & `emlvp-0.0.6/src/emlvp/validator.py`

 * *Files identical despite different names*

### Comparing `emlvp-0.0.5/src/emlvp.egg-info/PKG-INFO` & `emlvp-0.0.6/src/emlvp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlvp
-Version: 0.0.5
+Version: 0.0.6
 Summary: EMLvp (validator and parser)
 Home-page: https://github.com/servilla/EMLvp
 Author: Mark Servilla
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -215,38 +215,44 @@
 
 ![EMLvp](https://github.com/PASTAplus/EMLvp/actions/workflows/python-package-conda.yml/badge.svg) ![RTD](https://readthedocs.org/projects/emlvp/badge/?version=latest)
 
 See [this documentation](https://emlvp.readthedocs.io/en/latest/) on "Read the Docs".
 
 ## Introduction
 
-**EMLvp** is a Python 3 library to validate and parse Ecological Metadata Language XML documents for compliance with
-the EML metadata standard. See the
-[EML normative documentation](https://eml.ecoinformatics.org/validation-and-content-references.html) for reference.
-
-The **EMLvp** package is both a command line interface (CLI) application that can be used in a local environment and an
-EML validation and parsing API that may be imported into other Python modules. The CLI application, `emlvp`, is also
-used as a reference implementation for the emlvp API. The EMLvp package API provides three object classes that 1)
-perform XML schema validation - `Validator`, 2) EML compliance parsing - `Parser`, and 3) dereference EML 
+**EMLvp** is a Python 3 library to validate and parse Ecological Metadata
+Language XML documents for compliance with the EML metadata standard,
+including XML schema validation and ensuring that references resolve to
+existing ids. See the [EML normative documentation](https://eml.ecoinformatics.org/validation-and-content-references.html)
+for reference.
+
+The **EMLvp** package is both a command line interface (CLI) application that
+can be used in a local environment and an EML validation and parsing API that
+may be imported into other Python modules. The CLI application, `emlvp`, is
+also used as a reference implementation for the emlvp API. The EMLvp package
+API provides three object classes that 1) perform XML schema validation -
+`Validator`, 2) EML compliance parsing - `Parser`, and 3) dereference EML
 `<references>` elements into their normalized structures  - `Derefencer`.
 
 Compliance includes the following inspections:
  1.  `id` attributes in all elements are unique,
  2.  `references` elements for subject `id`,
  3.  for circular `references` (`references` parent elements with `id` attributes),
  4.  for `system` attribute consistency,
  5.  `customUnit` for STMML definitions,
  6.  parents of `annotation` elements for subject `id` (sans the annotations element),
  7.  `references` attribute of annotation(s) for subject id, and
  8.  `additionalMetadata` `describes` attribute for subject id.
 
-The `emlvp` application accepts an Ecological Metadata Language XML document file as input or a directory containing
-EML XML document files with a “.xml” file extension. Once an EML XML document is identified, the application will
-immediately perform a schema validation inspection followed by EML compliance parsing that verifies the
-document is compliant with rules that go beyond what is possible with XML schema validation (see above).
+The `emlvp` application accepts an Ecological Metadata Language XML document
+file as input or a directory containing EML XML document files with a “.xml”
+file extension. Once an EML XML document is identified, the application will
+immediately perform a schema validation inspection followed by EML compliance
+parsing that verifies the document is compliant with rules that go beyond what
+is possible with XML schema validation (see above).
 
 ## Installation
 
 **EMLvp** may be install using pip: `pip install emlvp`. You may also install from GitHub by cloning the repository
 and then using pip to install **EMLvp** with `setup.py`. The `emlvp` command line application is installed as part
 of the pip installation, as are the XML schema files for EML 2.1.0, 2.1.1, and 2.2.0. **EMPvp** is dependent on the
 following Python packages: `Python` >= 3.10, `lxml` >= 4.9.2, `click` >= 8.1.3, and `daiquiri` >= 3.0.0.
```

### Comparing `emlvp-0.0.5/src/emlvp.egg-info/SOURCES.txt` & `emlvp-0.0.6/src/emlvp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,8 +95,11 @@
 src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd
 src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd
 src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd
 src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd
 src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd
 src/emlvp/schemas/EML2.2.0/xsd/eml.xsd
 src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd
-src/emlvp/schemas/EML2.2.0/xsd/xml.xsd
+src/emlvp/schemas/EML2.2.0/xsd/xml.xsd
+tests/test_dereferencer.py
+tests/test_parser.py
+tests/test_validator.py
```

