# Comparing `tmp/mtrain-superclient-0.3.0.tar.gz` & `tmp/mtrain-superclient-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtrain-superclient-0.3.0.tar", max compression
+gzip compressed data, was "mtrain-superclient-0.3.1.tar", max compression
```

## Comparing `mtrain-superclient-0.3.0.tar` & `mtrain-superclient-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1077 2023-03-15 21:57:55.572106 mtrain-superclient-0.3.0/LICENSE
--rw-r--r--   0        0        0     2578 2023-03-15 21:57:55.572372 mtrain-superclient-0.3.0/README.md
--rw-r--r--   0        0        0     2059 2023-07-21 21:46:12.966356 mtrain-superclient-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-07-19 21:36:09.530106 mtrain-superclient-0.3.0/src/mtrain_superclient/__init__.py
--rw-r--r--   0        0        0     6539 2023-07-21 21:43:34.518350 mtrain-superclient-0.3.0/src/mtrain_superclient/__main__.py
--rw-r--r--   0        0        0      712 2023-07-19 21:24:21.644285 mtrain-superclient-0.3.0/src/mtrain_superclient/autoconfig.py
--rw-r--r--   0        0        0    12302 2023-07-11 19:34:52.086842 mtrain-superclient-0.3.0/src/mtrain_superclient/client.py
--rw-r--r--   0        0        0      209 2023-03-15 21:57:55.579228 mtrain-superclient-0.3.0/src/mtrain_superclient/exceptions.py
--rw-r--r--   0        0        0     4985 2023-07-21 17:52:51.991685 mtrain-superclient-0.3.0/src/mtrain_superclient/github_regimens.py
--rw-r--r--   0        0        0     3561 2023-07-21 20:14:32.385644 mtrain-superclient-0.3.0/src/mtrain_superclient/models.py
--rw-r--r--   0        0        0     1089 2023-06-28 19:40:18.564364 mtrain-superclient-0.3.0/src/mtrain_superclient/mtrain_lims.py
--rwxr-xr-x   0        0        0      325 2023-06-28 19:40:18.565151 mtrain-superclient-0.3.0/src/mtrain_superclient/mtrain_lims_upload.sh
--rw-r--r--   0        0        0        0 2023-03-15 21:57:55.579335 mtrain-superclient-0.3.0/src/mtrain_superclient/py.typed
--rw-r--r--   0        0        0     6916 2023-07-21 08:20:55.644089 mtrain-superclient-0.3.0/src/mtrain_superclient/utils.py
--rw-r--r--   0        0        0     3716 2023-07-21 21:50:30.262038 mtrain-superclient-0.3.0/setup.py
--rw-r--r--   0        0        0     3774 2023-07-21 21:50:30.263770 mtrain-superclient-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-15 21:57:55.572106 mtrain-superclient-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2578 2023-03-15 21:57:55.572372 mtrain-superclient-0.3.1/README.md
+-rw-r--r--   0        0        0     2059 2023-07-21 22:26:40.275992 mtrain-superclient-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-07-19 21:36:09.530106 mtrain-superclient-0.3.1/src/mtrain_superclient/__init__.py
+-rw-r--r--   0        0        0     6817 2023-07-21 22:26:10.893921 mtrain-superclient-0.3.1/src/mtrain_superclient/__main__.py
+-rw-r--r--   0        0        0      712 2023-07-19 21:24:21.644285 mtrain-superclient-0.3.1/src/mtrain_superclient/autoconfig.py
+-rw-r--r--   0        0        0    12302 2023-07-11 19:34:52.086842 mtrain-superclient-0.3.1/src/mtrain_superclient/client.py
+-rw-r--r--   0        0        0      209 2023-03-15 21:57:55.579228 mtrain-superclient-0.3.1/src/mtrain_superclient/exceptions.py
+-rw-r--r--   0        0        0     4985 2023-07-21 17:52:51.991685 mtrain-superclient-0.3.1/src/mtrain_superclient/github_regimens.py
+-rw-r--r--   0        0        0     3561 2023-07-21 20:14:32.385644 mtrain-superclient-0.3.1/src/mtrain_superclient/models.py
+-rw-r--r--   0        0        0     1089 2023-06-28 19:40:18.564364 mtrain-superclient-0.3.1/src/mtrain_superclient/mtrain_lims.py
+-rwxr-xr-x   0        0        0      325 2023-06-28 19:40:18.565151 mtrain-superclient-0.3.1/src/mtrain_superclient/mtrain_lims_upload.sh
+-rw-r--r--   0        0        0        0 2023-03-15 21:57:55.579335 mtrain-superclient-0.3.1/src/mtrain_superclient/py.typed
+-rw-r--r--   0        0        0     6916 2023-07-21 08:20:55.644089 mtrain-superclient-0.3.1/src/mtrain_superclient/utils.py
+-rw-r--r--   0        0        0     3716 2023-07-21 22:27:15.132262 mtrain-superclient-0.3.1/setup.py
+-rw-r--r--   0        0        0     3774 2023-07-21 22:27:15.132871 mtrain-superclient-0.3.1/PKG-INFO
```

### Comparing `mtrain-superclient-0.3.0/LICENSE` & `mtrain-superclient-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.3.0/README.md` & `mtrain-superclient-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.3.0/pyproject.toml` & `mtrain-superclient-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mtrain-superclient"
-version = "0.3.0"
+version = "0.3.1"
 description = "Mtrain Superclient"
 authors = ["Christopher Mochizuki <chrism@alleninstitute.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mochic/mtrain-superclient"
 repository = "https://github.com/mochic/mtrain-superclient"
 documentation = "https://mtrain-superclient.readthedocs.io"
```

### Comparing `mtrain-superclient-0.3.0/src/mtrain_superclient/__main__.py` & `mtrain-superclient-0.3.1/src/mtrain_superclient/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,20 +54,27 @@
     auth = Auth.Token(regimen_update_recipie.access_token)
     github_client = Github(auth=auth)
     # regimen = models.Regimen.from_yaml(regimen_yaml)
     with open(regimen_yaml, "r") as f:
         regimen_dict = github_regimens.ruamel_yaml.load(f.read())
     
     # todo add some sorta of fuzzy definition map?
+
     script = regimen_dict.get("_script", None)
     if script is not None and script.startswith("http"):
         regimen_dict["_script_md5"] = utils.generate_script_checksum(script)
     else:
         regimen_dict["_script_md5"] = script
 
+    # ugh...
+    for stage in regimen_dict["stages"].values():
+        if stage.get("script", None) is not None:
+            stage["script"] = script
+            stage["script_md5"] = utils.generate_script_checksum(stage["script"])
+
     # regimen_dict = regimen.model_dump_json()
     regimen_dict["name"] = utils.generate_regimen_version(
         regimen_dict["name"], 
         utils.UpdateType(version_update),
     )
 
     dumped = github_regimens.ruamel_yaml.dump_to_string(
@@ -76,16 +83,16 @@
     regimen = models.Regimen.from_dict(yaml.safe_load(dumped))
 
     response = mtrain_client.add_regimen(
         regimen_dict,
     )
     if not response.status_code in (200, ):
         response.raise_for_status()
-    
-    # logger.debug(regimen.name)
+    # logger.debug(json.dumps(regimen_dict, indent=2))
+    # logger.debug(dumped)
     
     github_regimens.put(
         github_client,
         (regimen, regimen_dict, ),
         regimen_update_recipie.github_repo_name,
         regimen.name.split("_")[0],
     )
```

### Comparing `mtrain-superclient-0.3.0/src/mtrain_superclient/autoconfig.py` & `mtrain-superclient-0.3.1/src/mtrain_superclient/autoconfig.py`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.3.0/src/mtrain_superclient/client.py` & `mtrain-superclient-0.3.1/src/mtrain_superclient/client.py`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.3.0/src/mtrain_superclient/github_regimens.py` & `mtrain-superclient-0.3.1/src/mtrain_superclient/github_regimens.py`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.3.0/src/mtrain_superclient/models.py` & `mtrain-superclient-0.3.1/src/mtrain_superclient/models.py`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.3.0/src/mtrain_superclient/mtrain_lims.py` & `mtrain-superclient-0.3.1/src/mtrain_superclient/mtrain_lims.py`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.3.0/src/mtrain_superclient/utils.py` & `mtrain-superclient-0.3.1/src/mtrain_superclient/utils.py`

 * *Files identical despite different names*

### Comparing `mtrain-superclient-0.3.0/setup.py` & `mtrain-superclient-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'ruamel.yaml>=0.17.32,<0.18.0']
 
 entry_points = \
 {'console_scripts': ['mtrain-superclient = mtrain_superclient.__main__:main']}
 
 setup_kwargs = {
     'name': 'mtrain-superclient',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Mtrain Superclient',
     'long_description': "# Mtrain Superclient\n\n[![PyPI](https://img.shields.io/pypi/v/mtrain-superclient.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/mtrain-superclient.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/mtrain-superclient)][python version]\n[![License](https://img.shields.io/pypi/l/mtrain-superclient)][license]\n\n[![Read the documentation at https://mtrain-superclient.readthedocs.io/](https://img.shields.io/readthedocs/mtrain-superclient/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/mochic/mtrain-superclient/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/mochic/mtrain-superclient/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/mtrain-superclient/\n[status]: https://pypi.org/project/mtrain-superclient/\n[python version]: https://pypi.org/project/mtrain-superclient\n[read the docs]: https://mtrain-superclient.readthedocs.io/\n[tests]: https://github.com/mochic/mtrain-superclient/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/mochic/mtrain-superclient\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Mtrain Superclient_ via [pip] from [PyPI]:\n\n```console\n$ pip install mtrain-superclient\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Mtrain Superclient_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/mochic/mtrain-superclient/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/mochic/mtrain-superclient/blob/main/LICENSE\n[contributor guide]: https://github.com/mochic/mtrain-superclient/blob/main/CONTRIBUTING.md\n[command-line reference]: https://mtrain-superclient.readthedocs.io/en/latest/usage.html\n",
     'author': 'Christopher Mochizuki',
     'author_email': 'chrism@alleninstitute.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mochic/mtrain-superclient',
```

### Comparing `mtrain-superclient-0.3.0/PKG-INFO` & `mtrain-superclient-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtrain-superclient
-Version: 0.3.0
+Version: 0.3.1
 Summary: Mtrain Superclient
 Home-page: https://github.com/mochic/mtrain-superclient
 License: MIT
 Author: Christopher Mochizuki
 Author-email: chrism@alleninstitute.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
```

