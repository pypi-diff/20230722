# Comparing `tmp/tendril-utils-db-0.5.3.tar.gz` & `tmp/tendril-utils-db-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-utils-db-0.5.3.tar", last modified: Mon Jun 26 17:47:36 2023, max compression
+gzip compressed data, was "tendril-utils-db-0.5.4.tar", last modified: Sat Jul 22 18:11:09 2023, max compression
```

## Comparing `tendril-utils-db-0.5.3.tar` & `tendril-utils-db-0.5.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.613386 tendril-utils-db-0.5.3/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-06-26 17:47:36.613386 tendril-utils-db-0.5.3/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2205 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/README.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2109 2022-12-08 14:04:07.000000 tendril-utils-db-0.5.3/alembic.ini
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13493 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      869 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1643 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-06-26 17:47:36.613386 tendril-utils-db-0.5.3/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3310 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.3/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.605386 tendril-utils-db-0.5.3/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:40.000000 tendril-utils-db-0.5.3/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2812 2023-03-28 18:11:09.000000 tendril-utils-db-0.5.3/src/tendril/config/db.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1599 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.3/src/tendril/config/db_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.3/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.3/src/tendril/db/controllers/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/src/tendril/db/migration/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.3/src/tendril/db/migration/README
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.3/src/tendril/db/migration/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2206 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.3/src/tendril/db/migration/env.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      494 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.3/src/tendril/db/migration/script.py.mako
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/src/tendril/db/migration/versions/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.3/src/tendril/db/migration/versions/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.609386 tendril-utils-db-0.5.3/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.3/src/tendril/db/models/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.613386 tendril-utils-db-0.5.3/src/tendril/utils/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:49.000000 tendril-utils-db-0.5.3/src/tendril/utils/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    10349 2023-06-26 17:46:53.000000 tendril-utils-db-0.5.3/src/tendril/utils/db.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.613386 tendril-utils-db-0.5.3/src/tendril_utils_db.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-06-26 17:47:36.000000 tendril-utils-db-0.5.3/src/tendril_utils_db.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1089 2023-06-26 17:47:36.000000 tendril-utils-db-0.5.3/src/tendril_utils_db.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-06-26 17:47:36.000000 tendril-utils-db-0.5.3/src/tendril_utils_db.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      763 2023-06-26 17:47:36.000000 tendril-utils-db-0.5.3/src/tendril_utils_db.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-06-26 17:47:36.000000 tendril-utils-db-0.5.3/src/tendril_utils_db.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 17:47:36.613386 tendril-utils-db-0.5.3/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.3/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.685383 tendril-utils-db-0.5.4/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-07-22 18:11:09.685383 tendril-utils-db-0.5.4/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2205 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/README.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2109 2022-12-08 14:04:07.000000 tendril-utils-db-0.5.4/alembic.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13493 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      869 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1643 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-22 18:11:09.685383 tendril-utils-db-0.5.4/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3310 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.4/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:40.000000 tendril-utils-db-0.5.4/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2812 2023-03-28 18:11:09.000000 tendril-utils-db-0.5.4/src/tendril/config/db.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1599 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.4/src/tendril/config/db_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.4/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.681383 tendril-utils-db-0.5.4/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.4/src/tendril/db/controllers/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.685383 tendril-utils-db-0.5.4/src/tendril/db/migration/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.4/src/tendril/db/migration/README
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.4/src/tendril/db/migration/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2206 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.4/src/tendril/db/migration/env.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      494 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.4/src/tendril/db/migration/script.py.mako
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.685383 tendril-utils-db-0.5.4/src/tendril/db/migration/versions/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.4/src/tendril/db/migration/versions/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.685383 tendril-utils-db-0.5.4/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.4/src/tendril/db/models/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.685383 tendril-utils-db-0.5.4/src/tendril/utils/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:49.000000 tendril-utils-db-0.5.4/src/tendril/utils/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    10762 2023-07-22 17:41:47.000000 tendril-utils-db-0.5.4/src/tendril/utils/db.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.685383 tendril-utils-db-0.5.4/src/tendril_utils_db.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-07-22 18:11:09.000000 tendril-utils-db-0.5.4/src/tendril_utils_db.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1089 2023-07-22 18:11:09.000000 tendril-utils-db-0.5.4/src/tendril_utils_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-22 18:11:09.000000 tendril-utils-db-0.5.4/src/tendril_utils_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      763 2023-07-22 18:11:09.000000 tendril-utils-db-0.5.4/src/tendril_utils_db.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-22 18:11:09.000000 tendril-utils-db-0.5.4/src/tendril_utils_db.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-22 18:11:09.685383 tendril-utils-db-0.5.4/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.4/tox.ini
```

### Comparing `tendril-utils-db-0.5.3/.gitignore` & `tendril-utils-db-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/.readthedocs.yml` & `tendril-utils-db-0.5.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/.travis.yml` & `tendril-utils-db-0.5.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/LICENSE` & `tendril-utils-db-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/PKG-INFO` & `tendril-utils-db-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-db
-Version: 0.5.3
+Version: 0.5.4
 Summary: Database utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-db
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-db.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-db/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-db
```

### Comparing `tendril-utils-db-0.5.3/README.rst` & `tendril-utils-db-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/alembic.ini` & `tendril-utils-db-0.5.4/alembic.ini`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/docs/Makefile` & `tendril-utils-db-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/docs/_static/custom.css` & `tendril-utils-db-0.5.4/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/docs/_static/favicon.ico` & `tendril-utils-db-0.5.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/docs/_static/logo.png` & `tendril-utils-db-0.5.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/docs/_static/logo_packed.png` & `tendril-utils-db-0.5.4/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/docs/_templates/about.html` & `tendril-utils-db-0.5.4/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/docs/conf.py` & `tendril-utils-db-0.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/docs/index.rst` & `tendril-utils-db-0.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/docs/installation.rst` & `tendril-utils-db-0.5.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/setup.py` & `tendril-utils-db-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/src/tendril/config/__init__.py` & `tendril-utils-db-0.5.4/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/src/tendril/config/db.py` & `tendril-utils-db-0.5.4/src/tendril/config/db.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/src/tendril/config/db_core.py` & `tendril-utils-db-0.5.4/src/tendril/config/db_core.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/src/tendril/db/migration/env.py` & `tendril-utils-db-0.5.4/src/tendril/db/migration/env.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/src/tendril/utils/db.py` & `tendril-utils-db-0.5.4/src/tendril/utils/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 contents of this utility module simplify and specify the application code's
 interaction with :mod:`sqlalchemy`
 
 .. rubric:: Module Contents
 
 """
 
+import json
 import importlib
+from decimal import Decimal
 from sqlalchemy import MetaData
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy import Column, Integer
 from sqlalchemy_utils import ArrowType
@@ -63,15 +65,29 @@
     defined by the :mod:`tendril.config` module.
 
     This function is called within the module and an engine is readily
     available in the module variable :data:`tendril.utils.db.engine`.
     Application code should not have to create a new engine for normal
     use cases.
     """
-    return create_engine(DATABASE_URI)
+
+    def _default(val):
+        if isinstance(val, Decimal):
+            return str(val)
+        raise TypeError()
+
+    def dumps(d):
+        return json.dumps(d, default=_default)
+
+    def loads(*args, **kwgs):
+        return json.loads(*args, parse_float=Decimal, **kwgs)
+
+    return create_engine(DATABASE_URI,
+                         json_serializer=dumps,
+                         json_deserializer=loads)
 
 
 #: The :class:`sqlalchemy.Engine` object
 engine = init_db_engine()
 
 #: The :class:`sqlalchemy.sessionmaker` bound to the database engine
 Session = sessionmaker(expire_on_commit=False)
```

### Comparing `tendril-utils-db-0.5.3/src/tendril_utils_db.egg-info/PKG-INFO` & `tendril-utils-db-0.5.4/src/tendril_utils_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-db
-Version: 0.5.3
+Version: 0.5.4
 Summary: Database utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-db
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-db.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-db/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-db
```

### Comparing `tendril-utils-db-0.5.3/src/tendril_utils_db.egg-info/SOURCES.txt` & `tendril-utils-db-0.5.4/src/tendril_utils_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/src/tendril_utils_db.egg-info/requires.txt` & `tendril-utils-db-0.5.4/src/tendril_utils_db.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/tests/coveralls.py` & `tendril-utils-db-0.5.4/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.3/tox.ini` & `tendril-utils-db-0.5.4/tox.ini`

 * *Files identical despite different names*

