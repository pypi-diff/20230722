# Comparing `tmp/m-run-script-test-1.0.1.tar.gz` & `tmp/m-run-script-test-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-run-script-test-1.0.1.tar", last modified: Mon Jun 12 01:17:57 2023, max compression
+gzip compressed data, was "m-run-script-test-1.0.2.tar", last modified: Sat Jul 22 07:09:50 2023, max compression
```

## Comparing `m-run-script-test-1.0.1.tar` & `m-run-script-test-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:17:57.205752 m-run-script-test-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     2170 2023-06-12 01:17:57.205752 m-run-script-test-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      966 2023-06-12 01:16:16.000000 m-run-script-test-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:17:57.203752 m-run-script-test-1.0.1/m_run_script_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2170 2023-06-12 01:17:57.000000 m-run-script-test-1.0.1/m_run_script_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      271 2023-06-12 01:17:57.000000 m-run-script-test-1.0.1/m_run_script_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 01:17:57.000000 m-run-script-test-1.0.1/m_run_script_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-12 01:17:57.000000 m-run-script-test-1.0.1/m_run_script_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-12 01:17:57.000000 m-run-script-test-1.0.1/m_run_script_test.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:17:57.199752 m-run-script-test-1.0.1/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:17:57.199752 m-run-script-test-1.0.1/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:17:57.204752 m-run-script-test-1.0.1/mobio/libs/run_script/
--rw-r--r--   0 root         (0) root         (0)    17958 2023-06-12 01:16:16.000000 m-run-script-test-1.0.1/mobio/libs/run_script/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-12 01:16:16.000000 m-run-script-test-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 01:17:57.206752 m-run-script-test-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9582 2023-06-12 01:17:56.000000 m-run-script-test-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 07:09:50.731759 m-run-script-test-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-07-22 07:09:50.731759 m-run-script-test-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-07-22 07:06:50.000000 m-run-script-test-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 07:09:50.729759 m-run-script-test-1.0.2/m_run_script_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-07-22 07:09:50.000000 m-run-script-test-1.0.2/m_run_script_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      271 2023-07-22 07:09:50.000000 m-run-script-test-1.0.2/m_run_script_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 07:09:50.000000 m-run-script-test-1.0.2/m_run_script_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-22 07:09:50.000000 m-run-script-test-1.0.2/m_run_script_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-22 07:09:50.000000 m-run-script-test-1.0.2/m_run_script_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 07:09:50.722759 m-run-script-test-1.0.2/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 07:09:50.722759 m-run-script-test-1.0.2/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 07:09:50.729759 m-run-script-test-1.0.2/mobio/libs/run_script/
+-rw-r--r--   0 root         (0) root         (0)    17857 2023-07-22 07:06:50.000000 m-run-script-test-1.0.2/mobio/libs/run_script/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-22 07:06:50.000000 m-run-script-test-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 07:09:50.732759 m-run-script-test-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9582 2023-07-22 07:09:50.000000 m-run-script-test-1.0.2/setup.py
```

### Comparing `m-run-script-test-1.0.1/PKG-INFO` & `m-run-script-test-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 Metadata-Version: 2.1
 Name: m-run-script-test
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ### Run Script
-        Thư viện xử lý chạy các script của project mỗi khi deploy version mới, sau khi chạy xong thì lưu lại vết script đã chạy để lần sau không chạy lại nữa. 
-        
-        
-        ### Cài đặt:
-        ```bash
-         $ pip3 install m-run-script
-         ```
-        
-        ### Sử dụng:
-        
-        ##### Chạy các script của project:
-           ```python
-            from mobio.libs.run_script import MobioRunScript
-            VERSION_CONFIG = {
-                "every_deploy": {
-                    "script": [
-                        "PYTHONPATH=./ python3.8 -u sync_mongodb_index.py",
-                        "PYTHONPATH=./ python3.8 -u sync_kafka_topic.py"
-                    ]
-                },
-                "version": {
-                    1: ["PYTHONPATH=./ python3.8 -u scripts/script_1.py",
-                        "PYTHONPATH=./ python3.8 -u scripts/script_2.py"],
-                    2: ["PYTHONPATH=./ python3.8 -u scripts/script_3.py"]
-                }
-            }
-        
-            MobioRunScript().run_script_by_version(VERSION_CONFIG)
-        
-           ```
-        #### Log - 1.0.0
-            - release sdk
-            
 Keywords: mobio,mobio-script,version-script
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+### Run Script
+Thư viện xử lý chạy các script của project mỗi khi deploy version mới, sau khi chạy xong thì lưu lại vết script đã chạy để lần sau không chạy lại nữa. 
+
+
+### Cài đặt:
+```bash
+ $ pip3 install m-run-script
+ ```
+
+### Sử dụng:
+
+##### Chạy các script của project:
+   ```python
+    from mobio.libs.run_script import MobioRunScript
+    VERSION_CONFIG = {
+        "every_deploy": {
+            "script": [
+                "PYTHONPATH=./ python3.8 -u sync_mongodb_index.py",
+                "PYTHONPATH=./ python3.8 -u sync_kafka_topic.py"
+            ]
+        },
+        "version": {
+            1: ["PYTHONPATH=./ python3.8 -u scripts/script_1.py",
+                "PYTHONPATH=./ python3.8 -u scripts/script_2.py"],
+            2: ["PYTHONPATH=./ python3.8 -u scripts/script_3.py"]
+        }
+    }
+
+    MobioRunScript().run_script_by_version(VERSION_CONFIG)
+
+   ```
+#### Log - 1.0.0
+    - release sdk
+
+#### Log - 1.0.1
+    - update
+    
+#### Log - 1.0.2
+    - chạy script theo thứ tự
+
```

### Comparing `m-run-script-test-1.0.1/README.md` & `m-run-script-test-1.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -27,8 +27,14 @@
     }
 
     MobioRunScript().run_script_by_version(VERSION_CONFIG)
 
    ```
 #### Log - 1.0.0
     - release sdk
+
+#### Log - 1.0.1
+    - update
+    
+#### Log - 1.0.2
+    - chạy script theo thứ tự
```

### Comparing `m-run-script-test-1.0.1/m_run_script_test.egg-info/PKG-INFO` & `m-run-script-test-1.0.2/m_run_script_test.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 Metadata-Version: 2.1
 Name: m-run-script-test
-Version: 1.0.1
+Version: 1.0.2
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ### Run Script
-        Thư viện xử lý chạy các script của project mỗi khi deploy version mới, sau khi chạy xong thì lưu lại vết script đã chạy để lần sau không chạy lại nữa. 
-        
-        
-        ### Cài đặt:
-        ```bash
-         $ pip3 install m-run-script
-         ```
-        
-        ### Sử dụng:
-        
-        ##### Chạy các script của project:
-           ```python
-            from mobio.libs.run_script import MobioRunScript
-            VERSION_CONFIG = {
-                "every_deploy": {
-                    "script": [
-                        "PYTHONPATH=./ python3.8 -u sync_mongodb_index.py",
-                        "PYTHONPATH=./ python3.8 -u sync_kafka_topic.py"
-                    ]
-                },
-                "version": {
-                    1: ["PYTHONPATH=./ python3.8 -u scripts/script_1.py",
-                        "PYTHONPATH=./ python3.8 -u scripts/script_2.py"],
-                    2: ["PYTHONPATH=./ python3.8 -u scripts/script_3.py"]
-                }
-            }
-        
-            MobioRunScript().run_script_by_version(VERSION_CONFIG)
-        
-           ```
-        #### Log - 1.0.0
-            - release sdk
-            
 Keywords: mobio,mobio-script,version-script
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+### Run Script
+Thư viện xử lý chạy các script của project mỗi khi deploy version mới, sau khi chạy xong thì lưu lại vết script đã chạy để lần sau không chạy lại nữa. 
+
+
+### Cài đặt:
+```bash
+ $ pip3 install m-run-script
+ ```
+
+### Sử dụng:
+
+##### Chạy các script của project:
+   ```python
+    from mobio.libs.run_script import MobioRunScript
+    VERSION_CONFIG = {
+        "every_deploy": {
+            "script": [
+                "PYTHONPATH=./ python3.8 -u sync_mongodb_index.py",
+                "PYTHONPATH=./ python3.8 -u sync_kafka_topic.py"
+            ]
+        },
+        "version": {
+            1: ["PYTHONPATH=./ python3.8 -u scripts/script_1.py",
+                "PYTHONPATH=./ python3.8 -u scripts/script_2.py"],
+            2: ["PYTHONPATH=./ python3.8 -u scripts/script_3.py"]
+        }
+    }
+
+    MobioRunScript().run_script_by_version(VERSION_CONFIG)
+
+   ```
+#### Log - 1.0.0
+    - release sdk
+
+#### Log - 1.0.1
+    - update
+    
+#### Log - 1.0.2
+    - chạy script theo thứ tự
+
```

### Comparing `m-run-script-test-1.0.1/mobio/libs/run_script/__init__.py` & `m-run-script-test-1.0.2/mobio/libs/run_script/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,17 +110,18 @@
     def save_result_script(cls, json_result):
         data_file = json.dumps(json_result)
         cls.save_data_to_file(PathFile.FILE_SCRIPT_RESULT, data_file)
 
     @classmethod
     def save_result_init_container(cls, value):
         # save_data_to_file(PathFile.FILE_CONTAINER_RESULT, value)
-        if value == ParamConfig.success:
-            image_name = cls.get_name_image_version()
-            cls.save_data_to_file(PathFile.IMAGE_VERSION, image_name)
+        # if value == ParamConfig.success:
+        #     image_name = cls.get_name_image_version()
+        #     cls.save_data_to_file(PathFile.IMAGE_VERSION, image_name)
+        pass
 
     @classmethod
     def run_script_has_first_deploy(cls, script_config):
         """
         :param script_config:
             {
                 "first_deploy": {
@@ -260,75 +261,80 @@
                     ]
                 },
                 "version": {
                 }
             }
         :return:
         """
-        try:
-            # script_result:
-            # {
-            # 	"first_deploy": {
-            #       "script_executed": [],
-            #       "status_success": 1/0
-            # 	},
-            # 	"every_deploy": {
-            # 		"script_executed": ["PYTHONPATH=./ python3.8 -u sync_kafka_topic.py",
-            # 		"PYTHONPATH=./ python3.8 -u sync_mongodb_index.py"]
-            # 	},
-            # 	"version": {
-            # 		"1": ["PYTHONPATH=./ python3.8 -u scripts/script_init_database.py"],
-            # 		"2": ["PYTHONPATH=./ python3.8 -u scripts/script_init_database.py"]
-            # 	}
-            # }
-            script_result = cls.get_json_script_result()
-            if ParamConfig.every_deploy not in script_result:
-                script_result[ParamConfig.every_deploy] = {}
-            if ParamConfig.version not in script_result:
-                script_result[ParamConfig.version] = {}
 
-            every_deploy_script = list(set(script_config.get(ParamConfig.every_deploy, {}).get(ParamConfig.script, [])))
-            print("run_script every_deploy_script: {}".format(every_deploy_script))
-            for script_run in every_deploy_script:
-                if cls.call_script(script_run) != 0:
-                    return cls.save_result_script(script_result)
-            script_result.get(ParamConfig.every_deploy, {})[ParamConfig.script_executed] = every_deploy_script
-            print("run_script script_result every_deploy: {}".format(script_result))
-
-            script_config[ParamConfig.version] = {int(k): v for k, v in
-                                                  script_config.get(ParamConfig.version, {}).items()}
-            script_result[ParamConfig.version] = {int(k): v for k, v in
-                                                  script_result.get(ParamConfig.version, {}).items()}
-            list_version = list(script_config.get(ParamConfig.version, {}).keys())
-            list_version.sort()
-            list_version_result = list(script_result.get(ParamConfig.version, {}).keys())
-            list_version_result.sort()
-            last_version = list_version_result[-1] if list_version_result else None
-            if last_version and last_version in list_version:
-                # lay script cuoi lan trc chay de dam bao da chay du
-                index_last = list_version.index(last_version)
-                list_version = list_version[index_last:]
-            print("run_script list_version: {}".format(list_version))
+        # script_result:
+        # {
+        # 	"first_deploy": {
+        #       "script_executed": [],
+        #       "status_success": 1/0
+        # 	},
+        # 	"every_deploy": {
+        # 		"script_executed": ["PYTHONPATH=./ python3.8 -u sync_kafka_topic.py",
+        # 		"PYTHONPATH=./ python3.8 -u sync_mongodb_index.py"]
+        # 	},
+        # 	"version": {
+        # 		"1": ["PYTHONPATH=./ python3.8 -u scripts/script_init_database.py"],
+        # 		"2": ["PYTHONPATH=./ python3.8 -u scripts/script_init_database.py"]
+        # 	}
+        # }
+        script_result = cls.get_json_script_result()
+        if ParamConfig.every_deploy not in script_result:
+            script_result[ParamConfig.every_deploy] = {}
+        if ParamConfig.version not in script_result:
+            script_result[ParamConfig.version] = {}
+
+        every_deploy_script = script_config.get(ParamConfig.every_deploy, {}).get(ParamConfig.script, [])
+        print("run_script every_deploy_script: {}".format(every_deploy_script))
+        for script_run in every_deploy_script:
+            if cls.call_script(script_run) != 0:
+                cls.raise_error_run_script(script_run)
+        script_result.get(ParamConfig.every_deploy, {})[ParamConfig.script_executed] = every_deploy_script
+        print("run_script script_result every_deploy: {}".format(script_result))
+
+        script_config[ParamConfig.version] = {int(k): v for k, v in
+                                              script_config.get(ParamConfig.version, {}).items()}
+        script_result[ParamConfig.version] = {int(k): v for k, v in
+                                              script_result.get(ParamConfig.version, {}).items()}
+        list_version = list(script_config.get(ParamConfig.version, {}).keys())
+        list_version.sort()
+        list_version_result = list(script_result.get(ParamConfig.version, {}).keys())
+        list_version_result.sort()
+        last_version = list_version_result[-1] if list_version_result else None
+        if last_version and last_version in list_version:
+            # lay script cuoi lan trc chay de dam bao da chay du
+            index_last = list_version.index(last_version)
+            list_version = list_version[index_last:]
+        print("run_script list_version: {}".format(list_version))
+
+        for version in list_version:
+            list_script_old = script_result.get(ParamConfig.version, {}).get(version, [])
+            list_script_new = script_config.get(ParamConfig.version, {}).get(version, [])
+            print("run_script version: {} list script: {}".format(version, list_script_new))
+            for script_run in list_script_new:
+                if script_run in list_script_old:
+                    print("{} has run".format(script_run))
+                    continue
+                if cls.call_script(script_run) != 0:  # call fail
+                    cls.save_result_script(script_result)
+                    cls.raise_error_run_script(script_run)
+                list_script_old.append(script_run)
+                script_result.get(ParamConfig.version, {})[version] = list_script_old
+        print("run_script script_result: {}".format(script_result))
+        cls.save_result_script(script_result)
+        cls.save_result_init_container(value=ParamConfig.success)
 
-            for version in list_version:
-                list_script_old = script_result.get(ParamConfig.version, {}).get(version, [])
-                list_script_new = script_config.get(ParamConfig.version, {}).get(version, [])
-                first_script_need_run = list(set(list_script_new) - set(list_script_old))
-                print("run_script version: {} list script: {}".format(version, first_script_need_run))
-                for script_run in first_script_need_run:
-                    if cls.call_script(script_run) != 0:  # call fail
-                        return cls.save_result_script(script_result)
-                    list_script_old.append(script_run)
-                    script_result.get(ParamConfig.version, {})[version] = list_script_old
-            print("run_script script_result version: {}".format(script_result))
-            cls.save_result_script(script_result)
-            cls.save_result_init_container(value=ParamConfig.success)
-        except Exception as err:
-            print("run_script err: {}".format(err))
 
+    @classmethod
+    def raise_error_run_script(cls, script_run):
+        raise ValueError("{} RUN FAIL".format(script_run))
 
     # def check_result_run_script():
     #     time.sleep(10)
     #     print("check_result_run_script file: {}".format(PathFile.FILE_CONTAINER_RESULT))
     #     content = get_content_from_file(PathFile.FILE_CONTAINER_RESULT)
     #     print("check_result_run_script content: {}".format(content))
     #     while True:
```

### Comparing `m-run-script-test-1.0.1/setup.py` & `m-run-script-test-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='1.0.1'
-version_prod='1.0.0'
+version_dev='1.0.2'
+version_prod='1.0.1'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -62,15 +62,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.1',  # Required
+    version='1.0.2',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

