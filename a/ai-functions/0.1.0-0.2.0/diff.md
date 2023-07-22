# Comparing `tmp/ai_functions-0.1.0.tar.gz` & `tmp/ai_functions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_functions-0.1.0.tar", max compression
+gzip compressed data, was "ai_functions-0.2.0.tar", max compression
```

## Comparing `ai_functions-0.1.0.tar` & `ai_functions-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       25 2023-07-21 15:27:00.845052 ai_functions-0.1.0/ai_functions/__init__.py
--rw-r--r--   0        0        0     6269 2023-07-21 16:59:14.895973 ai_functions-0.1.0/ai_functions/functions.py
--rw-r--r--   0        0        0      476 2023-07-21 17:04:24.023198 ai_functions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1520 2023-07-21 17:19:00.362094 ai_functions-0.1.0/README.md
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 ai_functions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-07-22 07:26:46.226935 ai_functions-0.2.0/ai_functions/__init__.py
+-rw-r--r--   0        0        0     6422 2023-07-22 07:27:08.800500 ai_functions-0.2.0/ai_functions/functions.py
+-rw-r--r--   0        0        0      614 2023-07-22 07:25:48.828267 ai_functions-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1520 2023-07-21 17:19:00.362094 ai_functions-0.2.0/README.md
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 ai_functions-0.2.0/PKG-INFO
```

### Comparing `ai_functions-0.1.0/ai_functions/functions.py` & `ai_functions-0.2.0/ai_functions/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 }
 
 
 def convert_response(ret):
     # convert content to be a string, for sure
     try:
         content = ret if isinstance(ret, str) else json.dumps(ret)
-    except TypeError as e:
+    except TypeError:
         content = str(ret)
     return content
 
 
 class AIFunctions:
     def __init__(self, funcs=[], *, loop=None, convert_output=convert_response):
         self.map = dict({f.__name__: f for f in funcs})
@@ -40,33 +40,33 @@
         if funcs:
             names = [f if isinstance(f, str) else f.__name__ for f in funcs]
             funcs = [v for k, v in self.map.items() if k in names]
         else:
             funcs = self.map.values()
         return get_openai_dict(funcs)
 
-    def execute(self, name: str, args: Union[str, dict], *, loop=None):
+    def execute(self, name: str, args: Union[str, dict], *, loop=None, **kws):
         """Run a named function"""
         return execute_function([self.map[name]], name, args, loop=loop or self.loop,
-                                convert_output=self.convert_output)
+                                convert_output=self.convert_output, **kws)
 
-    def openai_execute(self, call: dict, *, loop=None):
+    def openai_execute(self, call: dict, *, loop=None, **kws):
         """Run an openai style function_call"""
         name, args = call["name"], call["arguments"]
         return execute_function([self.map[name]], name, args, loop=loop or self.loop,
-                                convert_output=self.convert_output)
+                                convert_output=self.convert_output, **kws)
 
-    async def async_execute(self, name, args):
+    async def async_execute(self, name, args, **kws):
         """Async run a named function"""
-        return async_execute_function([self.map[name]], name, args, convert_output=self.convert_output)
+        return async_execute_function([self.map[name]], name, args, convert_output=self.convert_output, **kws)
 
-    async def async_openai_execute(self, call):
+    async def async_openai_execute(self, call, **kws):
         """Async run an openai style function"""
         name, args = call["name"], call["arguments"]
-        return async_execute_function([self.map[name]], name, args, convert_output=self.convert_output)
+        return async_execute_function([self.map[name]], name, args, convert_output=self.convert_output, **kws)
 
     def __contains__(self, func):
         name = func if isinstance(func, str) else  func.__name__
         return name in self.map
 
     def description(self, name):
         """Get description of a function"""
@@ -93,14 +93,16 @@
         if param.annotation == inspect.Parameter.empty or param.annotation == Any:
             return None
         if get_origin(param.annotation) is not Annotated:
             return None
         base_type = get_args(param.annotation)[0]
         param_type = JSON_TYPE_MAP[base_type]
         param_description = param.annotation.__metadata__[0]
+        if param_description is None:
+            continue
         annotated_args[param_name] = {"type": param_type, "description": param_description}
     return annotated_args
 
 
 def get_openai_dict(funcs: Iterable[Callable] = None):
     ret = []
     for func in funcs:
@@ -123,27 +125,27 @@
             )
         ))
 
     return ret
 
 
 def execute_function(funcs: Iterable[Callable], name: str, arguments: Union[str, dict], *, loop=None,
-                     convert_output=convert_response):
+                     convert_output=convert_response, **kws):
     args, func = prepare_function(arguments, funcs, name)
-    ret = func(**args)
+    ret = func(**{**args, **kws})
     while inspect.iscoroutine(ret):
         if not loop:
             raise ValueError(f"Function {name} cannot be run, because we need a loop for async functions")
         ret = asyncio.run_coroutine_threadsafe(ret, loop=loop).result()
     return convert_output(ret) if convert_output else ret
 
 
-async def async_execute_function(funcs: Iterable[Callable], name: str, arguments: str, convert_output=convert_response):
-    args, func = prepare_function(arguments, funcs, name)
-    ret = await func(**args)
+async def async_execute_function(funcs: Iterable[Callable], name: str, arguments: str, convert_output=convert_response, **kws):
+    args, func = prepare_function(arguments, funcs, name, **kws)
+    ret = await func(**{**args, **kws})
     return convert_output(ret) if convert_output else ret
 
 
 def prepare_function(arguments: Union[str, dict], funcs: Iterable[Callable], name: str, auto_cast=True):
     func = {f.__name__: f for f in funcs}.get(name)
 
     if not func:
```

### Comparing `ai_functions-0.1.0/README.md` & `ai_functions-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_functions-0.1.0/PKG-INFO` & `ai_functions-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-functions
-Version: 0.1.0
+Version: 0.2.0
 Summary: manage openai functions and execution
 License: MIT
 Author: erik aronesty
 Author-email: erik@q32.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

