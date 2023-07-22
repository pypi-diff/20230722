# Comparing `tmp/kubernetes_square-1.3.3.tar.gz` & `tmp/kubernetes_square-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernetes_square-1.3.3.tar", max compression
+gzip compressed data, was "kubernetes_square-1.4.0.tar", max compression
```

## Comparing `kubernetes_square-1.3.3.tar` & `kubernetes_square-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes_square-1.3.3/LICENSE
--rw-r--r--   0        0        0      756 2023-07-15 03:25:26.962133 kubernetes_square-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     3531 2021-09-06 17:16:58.000000 kubernetes_square-1.3.3/resources/defaultconfig.yaml
--rw-r--r--   0        0        0     1382 2023-07-15 03:25:26.962133 kubernetes_square-1.3.3/square/__init__.py
--rw-r--r--   0        0        0      203 2023-05-06 04:43:58.328074 kubernetes_square-1.3.3/square/__main__.py
--rw-r--r--   0        0        0     5095 2023-03-16 06:14:23.918379 kubernetes_square-1.3.3/square/cfgfile.py
--rw-r--r--   0        0        0     1851 2021-09-06 17:16:58.000000 kubernetes_square-1.3.3/square/dotdict.py
--rw-r--r--   0        0        0     6887 2023-07-15 02:12:53.911779 kubernetes_square-1.3.3/square/dtypes.py
--rw-r--r--   0        0        0    33744 2023-07-15 03:28:13.512977 kubernetes_square-1.3.3/square/k8s.py
--rw-r--r--   0        0        0    14924 2023-03-16 06:14:23.918379 kubernetes_square-1.3.3/square/main.py
--rw-r--r--   0        0        0    39403 2023-03-16 06:14:23.918379 kubernetes_square-1.3.3/square/manio.py
--rw-r--r--   0        0        0    29840 2023-03-16 06:14:23.918379 kubernetes_square-1.3.3/square/square.py
--rw-r--r--   0        0        0      536 1970-01-01 00:00:00.000000 kubernetes_square-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes_square-1.4.0/LICENSE
+-rw-r--r--   0        0        0      761 2023-07-22 06:51:23.778235 kubernetes_square-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3531 2023-07-22 06:18:28.743886 kubernetes_square-1.4.0/resources/defaultconfig.yaml
+-rw-r--r--   0        0        0     1382 2023-07-22 06:51:23.778235 kubernetes_square-1.4.0/square/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-06 04:43:58.328074 kubernetes_square-1.4.0/square/__main__.py
+-rw-r--r--   0        0        0     4897 2023-07-22 06:18:28.711887 kubernetes_square-1.4.0/square/cfgfile.py
+-rw-r--r--   0        0        0     2452 2023-07-22 06:08:22.385613 kubernetes_square-1.4.0/square/dotdict.py
+-rw-r--r--   0        0        0     8551 2023-07-22 06:18:28.731886 kubernetes_square-1.4.0/square/dtypes.py
+-rw-r--r--   0        0        0    33705 2023-07-22 06:18:28.683888 kubernetes_square-1.4.0/square/k8s.py
+-rw-r--r--   0        0        0    14837 2023-07-22 06:18:28.743886 kubernetes_square-1.4.0/square/main.py
+-rw-r--r--   0        0        0    39290 2023-07-22 06:18:28.747886 kubernetes_square-1.4.0/square/manio.py
+-rw-r--r--   0        0        0    29846 2023-07-22 06:18:28.735886 kubernetes_square-1.4.0/square/square.py
+-rw-r--r--   0        0        0     2068 2023-07-22 06:18:28.739886 kubernetes_square-1.4.0/square/yaml_io.py
+-rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 kubernetes_square-1.4.0/PKG-INFO
```

### Comparing `kubernetes_square-1.3.3/LICENSE` & `kubernetes_square-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernetes_square-1.3.3/pyproject.toml` & `kubernetes_square-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kubernetes-square"
-version = "1.3.3"
+version = "1.4.0"
 description = ""
 authors = ["Oliver Nagy <olitheolix@gmail.com>"]
 packages = [
     { include = "square" },
 ]
 include = ["resources/defaultconfig.yaml"]
 
@@ -12,18 +12,18 @@
 [tool.poetry.dependencies]
 backoff = "*"
 colorama = "*"
 colorlog = "*"
 google = "*"
 google-api-python-client = "*"
 jsonpatch = "*"
-pydantic = ">=1.8"
+pydantic = ">=2.0"
 python = ">=3.10"
 pyyaml = "*"
-requests = "*"
+requests = ">=2.31"
 
 [tool.poetry.dev-dependencies]
 bumpversion = "*"
 flake8 = "*"
 flake8-isort = "*"
 ipython = ">=8.10"
 isort = "*"
```

### Comparing `kubernetes_square-1.3.3/resources/defaultconfig.yaml` & `kubernetes_square-1.4.0/resources/defaultconfig.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 version: v1.0
 
 # Kubernetes credentials.
 kubeconfig: /path/to/kubeconfig
 kubecontext: null
 
 # Where Square will read and write manifests.
-folder: .
+folder: manifests/
 
 
 # -----------------------------------------------------------------------------
 # Square will only target resources that match *all* the selectors below.
 # -----------------------------------------------------------------------------
 selectors:
   # Target these resource kinds.
@@ -31,15 +31,15 @@
     - RoleBinding
     - Secret
     - Service
     - ServiceAccount
     - StatefulSet
 
   # Target these namespaces. Use an empty list to target all.
-  namespaces: ["default"]
+  namespaces: []
 
   # Example: ["app=square", "foo=bar"]. Use an empty list to ignore labels.
   labels: []
 
 
 # -----------------------------------------------------------------------------
 # Define the folder hierarchy that `square get` should create.
```

### Comparing `kubernetes_square-1.3.3/square/__init__.py` & `kubernetes_square-1.4.0/square/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 import sys
 
 from . import square
 from .cfgfile import load
 
-__version__ = '1.3.3'
+__version__ = '1.4.0'
 
 
 # ---------------------------------------------------------------------------
 # Global Runtime Constants
 # ---------------------------------------------------------------------------
 # Determine the base folder. This is usually the folder of this very file, but
 # will be different if we run inside a bundle produced by PyInstaller.
```

### Comparing `kubernetes_square-1.3.3/square/cfgfile.py` & `kubernetes_square-1.4.0/square/cfgfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,33 +5,34 @@
 dangerous, for Square to compute diffs on such field or patch them.
 
 This module defines utility functions to define these filters.
 
 """
 import copy
 import logging
-import typing
 from types import SimpleNamespace
-from typing import List, Tuple
+from typing import Tuple
 
 import pydantic
 import yaml
 
 from square.dtypes import Config, Filepath
 
+from .dtypes import FiltersKind
+
 # Convenience.
 logit = logging.getLogger("square")
 
 
-# Need to disable MyPy type checking because it would otherwise report the
-# first `if` statement as unreachable code. That warning is justified but
-# ignores the recursive nature of the function where one of the nested elements
-# may not adhere to the requirement.
-@typing.no_type_check
-def valid(filters: List[dict | list | str]) -> bool:
+def valid(filters: FiltersKind) -> bool:
+    """Return `True` iff `filters` is valid."""
+    return _valid(filters)
+
+
+def _valid(filters) -> bool:
     """Return `True` iff `filters` is valid."""
     if not isinstance(filters, list):
         logit.error(f"<{filters}> must be a list")
         return False
 
     # Iterate over all fields of all K8s resource type.
     for el in filters:
@@ -39,23 +40,23 @@
         if isinstance(el, dict):
             if len(el) != 1:
                 logit.error(f"<{el}> must have exactly one key")
                 return False
             value = list(el.values())[0]
 
             # Recursively check the dictionary values.
-            if not valid(value):
+            if not _valid(value):
                 logit.error(f"<{value}> is invalid")
                 return False
         elif isinstance(el, str):
             if el == "":
                 logit.error("Strings must be non-empty")
                 return False
         else:
-            logit.error(f"<{el}> must be a string")
+            logit.error(f"<{el}> must be a string or dict")
             return False
     return True
 
 
 def merge(src: list, dst: list) -> list:
     """Merge `src` into `dst` and return a copy of `dst`."""
     # Avoid side effects.
@@ -93,15 +94,15 @@
 
     _update(src, dst)
     return dst
 
 
 def load(fname: Filepath) -> Tuple[Config, bool]:
     """Parse the Square configuration file `fname` and return it as a `Config`."""
-    err_resp = Config(Filepath(""), kubeconfig=Filepath(""), kubecontext=None), True
+    err_resp = Config(folder=Filepath(""), kubeconfig=Filepath("")), True
     fname = Filepath(fname)
 
     # Load the configuration file.
     try:
         raw = yaml.safe_load(Filepath(fname).read_text())
     except FileNotFoundError as e:
         logit.error(f"Cannot load config file <{fname}>: {e.args[1]}")
@@ -112,29 +113,28 @@
         # Special case: parser supplied location information.
         mark = getattr(exc, "problem_mark", SimpleNamespace(line=-1, column=-1))
         line, col = (mark.line + 1, mark.column + 1)
         msg = f"YAML format error in {fname}: Line {line} Column {col}"
         logit.error(msg)
         return err_resp
 
-    if not isinstance(raw, dict):
-        logit.error(f"Config file <{fname}> has invalid structure")
-        return err_resp
-
     # Parse the configuration into `ConfigFile` structure.
     try:
-        cfg = Config(**raw)
+        cfg = Config.model_validate(raw)
+
+        # Explicitly access the computed `_kinds_names` attribute because
+        # Pydantic will not compute it until it is accessed.
+        cfg.selectors._kinds_names
+        cfg.selectors._kinds_only
     except (pydantic.ValidationError, TypeError) as e:
         logit.error(f"Schema is invalid: {e}")
         return err_resp
 
     # Remove the "_common_" filter and merge it into all the other filters.
     common = cfg.filters.pop("_common_", [])
     cfg.filters = {k: merge(common, v) for k, v in cfg.filters.items()}
     cfg.filters["_common_"] = common
 
     # Ensure the path is an absolute path.
     cfg.folder = fname.parent.absolute() / cfg.folder
 
-    # Convert the list to a set. No functional reason.
-    cfg.selectors.kinds = set(cfg.selectors.kinds)
     return cfg, False
```

### Comparing `kubernetes_square-1.3.3/square/dotdict.py` & `kubernetes_square-1.4.0/square/dotdict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+from typing import cast
 
 
 class DotDict(dict):
     """Dictionary that supports element access with '.'.
 
     Obviously, the usual Python rules apply. For instance, if
 
@@ -31,41 +32,55 @@
         # version of that copy.
         return make(copy.deepcopy(dict(self)))
 
     def __copy__(self, *args, **kwargs):
         return self.__deepcopy__(*args, **kwargs)
 
 
-def make(data):
+def make(data: dict):
     """Return `data` as a `DotDict`.
 
     This function will recursively replace all dictionary. It will also replace
     all tuples by lists.
 
     The intended input `data` of this function is any valid JSON structure.
 
     """
+    return cast(DotDict, _make(data))
+
+
+def _make(data):
+    """Recursively replace all Python dicts with `DotDict` instances."""
     if not isinstance(data, (list, tuple, dict)):
         return data
 
     # Recursively convert all elements in lists and dicts.
     if isinstance(data, (list, tuple)):
-        return [make(_) for _ in data]
+        return [_make(_) for _ in data]
     else:
-        return DotDict({k: make(v) for k, v in data.items()})
+        return DotDict({k: _make(v) for k, v in data.items()})
 
 
-def undo(data):
+def undo(data: DotDict | dict) -> dict:
     """Remove all `DotDict` instances from `data`.
 
     This function will recursively replace all `DotDict` instances with their
     plain Python equivalent.
 
     """
+    # Use an explicit cast because the `_undo` helper function is recursive and
+    # can thus, in theory, return something other than a dict. However, in
+    # practice it cannot because we already know that `data` is a dict and
+    # therefore so must be the return value.
+    return cast(dict, _undo(data))
+
+
+def _undo(data):
+    """Recursively replace all `DotDict` instances with their Python equivalent."""
     if not isinstance(data, (list, tuple, dict)):
         return data
 
     # Recursively convert all elements in lists and dicts.
     if isinstance(data, (list, tuple)):
-        return [undo(_) for _ in data]
+        return [_undo(_) for _ in data]
     else:
-        return dict({k: undo(v) for k, v in data.items()})
+        return dict({k: _undo(v) for k, v in data.items()})
```

### Comparing `kubernetes_square-1.3.3/square/dtypes.py` & `kubernetes_square-1.4.0/square/dtypes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-import dataclasses
 import pathlib
-from typing import (
-    TYPE_CHECKING, Any, Callable, Collection, Dict, List, NamedTuple, Optional,
-    Set, Tuple,
-)
+from typing import Any, Callable, Dict, List, NamedTuple, Optional, Set, Tuple
 
-if TYPE_CHECKING:
-    from dataclasses import dataclass
-else:
-    from pydantic.dataclasses import dataclass
+from pydantic import BaseModel, Field
 
 # All files in Square have this type.
 Filepath = pathlib.Path
 
 # Square will first save/deploy the resources in this list in this order.
 # Afterwards it will move on to all those resources not in this list. The order
 # in which it does that is undefined.
@@ -62,14 +55,15 @@
     kind: str
     namespace: Optional[str]
 
     # Every resource must have a name except for Namespaces, which encode their
     # name in the `namespace` field.
     name: str | None
 
+
 class K8sResource(NamedTuple):
     """Describe a specific K8s resource kind."""
     apiVersion: str   # "batch/v1beta1" or "extensions/v1beta1".
     kind: str         # "Deployment" (as specified in manifest)
     name: str         # "deployment" (usually lower case version of above)
     namespaced: bool  # Whether or not the resource is namespaced.
     url: str          # API endpoint, eg "k8s-host.com/api/v1/pods".
@@ -110,15 +104,15 @@
 # -----------------------------------------------------------------------------
 class JsonPatch(NamedTuple):
     """The URL for the patches as well as the patch payloads themselves."""
     # Send the patch to https://1.2.3.4/api/v1/namespace/foo/services
     url: str
 
     # The list of JSON patches.
-    ops: Collection[Dict[str, str]]
+    ops: List[Dict[str, str]]
 
 
 class DeltaCreate(NamedTuple):
     meta: MetaManifest
     url: str
     manifest: Dict[str, Any]
 
@@ -138,78 +132,125 @@
 class DeploymentPlan(NamedTuple):
     """Describe Square plan.
 
     Collects all resources manifests to add/delete as well as the JSON
     patches that make up a full plan.
 
     """
-    create: Collection[DeltaCreate]
-    patch: Collection[DeltaPatch]
-    delete: Collection[DeltaDelete]
+    create: List[DeltaCreate] | Tuple[DeltaCreate, ...]
+    patch: List[DeltaPatch] | Tuple[DeltaPatch, ...]
+    delete: List[DeltaDelete] | Tuple[DeltaDelete, ...]
 
 
 class DeploymentPlanMeta(NamedTuple):
     """Same as `DeploymentPlan` but contains `MetaManifests` only."""
-    create: Collection[MetaManifest]
-    patch: Collection[MetaManifest]
-    delete: Collection[MetaManifest]
+    create: List[MetaManifest] | Tuple[MetaManifest, ...]
+    patch: List[MetaManifest] | Tuple[MetaManifest, ...]
+    delete: List[MetaManifest] | Tuple[MetaManifest, ...]
 
 
 # -----------------------------------------------------------------------------
 #                             Square Configuration
 # -----------------------------------------------------------------------------
-def _factory(ret):
-    return dataclasses.field(default_factory=lambda: ret)
+class KindName(BaseModel):
+    """Holds a K8s resource Kind."""
+    kind: str = Field(min_length=1)  # Eg 'Service'
+    name: str                        # Eg. 'appname'
+
+
+class Selectors(BaseModel):
+    """Parameters to target specific groups of manifests."""
+    model_config = {"str_strip_whitespace": True}
 
+    kinds: Set[str] = set()
+    namespaces: List[str] = []
+    labels: List[str] = []
+
+    @property
+    def _kinds_names(self) -> List[KindName]:
+        """Deconstruct the Selector Kinds into Kind and Name.
+
+        These are the valid scenarios:
+          'Service'     -> ('Service', '')
+          'Service/'    -> ('Service', '')
+          'Service/foo' -> ('Service', 'foo')
+
+        """
+        # Unpack the 'Kind/Name' into a dedicated `KindName` model.
+        ans: List[KindName] = []
+        for src_kind in sorted(self.kinds):
+            # Ensure the `src_kind` has at most one '/'.
+            parts = src_kind.split("/")
+            if len(parts) == 1:
+                kind, name = parts[0], ""
+            elif len(parts) == 2:
+                kind, name = parts
+            else:
+                raise ValueError(f"Invalid kind {src_kind}")
+
+            # There must be no leading/trailing white space.
+            if (kind.strip() != kind) or (name.strip() != name):
+                raise ValueError(f"Invalid kind {src_kind}")
+
+            # Add the deconstructed Kind/Name selector.
+            ans.append(KindName(kind=kind, name=name))
+        return ans
+
+    @property
+    def _kinds_only(self) -> Set[str]:
+        """Compile the set of resource KINDS we are interested in.
+
+        NOTE: If the user selects `{"pod/app1", "deploy", "deploy/app1"}` then
+        we only want to retain `deploy` since `pod/app1` selects a unique Pod
+        whereas `deploy` selects all `Deployment` resources.
 
-@dataclass
-class Selectors:
-    """Comprises all the filters to select manifests."""
-    kinds: Set[str] = _factory(set(DEFAULT_PRIORITIES))
-    namespaces: List[str] = _factory([])
-    labels: List[str] = _factory([])
+        """
+        return {_.kind for _ in self._kinds_names if _.name == ""}
 
 
-@dataclass
-class GroupBy:
-    """Define how to organise downloaded manifest on the files system."""
+class GroupBy(BaseModel):
+    """Define how to organise downloaded manifests on the files system."""
     label: str = ""                  # "app"
-    order: List[str] = _factory([])  # ["ns", "label=app", kind"]
+    order: List[str] = []            # ["ns", "label=app", kind"]
+
+
+"""Define the filters to exclude sections of manifests."""
+FiltersKind = List[str | dict]
+Filters = Dict[str, FiltersKind]
 
 
-@dataclass
-class Config:
+class Config(BaseModel):
     """Uniform interface into top level Square API."""
     # Path to local manifests eg "./foo"
     folder: Filepath
 
     # Path to Kubernetes credentials.
     kubeconfig: Filepath
 
     # Kubernetes context (use `None` to use the default).
-    kubecontext: Optional[str]
+    kubecontext: Optional[str] = None
 
     # Only operate on resources that match the selectors.
-    selectors: Selectors = _factory(Selectors())
+    selectors: Selectors = Selectors()
 
     # Sort the manifest in this order, or alphabetically at the end if not in the list.
-    priorities: List[str] = _factory(list(DEFAULT_PRIORITIES))
+    priorities: List[str] = list(DEFAULT_PRIORITIES)
 
     # How to structure the folder directory when syncing manifests.
-    groupby: GroupBy = _factory(GroupBy())
+    groupby: GroupBy = GroupBy()
 
     # Define which fields to skip for which resource.
-    filters: Dict[str, List[str | dict]] = _factory({})
+    filters: Filters = {}
 
     # Callable: will be invoked for every local/server manifest that requires
     # patching before the actual patch will be computed.
     patch_callback: Optional[Callable] = None
 
     version: str = ""
 
 
 # -----------------------------------------------------------------------------
 #                                 Miscellaneous
 # -----------------------------------------------------------------------------
 LocalManifests = Dict[Filepath, Tuple[MetaManifest, dict]]
-LocalManifestLists = Dict[Filepath, Collection[Tuple[MetaManifest, dict]]]
-ServerManifests = Dict[MetaManifest, dict]
+LocalManifestLists = Dict[Filepath, List[Tuple[MetaManifest, dict]]]
+SquareManifests = Dict[MetaManifest, dict]
```

### Comparing `kubernetes_square-1.3.3/square/k8s.py` & `kubernetes_square-1.4.0/square/k8s.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import pathlib
 import re
 import subprocess
 import tempfile
 import warnings
 from collections import defaultdict
-from typing import Collection, Dict, List, Optional, Set, Tuple
+from typing import Dict, List, Optional, Set, Tuple, cast
 
 import backoff
 import google.auth
 import google.auth.exceptions
 import google.auth.transport.requests
 import requests
 import yaml
@@ -183,15 +183,15 @@
             logit.error(str(e))
             return (K8sConfig(), True)
 
     # Return the config data.
     logit.info("Assuming GKE cluster.")
     return K8sConfig(
         url=cluster["server"],
-        token=token,            # type: ignore
+        token=cast(str, token),
         ca_cert=ssl_ca_cert,
         client_cert=None,
         version="",
         name=cluster["name"],
     ), False
 
 
@@ -502,15 +502,15 @@
         # Return the correct URL, depending on whether we want all namespaces
         # or a particular one.
         url = f"{resource.url}/namespaces"
         if meta.name:
             url += f"/{meta.name}"
         return resource._replace(url=url), False
 
-    # Determine if the prefix for namespaced resources.
+    # Determine the prefix for namespaced resources.
     if meta.namespace is None:
         namespace = ""
     else:
         # Namespace name must conform to K8s standards.
         match = re.match(r"[a-z0-9]([-a-z0-9]*[a-z0-9])?", meta.namespace)
         if match is None or match.group() != meta.namespace:
             logit.error(f"Invalid namespace name <{meta.namespace}>.")
@@ -541,15 +541,15 @@
     return resource, False
 
 
 def request(
         client,
         method: str,
         url: str,
-        payload: Optional[dict],
+        payload: Optional[dict | list],
         headers: Optional[dict]) -> Tuple[dict, bool]:
     """Return response of web request made with `client`.
 
     Inputs:
         client: `requests` session with correct K8s certificates.
         url: str
             Eg `https://1.2.3.4/api/v1/namespaces`)
@@ -633,18 +633,18 @@
     resp, code = request(client, 'GET', url, payload=None, headers=None)
     err = (code != 200)
     if err:
         logit.error(f"{code} - GET - {url} - {resp}")
     return (resp, err)
 
 
-def patch(client, url: str, payload: Collection[Dict[str, str]]) -> Tuple[dict, bool]:
+def patch(client, url: str, payload: List[Dict[str, str]]) -> Tuple[dict, bool]:
     """Make PATCH requests to K8s (see `request`)."""
     headers = {'Content-Type': 'application/json-patch+json'}
-    resp, code = request(client, 'PATCH', url, payload, headers)  # type: ignore
+    resp, code = request(client, 'PATCH', url, payload, headers)
     err = (code != 200)
     if err:
         logit.error(f"{code} - PATCH - {url} - {resp}")
     return (resp, err)
 
 
 def post(client, url: str, payload: dict) -> Tuple[dict, bool]:
```

### Comparing `kubernetes_square-1.3.3/square/main.py` & `kubernetes_square-1.4.0/square/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import logging
 import os
-from typing import Optional, Tuple
+from typing import Any, Dict, Optional, Tuple
 
 import colorama
 
 import square
 import square.k8s
 import square.square
 from square import DEFAULT_CONFIG_FILE, __version__
@@ -80,15 +80,15 @@
         help='Mode', dest='parser', metavar="ACTION",
         title="Operation", required=True,
     )
 
     # Configuration for `kinds` positional arguments. Every sub-parser must
     # specify this one individually and here we define the kwargs to reduce
     # duplicated code.
-    kinds_kwargs = {
+    kinds_kwargs: Dict[str, Any] = {
         "dest": "kinds",
         "type": str,
         "nargs": '*',
         "metavar": "resource",
     }
 
     # Sub-command GET.
@@ -165,16 +165,16 @@
         Config, err
 
     """
     err_resp = Config(
         folder=Filepath(""),
         kubeconfig=Filepath(""),
         kubecontext=None,
-        selectors=Selectors(set(), namespaces=[], labels=[]),
-        groupby=GroupBy("", []),
+        selectors=Selectors(),
+        groupby=GroupBy(label="", order=[]),
         priorities=[],
     ), True
 
     # Convenience.
     p = cmdline_param
 
     # Load the default configuration unless the user specified an explicit one.
@@ -268,15 +268,15 @@
     # Use the value from the (default) config file unless the user overrode
     # them on the command line.
     kubeconfig = Filepath(kubeconfig)
     kubecontext = p.kubecontext or cfg.kubecontext
     namespaces = cfg.selectors.namespaces if p.namespaces is None else p.namespaces
     sel_labels = cfg.selectors.labels if p.labels is None else p.labels
     priorities = p.priorities or cfg.priorities
-    selectors = Selectors(kinds, namespaces, sel_labels)
+    selectors = Selectors(kinds=kinds, namespaces=namespaces, labels=sel_labels)
 
     # Use filters from (default) config file because they cannot be specified
     # on the command line.
     filters = cfg.filters
 
     # ------------------------------------------------------------------------
     # Verify inputs.
@@ -346,26 +346,24 @@
 
 def expand_all_kinds(cfg: Config) -> Tuple[Config, bool]:
     """Replace an empty `cfg.selector.kinds` with all available resources.
 
     Does nothing if `cfg.selectors.kinds` is non-empty.
 
     """
-    # Do nothing if the user specified at least on resource type.
+    # Do nothing if the user specified at least one resource type.
     if len(cfg.selectors.kinds) > 0:
         return cfg, False
 
     # Create a K8sConfig instance because it will contain all the info we need.
     k8sconfig, err = square.k8s.cluster_config(cfg.kubeconfig, cfg.kubecontext)
     if err:
         return (cfg, True)
 
-    # Replace the empty resource list with all kinds that K8s has to offer and
-    # that Square can manage (ie all kinds with the correct set of verbs to
-    # create, delete, get, and patch).
+    # Replace the empty resource list with all KINDS that K8s has to offer.
     cfg.selectors.kinds.clear()
     cfg.selectors.kinds.update(k8sconfig.kinds)
     return (cfg, False)
 
 
 def show_info(cfg: Config) -> bool:
     """Show some info about the configuration that will be used."""
@@ -392,15 +390,15 @@
     if param.parser == "config":
         fname = Filepath(param.folder or ".") / ".square.yaml"
         fname.parent.mkdir(parents=True, exist_ok=True)
         fname.write_text(DEFAULT_CONFIG_FILE.read_text())
         print(
             f"Created configuration file <{fname}>.\n"
             "Please open the file in an editor and adjust the values, most notably "
-            "<kubeconfig>, <kubecontext>, <folder> and <selectors.labels>."
+            "`kubeconfig` and `selectors.[kinds | namespaces | labels]`."
         )
         return 0
 
     # Initialise logging.
     square.square.setup_logging(param.verbosity)
 
     # Create Square configuration from command line arguments.
```

### Comparing `kubernetes_square-1.3.3/square/manio.py` & `kubernetes_square-1.4.0/square/manio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,34 @@
 import collections
 import copy
 import difflib
 import logging
 import multiprocessing
 import pathlib
-from typing import (
-    Collection, DefaultDict, Dict, Iterable, List, Optional, Tuple,
-)
+from typing import DefaultDict, Dict, Iterable, List, Optional, Tuple, cast
 
 import yaml.parser
 import yaml.scanner
 
 import square.cfgfile
 import square.dotdict
 import square.k8s
 from square.dtypes import (
-    Config, Filepath, GroupBy, K8sConfig, K8sResource, LocalManifestLists,
-    MetaManifest, Selectors, ServerManifests,
+    Config, Filepath, Filters, FiltersKind, GroupBy, K8sConfig, K8sResource,
+    KindName, LocalManifestLists, MetaManifest, Selectors, SquareManifests,
 )
+from square.yaml_io import Dumper, Loader
 
 # Convenience: global logger instance to avoid repetitive code.
 logit = logging.getLogger("square")
 DotDict = square.dotdict.DotDict
 
 
-# Use the fast CSafeLoader/CSafeDumper from the LibYAML C library if they are
-# available on the host, otherwise fall back to the slow Python loader/dumper.
-# NOTE: this import is excluded from the coverage report since it is difficult
-#       to write a meaningful test around a library import that may or may not
-#       exist on the host. I deem this acceptable in this case because it is a
-#       widely used snipped devoid of logic.
-try:                                 # codecov-skip
-    from yaml import (  # type: ignore
-        CSafeDumper as Dumper, CSafeLoader as Loader,
-    )
-    logit.debug("Using LibYAML C library")
-except ImportError:                  # codecov-skip
-    from yaml import Dumper, Loader  # type: ignore
-    logit.debug("Using Python YAML library")
-
-
 def make_meta(manifest: dict) -> MetaManifest:
-    """Compile `MetaManifest` information from `manifest` and return it.
+    """Extract the `MetaManifest` information from `manifest`.
 
     Throw `KeyError` if manifest lacks essential fields like `apiVersion`,
     `kind`, etc because it cannot possibly be a valid K8s manifest then.
 
     """
     # Unpack the namespace. For Namespace resources, this will be the "name".
     if manifest["kind"] == "Namespace":
@@ -71,94 +54,94 @@
         manifests: dict
         selectors: Selectors,
 
     Returns:
         bool: `True` iff the resource matches all selectors.
 
     """
-    # "kinds" cannot be an empty list or `None`.
-    if not selectors.kinds:
+    # The "kinds" selector must be non-empty.
+    if len(selectors.kinds) == 0:
         logit.error(f"BUG: selector must specify a `kind`: {selectors}")
         return False
 
     # Split all labels into tuples: "foo=bar" -> ("foo", "bar").
     # Sanity check: hard abort if the labels do not split.
     label_selectors = {tuple(_.split("=")) for _ in selectors.labels}
     assert all([len(_) == 2 for _ in label_selectors])
 
-    # Unpack the resource's kind and labels.
-    kind = manifest.get("kind", None)
+    # Unpack KIND, LABELS and NAME.
+    kind = manifest.get("kind", "_unknown_")
     labels = manifest.get("metadata", {}).get("labels", {})
     name = manifest.get("metadata", {}).get("name", "")
 
-    # Unpack the resource's namespace.
-    ns = manifest.get("metadata", {}).get("namespace", None)
-
     # We need to pay special attention to `Namespace` resources since they are
     # not themselves namespaced.
     #
     # Furthermore, we *never* mess with `default-token-*` Secrets or the
     # `default` service account. K8s automatically creates them in every new
     # namespace. We can thus never "restore" them with Square because the plan
-    # says to create them yet once Square created the namespace they also
-    # already exist and can only be patched. As a result, Square would abort
-    # unexpectedly.
+    # would create them yet once Square created the associated namespace the
+    # service account already exist and can only be patched, not created
+    # anymore. As a result, Square would abort unexpectedly.
+    ns = manifest.get("metadata", {}).get("namespace", None)
     if kind == "Namespace":
         ns = manifest.get("metadata", {}).get("name", None)
     elif kind == "Secret":
         if name.startswith("default-token-"):
             logit.info("Skipping `default-token` Secret")
             return False
     elif kind == "ServiceAccount":
         if name == "default":
             logit.info("Skipping `default` service account")
             return False
     else:
         pass
 
-    # Proceed only if the resource kind is among the desired ones.
-    if kind not in selectors.kinds:
-        logit.debug(f"Kind {kind} does not match selector {selectors.kinds}")
-        return False
-
-    # Include the resource if it is a) namespaced b) we have namespace
-    # selectors and c) the resource matches one of them.
-    if ns and selectors.namespaces and ns not in selectors.namespaces:
+    # Skip this resource if it is a) namespaced b) we have namespace
+    # selectors and c) the resource does not match it.
+    if (ns and selectors.namespaces) and ns not in selectors.namespaces:
         logit.debug(f"Namespace {ns} does not match selector {selectors.namespaces}")
         return False
 
-    # Convert the labels dictionary into a set of (key, value) tuples. We can
-    # then use set logic to determine if the resource specifies the desired
-    # labels or not.
-    labels = {(k, v) for k, v in labels.items()}
+    if KindName(kind=kind, name=name) in selectors._kinds_names:
+        return True
 
-    # The resource must match the label selectors unless we have no such selectors.
+    # Abort if this manifest does not have a KIND that matches the selector.
+    if kind not in selectors._kinds_only:
+        logit.debug(f"Kind {kind} does not match selector {selectors.kinds}")
+        return False
+
+    # The manifest must match all label selectors to be included.
     if label_selectors:
+        # Convert the labels dictionary into a Set of (key, value) tuples. We can
+        # then use set-logic to determine if the manifest has the necessary labels.
+        labels = set(labels.items())
+
         if not label_selectors.issubset(labels):
             logit.debug(f"Labels {labels} do not match selector {selectors.labels}")
             return False
 
     # If we get to here then the resource matches all selectors.
     return True
 
 
-def unpack_list(manifest_list: dict,
-                selectors: Selectors) -> Tuple[ServerManifests, bool]:
-    """Unpack a K8s List item, eg `DeploymentList` or `NamespaceList`.
+def unpack_k8s_resource_list(manifest_list: dict,
+                             selectors: Selectors) -> Tuple[SquareManifests, bool]:
+    """Return only those entries from `manifest_list` that match the `selectors`.
 
-    Return a dictionary where each key uniquely identifies the resource via a
-    `MetaManifest` tuple and the value is the actual JSON `manifest`.
+    The `manifest_list` must be a K8s List item, eg `DeploymentList` or
+    `NamespaceList`.
 
     Input:
         manifest_list: dict
             K8s response from GET request for eg `deployments`.
         selectors: Selectors
 
     Returns:
-        dict[MetaManifest:dict]
+        SquareManifests
 
     """
     # Ensure the server manifests have the essential fields. If not then
     # something is seriously wrong.
     must_have = ("apiVersion", "kind", "items")
     missing = [key for key in must_have if key not in manifest_list]
     if len(missing) > 0:
@@ -191,15 +174,15 @@
         manifest['apiVersion'] = apiversion
         if select(manifest, selectors):
             manifests[make_meta(manifest)] = manifest
     return (manifests, False)
 
 
 def _parse_worker(fname: Filepath,
-                  yaml_str: str) -> Tuple[Collection[dict], bool]:
+                  yaml_str: str) -> Tuple[List[dict], bool]:
     logit.debug(f"Parsing <{fname}>")
 
     # Decode the YAML documents in the current file.
     try:
         manifests = list(yaml.load_all(yaml_str, Loader=Loader))
         return manifests, False
     except (yaml.parser.ParserError, yaml.scanner.ScannerError) as err:
@@ -266,29 +249,29 @@
     num_manifests = [len(_) for _ in out.values()]
     logit.debug(f"Parsed {sum(num_manifests)} manifests in {len(num_manifests)} files")
 
     # Return the YAML parsed manifests.
     return (out, False)
 
 
-def unpack(manifests: LocalManifestLists) -> Tuple[ServerManifests, bool]:
-    """Convert `manifests` to `ServerManifests` for internal processing.
+def compile_square_manifests(manifests: LocalManifestLists) -> Tuple[SquareManifests, bool]:  # noqa
+    """Convert `manifests` into `SquareManifests` for internal processing.
 
     Returns `False` unless all resources in `manifests` are unique. For
     instance, returns False if two files define the same namespace or the same
     deployment.
 
     The primary use case is to convert the manifests we read from local files
     into the format Square uses internally for the server manifests as well.
 
     Inputs:
         manifests: LocalManifestLists
 
     Returns:
-        ServerManifests: flattened version of `manifests`.
+        SquareManifests: flattened version of `manifests`.
 
     """
     # Compile a dict that shows which meta manifest was defined in which file.
     # We will shortly use this information to determine if all resources were
     # defined exactly once across all files.
     all_meta: DefaultDict[MetaManifest, list] = collections.defaultdict(list)
     for fname in manifests:
@@ -311,67 +294,67 @@
 
     # Compile the input manifests into a new dict with the meta manifest as key.
     out = {k: v for fname in manifests for k, v in manifests[fname]}
     return (out, False)
 
 
 def sync(local_manifests: LocalManifestLists,
-         server_manifests: ServerManifests,
+         server_manifests: SquareManifests,
          selectors: Selectors,
          groupby: GroupBy) -> Tuple[LocalManifestLists, bool]:
     """Update the local manifests with the server values and return the result.
 
     Inputs:
         local_manifests: Dict[Filepath, Tuple[MetaManifest, dict]]
         server_manifests: Dict[MetaManifest, dict]
         selectors: Selectors
             Only operate on resources that match the selectors.
         groupby: GroupBy
             Specify relationship between new manifests and file names.
 
     Returns:
-        Dict[Filepath, Tuple[MetaManifest, dict]]
+        Dict[Filepath, List[Tuple[MetaManifest, dict]]]
 
     """
     # Avoid side effects.
     server_manifests = copy.deepcopy(server_manifests)
 
-    # Only retain server manifests with correct `kinds` and `namespaces`.
+    # Only retain server manifests that match the selectors.
     server_manifests = {
         meta: manifest for meta, manifest in server_manifests.items()
         if select(manifest, selectors)
     }
 
-    # Add all local manifests outside the specified `kinds` and `namespaces`
-    # to the server list. This will *not* propagate to the server in any way,
-    # but allows us to make the rest of the function oblivious to the fact that
-    # we only care about a subset of namespaces and resources by pretending
-    # that local and server manifests are already in sync.
+    # Add all local manifests that do not match the selectors to the server
+    # manifests. This will *not* propagate to K8s in any way. However, it will
+    # simplify the logic of this function because local and server manifests
+    # that were not selected will be automatically in sync and not appear in
+    # the diffs.
     for fname, manifests in local_manifests.items():
         for meta, manifest in manifests:
             if select(manifest, selectors):
                 continue
             server_manifests[meta] = manifest
 
     # Create map for MetaManifest -> (File, doc-idx). The doc-idx denotes the
-    # index of the manifest inside the YAML files (it may contain multiple
-    # manifests). We will need that information later to find out which
-    # manifest in which file we need to update.
+    # index of the manifest inside the YAML file which may contain multiple
+    # manifests. We will need this index later to update the correct manifest
+    # in the correct YAML file.
     meta_to_fname = {}
     for fname in local_manifests:
         for idx, (meta, _) in enumerate(local_manifests[fname]):
             meta_to_fname[meta] = (fname, idx)
             del meta
         del fname
 
     # Make a copy of the local manifests to avoid side effects for the caller.
     # Also put it into a default dict for convenience.
     out_add_mod: DefaultDict[Filepath, List[Tuple[MetaManifest, dict]]]
     out_add_mod = collections.defaultdict(list)
-    out_add_mod.update(copy.deepcopy(local_manifests))  # type: ignore
+    out_add_mod.update(copy.deepcopy(local_manifests))
     del local_manifests
 
     # If the server's meta manifest exists locally then update the local one,
     # otherwise add it to the catchall YAML file.
     for meta, manifest in server_manifests.items():
         try:
             # Find the file that defined `meta` and its position inside that file.
@@ -447,18 +430,15 @@
 
     # Default to the catch-all `_other.yaml` resource if the order did not
     # produce a file name. This typically happens when `grouping.order = []`.
     path = "_other.yaml" if path == "" else f"{path}.yaml"
     return Filepath(path), False
 
 
-def diff(config: Config,
-         k8sconfig: K8sConfig,
-         local: dict,
-         server: dict) -> Tuple[str, bool]:
+def diff(local: dict, server: dict) -> Tuple[str, bool]:
     """Return the human readable diff between the `local` and `server` manifest.
 
     The diff shows the necessary changes to transition the `server` manifest
     into the state of the `local` manifest.
 
     Inputs:
         config: Square configuration.
@@ -483,44 +463,43 @@
     diff_lines = difflib.unified_diff(srv_lines, loc_lines, lineterm='')
     return (str.join("\n", diff_lines), False)
 
 
 def strip(
     k8sconfig: K8sConfig,
     manifest: dict,
-    manifest_filters: Dict[str, list],
+    manifest_filters: Filters,
 ) -> Tuple[DotDict, dict, bool]:
     """Strip `manifest` according to the filters in `square.cfgfile`.
 
     Inputs:
         k8sconfig: K8sConfig
         manifest: dict
         manifest_filters: Dict[str, list]
             See tests for examples
 
     Returns:
         dict, dict: (stripped manifest, removed keys).
 
     """
     # Convenience: default return value if an error occurs.
-    ret_err: Tuple[DotDict, dict, bool] = (
-        square.dotdict.make({}), {}, True) # type: ignore
+    ret_err: Tuple[DotDict, dict, bool] = (square.dotdict.make({}), {}, True)
 
     # Parse the manifest.
     try:
         meta = make_meta(manifest)
         _, err = square.k8s.resource(k8sconfig, meta)
         assert not err
     except KeyError as e:
         logit.error(f"Manifest is missing the <{e.args[0]}> key.")
         return ret_err
     except AssertionError:
         return ret_err
 
-    def _update(filters: list, manifest: dict):
+    def _update(filters: FiltersKind, manifest: dict):
         """Recursively traverse the `manifest` and prune it according to `filters`.
 
         Returns dict with the excluded keys.
 
         Raise `KeyError` if an invalid key was found.
 
         """
@@ -565,44 +544,40 @@
 
     # Look up the filters for the current resource in the following order:
     # 1) Supplied `filters`
     # 2) Square default filters for this resource `kind`.
     # 3) Square default filters that apply to all resource kinds.
     # Pick the first one that matches.
     kind = manifest["kind"]
-    filters = manifest_filters.get(
-        kind,
-        square.DEFAULT_CONFIG.filters.get(
-            kind,
-            square.DEFAULT_CONFIG.filters["_common_"]
-        )
-    )
-    if not square.cfgfile.valid(filters):  # type: ignore
+
+    default_filter = cast(Filters, square.DEFAULT_CONFIG.filters["_common_"])
+    filters: FiltersKind = cast(FiltersKind, manifest_filters.get(kind, default_filter))
+    if not square.cfgfile.valid(filters):
         return ret_err
 
     # Remove the keys from the `manifest` according to `filters`.
     manifest = copy.deepcopy(manifest)
     removed = _update(filters, manifest)
-    return (square.dotdict.make(manifest), removed, False)  # type: ignore
+    return (square.dotdict.make(manifest), removed, False)
 
 
 def align_serviceaccount(
-        local_manifests: ServerManifests,
-        server_manifests: ServerManifests) -> Tuple[ServerManifests, bool]:
+        local_manifests: SquareManifests,
+        server_manifests: SquareManifests) -> Tuple[SquareManifests, bool]:
     """Insert the token secret from `server_manifest` into `local_manifest`.
 
     Every ServiceAccount (SA) has a "secrets" section that K8s automatically
     populates when it creates the SA. The name contains a random hash, eg
     "default-token-somerandomhash" for the default service account in every
     namespace.
 
     This makes it difficult to manage service accounts with Square because the
     token is not known in advance. One would have to
 
-        square apply; square plan; square get serviceaccount
+        square apply serviceaccount; square get serviceaccount
 
     to sync this, and even that is not portable because the token will be
     different on a new cluster.
 
     To avoid this problem, this function will read the token secret that K8s
     added (contained in `server_manifest`) and insert it into the
     `local_manifest`. This will ensure that Square creates a plan that
@@ -615,15 +590,15 @@
     Returns:
         Copy of `local_manifests` where all ServiceAccount token secrets match
         those of the server.
 
     """
     ReturnType = Tuple[Optional[str], List[Dict[str, str]], bool]
 
-    def _get_token(meta: MetaManifest, manifests: ServerManifests) -> ReturnType:
+    def _get_token(meta: MetaManifest, manifests: SquareManifests) -> ReturnType:
         """Return token secret from `manifest` as well as all other other secrets.
 
         Example input manifest:
             {
                 'apiVersion': v1,
                 'kind': ServiceAccount,
                 ...
@@ -757,20 +732,21 @@
 
 
 def load_files(
         folder: Filepath,
         fnames: Iterable[Filepath]) -> Tuple[Dict[Filepath, str], bool]:
     """Load all `fnames` in `folder` and return their content.
 
+    This is a convenience function for Square to recursively load all manifests
+    in a given manifest folder. It will either return the content of all files,
+    or an error. In particular, it will never return only a sub-set of files.
+
     The elements of `fname` can have sub-paths, eg `foo/bar/file.txt` is valid
     and would ultimately open f"{folder}/foo/bar/file.txt".
 
-    Either returns the content of all files or returns with an error and no
-    data. It will not return only a sub-set of the files.
-
     Inputs:
         folder: Path
         fnames: Iterable[str|Path]
             The file names relative to `folder`.
 
     Returns:
         Dict[Filepath, str]: the file names (relative to `folder`) and their
@@ -795,29 +771,30 @@
             logit.error(f"Could not find <{fname_abs}>")
             return ({}, True)
 
     # Return the read files.
     return (out, False)
 
 
-def load(folder: Filepath, selectors: Selectors) -> Tuple[
-         ServerManifests, LocalManifestLists, bool]:
-    """Recursively load all "*.yaml" files under `folder`.
+def load_manifests(folder: Filepath,
+                   selectors: Selectors) -> Tuple[SquareManifests,
+                                                  LocalManifestLists, bool]:
+    """Return all K8s manifest found in `folder`.
 
-    Ignores all files not ending in ".yaml". Also removes all manifests that do
-    not match the `selectors`.
+    Recursively load all "*.yaml" files in `folder` and return those manifests
+    that match the `selectors`.
 
-    Returns no data in the case of an error.
+    It will either return all manifests or none, if there was an error. In
+    particular, it will never return only a sub-set of files (cf `load_files`).
 
     NOTE: this is merely a wrapper around the various low-level functions to
-    load and parse the YAML files.
+    load and parse YAML files.
 
     Input:
         folder: Filepath
-            Source folder.
         selectors: Selectors
 
     Returns:
         (local manifest without file info, local manifests with file info)
 
     """
     # Python's `pathlib.Path` objects are simply nicer to work with...
@@ -834,41 +811,41 @@
         assert not err and fdata_raw is not None
 
         # Return the YAML parsed manifests.
         man_files, err = parse(fdata_raw, selectors)
         assert not err and man_files is not None
 
         # Remove the Filepath dimension.
-        man_meta, err = unpack(man_files)
+        man_meta, err = compile_square_manifests(man_files)
         assert not err and man_meta is not None
     except AssertionError:
         return ({}, {}, True)
 
     # Return the file based manifests and unpacked manifests.
     return (man_meta, man_files, False)
 
 
 def sort_manifests(
         file_manifests: LocalManifestLists,
-        priority: Collection[str]
-) -> Tuple[Dict[Filepath, Collection[MetaManifest]], bool]:
+        priority: List[str]
+) -> Tuple[Dict[Filepath, List[dict]], bool]:
     """Sort the manifests in each `file_manifests` by their `priority`.
 
     The returned data contains only the manifests without the `MetaData`. The
     idea is to pass that data directly to `save_files`.
 
     Inputs:
         file_manifests: the manifests that should go into each file.
-        priority: Collection[str]
+        priority: List[str]
             Sort the manifest in this order, or alphabetically at the end if
             not in the list.
 
     """
     # Sort the manifests in each file.
-    out: Dict[Filepath, Collection[MetaManifest]] = {}
+    out: Dict[Filepath, List[dict]] = {}
     for fname, manifests in file_manifests.items():
         # Group the manifests by their "kind" in order of `priority` and sort
         # each group alphabetically.
         man_sorted: list = []
         for kind in priority:
             # Partition the manifest list into the current `kind` and the rest.
             tmp = [_ for _ in manifests if _[0].kind == kind]
@@ -888,51 +865,56 @@
             # Append the manifests ordered by their MetaManifest.
             man_sorted += sorted(tmp, key=lambda _: _[0])
 
         # sanity check: we must have used up all manifests.
         assert len(manifests) == 0
 
         # Drop the MetaManifest, ie
-        # Dict[Filepath:Tuple[MetaManifest, manifest]] -> Dict[Filepath:manifest]
+        # List[Tuple[MetaManifest, dict]] -> List[dict]
         man_clean = [manifest for _, manifest in man_sorted]
 
         # Assign the grouped and sorted list of manifests to the output dict.
         out[fname] = man_clean
 
     return out, False
 
 
-def save(folder: Filepath, manifests: LocalManifestLists,
-         priority: Collection[str]) -> bool:
+def save(folder: Filepath,
+         manifests: LocalManifestLists,
+         priority: List[str]) -> bool:
     """Saves all `manifests` as YAMLs in `folder`.
 
     Input:
         folder: Filepath
             Source folder.
         file_manifests: Dict[Filepath, Tuple(MetaManifest, dict)]
             Names of files and their Python dicts to save as YAML.
-        priority: Collection[str]
+        priority: List[str]
             Sort the manifest in this order, or alphabetically at the end if
             not in the list.
 
     Returns:
         None
 
     """
     # Sort the manifest in each file by priority. Ignore the error flag because
     # `sort_manifests` always succeeds.
+    # out: Dict[FilePath, List[dict]]
     out, _ = sort_manifests(manifests, priority)
 
     # Ignore all files without manifests, ie empty files.
     out_nonempty = {k: v for k, v in out.items() if len(v) > 0}
     del out
 
-    # Ensure we have no `DotDicts` left. This will avoid problems with the YAML
-    # serialisation below.
-    out_clean = {k: square.dotdict.undo(v) for k, v in out_nonempty.items()}
+    # Ensure that our list of manifests does not contain any `DotDicts`
+    # anymore. This will avoid problems with the YAML serialisation below.
+    out_clean = {
+        fname: [square.dotdict.undo(man) for man in manifests]
+        for fname, manifests in out_nonempty.items()
+    }
     del out_nonempty
 
     # Ignore all hidden files.
     out_clean = {k: v for k, v in out_clean.items() if not k.name.startswith(".")}
 
     # Convert all manifest dicts into YAML strings.
     out_final: Dict[Filepath, str] = {}
@@ -947,15 +929,15 @@
         )
         return True
 
     # Save the files to disk.
     return save_files(folder, out_final)
 
 
-def download(config: Config, k8sconfig: K8sConfig) -> Tuple[ServerManifests, bool]:
+def download(config: Config, k8sconfig: K8sConfig) -> Tuple[SquareManifests, bool]:
     """Download and return the resources that match `selectors`.
 
     Set `selectors.namespace` to `None` to download the resources from all
     Kubernetes namespaces.
 
     Either returns all the data or an error; never returns partial results.
 
@@ -973,17 +955,24 @@
     # Ensure `namespaces` is always a list to avoid special casing below.
     all_namespaces: Iterable[Optional[str]]
     if not config.selectors.namespaces:
         all_namespaces = [None]
     else:
         all_namespaces = config.selectors.namespaces
 
+    # Determine all the resource endpoints we need to interrogate K8s. We
+    # cannot use `config.selectors._kinds_only` because it will be empty if the
+    # user selected only specific resources, eg `svc/foo` instead of just
+    # `svc`. We therefore need to compile the list of all resource types the
+    # user wanted which we can get from the `selectors._kinds_names`.
+    all_kinds = {_.kind for _ in config.selectors._kinds_names}
+
     # Download each resource type. Abort at the first error and return nothing.
     for namespace in all_namespaces:
-        for kind in sorted(config.selectors.kinds):
+        for kind in sorted(all_kinds):
             # Get the K8s URL for the current resource kind. Ignore this
             # resource if K8s does not know about it. The reason for that could
             # be a typo or that it is a Custom Resource that does not (yet) exist.
             resource, err = square.k8s.resource(k8sconfig, MetaManifest("", kind, namespace, ""))  # noqa
             if err:
                 logit.warning(f"Skipping unknown resource <{kind}>")
                 continue
@@ -991,15 +980,15 @@
             try:
                 # Download the resource manifests for the current `kind` from K8s.
                 manifest_list, err = square.k8s.get(k8sconfig.client, resource.url)
                 assert not err and manifest_list is not None
 
                 # Parse the K8s List (eg DeploymentList, NamespaceList, ...) into a
                 # Dict[MetaManifest, dict] dictionary.
-                manifests, err = unpack_list(manifest_list, config.selectors)
+                manifests, err = unpack_k8s_resource_list(manifest_list, config.selectors)
                 assert not err and manifests is not None
 
                 # Strip off the fields defined in `config.filters`.
                 ret = {k: strip(k8sconfig, man, config.filters)
                        for k, man in manifests.items()}
 
                 # Ensure `strip` worked for every manifest.
```

### Comparing `kubernetes_square-1.3.3/square/square.py` & `kubernetes_square-1.4.0/square/square.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,62 +14,67 @@
 
 import square.dotdict as dotdict
 import square.k8s as k8s
 import square.manio as manio
 from square.dtypes import (
     Config, DeltaCreate, DeltaDelete, DeltaPatch, DeploymentPlan,
     DeploymentPlanMeta, JsonPatch, K8sConfig, MetaManifest, Selectors,
-    ServerManifests,
+    SquareManifests,
 )
 
 # Convenience: global logger instance to avoid repetitive code.
 logit = logging.getLogger("square")
 
 
 def translate_resource_kinds(cfg: Config, k8sconfig: K8sConfig) -> Config:
     """Convert `cfg.Selectors.kind` and `cfg.priorities` to their canonical names.
 
     Example: "svc" -> "Service" or "ns" -> "Namespace".
 
     Silently ignore unknown resource kinds. This is necessary because the user
-    may have specified a custom resource that does not (yet) exist. Since we cannot
-    distinguish them from typos, we allow unknown resource kinds but
-    get/plan/apply cycles will ignore them.
+    may have specified a custom resource that does not (yet) exist. Since we
+    cannot distinguish those from typos we allow them here because the
+    get/plan/apply cycle will ignore them anyway.
 
     """
+    # Convenience
+    short2kind = k8sconfig.short2kind
+
     # Avoid side effects to the original `cfg`.
     cfg = copy.deepcopy(cfg)
 
-    # Translate the possibly colloquial names to their canonical K8s names. Use
-    # the original name if we cannot find the canonical name.
-    kinds = {k8sconfig.short2kind.get(_.lower(), _) for _ in cfg.selectors.kinds}
-    priorities = [k8sconfig.short2kind.get(_.lower(), _) for _ in cfg.priorities]
+    # Translate the shorthand names to their canonical K8s names. Use the
+    # original name if we cannot find a canonical name for it.
+    cfg.priorities = [short2kind.get(_.lower(), _) for _ in cfg.priorities]
 
-    # Return a copy of `cfg` with the translated resource kinds.
+    # Backup the original list of KIND selectors.
+    kinds_names = [(_.kind, _.name) for _ in cfg.selectors._kinds_names]
     cfg.selectors.kinds.clear()
-    cfg.selectors.kinds.update(kinds)
-    cfg.priorities.clear()
-    cfg.priorities.extend(priorities)
+
+    # Convert eg [("ns"), ("svc", "app1")] -> {"Namespace", "Service/app1"}.
+    for kind, name in kinds_names:
+        ans = short2kind.get(kind.lower(), kind)
+        ans = ans if name == "" else f"{ans}/{name}"
+        cfg.selectors.kinds.add(ans)
+
     return cfg
 
 
 def make_patch(
-        config: Config,
         k8sconfig: K8sConfig,
         local: dict,
         server: dict) -> Tuple[JsonPatch, bool]:
     """Return JSON patch to transition `server` to `local`.
 
     Inputs:
-        config: Square configuration.
         k8sconfig: K8sConfig
         local: dict
-            Usually on fo the dict manifests returned by `load_manifest`.
+            Usually one of the manifests returned by `load_manifest`.
         server: dict
-            Usually on fo the dict manifests returned by `manio.download`.
+            Usually one of the manifests returned by `manio.download`.
 
     Returns:
         Patch: the JSON patch and human readable diff in a `Patch` tuple.
 
     """
     # Convenience.
     loc, srv = local, server
@@ -102,31 +107,31 @@
     patch = json.loads(patch.to_string())
 
     # Return the patch.
     return (JsonPatch(res_srv.url, patch), False)
 
 
 def partition_manifests(
-        local: ServerManifests,
-        server: ServerManifests) -> Tuple[DeploymentPlanMeta, bool]:
+        local: SquareManifests,
+        server: SquareManifests) -> Tuple[DeploymentPlanMeta, bool]:
     """Compile `{local,server}` into CREATE, PATCH and DELETE groups.
 
     The returned deployment plan will contain *every* resource in
     `local` and `server` *exactly once*. Their relative
     order will also be preserved.
 
     Create: all resources that exist in `local` but not in `server`.
     Delete: all resources that exist in `server` but not in `local`.
     Patch : all resources that exist in both and therefore *may* need patching.
 
     Inputs:
-        local: ServerManifests
-            Usually the dictionary keys returned by `load_manifest`.
-        server: ServerManifests
-            Usually the dictionary keys returned by `manio.download`.
+        local: SquareManifests
+            Usually the dictionaries returned by `load_manifest`.
+        server: SquareManifests
+            Usually the dictionaries returned by `manio.download`.
 
     Returns:
         DeploymentPlanMeta
 
     """
     # Determine what needs adding, removing and patching to steer the K8s setup
     # towards what `local` specifies.
@@ -146,31 +151,31 @@
     # Return the deployment plan.
     plan = DeploymentPlanMeta(create_l, patch_l, delete_l)
     return (plan, False)
 
 
 def match_api_version(
         k8sconfig: K8sConfig,
-        local: ServerManifests,
-        server: ServerManifests) -> Tuple[ServerManifests, bool]:
+        local: SquareManifests,
+        server: SquareManifests) -> Tuple[SquareManifests, bool]:
     """Fetch the manifests from the endpoints defined in the local manifest.
 
     If a local manifest uses a different value for `apiVersion` then we need to
     re-fetch those manifests from K8s via that endpoint. This function does
     just that.
 
     This function returns `server` verbatim if there is no overlap with
     `server` and `local`.
 
     Inputs:
         config: Square configuration.
         k8sconfig: K8sConfig
-        local: ServerManifests
+        local: SquareManifests
             Should be output from `load_manifest` or `load`.
-        server: ServerManifests
+        server: SquareManifests
             Should be output from `manio.download`.
 
     Returns:
         `server` but possibly with some entries re-fetched from the same K8s
         endpoint that the equivalent resource in `local` specifies.
 
     """
@@ -232,17 +237,17 @@
 
     NOTE: modifies `local` and `server` inplace.
 
     Inputs:
         config: Square configuration.
         plan_patch: List[MetaManifest]
             The list of meta manifests that currently require a patch.
-        local: ServerManifests
+        local: SquareManifests
             Should be output from `load_manifest` or `load`.
-        server: ServerManifests
+        server: SquareManifests
             Should be output from `manio.download`.
 
     """
     # Do nothing and return immediately if the user did not provide a callback.
     cb = config.patch_callback
     if not cb:
         return False
@@ -267,28 +272,28 @@
         return True
     return False
 
 
 def compile_plan(
         config: Config,
         k8sconfig: K8sConfig,
-        local: ServerManifests,
-        server: ServerManifests) -> Tuple[DeploymentPlan, bool]:
+        local: SquareManifests,
+        server: SquareManifests) -> Tuple[DeploymentPlan, bool]:
     """Return the `DeploymentPlan` to transition K8s to the `local` state.
 
     The deployment plan is a named tuple. It specifies which resources to
     create, patch and delete to ensure that the state of K8s matches that
     specified in `local`.
 
     Inputs:
         config: Square configuration.
         k8sconfig: K8sConfig
-        local: ServerManifests
+        local: SquareManifests
             Should be output from `load_manifest` or `load`.
-        server: ServerManifests
+        server: SquareManifests
             Should be output from `manio.download`.
 
     Returns:
         DeploymentPlan
 
     """
     err_resp = (DeploymentPlan(tuple(), tuple(), tuple()), True)
@@ -298,44 +303,44 @@
         return err_resp
 
     # Replace the server resources fetched from K8s' preferred endpoint with
     # those from the endpoint declared in the local manifest.
     server, err = match_api_version(k8sconfig, local, server)
     assert not err
 
-    # Apply the filters to all local and server manifests before we compute patches.
-    server = {
+    # Strip the unwanted sections from the manifests before we compute patches.
+    stripped_server = {
         meta: manio.strip(k8sconfig, man, config.filters)
         for meta, man in server.items()
-    }                           # type: ignore
-    local = {
+    }
+    stripped_local = {
         meta: manio.strip(k8sconfig, man, config.filters)
         for meta, man in local.items()
-    }                           # type: ignore
+    }
 
     # Abort if any of the manifests could not be stripped.
-    err_srv = {_[2] for _ in server.values()}
-    err_loc = {_[2] for _ in local.values()}
-    if True in err_srv or True in err_loc:
+    err_srv = {_[2] for _ in stripped_server.values()}
+    err_loc = {_[2] for _ in stripped_local.values()}
+    if any(err_srv) or any(err_loc):
         logit.error("Could not strip all manifests.")
         return err_resp
 
-    # Unpack the stripped manifests (first element in the tuple returned from
-    # `manio.strip`).
-    server = {k: dotdict.undo(v[0]) for k, v in server.items()}  # type: ignore
-    local = {k: dotdict.undo(v[0]) for k, v in local.items()}    # type: ignore
+    # Unpack the stripped manifests (ie first element in the tuple returned
+    # by `manio.strip`).
+    server = {k: dotdict.undo(v[0]) for k, v in stripped_server.items()}
+    local = {k: dotdict.undo(v[0]) for k, v in stripped_local.items()}
 
     # Partition the set of meta manifests into create/delete/patch groups.
     plan, err = partition_manifests(local, server)
     if err:
         logit.error("Could not partition the manifests for the plan.")
         return err_resp
 
     # Sanity check: the resources to patch *must* exist in both local and
-    # server manifests. This is a bug if not.
+    # server manifests. If not, we have a bug.
     assert set(plan.patch).issubset(set(local.keys()))
     assert set(plan.patch).issubset(set(server.keys()))
 
     # For later: every DELETE request will have to pass along a `DeleteOptions`
     # manifest (see below).
     del_opts = {
         "apiVersion": "v1",
@@ -356,16 +361,16 @@
 
         # Compile the Delta and add it to the list.
         create.append(DeltaCreate(delta, resource.url, local[delta]))
 
     # Compile the Deltas to delete the excess resources.
     delete = []
     for meta in plan.delete:
-        # Resource URL. Ignore the error flag because the `strip` function
-        # above already called `k8s.resource` and would have aborted on error.
+        # Resource URL. Ignore the error flag because `strip` already called
+        # `k8s.resource` earlier and would have aborted if there was an error.
         resource, err = k8s.resource(k8sconfig, meta)
         assert not err
 
         # Compile the Delta and add it to the list.
         delete.append(DeltaDelete(meta, resource.url, del_opts.copy()))
 
     # Run the local/server manifests through a custom callback function that
@@ -375,22 +380,22 @@
 
     # Iterate over each manifest that needs patching and determine the
     # necessary JSON Patch to transition K8s into the state specified in the
     # local manifests.
     patches = []
     for meta in plan.patch:
         # Compute human readable diff.
-        diff_str, err = manio.diff(config, k8sconfig, local[meta], server[meta])
+        diff_str, err = manio.diff(local[meta], server[meta])
         if err or diff_str is None:
             logit.error(f"Could not compute the diff for <{meta}>.")
             return err_resp
 
         # Compute the JSON patch that will change the K8s state to match the
         # one in the local files.
-        patch, err = make_patch(config, k8sconfig, local[meta], server[meta])
+        patch, err = make_patch(k8sconfig, local[meta], server[meta])
         if err or patch is None:
             logit.error(f"Could not compute the patch for <{meta}>")
             return err_resp
 
         # Append the patch to the list of patches, unless it is empty.
         if len(patch.ops):
             patches.append(DeltaPatch(meta, diff_str, patch))
@@ -622,15 +627,15 @@
     )
     return out, False
 
 
 def valid_label(label: str) -> bool:
     """Return `True` if `label` is K8s and Square compatible.
 
-    The `label` contains both key and value, eg `dh/app=morty`.
+    The `label` contains both key and value, eg `app=square`.
 
     """
     # K8s uses this regex to validate the three individual label components
     # `name`, `part` and `suffix`.
     # Example: "name=part/suffix" -> ("name", "part", "value").
     pat = re.compile(r'^([A-Za-z0-9][-A-Za-z0-9_.]*)?[A-Za-z0-9]$')
 
@@ -741,15 +746,15 @@
         k8sconfig, err = k8s.cluster_config(cfg.kubeconfig, cfg.kubecontext)
         assert not err
 
         # Convert "Selectors.kinds" to their canonical names.
         cfg = translate_resource_kinds(cfg, k8sconfig)
 
         # Load manifests from local files.
-        local, _, err = manio.load(cfg.folder, cfg.selectors)
+        local, _, err = manio.load_manifests(cfg.folder, cfg.selectors)
         assert not err
 
         # Download manifests from K8s.
         server, err = manio.download(cfg, k8sconfig)
         assert not err
 
         # Align non-plannable fields, like the ServiceAccount tokens.
@@ -778,24 +783,25 @@
         k8sconfig, err = k8s.cluster_config(cfg.kubeconfig, cfg.kubecontext)
         assert not err
 
         # Convert "Selectors.kinds" to their canonical names.
         cfg = translate_resource_kinds(cfg, k8sconfig)
 
         # Use a wildcard Selector to ensure `manio.load` will read _all_ local
-        # manifests. This will allow `manio.sync` to modify the ones specified by
-        # the `selector` argument only, delete all the local manifests, and then
-        # write the new ones. This logic will ensure we never have stale manifests
-        # (see `manio.save_files` for details and how `manio.save`, which we call
-        # at the end of this function, uses it).
+        # manifests. This will allow `manio.sync` to modify the ones specified
+        # by the `selector` argument only, delete all the local manifests and
+        # then create the new ones. This logic will ensure we never have stale
+        # manifests. Refer to `manio.save_files` for details and how
+        # `manio.save` uses it.
         load_selectors = Selectors(kinds=k8sconfig.kinds, labels=[], namespaces=[])
 
         # Load manifests from local files.
-        local_meta, local_path, err = manio.load(cfg.folder, load_selectors)
+        local_meta, local_path, err = manio.load_manifests(cfg.folder, load_selectors)
         assert not err
+        del load_selectors
 
         # Download manifests from K8s.
         server, err = manio.download(cfg, k8sconfig)
         assert not err
 
         # Replace the server resources fetched from K8s' preferred endpoint with
         # the one from the endpoint referenced in the local manifest.
```

### Comparing `kubernetes_square-1.3.3/PKG-INFO` & `kubernetes_square-1.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: kubernetes-square
-Version: 1.3.3
+Version: 1.4.0
 Summary: 
 Author: Oliver Nagy
 Author-email: olitheolix@gmail.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff
 Requires-Dist: colorama
 Requires-Dist: colorlog
 Requires-Dist: google
 Requires-Dist: google-api-python-client
 Requires-Dist: jsonpatch
-Requires-Dist: pydantic (>=1.8)
+Requires-Dist: pydantic (>=2.0)
 Requires-Dist: pyyaml
-Requires-Dist: requests
+Requires-Dist: requests (>=2.31)
```

