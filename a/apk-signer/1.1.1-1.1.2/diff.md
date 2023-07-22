# Comparing `tmp/apk-signer-1.1.1.tar.gz` & `tmp/apk-signer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apk-signer-1.1.1.tar", last modified: Mon Feb 17 16:27:24 2020, max compression
+gzip compressed data, was "dist/apk-signer-1.1.2.tar", last modified: Sat Jul 22 11:13:17 2023, max compression
```

## Comparing `apk-signer-1.1.1.tar` & `apk-signer-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ksg        (501) staff       (20)        0 2020-02-17 16:27:24.259091 apk-signer-1.1.1/
--rw-r--r--   0 ksg        (501) staff       (20)     1293 2020-02-17 16:27:24.258826 apk-signer-1.1.1/PKG-INFO
--rw-r--r--   0 ksg        (501) staff       (20)      665 2020-02-17 16:25:44.000000 apk-signer-1.1.1/README.rst
-drwxr-xr-x   0 ksg        (501) staff       (20)        0 2020-02-17 16:27:24.256497 apk-signer-1.1.1/apk_signer/
--rw-r--r--   0 ksg        (501) staff       (20)       21 2020-02-17 16:20:04.000000 apk-signer-1.1.1/apk_signer/__init__.py
--rw-r--r--   0 ksg        (501) staff       (20)     2782 2020-02-17 16:20:04.000000 apk-signer-1.1.1/apk_signer/apksigner.py
--rw-r--r--   0 ksg        (501) staff       (20)      414 2020-02-17 16:20:04.000000 apk-signer-1.1.1/apk_signer/config.py
--rw-r--r--   0 ksg        (501) staff       (20)     2259 2020-02-17 16:20:04.000000 apk-signer-1.1.1/apk_signer/pyapksigner.jks
-drwxr-xr-x   0 ksg        (501) staff       (20)        0 2020-02-17 16:27:24.258437 apk-signer-1.1.1/apk_signer/scripts/
--rw-r--r--   0 ksg        (501) staff       (20)        0 2020-02-17 16:20:04.000000 apk-signer-1.1.1/apk_signer/scripts/__init__.py
--rw-r--r--   0 ksg        (501) staff       (20)     1590 2020-02-17 16:20:04.000000 apk-signer-1.1.1/apk_signer/scripts/launcher.py
-drwxr-xr-x   0 ksg        (501) staff       (20)        0 2020-02-17 16:27:24.257863 apk-signer-1.1.1/apk_signer.egg-info/
--rw-r--r--   0 ksg        (501) staff       (20)     1293 2020-02-17 16:27:24.000000 apk-signer-1.1.1/apk_signer.egg-info/PKG-INFO
--rw-r--r--   0 ksg        (501) staff       (20)      382 2020-02-17 16:27:24.000000 apk-signer-1.1.1/apk_signer.egg-info/SOURCES.txt
--rw-r--r--   0 ksg        (501) staff       (20)        1 2020-02-17 16:27:24.000000 apk-signer-1.1.1/apk_signer.egg-info/dependency_links.txt
--rw-r--r--   0 ksg        (501) staff       (20)       64 2020-02-17 16:27:24.000000 apk-signer-1.1.1/apk_signer.egg-info/entry_points.txt
--rw-r--r--   0 ksg        (501) staff       (20)       17 2020-02-17 16:27:24.000000 apk-signer-1.1.1/apk_signer.egg-info/requires.txt
--rw-r--r--   0 ksg        (501) staff       (20)       11 2020-02-17 16:27:24.000000 apk-signer-1.1.1/apk_signer.egg-info/top_level.txt
--rw-r--r--   0 ksg        (501) staff       (20)       38 2020-02-17 16:27:24.259190 apk-signer-1.1.1/setup.cfg
--rw-r--r--   0 ksg        (501) staff       (20)     1046 2020-02-17 16:27:20.000000 apk-signer-1.1.1/setup.py
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-22 11:13:17.000000 apk-signer-1.1.2/
+-rw-r--r--   0 ksg        (501) staff       (20)     5459 2023-07-22 11:13:17.000000 apk-signer-1.1.2/PKG-INFO
+-rw-r--r--   0 ksg        (501) staff       (20)     4431 2023-07-22 11:12:31.000000 apk-signer-1.1.2/README.rst
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer/
+-rw-r--r--   0 ksg        (501) staff       (20)       21 2020-02-17 16:20:04.000000 apk-signer-1.1.2/apk_signer/__init__.py
+-rw-r--r--   0 ksg        (501) staff       (20)     2782 2023-07-22 10:33:59.000000 apk-signer-1.1.2/apk_signer/apksigner.py
+-rw-r--r--   0 ksg        (501) staff       (20)      414 2020-02-17 16:20:04.000000 apk-signer-1.1.2/apk_signer/config.py
+-rw-r--r--   0 ksg        (501) staff       (20)     2259 2020-02-17 16:20:04.000000 apk-signer-1.1.2/apk_signer/pyapksigner.jks
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer/scripts/
+-rw-r--r--   0 ksg        (501) staff       (20)        0 2020-02-17 16:20:04.000000 apk-signer-1.1.2/apk_signer/scripts/__init__.py
+-rw-r--r--   0 ksg        (501) staff       (20)     1528 2023-07-22 10:29:15.000000 apk-signer-1.1.2/apk_signer/scripts/launcher.py
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/
+-rw-r--r--   0 ksg        (501) staff       (20)     5459 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/PKG-INFO
+-rw-r--r--   0 ksg        (501) staff       (20)      382 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 ksg        (501) staff       (20)        1 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       64 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/entry_points.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       17 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/requires.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       11 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/top_level.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       38 2023-07-22 11:13:17.000000 apk-signer-1.1.2/setup.cfg
+-rw-r--r--   0 ksg        (501) staff       (20)     1046 2023-07-22 11:13:14.000000 apk-signer-1.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `apk-signer-1.1.1/apk_signer/apksigner.py` & `apk-signer-1.1.2/apk_signer/apksigner.py`

 * *Files identical despite different names*

### Comparing `apk-signer-1.1.1/apk_signer/pyapksigner.jks` & `apk-signer-1.1.2/apk_signer/pyapksigner.jks`

 * *Files identical despite different names*

### Comparing `apk-signer-1.1.1/apk_signer/scripts/launcher.py` & `apk-signer-1.1.2/apk_signer/scripts/launcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 @click.option('--key_path', default='pyapksigner.jks')
 @click.argument('apk')
 def cli(apk: str, default: bool, key_path: str, key_alias: str, key_pass: str, ks_pass: str, run: bool, run_only: bool):
     apk_path = apk
     if not run_only:
         if key_path == 'pyapksigner.jks':
             if not default:
-                print("[Warning] Signing with default keystore.")
-                print("[Warning] Please pass --key_path, --key_alias, --key_pass, --ks_pass parameter, if you want to use your keystore")
+                print("Warning: Pass the --key_path, --key_alias, --key_pass, and --ks_pass parameters if you want to use your own keystore."
             key_path = str(config.ROOT_DIR.joinpath(key_path).resolve())
 
         apk_path = launcher(apk, key_path, key_alias, key_pass, ks_pass)
 
     if run or run_only:
        apk = APK(apk_path)
```

### Comparing `apk-signer-1.1.1/setup.py` & `apk-signer-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apk-signer",
     python_requires='>=3.5',
-    version="1.1.1",
+    version="1.1.2",
     author="ksg97031",
     author_email="ksg97031@gmail.com",
     description="Sign the apk file",
     install_requires=['click', 'androguard'],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/ksg97031/apk-signer",
```

