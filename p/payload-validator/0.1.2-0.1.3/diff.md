# Comparing `tmp/payload-validator-0.1.2.tar.gz` & `tmp/payload-validator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\payload-validator-0.1.2.tar", last modified: Sat Jul 22 08:37:06 2023, max compression
+gzip compressed data, was "dist\payload-validator-0.1.3.tar", last modified: Sat Jul 22 09:13:39 2023, max compression
```

## Comparing `payload-validator-0.1.2.tar` & `payload-validator-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 08:37:06.000000 payload-validator-0.1.2/
--rw-rw-rw-   0        0        0       74 2023-07-22 08:07:09.000000 payload-validator-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    11818 2023-07-22 08:37:06.000000 payload-validator-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    11050 2023-07-22 08:32:26.000000 payload-validator-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator/
--rw-rw-rw-   0        0        0        0 2023-07-22 07:50:18.000000 payload-validator-0.1.2/payload_validator/__init__.py
--rw-rw-rw-   0        0        0      837 2023-07-22 05:40:00.000000 payload-validator-0.1.2/payload_validator/exceptions.py
--rw-rw-rw-   0        0        0     5102 2023-07-22 08:36:39.000000 payload-validator-0.1.2/payload_validator/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/
--rw-rw-rw-   0        0        0    11818 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      796 2023-07-22 08:37:06.000000 payload-validator-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       68 2023-07-22 07:54:29.000000 payload-validator-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:13:39.000000 payload-validator-0.1.3/
+-rw-rw-rw-   0        0        0       74 2023-07-22 08:07:09.000000 payload-validator-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    11818 2023-07-22 09:13:39.000000 payload-validator-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11050 2023-07-22 08:32:26.000000 payload-validator-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 09:13:39.000000 payload-validator-0.1.3/payload_validator/
+-rw-rw-rw-   0        0        0        0 2023-07-22 07:50:18.000000 payload-validator-0.1.3/payload_validator/__init__.py
+-rw-rw-rw-   0        0        0      877 2023-07-22 09:11:30.000000 payload-validator-0.1.3/payload_validator/exceptions.py
+-rw-rw-rw-   0        0        0     5102 2023-07-22 09:11:30.000000 payload-validator-0.1.3/payload_validator/validators.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:13:39.000000 payload-validator-0.1.3/payload_validator.egg-info/
+-rw-rw-rw-   0        0        0    11818 2023-07-22 09:13:39.000000 payload-validator-0.1.3/payload_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-22 09:13:39.000000 payload-validator-0.1.3/payload_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:13:39.000000 payload-validator-0.1.3/payload_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-22 09:13:39.000000 payload-validator-0.1.3/payload_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      796 2023-07-22 09:13:39.000000 payload-validator-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       68 2023-07-22 07:54:29.000000 payload-validator-0.1.3/setup.py
```

### Comparing `payload-validator-0.1.2/PKG-INFO` & `payload-validator-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload-validator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Validating payload datas for Python
 Home-page: https://github.com/cwadven/payload-validator
 Author: cwadven
 Author-email: cwadven4@gmail.com
 Maintainer: cwadven
 License: MIT
 Keywords: django random
```

### Comparing `payload-validator-0.1.2/README.rst` & `payload-validator-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.2/payload_validator/exceptions.py` & `payload-validator-0.1.3/payload_validator/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,10 +16,12 @@
 
 class InvalidValueError(Exception):
     def __init__(self, error_value_by_key: Dict[str, str], skip_existing_errors: list = None):
         if skip_existing_errors is None:
             skip_existing_errors = []
         result = [key for key in skip_existing_errors if key not in error_value_by_key.keys()]
         if result:
-            raise MismatchedErrorKeysException(f"In error_exists_skip_keys {', '.join(result)} not in error_value_by_key")
+            raise MismatchedErrorKeysException(
+                "In error_exists_skip_keys {} not in error_value_by_key".format(', '.join(result))
+            )
         self.error_value_by_key = error_value_by_key
         self.skip_existing_errors = skip_existing_errors
```

### Comparing `payload-validator-0.1.2/payload_validator/validators.py` & `payload-validator-0.1.3/payload_validator/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from payload_validator.exceptions import (
     InvalidValueError,
     ValidationException,
     ValidationNotRunException,
 )
 
 
-T = TypeVar('T')  # Use TypeVar for arbitrary object types
+T = TypeVar("T")  # Use TypeVar for arbitrary object types
 
 
 class ValidatorErrorContext(ABC, dict):
     @abstractmethod
     def add_error(self, field: str, error: str):
         pass
 
@@ -27,50 +27,50 @@
 class NormalValidatorErrorContext(ValidatorErrorContext):
     def add_error(self, field: str, error: str):
         value = self.setdefault(field, [])
         value.append(error)
 
 
 class PayloadValidator(object):
-    DEFAULT_MANDATORY_ERROR_MESSAGE = 'mandatory data missing'
+    DEFAULT_MANDATORY_ERROR_MESSAGE = "mandatory data missing"
 
     def __init__(self, payload: dict, error_context: ValidatorErrorContext = None) -> None:
         self.payload = payload
         self._skip_validate_keys = set()
         self._validate_called = False
         self._error_context = (
             error_context
             if error_context is not None
             else NormalValidatorErrorContext()
         )
 
         self.meta = self._get_meta_attribute()
         if self.meta:
-            self.mandatory_keys = getattr(self.meta, 'mandatory_keys', {})
-            self.type_of_keys = getattr(self.meta, 'type_of_keys', {})
+            self.mandatory_keys = getattr(self.meta, "mandatory_keys", {})
+            self.type_of_keys = getattr(self.meta, "type_of_keys", {})
 
     def add_error_context(self, key: str, description: str) -> None:
         if key not in self._skip_validate_keys:
             self._error_context.add_error(key, description)
 
     def add_error_and_skip_validation_key(self, key: str, description: str) -> None:
         """
         add only main error so other errors cannot add
         """
         self.add_error_context(key, description)
         self._skip_validate_keys.add(key)
 
     def _get_meta_attribute(self) -> Optional[T]:
-        return getattr(self, 'Meta', None)
+        return getattr(self, "Meta", None)
 
     def _validate_mandatory_payloads(self) -> None:
         """
         mandatory_keys example:
         {
-            'displayable': 'displayable is required',  # if error message is not provided, default message will be used
+            "displayable": "displayable is required",  # if error message is not provided, default message will be used
         }
         """
         for key, error_message in self.mandatory_keys.items():
             if self.payload.get(key) is None:
                 self.add_error_and_skip_validation_key(key, error_message or self.DEFAULT_MANDATORY_ERROR_MESSAGE)
 
     def _validate_payloads_type(self) -> None:
@@ -108,15 +108,15 @@
         """
         override this method to add custom validation
         """
         pass
 
     def _validate_methods(self) -> None:
         for x, y in self.__class__.__dict__.items():
-            if type(y) == FunctionType and x.startswith('validate'):
+            if type(y) == FunctionType and x.startswith("validate"):
                 try:
                     y(self)
                 except InvalidValueError as e:
                     for key, value in e.error_value_by_key.items():
                         if key in e.skip_existing_errors:
                             self.add_error_and_skip_validation_key(key, value)
                         else:
@@ -131,15 +131,15 @@
             self._validate_called = True
         if self._error_context:
             raise ValidationException()
 
     @property
     def error_context(self) -> ValidatorErrorContext:
         if not self._validate_called:
-            raise ValidationNotRunException('validate method should run before accessing error_context')
+            raise ValidationNotRunException("validate method should run before accessing error_context")
         return self._error_context
 
     def is_valid(self) -> bool:
         try:
             self.validate()
         except ValidationException:
             return False
```

### Comparing `payload-validator-0.1.2/payload_validator.egg-info/PKG-INFO` & `payload-validator-0.1.3/payload_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload-validator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Validating payload datas for Python
 Home-page: https://github.com/cwadven/payload-validator
 Author: cwadven
 Author-email: cwadven4@gmail.com
 Maintainer: cwadven
 License: MIT
 Keywords: django random
```

### Comparing `payload-validator-0.1.2/setup.cfg` & `payload-validator-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6179 6c6f 6164 2d76 616c 6964   = payload-valid
 00000020: 6174 6f72 0d0a 7665 7273 696f 6e20 3d20  ator..version = 
-00000030: 302e 312e 320d 0a61 7574 686f 7220 3d20  0.1.2..author = 
+00000030: 302e 312e 330d 0a61 7574 686f 7220 3d20  0.1.3..author = 
 00000040: 6377 6164 7665 6e0d 0a61 7574 686f 725f  cwadven..author_
 00000050: 656d 6169 6c20 3d20 6377 6164 7665 6e34  email = cwadven4
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6d61 696e  @gmail.com..main
 00000070: 7461 696e 6572 203d 2063 7761 6476 656e  tainer = cwadven
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5661 6c69 6461 7469 6e67 2070 6179 6c6f  Validating paylo
 000000a0: 6164 2064 6174 6173 2066 6f72 2050 7974  ad datas for Pyt
```

