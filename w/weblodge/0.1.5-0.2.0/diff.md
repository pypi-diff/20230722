# Comparing `tmp/weblodge-0.1.5.tar.gz` & `tmp/weblodge-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblodge-0.1.5.tar", max compression
+gzip compressed data, was "weblodge-0.2.0.tar", max compression
```

## Comparing `weblodge-0.1.5.tar` & `weblodge-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0     1074 2023-07-06 14:06:29.155692 weblodge-0.1.5/LICENSE
--rw-r--r--   0        0        0      713 2023-07-11 21:51:42.521107 weblodge-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5635 2023-07-11 21:26:46.630621 weblodge-0.1.5/README.md
--rw-r--r--   0        0        0       98 2023-07-06 14:06:29.174572 weblodge-0.1.5/weblodge/__main__.py
--rw-r--r--   0        0        0      349 2023-07-06 14:06:29.174572 weblodge-0.1.5/weblodge/_azure/__init__.py
--rw-r--r--   0        0        0     3431 2023-07-06 14:06:29.175573 weblodge-0.1.5/weblodge/_azure/appservice.py
--rw-r--r--   0        0        0     2483 2023-07-09 19:00:39.100057 weblodge-0.1.5/weblodge/_azure/cli.py
--rw-r--r--   0        0        0     2209 2023-07-06 14:06:29.177571 weblodge-0.1.5/weblodge/_azure/resource_group.py
--rw-r--r--   0        0        0     1123 2023-07-06 14:06:29.177571 weblodge-0.1.5/weblodge/_azure/subscription.py
--rw-r--r--   0        0        0     4275 2023-07-09 19:00:39.101312 weblodge-0.1.5/weblodge/_azure/web_app.py
--rw-r--r--   0        0        0      147 2023-07-06 14:06:29.178571 weblodge-0.1.5/weblodge/cli/__init__.py
--rw-r--r--   0        0        0     3509 2023-07-11 20:05:23.730516 weblodge-0.1.5/weblodge/cli/main.py
--rw-r--r--   0        0        0      175 2023-07-06 14:06:29.179570 weblodge-0.1.5/weblodge/config/__init__.py
--rw-r--r--   0        0        0      877 2023-07-06 14:06:29.180572 weblodge-0.1.5/weblodge/config/item.py
--rw-r--r--   0        0        0       92 2023-07-09 19:00:39.102324 weblodge-0.1.5/weblodge/parameters/__init__.py
--rw-r--r--   0        0        0     3134 2023-07-11 18:58:24.005879 weblodge-0.1.5/weblodge/parameters/parameters.py
--rw-r--r--   0        0        0      165 2023-07-06 14:06:29.182572 weblodge-0.1.5/weblodge/state/__init__.py
--rw-r--r--   0        0        0      748 2023-07-06 14:06:29.182572 weblodge-0.1.5/weblodge/state/state.py
--rw-r--r--   0        0        0      256 2023-07-11 21:05:52.898919 weblodge-0.1.5/weblodge/web_app/__init__.py
--rw-r--r--   0        0        0     6328 2023-07-11 21:15:35.831949 weblodge-0.1.5/weblodge/web_app/build.py
--rw-r--r--   0        0        0     1320 2023-07-06 14:06:29.184570 weblodge-0.1.5/weblodge/web_app/delete.py
--rw-r--r--   0        0        0     4165 2023-07-09 19:00:39.108261 weblodge-0.1.5/weblodge/web_app/deploy.py
--rw-r--r--   0        0        0      696 2023-07-08 22:19:02.556642 weblodge-0.1.5/weblodge/web_app/logs.py
--rw-r--r--   0        0        0     1388 2023-07-11 19:24:32.536898 weblodge-0.1.5/weblodge/web_app/web_app.py
--rw-r--r--   0        0        0     7490 1970-01-01 00:00:00.000000 weblodge-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-06 14:06:29.155692 weblodge-0.2.0/LICENSE
+-rw-r--r--   0        0        0      755 2023-07-22 12:39:09.759331 weblodge-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6547 2023-07-20 17:13:36.192808 weblodge-0.2.0/README.md
+-rw-r--r--   0        0        0      106 2023-07-19 06:58:33.264146 weblodge-0.2.0/weblodge/__main__.py
+-rw-r--r--   0        0        0      241 2023-07-17 18:24:53.187041 weblodge-0.2.0/weblodge/_azure/__init__.py
+-rw-r--r--   0        0        0     2442 2023-07-22 11:51:41.892842 weblodge-0.2.0/weblodge/_azure/appservice.py
+-rw-r--r--   0        0        0     2956 2023-07-22 12:10:56.609822 weblodge-0.2.0/weblodge/_azure/cli.py
+-rw-r--r--   0        0        0      737 2023-07-18 14:34:05.043984 weblodge-0.2.0/weblodge/_azure/exceptions.py
+-rw-r--r--   0        0        0     3868 2023-07-22 07:24:17.325039 weblodge-0.2.0/weblodge/_azure/resource.py
+-rw-r--r--   0        0        0     1240 2023-07-22 11:52:03.132703 weblodge-0.2.0/weblodge/_azure/resource_group.py
+-rw-r--r--   0        0        0     3601 2023-07-22 12:03:50.990232 weblodge-0.2.0/weblodge/_azure/web_app.py
+-rw-r--r--   0        0        0      147 2023-07-06 14:06:29.178571 weblodge-0.2.0/weblodge/cli/__init__.py
+-rw-r--r--   0        0        0     1388 2023-07-16 06:28:22.045802 weblodge-0.2.0/weblodge/cli/args.py
+-rw-r--r--   0        0        0     3132 2023-07-22 12:10:28.119984 weblodge-0.2.0/weblodge/cli/main.py
+-rw-r--r--   0        0        0      175 2023-07-06 14:06:29.179570 weblodge-0.2.0/weblodge/config/__init__.py
+-rw-r--r--   0        0        0      877 2023-07-16 06:59:54.559965 weblodge-0.2.0/weblodge/config/item.py
+-rw-r--r--   0        0        0      537 2023-07-15 17:07:53.919944 weblodge-0.2.0/weblodge/parameters/__init__.py
+-rw-r--r--   0        0        0     4323 2023-07-16 14:53:20.295219 weblodge-0.2.0/weblodge/parameters/parameters.py
+-rw-r--r--   0        0        0      165 2023-07-06 14:06:29.182572 weblodge-0.2.0/weblodge/state/__init__.py
+-rw-r--r--   0        0        0      748 2023-07-06 14:06:29.182572 weblodge-0.2.0/weblodge/state/state.py
+-rw-r--r--   0        0        0       90 2023-07-15 14:26:01.276004 weblodge-0.2.0/weblodge/web_app/__init__.py
+-rw-r--r--   0        0        0     6307 2023-07-22 07:12:52.658584 weblodge-0.2.0/weblodge/web_app/build.py
+-rw-r--r--   0        0        0      794 2023-07-19 06:56:57.485772 weblodge-0.2.0/weblodge/web_app/delete.py
+-rw-r--r--   0        0        0     3760 2023-07-22 12:06:46.110134 weblodge-0.2.0/weblodge/web_app/deploy.py
+-rw-r--r--   0        0        0      463 2023-07-20 17:20:08.912029 weblodge-0.2.0/weblodge/web_app/exceptions.py
+-rw-r--r--   0        0        0     1059 2023-07-19 07:01:09.969752 weblodge-0.2.0/weblodge/web_app/logs.py
+-rw-r--r--   0        0        0     3136 2023-07-20 18:46:22.371674 weblodge-0.2.0/weblodge/web_app/web_app.py
+-rw-r--r--   0        0        0     8362 1970-01-01 00:00:00.000000 weblodge-0.2.0/PKG-INFO
```

### Comparing `weblodge-0.1.5/LICENSE` & `weblodge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.5/pyproject.toml` & `weblodge-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "weblodge"
-version = "0.1.5"
+version = "0.2.0"
 description = "A simple command line aiming to provide anyone with deployment and cloud management capabilities."
 authors = ["Vuillemot Florian <vuillemot.florian@outlook.fr>"]
 
 repository = "https://github.com/florian-vuillemot/weblodge"
 homepage = "https://github.com/florian-vuillemot/weblodge"
 
 readme = ["README.md", "LICENSE"]
 keywords = ["deployment", "azure"]
 
 [tool.poetry.scripts]
 weblodge = "weblodge.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-azure-cli = "2.50.0"
+azure-cli = ">=2.40.0"
+
+[tool.poetry.group.tests.dependencies]
 urllib3 = "^2.0.3"
 
 [tool.poetry.group.linter.dependencies]
 pylint = ">=2.17,<=3.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `weblodge-0.1.5/README.md` & `weblodge-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 - A Python [Flask](https://flask.palletsprojects.com/en/2.3.x/) application.
 - A `requirements.txt` with the application dependencies. 
 - Have an [Azure account](https://azure.microsoft.com/en-us/free).
 
 > Note: By default, **WebLodge** uses **Free** [Azure services](https://azure.microsoft.com/en-us/pricing/free-services) and lets the user specify non-free configurations.
 
 
+> Note: Today, **WebLodge** is only available for **Flask** applications.
+
+
 ## Deploying an application
 
 The simple way to deploy your local application is by running the command line `weblodge deploy --build` in your application directory.
 
 In that case, **WebLodge** will assume that your application entry point is named `app.py` and your dependencies file is `requirements.txt`.
 
 Behind the scene, **WebLodge** *build* then *deploy* your application.
 
+![CLI: weblodge deploy --build](./images/deploy.gif)
+
 ## Application structure
 
 **WebLodge** is sensible to the application structure. Applications must follow the pre-defined pattern or specify custom values.
 
 Here is an example of the standard pattern deployable without configuration:
 ```
 $ cat app.py  # The application filename entry point.
@@ -49,30 +54,30 @@
     return "<p>Hello, World!</p>"
 ```
 To be able to deploy the application, you must first *build* it and specify:
 - The entry point file: `main.py`.
 - The **Flask** application: `my_app`.
 ```
 # Build the application.
-weblodge build --entry-point main.py --app my_app
+weblodge build --entry-point main.py --flask-app my_app
 # Deploy the application.
 weblodge deploy
 ```
 
 ## Build
 
 The *build* operation collects and prepares the application for deployment on a specific platform.
 
 The *build* operation can handle the following options:
 | Option name | Description | Default value |
 |-|-|-|
 | src | Folder containing application sources. | `.` |
 | dist | Folder containing the application built. | `dist` |
 | entry-point | The application file to be executed with `python`. | `app.py` |
-| app | The Flask application object in the `entry-point` file. | `app` |
+| flask-app | The Flask application object in the `entry-point` file. | `app` |
 | requirements | The **requirements.txt** file path of the application. Ignores if a `requirements.txt` file is located at the root of the application. | `requirements.txt` |
 
 > Note: Here, the platform is implicitly [Azure App Service](https://azure.microsoft.com/en-us/products/app-service/web).
 
 Example:
 ```
 # Build the local application.
@@ -84,36 +89,40 @@
 
 ## Deploy
 
 The *deploy* operation creates the necessary infrastructure and uploads the build package - i.e. your code - on the infrastructure.
 
 | Option name | Description | Default value |
 |-|-|-|
-| app-name | The unique name of the application on the Internet. It will be included in the application URL. | `<randomly generated>` |
+| subdomain | The subdomain of the application on the Internet: `<subdomain>.azurewebsites.net`. Randomly generated if not provided. | `<randomly generated>` |
 | sku | The application [computational power](https://azure.microsoft.com/en-us/pricing/details/app-service/linux/). | `F1` |
 | location | The physical application location. | `northeurope` |
 | environment | The environment of your application. | `development` |
 | dist | Folder containing the application built. | `dist` |
 
 Example:
 ```
 # Deploy the local application.
 weblodge deploy
 
-# Deploy the local application with a custom name.
-weblodge deploy --app-name myapp
+# Deploy the local application with a custom subdomain.
+weblodge deploy --subdomain myapp
 ```
 
+> **ℹ️ Note**
+>
+> WebLodge considers the `subdomain` as the application name.
+
 ## Delete
 
 The *delete* operation deletes the infrastructure deployed but keeps the build.
 
 | Option name | Description | Default value |
 |-|-|-|
-| app-name | The name of the application to be deleted. | `<my-app>` |
+| subdomain | The subdomain of the application to be deleted. | `<my-subdomain>` |
 | yes | Do not prompt a validation message before deletion. | `false` |
 
 
 Example:
 ```
 # Delete the application previously deployed.
 weblodge delete
@@ -122,22 +131,30 @@
 
 ## Logs
 
 The *logs* operation streams your application logs. Because it is a stream, logs are truncated.
 
 | Option name | Description | Default value |
 |-|-|-|
-| app-name | The name of the application. | `<my-app>` |
+| subdomain | The subdomain of the application. | `<my-subdomain>` |
 
 Example:
 ```
 # Print logs of the application previously created.
 weblodge logs
 ```
 
+*** Log buffering ***
+
+Logs can be buffered and never appear in the stream.
+
+If you use the [print](https://docs.python.org/3/library/functions.html#print) method, you can force logs to be written to the console by sending them to the [stderr](https://docs.python.org/3/library/sys.html#sys.stderr) output or by using the `flush` option.
+
+If you use the [logging](https://docs.python.org/3/library/logging.html) module, only logs starting at the `WARNING` level will be displayed by default. Otherwise, update the [logging level](https://docs.python.org/3/library/logging.html#logging.Logger.setLevel) module to the required level.
+
 ## Configuration file: `.weblodge.json`
 
 At the end of a deployment, **WebLodge** creates a file named `.weblodge.json` by default.
 This file contains the previous configuration, enabling **WebLodge** to update your application with the same parameters. This file can be version-controlled and used in your Continuous Deployment.
 
 You can change the name of this file with the `--config-filename` option.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `weblodge-0.1.5/weblodge/_azure/appservice.py` & `weblodge-0.2.0/weblodge/_azure/appservice.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,89 @@
 """
 Azure AppService Plan abstraction.
 
 Allow to CRUD on Azure AppService Plan.
 """
-from typing import Dict, List
-from dataclasses import dataclass
+from typing import Dict
+
+from weblodge._azure.cli import Cli
 
 from .cli import Cli
-from .resource_group import ResourceGroupModel, ResourceGroup
+from .resource import Resource
+from .resource_group import ResourceGroup
 
 
-@dataclass(frozen=True)
-class AppServiceModel:
+class AppService(Resource):
     """
     Azure AppService Plan representation.
     """
-    id: str  # pylint: disable=invalid-name
-    name: str
-    number_of_sites: int
-    sku: str
-    location: str
-    resource_group: ResourceGroupModel
-    tags: Dict[str, str]
-
+    _cli_prefix = 'appservice plan'
 
-class AppService:
-    """
-    Helper class to manage Azure AppServices Plan.
-    """
-    def __init__(self, cli: Cli()) -> None:
-        self._cli = cli
-        self._resources = []
-
-    def list(self, force_reload=False) -> List[AppServiceModel]:
-        """
-        List all AppServices Plan.
-        """
-        if force_reload:
-            self._resources.clear()
-
-        if not self._resources:
-            appservices = self._cli.invoke('appservice plan list')
-            for asp in appservices:
-                self._resources.append(
-                    AppServiceModel(
-                        id=asp['id'],
-                        name=asp['name'],
-                        number_of_sites=int(asp['numberOfSites']),
-                        sku=asp['sku']['name'],
-                        resource_group=ResourceGroup(self._cli).get(asp['resourceGroup']),
-                        location=asp['location'],
-                        tags=asp['tags']
-                    )
-                )
-
-        return self._resources
-
-    def get(
+    # pylint: disable=too-many-arguments
+    def __init__(
             self,
-            name: str = None,
-            resource_group: ResourceGroupModel = None,
-            id_: str = None,
-            force_reload=True
-        ) -> AppServiceModel:
-        """
-        Return an appservice by its name or its id.
-        If resource_group is provided, it will used with the name based search.
-        """
-        for asp in self.list(force_reload=force_reload):
-            if asp.id == id_:
-                return asp
-            if asp.name == name:
-                if resource_group is None or asp.resource_group.name == resource_group.name:
-                    return asp
+            name: str,
+            resource_group: ResourceGroup,
+            cli: Cli = Cli(),
+            from_az: Dict = None
+        ) -> None:
+        super().__init__(name, cli, from_az)
+        self.resource_group = resource_group
+
+    @property
+    def id_(self) -> str:
+        """
+        Return the AppService Plan ID.
+        """
+        return self._from_az['id']
 
-        raise Exception(f"AppService '{name}' not found.")  # pylint: disable=broad-exception-raised
+    @property
+    def always_on_supported(self) -> bool:
+        """
+        Return True if the AppService Plan support AlwaysOn.
+        """
+        return self._from_az['sku']['name'] != 'F1'
 
-    def delete(self, asp: AppServiceModel) -> List[AppServiceModel]:
+    def create(self, sku: str) -> 'AppService':
         """
-        Delete an AppService Plan.
+        Create a Linux AppService Plan with Python.
         """
-        asp_name = asp.name
-        rg_name = asp.resource_group.name
+        tags = self.resource_group.tags
+        rg_name = self.resource_group.name
+        location = self.resource_group.location
 
         self._cli.invoke(
-            f'appservice plan delete --name {asp_name} --resource-group {rg_name} --yes',
-            to_json=False
+            f'{self._cli_prefix} create --name {self.name} --sku {sku} --resource-group {rg_name} --location {location} --is-linux',  # pylint: disable=line-too-long
+            tags=tags
         )
+        return self
 
-        return self.list(force_reload=True)
-
-    # pylint: disable=too-many-arguments
-    def create(
-            self,
-            name: str,
-            sku: str,
-            resource_group: ResourceGroupModel,
-            location: str = None,
-            tags: Dict[str, str] = None
-        ) -> AppServiceModel:
+    @classmethod
+    def from_id(cls, id_: str, cli: Cli) -> 'AppService':
         """
-        Create a Linux AppService Plan.
+        Return an App Service from an Azure App Service Plan ID.
         """
-        tags = tags or resource_group.tags
-        location = location or resource_group.location
+        from_az = cli.invoke(f'{cls._cli_prefix} show --ids {id_}')
+        return cls.from_az(from_az['name'], cli, from_az)
 
-        self._cli.invoke(
-            f'appservice plan create --name {name} --sku {sku} --resource-group {resource_group.name} --location {location} --is-linux',  # pylint: disable=line-too-long
-            tags=tags
+    @classmethod
+    def from_az(cls, name: str, cli: Cli, from_az: Dict):
+        """
+        Return an App Service from Azure AppService result.
+        """
+        return cls(
+            name=name,
+            resource_group=ResourceGroup(from_az['resourceGroup'], cli),
+            cli=cli,
+            from_az=from_az
         )
 
-        return self.get(name=name, resource_group=resource_group, force_reload=True)
+    def _load(self):
+        """
+        Load the AppService Plan from Azure.
+        """
+        self._from_az.update(
+            self._cli.invoke(
+                f'{self._cli_prefix} show --name {self.name} --resource-group {self.resource_group.name}'
+            )
+        )
+        return self
```

### Comparing `weblodge-0.1.5/weblodge/_azure/cli.py` & `weblodge-0.2.0/weblodge/_azure/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Interface to the Azure CLI.
 """
 import json
-import time
-from io import StringIO
 import logging
+from io import StringIO
+import time
 from typing import Dict, Union
 
 from azure.cli.core import get_default_cli
 
+from .exceptions import CLIException
+
 
 logger = logging.getLogger('weblodge')
 
 
 class Cli:
     """
     Azure CLI wrapper.
@@ -21,55 +23,64 @@
         self._first_invoke = True
         self.cli = get_default_cli()
 
     def invoke(
             self,
             command: str,
             to_json=True,
-            tags: Dict[str, str] = None
+            tags: Dict[str, str] = None,
+            log_outputs: bool = False
         ) -> Union[str, Dict]:
         """
         Execute an Azure CLI command and return its output.
         If `to_json` is True, the output is converted to a JSON object.
+        If `log_outputs` is True, the output is not returned but logged instead.
         """
         if self._first_invoke:
             self._first_invoke = False
 
             try:
-                return self._invoke(command, to_json=to_json, tags=tags)
-            except Exception:  # pylint: disable=broad-exception-caught
-                # Command may fail if the user is not logged in.
-                logger.info('Previous command failed, try login to Azure CLI...')
-                self._invoke('login', False, None)
-                logger.info('Login successful, retry previous command...')
-
-        try:
-            return self._invoke(command, to_json=to_json, tags=tags)
-        except Exception:  # pylint: disable=broad-exception-caught
-            logger.info(
-                'The previous command failed.\n'
-                'This may be due to simultaneous asynchronous operations.\n'
-                'Will try again in 30 seconds...'
-            )
-            time.sleep(30)
-            return self._invoke(command, to_json=to_json, tags=tags)
+                return self._invoke(command, to_json=to_json, tags=tags, log_outputs=log_outputs)
+            except Exception as exception:  # pylint: disable=broad-exception-caught
+                if 'az login' in str(exception):
+                    logger.info('Authentication is needed...')
+                    self._invoke('login', False, None, log_outputs=log_outputs)
+                    logger.info('Login successful, retry previous command...')
 
-    def _invoke(self, command: str, to_json: bool, tags) -> Union[str, Dict]:
+        return self._invoke(command, to_json=to_json, tags=tags, log_outputs=log_outputs)
+
+    def _invoke(self, command: str, to_json: bool, tags: Dict[str, str], log_outputs: bool) -> Union[str, Dict]:
         # Convert the string command to a array of arguments.
         cmd = command.split()
-        # Create a file-like object to store the output.
-        out_fd = StringIO()
+        # Redirect the output to a file if the log output is not asked.
+        out_fd = None if log_outputs else StringIO()
 
         if tags:
             cmd.append('--tags')
             cmd.extend(f'{k}={v}' for k, v in tags.items())
 
-        # Execute the Azure CLI command and store the return code.
-        if self.cli.invoke(cmd, out_file=out_fd):
-            raise Exception(f"Error during execution of the command '{command}'.")  # pylint: disable=broad-exception-raised
+        exception = None
+        for _ in range(10):
+            try:
+                # Execute the Azure CLI command.
+                if self.cli.invoke(cmd, out_file=out_fd):
+                    exception = CLIException(f"Error during execution of the command '{command}'.")  # pylint: disable=broad-exception-raised
+                else:
+                    exception = None
+                    break
+            except (SystemExit, Exception) as exception: # pylint: disable=broad-exception-caught
+                exception = CLIException(f"Error during execution of the command '{command}'.\nTraceback: {exception}") # pylint: disable=raise-missing-from
+            time.sleep(30)
+
+        if exception:
+            raise exception
+
+        # No output to return.
+        if log_outputs:
+            return None
 
         # Retrieve the output.
         output = out_fd.getvalue()
         out_fd.close()
 
         # Convert the output to a JSON object if needed.
         if to_json:
```

### Comparing `weblodge-0.1.5/weblodge/config/item.py` & `weblodge-0.2.0/weblodge/config/item.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.5/weblodge/state/state.py` & `weblodge-0.2.0/weblodge/state/state.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.5/weblodge/web_app/build.py` & `weblodge-0.2.0/weblodge/web_app/build.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,30 +7,19 @@
 - A generated Kudu deployment configuration file.
 - A generated startup file.
 
 This package is ready to be deployed on an Azure Web App.
 """
 import os
 from pathlib import Path
-from typing import List
 import zipfile
 
 from weblodge.config import Item as ConfigItem
 
-
-class BuildException(Exception):
-    """
-    Build exception.
-    """
-
-
-class RequirementsFileNotFound(BuildException):
-    """
-    The requirements file was not found.
-    """
+from .exceptions import RequirementsFileNotFound, EntryPointFileNotFound, FlaskAppNotFound
 
 
 class BuildConfig:
     """
     Build configuration.
 
     User-customizable fields are found in the `config` property. All are optional from the user's
@@ -42,103 +31,105 @@
     kudu_config: str = '.deployment'
     # Startup file.
     # Set in the deployment config too.
     startup_file: str = 'weblodge.startup'
     # Kudu needs a requirements file at the root of the zip.
     kudu_requirements_path = 'requirements.txt'
 
+    # Configurable items of the build.
+    items = [
+        ConfigItem(
+            name='src',
+            description='Application folder.',
+            default='.'
+        ),
+        ConfigItem(
+            name='dist',
+            description='Build destination.',
+            default='dist'
+        ),
+        ConfigItem(
+            name='entry_point',
+            description='Application entry point.',
+            default='app.py'
+        ),
+        ConfigItem(
+            name='flask_app',
+            description='The Flask application object.',
+            default='app'
+        ),
+        ConfigItem(
+            name='requirements',
+            description='Requirements.txt file path.',
+            default='requirements.txt'
+        )
+    ]
+
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         src: str,
         dist: str,
         entry_point: str,
-        app: str,
+        flask_app: str,
         requirements: str,
         *_args,
         **_kwargs
     ):
         # Source directory to zip.
         self.src = src
         # Destination directory to the zip file `name`.
         self.dist = dist
         # Application entrypoint.
         self.entry_point = entry_point
         # Flask application object.
-        self.app = app
+        self.flask_app = flask_app
         # User requirements file.
         self.requirements = requirements
 
     @property
     def package_path(self) -> str:
         """
         Return the package path.
         """
         return os.path.join(self.dist, self.package)
 
-    @classmethod
-    @property
-    def items(cls) -> List[ConfigItem]:
-        """
-        Items that can be configured.
-        """
-        return [
-            ConfigItem(
-                name='src',
-                description='Application folder.',
-                default='.'
-            ),
-            ConfigItem(
-                name='dist',
-                description='Build destination.',
-                default='dist'
-            ),
-            ConfigItem(
-                name='entry_point',
-                description='Application entry point.',
-                default='app.py'
-            ),
-            ConfigItem(
-                name='app',
-                description='Flask Application object.',
-                default='app'
-            ),
-            ConfigItem(
-                name='requirements',
-                description='Requirements.txt file path.',
-                default='requirements.txt'
-            )
-        ]
-
 
 def build(config: BuildConfig) -> None:
     """
     Build an application to a deployable format.
     """
     # Create the destination directory.
     os.makedirs(config.dist, exist_ok=True)
 
     # Zip all required files together.
     with zipfile.ZipFile(config.package_path, 'w', zipfile.ZIP_DEFLATED) as zipf:
-        requirements_file_included = _zip_user_application(config, zipf)
+        _user_application(config, zipf)
+        _user_requirements(config, zipf)
         _deployment_config(config, zipf)
         _startup_file(config, zipf)
 
-        # Add the requirements file if it was not included in the user application folder.
-        if not requirements_file_included:
-            _requirements(config, zipf)
-
 
-def _zip_user_application(config: BuildConfig, zipf: zipfile.ZipFile) -> bool:
+def _user_application(config: BuildConfig, zipf: zipfile.ZipFile):
     """
     Create the zip folder.
-
-    Return True if the requirements file was included at the root of the application folder.
     """
-    requirements_file_included = False
+    # The requirements file name.
+    # It will be added to the zip folder in a dedicated function.
+    # If it is added twice, the ZIP library prints an error.
+    requirements_filename = Path(config.requirements).name
+
+    # Ensure the entry point exists.
+    entry_point = Path(config.src) / config.entry_point
+    if not entry_point.exists():
+        raise EntryPointFileNotFound()
+
+    # Ensure the flask app is in the entry point file.
+    if config.flask_app not in entry_point.read_text():
+        raise FlaskAppNotFound()
 
     for root, _, files in os.walk(config.src):
         root = Path(root)
         # Skip hidden files and directories.
         if root.name.startswith('.'):
             continue
         # Skip bytecode files.
@@ -149,32 +140,36 @@
         if root.name.startswith(Path(config.dist).name):
             continue
         # Zip the files.
         for file in files:
             file_path = root / file
             relative_to = os.path.relpath(file_path, config.src)
 
-            zipf.write(file_path, relative_to)
-
-            if not requirements_file_included:
-                # If the requirements file is not already included at the root of the application
-                # folder, check if the current file is that one.
-                requirements_file_included = Path(relative_to) == Path(config.kudu_requirements_path)
+            # Skip the requirements file.
+            if relative_to == requirements_filename:
+                continue
 
-    return requirements_file_included
+            zipf.write(file_path, relative_to)
 
 
-def _requirements(config: BuildConfig, zipf: zipfile.ZipFile):
+def _user_requirements(config: BuildConfig, zipf: zipfile.ZipFile):
     """
     Add the requirements file to the zip folder from the user folder.
+    The file can be in the local folder or in the `src` folder.
     """
-    if not os.path.exists(config.requirements):
-        raise RequirementsFileNotFound()
+    if os.path.exists(config.requirements):
+        zipf.write(config.requirements, config.kudu_requirements_path)
+        return
+
+    requirements_in_src = Path(config.src) / config.requirements
+    if requirements_in_src.exists():
+        zipf.write(requirements_in_src, config.kudu_requirements_path)
+        return
 
-    zipf.write(config.requirements, config.kudu_requirements_path)
+    raise RequirementsFileNotFound()
 
 
 def _deployment_config(config: BuildConfig, zipf: zipfile.ZipFile):
     """
     Add the deployment config file to the zip folder.
     """
     # Kudu deployment config file.
@@ -194,15 +189,15 @@
     # Remove potentional .py extension.
     entrypoint = config.entry_point
     if entrypoint.endswith('.py'):
         entrypoint = entrypoint[:-3]
 
     # Add the application object if it's not already there.
     if ':' not in entrypoint:
-        entrypoint = f'{entrypoint}:{config.app}'
+        entrypoint = f'{entrypoint}:{config.flask_app}'
 
     # Default application configuration update with the user and entrypoint.
     # https://learn.microsoft.com/en-us/azure/developer/python/configure-python-web-app-on-app-service
     startup_file_content = f'gunicorn --bind=0.0.0.0 --timeout 600 {entrypoint}'
 
     # Add the startup file to the zip folder.
     zipf.writestr(config.startup_file, startup_file_content)
```

### Comparing `weblodge-0.1.5/weblodge/web_app/deploy.py` & `weblodge-0.2.0/weblodge/web_app/deploy.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,121 +9,109 @@
 All that infrastructure is created in the same Azure region and in the same Azure
 Resource Group.
 """
 import os
 import random
 import string
 import logging
-from typing import List, Optional
-from dataclasses import dataclass, field
-
-from urllib3 import Retry, request
 
 from weblodge.config import Item as ConfigItem
-from weblodge._azure import Cli, ResourceGroup, AppService, WebApp
+from weblodge._azure import ResourceGroup, AppService, WebApp as AzureWebApp
 
 
 logger = logging.getLogger('weblodge')
 
 
-@dataclass
-class Deploy:
+class DeploymentConfig:
     """
-    Facade to the deployment process.
+    Deployment configuration.
 
-    Create the infrastructure that will host the application.
+    Configuration of the infrastructure that will host the application.
     If not provide, a random name will be generated to allow user to deploy an application
     without providing any input.
     """
-    # Application name.
-    # This name must be unique across all of Azure WebApplication.
-    # It will be used as the URL of the application and for created Azure resources.
-    app_name: str = ''.join(random.choice(string.ascii_lowercase) for _ in range(20))
-    # Application SKU (https://azure.microsoft.com/en-us/pricing/details/app-service/linux/).
-    sku: str = 'F1'
-    # Application location.
-    location: str = 'northeurope'
-    # Application environment.
-    environment: str = 'development'
-    # Dist directory containing the application zipped.
-    dist: str = 'dist'
-
-    # Infrastructure tags.
-    tags: dict = field(default_factory=dict)
-
-    @classmethod
-    @property
-    def config(cls) -> List[ConfigItem]:
-        """
-        Configure the deployment.
-        """
-        return [
-            ConfigItem(
-                name='app_name',
-                description='Unique name of the application within Azure. If not provide, a random name is used.',  # pylint: disable=line-too-long
-                default=cls.app_name
-            ),
-            ConfigItem(
-                name='sku',
-                description='The application computational power (https://azure.microsoft.com/en-us/pricing/details/app-service/linux/).',  # pylint: disable=line-too-long
-                default=cls.sku
-            ),
-            ConfigItem(
-                name='location',
-                description='The physical application location.',
-                default=cls.location
-            ),
-            ConfigItem(
-                name='environment',
-                description='The environment of your application.',
-                default=cls.environment
-            ),
-            ConfigItem(
-                name='dist',
-                description='Folder containing the application zipped.',
-                default=cls.dist
-            ),
-        ]
-
-    def deploy(self, package_name: str='azwebapp.zip') -> Optional[str]:
-        """
-        Deploy the application to Azure and return its URL.
-        """
-        default_name = f'{self.app_name}-{self.environment}-{self.location}'
-
-        cli = Cli()
-        web_app_cls = WebApp(cli)
-
-        logger.info('The infrastructure is being created or updated...')
-        web_app = web_app_cls.create(
-            self.app_name,
-            AppService(cli).create(
-                f'asp-{default_name}',
-                self.sku,
-                ResourceGroup(cli).create(
-                    f'rg-{default_name}',
-                    self.location,
-                    tags=self.tags
-                )
-            )
-        )
-        logger.info('The infrastructure has been created or updated.')
-
-        logger.info('Uploading the application...')
-        web_app_cls.deploy(web_app, os.path.join(self.dist, package_name))
-        logger.info('The application has been uploaded.')
-
-        return web_app.host_names[0]
-
-    def ping(self, web_app: WebApp) -> bool:
-        """
-        Ping the application to warm it up.
-        Return True if the application is up and running.
-        """
-        try:
-            return request(
-                "GET",
-                web_app.host_names[0],
-                retries=Retry(total=10, backoff_factor=5)
-            ).status < 400
-        except:  # pylint: disable=bare-except
-            return False
+    # Zip file that contains the user application code.
+    package: str = 'azwebapp.zip'
+
+    # Configurable items of the deployment.
+    items = [
+        ConfigItem(
+            name='subdomain',
+            description='Unique subdomain of the application within Azure. If not provide, a random subdomain is used.',  # pylint: disable=line-too-long
+            default=''.join(random.choice(string.ascii_lowercase) for _ in range(20))
+        ),
+        ConfigItem(
+            name='sku',
+            description='The application computational power (https://azure.microsoft.com/en-us/pricing/details/app-service/linux/).',  # pylint: disable=line-too-long
+            default='F1'
+        ),
+        ConfigItem(
+            name='location',
+            description='The physical application location.',
+            default='northeurope'
+        ),
+        ConfigItem(
+            name='environment',
+            description='The environment of your application.',
+            default='production'
+        ),
+        ConfigItem(
+            name='dist',
+            description='Folder containing the application zipped.',
+            default='dist'
+        ),
+    ]
+
+    # pylint: disable=too-many-arguments
+    def __init__(
+            self,
+            subdomain,
+            sku,
+            location,
+            environment,
+            dist,
+            *_args,
+            **_kwargs
+        ):
+        # Application subdomain.
+        # This name must be unique across all of Azure WebApplication.
+        # It will be used as the URL of the application and for created Azure resources.
+        self.subdomain = subdomain
+        # Application SKU (https://azure.microsoft.com/en-us/pricing/details/app-service/linux/).
+        self.sku = sku
+        # Application location.
+        self.location = location
+        # Application environment.
+        self.environment = environment
+        # Dist directory containing the application zipped.
+        self.dist = dist
+
+        # Infrastructure tags.
+        self.tags = {
+            'environment': self.environment
+        }
+
+
+def deploy(config: DeploymentConfig) -> AzureWebApp:
+    """
+    Deploy the application to Azure and return its URL.
+    """
+    resource_group = ResourceGroup(config.subdomain)
+    asp_service = AppService(config.subdomain, resource_group)
+    web_app = AzureWebApp(config.subdomain, resource_group, asp_service)
+
+    if not web_app.exists():
+        # Test web app name of
+        logger.info('The infrastructure is being created...')
+        if not asp_service.exists():
+            # Test asp sku
+            if not resource_group.exists():
+                resource_group.create(location=config.location, tags=config.tags)
+            asp_service.create(config.sku)
+        web_app.create()
+        logger.info('The infrastructure is created.')
+
+    logger.info('Uploading the application...')
+    web_app.deploy(os.path.join(config.dist, config.package))
+    logger.info('The application has been uploaded.')
+
+    return web_app
```

### Comparing `weblodge-0.1.5/PKG-INFO` & `weblodge-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: weblodge
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple command line aiming to provide anyone with deployment and cloud management capabilities.
 Home-page: https://github.com/florian-vuillemot/weblodge
 Keywords: deployment,azure
 Author: Vuillemot Florian
 Author-email: vuillemot.florian@outlook.fr
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: azure-cli (==2.50.0)
-Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
+Requires-Dist: azure-cli (>=2.40.0)
 Project-URL: Repository, https://github.com/florian-vuillemot/weblodge
 Description-Content-Type: text/markdown
 
 # WebLodge
 
 **WebLodge** is a command line aiming to provide anyone with deployment and cloud management capabilities.
 
@@ -27,22 +26,27 @@
 - A Python [Flask](https://flask.palletsprojects.com/en/2.3.x/) application.
 - A `requirements.txt` with the application dependencies. 
 - Have an [Azure account](https://azure.microsoft.com/en-us/free).
 
 > Note: By default, **WebLodge** uses **Free** [Azure services](https://azure.microsoft.com/en-us/pricing/free-services) and lets the user specify non-free configurations.
 
 
+> Note: Today, **WebLodge** is only available for **Flask** applications.
+
+
 ## Deploying an application
 
 The simple way to deploy your local application is by running the command line `weblodge deploy --build` in your application directory.
 
 In that case, **WebLodge** will assume that your application entry point is named `app.py` and your dependencies file is `requirements.txt`.
 
 Behind the scene, **WebLodge** *build* then *deploy* your application.
 
+![CLI: weblodge deploy --build](./images/deploy.gif)
+
 ## Application structure
 
 **WebLodge** is sensible to the application structure. Applications must follow the pre-defined pattern or specify custom values.
 
 Here is an example of the standard pattern deployable without configuration:
 ```
 $ cat app.py  # The application filename entry point.
@@ -68,30 +72,30 @@
     return "<p>Hello, World!</p>"
 ```
 To be able to deploy the application, you must first *build* it and specify:
 - The entry point file: `main.py`.
 - The **Flask** application: `my_app`.
 ```
 # Build the application.
-weblodge build --entry-point main.py --app my_app
+weblodge build --entry-point main.py --flask-app my_app
 # Deploy the application.
 weblodge deploy
 ```
 
 ## Build
 
 The *build* operation collects and prepares the application for deployment on a specific platform.
 
 The *build* operation can handle the following options:
 | Option name | Description | Default value |
 |-|-|-|
 | src | Folder containing application sources. | `.` |
 | dist | Folder containing the application built. | `dist` |
 | entry-point | The application file to be executed with `python`. | `app.py` |
-| app | The Flask application object in the `entry-point` file. | `app` |
+| flask-app | The Flask application object in the `entry-point` file. | `app` |
 | requirements | The **requirements.txt** file path of the application. Ignores if a `requirements.txt` file is located at the root of the application. | `requirements.txt` |
 
 > Note: Here, the platform is implicitly [Azure App Service](https://azure.microsoft.com/en-us/products/app-service/web).
 
 Example:
 ```
 # Build the local application.
@@ -103,36 +107,40 @@
 
 ## Deploy
 
 The *deploy* operation creates the necessary infrastructure and uploads the build package - i.e. your code - on the infrastructure.
 
 | Option name | Description | Default value |
 |-|-|-|
-| app-name | The unique name of the application on the Internet. It will be included in the application URL. | `<randomly generated>` |
+| subdomain | The subdomain of the application on the Internet: `<subdomain>.azurewebsites.net`. Randomly generated if not provided. | `<randomly generated>` |
 | sku | The application [computational power](https://azure.microsoft.com/en-us/pricing/details/app-service/linux/). | `F1` |
 | location | The physical application location. | `northeurope` |
 | environment | The environment of your application. | `development` |
 | dist | Folder containing the application built. | `dist` |
 
 Example:
 ```
 # Deploy the local application.
 weblodge deploy
 
-# Deploy the local application with a custom name.
-weblodge deploy --app-name myapp
+# Deploy the local application with a custom subdomain.
+weblodge deploy --subdomain myapp
 ```
 
+> **ℹ️ Note**
+>
+> WebLodge considers the `subdomain` as the application name.
+
 ## Delete
 
 The *delete* operation deletes the infrastructure deployed but keeps the build.
 
 | Option name | Description | Default value |
 |-|-|-|
-| app-name | The name of the application to be deleted. | `<my-app>` |
+| subdomain | The subdomain of the application to be deleted. | `<my-subdomain>` |
 | yes | Do not prompt a validation message before deletion. | `false` |
 
 
 Example:
 ```
 # Delete the application previously deployed.
 weblodge delete
@@ -141,22 +149,30 @@
 
 ## Logs
 
 The *logs* operation streams your application logs. Because it is a stream, logs are truncated.
 
 | Option name | Description | Default value |
 |-|-|-|
-| app-name | The name of the application. | `<my-app>` |
+| subdomain | The subdomain of the application. | `<my-subdomain>` |
 
 Example:
 ```
 # Print logs of the application previously created.
 weblodge logs
 ```
 
+*** Log buffering ***
+
+Logs can be buffered and never appear in the stream.
+
+If you use the [print](https://docs.python.org/3/library/functions.html#print) method, you can force logs to be written to the console by sending them to the [stderr](https://docs.python.org/3/library/sys.html#sys.stderr) output or by using the `flush` option.
+
+If you use the [logging](https://docs.python.org/3/library/logging.html) module, only logs starting at the `WARNING` level will be displayed by default. Otherwise, update the [logging level](https://docs.python.org/3/library/logging.html#logging.Logger.setLevel) module to the required level.
+
 ## Configuration file: `.weblodge.json`
 
 At the end of a deployment, **WebLodge** creates a file named `.weblodge.json` by default.
 This file contains the previous configuration, enabling **WebLodge** to update your application with the same parameters. This file can be version-controlled and used in your Continuous Deployment.
 
 You can change the name of this file with the `--config-filename` option.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

