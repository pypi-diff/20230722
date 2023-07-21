# Comparing `tmp/jag-panzer-0.1.21.tar.gz` & `tmp/jag-panzer-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jag-panzer-0.1.21.tar", last modified: Sat Jun 10 02:03:13 2023, max compression
+gzip compressed data, was "jag-panzer-0.1.23.tar", last modified: Fri Jul 21 23:37:30 2023, max compression
```

## Comparing `jag-panzer-0.1.21.tar` & `jag-panzer-0.1.23.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.612119 jag-panzer-0.1.21/
--rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.1.21/LICENSE
--rw-rw-rw-   0        0        0       46 2023-06-09 02:05:06.000000 jag-panzer-0.1.21/MANIFEST.in
--rw-rw-rw-   0        0        0      561 2023-06-10 02:03:13.612119 jag-panzer-0.1.21/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.1.21/README.md
--rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.1.21/pyproject.toml
--rw-rw-rw-   0        0        0      672 2023-06-10 02:03:13.619096 jag-panzer-0.1.21/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:10.393728 jag-panzer-0.1.21/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.383087 jag-panzer-0.1.21/src/jag_panzer/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:13:59.000000 jag-panzer-0.1.21/src/jag_panzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.480120 jag-panzer-0.1.21/src/jag_panzer/assets/
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.759076 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/
--rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/base.html
--rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/dir_icon.svg
--rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/download_icon.svg
--rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/file_icon.svg
--rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/script.js
--rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/style.css
--rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.1.21/src/jag_panzer/assets/reject.html
--rw-rw-rw-   0        0        0    20150 2023-06-10 02:01:28.000000 jag-panzer-0.1.21/src/jag_panzer/base_room.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.912085 jag-panzer-0.1.21/src/jag_panzer/cgi/
--rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/__init__.py
--rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/burn_power.py
--rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/hitman.py
--rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/jag.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.918069 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.941103 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.977094 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
--rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
--rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
--rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
--rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
--rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/cgi/templates/unit.service
--rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.1.21/src/jag_panzer/dir_list.py
--rw-rw-rw-   0        0        0      369 2023-06-07 05:17:03.000000 jag-panzer-0.1.21/src/jag_panzer/jag_util.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:10.720021 jag-panzer-0.1.21/src/jag_panzer/libs/
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:12.225111 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/
--rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:12.443199 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/
--rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/__init__.py
--rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_html5lib.py
--rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_htmlparser.py
--rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_lxml.py
--rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/css.py
--rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/dammit.py
--rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/diagnose.py
--rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/element.py
--rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/formatter.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:12.937154 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/
--rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.171061 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/
--rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
--rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
--rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
--rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
--rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
--rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
--rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
--rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
--rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
--rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
--rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
--rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_builder.py
--rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
--rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_css.py
--rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_dammit.py
--rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_docs.py
--rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_element.py
--rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_formatter.py
--rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_fuzz.py
--rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_html5lib.py
--rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
--rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_lxml.py
--rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
--rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_pageelement.py
--rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_soup.py
--rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_tag.py
--rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_tree.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.438156 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/
--rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/__init__.py
--rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/__meta__.py
--rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_match.py
--rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_parser.py
--rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_types.py
--rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/pretty.py
--rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/py.typed
--rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/util.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.568591 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/
--rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/__init__.py
--rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/doc.py
--rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/indentation.py
--rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/py.typed
--rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.1.21/src/jag_panzer/libs/yattag/simpledoc.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:13.608094 jag-panzer-0.1.21/src/jag_panzer/mimes/
--rw-rw-rw-   0        0        0     2762 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/mimes/mime_types_base.py
--rw-rw-rw-   0        0        0     1938 2023-06-03 17:16:43.000000 jag-panzer-0.1.21/src/jag_panzer/response_codes.py
--rw-rw-rw-   0        0        0     7795 2023-06-10 01:24:17.000000 jag-panzer-0.1.21/src/jag_panzer/server.py
--rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.1.21/src/jag_panzer/test.cmd
-drwxrwxrwx   0        0        0        0 2023-06-10 02:03:11.475123 jag-panzer-0.1.21/src/jag_panzer.egg-info/
--rw-rw-rw-   0        0        0      561 2023-06-10 02:03:10.000000 jag-panzer-0.1.21/src/jag_panzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3986 2023-06-10 02:03:10.000000 jag-panzer-0.1.21/src/jag_panzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 02:03:10.000000 jag-panzer-0.1.21/src/jag_panzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-10 02:03:10.000000 jag-panzer-0.1.21/src/jag_panzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.481122 jag-panzer-0.1.23/
+-rw-rw-rw-   0        0        0      161 2023-06-09 00:40:57.000000 jag-panzer-0.1.23/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-06-09 02:05:06.000000 jag-panzer-0.1.23/MANIFEST.in
+-rw-rw-rw-   0        0        0      561 2023-07-21 23:37:30.481122 jag-panzer-0.1.23/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-09 00:32:58.000000 jag-panzer-0.1.23/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-09 00:12:29.000000 jag-panzer-0.1.23/pyproject.toml
+-rw-rw-rw-   0        0        0      672 2023-07-21 23:37:30.488117 jag-panzer-0.1.23/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.245005 jag-panzer-0.1.23/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.276985 jag-panzer-0.1.23/src/jag_panzer/
+-rw-rw-rw-   0        0        0        0 2023-06-11 10:49:01.000000 jag-panzer-0.1.23/src/jag_panzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.308969 jag-panzer-0.1.23/src/jag_panzer/assets/
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.320963 jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/
+-rw-rw-rw-   0        0        0      356 2023-06-08 21:39:34.000000 jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/base.html
+-rw-rw-rw-   0        0        0      446 2023-06-06 00:39:53.000000 jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/dir_icon.svg
+-rw-rw-rw-   0        0        0      682 2023-06-07 06:27:42.000000 jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/download_icon.svg
+-rw-rw-rw-   0        0        0      704 2023-06-06 00:40:06.000000 jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/file_icon.svg
+-rw-rw-rw-   0        0        0       21 2023-06-06 01:12:59.000000 jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/script.js
+-rw-rw-rw-   0        0        0     1355 2023-06-07 07:34:01.000000 jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/style.css
+-rw-rw-rw-   0        0        0      260 2023-06-07 02:18:15.000000 jag-panzer-0.1.23/src/jag_panzer/assets/reject.html
+-rw-rw-rw-   0        0        0    22167 2023-07-20 11:57:25.000000 jag-panzer-0.1.23/src/jag_panzer/base_room.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.326971 jag-panzer-0.1.23/src/jag_panzer/cgi/
+-rw-rw-rw-   0        0        0        0 2023-06-09 00:00:24.000000 jag-panzer-0.1.23/src/jag_panzer/cgi/__init__.py
+-rw-rw-rw-   0        0        0     5087 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/cgi/burn_power.py
+-rw-rw-rw-   0        0        0      451 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/cgi/hitman.py
+-rw-rw-rw-   0        0        0     6691 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/cgi/jag.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.328958 jag-panzer-0.1.23/src/jag_panzer/cgi/templates/
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.329957 jag-panzer-0.1.23/src/jag_panzer/cgi/templates/light_httpd/
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.335955 jag-panzer-0.1.23/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/
+-rw-rw-rw-   0        0        0       91 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-accesslog.conf
+-rw-rw-rw-   0        0        0      306 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-cgi.conf
+-rw-rw-rw-   0        0        0      454 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/cgi/templates/light_httpd/conf-enabled/10-status.conf
+-rw-rw-rw-   0        0        0     2245 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf
+-rw-rw-rw-   0        0        0      403 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/cgi/templates/unit.service
+-rw-rw-rw-   0        0        0     2539 2023-06-08 21:42:17.000000 jag-panzer-0.1.23/src/jag_panzer/dir_list.py
+-rw-rw-rw-   0        0        0     2610 2023-07-12 20:58:31.000000 jag-panzer-0.1.23/src/jag_panzer/eztag.py
+-rw-rw-rw-   0        0        0      456 2023-07-12 02:05:06.000000 jag-panzer-0.1.23/src/jag_panzer/jag_util.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.252999 jag-panzer-0.1.23/src/jag_panzer/libs/
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.355152 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/
+-rw-rw-rw-   0        0        0    33822 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.377180 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/builder/
+-rw-rw-rw-   0        0        0    24393 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/builder/__init__.py
+-rw-rw-rw-   0        0        0    19078 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/builder/_html5lib.py
+-rw-rw-rw-   0        0        0    14919 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/builder/_htmlparser.py
+-rw-rw-rw-   0        0        0    14904 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/builder/_lxml.py
+-rw-rw-rw-   0        0        0    10077 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/css.py
+-rw-rw-rw-   0        0        0    41158 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/dammit.py
+-rw-rw-rw-   0        0        0     7195 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/diagnose.py
+-rw-rw-rw-   0        0        0    92716 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/element.py
+-rw-rw-rw-   0        0        0     7184 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/formatter.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.405165 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/
+-rw-rw-rw-   0        0        0    48391 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.441158 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/
+-rw-rw-rw-   0        0        0       23 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
+-rw-rw-rw-   0        0        0       30 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
+-rw-rw-rw-   0        0        0    19469 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
+-rw-rw-rw-   0        0        0        5 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
+-rw-rw-rw-   0        0        0       35 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
+-rw-rw-rw-   0        0        0    51495 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
+-rw-rw-rw-   0        0        0    10380 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
+-rw-rw-rw-   0        0        0       19 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
+-rw-rw-rw-   0        0        0     3546 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
+-rw-rw-rw-   0        0        0      124 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
+-rw-rw-rw-   0        0        0     2607 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
+-rw-rw-rw-   0        0        0     1115 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_builder.py
+-rw-rw-rw-   0        0        0     5114 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_builder_registry.py
+-rw-rw-rw-   0        0        0    17279 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_css.py
+-rw-rw-rw-   0        0        0    15451 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_dammit.py
+-rw-rw-rw-   0        0        0     1127 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_docs.py
+-rw-rw-rw-   0        0        0     2377 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_element.py
+-rw-rw-rw-   0        0        0     4148 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     3637 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_fuzz.py
+-rw-rw-rw-   0        0        0     8322 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_html5lib.py
+-rw-rw-rw-   0        0        0     6256 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_htmlparser.py
+-rw-rw-rw-   0        0        0     7635 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_lxml.py
+-rw-rw-rw-   0        0        0     5081 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_navigablestring.py
+-rw-rw-rw-   0        0        0    14274 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_pageelement.py
+-rw-rw-rw-   0        0        0    19877 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_soup.py
+-rw-rw-rw-   0        0        0     9016 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_tag.py
+-rw-rw-rw-   0        0        0    48129 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_tree.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.454137 jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/
+-rw-rw-rw-   0        0        0     4630 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/__init__.py
+-rw-rw-rw-   0        0        0     6842 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/__meta__.py
+-rw-rw-rw-   0        0        0    58152 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/css_match.py
+-rw-rw-rw-   0        0        0    47063 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/css_parser.py
+-rw-rw-rw-   0        0        0    10337 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/css_types.py
+-rw-rw-rw-   0        0        0     4053 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/pretty.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/py.typed
+-rw-rw-rw-   0        0        0     3374 2023-06-06 00:22:44.000000 jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/util.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.464146 jag-panzer-0.1.23/src/jag_panzer/libs/yattag/
+-rw-rw-rw-   0        0        0     1743 2023-03-03 09:07:48.000000 jag-panzer-0.1.23/src/jag_panzer/libs/yattag/__init__.py
+-rw-rw-rw-   0        0        0    18197 2020-08-06 21:26:32.000000 jag-panzer-0.1.23/src/jag_panzer/libs/yattag/doc.py
+-rw-rw-rw-   0        0        0    12029 2023-01-02 11:12:52.000000 jag-panzer-0.1.23/src/jag_panzer/libs/yattag/indentation.py
+-rw-rw-rw-   0        0        0        0 2019-12-25 20:07:02.000000 jag-panzer-0.1.23/src/jag_panzer/libs/yattag/py.typed
+-rw-rw-rw-   0        0        0    18081 2019-12-24 00:01:02.000000 jag-panzer-0.1.23/src/jag_panzer/libs/yattag/simpledoc.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.465143 jag-panzer-0.1.23/src/jag_panzer/mimes/
+-rw-rw-rw-   0        0        0     2762 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/mimes/mime_types_base.py
+-rw-rw-rw-   0        0        0     1938 2023-06-03 17:16:43.000000 jag-panzer-0.1.23/src/jag_panzer/response_codes.py
+-rw-rw-rw-   0        0        0     7874 2023-07-21 23:21:40.000000 jag-panzer-0.1.23/src/jag_panzer/server.py
+-rwxrwxrwx   0        0        0       12 2023-06-07 01:47:22.000000 jag-panzer-0.1.23/src/jag_panzer/test.cmd
+drwxrwxrwx   0        0        0        0 2023-07-21 23:37:30.306970 jag-panzer-0.1.23/src/jag_panzer.egg-info/
+-rw-rw-rw-   0        0        0      561 2023-07-21 23:37:30.000000 jag-panzer-0.1.23/src/jag_panzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4010 2023-07-21 23:37:30.000000 jag-panzer-0.1.23/src/jag_panzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 23:37:30.000000 jag-panzer-0.1.23/src/jag_panzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-21 23:37:30.000000 jag-panzer-0.1.23/src/jag_panzer.egg-info/top_level.txt
```

### Comparing `jag-panzer-0.1.21/PKG-INFO` & `jag-panzer-0.1.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.1.21
+Version: 0.1.23
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.1.21/setup.cfg` & `jag-panzer-0.1.23/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206a 6167 2d70 616e 7a65 720d 0a76   = jag-panzer..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e32 310d  ersion = 0.1.21.
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e32 330d  ersion = 0.1.23.
 00000030: 0a61 7574 686f 7220 3d20 4d72 2e4b 6c65  .author = Mr.Kle
 00000040: 696e 6572 0d0a 6175 7468 6f72 5f65 6d61  iner..author_ema
 00000050: 696c 203d 206d 6567 6161 6472 656e 616c  il = megaadrenal
 00000060: 696e 6531 3035 3540 676d 6169 6c2e 636f  ine1055@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2053 696d 706c 6520 4854 5450 2073 6572   Simple HTTP ser
 00000090: 7665 7220 616c 6c6f 7769 6e67 2070 7572  ver allowing pur
```

### Comparing `jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/download_icon.svg` & `jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/download_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/file_icon.svg` & `jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/file_icon.svg`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/assets/dir_listing/style.css` & `jag-panzer-0.1.23/src/jag_panzer/assets/dir_listing/style.css`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/base_room.py` & `jag-panzer-0.1.23/src/jag_panzer/base_room.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,758 +1,801 @@
-from jag_util import dict_pretty_print
-
-
-_room_echo = '[Request Evaluator]'
-_rebind = print
-
-def conlog(*args):
-	print(_room_echo, *args)
-
-
-
-def _default_room(request, response, services):
-	conlog('Executing default action', request.abspath)
-
-	# for this to work it has to be a GET request
-	if request.method == 'get':
-
-		# anything that is not inside the server shall get rejected
-		if not request.abspath.resolve().is_relative_to(request.srv_res.doc_root):
-			request.reject()
-			return
-
-		# first check if path explicitly points to a file
-		if request.abspath.is_file():
-			services.serve_file()
-			return
-
-		# if it's not a file - check whether the target dir has an index.html file
-		if (request.abspath / 'index.html').is_file():
-			services.serve_dir_index()
-			return
-
-		# if it's just a directory - list it
-		if request.abspath.is_dir() and request.srv_res.cfg['dir_listing']['enabled']:
-			services.list_dir()
-			return
-
-
-	# otherwise - reject
-	request.reject()
-
-
-
-# A bunch of default services the server can provide
-class sv_services:
-	"""
-	A bunch of default services the server can provide.
-	Most notable one: Serving GET requests
-	"""
-	def __init__(self, request, response):
-		self.request = request
-		self.response = response
-
-	# Serve a file to the client in a CDN manner
-	# If no file is provided - serve path from the request
-	def serve_file(self, tgt_file=None, respect_range=True):
-		"""
-		Serve a file to the client.
-		It's possible to specify a target file.
-		If no target file is specified, then reuqest path is used.
-		- tgt_file: Path to the file to serve, defaults to request path.
-		- respect_range: Take the "Range" header into account.
-		"""
-		request = self.request
-		response = self.response
-
-		if not request.abspath.is_file():
-			self.request.reject()
-			return
-
-		# all good - set content type and send the shit
-		response.content_type = (
-			request.srv_res.mimes['signed'].get(request.abspath.suffix)
-			or
-			'application/octet-stream'
-		)
-
-		# if the size is too big for a single flush - stream in chunks
-		# This is very important, because serving a 2kb svg in chunks slows the response time
-		# and serving an 18gb .mkv Blu-ray remux in a single flush is impossible
-		if request.abspath.stat().st_size > request.srv_res.cfg['buffers']['max_file_len']:
-			with open(str(request.abspath), 'r+b') as f:
-				# if request comes with a Range header - try serving the requested byterange
-				# '0-' VERY funny, fuck right off
-				if request.byterange and (request.headers.get('range', 'bytes=0-').strip() != 'bytes=0-') and respect_range:
-					conlog('The client has fucked us over:', request.headers.get('range', '0-').strip())
-					response.serve_range(f)
-				else:
-					response.stream_buffer(f, (1024*1024)*5)
-		else:
-			response.flush_buffer(request.abspath.read_bytes())
-
-		self.request.terminate()
-
-	# List directory as an html page
-	def list_dir(self):
-		"""
-		- Set content type to text/html
-		- Progressively generate listing for a directory and stream it to the client
-		- Close connection
-		"""
-		self.response.content_type = 'text/html'
-
-		with self.response.stream_bytechunks() as stream:
-			for chunk in self.request.srv_res.list_dir.dir_as_html(self.request.abspath):
-				stream.send(chunk)
-
-
-	# Serve "index.html" from the requested path
-	# according to server config
-	def serve_dir_index(self):
-		"""
-		Serve "index.html" from the requested path
-		If the file mentioned above doesn't exist in the dir - reject
-		"""
-		if not (self.request.abspath / 'index.html').is_file():
-			self.request.reject()
-
-		self.response.content_type = 'text/html'
-		self.response.flush_buffer(
-			(self.request.abspath / 'index.html').read_bytes()
-		)
-
-	# Because why not
-	def default(self):
-		"""
-		Execute default stack of actions:
-		- if it's a GET request (reject otherwise):
-			- If request path is not relative to the doc root - reject
-			- If request points to a file - serve it
-			- If request points to a directory - list it IF dir listing is enabled
-		"""
-		_default_room(self.request, self.response, self)
-
-
-
-
-
-
-
-# Stream chunks
-class _chunkstream:
-	def __init__(self, request, cl_con, self_terminate):
-		self.cl_con = cl_con
-		self.request = request
-		self.auto_term = self_terminate
-
-	def __enter__(self):
-		return self
-
-	def __exit__(self, type, value, traceback):
-		self.cl_con.sendall(b'0\r\n\r\n')
-		# No auto termination, because it's speculated,
-		# that it's possible to send some sort of trailing headers or whatever
-		if self.auto_term:
-			self.request.terminate()
-
-	def send(self, data):
-		# send the chunk size
-		self.cl_con.sendall(f"""{hex(len(data)).lstrip('0x')}\r\n""".encode())
-		# send the chunk itself
-		self.cl_con.sendall(data)
-		# send separator
-		self.cl_con.sendall(b'\r\n')
-
-
-
-
-# Read part of a buffer in chunks (start:end)
-# todo: There are 0 validations
-# (neither end or start can be negative)
-# (end cannot be smaller than start)
-# (start and end cannot be the same)
-# (start and end should not result into 0 bytes read)
-
-# src  -----------------------
-# rng        ^         ^      
-# prog       -----            
-# want            ---------   
-# let             ------      
-
-# RANGES ARE INCLUSIVE IN HTTP !
-class aligned_buf_read:
-	def __init__(self, buf, start, end):
-		# START is inclusive
-		# END is NOT inclusive
-		self.buf = buf
-		self.start = start
-		self.end = end
-		self.target_amount = end - start
-		self.progress = 0
-
-		# seek to the beginning
-		self.buf.seek(start, 0)
-
-	def read(self, amt):
-		# max(smallest, min(n, largest))
-		# Todo: is this slow ?
-		allowed_amount = max(0, min(amt, self.end - self.progress))
-		chunk = self.buf.read(allowed_amount)
-		self.progress += allowed_amount
-		return chunk
-
-
-
-
-class sv_response:
-	def __init__(self, request, cl_con, srv_res):
-		self.request = request
-		self.cl_con = cl_con
-		self.srv_res = srv_res
-		self.headers = {
-			'Server': 'Jag',
-		}
-
-		self.content_type = 'application/octet-stream'
-		self.code = 200
-
-		self.offered_services = sv_services(self.request, self)
-
-	# dump headers and response code to the client
-	def send_preflight(self):
-		"""
-		Dump headers and response code to the client
-		"""
-
-		# send response code
-		self.cl_con.sendall(
-			f"""HTTP/1.1 {self.srv_res.response_codes[self.code]}\r\n""".encode()
-		)
-
-		# important todo: better way of achieving this
-		self.headers['Content-Type'] = self.content_type
-
-		# send headers
-		for header_name, header_value in self.headers.items():
-			self.cl_con.sendall(
-				f"""{header_name}: {header_value}\r\n""".encode()
-			)
-
-		# Send an extra \r\n to indicate the end of headers
-		self.cl_con.sendall('\r\n'.encode())
-
-		# important todo: There's a built-in way to make functions only fire once
-		# Yes, BUT, it costs A LOT of time and effort for the machine
-		# Such a simple buttplug is WAY more efficient
-		self.send_preflight = lambda: None
-
-	# mark response as a download
-	def mark_as_xfiles(self, filename):
-		"""
-		This is needed if you want the response body to be treated
-		as a file download by the client.
-		Useful when a media file, like .mp4 video should be downloaded
-		by the client instead of playing back.
-		"""
-		self.headers['Content-Disposition'] = f'attachment; filename="{str(filename)}"'
-
-	# - Send headers to the client
-	# - Send the entirety of the provided buffer/bytes in one go
-	# - Collapse connection
-	def flush_buffer(self, data):
-		if not isinstance(data, bytes):
-			data = data.getvalue()
-
-		# important todo: the response should either be chunked or have Content-Length header
-		self.headers['Content-Length'] = len(data)
-
-		# send headers
-		self.send_preflight()
-
-		# send the body
-		self.cl_con.sendall(data)
-
-		# terminate
-		self.request.terminate()
-
-	def stream_bytechunks(self, self_terminate=True):
-		"""
-		Stream data to the client in HTTP chunks:
-		- set 'Transfer-Encoding' header to 'chunked'
-		- Dump headers
-		- Start streaming chunks:
-			- This returns an object for use with "with" keyword.
-			- The object only has 1 method: send()
-			  Which only takes 1 argument: Bytes to send
-		"""
-
-		# This cannot be otherwise
-		self.headers['Transfer-Encoding'] = 'chunked'
-		# It's impossible to stream multiple groups of chunks
-		self.send_preflight()
-
-		return _chunkstream(self.request, self.cl_con, self_terminate)
-
-	# Automated action:
-	# - Add 'Transfer-Encoding: chunked' header
-	# - Send headers to the client
-	# - Stream the entirety of the provided buffer in chunks
-	# - Collapse the connection
-	def stream_buffer(self, data, chunk_size=None):
-		"""
-		Send the data in chunks.
-		data = io.BytesIO object.
-		chunk_size = the size of a single chunk in bytes, default to server config
-		Example usage: Pass buffer of an open file to stream it to the client.
-		"""
-
-		# The response is EITHER chunked OR has Content-Length
-		self.headers['Transfer-Encoding'] = 'chunked'
-
-		# first - dump headers
-		self.send_preflight()
-
-		# Safety (tin foil hat): Move the carret to the very beginning of the buffer
-		data.seek(0, 0)
-		# stream chunks
-		with self.stream_bytechunks() as stream:
-			while True:
-				# read chunk
-				chunk = data.read(
-					chunk_size or self.srv_res.cfg['buffers']['bufstream_chunk_len']
-				)
-				# check if there's still any data
-				if not chunk:
-					break
-				stream.send(chunk)
-
-
-	# Serve specified buffer according to the Range header
-	# important todo: This is 100% raw/bare
-	# nothing is checked or validated
-	def serve_range(self, buf):
-		# Set code to partial-content
-		self.code = 206
-		# It'd be stupid not to do it this way...
-		self.headers['Transfer-Encoding'] = 'chunked'
-		self.send_preflight()
-
-		buf_size = buf.seek(0, 2)
-
-		# begin streaming
-		with self.stream_bytechunks() as stream:
-			# stream all chunk groups
-			# (order is preserved)
-			for chunk_start, chunk_end in self.request.byterange:
-				# Python is amazing: array[37:None] is a valid syntax
-				_start = chunk_start
-				_end = chunk_end or buf_size
-
-				conlog('Serving partial content', self.request.byterange, _start, _end)
-
-				# If only end is specified - stream suffix
-				# Todo: current implementation requires calculating
-				# start offset, which means that buffer should be of known size
-				if chunk_end and not chunk_start:
-					_end = buf_size
-					_start = _end - chunk_end
-
-				aligned_reader = aligned_buf_read(buf, _start, _end)
-				while True:
-					data = aligned_reader.read(self.srv_res.cfg['buffers']['bufstream_chunk_len'])
-					if not data:
-						break
-					stream.send(data)
-
-
-
-
-
-
-class cl_request:
-	def __init__(self, cl_con, cl_addr, srv_res):
-		self.cl_con = cl_con
-		self.cl_addr = cl_addr
-		self.srv_res = srv_res
-
-		self.headers = {}
-
-		# Initialize the response class
-		# Early init of this class is needed
-		# for rejecting certain requests
-		self.response = sv_response(self, cl_con, srv_res)
-
-		# Some widely-used headers are lazily processed
-		# for easier use
-		self._cookie = None
-		self._cache_control = None
-		self._accept = None
-		self._byterange = None
-
-		# Try/Except in case of malformed request
-		# Why bother?
-		# It's client's responsibility to perform good requests
-		try:
-			self._eval_request()
-		except Exception as e:
-			self.reject(400)
-			raise e
-		
-
-	# Init
-	# =================
-
-	# Keep eating bytes from the client
-	# until the entire Request Header arrives
-	def collect_head_buf(self):
-
-		io = self.srv_res.pylib.io
-
-		self.head_buf = io.BytesIO()
-		self.body_buf = io.BytesIO()
-
-		double_rn = 0
-		expect_r = False
-
-		# important todo: This is extremely (relatively) slow
-		# simple http server from python base library does something like
-		# do 1 byte receive from client till \r\n\r\n
-		# OR
-		# Read 65535 bytes and then process the thing
-		while True:
-			data = self.cl_con.recv(65535)
-			for idx, char in enumerate(data):
-				# conlog('Char:', chr(char).encode())
-
-				if char != 10 and char != 13:
-					# conlog('^ no match, abort')
-					expect_r = False
-					double_rn = 0
-					continue
-
-				if char == 13:
-					# conlog('^ found 13')
-					expect_r = True
-					continue
-
-				if expect_r and char != 10:
-					# conlog('^ is not 10, abort')
-					expect_r = False
-					double_rn = 0
-					continue
-
-				if expect_r and char == 10:
-					# conlog('^ found 10, +1')
-					double_rn += 1
-					expect_r = False
-
-				if double_rn == 2:
-					# conlog('Writing to body buffer:', bytes(data[(idx+1):]))
-					self.body_buf.write(bytes(data[(idx+1):]))
-					self.head_buf.write(bytes(data[:idx]))
-					break
-
-			if double_rn == 2:
-				conlog('Header Buf', self.head_buf.getvalue().decode())
-				break
-
-			self.head_buf.write(data)
-
-			if self.head_buf.tell() >= self.srv_res.cfg['buffers']['max_header_len']:
-				self.response.reject(431)
-
-	# Request evaluation has a dedicated function for easier error handling
-	def _eval_request(self):
-		# io = self.srv_res.pylib.io
-		# sys = self.srv_res.pylib.sys
-		urllib = self.srv_res.pylib.urllib
-		Path = self.srv_res.pylib.Path
-
-		# Fully custom method of receiving the Request Header
-		# gives a lot of benefits
-		self.collect_head_buf()
-
-		# raw bytes of the header
-		header_data = self.head_buf.getvalue()
-		conlog(header_data.decode())
-
-		# split header into lines
-		header_data = header_data.decode().split('\r\n')
-		conlog('\n'.join(header_data))
-
-		# First line of the header is always the request method, path and http version
-		# It's up to the client to send valid data
-		self.method, self.path, self.protocol = header_data[0].split(' ')
-		conlog(self.method, self.path, self.protocol)
-		self.method = self.method.lower()
-
-		# deconstruct the url into components
-		parsed_url = urllib.parse.urlparse(self.path)
-
-		# important todo: lazy processing
-		# first - evaluate query params
-		self.query_params = {k:(''.join(v)) for (k,v) in urllib.parse.parse_qs(parsed_url.query, True).items()}
-
-		# then, evaluate path
-		decoded_url_path = urllib.parse.unquote(parsed_url.path)
-		self.abspath = self.srv_res.doc_root / Path(decoded_url_path.lstrip('/'))
-		self.relpath = Path(decoded_url_path.lstrip('/'))
-		self.trimpath = self.relpath
-
-		# Delete the first line as it's no longer needed
-		del header_data[0]
-
-		# parse the remaining headers into a dict
-		request_dict = {}
-		for line in header_data:
-			# skip empty stuff
-			if line.strip() == '':
-				continue
-			line_split = line.split(': ')
-			request_dict[line_split[0].lower()] = ': '.join(line_split[1:])
-
-		dict_pretty_print(request_dict)
-
-		self.headers = request_dict
-
-
-	# Actions
-	# =================
-
-	# Properly collapse the tunnel between server and client
-	def terminate(self):
-		socket = self.srv_res.pylib.socket
-		self.cl_con.shutdown(socket.SHUT_RDWR)
-		self.cl_con.close()
-
-		# Termination is only possible once
-		self.terminate = lambda: None
-
-	# Send a very simple html document
-	# with a short description of the provided Status Code
-	def reject(self, code=401, hint=''):
-		self.response.code = code
-		self.response.content_type = 'text/html'
-		self.response.flush_buffer(
-			self.srv_res.reject_precache
-			.replace(b'$$reason', self.srv_res.response_codes[code].encode())
-			.replace(b'$$hint', str(hint).encode())
-		)
-
-	# I cannot be bothered. Here, have *args and fuckoff
-	def match_path(self, action_dict, *args, trim_path=True):
-		"""
-		Sample set/list:
-		{
-			('/pootis/sandwich/dispenser', func_name1),
-			('/pootis',                    func_name2),
-		}
-		"""
-		comparator = '/' + self.relpath.as_posix()
-
-		for rpath, func in action_dict:
-			# print(rpath, 'startswith', )
-			if comparator.startswith(rpath):
-				if trim_path:
-					self.trimpath = self.srv_res.pylib.Path(comparator.lstrip(rpath))
-				return func(self, self.response, self.response.offered_services, *args)
-
-		# if no match was found - return false
-		return False
-
-
-	def read_body_stream(self):
-		"""
-		(Generator)
-		Progressively read the incoming body of the request
-		"""
-		content_length = int(self.headers['content-length'])
-		read_progress = self.body_buf.seek(0, 2)
-		yield self.body_buf.getvalue()
-		while True:
-			if read_progress >= content_length:
-				break
-			# todo: finetune this value
-			# or expose it in the config
-			received_data = self.cl_con.recv(65535)
-			yield received_data
-			read_progress += len(received_data)
-
-
-	# Utility
-	# =================
-	def parse_kv(self, kvs, separator=',', key_to_lower=True):
-		pairs = kvs.split(separator)
-		result = {}
-		for pair in pairs:
-			pair_split = pair.split('=')
-			if key_to_lower:
-				pair_split[0] = pair_split[0].upper()
-
-			if len(pair_split) == 1:
-				result[pair_split[0]] = True
-				continue
-
-			val = '='.join(pair_split[1:])
-			# important todo: is this really needed ?
-			try:
-				val = float(val)
-			# important todo: generic exceptions are very bad
-			except:
-				pass
-			try:
-				val = int(val)
-			except:
-				pass
-
-			result[pair_split[0]] = val
-
-		return result
-
-
-	# Processed headers
-	# =================
-
-	@property
-	def cookie(self):
-		"""
-		Nicely formatted cookie header
-		"""
-		if self._cookie:
-			return self._cookie
-
-		cookie_data = self.headers.get('cookie')
-		if not cookie_data:
-			return None
-
-		self._cookie = self.parse_kv(cookie_data, separator=';')
-
-		return self._cookie
-
-	# Even though server doesn't support advanced caching...
-	@property
-	def cache_control(self):
-		if self._cache_control:
-			return self._cache_control
-
-		cache_data = self.headers.get('cache-control')
-		if not cache_data:
-			return None
-
-		self._cache_control = self.parse_kv(cookie_data, separator=',')
-
-		return self._cache_control
-
-
-	@property
-	def byterange(self):
-		if self._byterange:
-			return self._byterange
-
-		range_data = self.headers.get('range')
-		if not range_data:
-			return None
-
-		# todo: it's always assumed that range is in bytes
-		ranges = range_data.split('=')[1].split(',')
-
-		self._byterange = []
-		for chunk in ranges:
-			chunk_split = chunk.strip().split('-')
-			rstart = max(int(chunk_split[0]) - 1, 0) if chunk_split[0] else None
-			rend =   max(int(chunk_split[1]) - 1, 0) if chunk_split[1] else None
-			self._byterange.append(
-				(rstart, rend)
-			)
-
-		return self._byterange
-
-
-
-
-
-
-# The server creates "rooms" for every incoming connection.
-# The Base Room does some setup, like evaluating the request.
-# Further actions depend on the server setup:
-# If callback function is specified, then it's triggered
-# without any automatic actions
-# If callback function is NOT specified, then server provides
-# Some of its default services
-def base_room(cl_con, cl_addr, srv_res):
-	import sys, traceback
-	import importlib.util
-
-	try:
-		# precache some commonly-used python libraries
-		# important todo: is this even needed?
-		srv_res.reload_libs()
-
-		# Evaluate the request
-		evaluated_request = cl_request(cl_con, cl_addr, srv_res)
-		conlog('Initialized basic room, evaluated request')
-
-		# Create service object
-		# offered_services = sv_services(evaluated_request, evaluated_request.response)
-
-		# Now either pass the control to the room specified in the config
-		# or the default room
-		if srv_res.cfg['room_file']:
-			spec = importlib.util.spec_from_file_location('main', str(srv_res.cfg['room_file']))
-			custom_func = importlib.util.module_from_spec(spec)
-			spec.loader.exec_module(custom_func)
-			custom_func.main(
-				evaluated_request,
-				evaluated_request.response,
-				evaluated_request.response.offered_services
-			)
-		else:
-			_default_room(
-				evaluated_request,
-				evaluated_request.response,
-				evaluated_request.response.offered_services
-			)
-
-	except Exception as err:
-		conlog(
-			''.join(
-				traceback.format_exception(
-					type(err),
-					err,
-					err.__traceback__
-				)
-			)
-		)
-
-		_trback = ''.join(
-			traceback.format_exception(
-				type(err),
-				err,
-				err.__traceback__
-			)
-		)
-		cl_con.sendall('HTTP/1.1 500 Internal Server Error\r\n'.encode())
-		_rcontent = f"""<!DOCTYPE HTML>
-			<html>
-				<head>
-					<meta http-equiv="Content-Type" content="text/html;charset=utf-8">
-					<title>Rejected</title>
-				</head>
-				<body>
-					<h1>500 Internal Server Error</h1>
-					<h3>Server: Jag</h3>
-					<p style="white-space: pre;">{_trback}</p>
-				</body>
-			</html>
-		"""
-		cl_con.sendall(f'Content-Length: {len(_rcontent)}\r\n\r\n'.encode())
-		cl_con.sendall(_rcontent.encode())
-
-		raise err
-
-
-	cl_con.close()
-	sys.exit()
-
-
-
+from pathlib import Path
+import sys
+from mstime import perftest
+
+
+sys.path.append(str(Path(__file__).parent))
+
+from jag_util import dict_pretty_print
+
+
+_room_echo = '[Request Evaluator]'
+_rebind = print
+
+
+def conlog(*args):
+	return
+	print(_room_echo, *args)
+
+
+
+def _default_room(request, response, services):
+	conlog('Executing default action', request.abspath)
+
+	# for this to work it has to be a GET request
+	if request.method == 'get':
+
+		# anything that is not inside the server shall get rejected
+		if not request.abspath.resolve().is_relative_to(request.srv_res.doc_root):
+			request.reject()
+			return
+
+		# first check if path explicitly points to a file
+		if request.abspath.is_file():
+			services.serve_file()
+			return
+
+		# if it's not a file - check whether the target dir has an index.html file
+		if (request.abspath / 'index.html').is_file():
+			services.serve_dir_index()
+			return
+
+		# if it's just a directory - list it
+		if request.abspath.is_dir() and request.srv_res.cfg['dir_listing']['enabled']:
+			services.list_dir()
+			return
+
+
+	# otherwise - reject
+	request.reject()
+
+
+
+class sv_services:
+	"""
+	A bunch of default services the server can provide.
+	Most notable one: Serving GET requests
+	"""
+	def __init__(self, request, response):
+		self.request = request
+		self.response = response
+
+	# Serve a file to the client in a CDN manner
+	# If no file is provided - serve path from the request
+	def serve_file(self, tgt_file=None, respect_range=True, _force_oneflush=False):
+		"""
+		Serve a file to the client.
+		It's possible to specify a target file.
+		If no target file is specified, then reuqest path is used.
+		- tgt_file: Path to the file to serve, defaults to request path.
+		- respect_range: Take the "Range" header into account.
+		"""
+		request = self.request
+		response = self.response
+
+		if not request.abspath.is_file():
+			self.request.reject()
+			return
+
+		# all good - set content type and send the shit
+		response.content_type = (
+			request.srv_res.mimes['signed'].get(request.abspath.suffix)
+			or
+			'application/octet-stream'
+		)
+
+		# Basically, debugging
+		if _force_oneflush:
+			response.flush_buffer(request.abspath.read_bytes())
+			self.request.terminate()
+			return
+
+		# if the size is too big for a single flush - stream in chunks
+		# This is very important, because serving a 2kb svg in chunks slows the response time
+		# and serving an 18gb .mkv Blu-Ray remux in a single flush is impossible
+		if request.abspath.stat().st_size > request.srv_res.cfg['buffers']['max_file_len']:
+			with open(str(request.abspath), 'r+b') as f:
+				# if request comes with a Range header - try serving the requested byterange
+				# '0-' VERY funny, fuck right off
+				if request.byterange and (request.headers.get('range', 'bytes=0-').strip() != 'bytes=0-') and respect_range:
+					conlog('The client has fucked us over:', request.headers.get('range', '0-').strip())
+					response.serve_range(f)
+				else:
+					response.stream_buffer(f, (1024*1024)*5)
+		else:
+			response.flush_buffer(request.abspath.read_bytes())
+
+		self.request.terminate()
+
+	# List directory as an html page
+	def list_dir(self):
+		"""
+		- Set content type to text/html
+		- Progressively generate listing for a directory and stream it to the client
+		- Close connection
+		"""
+		from dir_list import dirlist
+		lister = dirlist(self.request.srv_res)
+
+		self.response.content_type = 'text/html'
+
+		with self.response.stream_bytechunks() as stream:
+			for chunk in self.request.srv_res.list_dir.dir_as_html(self.request.abspath):
+				stream.send(chunk)
+
+
+	# Serve "index.html" from the requested path
+	# according to server config
+	def serve_dir_index(self):
+		"""
+		Serve "index.html" from the requested path
+		If the file mentioned above doesn't exist in the dir - reject
+		"""
+		if not (self.request.abspath / 'index.html').is_file():
+			self.request.reject()
+
+		self.response.content_type = 'text/html'
+		self.response.flush_buffer(
+			(self.request.abspath / 'index.html').read_bytes()
+		)
+
+	# Because why not
+	def default(self):
+		"""
+		Execute default stack of actions:
+		- if it's a GET request (reject otherwise):
+			- If request path is not relative to the doc root - reject
+			- If request points to a file - serve it
+			- If request points to a directory - list it IF dir listing is enabled
+		"""
+		_default_room(self.request, self.response, self)
+
+
+
+
+
+
+
+# Stream chunks
+class _chunkstream:
+	def __init__(self, request, cl_con, self_terminate):
+		self.cl_con = cl_con
+		self.request = request
+		self.auto_term = self_terminate
+
+	def __enter__(self):
+		return self
+
+	def __exit__(self, type, value, traceback):
+		self.cl_con.sendall(b'0\r\n\r\n')
+		# No auto termination, because it's speculated,
+		# that it's possible to send some sort of trailing headers or whatever
+		if self.auto_term:
+			self.request.terminate()
+
+	def send(self, data):
+		# send the chunk size
+		self.cl_con.sendall(f"""{hex(len(data)).lstrip('0x')}\r\n""".encode())
+		# send the chunk itself
+		self.cl_con.sendall(data)
+		# send separator
+		self.cl_con.sendall(b'\r\n')
+
+
+
+
+# Read part of a buffer in chunks (start:end)
+# todo: There are 0 validations
+# (neither end or start can be negative)
+# (end cannot be smaller than start)
+# (start and end cannot be the same)
+# (start and end should not result into 0 bytes read)
+
+# src  -----------------------
+# rng        ^         ^      
+# prog       -----            
+# want            ---------   
+# let             ------      
+
+# RANGES ARE INCLUSIVE IN HTTP !
+class aligned_buf_read:
+	def __init__(self, buf, start, end):
+		# START is inclusive
+		# END is NOT inclusive
+		self.buf = buf
+		self.start = start
+		self.end = end
+		self.target_amount = end - start
+		self.progress = 0
+
+		# seek to the beginning
+		self.buf.seek(start, 0)
+
+	def read(self, amt):
+		# max(smallest, min(n, largest))
+		# Todo: is this slow ?
+		allowed_amount = max(0, min(amt, self.end - self.progress))
+		chunk = self.buf.read(allowed_amount)
+		self.progress += allowed_amount
+		return chunk
+
+
+
+
+class sv_response:
+	def __init__(self, request, cl_con, srv_res):
+		self.request = request
+		self.cl_con = cl_con
+		self.srv_res = srv_res
+		self.headers = {
+			'Server': 'Jag',
+		}
+
+		self.content_type = 'application/octet-stream'
+		self.code = 200
+
+		self.offered_services = sv_services(self.request, self)
+
+	# dump headers and response code to the client
+	def send_preflight(self):
+		"""
+		Dump headers and response code to the client
+		"""
+
+		# send response code
+		self.cl_con.sendall(
+			f"""HTTP/1.1 {self.srv_res.response_codes[self.code]}\r\n""".encode()
+		)
+
+		# important todo: better way of achieving this
+		self.headers['Content-Type'] = self.content_type
+
+		# send headers
+		for header_name, header_value in self.headers.items():
+			self.cl_con.sendall(
+				f"""{header_name}: {header_value}\r\n""".encode()
+			)
+
+		# Send an extra \r\n to indicate the end of headers
+		self.cl_con.sendall('\r\n'.encode())
+
+		# important todo: There's a built-in way to make functions only fire once
+		# Yes, BUT, it costs A LOT of time and effort for the machine
+		# Such a simple buttplug is WAY more efficient
+		self.send_preflight = lambda: None
+
+	# mark response as a download
+	def mark_as_xfiles(self, filename):
+		"""
+		This is needed if you want the response body to be treated
+		as a file download by the client.
+		Useful when a media file, like .mp4 video should be downloaded
+		by the client instead of playing back.
+		"""
+		self.headers['Content-Disposition'] = f'attachment; filename="{str(filename)}"'
+
+	# - Send headers to the client
+	# - Send the entirety of the provided buffer/bytes in one go
+	# - Collapse connection
+	def flush_buffer(self, data):
+		if not isinstance(data, bytes):
+			data = data.getvalue()
+
+		# important todo: the response should either be chunked or have Content-Length header
+		self.headers['Content-Length'] = len(data)
+
+		# send headers
+		self.send_preflight()
+
+		# send the body
+		self.cl_con.sendall(data)
+
+		# terminate
+		self.request.terminate()
+
+	def stream_bytechunks(self, self_terminate=True):
+		"""
+		Stream data to the client in HTTP chunks:
+		- set 'Transfer-Encoding' header to 'chunked'
+		- Dump headers
+		- Start streaming chunks:
+			- This returns an object for use with "with" keyword.
+			- The object only has 1 method: send()
+			  Which only takes 1 argument: Bytes to send
+		"""
+
+		# This cannot be otherwise
+		self.headers['Transfer-Encoding'] = 'chunked'
+		# It's impossible to stream multiple groups of chunks
+		self.send_preflight()
+
+		return _chunkstream(self.request, self.cl_con, self_terminate)
+
+	# Automated action:
+	# - Add 'Transfer-Encoding: chunked' header
+	# - Send headers to the client
+	# - Stream the entirety of the provided buffer in chunks
+	# - Collapse the connection
+	def stream_buffer(self, data, chunk_size=None):
+		"""
+		Send the data in chunks.
+		data = io.BytesIO object.
+		chunk_size = the size of a single chunk in bytes, default to server config
+		Example usage: Pass buffer of an open file to stream it to the client.
+		"""
+
+		# The response is EITHER chunked OR has Content-Length
+		self.headers['Transfer-Encoding'] = 'chunked'
+
+		# first - dump headers
+		self.send_preflight()
+
+		# Safety (tin foil hat): Move the carret to the very beginning of the buffer
+		data.seek(0, 0)
+		# stream chunks
+		with self.stream_bytechunks() as stream:
+			while True:
+				# read chunk
+				chunk = data.read(
+					chunk_size or self.srv_res.cfg['buffers']['bufstream_chunk_len']
+				)
+				# check if there's still any data
+				if not chunk:
+					break
+				stream.send(chunk)
+
+
+	# Serve specified buffer according to the Range header
+	# important todo: This is 100% raw/bare
+	# nothing is checked or validated
+	def serve_range(self, buf):
+		# Set code to partial-content
+		self.code = 206
+		# It'd be stupid not to do it this way...
+		self.headers['Transfer-Encoding'] = 'chunked'
+		self.send_preflight()
+
+		buf_size = buf.seek(0, 2)
+
+		# begin streaming
+		with self.stream_bytechunks() as stream:
+			# stream all chunk groups
+			# (order is preserved)
+			for chunk_start, chunk_end in self.request.byterange:
+				# Python is amazing: array[37:None] is a valid syntax
+				_start = chunk_start
+				_end = chunk_end or buf_size
+
+				conlog('Serving partial content', self.request.byterange, _start, _end)
+
+				# If only end is specified - stream suffix
+				# Todo: current implementation requires calculating
+				# start offset, which means that buffer should be of known size
+				if chunk_end and not chunk_start:
+					_end = buf_size
+					_start = _end - chunk_end
+
+				aligned_reader = aligned_buf_read(buf, _start, _end)
+				while True:
+					data = aligned_reader.read(self.srv_res.cfg['buffers']['bufstream_chunk_len'])
+					if not data:
+						break
+					stream.send(data)
+
+
+
+
+
+
+class cl_request:
+	def __init__(self, cl_con, cl_addr, srv_res):
+		self.cl_con = cl_con
+		self.cl_addr = cl_addr
+		self.srv_res = srv_res
+
+		self.headers = {}
+
+		# Initialize the response class
+		# Early init of this class is needed
+		# for rejecting certain requests
+		self.response = sv_response(self, cl_con, srv_res)
+
+		# Some widely-used headers are lazily processed
+		# for easier use
+		self._cookie = None
+		self._cache_control = None
+		self._accept = None
+		self._byterange = None
+
+		# Try/Except in case of malformed request
+		# Why bother?
+		# It's client's responsibility to perform good requests
+		try:
+			self._eval_request()
+		except Exception as e:
+			self.reject(400)
+			raise e
+		
+
+	# Init
+	# =================
+
+	# Keep eating bytes from the client
+	# until the entire Request Header arrives
+	def collect_head_buf(self):
+
+		io = self.srv_res.pylib.io
+
+		self.head_buf = io.BytesIO()
+		self.body_buf = io.BytesIO()
+
+		double_rn = 0
+		expect_r = False
+
+		# important todo: This is extremely (relatively) slow
+		# simple http server from python base library does something like
+		# do 1 byte receive from client till \r\n\r\n
+		# OR
+		# Read 65535 bytes and then process the thing
+		while True:
+			data = self.cl_con.recv(65535)
+			for idx, char in enumerate(data):
+				# conlog('Char:', chr(char).encode())
+
+				if char != 10 and char != 13:
+					# conlog('^ no match, abort')
+					expect_r = False
+					double_rn = 0
+					continue
+
+				if char == 13:
+					# conlog('^ found 13')
+					expect_r = True
+					continue
+
+				if expect_r and char != 10:
+					# conlog('^ is not 10, abort')
+					expect_r = False
+					double_rn = 0
+					continue
+
+				if expect_r and char == 10:
+					# conlog('^ found 10, +1')
+					double_rn += 1
+					expect_r = False
+
+				if double_rn == 2:
+					# conlog('Writing to body buffer:', bytes(data[(idx+1):]))
+					self.body_buf.write(bytes(data[(idx+1):]))
+					self.head_buf.write(bytes(data[:idx]))
+					break
+
+			if double_rn == 2:
+				conlog('Header Buf', self.head_buf.getvalue().decode())
+				break
+
+			self.head_buf.write(data)
+
+			if self.head_buf.tell() >= self.srv_res.cfg['buffers']['max_header_len']:
+				self.response.reject(431)
+
+	# Request evaluation has a dedicated function for easier error handling
+	def _eval_request(self):
+		# io = self.srv_res.pylib.io
+		# sys = self.srv_res.pylib.sys
+		urllib = self.srv_res.pylib.urllib
+		Path = self.srv_res.pylib.Path
+
+		# Fully custom method of receiving the Request Header
+		# gives a lot of benefits
+		self.collect_head_buf()
+
+		# raw bytes of the header
+		header_data = self.head_buf.getvalue()
+		conlog(header_data.decode())
+
+		# split header into lines
+		header_data = header_data.decode().split('\r\n')
+		conlog('\n'.join(header_data))
+
+		# First line of the header is always the request method, path and http version
+		# It's up to the client to send valid data
+		self.method, self.path, self.protocol = header_data[0].split(' ')
+		conlog(self.method, self.path, self.protocol)
+		self.method = self.method.lower()
+
+		# deconstruct the url into components
+		parsed_url = urllib.parse.urlparse(self.path)
+
+		# important todo: lazy processing
+		# first - evaluate query params
+		self.query_params = {k:(''.join(v)) for (k,v) in urllib.parse.parse_qs(parsed_url.query, True).items()}
+
+		# then, evaluate path
+		decoded_url_path = urllib.parse.unquote(parsed_url.path)
+		self.abspath = self.srv_res.doc_root / Path(decoded_url_path.lstrip('/'))
+		self.relpath = Path(decoded_url_path.lstrip('/'))
+		self.trimpath = self.relpath
+
+		# Delete the first line as it's no longer needed
+		del header_data[0]
+
+		# parse the remaining headers into a dict
+		request_dict = {}
+		for line in header_data:
+			# skip empty stuff
+			if line.strip() == '':
+				continue
+			line_split = line.split(': ')
+			request_dict[line_split[0].lower()] = ': '.join(line_split[1:])
+
+		dict_pretty_print(request_dict)
+
+		self.headers = request_dict
+
+
+	# Actions
+	# =================
+
+	# Properly collapse the tunnel between server and client
+	def terminate(self):
+		socket = self.srv_res.pylib.socket
+		self.cl_con.shutdown(socket.SHUT_RDWR)
+		self.cl_con.close()
+
+		# Termination is only possible once
+		self.terminate = lambda: None
+
+	# Send a very simple html document
+	# with a short description of the provided Status Code
+	def reject(self, code=401, hint=''):
+		self.response.code = code
+		self.response.content_type = 'text/html'
+		self.response.flush_buffer(
+			self.srv_res.reject_precache
+			.replace(b'$$reason', self.srv_res.response_codes[code].encode())
+			.replace(b'$$hint', str(hint).encode())
+		)
+
+	# I cannot be bothered. Here, have *args and fuckoff
+	def match_path(self, action_dict, *args, trim_path=True):
+		"""
+		Sample set/list:
+		{
+			('/pootis/sandwich/dispenser', func_name1),
+			('/pootis',                    func_name2),
+		}
+		"""
+		comparator = '/' + self.relpath.as_posix()
+
+		for rpath, func in action_dict:
+			# print(rpath, 'startswith', )
+			if comparator.startswith(rpath):
+				if trim_path:
+					self.trimpath = self.srv_res.pylib.Path(comparator.lstrip(rpath))
+				return func(self, self.response, self.response.offered_services, *args)
+
+		# if no match was found - return false
+		return False
+
+
+	def read_body_stream(self):
+		"""
+		(Generator)
+		Progressively read body of the incoming request
+		"""
+		content_length = int(self.headers['content-length'])
+		read_progress = self.body_buf.seek(0, 2)
+		yield self.body_buf.getvalue()
+		while True:
+			if read_progress >= content_length:
+				break
+			# todo: finetune this value
+			# or expose it in the config
+			received_data = self.cl_con.recv(65535)
+			yield received_data
+			read_progress += len(received_data)
+
+
+	def read_body(self, as_buf=False):
+		import io
+		buf = io.BytesIO()
+		for chunk in self.read_body_stream():
+			buf.write(chunk)
+
+		if as_buf:
+			return buf
+		else:
+			return buf.getvalue()
+
+
+	# Utility
+	# =================
+	def parse_kv(self, kvs, separator=',', key_to_lower=True):
+		pairs = kvs.split(separator)
+		result = {}
+		for pair in pairs:
+			pair_split = pair.split('=')
+			if key_to_lower:
+				pair_split[0] = pair_split[0].upper()
+
+			if len(pair_split) == 1:
+				result[pair_split[0]] = True
+				continue
+
+			val = '='.join(pair_split[1:])
+			# important todo: is this really needed ?
+			try:
+				val = float(val)
+			# important todo: generic exceptions are very bad
+			except:
+				pass
+			try:
+				val = int(val)
+			except:
+				pass
+
+			result[pair_split[0]] = val
+
+		return result
+
+
+	# Processed headers
+	# =================
+
+	@property
+	def cookie(self):
+		"""
+		Nicely formatted cookie header
+		"""
+		if self._cookie:
+			return self._cookie
+
+		cookie_data = self.headers.get('cookie')
+		if not cookie_data:
+			return None
+
+		self._cookie = self.parse_kv(cookie_data, separator=';')
+
+		return self._cookie
+
+	# Even though server doesn't support advanced caching...
+	@property
+	def cache_control(self):
+		if self._cache_control:
+			return self._cache_control
+
+		cache_data = self.headers.get('cache-control')
+		if not cache_data:
+			return None
+
+		self._cache_control = self.parse_kv(cookie_data, separator=',')
+
+		return self._cache_control
+
+
+	# A client may ask for an access to a specific chunk of the target file.
+	# In this case a "Range" header is present.
+	# It has a format of start-end (both inclusive)
+	# This function returns an evaluated tuple from the following header.
+	# If "Range" header is not present - None is returned.
+	# Tuple format is as follows: (int|None, int|None)
+	# Negative numbers are clamped to 0
+	@property
+	def byterange(self):
+		if self._byterange:
+			return self._byterange
+
+		range_data = self.headers.get('range')
+		if not range_data:
+			return None
+
+		# todo: it's always assumed that range is in bytes
+		ranges = range_data.split('=')[1].split(',')
+
+		self._byterange = []
+		for chunk in ranges:
+			chunk_split = chunk.strip().split('-')
+			rstart = max(int(chunk_split[0]) - 1, 0) if chunk_split[0] else None
+			rend =   max(int(chunk_split[1]) - 1, 0) if chunk_split[1] else None
+			self._byterange.append(
+				(rstart, rend)
+			)
+
+		return self._byterange
+
+
+
+
+
+
+# The server creates "rooms" for every incoming connection.
+# The Base Room does some setup, like evaluating the request.
+# Further actions depend on the server setup:
+# If callback function is specified, then it's triggered
+# without any automatic actions
+# If callback function is NOT specified, then server provides
+# Some of its default services
+def base_room(cl_con, cl_addr, srv_res):
+	import sys, traceback
+	import importlib.util
+
+	try:
+		# precache some commonly-used python libraries
+		# important todo: is this even needed?
+		srv_res.reload_libs()
+
+		# Evaluate the request
+		with perftest('RQ EVAL', as_return=True) as tm:
+			evaluated_request = cl_request(cl_con, cl_addr, srv_res)
+		evaluated_request.response.headers['Timings'] = ''
+		evaluated_request.response.headers['Timings'] += tm.final + ' | '
+
+		conlog('Initialized basic room, evaluated request')
+
+		# Create service object
+		# offered_services = sv_services(evaluated_request, evaluated_request.response)
+
+		# Now either pass the control to the room specified in the config
+		# or the default room
+		if srv_res.cfg['room_file']:
+			with perftest('ROOM FILE IMPORT', as_return=True) as tm:
+				spec = importlib.util.spec_from_file_location('main', str(srv_res.cfg['room_file']))
+				custom_func = importlib.util.module_from_spec(spec)
+				spec.loader.exec_module(custom_func)
+			evaluated_request.response.headers['Timings'] += tm.final + ' | '
+
+			custom_func.main(
+				evaluated_request,
+				evaluated_request.response,
+				evaluated_request.response.offered_services
+			)
+		else:
+			_default_room(
+				evaluated_request,
+				evaluated_request.response,
+				evaluated_request.response.offered_services
+			)
+
+	except Exception as err:
+		conlog(
+			''.join(
+				traceback.format_exception(
+					type(err),
+					err,
+					err.__traceback__
+				)
+			)
+		)
+
+		_trback = ''.join(
+			traceback.format_exception(
+				type(err),
+				err,
+				err.__traceback__
+			)
+		)
+		cl_con.sendall('HTTP/1.1 500 Internal Server Error\r\n'.encode())
+		_rcontent = f"""<!DOCTYPE HTML>
+			<html>
+				<head>
+					<meta http-equiv="Content-Type" content="text/html;charset=utf-8">
+					<title>Rejected</title>
+				</head>
+				<body>
+					<h1 style="border-left: 2px #9F2E25;">500 Internal Server Error</h1>
+					<h3>Server: Jag</h3>
+					<p style="white-space: pre;">{_trback}</p>
+				</body>
+			</html>
+		"""
+		cl_con.sendall(f'Content-Length: {len(_rcontent)}\r\n\r\n'.encode())
+		cl_con.sendall(_rcontent.encode())
+
+		raise err
+
+
+	cl_con.close()
+	sys.exit()
+
+
+
```

### Comparing `jag-panzer-0.1.21/src/jag_panzer/cgi/burn_power.py` & `jag-panzer-0.1.23/src/jag_panzer/cgi/burn_power.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/cgi/jag.py` & `jag-panzer-0.1.23/src/jag_panzer/cgi/jag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf` & `jag-panzer-0.1.23/src/jag_panzer/cgi/templates/light_httpd/server_prms.conf`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/dir_list.py` & `jag-panzer-0.1.23/src/jag_panzer/dir_list.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/__init__.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/__init__.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_html5lib.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/builder/_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_htmlparser.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/builder/_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/builder/_lxml.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/builder/_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/css.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/dammit.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/diagnose.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/diagnose.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/element.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/formatter.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/__init__.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_builder.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_builder_registry.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_builder_registry.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_css.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_dammit.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_dammit.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_docs.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_element.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_formatter.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_fuzz.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_html5lib.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_html5lib.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_htmlparser.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_htmlparser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_lxml.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_lxml.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_navigablestring.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_navigablestring.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_pageelement.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_pageelement.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_soup.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_soup.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_tag.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/bs4/tests/test_tree.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/bs4/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/__init__.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/__meta__.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/__meta__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_match.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/css_match.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_parser.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/css_parser.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/css_types.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/css_types.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/pretty.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/pretty.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/soupsieve/util.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/soupsieve/util.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/yattag/__init__.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/yattag/__init__.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/yattag/doc.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/yattag/doc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/yattag/indentation.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/yattag/indentation.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/libs/yattag/simpledoc.py` & `jag-panzer-0.1.23/src/jag_panzer/libs/yattag/simpledoc.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/mimes/mime_types_base.py` & `jag-panzer-0.1.23/src/jag_panzer/mimes/mime_types_base.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/response_codes.py` & `jag-panzer-0.1.23/src/jag_panzer/response_codes.py`

 * *Files identical despite different names*

### Comparing `jag-panzer-0.1.21/src/jag_panzer/server.py` & `jag-panzer-0.1.23/src/jag_panzer/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # important todo: wat ?
 # (this library simply has to be a proper package)
 sys.path.append(str(Path(__file__).parent))
 
 from base_room import base_room
 import jag_util
 
+
 _main_init = '[root]'
 _server_proc = '[Server Process]'
 
 
 
-
 # Path
 # jag_util
 # socket
 # threading
 # time
 # sys
 # hashlib
@@ -80,24 +80,24 @@
 class server_info:
 	"""
 	Server info.
 	This class contains the config itself,
 	some preloaded python libraries,
 	and other stuff
 	"""
-	def __init__(self, config=None):
+	def __init__(self, init_config=None):
 		from mimes.mime_types_base import base_mimes
 		from mimes.mime_types_base import base_mimes_signed
 		from response_codes import codes as _rcodes
 
 		from pathlib import Path
 		import io
 		import jag_util
 
-		config = config or {}
+		config = init_config or {}
 
 		# root of the python package
 		self.sysroot = Path(__file__).parent
 
 		# extend python paths with included libs
 		sys.path.append(str(self.sysroot / 'libs'))
 
@@ -140,21 +140,18 @@
 		self.doc_root = Path(self.cfg['doc_root'])
 
 
 		#
 		# Directory Listing
 		# 
 		self.cfg['dir_listing'] = {
-			'enabled': True,
+			'enabled': False,
 			'dark_theme': False,
 		} | (config.get('dir_listing') or {})
 
-		if self.cfg['dir_listing']['enabled']:
-			from dir_list import dirlist
-			self.list_dir = dirlist(self)
 
 
 		# 
 		# Advanced CDN serving
 		# 
 		self.cfg['static_cdn'] = {
 			# Path to the static CDN
@@ -190,109 +187,109 @@
 			'max_file_len': (1024**2)*8,
 
 			# Max size of the header buffer
 			# Default to 512kb
 			'max_header_len': 1024*512,
 
 			# Default size of a single chunk when streaming buffers
-			# Default to 8mb
-			'bufstream_chunk_len': (1024**2)*8,
+			# Default to 5mb
+			'bufstream_chunk_len': (1024**2)*5,
 		} | (config.get('buffers') or {})
 
 
-	def precache_cdn(self):
-		for file in self.cdn_path.rglob(self.cfg['static_cdn']['pattern'] or '*'):
-			self.cdn_cache[file.relative_to(self.cdn_path).as_posix()] = \
-				io.BytesIO(file.read_bytes())
-
-		print(
-			_server_proc,
-			'precached CDN',
-			jag_util.dict_pretty_print(self.cdn_cache)
-		)
-
 	def reload_libs(self):
-		import time
-		ded = time.time()
 		# preload python libraries
 		self.pylib = pylib_preload()
-		print('Preloaded libs in', (time.time() - ded)*1000)
+
+
+
 
 
 
 def sock_server(sv_cfg):
 	# Preload resources n stuff
-	print(_server_proc, 'Preloading resources...')
+	print(_server_proc, 'Preloading resources... (4/7)')
 	server_resources = server_info(sv_cfg)
-	print(_server_proc, 'Binding server to a port...')
+	print(_server_proc, 'Binding server to a port... (5/7)')
 	# Port to run the server on
 	# port = 56817
 	port = server_resources.cfg['port']
 	# Create the Server object
 	s = socket.socket()
 
 	# Bind server to the specified port. 0 = Find the closest free port and run stuff on it
+	# todo: is this really the only way to bind stuff to the current IP ?
 	_get_ip_s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 	_get_ip_s.connect(('8.8.8.8', 0))
 	current_ip = _get_ip_s.getsockname()[0]
 	s.bind(
 		(current_ip, port)
 	)
 
 	# Basically launch the server
 	# The number passed to this function identifies the max amount of simultaneous connections
 	# If the amount of connections exceeds this limit -
 	# connections become rejected till other ones are resolved (aka closed)
 	# 0 = infinite
 	s.listen(server_resources.cfg['max_connections'])
 
-	print(_server_proc, 'Server listening on port', s.getsockname()[1])
+	print(_server_proc, 'Server listening on port (6/7)', s.getsockname()[1])
 
 	# important todo: does this actually slow the shit down?
 	# important todo: is it just me or this crashes the system ???!!?!??!?!?!?!?
 	# important todo: this creates a bunch of threads as a side effect
 	# important todo: Pickling is EXTREMELY slow and bad
 
 	# Multiprocess pool automatically takes care of a bunch of stuff
 	# But most importantly, it takes care of shadow processess left after collapsed rooms
 	# (linux moment)
-	with multiprocessing.Pool() as pool:
-		while True:
-			print(_server_proc, 'Entering the main listen cycle which would spawn rooms upon incoming connection requests...')
-			# Try establishing connection, nothing below this line gets executed
-			# until server receives a new connection
-			conn, address = s.accept()
-			print(_server_proc, 'Got connection, spawning a room. Client info:', address)
-			# Create a basic room
-			pool.apply_async(base_room, (conn, address, server_resources))
 
-			print(_server_proc, 'Spawned a room, continue accepting new connections')
+	# EXCEPT, process pool is garbage: It's a pool with a fixed amount of workers,
+	# where tasks are distributed between them. Shit
+
+	# with multiprocessing.Pool() as pool:
+	print(_server_proc, 'Accepting connections... (7/7)')
+	while True:
+		# conlog('Entering the main listen cycle which would spawn rooms upon incoming connection requests...', echo=_server_proc)
+		# Try establishing connection, nothing below this line gets executed
+		# until server receives a new connection
+		conn, address = s.accept()
+		# conlog('Got connection, spawning a room. Client info:', address, echo=_server_proc)
+		# Create a basic room
+		# pool.apply_async(base_room, (conn, address, server_resources))
+
+		# conlog('Spawned a room, continue accepting new connections', echo=_server_proc)
+		# poot = multiprocessing.Process(target=base_room, args=(conn, address, server_resources,), daemon=True).start()
+		multiprocessing.Process(target=base_room, args=(conn, address, server_resources,), daemon=True).start()
+
+
 
 
 def server_process(srv_params, stfu=False):
-	print(_main_init, 'Creating and starting the server process...')
+	print(_main_init, 'Creating and starting the server process... (1/7)')
 	# Create a new process containing the main incoming connections listener
 	server_ctrl = multiprocessing.Process(target=sock_server, args=(srv_params,))
-	print(_main_init, 'Created the process instructions, attempting launch...')
+	print(_main_init, 'Created the process instructions, attempting launch... (2/7)')
 	# Initialize the created process
 	# (It's not requred to create a new variable, it could be done in 1 line with .start() in the end)
 	server_ctrl.start()
 
-	print(_main_init, 'Launched the server process...')
+	print(_main_init, 'Launched the server process... (3/7)')
 
 
 
 
 if __name__ == '__main__':
 	server_params = {
 		'doc_root': r'E:\!webdesign\jag',
 		'port': 56817,
 		'dir_listing': {
 			'enabled': True,
-		}
+		},
+		# 'routes': _routes,
 	}
 	server_process(server_params)
```

### Comparing `jag-panzer-0.1.21/src/jag_panzer.egg-info/PKG-INFO` & `jag-panzer-0.1.23/src/jag_panzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jag-panzer
-Version: 0.1.21
+Version: 0.1.23
 Summary: Simple HTTP server allowing pure python workflow
 Home-page: https://github.com/MrKleiner/jag
 Author: Mr.Kleiner
 Author-email: megaadrenaline1055@gmail.com
 Project-URL: Bug Tracker, https://github.com/MrKleiner/jag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jag-panzer-0.1.21/src/jag_panzer.egg-info/SOURCES.txt` & `jag-panzer-0.1.23/src/jag_panzer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/jag_panzer/__init__.py
 src/jag_panzer/base_room.py
 src/jag_panzer/dir_list.py
+src/jag_panzer/eztag.py
 src/jag_panzer/jag_util.py
 src/jag_panzer/response_codes.py
 src/jag_panzer/server.py
 src/jag_panzer/test.cmd
 src/jag_panzer.egg-info/PKG-INFO
 src/jag_panzer.egg-info/SOURCES.txt
 src/jag_panzer.egg-info/dependency_links.txt
```

