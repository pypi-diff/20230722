# Comparing `tmp/UW-RestClients-AdSel-1.9.tar.gz` & `tmp/UW-RestClients-AdSel-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-AdSel-1.9.tar", last modified: Thu Jul 28 01:08:57 2022, max compression
+gzip compressed data, was "UW-RestClients-AdSel-1.9.1.tar", last modified: Fri Jul 21 23:25:07 2023, max compression
```

## Comparing `UW-RestClients-AdSel-1.9.tar` & `UW-RestClients-AdSel-1.9.1.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.507911 UW-RestClients-AdSel-1.9/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       53 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      662 2022-07-28 01:08:57.507911 UW-RestClients-AdSel-1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/UW_RestClients_AdSel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      662 2022-07-28 01:08:57.000000 UW-RestClients-AdSel-1.9/UW_RestClients_AdSel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2335 2022-07-28 01:08:57.000000 UW-RestClients-AdSel-1.9/UW_RestClients_AdSel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-28 01:08:57.000000 UW-RestClients-AdSel-1.9/UW_RestClients_AdSel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       50 2022-07-28 01:08:57.000000 UW-RestClients-AdSel-1.9/UW_RestClients_AdSel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-07-28 01:08:57.000000 UW-RestClients-AdSel-1.9/UW_RestClients_AdSel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-07-28 01:08:57.507911 UW-RestClients-AdSel-1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1329 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/
--rw-r--r--   0 runner    (1001) docker     (116)        4 2022-07-28 01:08:56.000000 UW-RestClients-AdSel-1.9/uw_adsel/VERSION
--rw-r--r--   0 runner    (1001) docker     (116)    19783 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      332 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/dao.py
--rw-r--r--   0 runner    (1001) docker     (116)       64 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    10202 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.499910 UW-RestClients-AdSel-1.9/uw_adsel/resources/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.499910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.499910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.499910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/
--rw-r--r--   0 runner    (1001) docker     (116)      406 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/academicqtr
--rw-r--r--   0 runner    (1001) docker     (116)     1883 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/activities
--rw-r--r--   0 runner    (1001) docker     (116)      503 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/activities?Page=2
--rw-r--r--   0 runner    (1001) docker     (116)      502 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/activities?assignmentType=major
--rw-r--r--   0 runner    (1001) docker     (116)      938 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage
--rw-r--r--   0 runner    (1001) docker     (116)     1772 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/
--rw-r--r--   0 runner    (1001) docker     (116)     1234 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/
--rw-r--r--   0 runner    (1001) docker     (116)      368 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/0
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/major/
--rw-r--r--   0 runner    (1001) docker     (116)      568 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/major/1
--rw-r--r--   0 runner    (1001) docker     (116)      599 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/major/2
--rw-r--r--   0 runner    (1001) docker     (116)     3079 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/majors
--rw-r--r--   0 runner    (1001) docker     (116)     2738 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/applications/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/applications/0/
--rw-r--r--   0 runner    (1001) docker     (116)     1019 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/applications/0/123
--rw-r--r--   0 runner    (1001) docker     (116)     1023 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/applications/0/all
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/
--rw-r--r--   0 runner    (1001) docker     (116)     2073 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/assignments/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.507911 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/
--rw-r--r--   0 runner    (1001) docker     (116)      310 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/bulk
--rw-r--r--   0 runner    (1001) docker     (116)      306 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/assignments/departmentalDecision
--rw-r--r--   0 runner    (1001) docker     (116)      310 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/assignments/major
--rw-r--r--   0 runner    (1001) docker     (116)      310 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/assignments/purpleAndGold
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.507911 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/cohorts/
--rw-r--r--   0 runner    (1001) docker     (116)      711 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/cohorts/0
--rw-r--r--   0 runner    (1001) docker     (116)      700 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2
--rw-r--r--   0 runner    (1001) docker     (116)      709 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/cohorts/1
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.507911 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/
--rw-r--r--   0 runner    (1001) docker     (116)     1508 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0
--rw-r--r--   0 runner    (1001) docker     (116)     1509 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1
--rw-r--r--   0 runner    (1001) docker     (116)     3477 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/filter
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.503910 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.507911 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.507911 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/0/
--rw-r--r--   0 runner    (1001) docker     (116)      312 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_BIOL_1
--rw-r--r--   0 runner    (1001) docker     (116)      286 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CHEM_1
--rw-r--r--   0 runner    (1001) docker     (116)      328 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CSE_1
--rw-r--r--   0 runner    (1001) docker     (116)     1040 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100
--rw-r--r--   0 runner    (1001) docker     (116)      978 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100
--rw-r--r--   0 runner    (1001) docker     (116)      969 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100
--rw-r--r--   0 runner    (1001) docker     (116)      382 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:57.507911 UW-RestClients-AdSel-1.9/uw_adsel/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10907 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/tests/test_adsel.py
--rw-r--r--   0 runner    (1001) docker     (116)      119 2022-07-28 01:08:41.000000 UW-RestClients-AdSel-1.9/uw_adsel/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-21 23:25:05.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)    20643 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10671 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/academicqtr
+-rw-r--r--   0 runner    (1001) docker     (122)     1883 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?Page=2
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?assignmentType=major
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage
+-rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/0
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/1
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/2
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/majors
+-rw-r--r--   0 runner    (1001) docker     (122)     2738 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/123
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/all
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/
+-rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/bulk
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/departmentalDecision
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/major
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/purpleAndGold
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/0
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/1
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1
+-rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/filter
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_BIOL_1
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CHEM_1
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CSE_1
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/workspaces/20194
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/uw_adsel/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11871 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/tests/test_adsel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/utilities.py
```

### Comparing `UW-RestClients-AdSel-1.9/LICENSE` & `UW-RestClients-AdSel-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/PKG-INFO` & `UW-RestClients-AdSel-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-AdSel
-Version: 1.9
+Version: 1.9.1
 Summary: A library for connecting to the AdSel API at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-adsel
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 
 
 See the README on `GitHub
 <https://github.com/uw-it-aca/uw-restclients-adsel>`_.
-
-
```

### Comparing `UW-RestClients-AdSel-1.9/README.md` & `UW-RestClients-AdSel-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/UW_RestClients_AdSel.egg-info/PKG-INFO` & `UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-AdSel
-Version: 1.9
+Version: 1.9.1
 Summary: A library for connecting to the AdSel API at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-adsel
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 
 
 See the README on `GitHub
 <https://github.com/uw-it-aca/uw-restclients-adsel>`_.
-
-
```

### Comparing `UW-RestClients-AdSel-1.9/UW_RestClients_AdSel.egg-info/SOURCES.txt` & `UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,9 +41,10 @@
 uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1
 uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100
 uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100
 uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100
 uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_BIOL_1
 uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CHEM_1
 uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CSE_1
+uw_adsel/resources/adsel/file/api/v1/workspaces/20194
 uw_adsel/tests/__init__.py
 uw_adsel/tests/test_adsel.py
```

### Comparing `UW-RestClients-AdSel-1.9/setup.py` & `UW-RestClients-AdSel-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/__init__.py` & `UW-RestClients-AdSel-1.9.1/uw_adsel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import json
 import logging
 from restclients_core.exceptions import DataFailureException
 from restclients_core.dao import MockDAO
 from uw_adsel.dao import ADSEL_DAO
 from uw_adsel.models import Major, Cohort, Quarter, Activity, Application, \
-    Decision, AdminMajor, AdminCohort
+    Decision, AdminMajor, AdminCohort, Workspace
 import dateutil.parser
 from datetime import datetime
 import urllib.parse
 
 
 logger = logging.getLogger(__name__)
 
@@ -421,14 +421,34 @@
         params = {k: v for k, v in filters.items() if v is not None}
         filter_url = urllib.parse.urlencode(params)
         if len(filter_url) > 0:
             url = url + "?" + filter_url
         response = self._get_resource(url)
         return response
 
+    def create_workspace(self, workspace):
+        url = "{}/admin/workspace".format(self.API)
+        return self._post_resource(url, workspace.json_data())
+
+    def get_workspaces_by_qtr(self, qtr):
+        url = "{}/workspaces/{}".format(self.API, qtr)
+        response = self._get_resource(url)
+        workspaces = self._workspaces_from_json(response)
+        return workspaces
+
+    def _workspaces_from_json(self, response):
+        workspaces = []
+        for workspace in response:
+            json_data = {'academic_qtr_id': workspace['academicQtrKeyId'],
+                         'workspace_id': workspace['workspaceId'],
+                         'workspace_name': workspace['workspaceName'],
+                         'owner_alias': workspace['ownerAlias']}
+            workspaces.append(Workspace(**json_data))
+        return workspaces
+
     def _get_resource(self, url):
         response = self.DAO.getURL(url, self._headers())
 
         if response.status != 200:
             self._log_error(url, response)
             raise DataFailureException(url, response.status, response.data)
```

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/models.py` & `UW-RestClients-AdSel-1.9.1/uw_adsel/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,7 +247,22 @@
             "admitDecision": self.admit_decision,
             "protectedGroupInd": self.protected_group,
             "enforceExceptionsInd": self.enforce_exceptions,
             "activeCohortInd": self.active_cohort,
             "recordUpdateDateTime": self.record_updated,
             "recordUpdateUser": self.record_update_user
         }
+
+
+class Workspace(models.Model):
+    academic_qtr_id = models.IntegerField()
+    workspace_id = models.IntegerField()
+    workspace_name = models.CharField(max_length=255)
+    owner_alias = models.CharField(max_length=255)
+
+    def json_data(self):
+        return {
+            "academicQtrKeyId": self.academic_qtr_id,
+            "workspaceId": self.workspace_id,
+            "workspaceName": self.workspace_name,
+            "ownerAlias": self.owner_alias
+        }
```

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/activities` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/major/1` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/1`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/major/2` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/2`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/majors` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/majors`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/applications/0/123` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/123`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/applications/0/all` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/all`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/cohorts/0` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/cohorts/1` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/1`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/filter` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/filter`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100` & `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9/uw_adsel/tests/test_adsel.py` & `UW-RestClients-AdSel-1.9.1/uw_adsel/tests/test_adsel.py`

 * *Files 6% similar despite different names*

```diff
@@ -267,7 +267,34 @@
     def test_filter_values(self):
         client = AdSel()
         filters = client.get_filter_values()
         self.assertEqual(len(filters), 15)
         self.assertEqual(len(filters['internationalScores'].items()), 12)
         with self.assertRaises(DataFailureException):
             client.get_filter_values(year=2022)
+
+    def test_workspaces_from_json(self):
+        json = [
+            {
+                "academicQtrKeyId": 20194,
+                "workspaceId": 1,
+                "workspaceName": "My Workspace",
+                "ownerAlias": "javerage"
+            },
+            {
+                "academicQtrKeyId": 20194,
+                "workspaceId": 2,
+                "workspaceName": "Demo Workspace",
+                "ownerAlias": "javerage"
+            }
+        ]
+
+        workspaces = AdSel()._workspaces_from_json(json)
+        self.assertEqual(len(workspaces), 2)
+        self.assertEqual(workspaces[0].workspace_id, 1)
+        self.assertEqual(workspaces[0].workspace_name, "My Workspace")
+        self.assertEqual(workspaces[0].owner_alias, "javerage")
+        self.assertEqual(workspaces[0].academic_qtr_id, 20194)
+
+    def test_get_worspaces_by_qtr(self):
+        workspaces = AdSel().get_workspaces_by_qtr(20194)
+        self.assertEqual(len(workspaces), 9)
```

