# Comparing `tmp/cccs-yara-2.0.tar.gz` & `tmp/cccs-yara-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cccs-yara-2.0.tar", last modified: Tue Jul 18 19:59:24 2023, max compression
+gzip compressed data, was "cccs-yara-2.1.tar", last modified: Sat Jul 22 04:24:42 2023, max compression
```

## Comparing `cccs-yara-2.0.tar` & `cccs-yara-2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:24.616708 cccs-yara-2.0/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:24.616708 cccs-yara-2.0/.github/
--rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-07-18 19:59:12.000000 cccs-yara-2.0/.github/dependabot.yml
--rw-r--r--   0 vsts      (1001) docker     (122)       33 2023-07-18 19:59:12.000000 cccs-yara-2.0/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:12.000000 cccs-yara-2.0/.gitmodules
--rw-r--r--   0 vsts      (1001) docker     (122)     9638 2023-07-18 19:59:12.000000 cccs-yara-2.0/CCCS_YARA.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     7912 2023-07-18 19:59:12.000000 cccs-yara-2.0/CCCS_YARA_values.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     1401 2023-07-18 19:59:12.000000 cccs-yara-2.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)    12251 2023-07-18 19:59:24.616708 cccs-yara-2.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    12079 2023-07-18 19:59:12.000000 cccs-yara-2.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:24.616708 cccs-yara-2.0/cccs_yara.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    12251 2023-07-18 19:59:24.000000 cccs-yara-2.0/cccs_yara.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      784 2023-07-18 19:59:24.000000 cccs-yara-2.0/cccs_yara.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-18 19:59:24.000000 cccs-yara-2.0/cccs_yara.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-18 19:59:24.000000 cccs-yara-2.0/cccs_yara.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-18 19:59:24.000000 cccs-yara-2.0/cccs_yara.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-07-18 19:59:24.000000 cccs-yara-2.0/cccs_yara.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:24.616708 cccs-yara-2.0/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (122)     1141 2023-07-18 19:59:12.000000 cccs-yara-2.0/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-18 19:59:12.000000 cccs-yara-2.0/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-07-18 19:59:12.000000 cccs-yara-2.0/settings.json
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-18 19:59:24.616708 cccs-yara-2.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      688 2023-07-18 19:59:12.000000 cccs-yara-2.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:24.616708 cccs-yara-2.0/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      435 2023-07-18 19:59:12.000000 cccs-yara-2.0/templates/CCCS_Yara_Template.yara
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:24.616708 cccs-yara-2.0/yara_validator/
--rw-r--r--   0 vsts      (1001) docker     (122)     9638 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/CCCS_YARA.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     7912 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/CCCS_YARA_values.yml
--rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14526 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)      556 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/constants.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:24.616708 cccs-yara-2.0/yara_validator/stix2_patch/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/stix2_patch/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1167 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/stix2_patch/filter_casefold.py
--rw-r--r--   0 vsts      (1001) docker     (122)    43219 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/validator.py
--rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/validator_cfg.yml
--rw-r--r--   0 vsts      (1001) docker     (122)    42885 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/validator_functions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30198 2023-07-18 19:59:12.000000 cccs-yara-2.0/yara_validator/yara_file_processor.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:42.864988 cccs-yara-2.1/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:42.860988 cccs-yara-2.1/.github/
+-rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-07-22 04:24:30.000000 cccs-yara-2.1/.github/dependabot.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)       33 2023-07-22 04:24:30.000000 cccs-yara-2.1/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:30.000000 cccs-yara-2.1/.gitmodules
+-rw-r--r--   0 vsts      (1001) docker     (122)     9638 2023-07-22 04:24:30.000000 cccs-yara-2.1/CCCS_YARA.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     7912 2023-07-22 04:24:30.000000 cccs-yara-2.1/CCCS_YARA_values.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1401 2023-07-22 04:24:30.000000 cccs-yara-2.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)    12251 2023-07-22 04:24:42.864988 cccs-yara-2.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    12079 2023-07-22 04:24:30.000000 cccs-yara-2.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:42.864988 cccs-yara-2.1/cccs_yara.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    12251 2023-07-22 04:24:42.000000 cccs-yara-2.1/cccs_yara.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      784 2023-07-22 04:24:42.000000 cccs-yara-2.1/cccs_yara.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-22 04:24:42.000000 cccs-yara-2.1/cccs_yara.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-22 04:24:42.000000 cccs-yara-2.1/cccs_yara.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-22 04:24:42.000000 cccs-yara-2.1/cccs_yara.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-07-22 04:24:42.000000 cccs-yara-2.1/cccs_yara.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:42.864988 cccs-yara-2.1/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1141 2023-07-22 04:24:30.000000 cccs-yara-2.1/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-22 04:24:30.000000 cccs-yara-2.1/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      785 2023-07-22 04:24:30.000000 cccs-yara-2.1/settings.json
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-22 04:24:42.864988 cccs-yara-2.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      688 2023-07-22 04:24:30.000000 cccs-yara-2.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:42.864988 cccs-yara-2.1/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      435 2023-07-22 04:24:30.000000 cccs-yara-2.1/templates/CCCS_Yara_Template.yara
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:42.864988 cccs-yara-2.1/yara_validator/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9638 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/CCCS_YARA.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     7912 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/CCCS_YARA_values.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14526 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      556 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/constants.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:42.864988 cccs-yara-2.1/yara_validator/stix2_patch/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/stix2_patch/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1167 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/stix2_patch/filter_casefold.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    43219 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/validator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/validator_cfg.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)    40919 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/validator_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30198 2023-07-22 04:24:30.000000 cccs-yara-2.1/yara_validator/yara_file_processor.py
```

### Comparing `cccs-yara-2.0/CCCS_YARA.yml` & `cccs-yara-2.1/CCCS_YARA.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/CCCS_YARA_values.yml` & `cccs-yara-2.1/CCCS_YARA_values.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/LICENSE` & `cccs-yara-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/PKG-INFO` & `cccs-yara-2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cccs-yara
-Version: 2.0
+Version: 2.1
 Summary: A CCCS utility for YARA rule metadata validation
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Canadian Centre for Cyber Security
 
 ## CCCS YARA Specification
```

### Comparing `cccs-yara-2.0/README.md` & `cccs-yara-2.1/README.md`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/cccs_yara.egg-info/PKG-INFO` & `cccs-yara-2.1/cccs_yara.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cccs-yara
-Version: 2.0
+Version: 2.1
 Summary: A CCCS utility for YARA rule metadata validation
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Canadian Centre for Cyber Security
 
 ## CCCS YARA Specification
```

### Comparing `cccs-yara-2.0/cccs_yara.egg-info/SOURCES.txt` & `cccs-yara-2.1/cccs_yara.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/pipelines/publish.yaml` & `cccs-yara-2.1/pipelines/publish.yaml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/settings.json` & `cccs-yara-2.1/settings.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925%*

 * *Differences: {"'yara.metaEntries'": "{'date': '${CURRENT_YEAR}-${CURRENT_MONTH}-${CURRENT_DATE}', 'modified': "*

 * *                       "'${CURRENT_YEAR}-${CURRENT_MONTH}-${CURRENT_DATE}', 'minimum_yara': '4.2', "*

 * *                       "delete: ['creation_date', 'last_modified', 'yara_version']}"}*

```diff
@@ -1,22 +1,22 @@
 {
     "yara.metaEntries": {
         "actor": "<known_mitre_alias>",
         "actor_type": "APT|CRIMEWARE|FIN",
         "author": "analyst@CCCS",
         "category": "INFO|EXPLOIT|TECHNIQUE|TOOL|MALWARE",
-        "creation_date": "${CURRENT_YEAR}-${CURRENT_MONTH}-${CURRENT_DATE}",
+        "date": "${CURRENT_YEAR}-${CURRENT_MONTH}-${CURRENT_DATE}",
         "description": "",
         "hash": "d9fcd5af3564d87dc22f1e72763a7959",
-        "last_modified": "${CURRENT_YEAR}-${CURRENT_MONTH}-${CURRENT_DATE}",
         "malware_type": "",
+        "minimum_yara": "4.2",
         "mitre_att": "TA####|T####|M####|G####|S####",
+        "modified": "${CURRENT_YEAR}-${CURRENT_MONTH}-${CURRENT_DATE}",
         "reference": "https://cccs/report.html",
         "report": "TA20-0192",
         "sharing": "TLP:AMBER",
         "source": "CCCS",
         "status": "TESTING|RELEASED|DEPRECATED",
-        "version": "1.0",
-        "yara_version": "4.2"
+        "version": "1.0"
     },
     "yara.sortMeta": false
 }
```

### Comparing `cccs-yara-2.0/setup.py` & `cccs-yara-2.1/setup.py`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/yara_validator/CCCS_YARA.yml` & `cccs-yara-2.1/yara_validator/CCCS_YARA.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/yara_validator/CCCS_YARA_values.yml` & `cccs-yara-2.1/yara_validator/CCCS_YARA_values.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/yara_validator/cli.py` & `cccs-yara-2.1/yara_validator/cli.py`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/yara_validator/constants.py` & `cccs-yara-2.1/yara_validator/constants.py`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/yara_validator/stix2_patch/filter_casefold.py` & `cccs-yara-2.1/yara_validator/stix2_patch/filter_casefold.py`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/yara_validator/validator.py` & `cccs-yara-2.1/yara_validator/validator.py`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/yara_validator/validator_cfg.yml` & `cccs-yara-2.1/yara_validator/validator_cfg.yml`

 * *Files identical despite different names*

### Comparing `cccs-yara-2.0/yara_validator/validator_functions.py` & `cccs-yara-2.1/yara_validator/validator_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,34 @@
 from yara_validator.stix2_patch.filter_casefold import FilterCasefold
 
 METADATA = 'metadata'
 BASE62_REGEX = r'^[0-9a-zA-z]+$'
 UNIVERSAL_REGEX = r'^[^a-z]*$'
 MITRE_GROUP_NAME = 'name'
 CHILD_PLACE_HOLDER = 'child_place_holder'
-DATE_FORMATS = ["%Y-%m", "%Y.%m", "%Y/%m",
-                "%m/%d/%Y", "%m/%d/%y", "%d/%m/%Y", "%d/%m/%y",
-                "%d-%m-%Y", "%m-%d-%Y", "%m-%d-%y", "%Y-%m-%d",
-                "%d.%m.%Y", "%m.%d.%Y", "%m.%d.%y", "%Y.%m.%d",
-                "%f/%e/%Y", "%f/%e/%y", "%e/%f/%Y", "%e/%f/%y",
-                "%f-%e-%Y", "%f-%e-%y", "%e-%f-%Y", "%e-%f-%y",
-                "%f.%e.%Y", "%f.%e.%y", "%e.%f.%Y", "%e.%f.%y",
-                "%b %e, %Y", "%B %e, %Y",
-                "%b %d, %Y", "%B %d, %Y",
-                "%b %e %Y", "%B %e %Y", "%e %b %Y", "%e %B %Y",
-                "%b %d %Y", "%B %d %Y", "%d %b %Y", "%d %B %Y",
-                "%Y-%m-%d %I:%M:%S %p", "%Y-%m-%d %I:%M:%S %p"]
+DATE_FORMATS = [
+    "%Y-%m", "%Y.%m", "%Y/%m",
+    "%m/%d/%Y", "%d/%m/%Y",
+    "%m/%d/%y", "%d/%m/%y",
+    "%Y/%d/%m", "%y/%d/%m",
+    "%Y/%m/%d", "%y/%m/%d",
+    "%Y.%d.%m", "%y.%d.%m",
+    "%Y.%m.%d", "%y.%m.%d",
+    "%d-%m-%Y", "%m-%d-%Y", "%m-%d-%y", "%Y-%m-%d",
+    "%d.%m.%Y", "%m.%d.%Y", "%m.%d.%y", "%Y.%m.%d",
+    "%f/%e/%Y", "%f/%e/%y", "%e/%f/%Y", "%e/%f/%y",
+    "%f-%e-%Y", "%f-%e-%y", "%e-%f-%Y", "%e-%f-%y",
+    "%f.%e.%Y", "%f.%e.%y", "%e.%f.%Y", "%e.%f.%y",
+    "%b %e, %Y", "%B %e, %Y",
+    "%b %d, %Y", "%B %d, %Y",
+    "%b %e %Y", "%B %e %Y", "%e %b %Y", "%e %B %Y",
+    "%b %d %Y", "%B %d %Y", "%d %b %Y", "%d %B %Y",
+    "%Y-%m-%d %I:%M:%S %p", "%Y/%m/%d %I:%M:%S %p"
+    "%Y-%m-%d %H:%M:%S", "%Y/%m/%d %H:%M:%S"
+]
 
 
 # potential values of MetadataAttributes.optional variable
 class MetadataOpt(Enum):
     REQ_PROVIDED = 'req_provided'
     REQ_OPTIONAL = 'req_optional'
     OPT_OPTIONAL = 'opt_optional'
@@ -165,14 +173,19 @@
         :param metadata_index: used to reference what the array index of the id metadata value is
         :param metadata_key: the name of the metadata value that is being processed
         :return: True if the value of the metadata value follows the regex expression or
             False if the value is does not match the expression
         """
         value = list(rule_to_validate[METADATA][metadata_index].values())[0]
 
+        if METADATA == 'hash':
+            # Strip any whitespace before validation
+            value = str(value).strip()
+            rule_to_validate[METADATA].insert(metadata_index, {METADATA: value})
+
         self.required_fields[metadata_key].attributefound()
         self.required_fields_index[self.required_fields[metadata_key].position].increment_count()
 
         regex_expression = self.required_fields[metadata_key].argument.get('regexExpression')
 
         if re.fullmatch(regex_expression, value):
             self.required_fields[metadata_key].attributevalid()
@@ -373,54 +386,14 @@
 
         if self.required_fields[MITRE_ATT].valid and mitre_att_to_validate.startswith('S'):
             soft_codes_found = self.required_fields[MITRE_ATT].check_argument_list_var(MITRE_SOFTWAREID_FOUND)
             soft_codes_found.append(mitre_att_to_validate)
 
         return self.required_fields[MITRE_ATT].valid
 
-    def valid_al_config_dumper(self, rule_to_validate_al_config_d, metadata_index, metadata_key, alias=None):
-        """
-        Makes the al_config_parser metadata value required if this is found first.
-        :param rule_to_validate_al_config_d: the plyara parsed rule that is being validated
-        :param metadata_index: used to reference what the array index of the actor metadata value is
-        :param metadata_key: the name of the metadata value that is being processed
-        :return: True all the time because the value is never verified...
-        """
-        AL_CONFIG_D = metadata_key
-        self.required_fields[AL_CONFIG_D].attributefound()
-        self.required_fields_index[self.required_fields[AL_CONFIG_D].position].increment_count()
-
-        # Because there is an al_config_dumper al_config_parser becomes required
-        self.required_fields[AL_CONFIG_D].optional = MetadataOpt.REQ_PROVIDED
-
-        # Because we are not validating the value... So much pain!
-        self.required_fields[AL_CONFIG_D].attributevalid()
-
-        return self.required_fields[AL_CONFIG_D].valid
-
-    def valid_al_config_parser(self, rule_to_validate_al_config_p, metadata_index, metadata_key, alias=None):
-        """
-        Makes the al_config_dumper metadata value required if this is found first.
-        :param rule_to_validate_al_config_p: the plyara parsed rule that is being validated
-        :param metadata_index: used to reference what the array index of the actor metadata value is
-        :param metadata_key: the name of the metadata value that is being processed
-        :return: True all the time because the value is never verified...
-        """
-        AL_CONFIG_P = metadata_key
-        self.required_fields[AL_CONFIG_P].attributefound()
-        self.required_fields_index[self.required_fields[AL_CONFIG_P].position].increment_count()
-
-        # Because there is an al_config_parser al_config_dumper becomes required
-        self.required_fields[AL_CONFIG_P].optional = MetadataOpt.REQ_PROVIDED
-
-        # Because we are not validating the value... So much pain!
-        self.required_fields[AL_CONFIG_P].attributevalid()
-
-        return self.required_fields[AL_CONFIG_P].valid
-
     def valid_category(self, rule_to_validate_category, metadata_index, metadata_key, alias=None):
         """
         Pulls the value of the category metadata value and checks if it is a valid category type.
             Valid options are stored in self.category_types. If the category value is valid and a new metadata
             metadata with a name the same as the category value is added to be searched for.
             This new metadata value links to the same object as the initially created
             self.required_fields[CATEGORY_TYPE].
```

### Comparing `cccs-yara-2.0/yara_validator/yara_file_processor.py` & `cccs-yara-2.1/yara_validator/yara_file_processor.py`

 * *Files identical despite different names*

