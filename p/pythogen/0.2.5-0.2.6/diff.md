# Comparing `tmp/pythogen-0.2.5.tar.gz` & `tmp/pythogen-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.2.5.tar", max compression
+gzip compressed data, was "pythogen-0.2.6.tar", max compression
```

## Comparing `pythogen-0.2.5.tar` & `pythogen-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-07-13 08:24:12.427281 pythogen-0.2.5/LICENSE
--rw-r--r--   0        0        0     2097 2023-07-13 08:24:12.427281 pythogen-0.2.5/README.md
--rw-r--r--   0        0        0     1567 2023-07-13 08:24:12.427281 pythogen-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 08:24:12.427281 pythogen-0.2.5/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1585 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/entrypoint.py
--rw-r--r--   0        0        0     7660 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/models.py
--rw-r--r--   0        0        0     2329 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3307 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/document.py
--rw-r--r--   0        0        0      576 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3239 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2132 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2437 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1074 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3512 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1810 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/response.py
--rw-r--r--   0        0        0    17663 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0    10011 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/renderer.py
--rw-r--r--   0        0        0      172 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/settings.py
--rw-r--r--   0        0        0     5149 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/client/httpx-method.j2
--rw-r--r--   0        0        0     1668 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/client/httpx-request-metrics.j2
--rw-r--r--   0        0        0    11016 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/httpx.j2
--rw-r--r--   0        0        0       33 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/init-py.j2
--rw-r--r--   0        0        0      312 2023-07-13 08:24:12.431281 pythogen-0.2.5/pythogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-21 22:56:27.787128 pythogen-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2097 2023-07-21 22:56:27.787128 pythogen-0.2.6/README.md
+-rw-r--r--   0        0        0     1616 2023-07-21 22:56:27.791128 pythogen-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1585 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/main.py
+-rw-r--r--   0        0        0     7660 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/models.py
+-rw-r--r--   0        0        0     2355 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3239 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-21 22:56:27.791128 pythogen-0.2.6/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    17663 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0    10037 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/renderer.py
+-rw-r--r--   0        0        0      286 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/settings.py
+-rw-r--r--   0        0        0    10891 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client/main.j2
+-rw-r--r--   0        0        0     5136 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client/method.j2
+-rw-r--r--   0        0        0     1513 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client/request-metrics.j2
+-rw-r--r--   0        0        0       33 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client_package/init-py.j2
+-rw-r--r--   0        0        0      312 2023-07-21 22:56:27.795128 pythogen-0.2.6/pythogen/templates/http_client_package/pyproject-toml.j2
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 pythogen-0.2.6/PKG-INFO
```

### Comparing `pythogen-0.2.5/LICENSE` & `pythogen-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/README.md` & `pythogen-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pyproject.toml` & `pythogen-0.2.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.2.5"
+version = "0.2.6"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
@@ -36,27 +36,29 @@
 jinja2 = "^3.1.1"
 rich = "^12.2.0"
 inflection = "^0.5.1"
 black = "^23.3.0"
 autoflake = "^2.2.0"
 isort = "^5.12.0"
 pydantic = "^2.0.2"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.scripts]
 pythogen = 'pythogen.entrypoint:run'
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 importlib-metadata = "^4.11.4"
 pre-commit = "^2.19.0"
 
 [tool.poetry.group.dev.dependencies]
 httpx = "^0.24.1"
 pydantic = "^2.0.0"
+pytest-asyncio = "^0.21.1"
 
 [build-system]
 requires = ["poetry>=1.4.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `pythogen-0.2.5/pythogen/entrypoint.py` & `pythogen-0.2.6/pythogen/main.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/models.py` & `pythogen-0.2.6/pythogen/models.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/packager.py` & `pythogen-0.2.6/pythogen/packager.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     _create_init_file(sources_path, package_name)
 
     return InitPackageResponse(client_output_path=str(sources_path.joinpath(f'{package_name}.py')))
 
 
 def _create_pyproject_file(output_dir: Path, package_name: str, version: str, authors: str | None = None) -> None:
     env = Environment(
-        loader=FileSystemLoader(settings.TEMPLATES_DIR_PATH),
+        loader=FileSystemLoader(settings.HTTP_PACKAGE_TEMPLATES_DIR_PATH),
         extensions=['jinja2.ext.loopcontrols'],
     )
     template = env.get_template('pyproject-toml.j2')
 
     pyproject_path = output_dir.joinpath('pyproject.toml')
 
     with open(pyproject_path, 'w') as pyproject_file:
@@ -55,15 +55,15 @@
                 authors=authors,
             )
         )
 
 
 def _create_init_file(output_dir: Path, module_name: str) -> None:
     env = Environment(
-        loader=FileSystemLoader(settings.TEMPLATES_DIR_PATH),
+        loader=FileSystemLoader(settings.HTTP_PACKAGE_TEMPLATES_DIR_PATH),
         extensions=['jinja2.ext.loopcontrols'],
     )
     template = env.get_template('init-py.j2')
 
     init_path = output_dir.joinpath('__init__.py')
 
     with open(init_path, 'w') as init_file:
```

### Comparing `pythogen-0.2.5/pythogen/parsers/document.py` & `pythogen-0.2.6/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.6/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/parsers/operations.py` & `pythogen-0.2.6/pythogen/parsers/operations.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/parsers/parameters.py` & `pythogen-0.2.6/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/parsers/paths.py` & `pythogen-0.2.6/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/parsers/references.py` & `pythogen-0.2.6/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/parsers/request_body.py` & `pythogen-0.2.6/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/parsers/response.py` & `pythogen-0.2.6/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/parsers/schemas.py` & `pythogen-0.2.6/pythogen/parsers/schemas.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.5/pythogen/renderer.py` & `pythogen-0.2.6/pythogen/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     Arguments
     ---------
     output_path
         Пудо до файла, в который запишется сгенерированный клиент
     document
         Спаршенный в python-объекты OpenApi-файл
     """
-    env = Environment(loader=FileSystemLoader(settings.TEMPLATES_DIR_PATH), extensions=['jinja2.ext.loopcontrols'])
+    env = Environment(
+        loader=FileSystemLoader(settings.HTTP_CLIENT_TEMPLATES_DIR_PATH), extensions=['jinja2.ext.loopcontrols']
+    )
     template = env.get_template(
         settings.CLIENT_TEMPLATE_NAME,
         globals={
             'varname': varname,
             'classname': classname,
             'typerepr': j2_typerepr,
             'responserepr': j2_responserepr,
```

### Comparing `pythogen-0.2.5/pythogen/templates/client/httpx-method.j2` & `pythogen-0.2.6/pythogen/templates/http_client/method.j2`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         # let library do it for us
         headers_.pop("Content-Type", None)
         {% endif %}
         if headers:
             headers_ = headers
 
 {%- with req_body=operation.request_body -%}
-{% include 'client/httpx-request-metrics.j2' %}
+{% include 'request-metrics.j2' %}
 {%- endwith %}
         req = RequestBox(
             client_name=self.client_name,
             method="{{ method }}",
             url=url,
             params=params,
             headers=headers_,
```

### Comparing `pythogen-0.2.5/pythogen/templates/client/httpx-request-metrics.j2` & `pythogen-0.2.6/pythogen/templates/http_client/request-metrics.j2`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 
         try:
             response = {% if not sync %}await {% endif %}self.client.request("{{ method }}", url, {%- if operation.request_body %} {%- if req_body.is_form_data or req_body.is_multipart_form_data %} data{%- else %} json{%- endif %}=json, {%- endif %} headers=headers_, params=params, content=content, auth=auth_{%- if operation.request_body and req_body.is_multipart_form_data %}, files=files{%- endif %})
         except Exception as exc:
-            {%- if metrics %}
             if self.metrics_integration:
-                if self.metrics_integration.shadow_path:
-                    self.metrics_integration.on_request_error(self.client_name, exc, "{{ method }}", "{{ path | replace('{', ':') | replace('}', '') }}")
+                if self.metrics_integration.shadow_path():
+                    metrics_path = "{{ path | replace('{', ':') | replace('}', '') }}"
                 else:
-                    self.metrics_integration.on_request_error(self.client_name, exc, "{{ method }}", f"{{ path }}")
+                    metrics_path = f"{{ path }}"
+                self.metrics_integration.on_request_error(self.client_name, exc, "{{ method }}", metrics_path)
 
-            {%- endif %}
             raise exc
         {#
             https://www.python-httpx.org/api/#response
             .elapsed - The amount of time elapsed between sending the request
             and calling close() on the corresponding response received for that request.
             total_seconds() to correctly get the total elapsed seconds.
         #}
-        {%- if metrics %}
         if self.metrics_integration:
-            if self.metrics_integration.shadow_path:
-                self.metrics_integration.on_request_success(self.client_name, response, "{{ method }}", "{{ path | replace('{', ':') | replace('}', '') }}")
+            if self.metrics_integration.shadow_path():
+                metrics_path = "{{ path | replace('{', ':') | replace('}', '') }}"
             else:
-                self.metrics_integration.on_request_success(self.client_name, response, "{{ method }}",  f"{{ path }}")
-        {%- endif %}
+                metrics_path = f"{{ path }}"
+            self.metrics_integration.on_request_success(self.client_name, response, "{{ method }}",  metrics_path)
```

### Comparing `pythogen-0.2.5/pythogen/templates/httpx.j2` & `pythogen-0.2.6/pythogen/templates/http_client/main.j2`

 * *Files 2% similar despite different names*

```diff
@@ -51,34 +51,36 @@
 
 # backward compatibility for httpx<0.18.2
 try:
     DEFAULT_AUTH = httpx.USE_CLIENT_DEFAULT
 except AttributeError:
     DEFAULT_AUTH = None
 
-{%- if metrics %}
-class MetricsIntegration(Protocol):
-    def __init__(
-        self,
-        client_response_time_histogram: Histogram | None = None,
-        client_non_http_errors_counter: Counter | None = None,
-        shadow_path: bool = True,
-    ):
-        self._client_response_time_histogram = client_response_time_histogram
-        self._client_non_http_errors_counter = client_non_http_errors_counter
-        self.shadow_path = shadow_path
 
+class MetricsIntegration(Protocol):
     def on_request_error(self, client_name: str, error: Exception, http_method: str, http_target: str) -> None:
         ...
 
     def on_request_success(self, client_name: str, response, http_method: str, http_target: str) -> None:
         ...
 
+    def shadow_path(self) -> bool:
+        ...
+
 
+{%- if metrics %}
 class DefaultMetricsIntegration:
+    def __init__(
+        self,
+        client_response_time_histogram: Histogram | None = None,
+        client_non_http_errors_counter: Counter | None = None,
+    ):
+        self._client_response_time_histogram = client_response_time_histogram
+        self._client_non_http_errors_counter = client_non_http_errors_counter
+
     def on_request_error(self, client_name: str, error: Exception, http_method: str, http_target: str) -> None:
         self._client_non_http_errors_counter.labels(
             client_name=client_name,
             http_method=http_method,
             http_target=http_target,
             exception=error.__class__.__name__,
         ).inc(1)
@@ -87,14 +89,17 @@
     def on_request_success(self, client_name: str, response, http_method: str, http_target: str) -> None:
         self._client_response_time_histogram.labels(
             client_name=client_name,
             http_method=http_method,
             http_target=http_target,
             http_status_code=response.status_code,
         ).observe(response.elapsed.total_seconds())
+
+    def shadow_path(self) -> bool:
+        return True
 {%- endif %}
 
 
 @dataclass
 class RequestBox:
     client_name: str
     method: str
@@ -268,59 +273,55 @@
         client_name: str = "{{ name | replace('Client', '') | lower }}",
         {%- if sync %}
         client: httpx.Client | None = None,
         {%- else %}
         client: httpx.AsyncClient | None = None,
         {%- endif %}
         headers: dict[str, str] | None = None,
-        {%- if metrics %}
         metrics_integration: MetricsIntegration | None = None,
-        {%- endif %}
         logs_integration: LogsIntegration | None = DefaultLogsIntegration(),
     ):
         {%- if sync %}
         self.client = client or httpx.Client(timeout=Timeout(timeout))
         {%- else %}
         self.client = client or httpx.AsyncClient(timeout=Timeout(timeout))
         {%- endif %}
         self.base_url = base_url
         self.headers = headers or {}
-        {%- if metrics %}
-        self.metrics_integration=metrics_integration
-        {%- endif %}
+        self.metrics_integration = metrics_integration
         self.logs_integration = logs_integration
         self.client_name = client_name
         {% if required_headers %}
         if set({{ required_headers }}) != set(self.headers):
             raise RequiredHeaders("Headers {{ required_headers }} is required")
         {%- endif %}
 
     {#-  get items begin  #}
     {% with items=get.items(), method='get'%}
-    {%- include 'client/httpx-method.j2' %}
+    {%- include 'method.j2' %}
     {%- endwith %}
     {#-  get items end  #}
     {#-  post items begin  #}
     {%- with items=post.items(), method='post'%}
-    {%- include 'client/httpx-method.j2' %}
+    {%- include 'method.j2' %}
     {%- endwith %}
     {#-  post items end  #}
     {#-  patch items begin  #}
     {%- with items=patch.items(), method='patch'%}
-    {%- include 'client/httpx-method.j2' %}
+    {%- include 'method.j2' %}
     {%- endwith %}
     {#-  patch items end  #}
     {#-  put items begin  #}
     {%- with items=put.items(), method='put'%}
-    {%- include 'client/httpx-method.j2' %}
+    {%- include 'method.j2' %}
     {%- endwith %}
     {#-  put items end  #}
     {#-  delete_no_body items begin  #}
     {%- with items=delete_no_body.items(), method='delete', body=False %}
-    {%- include 'client/httpx-method.j2' %}
+    {%- include 'method.j2' %}
     {%- endwith %}
     {#-  delete_no_body items end  #}
     {% if sync %}
     def close(self) -> None:
         self.client.close()
     {%- else %}
     async def close(self) -> None:
```

### Comparing `pythogen-0.2.5/PKG-INFO` & `pythogen-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.2.5
+Version: 0.2.6
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.10,<4.0
@@ -22,14 +22,15 @@
 Classifier: Typing :: Typed
 Requires-Dist: autoflake (>=2.2.0,<3.0.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: jinja2 (>=3.1.1,<4.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=12.2.0,<13.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/artsmolin/pythogen
 Description-Content-Type: text/markdown
 
 <h2 align="center">Awesome python HTTP-clients from  OpenAPI</h2>
```

