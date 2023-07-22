# Comparing `tmp/akamai_purge_cache-0.1.3.tar.gz` & `tmp/akamai_purge_cache-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akamai_purge_cache-0.1.3.tar", max compression
+gzip compressed data, was "akamai_purge_cache-0.1.5.tar", max compression
```

## Comparing `akamai_purge_cache-0.1.3.tar` & `akamai_purge_cache-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-19 02:42:42.924833 akamai_purge_cache-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-22 07:11:33.680448 akamai_purge_cache-0.1.3/akamai_purge_cache/__init__.py
--rwxr-xr-x   0        0        0      844 2023-07-22 07:01:37.281113 akamai_purge_cache-0.1.3/akamai_purge_cache/purge.py
--rw-r--r--   0        0        0      582 2023-07-22 07:37:40.614569 akamai_purge_cache-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 akamai_purge_cache-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 02:42:42.924833 akamai_purge_cache-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-22 07:11:33.680448 akamai_purge_cache-0.1.5/akamai-purge-cache/__init__.py
+-rwxr-xr-x   0        0        0      852 2023-07-22 08:16:41.104624 akamai_purge_cache-0.1.5/akamai-purge-cache/purge.py
+-rw-r--r--   0        0        0      669 2023-07-22 08:19:40.615068 akamai_purge_cache-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 akamai_purge_cache-0.1.5/PKG-INFO
```

### Comparing `akamai_purge_cache-0.1.3/akamai_purge_cache/purge.py` & `akamai_purge_cache-0.1.5/akamai-purge-cache/purge.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import click
 
 
 @click.command()
 @click.option('paths', '--path', '-p', multiple=True, help="A single URL to Purge (This option is repeatable for additional URLs)")
 @click.option('--dryrun', '-d', is_flag=True, help="Just print the command and args that will be run and exit")
 
-def purge(paths: list[str], dryrun: bool):
+def mgpurge(paths: list[str], dryrun: bool):
   # Omit credentials to read from ~/.edgerc
   client = FastPurgeClient()
   if dryrun:
     print('These paths will be purged:')
     for path in paths:
       click.echo(path)
   else:
 
     # Start purge of some URLs
-    purge = client.purge_by_url(paths)
+    mgpurge = client.purge_by_url(paths)
     # purge is a Future, if we want to ensure purge completed
     # we can block on the result:
-    result = purge.result()
+    result = mgpurge.result()
     # print("Purge completed:")
     print("Purge completed:", result)
   
 if __name__ == "__main__":
-  purge()
+  mgpurge()
```

### Comparing `akamai_purge_cache-0.1.3/PKG-INFO` & `akamai_purge_cache-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: akamai-purge-cache
-Version: 0.1.3
-Summary: 
+Version: 0.1.5
+Summary: Marriott CDN Team Fastpurge POC script
 Author: Alan Janis
 Author-email: alan.janis@marriott.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: awslambdaric (>=2.0.4,<3.0.0)
```

