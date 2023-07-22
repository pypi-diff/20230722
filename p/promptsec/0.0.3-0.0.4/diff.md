# Comparing `tmp/promptsec-0.0.3.tar.gz` & `tmp/promptsec-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptsec-0.0.3.tar", last modified: Thu Jul 20 00:20:12 2023, max compression
+gzip compressed data, was "promptsec-0.0.4.tar", last modified: Sat Jul 22 12:15:11 2023, max compression
```

## Comparing `promptsec-0.0.3.tar` & `promptsec-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 track     (1000) track     (1000)        0 2023-07-20 00:20:12.864063 promptsec-0.0.3/
--rw-rw-r--   0 track     (1000) track     (1000)       28 2023-07-19 03:49:18.000000 promptsec-0.0.3/LICENSE
--rw-rw-r--   0 track     (1000) track     (1000)       22 2023-07-19 22:41:28.000000 promptsec-0.0.3/MANIFEST.in
--rw-rw-r--   0 track     (1000) track     (1000)      229 2023-07-20 00:20:12.864063 promptsec-0.0.3/PKG-INFO
--rw-r--r--   0 track     (1000) track     (1000)     1140 2023-07-18 22:59:24.000000 promptsec-0.0.3/README.md
--rw-rw-r--   0 track     (1000) track     (1000)       20 2023-07-20 00:20:09.000000 promptsec-0.0.3/pkg_version.py
-drwxrwxr-x   0 track     (1000) track     (1000)        0 2023-07-20 00:20:12.864063 promptsec-0.0.3/promptsec/
--rw-r--r--   0 track     (1000) track     (1000)       83 2023-07-19 23:56:08.000000 promptsec-0.0.3/promptsec/__init__.py
--rw-r--r--   0 track     (1000) track     (1000)     2057 2023-07-20 00:02:44.000000 promptsec-0.0.3/promptsec/_common.py
-drwxrwxr-x   0 track     (1000) track     (1000)        0 2023-07-20 00:20:12.864063 promptsec-0.0.3/promptsec/langchain/
--rw-rw-r--   0 track     (1000) track     (1000)        0 2023-07-19 22:40:53.000000 promptsec-0.0.3/promptsec/langchain/__init__.py
--rw-rw-r--   0 track     (1000) track     (1000)      934 2023-07-19 23:09:37.000000 promptsec-0.0.3/promptsec/langchain/llms.py
--rw-rw-r--   0 track     (1000) track     (1000)      787 2023-07-19 23:09:45.000000 promptsec-0.0.3/promptsec/langchain/monkey_patch.py
-drwxrwxr-x   0 track     (1000) track     (1000)        0 2023-07-20 00:20:12.864063 promptsec-0.0.3/promptsec.egg-info/
--rw-rw-r--   0 track     (1000) track     (1000)      229 2023-07-20 00:20:12.000000 promptsec-0.0.3/promptsec.egg-info/PKG-INFO
--rw-rw-r--   0 track     (1000) track     (1000)      356 2023-07-20 00:20:12.000000 promptsec-0.0.3/promptsec.egg-info/SOURCES.txt
--rw-rw-r--   0 track     (1000) track     (1000)        1 2023-07-20 00:20:12.000000 promptsec-0.0.3/promptsec.egg-info/dependency_links.txt
--rw-rw-r--   0 track     (1000) track     (1000)       26 2023-07-20 00:20:12.000000 promptsec-0.0.3/promptsec.egg-info/requires.txt
--rw-rw-r--   0 track     (1000) track     (1000)       10 2023-07-20 00:20:12.000000 promptsec-0.0.3/promptsec.egg-info/top_level.txt
--rw-rw-r--   0 track     (1000) track     (1000)       38 2023-07-20 00:20:12.864063 promptsec-0.0.3/setup.cfg
--rw-rw-r--   0 track     (1000) track     (1000)      427 2023-07-19 23:56:42.000000 promptsec-0.0.3/setup.py
+drwxrwxr-x   0 track     (1000) track     (1000)        0 2023-07-22 12:15:11.291402 promptsec-0.0.4/
+-rw-rw-r--   0 track     (1000) track     (1000)       28 2023-07-19 03:49:18.000000 promptsec-0.0.4/LICENSE
+-rw-rw-r--   0 track     (1000) track     (1000)       22 2023-07-19 22:41:28.000000 promptsec-0.0.4/MANIFEST.in
+-rw-rw-r--   0 track     (1000) track     (1000)      229 2023-07-22 12:15:11.291402 promptsec-0.0.4/PKG-INFO
+-rw-r--r--   0 track     (1000) track     (1000)     1140 2023-07-18 22:59:24.000000 promptsec-0.0.4/README.md
+-rw-rw-r--   0 track     (1000) track     (1000)       20 2023-07-22 12:15:08.000000 promptsec-0.0.4/pkg_version.py
+drwxrwxr-x   0 track     (1000) track     (1000)        0 2023-07-22 12:15:11.287402 promptsec-0.0.4/promptsec/
+-rw-r--r--   0 track     (1000) track     (1000)       83 2023-07-19 23:56:08.000000 promptsec-0.0.4/promptsec/__init__.py
+-rw-rw-r--   0 track     (1000) track     (1000)     5119 2023-07-22 12:08:24.000000 promptsec-0.0.4/promptsec/_common.py
+drwxrwxr-x   0 track     (1000) track     (1000)        0 2023-07-22 12:15:11.291402 promptsec-0.0.4/promptsec/langchain/
+-rw-rw-r--   0 track     (1000) track     (1000)        0 2023-07-19 22:40:53.000000 promptsec-0.0.4/promptsec/langchain/__init__.py
+-rw-rw-r--   0 track     (1000) track     (1000)      934 2023-07-19 23:09:37.000000 promptsec-0.0.4/promptsec/langchain/llms.py
+-rw-rw-r--   0 track     (1000) track     (1000)      787 2023-07-19 23:09:45.000000 promptsec-0.0.4/promptsec/langchain/monkey_patch.py
+drwxrwxr-x   0 track     (1000) track     (1000)        0 2023-07-22 12:15:11.291402 promptsec-0.0.4/promptsec.egg-info/
+-rw-rw-r--   0 track     (1000) track     (1000)      229 2023-07-22 12:15:11.000000 promptsec-0.0.4/promptsec.egg-info/PKG-INFO
+-rw-rw-r--   0 track     (1000) track     (1000)      356 2023-07-22 12:15:11.000000 promptsec-0.0.4/promptsec.egg-info/SOURCES.txt
+-rw-rw-r--   0 track     (1000) track     (1000)        1 2023-07-22 12:15:11.000000 promptsec-0.0.4/promptsec.egg-info/dependency_links.txt
+-rw-rw-r--   0 track     (1000) track     (1000)       26 2023-07-22 12:15:11.000000 promptsec-0.0.4/promptsec.egg-info/requires.txt
+-rw-rw-r--   0 track     (1000) track     (1000)       10 2023-07-22 12:15:11.000000 promptsec-0.0.4/promptsec.egg-info/top_level.txt
+-rw-rw-r--   0 track     (1000) track     (1000)       38 2023-07-22 12:15:11.291402 promptsec-0.0.4/setup.cfg
+-rw-rw-r--   0 track     (1000) track     (1000)      427 2023-07-19 23:56:42.000000 promptsec-0.0.4/setup.py
```

### Comparing `promptsec-0.0.3/README.md` & `promptsec-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `promptsec-0.0.3/promptsec/langchain/llms.py` & `promptsec-0.0.4/promptsec/langchain/llms.py`

 * *Files identical despite different names*

### Comparing `promptsec-0.0.3/promptsec/langchain/monkey_patch.py` & `promptsec-0.0.4/promptsec/langchain/monkey_patch.py`

 * *Files identical despite different names*

