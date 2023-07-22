# Comparing `tmp/idkwhttph-0.2.2.tar.gz` & `tmp/idkwhttph-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idkwhttph-0.2.2.tar", max compression
+gzip compressed data, was "idkwhttph-0.2.3.tar", max compression
```

## Comparing `idkwhttph-0.2.2.tar` & `idkwhttph-0.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    41992 2023-07-20 10:35:13.808375 idkwhttph-0.2.2/idkwhttph/__init__.py
--rw-r--r--   0        0        0      295 2023-07-20 10:35:16.360370 idkwhttph-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      492 2023-07-20 10:35:19.723092 idkwhttph-0.2.2/setup.py
--rw-r--r--   0        0        0      239 2023-07-20 10:35:19.723553 idkwhttph-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    24265 2023-07-22 02:55:05.523956 idkwhttph-0.2.3/idkwhttph/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-20 10:39:06.808968 idkwhttph-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-07-22 02:55:25.441174 idkwhttph-0.2.3/setup.py
+-rw-r--r--   0        0        0      239 2023-07-22 02:55:25.441504 idkwhttph-0.2.3/PKG-INFO
```

