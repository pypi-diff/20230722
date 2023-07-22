# Comparing `tmp/botocore-a-la-carte-marketplace-entitlement-1.31.8.tar.gz` & `tmp/botocore_a_la_carte_marketplace_entitlement-1.31.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-marketplace-entitlement-1.31.8.tar", last modified: Fri Jul 21 01:21:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

