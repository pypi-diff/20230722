# Comparing `tmp/cmlibs.importer-0.5.0.tar.gz` & `tmp/cmlibs.importer-0.5.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmlibs.importer-0.5.0.tar", last modified: Sat Apr 15 02:16:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

