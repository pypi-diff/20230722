# Comparing `tmp/nonebot_plugin_dall-e-0.5.tar.gz` & `tmp/nonebot_plugin_dall_e-0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_dall-e-0.5.tar", last modified: Wed Jul 19 02:31:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

