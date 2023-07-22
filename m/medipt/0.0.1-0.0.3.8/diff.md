# Comparing `tmp/medipt-0.0.1.tar.gz` & `tmp/medipt-0.0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\ImageProcessingTools\dist\.tmp-bqfk6xud\medipt-0.0.1.tar", last modified: Sat Jul 22 17:01:24 2023, max compression
+gzip compressed data, was "medipt-0.0.3.8.tar", last modified: Sat Jul 22 21:01:01 2023, max compression
```

## Comparing `medipt-0.0.1.tar` & `medipt-0.0.3.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 17:01:24.000000 medipt-0.0.1/
--rw-rw-rw-   0        0        0      259 2023-07-22 17:01:24.000000 medipt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       71 2023-07-13 15:27:56.000000 medipt-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 17:01:24.000000 medipt-0.0.1/imageprocessingtools/
--rw-rw-rw-   0        0        0      120 2023-07-21 17:12:49.000000 medipt-0.0.1/imageprocessingtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:01:24.000000 medipt-0.0.1/medipt.egg-info/
--rw-rw-rw-   0        0        0      259 2023-07-22 17:01:24.000000 medipt-0.0.1/medipt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-22 17:01:24.000000 medipt-0.0.1/medipt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 17:01:24.000000 medipt-0.0.1/medipt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-22 17:01:24.000000 medipt-0.0.1/medipt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-22 17:01:24.000000 medipt-0.0.1/medipt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      688 2023-07-22 17:00:24.000000 medipt-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       28 2023-07-22 15:53:55.000000 medipt-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 17:01:24.000000 medipt-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:01:01.500985 medipt-0.0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-22 21:00:38.000000 medipt-0.0.3.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:01:01.496985 medipt-0.0.3.8/MedIPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-22 21:00:38.000000 medipt-0.0.3.8/MedIPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-22 21:01:01.500985 medipt-0.0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-22 21:00:38.000000 medipt-0.0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:01:01.500985 medipt-0.0.3.8/medipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-22 21:01:01.000000 medipt-0.0.3.8/medipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-22 21:01:01.000000 medipt-0.0.3.8/medipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 21:01:01.000000 medipt-0.0.3.8/medipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 21:01:01.000000 medipt-0.0.3.8/medipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-22 21:01:01.000000 medipt-0.0.3.8/medipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-22 21:00:38.000000 medipt-0.0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-22 21:00:38.000000 medipt-0.0.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 21:01:01.500985 medipt-0.0.3.8/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

