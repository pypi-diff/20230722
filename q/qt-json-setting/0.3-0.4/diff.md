# Comparing `tmp/qt-json-setting-0.3.tar.gz` & `tmp/qt-json-setting-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt-json-setting-0.3.tar", last modified: Fri Jul  7 01:38:55 2023, max compression
+gzip compressed data, was "qt-json-setting-0.4.tar", last modified: Sat Jul 22 05:21:19 2023, max compression
```

## Comparing `qt-json-setting-0.3.tar` & `qt-json-setting-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:38:55.278487 qt-json-setting-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-07 01:38:45.000000 qt-json-setting-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 01:38:55.278487 qt-json-setting-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 01:38:45.000000 qt-json-setting-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:38:55.278487 qt-json-setting-0.3/qt_json_setting/
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-07 01:38:45.000000 qt-json-setting-0.3/qt_json_setting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:38:55.278487 qt-json-setting-0.3/qt_json_setting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:38:55.278487 qt-json-setting-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-07 01:38:45.000000 qt-json-setting-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:21:19.729255 qt-json-setting-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-22 05:21:11.000000 qt-json-setting-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-22 05:21:19.729255 qt-json-setting-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-22 05:21:11.000000 qt-json-setting-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:21:19.729255 qt-json-setting-0.4/qt_json_setting/
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-22 05:21:11.000000 qt-json-setting-0.4/qt_json_setting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:21:19.729255 qt-json-setting-0.4/qt_json_setting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-22 05:21:19.000000 qt-json-setting-0.4/qt_json_setting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 05:21:19.729255 qt-json-setting-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-22 05:21:11.000000 qt-json-setting-0.4/setup.py
```

### Comparing `qt-json-setting-0.3/LICENSE` & `qt-json-setting-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qt-json-setting-0.3/PKG-INFO` & `qt-json-setting-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-json-setting
-Version: 0.3
+Version: 0.4
 Summary: 根据json schema生成设置界面
 Home-page: https://github.com/ovo-Tim/pyqt-json-settingt
 Author: ovo-tim
 Author-email: ovo-tim@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `qt-json-setting-0.3/qt_json_setting/__init__.py` & `qt-json-setting-0.4/qt_json_setting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
         self.btns = QHBoxLayout(self)
         self.main_layout.addLayout(self.btns)
         self.btns.addStretch(1)
         self.appely_btn = QPushButton(text = self.tr('appely'))
         self.appely_btn.clicked.connect(self.save)
         self.close_btn = QPushButton(text = self.tr('close'))
-        self.close_btn.clicked.connect(sys.exit)
+        self.close_btn.clicked.connect(self.close)
         self.ok_btn = QPushButton(text = self.tr('ok'))
         self.ok_btn.clicked.connect(lambda: self.save(close=True))
         self.btns.addWidget(self.appely_btn)
         self.btns.addWidget(self.close_btn)
         self.btns.addWidget(self.ok_btn)
 
         for page, setting in self.setting.items():
@@ -148,15 +148,15 @@
                 _schema = self.json_schema['properties'][page]['properties'][name]
                 page_layout.addWidget(setting_widget(self.setting, page, name,_schema))
 
     def save(self, close=False):
         with open(self.json_path, 'w') as f:
             f.write(json.encode(self.setting))
         if close:
-            sys.exit()
+            self.close()
         
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
     win = seting_window('./example/example.json', './example/example-schema.json')
     win.show()
-    app.exec_()
+    app.exec_()
```

### Comparing `qt-json-setting-0.3/qt_json_setting.egg-info/PKG-INFO` & `qt-json-setting-0.4/qt_json_setting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-json-setting
-Version: 0.3
+Version: 0.4
 Summary: 根据json schema生成设置界面
 Home-page: https://github.com/ovo-Tim/pyqt-json-settingt
 Author: ovo-tim
 Author-email: ovo-tim@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `qt-json-setting-0.3/setup.py` & `qt-json-setting-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qt-json-setting",
-    version="0.3",
+    version="0.4",
     author="ovo-tim",
     author_email="ovo-tim@qq.com",
     description="根据json schema生成设置界面",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ovo-Tim/pyqt-json-settingt",
     packages=setuptools.find_packages(),
@@ -19,8 +19,8 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'Pyside6',
         'jsonschema',
         'ujson'
     ]
-)
+)
```

