# Comparing `tmp/django-cachalot-2.6.0.tar.gz` & `tmp/django-cachalot-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cachalot-2.6.0.tar", last modified: Fri Jul 21 09:55:41 2023, max compression
+gzip compressed data, was "django-cachalot-2.6.1.tar", last modified: Fri Jul 21 22:32:47 2023, max compression
```

## Comparing `django-cachalot-2.6.0.tar` & `django-cachalot-2.6.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/admin_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/admin_tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/admin_tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/jinja2ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/management/commands/invalidate_cachalot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/panels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.076571 django-cachalot-2.6.0/cachalot/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/templates/cachalot/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/templates/cachalot/panel.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.080571 django-cachalot-2.6.0/cachalot/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/templatetags/cachalot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.084571 django-cachalot-2.6.0/cachalot/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/db_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/debug_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/loaddata_fixture.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.084571 django-cachalot-2.6.0/cachalot/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/multi_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    51433 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/tests_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/thread_safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    39198 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/tests/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/cachalot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/django_cachalot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 09:55:41.000000 django-cachalot-2.6.0/django_cachalot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/how.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/legacy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/limits.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/reporting.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/docs/todo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/runtests_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:55:41.088571 django-cachalot-2.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1446 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-21 09:55:30.000000 django-cachalot-2.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.440322 django-cachalot-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-21 22:32:47.440322 django-cachalot-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.432321 django-cachalot-2.6.1/cachalot/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.432321 django-cachalot-2.6.1/cachalot/admin_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/admin_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/admin_tests/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.432321 django-cachalot-2.6.1/cachalot/admin_tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/admin_tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/admin_tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/admin_tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/admin_tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/jinja2ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.432321 django-cachalot-2.6.1/cachalot/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.432321 django-cachalot-2.6.1/cachalot/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/management/commands/invalidate_cachalot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.432321 django-cachalot-2.6.1/cachalot/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.432321 django-cachalot-2.6.1/cachalot/templates/cachalot/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/templates/cachalot/panel.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.436322 django-cachalot-2.6.1/cachalot/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/templatetags/cachalot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.436322 django-cachalot-2.6.1/cachalot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/db_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/debug_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/loaddata_fixture.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.436322 django-cachalot-2.6.1/cachalot/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/multi_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51433 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/tests_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/thread_safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39198 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/tests/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/cachalot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.436322 django-cachalot-2.6.1/django_cachalot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-21 22:32:47.000000 django-cachalot-2.6.1/django_cachalot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-21 22:32:47.000000 django-cachalot-2.6.1/django_cachalot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:32:47.000000 django-cachalot-2.6.1/django_cachalot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:32:47.000000 django-cachalot-2.6.1/django_cachalot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 22:32:47.000000 django-cachalot-2.6.1/django_cachalot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 22:32:47.000000 django-cachalot-2.6.1/django_cachalot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:32:47.440322 django-cachalot-2.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/how.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/legacy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/limits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/reporting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/docs/todo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/runtests_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:32:47.440322 django-cachalot-2.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1446 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-21 22:32:38.000000 django-cachalot-2.6.1/tox.ini
```

### Comparing `django-cachalot-2.6.0/CHANGELOG.rst` & `django-cachalot-2.6.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 What’s new in django-cachalot?
 ==============================
 
+2.6.1
+-----
+
+- Hot fix when Django is externally imported due to connections import (#242)
+
 2.6.0
 -----
 
 - Dropped Django 2.2 and 4.0 support
 - Added Django 4.2 and Python 3.11 support
 - Added psycopg support (#229)
 - Updated tests to account for the `BEGIN` and `COMMIT` query changes in Django 4.2
```

### Comparing `django-cachalot-2.6.0/LICENSE` & `django-cachalot-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/PKG-INFO` & `django-cachalot-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cachalot
-Version: 2.6.0
+Version: 2.6.1
 Summary: Caches your Django ORM queries and automatically invalidates them.
 Home-page: https://github.com/noripyt/django-cachalot
 Author: Bertrand Bordage, Andrew Chen Wang
 Author-email: acwangpython@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-cachalot-2.6.0/README.rst` & `django-cachalot-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/admin_tests/migrations/0001_initial.py` & `django-cachalot-2.6.1/cachalot/admin_tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/admin_tests/models.py` & `django-cachalot-2.6.1/cachalot/admin_tests/models.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/admin_tests/test_admin.py` & `django-cachalot-2.6.1/cachalot/admin_tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/api.py` & `django-cachalot-2.6.1/cachalot/api.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/apps.py` & `django-cachalot-2.6.1/cachalot/apps.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/cache.py` & `django-cachalot-2.6.1/cachalot/cache.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/jinja2ext.py` & `django-cachalot-2.6.1/cachalot/jinja2ext.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/management/commands/invalidate_cachalot.py` & `django-cachalot-2.6.1/cachalot/management/commands/invalidate_cachalot.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/monkey_patch.py` & `django-cachalot-2.6.1/cachalot/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/panels.py` & `django-cachalot-2.6.1/cachalot/panels.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/settings.py` & `django-cachalot-2.6.1/cachalot/settings.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/templates/cachalot/panel.html` & `django-cachalot-2.6.1/cachalot/templates/cachalot/panel.html`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/__init__.py` & `django-cachalot-2.6.1/cachalot/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/api.py` & `django-cachalot-2.6.1/cachalot/tests/api.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/db_router.py` & `django-cachalot-2.6.1/cachalot/tests/db_router.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/debug_toolbar.py` & `django-cachalot-2.6.1/cachalot/tests/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/migrations/0001_initial.py` & `django-cachalot-2.6.1/cachalot/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/models.py` & `django-cachalot-2.6.1/cachalot/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/multi_db.py` & `django-cachalot-2.6.1/cachalot/tests/multi_db.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/postgres.py` & `django-cachalot-2.6.1/cachalot/tests/postgres.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/read.py` & `django-cachalot-2.6.1/cachalot/tests/read.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/settings.py` & `django-cachalot-2.6.1/cachalot/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/signals.py` & `django-cachalot-2.6.1/cachalot/tests/signals.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/test_utils.py` & `django-cachalot-2.6.1/cachalot/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/tests_decorators.py` & `django-cachalot-2.6.1/cachalot/tests/tests_decorators.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/thread_safety.py` & `django-cachalot-2.6.1/cachalot/tests/thread_safety.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/transaction.py` & `django-cachalot-2.6.1/cachalot/tests/transaction.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/tests/write.py` & `django-cachalot-2.6.1/cachalot/tests/write.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/transaction.py` & `django-cachalot-2.6.1/cachalot/transaction.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/cachalot/utils.py` & `django-cachalot-2.6.1/cachalot/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from decimal import Decimal
 from hashlib import sha1
 from time import time
 from typing import TYPE_CHECKING
 from uuid import UUID
 
 from django.contrib.postgres.functions import TransactionNow
-from django.db import connections, connection
 from django.db.models import Exists, QuerySet, Subquery
 from django.db.models.expressions import RawSQL
 from django.db.models.functions import Now
 from django.db.models.sql import Query, AggregateQuery
 from django.db.models.sql.where import ExtraWhere, WhereNode, NothingNode
 
 from .settings import ITERABLES, cachalot_settings
@@ -31,32 +30,22 @@
 
 CACHABLE_PARAM_TYPES = {
     bool, int, float, Decimal, bytearray, bytes, str, type(None),
     datetime.date, datetime.time, datetime.datetime, datetime.timedelta, UUID,
 }
 UNCACHABLE_FUNCS = {Now, TransactionNow}
 
-# Check if psycopg2 or 3 is used
-connection.ensure_connection()
-underlying_connection = connection.connection
-
-if underlying_connection.__class__.__module__.startswith('psycopg2'):
-    from psycopg2 import Binary
-    from psycopg2.extras import (
-        NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet, Json)
-    CACHABLE_PARAM_TYPES.update((
-        Binary, NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet,
-        Json,))
-elif underlying_connection.__class__.__module__.startswith('psycopg'):
-    from django.db.backends.postgresql.psycopg_any import (
-        NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet,
-    )
 
+try:
     from psycopg.dbapi20 import Binary
 
+    from django.db.backends.postgresql.psycopg_any import (
+        NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet,
+    )
+    
     from psycopg.types.numeric import (
         Int2, Int4, Int8, Float4, Float8,
     )
 
     from ipaddress import (
         IPv4Address,
         IPv6Address,
@@ -67,14 +56,25 @@
     )
 
     CACHABLE_PARAM_TYPES.update((
         NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet, Json, Jsonb,
         Int2, Int4, Int8, Float4, Float8, IPv4Address, IPv6Address,
         Binary,
     ))
+except ImportError:
+    try:
+        from psycopg2 import Binary
+        from psycopg2.extras import (
+            NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet, Json)
+        CACHABLE_PARAM_TYPES.update((
+            Binary, NumericRange, DateRange, DateTimeRange, DateTimeTZRange, Inet,
+            Json,))
+    except ImportError:
+        pass
+
 
 def check_parameter_types(params):
     for p in params:
         cl = p.__class__
         if cl not in CACHABLE_PARAM_TYPES:
             if cl in ITERABLES:
                 check_parameter_types(p)
@@ -214,14 +214,16 @@
             if hasattr(expr, 'flatten'):
                 yield from _flatten(expr)
             else:
                 yield expr
 
 
 def _get_tables(db_alias, query, compiler=False):
+    from django.db import connections
+
     if query.select_for_update or (
             not cachalot_settings.CACHALOT_CACHE_RANDOM
             and '?' in query.order_by):
         raise UncachableQuery
 
     try:
         if query.extra_select:
```

### Comparing `django-cachalot-2.6.0/django_cachalot.egg-info/PKG-INFO` & `django-cachalot-2.6.1/django_cachalot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cachalot
-Version: 2.6.0
+Version: 2.6.1
 Summary: Caches your Django ORM queries and automatically invalidates them.
 Home-page: https://github.com/noripyt/django-cachalot
 Author: Bertrand Bordage, Andrew Chen Wang
 Author-email: acwangpython@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-cachalot-2.6.0/django_cachalot.egg-info/SOURCES.txt` & `django-cachalot-2.6.1/django_cachalot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/Makefile` & `django-cachalot-2.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/benchmark.rst` & `django-cachalot-2.6.1/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/conf.py` & `django-cachalot-2.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/how.rst` & `django-cachalot-2.6.1/docs/how.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/index.rst` & `django-cachalot-2.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/introduction.rst` & `django-cachalot-2.6.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/legacy.rst` & `django-cachalot-2.6.1/docs/legacy.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/limits.rst` & `django-cachalot-2.6.1/docs/limits.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/quickstart.rst` & `django-cachalot-2.6.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/reporting.rst` & `django-cachalot-2.6.1/docs/reporting.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/docs/todo.rst` & `django-cachalot-2.6.1/docs/todo.rst`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/settings.py` & `django-cachalot-2.6.1/settings.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/setup.py` & `django-cachalot-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-cachalot-2.6.0/tox.ini` & `django-cachalot-2.6.1/tox.ini`

 * *Files identical despite different names*

