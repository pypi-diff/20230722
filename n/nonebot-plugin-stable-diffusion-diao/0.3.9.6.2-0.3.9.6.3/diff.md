# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.6.2.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.6.2.tar", last modified: Sat Jul 22 04:02:09 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.6.3.tar", last modified: Sat Jul 22 04:24:13 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    27841 2023-07-22 03:28:50.083794 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6226 2023-07-22 03:14:33.094866 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    16093 2023-07-16 04:28:25.749676 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     6015 2023-07-17 06:15:44.003068 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    18835 2023-07-22 03:38:44.232347 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0    10771 2023-07-20 07:00:30.079891 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2754 2023-07-16 04:01:07.429355 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11332 2023-07-20 14:22:22.328291 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    41827 2023-07-22 04:01:57.684358 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6163 2023-07-14 13:25:19.581758 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      726 2023-07-20 08:05:34.470705 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      730 2023-07-22 04:02:09.072102 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    27841 2023-07-22 03:28:50.083794 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6226 2023-07-22 03:14:33.094866 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    16093 2023-07-16 04:28:25.749676 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     6015 2023-07-17 06:15:44.003068 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    18835 2023-07-22 03:38:44.232347 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0    10771 2023-07-20 07:00:30.079891 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2754 2023-07-16 04:01:07.429355 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11332 2023-07-20 14:22:22.328291 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    41827 2023-07-22 04:01:57.684358 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     6606 2023-07-22 04:23:53.420725 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6163 2023-07-14 13:25:19.581758 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      726 2023-07-20 08:05:34.470705 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      730 2023-07-22 04:24:13.253700 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/pyproject.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,110 +22,122 @@
             return result
 
 
 async def translate_bing(text: str, to: str):
     """
     en,jp,zh_Hans
     """
-    if to == "zh":
-        to = "zh-Hans"
-    key = config.bing_key
-    if not key:
-        return None
-    header = {
-        "Ocp-Apim-Subscription-Key": key,
-        "Content-Type": "application/json",
-    }
-    async with aiohttp.ClientSession() as session:
-        body = [{'text': text}]
-        params = {
-            "api-version": "3.0",
-            "to": to,
-            "profanityAction": "Deleted",
+    try:
+        if to == "zh":
+            to = "zh-Hans"
+        key = config.bing_key
+        if not key:
+            return None
+        header = {
+            "Ocp-Apim-Subscription-Key": key,
+            "Content-Type": "application/json",
         }
-        async with session.post('https://api.cognitive.microsofttranslator.com/translate', json=body, params=params, headers=header) as resp:
-            if resp.status != 200:
-                logger.error(f"Bing翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
-                return None
-            jsonresult = await resp.json()
-            result=jsonresult[0]["translations"][0]["text"]
-            logger.debug(f"Bing翻译启动，获取到{text},翻译后{result}")
-            return result
+        async with aiohttp.ClientSession() as session:
+            body = [{'text': text}]
+            params = {
+                "api-version": "3.0",
+                "to": to,
+                "profanityAction": "Deleted",
+            }
+            async with session.post('https://api.cognitive.microsofttranslator.com/translate', json=body, params=params, headers=header) as resp:
+                if resp.status != 200:
+                    logger.error(f"Bing翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
+                    return None
+                jsonresult = await resp.json()
+                result=jsonresult[0]["translations"][0]["text"]
+                logger.debug(f"Bing翻译启动，获取到{text},翻译后{result}")
+                return result
+    except Exception:
+        return None
 
 
 async def translate_deepl(text: str, to: str):
     """
     EN,JA,ZH
     """
-    to = to.upper()
-    key = config.deepl_key
-    if not key:
+    try:
+        to = to.upper()
+        key = config.deepl_key
+        if not key:
+            return None
+        async with aiohttp.ClientSession() as session:
+            params = {
+                "auth_key":key,
+                "text": text,
+                "target_lang": to,
+            }
+            async with session.get('https://api-free.deepl.com/v2/translate', params=params) as resp:
+                if resp.status != 200:
+                    logger.error(f"DeepL翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
+                    return None
+                jsonresult = await resp.json()
+                result=jsonresult["translations"][0]["text"]
+                logger.debug(f"DeepL翻译启动，获取到{text},翻译后{result}")
+                return result
+    except Exception:
         return None
-    async with aiohttp.ClientSession() as session:
-        params = {
-            "auth_key":key,
-            "text": text,
-            "target_lang": to,
-        }
-        async with session.get('https://api-free.deepl.com/v2/translate', params=params) as resp:
-            if resp.status != 200:
-                logger.error(f"DeepL翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
-                return None
-            jsonresult = await resp.json()
-            result=jsonresult["translations"][0]["text"]
-            logger.debug(f"DeepL翻译启动，获取到{text},翻译后{result}")
-            return result
 
 
 async def translate_youdao(input: str, type: str):
     """
     默认auto
     ZH_CH2EN 中译英
     EN2ZH_CN 英译汉
     """
-    if type == "zh":
-        type = "EN2ZH_CN"
-    elif type == "en":
-        type = "ZH_CH2EN"
-    async with aiohttp.ClientSession() as session:
-        data = {
-            'doctype': 'json',
-            'type': type,
-            'i': input
-        }
-        async with session.post("http://fanyi.youdao.com/translate", data=data) as resp:
-            if resp.status != 200:
-                logger.error(f"有道翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
-                return None
-            result = await resp.json()
-            result=result["translateResult"][0][0]["tgt"]
-            logger.debug(f"有道翻译启动，获取到{input},翻译后{result}")
-            return result
+    try:
+        if type == "zh":
+            type = "EN2ZH_CN"
+        elif type == "en":
+            type = "ZH_CH2EN"
+        async with aiohttp.ClientSession() as session:
+            data = {
+                'doctype': 'json',
+                'type': type,
+                'i': input
+            }
+            async with session.post("http://fanyi.youdao.com/translate", data=data) as resp:
+                if resp.status != 200:
+                    logger.error(f"有道翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
+                    return None
+                result = await resp.json()
+                result=result["translateResult"][0][0]["tgt"]
+                logger.debug(f"有道翻译启动，获取到{input},翻译后{result}")
+                return result
+    except Exception:
+        return None
 
 
 async def translate_google_proxy(input: str, to: str):
     """
     en,jp,zh 需要来源语言
     """
-    if to == "zh":
-        from_ = "en"
-    else:
-        from_="zh"
-    async with aiohttp.ClientSession()as session:
-        data = {"data": [input, from_, to]}
-        async with session.post("https://mikeee-gradio-gtr.hf.space/api/predict", json=data)as resp:
-            if resp.status != 200:
-                logger.error(f"谷歌代理翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
-                return None
-            result = await resp.json()
-            result=result["data"][0]
-            if "429" in result:
-                return None
-            logger.debug(f"谷歌代理翻译启动，获取到{input},翻译后{result}")
-            return result
+    try:
+        if to == "zh":
+            from_ = "en"
+        else:
+            from_="zh"
+        async with aiohttp.ClientSession()as session:
+            data = {"data": [input, from_, to]}
+            async with session.post("https://mikeee-gradio-gtr.hf.space/api/predict", json=data)as resp:
+                if resp.status != 200:
+                    logger.error(f"谷歌代理翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
+                    return None
+                result = await resp.json()
+                result=result["data"][0]
+                if "429" in result:
+                    return None
+                logger.debug(f"谷歌代理翻译启动，获取到{input},翻译后{result}")
+                return result
+    except Exception:
+        return None
 
 
 async def get_access_token():
     """
     百度云access_token
     使用 AK，SK 生成鉴权签名（Access Token）
     :return: access_token，或是None(如果错误)
@@ -137,24 +149,27 @@
     async with aiohttp.ClientSession() as session:
         async with session.post(url=url, params=params) as resp:
             json = await resp.json()
     return json["access_token"]
 
 
 async def translate_baidu(input: str, to: str):
-    key = config.baidu_translate_key
-    if not key:
-        return None
-    token = await get_access_token()
-    url = 'https://aip.baidubce.com/rpc/2.0/mt/texttrans/v1?access_token=' + token
-    # For list of language codes, please refer to `https://ai.baidu.com/ai-doc/MT/4kqryjku9#语种列表`
-    term_ids = '' # 术语库id，多个逗号隔开
-    headers = {'Content-Type': 'application/json'}
-    payload = {'q': input, 'from': 'zh', 'to': to, 'termIds' : term_ids}
-    async with aiohttp.ClientSession(headers=headers) as session:
-        async with session.post(url=url, json=payload) as resp:
-            if resp.status != 200:
-                logger.error(f"百度翻译接口错误, 错误代码{resp.status},{await resp.text()}")
-                return None
-            json_ = await resp.json()
-            result = json_["result"]["trans_result"][0]["dst"]
-    return result
+    try:
+        key = config.baidu_translate_key
+        if not key:
+            return None
+        token = await get_access_token()
+        url = 'https://aip.baidubce.com/rpc/2.0/mt/texttrans/v1?access_token=' + token
+        # For list of language codes, please refer to `https://ai.baidu.com/ai-doc/MT/4kqryjku9#语种列表`
+        term_ids = '' # 术语库id，多个逗号隔开
+        headers = {'Content-Type': 'application/json'}
+        payload = {'q': input, 'from': 'zh', 'to': to, 'termIds' : term_ids}
+        async with aiohttp.ClientSession(headers=headers) as session:
+            async with session.post(url=url, json=payload) as resp:
+                if resp.status != 200:
+                    logger.error(f"百度翻译接口错误, 错误代码{resp.status},{await resp.text()}")
+                    return None
+                json_ = await resp.json()
+                result = json_["result"]["trans_result"][0]["dst"]
+        return result
+    except Exception:
+        return None
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.6.2/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.9.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.9.6.2"
+version = "0.3.9.6.3"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

