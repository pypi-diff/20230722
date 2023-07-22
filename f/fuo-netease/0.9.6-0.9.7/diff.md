# Comparing `tmp/fuo_netease-0.9.6.tar.gz` & `tmp/fuo_netease-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo_netease-0.9.6.tar", last modified: Thu Jun  8 05:22:53 2023, max compression
+gzip compressed data, was "fuo_netease-0.9.7.tar", last modified: Sat Jul 22 08:46:36 2023, max compression
```

## Comparing `fuo_netease-0.9.6.tar` & `fuo_netease-0.9.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/fuo_netease/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/fuo_netease/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/assets/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/fuo_netease/cloud_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/cloud_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/cloud_helpers/cloud_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/cloud_helpers/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/excs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/login_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/nem.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/page_daily_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/page_explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/page_fav.py
--rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/fuo_netease/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/fuo_netease.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 05:22:53.000000 fuo_netease-0.9.6/fuo_netease.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 05:22:53.462399 fuo_netease-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-08 05:22:51.000000 fuo_netease-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:46:36.008524 fuo_netease-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-22 08:46:36.008524 fuo_netease-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:46:36.008524 fuo_netease-0.9.7/fuo_netease/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:46:36.008524 fuo_netease-0.9.7/fuo_netease/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/assets/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:46:36.008524 fuo_netease-0.9.7/fuo_netease/cloud_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/cloud_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/cloud_helpers/cloud_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/cloud_helpers/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/excs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/login_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/nem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/page_daily_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/page_explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/page_fav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:46:36.008524 fuo_netease-0.9.7/fuo_netease.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/fuo_netease.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-22 08:46:36.008524 fuo_netease-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-22 08:46:35.000000 fuo_netease-0.9.7/setup.py
```

### Comparing `fuo_netease-0.9.6/PKG-INFO` & `fuo_netease-0.9.7/fuo_netease.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fuo_netease
-Version: 0.9.6
+Name: fuo-netease
+Version: 0.9.7
 Summary: feeluown netease plugin
 Home-page: https://github.com/feeluown/feeluown-netease
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: feeluown,plugin,netease
```

### Comparing `fuo_netease-0.9.6/README.md` & `fuo_netease-0.9.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 ```sh
 pip3 install fuo-netease
 ```
 
 ## changelog
 
+### 0.9.7 (2023-07-22)
+- 修复登录失败的问题：'NoneType' object has no attribute 'cache_get'
+
 ### 0.9.6 (2023-06-08)
 - 移除对 feeluown.models 的依赖
 
 ### 0.9.5 (2023-04-27)
 - 提供双语歌词
 
 ### 0.9.4 (2023-03-27)
```

### Comparing `fuo_netease-0.9.6/fuo_netease/__init__.py` & `fuo_netease-0.9.7/fuo_netease/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/api.py` & `fuo_netease-0.9.7/fuo_netease/api.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/assets/icon.svg` & `fuo_netease-0.9.7/fuo_netease/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/cloud_helpers/__init__.py` & `fuo_netease-0.9.7/fuo_netease/cloud_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/cloud_helpers/cloud_api.py` & `fuo_netease-0.9.7/fuo_netease/cloud_helpers/cloud_api.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/cloud_helpers/security.py` & `fuo_netease-0.9.7/fuo_netease/cloud_helpers/security.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/downloader.py` & `fuo_netease-0.9.7/fuo_netease/downloader.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/login_controller.py` & `fuo_netease-0.9.7/fuo_netease/login_controller.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/models.py` & `fuo_netease-0.9.7/fuo_netease/models.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/nem.py` & `fuo_netease-0.9.7/fuo_netease/nem.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,30 @@
         self._app.browser.route('/providers/netease/daily_recommendation')(dr_render)
 
     def ready_to_login(self):
         if self._user is not None:
             logger.debug('You have already logined in.')
             asyncio.ensure_future(self.login_as(self._user))
             return
+
         logger.debug('Trying to load last login user...')
         user = LoginController.load()
-        cookies, exists = user.cache_get('cookies')
-        assert exists
-        if user is None or 'MUSIC_U' not in cookies:
-            logger.debug('Trying to load last login user...failed')
-            self.login_dialog.show()
-            self.login_dialog.load_user_pw()
-            self.login_dialog.login_success.connect(
-                lambda user: asyncio.ensure_future(self.login_as(user)))
-        else:
-            logger.debug('Trying to load last login user...done')
-            asyncio.ensure_future(self.login_as(user))
+        if user is not None:
+            cookies, exists = user.cache_get('cookies')
+            assert exists
+            if 'MUSIC_U' in cookies:
+                logger.debug('Trying to load last login user...done')
+                asyncio.ensure_future(self.login_as(user))
+                return
+
+        logger.debug('Trying to load last login user...failed')
+        self.login_dialog.show()
+        self.login_dialog.load_user_pw()
+        self.login_dialog.login_success.connect(
+            lambda user: asyncio.ensure_future(self.login_as(user)))
 
     async def login_as(self, user):
         provider.auth(user)
         self._user = user
         LoginController.save(user)
         left_panel = self._app.ui.left_panel
         left_panel.playlists_con.show()
```

### Comparing `fuo_netease-0.9.6/fuo_netease/page_daily_recommendation.py` & `fuo_netease-0.9.7/fuo_netease/page_daily_recommendation.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/page_explore.py` & `fuo_netease-0.9.7/fuo_netease/page_explore.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/page_fav.py` & `fuo_netease-0.9.7/fuo_netease/page_fav.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/provider.py` & `fuo_netease-0.9.7/fuo_netease/provider.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/schemas.py` & `fuo_netease-0.9.7/fuo_netease/schemas.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease/ui.py` & `fuo_netease-0.9.7/fuo_netease/ui.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/fuo_netease.egg-info/PKG-INFO` & `fuo_netease-0.9.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fuo-netease
-Version: 0.9.6
+Name: fuo_netease
+Version: 0.9.7
 Summary: feeluown netease plugin
 Home-page: https://github.com/feeluown/feeluown-netease
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: feeluown,plugin,netease
```

### Comparing `fuo_netease-0.9.6/fuo_netease.egg-info/SOURCES.txt` & `fuo_netease-0.9.7/fuo_netease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuo_netease-0.9.6/setup.py` & `fuo_netease-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='fuo_netease',
-    version='0.9.6',
+    version='0.9.7',
     description='feeluown netease plugin',
     author='Cosven',
     author_email='yinshaowen241@gmail.com',
     packages=find_packages(exclude=('tests*',)),
     package_data={
         '': ['assets/*.svg',
              ]
```

