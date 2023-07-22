# Comparing `tmp/wow_ai_ml-0.2.4.tar.gz` & `tmp/wow_ai_ml-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_ml-0.2.4.tar", max compression
+gzip compressed data, was "wow_ai_ml-0.2.5.tar", max compression
```

## Comparing `wow_ai_ml-0.2.4.tar` & `wow_ai_ml-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.4/README.md
--rw-r--r--   0        0        0      261 2023-07-21 07:53:51.702038 wow_ai_ml-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.4/wow_ai_ml/__init__.py
--rw-r--r--   0        0        0     8957 2023-07-21 07:52:00.443983 wow_ai_ml-0.2.4/wow_ai_ml/api.py
--rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.4/wow_ai_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.4/wow_ai_ml/default_configs/README.md
--rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.4/wow_ai_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.4/wow_ai_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.4/wow_ai_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.4/wow_ai_ml/exceptions.py
--rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.4/wow_ai_ml/helpers.py
--rw-r--r--   0        0        0    33543 2023-07-21 07:45:55.771112 wow_ai_ml-0.2.4/wow_ai_ml/model.py
--rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.4/wow_ai_ml/server.py
--rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.4/wow_ai_ml/templates/preview.html
--rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.4/wow_ai_ml/utils.py
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.5/README.md
+-rw-r--r--   0        0        0      261 2023-07-22 09:46:51.230680 wow_ai_ml-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.5/wow_ai_ml/__init__.py
+-rw-r--r--   0        0        0     8957 2023-07-22 09:40:33.052501 wow_ai_ml-0.2.5/wow_ai_ml/api.py
+-rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.5/wow_ai_ml/exceptions.py
+-rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.5/wow_ai_ml/helpers.py
+-rw-r--r--   0        0        0    34614 2023-07-22 09:46:19.605016 wow_ai_ml-0.2.5/wow_ai_ml/model.py
+-rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.5/wow_ai_ml/server.py
+-rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.5/wow_ai_ml/templates/preview.html
+-rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.5/wow_ai_ml/utils.py
+-rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.5/PKG-INFO
```

### Comparing `wow_ai_ml-0.2.4/README.md` & `wow_ai_ml-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.4/wow_ai_ml/api.py` & `wow_ai_ml-0.2.5/wow_ai_ml/api.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.4/wow_ai_ml/default_configs/README.md` & `wow_ai_ml-0.2.5/wow_ai_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.4/wow_ai_ml/default_configs/_wsgi.py.tmpl` & `wow_ai_ml-0.2.5/wow_ai_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.4/wow_ai_ml/default_configs/docker-compose.yml` & `wow_ai_ml-0.2.5/wow_ai_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.4/wow_ai_ml/exceptions.py` & `wow_ai_ml-0.2.5/wow_ai_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.4/wow_ai_ml/helpers.py` & `wow_ai_ml-0.2.5/wow_ai_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.4/wow_ai_ml/model.py` & `wow_ai_ml-0.2.5/wow_ai_ml/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,16 +306,19 @@
 
     @abstractmethod
     def predict(self, tasks, **kwargs):
         pass
     @abstractmethod
     def toolbar_predict(self, image, clickpoint, polygons, vertices,project, **kwargs):
         pass
+    # @abstractmethod
+    # def toolbar_predict_sam(self, image, clickpoint, polygons, vertices,project,voice,prompt,image_pref,draw_polygons, **kwargs):
+    #     pass
     @abstractmethod
-    def toolbar_predict_sam(self, image, clickpoint, polygons, vertices,project,voice,prompt,image_pref,draw_polygons, **kwargs):
+    def action(self, project,command, collection, **kwargs):
         pass
     @abstractmethod
     def model(self,project, **kwargs):
         pass
     @abstractmethod
     def preview(self,project, **kwargs):
         pass
@@ -617,31 +620,49 @@
             return predictions, m
 
         if not cls._current_model:
             raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
         predictions = m.model.toolbar_predict( image, clickpoint, polygons, vertices,project, **kwargs)
         return predictions, m
     @classmethod
-    def toolbar_predict_sam(
-        cls, image, clickpoint, polygons, vertices, project=None, voice=None,prompt=None,image_pref=None,draw_polygons=None,label_config=None, force_reload=True, try_fetch=False, **kwargs
+    def action(
+        cls,  project=None, command=None, collection=None, label_config=None, force_reload=True, try_fetch=False, **kwargs
     ):
         if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
             if try_fetch:
                 m = cls.fetch(project, label_config, force_reload)
             else:
                 m = cls.get(project)
                 if not m:
                     raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
-            predictions = m.model.toolbar_predict_sam(image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+            predictions = m.model.action(project, command,collection,**kwargs)
             return predictions, m
 
         if not cls._current_model:
             raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
-        predictions = m.model.toolbar_predict_sam( image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+        predictions = m.model.action( project,  command,collection,**kwargs)
         return predictions, m
+    # @classmethod
+    # def toolbar_predict_sam(
+    #     cls, image, clickpoint, polygons, vertices, project=None, voice=None,prompt=None,image_pref=None,draw_polygons=None,label_config=None, force_reload=True, try_fetch=False, **kwargs
+    # ):
+    #     if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
+    #         if try_fetch:
+    #             m = cls.fetch(project, label_config, force_reload)
+    #         else:
+    #             m = cls.get(project)
+    #             if not m:
+    #                 raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
+    #         predictions = m.model.toolbar_predict_sam(image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+    #         return predictions, m
+
+    #     if not cls._current_model:
+    #         raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
+    #     predictions = m.model.toolbar_predict_sam( image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+    #     return predictions, m
     @classmethod
     def model(cls,project=None,label_config=None, force_reload=True, try_fetch=False, **kwargs):
         if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
             if try_fetch:
                 m = cls.fetch(project, label_config, force_reload)
             else:
                 m = cls.get(project)
```

### Comparing `wow_ai_ml-0.2.4/wow_ai_ml/server.py` & `wow_ai_ml-0.2.5/wow_ai_ml/server.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.4/wow_ai_ml/utils.py` & `wow_ai_ml-0.2.5/wow_ai_ml/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.4/PKG-INFO` & `wow_ai_ml-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-ml
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.inc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

