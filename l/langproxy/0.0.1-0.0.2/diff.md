# Comparing `tmp/langproxy-0.0.1.tar.gz` & `tmp/langproxy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langproxy-0.0.1.tar", last modified: Sat Jul 22 14:29:53 2023, max compression
+gzip compressed data, was "langproxy-0.0.2.tar", last modified: Sat Jul 22 15:11:33 2023, max compression
```

## Comparing `langproxy-0.0.1.tar` & `langproxy-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 jinto      (501) staff       (20)        0 2023-07-22 14:29:53.701374 langproxy-0.0.1/
--rw-r--r--   0 jinto      (501) staff       (20)      280 2023-07-22 14:29:53.701270 langproxy-0.0.1/PKG-INFO
-drwxr-xr-x   0 jinto      (501) staff       (20)        0 2023-07-22 14:29:53.700484 langproxy-0.0.1/langproxy/
--rw-r--r--   0 jinto      (501) staff       (20)       22 2023-07-22 14:28:05.000000 langproxy-0.0.1/langproxy/__init__.py
-drwxr-xr-x   0 jinto      (501) staff       (20)        0 2023-07-22 14:29:53.701129 langproxy-0.0.1/langproxy.egg-info/
--rw-r--r--   0 jinto      (501) staff       (20)      280 2023-07-22 14:29:53.000000 langproxy-0.0.1/langproxy.egg-info/PKG-INFO
--rw-r--r--   0 jinto      (501) staff       (20)      209 2023-07-22 14:29:53.000000 langproxy-0.0.1/langproxy.egg-info/SOURCES.txt
--rw-r--r--   0 jinto      (501) staff       (20)        1 2023-07-22 14:29:53.000000 langproxy-0.0.1/langproxy.egg-info/dependency_links.txt
--rw-r--r--   0 jinto      (501) staff       (20)        1 2023-07-22 14:29:53.000000 langproxy-0.0.1/langproxy.egg-info/not-zip-safe
--rw-r--r--   0 jinto      (501) staff       (20)       10 2023-07-22 14:29:53.000000 langproxy-0.0.1/langproxy.egg-info/top_level.txt
--rw-r--r--   0 jinto      (501) staff       (20)       76 2023-07-22 14:29:51.000000 langproxy-0.0.1/pyproject.toml
--rw-r--r--   0 jinto      (501) staff       (20)       38 2023-07-22 14:29:53.701405 langproxy-0.0.1/setup.cfg
--rw-r--r--   0 jinto      (501) staff       (20)      496 2023-07-22 14:27:45.000000 langproxy-0.0.1/setup.py
+drwxr-xr-x   0 jinto      (501) staff       (20)        0 2023-07-22 15:11:33.519334 langproxy-0.0.2/
+-rw-r--r--   0 jinto      (501) staff       (20)      280 2023-07-22 15:11:33.519209 langproxy-0.0.2/PKG-INFO
+-rw-r--r--   0 jinto      (501) staff       (20)     2126 2023-07-22 15:04:52.000000 langproxy-0.0.2/README.md
+drwxr-xr-x   0 jinto      (501) staff       (20)        0 2023-07-22 15:11:33.518486 langproxy-0.0.2/langproxy/
+-rw-r--r--   0 jinto      (501) staff       (20)       51 2023-07-22 15:09:36.000000 langproxy-0.0.2/langproxy/__init__.py
+-rw-r--r--   0 jinto      (501) staff       (20)     1061 2023-07-22 14:42:06.000000 langproxy-0.0.2/langproxy/session.py
+drwxr-xr-x   0 jinto      (501) staff       (20)        0 2023-07-22 15:11:33.519043 langproxy-0.0.2/langproxy.egg-info/
+-rw-r--r--   0 jinto      (501) staff       (20)      280 2023-07-22 15:11:33.000000 langproxy-0.0.2/langproxy.egg-info/PKG-INFO
+-rw-r--r--   0 jinto      (501) staff       (20)      240 2023-07-22 15:11:33.000000 langproxy-0.0.2/langproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 jinto      (501) staff       (20)        1 2023-07-22 15:11:33.000000 langproxy-0.0.2/langproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 jinto      (501) staff       (20)        1 2023-07-22 15:11:33.000000 langproxy-0.0.2/langproxy.egg-info/not-zip-safe
+-rw-r--r--   0 jinto      (501) staff       (20)       10 2023-07-22 15:11:33.000000 langproxy-0.0.2/langproxy.egg-info/top_level.txt
+-rw-r--r--   0 jinto      (501) staff       (20)       76 2023-07-22 14:29:51.000000 langproxy-0.0.2/pyproject.toml
+-rw-r--r--   0 jinto      (501) staff       (20)       38 2023-07-22 15:11:33.519370 langproxy-0.0.2/setup.cfg
+-rw-r--r--   0 jinto      (501) staff       (20)      633 2023-07-22 15:10:40.000000 langproxy-0.0.2/setup.py
```

