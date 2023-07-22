# Comparing `tmp/odoo-configurator-3.0.1.tar.gz` & `tmp/odoo-configurator-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo-configurator-3.0.1.tar", last modified: Mon Jul 17 18:44:57 2023, max compression
+gzip compressed data, was "odoo-configurator-3.1.0.tar", last modified: Sat Jul 22 16:39:38 2023, max compression
```

## Comparing `odoo-configurator-3.0.1.tar` & `odoo-configurator-3.1.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.286245 odoo-configurator-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-17 18:44:57.286245 odoo-configurator-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:44:57.286245 odoo-configurator-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.266245 odoo-configurator-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.270245 odoo-configurator-3.0.1/src/odoo_configurator/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.278245 odoo-configurator-3.0.1/src/odoo_configurator/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7008 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5058 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2649 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      293 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10062 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/datas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7236 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/import_configurator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/imports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/mattermost.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5425 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/modules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1940 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/roles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1780 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/translations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1312 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/apps/website.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6763 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/configurator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8694 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/import_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8821 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/odoo_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2211 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/odoo_configurator/password_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.270245 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 18:44:57.000000 odoo-configurator-3.0.1/src/odoo_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.282245 odoo-configurator-3.0.1/src/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/0_base.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:44:57.282245 odoo-configurator-3.0.1/src/templates/14.0/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/14.0/0_base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/1_base_auto_entreprise.yml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/1_base_entreprise.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_account.yml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_account_14.yml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_account_entreprise.yml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_crm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_event.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_expense.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_ged.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_hr.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_maintenance.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_marketing.yml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_mrp.yml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_purchase.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_sale.yml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_sale_subscription.yml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_sign.yml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/src/templates/2_base_website.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      247 2023-07-17 18:44:45.000000 odoo-configurator-3.0.1/start_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:39:38.386765 odoo-configurator-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-22 16:39:38.386765 odoo-configurator-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:39:38.386765 odoo-configurator-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:39:38.378764 odoo-configurator-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:39:38.382764 odoo-configurator-3.1.0/src/odoo_configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:39:38.382764 odoo-configurator-3.1.0/src/odoo_configurator/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7008 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5058 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/call.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2649 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      293 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11932 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/datas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7236 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/import_configurator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/mattermost.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5425 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1940 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/roles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1780 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/translations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1312 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/apps/website.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7333 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/configurator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8694 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/import_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8821 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/odoo_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2211 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/odoo_configurator/password_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:39:38.382764 odoo-configurator-3.1.0/src/odoo_configurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-22 16:39:38.000000 odoo-configurator-3.1.0/src/odoo_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-22 16:39:38.000000 odoo-configurator-3.1.0/src/odoo_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:39:38.000000 odoo-configurator-3.1.0/src/odoo_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-22 16:39:38.000000 odoo-configurator-3.1.0/src/odoo_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-22 16:39:38.000000 odoo-configurator-3.1.0/src/odoo_configurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 16:39:38.000000 odoo-configurator-3.1.0/src/odoo_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:39:38.386765 odoo-configurator-3.1.0/src/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/0_base.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:39:38.386765 odoo-configurator-3.1.0/src/templates/14.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/14.0/0_base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/1_base_auto_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/1_base_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_account.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_account_14.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_account_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_crm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_event.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_expense.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_ged.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_hr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_maintenance.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_marketing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_mrp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_purchase.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_sale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_sale_subscription.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_sign.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/src/templates/2_base_website.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      247 2023-07-22 16:39:26.000000 odoo-configurator-3.1.0/start_config.py
```

### Comparing `odoo-configurator-3.0.1/LICENCE` & `odoo-configurator-3.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/PKG-INFO` & `odoo-configurator-3.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-configurator
-Version: 3.0.1
+Version: 3.1.0
 Summary: Configure and update Odoo database with YAML files
 Author-email: Michel Perrocheau <myrrkel@gmail.com>, David Halgand <david@scalizer.fr>
 Project-URL: Homepage, https://github.com/TeclibERP/odoo-configurator
 Keywords: odoo,configurator,xmlprc,yaml
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,20 +13,25 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
 odoo-configurator
 =================
 
-Update Odoo database with YAML files
+Odoo Configurator simplifies and automates the configuration of Odoo using YAML files. 
+It allows you to update the database, install/update/uninstall modules, configure settings, 
+manage users, and perform various data manipulation operations. 
+It is an essential tool for Odoo administrators looking to streamline their configuration workflow.
 
 ## Installation
+
     pip install odoo-configurator
 
 ## Usage
+
     odoo-configurator ./work_dir/cutomer_name.local.yml
 
 Provided file must contain the auth/odoo section to set connexion parameters.
 
 #### name.local.yml
 
     ---
@@ -46,29 +51,37 @@
 
 Inherits param provide a list of configuration files witch content is merged before execution.
 
     inherits:
         - ../work_dir/cutomer_name/sales.yml
         - ../work_dir/cutomer_name/account.yml
     
-# Script Files
+## Script Files
 
 Script Files param provide a list of configuration files witch content will be executed sequentially.
 
     script_files:
         - ../work_dir/cutomer_name/script1.yml
         - ../work_dir/cutomer_name/script2.yml
     
 ## Parameters
 
 **Install Mode**: To import datas with the value **on_install_only: True** add the "--install" parameter in command
 line:
 
     ./start_config.py ./clients/name/name.local.yml --install
 
+## Environment variables
+
+Some parameters can be provided by environment variable.
+
+Use ODOO_URL, ODOO_DB, ODOO_USER and ODOO_PASSWORD instead of using auth/odoo params in config file
+
+Use KEEPASS_PASSWORD instead of --keepass command line parameter
+
 ## Pre Update
 
 To prepare a configuration or add a fix use "pre_update", the given scripts will be executed before the normal configuration.
 
     pre_update:
         - ../exemple/exemple.pre_update_script.yml
 
@@ -89,40 +102,79 @@
     
 To uninstall modules use "uninstall_modules"
 
     base:
       uninstall_modules:
         - example_module
 
-# Set config parameters (Settings)
+## Set config parameters (Settings)
 
 to set the value of a setting (res.config.settings)
 
     settings:
       config:
         group_use_lead: True
 
 For a specific company:
 
     settings main_company:
       config:
         company_id: get_ref("base.main_company")
         chart_template_id: get_ref("l10n_fr.l10n_fr_pcg_chart_template")
 
-# Update data
+## Create or update records
+    
+If the record with the xml id provided with force_id don't exist, the record will be created.    
+
+    Records to create:
+        datas:
+            My record 1:
+                model: res.partner
+                force_id: external_config.partner_1
+                values:
+                    name: Partner 1
+                    ref: PARTNER1
+            My record 2:
+                model: res.user
+                force_id: base.user_admin
+                values:
+                    name: Admin User
+
+
+## Load records
+
+Using load parameter will speed up creation and update of record compared to single record update.
+
+    Records to load:
+        load: True
+        model: res.partner
+        datas:
+            My record 1:
+                force_id: external_config.record1
+                values:
+                    name: Record 1
+                    ref: REC1
+            My record 2:
+                force_id: external_config.record2
+                values:
+                    name: Record 2
+                    ref: REC2
 
-You can update values on a model according to a domain with "update_domain":
+## Update records with a domain
+
+To update values of multiple records, set a domain with "update_domain" :
 
     Update Example:
       model: res.partner
       update_domain: "[('email','=','example@test.com')]"
       values:
         name: Example
 
-# Server Actions and Functions
+## Server Actions and Functions
+
 To call a model function:
 
     001 Call Function:
       datas:
         Call Function:
           function: example_function
           model: res.parnter
@@ -234,20 +286,20 @@
             specific_import: base/import_specific.py
             specific_method: import_partner
             batch_size: 200
             skip_line: 1420
             limit: 100
             context: {'install_mode': True}
 
-Required fields:
+### Required fields:
 
   - model
   - file_path
 
-Optional fields:
+### Optional fields:
 
   - **name_create_enabled_fields** : List of the fields which are allowed to "Create the record if it doesn't exist"
   - **on_install_only** : Do the csv export only in **Install Mode**
   - **context** : Provide a specific context for imports
   - **specific_import** : Path to a specific Python file
   - **specific_method** : Import method to use form the file **specific_import**
   - **batch_size** : Number of records by load batch
```

### Comparing `odoo-configurator-3.0.1/README.md` & `odoo-configurator-3.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 odoo-configurator
 =================
 
-Update Odoo database with YAML files
+Odoo Configurator simplifies and automates the configuration of Odoo using YAML files. 
+It allows you to update the database, install/update/uninstall modules, configure settings, 
+manage users, and perform various data manipulation operations. 
+It is an essential tool for Odoo administrators looking to streamline their configuration workflow.
 
 ## Installation
+
     pip install odoo-configurator
 
 ## Usage
+
     odoo-configurator ./work_dir/cutomer_name.local.yml
 
 Provided file must contain the auth/odoo section to set connexion parameters.
 
 #### name.local.yml
 
     ---
@@ -30,29 +35,37 @@
 
 Inherits param provide a list of configuration files witch content is merged before execution.
 
     inherits:
         - ../work_dir/cutomer_name/sales.yml
         - ../work_dir/cutomer_name/account.yml
     
-# Script Files
+## Script Files
 
 Script Files param provide a list of configuration files witch content will be executed sequentially.
 
     script_files:
         - ../work_dir/cutomer_name/script1.yml
         - ../work_dir/cutomer_name/script2.yml
     
 ## Parameters
 
 **Install Mode**: To import datas with the value **on_install_only: True** add the "--install" parameter in command
 line:
 
     ./start_config.py ./clients/name/name.local.yml --install
 
+## Environment variables
+
+Some parameters can be provided by environment variable.
+
+Use ODOO_URL, ODOO_DB, ODOO_USER and ODOO_PASSWORD instead of using auth/odoo params in config file
+
+Use KEEPASS_PASSWORD instead of --keepass command line parameter
+
 ## Pre Update
 
 To prepare a configuration or add a fix use "pre_update", the given scripts will be executed before the normal configuration.
 
     pre_update:
         - ../exemple/exemple.pre_update_script.yml
 
@@ -73,40 +86,79 @@
     
 To uninstall modules use "uninstall_modules"
 
     base:
       uninstall_modules:
         - example_module
 
-# Set config parameters (Settings)
+## Set config parameters (Settings)
 
 to set the value of a setting (res.config.settings)
 
     settings:
       config:
         group_use_lead: True
 
 For a specific company:
 
     settings main_company:
       config:
         company_id: get_ref("base.main_company")
         chart_template_id: get_ref("l10n_fr.l10n_fr_pcg_chart_template")
 
-# Update data
+## Create or update records
+    
+If the record with the xml id provided with force_id don't exist, the record will be created.    
+
+    Records to create:
+        datas:
+            My record 1:
+                model: res.partner
+                force_id: external_config.partner_1
+                values:
+                    name: Partner 1
+                    ref: PARTNER1
+            My record 2:
+                model: res.user
+                force_id: base.user_admin
+                values:
+                    name: Admin User
+
+
+## Load records
+
+Using load parameter will speed up creation and update of record compared to single record update.
+
+    Records to load:
+        load: True
+        model: res.partner
+        datas:
+            My record 1:
+                force_id: external_config.record1
+                values:
+                    name: Record 1
+                    ref: REC1
+            My record 2:
+                force_id: external_config.record2
+                values:
+                    name: Record 2
+                    ref: REC2
 
-You can update values on a model according to a domain with "update_domain":
+## Update records with a domain
+
+To update values of multiple records, set a domain with "update_domain" :
 
     Update Example:
       model: res.partner
       update_domain: "[('email','=','example@test.com')]"
       values:
         name: Example
 
-# Server Actions and Functions
+## Server Actions and Functions
+
 To call a model function:
 
     001 Call Function:
       datas:
         Call Function:
           function: example_function
           model: res.parnter
@@ -218,20 +270,20 @@
             specific_import: base/import_specific.py
             specific_method: import_partner
             batch_size: 200
             skip_line: 1420
             limit: 100
             context: {'install_mode': True}
 
-Required fields:
+### Required fields:
 
   - model
   - file_path
 
-Optional fields:
+### Optional fields:
 
   - **name_create_enabled_fields** : List of the fields which are allowed to "Create the record if it doesn't exist"
   - **on_install_only** : Do the csv export only in **Install Mode**
   - **context** : Provide a specific context for imports
   - **specific_import** : Path to a specific Python file
   - **specific_method** : Import method to use form the file **specific_import**
   - **batch_size** : Number of records by load batch
```

### Comparing `odoo-configurator-3.0.1/pyproject.toml` & `odoo-configurator-3.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "odoo-configurator"
-version = "3.0.1"
+version = "3.1.0"
 description = "Configure and update Odoo database with YAML files"
 readme = "README.md"
 authors = [{ name = "Michel Perrocheau", email = "myrrkel@gmail.com" },
 { name = "David Halgand", email = "david@scalizer.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
```

### Comparing `odoo-configurator-3.0.1/requirements.txt` & `odoo-configurator-3.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/__main__.py` & `odoo-configurator-3.1.0/src/odoo_configurator/__main__.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/__init__.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/account.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/account.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/base.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/base.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/call.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/call.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/config.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/config.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/datas.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/datas.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 from collections import OrderedDict
 from ast import literal_eval
 
 from . import base
 from .config import OdooConfig
 
 
+def prepare_load_values(load_fields, fields, values):
+    load_values = []
+    for load_field in load_fields:
+        if load_field in fields:
+            value = values[fields.index(load_field)]
+        else:
+            value = False
+        load_values.append(value)
+
+    return load_values
+
+
 class OdooDatas(base.OdooModule):
     _name = "Datas"
 
     def apply(self):
         pass  # For remove standard log
 
     def execute(self, datas):
@@ -33,30 +45,42 @@
     def execute_pre_update_config_datas(self):
         self.logger.info("Apply Pre-%s" % self._name)
         if self._pre_datas:
             self.execute(self._pre_datas)
 
     def execute_update_config_datas(self):
         self.logger.info("Apply %s" % self._name)
+        self.get_external_config_xmlid_cache()
         self.execute(self._datas)
 
+    def get_external_config_xmlid_cache(self):
+        domain = [['module', '=', 'external_config']]
+        datas = self.execute_odoo('ir.model.data', 'search_read', [domain, ['name', 'res_id']], {'context': {}})
+        for data in datas:
+            self._configurator.xmlid_cache['external_config.%s' % data['name']] = data['res_id']
+
     def execute_config(self, config):
         if config:
             self.pre_config(config)
             self._connection.execute_config(config)
 
     def odoo_datas(self, datas):
         self.pre_config(datas)
+        raw_load_values = []
+        load_fields = []
+        load = datas.pop('load', False)
+        model = datas.pop('model', False)
         for data in datas:
+            object_ids = False
             self.logger.info("\t\t* %s" % data)
             if not isinstance(datas[data], dict):
                 return
             if 'install' not in self._mode and datas[data].get('on_install_only', False):
                 return
-            model = datas[data].get('model')
+            model = datas[data].get('model') or model
             key = datas[data].get('key', False)
             force_id = datas[data].get('force_id', False)
             delete_all = datas[data].get('delete_all', False)
             delete_domain = datas[data].get('delete_domain', False)
             delete_id = datas[data].get('delete_id', False)
             deactivate = datas[data].get('deactivate', False)
             activate = datas[data].get('activate', False)
@@ -121,15 +145,18 @@
                 continue
 
             if key:
                 object_ids = self.execute_odoo(model, 'search',
                                                [[(key, '=', values[key])], 0, 0, "id", False],
                                                {'context': config_context})
             elif force_id:
-                values, object_ids = self.set_force_id(model, values, config_context, force_id)
+                if load:
+                    values['id'] = force_id
+                else:
+                    values, object_ids = self.set_force_id(model, values, config_context, force_id)
             elif action_server_id:
                 self.exec_action_server(action_server_id, datas[data], config_context, no_raise)
                 continue
             elif function:
                 self.exec_function(function, datas[data], config_context, no_raise)
                 continue
             else:
@@ -138,47 +165,66 @@
 
             # prepare many2many list of xmlid
             for key in values.keys():
                 if isinstance(values[key], list) and '/id' in key:
                     if values[key] and isinstance(values[key][0], str) and '.' in values[key][0]:
                         values[key] = ','.join(values[key])
 
-            for language in languages:
-                config_context['lang'] = language
-                self.save_values(model, values, config_context, force_id, object_ids)
+            if load:
+
+                fields, rec_values = self.save_values(model, values, config_context, force_id, object_ids,
+                                                      load_batch=load)
+                load_fields = list(set(load_fields + fields))
+                raw_load_values.append((fields, rec_values[0]))
+            else:
+                for language in languages:
+                    config_context['lang'] = language
+                    self.save_values(model, values, config_context, force_id, object_ids)
+
+        if load:
+            load_values = [prepare_load_values(load_fields, v[0], v[1]) for v in raw_load_values]
+            context = self._context
+            self.execute_load(model, load_fields, load_values, context)
 
-    def save_values(self, model, values, config_context, force_id, object_ids):
+    def save_values(self, model, values, config_context, force_id, object_ids, load_batch=False):
         if not force_id or isinstance(force_id, int):
             if object_ids:
                 self.execute_odoo(model, 'write', [object_ids, dict(values)], {'context': config_context})
             else:
                 self.execute_odoo(model, 'create', [dict(values)], {'context': config_context})
         else:
             load_keys = list(values.keys())
             load_data = [[]]
             for i in load_keys:
                 if isinstance(values[i], bool):
                     load_data[0].append(str(values[i]))
                 else:
                     load_data[0].append(values[i])
             self.logger.debug('%s: %s %s' % (model, load_keys, load_data))
-            # print(load_keys, load_data)
-            res = self.execute_odoo(model, 'load', [load_keys, load_data], {'context': config_context})
-            for message in res['messages']:
-                self.logger.error("%s : %s" % (message['record'], message['message']))
+            if load_batch:
+                return load_keys, load_data
+            else:
+                self.execute_load(model, load_keys, load_data, config_context)
+
+    def execute_load(self, model, load_keys, load_data, config_context):
+        res = self.execute_odoo(model, 'load', [load_keys, load_data], {'context': config_context})
+        for message in res['messages']:
+            self.logger.error("%s : %s" % (message['record'], message['message']))
 
     def set_force_id(self, model, values, config_context, force_id=False):
         if isinstance(force_id, int):
             values['id'] = force_id
             object_ids = self.execute_odoo(model, 'search', [[('id', '=', force_id)], 0, 0, "id", False],
                                            {'context': config_context})
         else:
             if '.' not in force_id:
                 force_id = "external_config." + force_id
             values['id'] = force_id
+            if force_id in self._configurator.xmlid_cache:
+                return values, self._configurator.xmlid_cache[force_id]
             module, name = force_id.split('.')
             if self.execute_odoo('ir.model.data', 'search',
                                  [[('module', '=', module), ('name', '=', name)], 0, 0, "id", False],
                                  {'context': config_context}):
                 object_ids = self._connection.get_ref(force_id)
             else:
                 object_ids = []
```

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/defaults.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/defaults.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/import_configurator.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/import_configurator.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/imports.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/imports.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/mattermost.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/mattermost.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/modules.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/modules.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/roles.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/roles.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/translations.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/translations.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/users.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/users.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/apps/website.py` & `odoo-configurator-3.1.0/src/odoo_configurator/apps/website.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/import_manager.py` & `odoo-configurator-3.1.0/src/odoo_configurator/import_manager.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/odoo_connection.py` & `odoo-configurator-3.1.0/src/odoo_configurator/odoo_connection.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator/password_manager.py` & `odoo-configurator-3.1.0/src/odoo_configurator/password_manager.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator.egg-info/PKG-INFO` & `odoo-configurator-3.1.0/src/odoo_configurator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-configurator
-Version: 3.0.1
+Version: 3.1.0
 Summary: Configure and update Odoo database with YAML files
 Author-email: Michel Perrocheau <myrrkel@gmail.com>, David Halgand <david@scalizer.fr>
 Project-URL: Homepage, https://github.com/TeclibERP/odoo-configurator
 Keywords: odoo,configurator,xmlprc,yaml
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,20 +13,25 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
 odoo-configurator
 =================
 
-Update Odoo database with YAML files
+Odoo Configurator simplifies and automates the configuration of Odoo using YAML files. 
+It allows you to update the database, install/update/uninstall modules, configure settings, 
+manage users, and perform various data manipulation operations. 
+It is an essential tool for Odoo administrators looking to streamline their configuration workflow.
 
 ## Installation
+
     pip install odoo-configurator
 
 ## Usage
+
     odoo-configurator ./work_dir/cutomer_name.local.yml
 
 Provided file must contain the auth/odoo section to set connexion parameters.
 
 #### name.local.yml
 
     ---
@@ -46,29 +51,37 @@
 
 Inherits param provide a list of configuration files witch content is merged before execution.
 
     inherits:
         - ../work_dir/cutomer_name/sales.yml
         - ../work_dir/cutomer_name/account.yml
     
-# Script Files
+## Script Files
 
 Script Files param provide a list of configuration files witch content will be executed sequentially.
 
     script_files:
         - ../work_dir/cutomer_name/script1.yml
         - ../work_dir/cutomer_name/script2.yml
     
 ## Parameters
 
 **Install Mode**: To import datas with the value **on_install_only: True** add the "--install" parameter in command
 line:
 
     ./start_config.py ./clients/name/name.local.yml --install
 
+## Environment variables
+
+Some parameters can be provided by environment variable.
+
+Use ODOO_URL, ODOO_DB, ODOO_USER and ODOO_PASSWORD instead of using auth/odoo params in config file
+
+Use KEEPASS_PASSWORD instead of --keepass command line parameter
+
 ## Pre Update
 
 To prepare a configuration or add a fix use "pre_update", the given scripts will be executed before the normal configuration.
 
     pre_update:
         - ../exemple/exemple.pre_update_script.yml
 
@@ -89,40 +102,79 @@
     
 To uninstall modules use "uninstall_modules"
 
     base:
       uninstall_modules:
         - example_module
 
-# Set config parameters (Settings)
+## Set config parameters (Settings)
 
 to set the value of a setting (res.config.settings)
 
     settings:
       config:
         group_use_lead: True
 
 For a specific company:
 
     settings main_company:
       config:
         company_id: get_ref("base.main_company")
         chart_template_id: get_ref("l10n_fr.l10n_fr_pcg_chart_template")
 
-# Update data
+## Create or update records
+    
+If the record with the xml id provided with force_id don't exist, the record will be created.    
+
+    Records to create:
+        datas:
+            My record 1:
+                model: res.partner
+                force_id: external_config.partner_1
+                values:
+                    name: Partner 1
+                    ref: PARTNER1
+            My record 2:
+                model: res.user
+                force_id: base.user_admin
+                values:
+                    name: Admin User
+
+
+## Load records
+
+Using load parameter will speed up creation and update of record compared to single record update.
+
+    Records to load:
+        load: True
+        model: res.partner
+        datas:
+            My record 1:
+                force_id: external_config.record1
+                values:
+                    name: Record 1
+                    ref: REC1
+            My record 2:
+                force_id: external_config.record2
+                values:
+                    name: Record 2
+                    ref: REC2
 
-You can update values on a model according to a domain with "update_domain":
+## Update records with a domain
+
+To update values of multiple records, set a domain with "update_domain" :
 
     Update Example:
       model: res.partner
       update_domain: "[('email','=','example@test.com')]"
       values:
         name: Example
 
-# Server Actions and Functions
+## Server Actions and Functions
+
 To call a model function:
 
     001 Call Function:
       datas:
         Call Function:
           function: example_function
           model: res.parnter
@@ -234,20 +286,20 @@
             specific_import: base/import_specific.py
             specific_method: import_partner
             batch_size: 200
             skip_line: 1420
             limit: 100
             context: {'install_mode': True}
 
-Required fields:
+### Required fields:
 
   - model
   - file_path
 
-Optional fields:
+### Optional fields:
 
   - **name_create_enabled_fields** : List of the fields which are allowed to "Create the record if it doesn't exist"
   - **on_install_only** : Do the csv export only in **Install Mode**
   - **context** : Provide a specific context for imports
   - **specific_import** : Path to a specific Python file
   - **specific_method** : Import method to use form the file **specific_import**
   - **batch_size** : Number of records by load batch
```

### Comparing `odoo-configurator-3.0.1/src/odoo_configurator.egg-info/SOURCES.txt` & `odoo-configurator-3.1.0/src/odoo_configurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/templates/1_base_auto_entreprise.yml` & `odoo-configurator-3.1.0/src/templates/1_base_auto_entreprise.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/templates/2_base_account.yml` & `odoo-configurator-3.1.0/src/templates/2_base_account.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/templates/2_base_account_14.yml` & `odoo-configurator-3.1.0/src/templates/2_base_account_14.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.0.1/src/templates/2_base_sale.yml` & `odoo-configurator-3.1.0/src/templates/2_base_sale.yml`

 * *Files identical despite different names*

