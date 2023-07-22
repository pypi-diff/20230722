# Comparing `tmp/wagtail-all-in-one-accessibility-1.4.tar.gz` & `tmp/wagtail_all_in_one_accessibility-1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-all-in-one-accessibility-1.4.tar", last modified: Tue Jun 13 09:36:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

