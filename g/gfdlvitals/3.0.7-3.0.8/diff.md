# Comparing `tmp/gfdlvitals-3.0.7.tar.gz` & `tmp/gfdlvitals-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfdlvitals-3.0.7.tar", last modified: Sat Mar 11 22:18:43 2023, max compression
+gzip compressed data, was "gfdlvitals-3.0.8.tar", last modified: Sat Jul 22 12:14:33 2023, max compression
```

## Comparing `gfdlvitals-3.0.7.tar` & `gfdlvitals-3.0.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.425490 gfdlvitals-3.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-11 22:18:43.425490 gfdlvitals-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.413489 gfdlvitals-3.0.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.417490 gfdlvitals-3.0.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.417490 gfdlvitals-3.0.7/gfdlvitals/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.417490 gfdlvitals-3.0.7/gfdlvitals/averagers/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/averagers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/averagers/cubesphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/averagers/ice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/averagers/land_lm3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/averagers/land_lm4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/averagers/latlon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/averagers/tripolar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5132 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.417490 gfdlvitals-3.0.7/gfdlvitals/diags/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/diags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/diags/amoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/diags/fms.py
--rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/diags/m6toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.417490 gfdlvitals-3.0.7/gfdlvitals/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2888 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/models/CM4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2054 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/models/ESM2.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.417490 gfdlvitals-3.0.7/gfdlvitals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    15915 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/LM3_variable_dictionary.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.417490 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.421490 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171072 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   177120 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   170348 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   174520 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   173516 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   170012 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   176184 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171656 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   176428 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171272 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171500 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   175872 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.425490 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   169352 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   175420 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   174736 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   167568 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   174908 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   169848 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/historical.db
--rw-r--r--   0 runner    (1001) docker     (123)    23552 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/resources/picontrol.db
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.425490 gfdlvitals-3.0.7/gfdlvitals/util/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/util/average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/util/extract_ocean_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/util/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/util/gmeantools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/util/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/util/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/util/xrtools.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/gfdlvitals/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.417490 gfdlvitals-3.0.7/gfdlvitals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-11 22:18:43.000000 gfdlvitals-3.0.7/gfdlvitals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-11 22:18:43.000000 gfdlvitals-3.0.7/gfdlvitals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 22:18:43.000000 gfdlvitals-3.0.7/gfdlvitals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 22:18:43.000000 gfdlvitals-3.0.7/gfdlvitals.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-11 22:18:43.000000 gfdlvitals-3.0.7/gfdlvitals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-11 22:18:43.000000 gfdlvitals-3.0.7/gfdlvitals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 22:18:43.425490 gfdlvitals-3.0.7/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5807 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/scripts/db2nc
--rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/scripts/gfdlvitals
--rwxr-xr-x   0 runner    (1001) docker     (123)     1645 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/scripts/plotdb
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-11 22:18:43.425490 gfdlvitals-3.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-11 22:18:33.000000 gfdlvitals-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.649264 gfdlvitals-3.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-22 12:14:33.649264 gfdlvitals-3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.621263 gfdlvitals-3.0.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.625264 gfdlvitals-3.0.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.629263 gfdlvitals-3.0.8/gfdlvitals/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.633263 gfdlvitals-3.0.8/gfdlvitals/averagers/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/averagers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/averagers/cubesphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/averagers/ice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/averagers/land_lm3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/averagers/land_lm4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/averagers/latlon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/averagers/tripolar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5132 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.633263 gfdlvitals-3.0.8/gfdlvitals/diags/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/diags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/diags/amoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/diags/fms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/diags/m6toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18598 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.633263 gfdlvitals-3.0.8/gfdlvitals/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2888 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/models/CM4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2054 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/models/ESM2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.633263 gfdlvitals-3.0.8/gfdlvitals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    15915 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/LM3_variable_dictionary.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.625264 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.641264 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   171072 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   177120 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   170348 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   174520 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   173516 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   170012 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   176184 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171656 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   176428 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171272 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171500 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   175872 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.645264 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   169352 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   175420 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   174736 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   167568 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   174908 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   169848 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/historical.db
+-rw-r--r--   0 runner    (1001) docker     (123)    23552 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/resources/picontrol.db
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.645264 gfdlvitals-3.0.8/gfdlvitals/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/util/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/util/extract_ocean_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/util/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/util/gmeantools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/util/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/util/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/util/xrtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/gfdlvitals/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.629263 gfdlvitals-3.0.8/gfdlvitals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-22 12:14:33.000000 gfdlvitals-3.0.8/gfdlvitals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-22 12:14:33.000000 gfdlvitals-3.0.8/gfdlvitals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 12:14:33.000000 gfdlvitals-3.0.8/gfdlvitals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 12:14:33.000000 gfdlvitals-3.0.8/gfdlvitals.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-22 12:14:33.000000 gfdlvitals-3.0.8/gfdlvitals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 12:14:33.000000 gfdlvitals-3.0.8/gfdlvitals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:14:33.649264 gfdlvitals-3.0.8/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5807 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/scripts/db2nc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/scripts/gfdlvitals
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1645 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/scripts/plotdb
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-22 12:14:33.649264 gfdlvitals-3.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-22 12:14:16.000000 gfdlvitals-3.0.8/setup.py
```

### Comparing `gfdlvitals-3.0.7/PKG-INFO` & `gfdlvitals-3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfdlvitals
-Version: 3.0.7
+Version: 3.0.8
 Summary: Tools for calculating scalar diagnostics from GFDL models
 Home-page: https://github.com/jkrasting/gfdlvitals
 Author: John Krasting
 Author-email: john.krasting@noaa.gov
 Keywords: climate model analysis scalar diagnostics gfdl AM4 CM4 ESM4 OM4 LM4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gfdlvitals-3.0.7/docs/source/conf.py` & `gfdlvitals-3.0.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/averagers/cubesphere.py` & `gfdlvitals-3.0.8/gfdlvitals/averagers/cubesphere.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/averagers/ice.py` & `gfdlvitals-3.0.8/gfdlvitals/averagers/ice.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/averagers/land_lm3.py` & `gfdlvitals-3.0.8/gfdlvitals/averagers/land_lm3.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/averagers/land_lm4.py` & `gfdlvitals-3.0.8/gfdlvitals/averagers/land_lm4.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/averagers/latlon.py` & `gfdlvitals-3.0.8/gfdlvitals/averagers/latlon.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/averagers/tripolar.py` & `gfdlvitals-3.0.8/gfdlvitals/averagers/tripolar.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/cli.py` & `gfdlvitals-3.0.8/gfdlvitals/cli.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/diags/amoc.py` & `gfdlvitals-3.0.8/gfdlvitals/diags/amoc.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/diags/fms.py` & `gfdlvitals-3.0.8/gfdlvitals/diags/fms.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/diags/m6toolbox.py` & `gfdlvitals-3.0.8/gfdlvitals/diags/m6toolbox.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/extensions.py` & `gfdlvitals-3.0.8/gfdlvitals/extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
         self
             Extended dataset
         """
         endyear = tuple(self.index[-1].timetuple())
         padding = np.arange(1, maxlen - len(self.index) + 1) + endyear[0]
         added_index = [cftime.DatetimeNoLeap(x, *endyear[1:]) for x in padding]
         _df = pd.DataFrame({"times": added_index}).set_index("times")
-        _df = self.append(_df)
+        _df = pd.concat([self,_df])
         _df.attrs = self.attrs
         for column in self.columns:
             _df[column].attrs = self[column].attrs
         return _df
 
     def detrend(self, reference=None, order=1, anomaly=True, return_coefs=False):
         """Detrend VitalsDataFrame object
```

### Comparing `gfdlvitals-3.0.7/gfdlvitals/models/CM4.py` & `gfdlvitals-3.0.8/gfdlvitals/models/CM4.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/models/ESM2.py` & `gfdlvitals-3.0.8/gfdlvitals/models/ESM2.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/plot.py` & `gfdlvitals-3.0.8/gfdlvitals/plot.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/LM3_variable_dictionary.pkl` & `gfdlvitals-3.0.8/gfdlvitals/resources/LM3_variable_dictionary.pkl`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/LICENSE.txt` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Black.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-BlackItalic.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Bold.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-BoldItalic.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Italic.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Light.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-LightItalic.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Medium.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-MediumItalic.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Regular.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-Thin.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto/Roboto-ThinItalic.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/LICENSE.txt` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Bold.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Bold.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-BoldItalic.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Italic.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Italic.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Light.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Light.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-LightItalic.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Regular.ttf` & `gfdlvitals-3.0.8/gfdlvitals/resources/fonts/Roboto_Condensed/RobotoCondensed-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/historical.db` & `gfdlvitals-3.0.8/gfdlvitals/resources/historical.db`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/resources/picontrol.db` & `gfdlvitals-3.0.8/gfdlvitals/resources/picontrol.db`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/util/average.py` & `gfdlvitals-3.0.8/gfdlvitals/util/average.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/util/extract_ocean_scalar.py` & `gfdlvitals-3.0.8/gfdlvitals/util/extract_ocean_scalar.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/util/git.py` & `gfdlvitals-3.0.8/gfdlvitals/util/git.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/util/gmeantools.py` & `gfdlvitals-3.0.8/gfdlvitals/util/gmeantools.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/util/merge.py` & `gfdlvitals-3.0.8/gfdlvitals/util/merge.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/util/netcdf.py` & `gfdlvitals-3.0.8/gfdlvitals/util/netcdf.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals/util/xrtools.py` & `gfdlvitals-3.0.8/gfdlvitals/util/xrtools.py`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/gfdlvitals.egg-info/PKG-INFO` & `gfdlvitals-3.0.8/gfdlvitals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfdlvitals
-Version: 3.0.7
+Version: 3.0.8
 Summary: Tools for calculating scalar diagnostics from GFDL models
 Home-page: https://github.com/jkrasting/gfdlvitals
 Author: John Krasting
 Author-email: john.krasting@noaa.gov
 Keywords: climate model analysis scalar diagnostics gfdl AM4 CM4 ESM4 OM4 LM4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gfdlvitals-3.0.7/gfdlvitals.egg-info/SOURCES.txt` & `gfdlvitals-3.0.8/gfdlvitals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/scripts/db2nc` & `gfdlvitals-3.0.8/scripts/db2nc`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/scripts/plotdb` & `gfdlvitals-3.0.8/scripts/plotdb`

 * *Files identical despite different names*

### Comparing `gfdlvitals-3.0.7/setup.cfg` & `gfdlvitals-3.0.8/setup.cfg`

 * *Files identical despite different names*

