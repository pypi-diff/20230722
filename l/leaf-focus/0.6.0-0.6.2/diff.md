# Comparing `tmp/leaf-focus-0.6.0.tar.gz` & `tmp/leaf-focus-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaf-focus-0.6.0.tar", last modified: Sun May 28 10:06:04 2023, max compression
+gzip compressed data, was "leaf-focus-0.6.2.tar", last modified: Sat Jul 22 07:45:29 2023, max compression
```

## Comparing `leaf-focus-0.6.0.tar` & `leaf-focus-0.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.510548 leaf-focus-0.6.0/
--rw-rw-rw-   0        0        0    11558 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/LICENSE
--rw-rw-rw-   0        0        0       73 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3772 2023-05-28 10:06:04.510548 leaf-focus-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2468 2022-12-29 10:38:30.000000 leaf-focus-0.6.0/README.md
--rw-rw-rw-   0        0        0        7 2023-05-28 03:56:32.000000 leaf-focus-0.6.0/VERSION
--rw-rw-rw-   0        0        0     4488 2023-05-28 09:56:14.000000 leaf-focus-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0      458 2023-05-28 03:40:07.000000 leaf-focus-0.6.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      170 2023-05-28 09:41:38.000000 leaf-focus-0.6.0/requirements.txt
--rw-rw-rw-   0        0        0      147 2023-05-28 10:06:04.511549 leaf-focus-0.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.490492 leaf-focus-0.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.498545 leaf-focus-0.6.0/src/leaf_focus/
--rw-rw-rw-   0        0        0      116 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/src/leaf_focus/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-05-28 07:35:10.000000 leaf-focus-0.6.0/src/leaf_focus/app.py
--rw-rw-rw-   0        0        0     3133 2023-05-28 07:45:43.000000 leaf-focus-0.6.0/src/leaf_focus/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.504546 leaf-focus-0.6.0/src/leaf_focus/ocr/
--rw-rw-rw-   0        0        0       46 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/src/leaf_focus/ocr/__init__.py
--rw-rw-rw-   0        0        0    10632 2023-05-28 09:27:03.000000 leaf-focus-0.6.0/src/leaf_focus/ocr/keras_ocr.py
--rw-rw-rw-   0        0        0    14366 2023-05-28 07:42:51.000000 leaf-focus-0.6.0/src/leaf_focus/ocr/model.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.506548 leaf-focus-0.6.0/src/leaf_focus/pdf/
--rw-rw-rw-   0        0        0       45 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/src/leaf_focus/pdf/__init__.py
--rw-rw-rw-   0        0        0    18405 2023-05-28 07:46:32.000000 leaf-focus-0.6.0/src/leaf_focus/pdf/model.py
--rw-rw-rw-   0        0        0    13199 2023-05-28 08:58:13.000000 leaf-focus-0.6.0/src/leaf_focus/pdf/xpdf.py
--rw-rw-rw-   0        0        0     7347 2023-05-28 08:58:13.000000 leaf-focus-0.6.0/src/leaf_focus/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.502546 leaf-focus-0.6.0/src/leaf_focus.egg-info/
--rw-rw-rw-   0        0        0     3772 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      487 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.509547 leaf-focus-0.6.0/tests/
--rw-rw-rw-   0        0        0     3111 2022-12-29 08:57:39.000000 leaf-focus-0.6.0/tests/test_cli.py
--rw-rw-rw-   0        0        0     7477 2023-05-28 07:51:11.000000 leaf-focus-0.6.0/tests/test_keras_ocr.py
--rw-rw-rw-   0        0        0     2191 2023-05-28 07:14:26.000000 leaf-focus-0.6.0/tests/test_utils.py
--rw-rw-rw-   0        0        0     3259 2022-12-29 08:57:39.000000 leaf-focus-0.6.0/tests/test_xpdf_image.py
--rw-rw-rw-   0        0        0     9123 2022-12-29 08:57:39.000000 leaf-focus-0.6.0/tests/test_xpdf_info.py
--rw-rw-rw-   0        0        0     3194 2022-12-29 08:57:39.000000 leaf-focus-0.6.0/tests/test_xpdf_text.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:45:29.126876 leaf-focus-0.6.2/
+-rw-rw-rw-   0        0        0    11558 2022-12-10 10:38:01.000000 leaf-focus-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0       73 2022-12-10 10:38:01.000000 leaf-focus-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3771 2023-07-22 07:45:29.126876 leaf-focus-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2468 2022-12-29 10:38:30.000000 leaf-focus-0.6.2/README.md
+-rw-rw-rw-   0        0        0        7 2023-07-22 06:50:59.000000 leaf-focus-0.6.2/VERSION
+-rw-rw-rw-   0        0        0     4184 2023-07-22 07:28:07.000000 leaf-focus-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0      304 2023-06-24 00:55:34.000000 leaf-focus-0.6.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0      180 2023-07-22 04:31:04.000000 leaf-focus-0.6.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 07:45:29.126876 leaf-focus-0.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 07:45:29.109876 leaf-focus-0.6.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 07:45:29.115876 leaf-focus-0.6.2/src/leaf_focus/
+-rw-rw-rw-   0        0        0      116 2022-12-10 10:38:01.000000 leaf-focus-0.6.2/src/leaf_focus/__init__.py
+-rw-rw-rw-   0        0        0     6215 2023-07-22 04:40:50.000000 leaf-focus-0.6.2/src/leaf_focus/app.py
+-rw-rw-rw-   0        0        0     3104 2023-07-22 04:46:54.000000 leaf-focus-0.6.2/src/leaf_focus/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:45:29.120876 leaf-focus-0.6.2/src/leaf_focus/ocr/
+-rw-rw-rw-   0        0        0       46 2022-12-10 10:38:01.000000 leaf-focus-0.6.2/src/leaf_focus/ocr/__init__.py
+-rw-rw-rw-   0        0        0    10362 2023-07-22 05:04:29.000000 leaf-focus-0.6.2/src/leaf_focus/ocr/keras_ocr.py
+-rw-rw-rw-   0        0        0    14364 2023-07-22 05:07:29.000000 leaf-focus-0.6.2/src/leaf_focus/ocr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:45:29.122876 leaf-focus-0.6.2/src/leaf_focus/pdf/
+-rw-rw-rw-   0        0        0       45 2022-12-10 10:38:01.000000 leaf-focus-0.6.2/src/leaf_focus/pdf/__init__.py
+-rw-rw-rw-   0        0        0    17887 2023-07-22 04:47:49.000000 leaf-focus-0.6.2/src/leaf_focus/pdf/model.py
+-rw-rw-rw-   0        0        0    14325 2023-07-22 06:19:20.000000 leaf-focus-0.6.2/src/leaf_focus/pdf/xpdf.py
+-rw-rw-rw-   0        0        0     8038 2023-07-22 06:22:35.000000 leaf-focus-0.6.2/src/leaf_focus/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 07:45:29.118876 leaf-focus-0.6.2/src/leaf_focus.egg-info/
+-rw-rw-rw-   0        0        0     3771 2023-07-22 07:45:29.000000 leaf-focus-0.6.2/src/leaf_focus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-07-22 07:45:29.000000 leaf-focus-0.6.2/src/leaf_focus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 07:45:29.000000 leaf-focus-0.6.2/src/leaf_focus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-22 07:45:29.000000 leaf-focus-0.6.2/src/leaf_focus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      351 2023-07-22 07:45:29.000000 leaf-focus-0.6.2/src/leaf_focus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-22 07:45:29.000000 leaf-focus-0.6.2/src/leaf_focus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 07:45:29.125877 leaf-focus-0.6.2/tests/
+-rw-rw-rw-   0        0        0     3111 2022-12-29 08:57:39.000000 leaf-focus-0.6.2/tests/test_cli.py
+-rw-rw-rw-   0        0        0     7477 2023-05-28 07:51:11.000000 leaf-focus-0.6.2/tests/test_keras_ocr.py
+-rw-rw-rw-   0        0        0     2191 2023-05-28 07:14:26.000000 leaf-focus-0.6.2/tests/test_utils.py
+-rw-rw-rw-   0        0        0     5763 2023-07-22 06:34:11.000000 leaf-focus-0.6.2/tests/test_xpdf_image.py
+-rw-rw-rw-   0        0        0     9123 2022-12-29 08:57:39.000000 leaf-focus-0.6.2/tests/test_xpdf_info.py
+-rw-rw-rw-   0        0        0     5920 2023-07-22 06:49:59.000000 leaf-focus-0.6.2/tests/test_xpdf_text.py
```

### Comparing `leaf-focus-0.6.0/LICENSE` & `leaf-focus-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.6.0/PKG-INFO` & `leaf-focus-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: leaf-focus
-Version: 0.6.0
+Version: 0.6.2
 Summary: Extract structured text from pdf files.
 Project-URL: Homepage, https://github.com/anotherbyte-net/leaf-focus
 Project-URL: Changelog, https://github.com/anotherbyte-net/leaf-focus/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/anotherbyte-net/leaf-focus
 Project-URL: Tracker, https://github.com/anotherbyte-net/leaf-focus/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `leaf-focus-0.6.0/README.md` & `leaf-focus-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.6.0/pyproject.toml` & `leaf-focus-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [project]
 name = "leaf-focus"
 description = "Extract structured text from pdf files."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Environment :: Console",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -96,15 +96,15 @@
     "src",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
-envlist = py38,py39,py310,py311,py312
+envlist = py38,py39,py310,py311
 
 [testenv]
 #recreate = true
 deps =
     -r requirements.txt
     -r requirements-dev.txt
 allowlist_externals =
@@ -114,15 +114,15 @@
     TEST_INCLUDE_SLOW
 commands =
     echo "::group::Show app help"
     leaf-focus --version
     leaf-focus --help
     echo "::endgroup::"
     echo "::group::Test coverage"
-    python -X dev -m coverage run -m pytest --tb=line --doctest-modules
+    python -X dev -m coverage run -m pytest --doctest-modules
     echo "::endgroup::"
     echo "::group::Coverage report"
     -python -X dev -m coverage report
     echo "::endgroup::"
     echo "::group::Linter - mypy"
     -python -X dev -m mypy src
     echo "::endgroup::"
@@ -131,30 +131,20 @@
     echo "::endgroup::"
     echo "::group::Linter - ruff"
     -python -X dev -m ruff check .
     echo "::endgroup::"
     echo "::group::Linter - pylint"
     -python -X dev -m pylint src
     echo "::endgroup::"
-    echo "::group::Linter - pydocstyle"
-    -python -X dev -m pydocstyle src
-    echo "::endgroup::"
-    echo "::group::Linter - flake8"
-    -python -X dev -m flake8 src --count --show-source --statistics --exit-zero
-    echo "::endgroup::"
     echo "::group::Build"
-    python -m build --sdist --wheel --outdir dist/ .
+    python -m build --sdist --wheel --outdir build/dist-test/{env_name}/ .
     echo "::endgroup::"
 """
 
-[tool.pydocstyle]
-convention = 'google'
-
 [tool.mypy]
-#strict = true
 ignore_missing_imports = true
 check_untyped_defs = true
 no_implicit_optional = true
 
 [tool.ruff]
 line-length = 88
 show-fixes = true
@@ -168,10 +158,9 @@
     "ANN102", # Missing type annotation for `cls` in classmethod
     "ERA001", # commented-out-code
     "RET504", # Unnecessary variable assignment before `return` statement
     "TD002", # Missing author in TODO; try: `# TODO(<author_name>): ...`
     "TD003", # Missing issue link on the line following this TODO
 ]
 
-
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `leaf-focus-0.6.0/src/leaf_focus/app.py` & `leaf-focus-0.6.2/src/leaf_focus/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 """Main application."""
+from __future__ import annotations
+
 import dataclasses
 import datetime
 import logging
-import pathlib
 import typing
 
 from leaf_focus import utils
 from leaf_focus.ocr import keras_ocr
 from leaf_focus.ocr import model as ocr_model
 from leaf_focus.pdf import model as pdf_model
 from leaf_focus.pdf import xpdf
 from leaf_focus.utils import ValidatePathMethod
 
+if typing.TYPE_CHECKING:
+    import pathlib
+
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class AppArgs:
     """Arguments for running the application."""
 
     input_pdf: pathlib.Path
     """path to the pdf file"""
 
     output_dir: pathlib.Path
     """path to the output directory to save text files"""
 
-    first_page: typing.Optional[int] = None
+    first_page: int | None = None
     """the first pdf page to process"""
 
-    last_page: typing.Optional[int] = None
+    last_page: int | None = None
     """the last pdf page to process"""
 
     save_page_images: bool = False
     """save each page of the pdf to a separate image"""
 
     run_ocr: bool = False
     """run OCR over each page of the pdf"""
 
-    log_level: typing.Optional[str] = None
+    log_level: str | None = None
     """the log level"""
 
 
 class App:
     """The main application."""
 
     def __init__(self, exe_dir: pathlib.Path) -> None:
@@ -60,15 +64,15 @@
 
         Args:
             app_args: The application arguments.
 
         Returns:
             bool: True if the text extraction succeeded, otherwise false.
         """
-        timestamp_start = datetime.datetime.utcnow()
+        timestamp_start = datetime.datetime.now(tz=datetime.timezone.utc)
         logger.info("Starting leaf-focus")
 
         input_pdf = utils.validate_path(
             "input pdf",
             app_args.input_pdf,
             ValidatePathMethod.MUST_EXIST,
         )
@@ -102,15 +106,15 @@
         if app_args.save_page_images or app_args.run_ocr:
             xpdf_image = self.pdf_images(xpdf_prog, app_args)
 
         # pdf page image ocr
         if app_args.run_ocr and xpdf_image:
             list(self.pdf_ocr(xpdf_image, app_args))
 
-        timestamp_finish = datetime.datetime.utcnow()
+        timestamp_finish = datetime.datetime.now(tz=datetime.timezone.utc)
         program_duration = timestamp_finish - timestamp_start
         logger.info("Finished (duration %s)", program_duration)
         return True
 
     def pdf_info(
         self,
         prog: xpdf.XpdfProgram,
```

### Comparing `leaf-focus-0.6.0/src/leaf_focus/cli.py` & `leaf-focus-0.6.2/src/leaf_focus/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Command line for leaf focus."""
+from __future__ import annotations
 
 import argparse
 import logging
 import pathlib
 import sys
-import typing
 
 from leaf_focus import app, utils
 
 
-def main(args: typing.Optional[typing.List[str]] = None) -> int:
+def main(args: list[str] | None = None) -> int:
     """Run as a command line program.
 
     Args:
         args: The program arguments.
 
     Returns:
         int: Program exit code.
@@ -95,20 +95,22 @@
             run_ocr=parsed_args.ocr,
             log_level=parsed_args.log_level,
         )
 
         logging.getLogger().setLevel((app_args.log_level or "info").upper())
 
         result = app_inst.run(app_args)
-        return 0 if result is True else 1
+        if result is True:
+            return 0
+        return 1
 
     except utils.LeafFocusError as error:
-        logger.error("Error: %s - %s", error.__class__.__name__, str(error))
+        logger.exception("Error: %s", error.__class__.__name__)
         return 1
 
-    except Exception as error:  # pylint: disable=broad-except
-        logger.error("Error: %s - %s", error.__class__.__name__, str(error))
+    except Exception as error:
+        logger.exception("Error: %s", error.__class__.__name__)
         return 2
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `leaf-focus-0.6.0/src/leaf_focus/ocr/keras_ocr.py` & `leaf-focus-0.6.2/src/leaf_focus/ocr/keras_ocr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """OCR using keras-ocr."""
+from __future__ import annotations
+
 import logging
 import os
-import pathlib
 import typing
 
-import numpy as np
-
 from leaf_focus import utils
 from leaf_focus.ocr import model
 
+if typing.TYPE_CHECKING:
+    import pathlib
+
+    import numpy as np
+
 logger = logging.getLogger(__name__)
 
 
 class OpticalCharacterRecognition:
     """OCR implementation using keras-ocr."""
 
     def __init__(self) -> None:
@@ -38,29 +42,29 @@
             logging.DEBUG: "0",
             logging.INFO: "1",
             logging.WARNING: "2",
             logging.ERROR: "3",
         }
         os.environ["TF_CPP_MIN_LOG_LEVEL"] = tf_log_level_map.get(log_level, "1")
 
-        import tensorflow as tf  # pylint: disable=import-outside-toplevel
+        import tensorflow as tf
 
         # also set the tf logger level
 
         tf.get_logger().setLevel(log_level)
 
         # check the CPU / GPU in use
         gpus = tf.config.list_physical_devices("GPU")
         logger.info("GPUs in use: '%s'.", gpus)
 
         try:
-            import keras_ocr  # pylint: disable=import-outside-toplevel
+            import keras_ocr
         except ModuleNotFoundError as error:
             msg = "Cannot run ocr on this Python version."
-            logger.error(msg)
+            logger.exception(msg)
             raise utils.LeafFocusError(msg) from error
 
         # TODO: allow specifying path to weights files for detector
         # detector_weights_path = ""
         # detector = keras_ocr.detection.Detector(weights=None)
         # detector.model = keras_ocr.detection.build_keras_model(
         #     weights_path=detector_weights_path, backbone_name="vgg"
@@ -83,26 +87,26 @@
             detector=detector,
             recognizer=recognizer,
         )
 
     def engine_run(
         self,
         image_file: pathlib.Path,
-    ) -> typing.Tuple[typing.List, typing.Any]:
+    ) -> tuple[list, typing.Any]:
         """Run the recognition engine.
 
         Args:
             image_file: The path to the image file.
 
         Returns:
             typing.Tuple[typing.List, typing.Any]: The list of images
                 and list of recognition results.
         """
         try:
-            import keras_ocr  # pylint: disable=import-outside-toplevel
+            import keras_ocr
         except ModuleNotFoundError as error:
             msg = "Cannot run ocr on this Python version."
             logger.error(msg)
             raise utils.LeafFocusError(msg) from error
 
         self.engine_create()
 
@@ -112,30 +116,30 @@
             raise utils.LeafFocusError(msg)
 
         images = [keras_ocr.tools.read(str(image_file))]
         return images, self._pipeline.recognize(images)
 
     def engine_annotate(
         self,
-        image: typing.Optional[np.ndarray],
-        predictions: typing.List[typing.Tuple[typing.Any, typing.Any]],
+        image: np.ndarray | None,
+        predictions: list[tuple[typing.Any, typing.Any]],
         axis,
     ) -> None:
         """Run the annotation engine.
 
         Args:
             image: The image data.
             predictions: The recognised text from the image.
             axis: The plot axis for drawing annotations.
 
         Returns:
             None
         """
         try:
-            import keras_ocr  # pylint: disable=import-outside-toplevel
+            import keras_ocr
         except ModuleNotFoundError as error:
             msg = "Cannot run ocr on this Python version."
             logger.error(msg)
             raise utils.LeafFocusError(msg) from error
 
         keras_ocr.tools.drawAnnotations(image=image, predictions=predictions, ax=axis)
 
@@ -205,16 +209,16 @@
             result.items = items
 
         return result
 
     def save_figure(
         self,
         annotation_file: pathlib.Path,
-        image: typing.Optional[np.ndarray],
-        predictions: typing.List[typing.Tuple[typing.Any, typing.Any]],
+        image: np.ndarray | None,
+        predictions: list[tuple[typing.Any, typing.Any]],
     ) -> None:
         """Save the annotated image.
 
         Args:
             annotation_file: The path to the file containing annotations.
             image: The image data.
             predictions: The text recognition results.
@@ -232,32 +236,32 @@
             msg = f"Must supply valid image data, not '{msg_image}'."
             raise utils.LeafFocusError(msg)
         if not predictions:
             predictions = []
 
         logger.info("Saving OCR image to '%s'.", annotation_file)
 
-        import matplotlib as mpl  # pylint: disable=import-outside-toplevel
-        from matplotlib import pyplot as plt  # pylint: disable=import-outside-toplevel
+        import matplotlib as mpl
+        from matplotlib import pyplot as plt
 
         mpl.use("agg")
 
         annotation_file.parent.mkdir(exist_ok=True, parents=True)
 
         fig, axis = plt.subplots(figsize=(20, 20))
 
         self.engine_annotate(image, predictions, axis)
 
         fig.savefig(str(annotation_file))
         plt.close(fig)
 
     def convert_predictions(
         self,
-        predictions: typing.List[typing.Tuple[typing.Any, typing.Any]],
-    ) -> typing.List[typing.List[model.TextItem]]:
+        predictions: list[tuple[typing.Any, typing.Any]],
+    ) -> list[list[model.TextItem]]:
         """Convert predictions to items.
 
         Args:
             predictions: The list of recognised text.
 
         Returns:
             typing.List[typing.List[model.TextItem]]: The equivalent text items.
```

### Comparing `leaf-focus-0.6.0/src/leaf_focus/ocr/model.py` & `leaf-focus-0.6.2/src/leaf_focus/ocr/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
             "top_right_x",
             "top_right_y",
             "bottom_right_x",
             "bottom_right_y",
             "bottom_left_x",
             "bottom_left_y",
         ]
-        with open(path, "w", newline="", encoding="utf8") as file_path:
+        with path.open("w", newline="", encoding="utf8") as file_path:
             writer = csv.DictWriter(file_path, fields)
             writer.writeheader()
             sorted_items = sorted(
                 items,
                 key=lambda i: (i.line_number or 0, i.line_order or 0),
             )
             writer.writerows([dataclasses.asdict(i) for i in sorted_items])
@@ -329,15 +329,15 @@
 
         Returns:
             typing.Generator["TextItem", typing.Any, None]: Items from the file.
         """
         logger.debug("Loading OCR output items.")
         count = 0
 
-        with open(path, encoding="utf8") as file_path:
+        with path.open(encoding="utf8") as file_path:
             reader = csv.DictReader(file_path)
             for row in reader:
                 line_number = row.get("line_number", "").strip()
                 line_number = int(line_number) if line_number else None
 
                 line_order = row.get("line_order", "").strip()
                 line_order = int(line_order) if line_order else None
```

### Comparing `leaf-focus-0.6.0/src/leaf_focus/pdf/model.py` & `leaf-focus-0.6.2/src/leaf_focus/pdf/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,135 @@
 """PDF processing models."""
+from __future__ import annotations
 
 import dataclasses
 import logging
-import pathlib
 import platform
 import typing
-from datetime import datetime
+
+if typing.TYPE_CHECKING:
+    import pathlib
+    from datetime import datetime
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class XpdfArgs:
     """xpdf arguments common to all commands."""
 
-    owner_password: typing.Optional[str] = dataclasses.field(
+    owner_password: str | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-opw", "cmd_type": "single"}},
         default=None,
     )
     """
     Specify the owner password for the PDF file.
     Providing this will bypass all security restrictions.
 
     -opw <string>          : owner password (for encrypted files)
     """
 
-    user_password: typing.Optional[str] = dataclasses.field(
+    user_password: str | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-upw", "cmd_type": "single"}},
         default=None,
     )
     """
     Specify the user password for the PDF file.
 
     -upw <string>          : user password (for encrypted files)
     """
 
-    first_page: typing.Optional[int] = dataclasses.field(
+    first_page: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-f", "cmd_type": "single"}},
         default=None,
     )
     """
     Specifies the first page to convert.
 
     -f <int>               : first page to convert
     """
 
-    last_page: typing.Optional[int] = dataclasses.field(
+    last_page: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-l", "cmd_type": "single"}},
         default=None,
     )
     """
     Specifies the last page to convert.
 
     -l <int>               : last page to convert
     """
 
-    use_verbose: typing.Optional[bool] = dataclasses.field(
+    use_verbose: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-verbose", "cmd_type": "bool"}},
         default=False,
     )
     """
     Print a status message (to stdout) before processing each page.
 
     -verbose               : print per-page status information
     """
 
-    config_file: typing.Optional[pathlib.Path] = dataclasses.field(
+    config_file: pathlib.Path | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-cfg", "cmd_type": "single"}},
         default=None,
     )
     """
     Read config-file in place of ~/.xpdfrc or the system-wide config file.
 
     -cfg <string>     : configuration file to use in place of .xpdfrc
     """
 
-    program_info: typing.Optional[bool] = dataclasses.field(
+    program_info: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-v", "cmd_type": "bool"}},
         default=False,
     )
     """
     Print copyright and version information.
 
     -v                : print copyright and version info
     """
 
 
 @dataclasses.dataclass
 class XpdfInfoArgs(XpdfArgs):
     """Arguments for xpdf pdfinfo program."""
 
-    include_page_bounding_boxes: typing.Optional[bool] = dataclasses.field(
+    include_page_bounding_boxes: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-box", "cmd_type": "bool"}},
         default=False,
     )
     """
     Prints the page box bounding boxes:
     MediaBox, CropBox, BleedBox, TrimBox, and ArtBox.
 
     -box              : print the page bounding boxes
     """
 
-    include_metadata: typing.Optional[bool] = dataclasses.field(
+    include_metadata: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-meta", "cmd_type": "bool"}},
         default=False,
     )
     """
     Prints document-level metadata.
     This is the "Metadata" stream from the PDF file`s Catalog object.
 
     -meta             : print the document metadata (XML)
     """
 
-    include_raw_dates: typing.Optional[bool] = dataclasses.field(
+    include_raw_dates: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-rawdates", "cmd_type": "bool"}},
         default=False,
     )
     """
     Prints the raw (undecoded) date strings, directly from the PDF file.
 
     -rawdates         : print the undecoded date strings directly from the PDF file
     """
 
-    encoding: typing.Optional[str] = dataclasses.field(
+    encoding: str | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-enc", "cmd_type": "single"}},
         default="Latin1",
     )
     """
     Sets the encoding to use for text output.
     The encoding-name must be defined with the unicodeMap command.
     This defaults to "Latin1" (which is a built-in encoding).
@@ -136,138 +139,138 @@
 
 
 @dataclasses.dataclass
 class XpdfInfoResult:
     """Result from xpdf pdfinfo program."""
 
     # pdf info
-    title: typing.Optional[str] = dataclasses.field(
+    title: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Title"}},
     )
-    subject: typing.Optional[str] = dataclasses.field(
+    subject: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Subject"}},
     )
-    keywords: typing.Optional[str] = dataclasses.field(
+    keywords: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Keywords"}},
     )
-    author: typing.Optional[str] = dataclasses.field(
+    author: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Author"}},
     )
-    creator: typing.Optional[str] = dataclasses.field(
+    creator: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Creator"}},
     )
-    producer: typing.Optional[str] = dataclasses.field(
+    producer: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Producer"}},
     )
-    creation_date: typing.Optional[datetime] = dataclasses.field(
+    creation_date: datetime | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "CreationDate"}},
     )
-    modification_date: typing.Optional[datetime] = dataclasses.field(
+    modification_date: datetime | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "ModDate"}},
     )
 
     # addtional info
-    tagged: typing.Optional[bool] = dataclasses.field(
+    tagged: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Tagged"}},
     )
-    form: typing.Optional[str] = dataclasses.field(
+    form: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Form"}},
     )
-    pages: typing.Optional[int] = dataclasses.field(
+    pages: int | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Pages"}},
     )
-    encrypted: typing.Optional[bool] = dataclasses.field(
+    encrypted: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Encrypted"}},
     )
-    page_size: typing.Optional[str] = dataclasses.field(
+    page_size: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Page size"}},
     )
-    media_box: typing.Optional[str] = dataclasses.field(
+    media_box: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "MediaBox"}},
     )
-    crop_box: typing.Optional[str] = dataclasses.field(
+    crop_box: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "CropBox"}},
     )
-    bleed_box: typing.Optional[str] = dataclasses.field(
+    bleed_box: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "BleedBox"}},
     )
-    trim_box: typing.Optional[str] = dataclasses.field(
+    trim_box: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "TrimBox"}},
     )
-    art_box: typing.Optional[str] = dataclasses.field(
+    art_box: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "ArtBox"}},
     )
-    file_size_bytes: typing.Optional[int] = dataclasses.field(
+    file_size_bytes: int | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "File size"}},
     )
-    optimized: typing.Optional[bool] = dataclasses.field(
+    optimized: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Optimized"}},
     )
-    pdf_version: typing.Optional[str] = dataclasses.field(
+    pdf_version: str | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "PDF version"}},
     )
 
     # xml metadata
-    metadata: typing.Optional[dict] = dataclasses.field(
+    metadata: dict | None = dataclasses.field(
         metadata={"leaf_focus": {"name": "Metadata"}},
     )
 
 
 @dataclasses.dataclass
 class XpdfTextArgs(XpdfArgs):
     """Arguments for xpdf pdftotext program."""
 
-    use_original_layout: typing.Optional[bool] = dataclasses.field(
+    use_original_layout: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-layout", "cmd_type": "bool"}},
         default=False,
     )
     """
     Maintain (as best as possible) the original physical layout of the text.
 
     -layout                : maintain original physical layout
     """
 
-    use_simple_layout: typing.Optional[bool] = dataclasses.field(
+    use_simple_layout: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-simple", "cmd_type": "bool"}},
         default=False,
     )
     """
     optimized for simple one-column pages.
     This mode will do a better job of maintaining horizontal spacing,
     but it will only work properly with a single column of text.
 
     -simple                : simple one-column page layout
     """
 
-    use_simple2_layout: typing.Optional[bool] = dataclasses.field(
+    use_simple2_layout: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-simple2", "cmd_type": "bool"}},
         default=False,
     )
     """
     handles slightly rotated text (e.g., OCR output) better.
     Only works for pages with a single column of text.
 
     -simple2               : simple one-column page layout, version 2
     """
 
-    use_table_layout: typing.Optional[bool] = dataclasses.field(
+    use_table_layout: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-table", "cmd_type": "bool"}},
         default=False,
     )
     """
     Table mode is similar to physical layout mode, but optimized for tabular data,
     with the goal of keeping rows and columns aligned
     (at the expense of inserting extra whitespace).
     If the -fixed option is given, character spacing within
     each line will be determined by the specified character pitch.
 
     -table                 : similar to -layout, but optimized for tables
     """
 
-    use_line_printer: typing.Optional[bool] = dataclasses.field(
+    use_line_printer: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-lineprinter", "cmd_type": "bool"}},
         default=False,
     )
     """
     Line printer mode uses a strict fixed-character-pitch and -height layout.
     That is, the page is broken into a grid, and characters are placed into that grid.
     If the grid spacing is too small for the actual characters,
@@ -276,153 +279,153 @@
     The grid spacing can be specified using the -fixed and -linespacing options.
     If one or both are not given on the command line,
     pdftotext will attempt to compute appropriate value(s).
 
     -lineprinter           : use strict fixed-pitch/height layout
     """
 
-    use_raw_string_order: typing.Optional[bool] = dataclasses.field(
+    use_raw_string_order: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-raw", "cmd_type": "bool"}},
         default=False,
     )
     """
     Keep the text in content stream order.
     Depending on how the PDF file was generated, this may or may not be useful.
 
     -raw                   : keep strings in content stream order
     """
 
-    use_text_clip: typing.Optional[bool] = dataclasses.field(
+    use_text_clip: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-clip", "cmd_type": "bool"}},
         default=False,
     )
     """
     Text which is hidden because of clipping is removed before doing layout,
     and then added back in. This can be helpful for tables where
     clipped (invisible) text would overlap the next column.
 
     -clip                  : separate clipped text
     """
 
-    use_no_diag: typing.Optional[bool] = dataclasses.field(
+    use_no_diag: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-nodiag", "cmd_type": "bool"}},
         default=False,
     )
     """
     Diagonal text, i.e., text that is not close to one of
     the 0, 90, 180, or 270 degree axes, is discarded.
     This is useful to skip watermarks drawn on top of body text, etc.
 
     -nodiag                : discard diagonal text
     """
 
-    use_no_page_break: typing.Optional[bool] = dataclasses.field(
+    use_no_page_break: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-nopgbrk", "cmd_type": "bool"}},
         default=False,
     )
     """
     Don't insert a page break (form feed character) at the
     end of each page.
 
     -nopgbrk               : don't insert a page break at the end of each page
     """
 
-    use_bom: typing.Optional[bool] = dataclasses.field(
+    use_bom: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-nom", "cmd_type": "bool"}},
         default=False,
     )
     """
     Insert a Unicode byte order marker (BOM) at the start of the text output.
 
     -bom                   : insert a Unicode BOM at the start of the text file
     """
 
-    use_verbose: typing.Optional[bool] = dataclasses.field(
+    use_verbose: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-verbose", "cmd_type": "bool"}},
         default=False,
     )
     """
     Print a status message (to stdout) before processing each page.
 
     -verbose               : print per-page status information
     """
 
-    fixed_text_number: typing.Optional[int] = dataclasses.field(
+    fixed_text_number: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-fixed", "cmd_type": "single"}},
         default=None,
     )
     """
     Specify the character pitch (character width), in points,
     for physical layout, table, or line printer mode.
     This is ignored in all other modes.
 
     -fixed <number>        : assume fixed-pitch (or tabular) text
     """
 
-    line_space_number: typing.Optional[int] = dataclasses.field(
+    line_space_number: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-linespacing", "cmd_type": "single"}},
         default=None,
     )
     """
     Specify the line spacing, in points, for line printer mode.
     This is ignored in all other modes.
 
     -linespacing <number>  : fixed line spacing for LinePrinter mode
     """
 
-    line_end_type: typing.Optional[str] = dataclasses.field(
+    line_end_type: str | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-eol", "cmd_type": "single"}},
         default=None,
     )
     """
     Sets the end-of-line convention to use for text output.
 
     -eol <string>          : output end-of-line convention (unix, dos, or mac)
     """
 
-    margin_left_number: typing.Optional[int] = dataclasses.field(
+    margin_left_number: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-marginl", "cmd_type": "single"}},
         default=0,
     )
     """
     Specifies the left margin, in points.
     Text in the left margin
     (i.e., within that many points of the left edge of the page) is discarded.
     The default value is zero.
 
     -marginl <number>      : left page margin
     """
 
-    margin_right_number: typing.Optional[int] = dataclasses.field(
+    margin_right_number: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-marginr", "cmd_type": "single"}},
         default=0,
     )
     """
     Specifies the right margin, in points.
     Text in the right margin (i.e., within that many points of the
     right edge of the page) is discarded.
     The default value is zero.
 
     -marginr <number>      : right page margin
     """
 
-    margin_topnumber: typing.Optional[int] = dataclasses.field(
+    margin_topnumber: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-margint", "cmd_type": "single"}},
         default=0,
     )
     """
     Specifies the top margin, in points.
     Text in the top margin (i.e., within that many points of the top
     edge of the page) is discarded.
     The default value is zero.
 
     -margint <number>      : top page margin
     """
 
-    margin_bottom_number: typing.Optional[int] = dataclasses.field(
+    margin_bottom_number: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-marginb", "cmd_type": "single"}},
         default=0,
     )
     """
     Specifies the bottom margin, in points.
     Text in the bottom margin (i.e., within that many points of the
     bottom edge of the page) is discarded.
@@ -457,86 +460,86 @@
     stderr: typing.Collection[str] = dataclasses.field(default_factory=list)
 
 
 @dataclasses.dataclass
 class XpdfImageArgs(XpdfArgs):
     """Arguments for xpdf pdftopng program."""
 
-    resolution: typing.Optional[int] = dataclasses.field(
+    resolution: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-r", "cmd_type": "single"}},
         default=150,
     )
     """
     Specifies the resolution, in DPI. The default is 150 DPI.
 
     -r <number>       : resolution, in DPI (default is 150)
     """
-    use_monochrome: typing.Optional[bool] = dataclasses.field(
+    use_monochrome: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-mono", "cmd_type": "bool"}},
         default=False,
     )
     """
     Generate a monochrome image (instead of a color image).
 
     -mono             : generate a monochrome PNG file
     """
 
-    use_grayscale: typing.Optional[bool] = dataclasses.field(
+    use_grayscale: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-gray", "cmd_type": "bool"}},
         default=False,
     )
     """
     Generate a grayscale image (instead of a color image).
 
     -gray             : generate a grayscale PNG file
     """
-    use_alpha_channel: typing.Optional[bool] = dataclasses.field(
+    use_alpha_channel: bool | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-alpha", "cmd_type": "bool"}},
         default=False,
     )
     """
     Generate an alpha channel in the PNG file.
     This is only useful with PDF files that have been constructed
     with a transparent background.
     The -alpha flag cannot be used with -mono.
 
     -alpha            : include an alpha channel in the PNG file
     """
 
-    rotation: typing.Optional[int] = dataclasses.field(
+    rotation: int | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-rot", "cmd_type": "single"}},
         default=None,
     )
     """
     Rotate pages by 0 (the default), 90, 180, or 270 degrees.
 
     -rot <int>        : set page rotation: 0, 90, 180, or 270
     """
 
-    free_type: typing.Optional[str] = dataclasses.field(
+    free_type: str | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-freetype", "cmd_type": "single"}},
         default="yes",
     )
     """
     Enable or disable FreeType (a TrueType / Type 1 font rasterizer).
     This defaults to "yes".
 
     -freetype <string>: enable FreeType font rasterizer: yes, no
     """
-    anti_aliasing: typing.Optional[str] = dataclasses.field(
+    anti_aliasing: str | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-aa", "cmd_type": "single"}},
         default="yes",
     )
     """
     Enable or disable font anti-aliasing.
     This defaults to "yes".
 
     -aa <string>      : enable font anti-aliasing: yes, no
     """
-    vector_anti_aliasing: typing.Optional[str] = dataclasses.field(
+    vector_anti_aliasing: str | None = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-aaVector", "cmd_type": "single"}},
         default="yes",
     )
     """
     Enable or disable vector anti-aliasing.
     This defaults to "yes".
```

### Comparing `leaf-focus-0.6.0/src/leaf_focus/pdf/xpdf.py` & `leaf-focus-0.6.2/src/leaf_focus/pdf/xpdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 
 logger = logging.getLogger(__name__)
 
 
 class XpdfProgram:
     """Interact with xpdf tools."""
 
-    OPTS_TEXT_ENCODING = [
+    OPTS_TEXT_ENCODING: tuple = (
         "Latin1",
         "ASCII7",
         "Symbol",
         "ZapfDingbats",
         "UTF-8",
         "UCS-2",
-    ]
-    OPTS_TEXT_LINE_ENDING = ["unix", "dos", "mac"]
-    OPTS_IMAGE_ROTATION = [0, 90, 180, 270]
-    OPTS_IMAGE_FREETYPE = ["yes", "no"]
-    OPTS_IMAGE_ANTI_ALIAS = ["yes", "no"]
-    OPTS_IMAGE_VEC_ANTI_ALIAS = ["yes", "no"]
+    )
+    OPTS_TEXT_LINE_ENDING: tuple = ("unix", "dos", "mac")
+    OPTS_IMAGE_ROTATION: tuple = (0, 90, 180, 270)
+    OPTS_IMAGE_FREETYPE: tuple = ("yes", "no")
+    OPTS_IMAGE_ANTI_ALIAS: tuple = ("yes", "no")
+    OPTS_IMAGE_VEC_ANTI_ALIAS: tuple = ("yes", "no")
 
     def __init__(self, directory: pathlib.Path) -> None:
         """Create a new xpdf program class to interact with xpdf tools.
 
         Args:
             directory: The path to the directory containing xpdf tools.
         """
@@ -58,14 +58,16 @@
         Returns:
             The pdf file information.
         """
         # validation
         enc = xpdf_args.encoding
         utils.validate("text encoding", enc, self.OPTS_TEXT_ENCODING)
 
+        utils.validate_pages(xpdf_args.first_page, xpdf_args.last_page)
+
         if not pdf_path.exists():
             msg = f"Pdf file not found '{pdf_path}'."
             raise utils.LeafFocusError(msg) from FileNotFoundError(pdf_path)
 
         output_file = utils.output_root(pdf_path, "info", output_dir)
         output_file = output_file.with_suffix(".json")
 
@@ -91,52 +93,18 @@
             capture_output=True,
             check=True,
             timeout=30,
             text=True,
         )
         lines = result.stdout.splitlines()
 
-        fields_map = {
-            field.metadata.get("leaf_focus", {}).get("name"): field
-            for field in dataclasses.fields(model.XpdfInfoResult)
-        }
-        metadata_line_index: int | None = None
-
-        data: dict[str, typing.Any] = {i.name: None for i in fields_map.values()}
-        for index, line in enumerate(lines):
-            if line.startswith("Metadata:"):
-                metadata_line_index = index
-                break
-
-            value: typing.Any = None
-            key, value = line.split(":", maxsplit=1)
-            key = key.strip()
-
-            field = fields_map.get(key)
-            if not field:
-                raise ValueError(f"Unknown pdf info key '{key}' in '{pdf_path}'.")
-
-            data_key = field.name
-            if data.get(data_key) is not None:
-                raise ValueError(f"Duplicate pdf info key '{key}' in '{pdf_path}'.")
-
-            if field.type == str or str in typing.get_args(field.type):
-                value = value.strip()
-            elif field.type == datetime or datetime in typing.get_args(field.type):
-                value = utils.parse_date(value.strip())
-            elif field.type == bool or bool in typing.get_args(field.type):
-                value = value.strip().lower() == "yes"
-            elif field.type == int or int in typing.get_args(field.type):
-                if data_key == "file_size_bytes":
-                    value = value.replace(" bytes", "")
-                value = int(value.strip().lower())
-            else:
-                raise ValueError(f"Unknown key '{key}' type '{field.type}'")
-
-            data[data_key] = value
+        metadata_line_index, data = self.build_field_metadata(
+            pdf_path,
+            lines,
+        )
 
         # metadata
         if metadata_line_index is not None:
             start = metadata_line_index + 1
             metadata = "\n".join(lines[start:])
             root = ElementTree.fromstring(metadata)
             data["metadata"] = utils.xml_to_element(root).to_dict()
@@ -165,14 +133,16 @@
         Returns:
             The result from running the text extraction program.
         """
         # validation
         eol = xpdf_args.line_end_type
         utils.validate("end of line", eol, self.OPTS_TEXT_LINE_ENDING)
 
+        utils.validate_pages(xpdf_args.first_page, xpdf_args.last_page)
+
         if not pdf_path.exists():
             msg = f"Pdf file not found '{pdf_path}'."
             raise utils.LeafFocusError(msg) from FileNotFoundError(str(pdf_path))
 
         # build command
 
         cmd_args = self.build_cmd(xpdf_args)
@@ -252,14 +222,16 @@
         anti_alias_vec = xpdf_args.anti_aliasing
         utils.validate(
             "vector anti-aliasing",
             anti_alias_vec,
             self.OPTS_IMAGE_VEC_ANTI_ALIAS,
         )
 
+        utils.validate_pages(xpdf_args.first_page, xpdf_args.last_page)
+
         if not pdf_path.exists():
             msg = f"Pdf file not found '{pdf_path}'."
             raise utils.LeafFocusError(msg) from FileNotFoundError(str(pdf_path))
 
         logger.info("Saving each pdf page as an image.")
 
         # build command
@@ -313,15 +285,15 @@
         return model.XpdfImageResult(
             stdout=(result.stdout or "").splitlines(),
             stderr=(result.stderr or "").splitlines(),
             output_dir=output_dir,
             output_files=output_files,
         )
 
-    def build_cmd(self, tool_args):
+    def build_cmd(self, tool_args) -> list[str]:
         """Build the command arguments from a data class."""
         arg_class = tool_args.__class__
         cmd_args = []
         for field in dataclasses.fields(arg_class):
             name = field.name
             value = getattr(tool_args, name)
 
@@ -339,26 +311,31 @@
             if not cmd_type:
                 msg = f"Args incorrectly configured: missing 'cmd_type' for '{name}'."
                 raise ValueError(msg)
 
             # add the arg
             if cmd_type == "bool":
                 if value is not None and value is not True and value is not False:
-                    msg = f"Argument '{name}' must be None, True, or False, not '{value}'."
+                    msg = (
+                        f"Argument '{name}' must be None, True, or False, "
+                        f"not '{value}'."
+                    )
                     raise ValueError(msg)
 
                 if value is True:
                     cmd_args.extend([str(cmd_key)])
 
             elif cmd_type == "single":
                 if field_default is None and value is not None:
                     cmd_args.extend([str(cmd_key), str(value)])
                 elif field_default != value:
                     cmd_args.extend([str(cmd_key), str(value)])
-
+                else:
+                    # no need to add cmd
+                    pass
             else:
                 msg = (
                     f"Argument '{name}' has unknown cmd_type '{cmd_type}'. "
                     "Expected one of 'bool, single'."
                 )
                 raise ValueError(msg)
 
@@ -384,7 +361,62 @@
                 continue
             output_files.append(file_path)
 
         if not output_files:
             logger.warning("No page images found.")
 
         return output_files
+
+    def build_field_metadata(
+        self,
+        pdf_path: pathlib.Path,
+        lines: typing.Iterable[str],
+    ) -> tuple[int | None, dict[str, typing.Any]]:
+        fields_map = {
+            field.metadata.get("leaf_focus", {}).get("name"): field
+            for field in dataclasses.fields(model.XpdfInfoResult)
+        }
+        metadata_line_index: int | None = None
+
+        data: dict[str, typing.Any] = {i.name: None for i in fields_map.values()}
+        for index, line in enumerate(lines):
+            if line.startswith("Metadata:"):
+                metadata_line_index = index
+                break
+
+            value: typing.Any = None
+            key, value = line.split(":", maxsplit=1)
+            key = key.strip()
+
+            field = fields_map.get(key)
+            if not field:
+                msg = f"Unknown pdf info key '{key}' in '{pdf_path}'."
+                raise utils.LeafFocusError(msg)
+
+            data_key = field.name
+            if data.get(data_key) is not None:
+                msg = f"Duplicate pdf info key '{key}' in '{pdf_path}'."
+                raise utils.LeafFocusError(msg)
+
+            typing_arg = typing.get_args(field.type)
+            types_str = [str, "str", "str | None"]
+            types_bool = [bool, "bool", "bool | None"]
+            types_int = [int, "int", "int | None"]
+            types_datetime = [datetime, "datetime", "datetime | None"]
+
+            if field.type in types_str or str in typing_arg:
+                value = value.strip()
+            elif field.type in types_datetime or datetime in typing_arg:
+                value = utils.parse_date(value.strip())
+            elif field.type in types_bool or bool in typing_arg:
+                value = value.strip().lower() == "yes"
+            elif field.type in types_int or int in typing_arg:
+                if data_key == "file_size_bytes":
+                    value = value.replace(" bytes", "")
+                value = int(value.strip().lower())
+            else:
+                msg = f"Unknown key '{key}' type '{field.type}'"
+                raise ValueError(msg)
+
+            data[data_key] = value
+
+        return metadata_line_index, data
```

### Comparing `leaf-focus-0.6.0/src/leaf_focus/utils.py` & `leaf-focus-0.6.2/src/leaf_focus/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Small utility functions."""
 from __future__ import annotations
 
 import dataclasses
 import datetime
 import json
+import logging
 import platform
 import re
 import typing
 import unicodedata
 from enum import Enum
 
 if typing.TYPE_CHECKING:
     import pathlib
     from xml.etree.ElementTree import Element
 
 from importlib_metadata import PackageNotFoundError, distribution
 from importlib_resources import as_file, files
 
+logger = logging.getLogger(__name__)
+
 
 def get_name_dash() -> str:
     """Get the package name with word separated by dashes."""
     return "leaf-focus"
 
 
 def get_name_under() -> str:
@@ -28,18 +31,20 @@
     return "leaf_focus"
 
 
 def get_version() -> str | None:
     """Get the package version."""
     try:
         dist = distribution(get_name_dash())
-        return dist.version
     except PackageNotFoundError:
         pass
 
+    else:
+        return dist.version
+
     try:
         with as_file(files(get_name_under()).joinpath("cli.py")) as file_path:
             return (file_path.parent.parent.parent / "VERSION").read_text().strip()
     except FileNotFoundError:
         pass
 
     return None
@@ -51,27 +56,29 @@
         # e.g. 'Thu Aug 13 11:09:00 2020'
         "%a %b %d %H:%M:%S %Y",
     ]
     for fmt in formats:
         try:
             return datetime.datetime.strptime(value, fmt)
         except ValueError:
-            pass
+            logger.debug("Value '%s' did not match date format '%s'.", value, fmt)
     return None
 
 
-def validate(name: str, value, expected: list) -> None:
+def validate(name: str, value, expected: typing.Iterable[str]) -> None:
     """Validate that a value is one of the expected values."""
     if value is not None and value not in expected:
         opts = ", ".join(sorted([str(i) for i in expected]))
         msg = f"Invalid {name} '{value}'. Expected one of '{opts}'."
         raise LeafFocusError(msg)
 
 
 class ValidatePathMethod(Enum):
+    """Options for how to validate a path."""
+
     NO_OPINION = 0
     MUST_EXIST = 1
 
 
 def validate_path(
     name: str,
     value: pathlib.Path,
@@ -84,19 +91,41 @@
 
     try:
         if must_exist == ValidatePathMethod.MUST_EXIST:
             abs_path = value.resolve(strict=True)
         else:
             abs_path = value.absolute()
 
-        return abs_path
     except Exception as error:
         msg = f"Invalid path '{value}'."
         raise LeafFocusError(msg) from error
 
+    else:
+        return abs_path
+
+
+def validate_pages(first_page: int | None, last_page: int | None) -> None:
+    """Validate the page range.
+
+    Args:
+        first_page: The first page.
+        last_page: The last page.
+
+    Returns:
+        None
+    """
+    if first_page is None or last_page is None:
+        return
+    if first_page > last_page:
+        msg = (
+            f"First page ({first_page}) must be less than or equal "
+            f"to last page ({last_page})."
+        )
+        raise LeafFocusError(msg)
+
 
 def select_exe(value: pathlib.Path) -> pathlib.Path:
     """Select the executable path based on the platform."""
     if platform.system() == "Windows":
         value = value.with_suffix(".exe")
 
     if not value.exists():
@@ -223,18 +252,16 @@
 
 def xml_to_element(element: Element) -> XmlElement:
     """Convert xml into nested dicts."""
     attrib = element.attrib or {}
     tag = element.tag
     text = element.text
     tail = element.tail
-    children = []
 
-    for child in element:
-        children.append(xml_to_element(child))
+    children = [xml_to_element(child) for child in element]
 
     tag_ns, tag_name = xml_tag_ns(tag)
 
     attrib_ns = []
     for key, value in attrib.items():
         extracted_ns, extracted_tag = xml_tag_ns(key)
         attrib_ns.append((extracted_ns, extracted_tag, value))
```

### Comparing `leaf-focus-0.6.0/src/leaf_focus.egg-info/PKG-INFO` & `leaf-focus-0.6.2/src/leaf_focus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: leaf-focus
-Version: 0.6.0
+Version: 0.6.2
 Summary: Extract structured text from pdf files.
 Project-URL: Homepage, https://github.com/anotherbyte-net/leaf-focus
 Project-URL: Changelog, https://github.com/anotherbyte-net/leaf-focus/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/anotherbyte-net/leaf-focus
 Project-URL: Tracker, https://github.com/anotherbyte-net/leaf-focus/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `leaf-focus-0.6.0/src/leaf_focus.egg-info/SOURCES.txt` & `leaf-focus-0.6.2/src/leaf_focus.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 pyproject.toml
 requirements-dev.txt
 requirements.txt
-setup.cfg
 src/leaf_focus/__init__.py
 src/leaf_focus/app.py
 src/leaf_focus/cli.py
 src/leaf_focus/utils.py
 src/leaf_focus.egg-info/PKG-INFO
 src/leaf_focus.egg-info/SOURCES.txt
 src/leaf_focus.egg-info/dependency_links.txt
```

### Comparing `leaf-focus-0.6.0/tests/test_cli.py` & `leaf-focus-0.6.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.6.0/tests/test_keras_ocr.py` & `leaf-focus-0.6.2/tests/test_keras_ocr.py`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.6.0/tests/test_utils.py` & `leaf-focus-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.6.0/tests/test_xpdf_image.py` & `leaf-focus-0.6.2/tests/test_xpdf_image.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import pathlib
 import platform
+import re
 import subprocess
-from importlib_resources import files, as_file
 from subprocess import CompletedProcess
 
 import pytest
-
 from helper import (
     check_skip_slow,
     check_skip_slow_msg,
     check_skip_xpdf_exe_dir,
     check_skip_xpdf_exe_dir_msg,
 )
+from importlib_resources import as_file, files
+
+from leaf_focus import utils
 from leaf_focus.pdf.model import XpdfImageArgs
 from leaf_focus.pdf.xpdf import XpdfProgram
 
 
 @pytest.mark.skipif(check_skip_xpdf_exe_dir(), reason=check_skip_xpdf_exe_dir_msg)
 @pytest.mark.skipif(check_skip_slow(), reason=check_skip_slow_msg)
 def test_xpdf_image_with_exe(capsys, caplog, resource_example1, tmp_path):
@@ -43,16 +45,59 @@
     stdout, stderr = capsys.readouterr()
     assert stdout == ""
     assert stderr == ""
 
     assert caplog.record_tuples == []
 
 
+@pytest.mark.skipif(check_skip_xpdf_exe_dir(), reason=check_skip_xpdf_exe_dir_msg)
+@pytest.mark.skipif(check_skip_slow(), reason=check_skip_slow_msg)
+def test_xpdf_image_valid_pgs_with_exe(capsys, caplog, resource_example1, tmp_path):
+    package = resource_example1.package
+    package_path = files(package)
+    first_page = 3
+    last_page = 25
+    count_pages = 23
+    pdf = resource_example1.pdf_name
+    with as_file(package_path.joinpath(pdf)) as p:
+        pdf_path = p
+
+    output_path = tmp_path / "output-dir"
+    output_path.mkdir(exist_ok=True, parents=True)
+
+    exe_dir = pathlib.Path(os.getenv("TEST_XPDF_EXE_DIR"))
+
+    prog = XpdfProgram(exe_dir)
+    args = XpdfImageArgs(first_page=first_page, last_page=last_page)
+    result = prog.image(pdf_path, output_path, args)
+
+    assert result.output_dir
+    assert len(result.output_files) == count_pages
+
+    output_contents = set()
+    for index, output_file in enumerate(result.output_files):
+        assert output_file.name.endswith(f"-{index + first_page:06}.png")
+
+        output_content = output_file.read_bytes()
+        assert output_content not in output_contents
+        output_contents.add(output_content)
+
+    stdout, stderr = capsys.readouterr()
+    assert stdout == ""
+    assert stderr == ""
+
+    assert caplog.record_tuples == []
+
+
 def test_xpdf_image_without_exe(
-    capsys, caplog, resource_example1, tmp_path, monkeypatch
+    capsys,
+    caplog,
+    resource_example1,
+    tmp_path,
+    monkeypatch,
 ):
     package = resource_example1.package
     package_path = files(package)
     pg = 22
     pdf = resource_example1.pdf_name
     with as_file(package_path.joinpath(pdf)) as p:
         pdf_path = p
@@ -82,24 +127,56 @@
         if cmd == cmd_args:
             return CompletedProcess(
                 args=cmd_args,
                 returncode=0,
                 stdout="",
                 stderr="Config Error: No display font for 'Symbol'\nConfig Error: No display font for 'ZapfDingbats'\n",
             )
-        raise ValueError(f"Unknown cmd '{cmd}'")
+        msg = f"Unknown cmd '{cmd}'"
+        raise ValueError(msg)
 
     monkeypatch.setattr(subprocess, "run", mock_subprocess_run)
 
     prog = XpdfProgram(exe_dir)
     args = XpdfImageArgs(first_page=pg, last_page=pg, use_grayscale=True)
     result = prog.image(pdf_path, output_path, args)
 
     assert result.output_dir == output_path / output_file
 
     stdout, stderr = capsys.readouterr()
     assert stdout == ""
     assert stderr == ""
 
     assert caplog.record_tuples == [
-        ("leaf_focus.pdf.xpdf", 30, "No page images found.")
+        ("leaf_focus.pdf.xpdf", 30, "No page images found."),
     ]
+
+
+@pytest.mark.skipif(check_skip_xpdf_exe_dir(), reason=check_skip_xpdf_exe_dir_msg)
+@pytest.mark.skipif(check_skip_slow(), reason=check_skip_slow_msg)
+def test_xpdf_image_invalid_pgs_with_exe(capsys, caplog, resource_example1, tmp_path):
+    package = resource_example1.package
+    package_path = files(package)
+    first_page = 6
+    last_page = 5
+    pdf = resource_example1.pdf_name
+    with as_file(package_path.joinpath(pdf)) as p:
+        pdf_path = p
+
+    output_path = tmp_path / "output-dir"
+    output_path.mkdir(exist_ok=True, parents=True)
+
+    exe_dir = pathlib.Path(os.getenv("TEST_XPDF_EXE_DIR"))
+
+    prog = XpdfProgram(exe_dir)
+    args = XpdfImageArgs(first_page=first_page, last_page=last_page)
+    with pytest.raises(
+        utils.LeafFocusError,
+        match=re.escape("First page (6) must be less than or equal to last page (5)."),
+    ):
+        prog.image(pdf_path, output_path, args)
+
+    stdout, stderr = capsys.readouterr()
+    assert stdout == ""
+    assert stderr == ""
+
+    assert caplog.record_tuples == []
```

### Comparing `leaf-focus-0.6.0/tests/test_xpdf_info.py` & `leaf-focus-0.6.2/tests/test_xpdf_info.py`

 * *Files identical despite different names*

