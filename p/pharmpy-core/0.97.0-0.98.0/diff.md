# Comparing `tmp/pharmpy-core-0.97.0.tar.gz` & `tmp/pharmpy-core-0.98.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharmpy-core-0.97.0.tar", last modified: Wed Jun 28 07:02:54 2023, max compression
+gzip compressed data, was "pharmpy-core-0.98.0.tar", last modified: Sat Jul 22 10:50:10 2023, max compression
```

## Comparing `pharmpy-core-0.97.0.tar` & `pharmpy-core-0.98.0.tar`

### file list

```diff
@@ -1,1197 +1,1199 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.551107 pharmpy-core-0.97.0/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/LICENSE.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    48318 2023-06-28 07:02:54.551107 pharmpy-core-0.97.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.403094 pharmpy-core-0.97.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/NONMEM.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/Pharmpy_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/Pharmpy_logo_dark.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.403094 pharmpy-core-0.97.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/_ext/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/_ext/pharmpy_snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/allometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/amd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/api_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/api_modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/api_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/api_workflows.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/bootstrap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/cdd.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/covsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/crossval.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/developers.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/estmethod.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/frem.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/iivsearch.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.403094 pharmpy-core-0.97.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/images/Pharmpy_symbol.svg
--rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/images/tools.png
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/iovsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/linearize.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/modelfit.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16627 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/modelsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/nonmem_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/pharmr_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/plots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/psn_resmod.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/psn_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/qa.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/ruvsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/scm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/simeval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/docs/using_r.rst
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-28 07:02:54.551107 pharmpy-core-0.97.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.403094 pharmpy-core-0.97.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.403094 pharmpy-core-0.97.0/src/pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    80641 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.403094 pharmpy-core-0.97.0/src/pharmpy/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/deps/altair.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/deps/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/deps/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/deps/sympy_printing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.403094 pharmpy-core-0.97.0/src/pharmpy/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/code_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.403094 pharmpy-core-0.97.0/src/pharmpy/internals/ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/ds/ordered_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.407094 pharmpy-core-0.97.0/src/pharmpy/internals/expr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/subs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/expr/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.407094 pharmpy-core-0.97.0/src/pharmpy/internals/fn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/fn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/fn/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/fn/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.407094 pharmpy-core-0.97.0/src/pharmpy/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/fs/cwd.py
--rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/fs/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/fs/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/fs/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.371091 pharmpy-core-0.97.0/src/pharmpy/internals/graph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.407094 pharmpy-core-0.97.0/src/pharmpy/internals/graph/directed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/graph/directed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/graph/directed/connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/graph/directed/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/graph/directed/reachability.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.407094 pharmpy-core-0.97.0/src/pharmpy/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/module/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.407094 pharmpy-core-0.97.0/src/pharmpy/internals/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/parse/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/parse/ignored.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/parse/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/parse/prettyprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/parse/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/parse/treeprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.407094 pharmpy-core-0.97.0/src/pharmpy/internals/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/sequence/lcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.407094 pharmpy-core-0.97.0/src/pharmpy/internals/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/set/partitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/set/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/internals/unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.411095 pharmpy-core-0.97.0/src/pharmpy/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    30935 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/datainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.411095 pharmpy-core-0.97.0/src/pharmpy/model/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/distributions/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/distributions/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.411095 pharmpy-core-0.97.0/src/pharmpy/model/external/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.411095 pharmpy-core-0.97.0/src/pharmpy/model/external/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/fcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/fcon/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.411095 pharmpy-core-0.97.0/src/pharmpy/model/external/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/generic/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.411095 pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/ini.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/model_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/name_mangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/sanity_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.411095 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22606 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/advan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/nmtran_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    29064 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.415095 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/abbreviated_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    25255 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/code_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/data_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/etas_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.415095 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/definitions.lark
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/option_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/problem_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/omega_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/problem_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/raw_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/record.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/simulation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/sizes_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/subroutine_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/table_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/theta_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    65273 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.415095 pharmpy-core-0.97.0/src/pharmpy/model/external/rxode/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/rxode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/rxode/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/external/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    73469 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/model/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.419095 pharmpy-core-0.97.0/src/pharmpy/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/blq.py
--rw-r--r--   0 runner    (1001) docker     (123)    17482 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    49871 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    37095 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.423096 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/
--rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/moxo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/moxo.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.tab
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.lst
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.phi
--rw-r--r--   0 runner    (1001) docker     (123)    45809 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)    70962 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/odes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    34944 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/parameter_variability.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    25760 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/modeling/write_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.423096 pharmpy-core-0.97.0/src/pharmpy/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/reporting/altairplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/reporting/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/reporting/custom.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     5634 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/reporting/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.423096 pharmpy-core-0.97.0/src/pharmpy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.423096 pharmpy-core-0.97.0/src/pharmpy/tools/allometry/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/allometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/allometry/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.423096 pharmpy-core-0.97.0/src/pharmpy/tools/amd/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/amd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/amd/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/amd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16449 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/amd/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/bootstrap/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/bootstrap/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/bootstrap/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/cdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/cdd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/covsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/covsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/covsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/covsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/crossval/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/crossval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/crossval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/estmethod/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/estmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/estmethod/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/estmethod/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/estmethod/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/evaldesign/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/evaldesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/evaldesign/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/external/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/external/nlmixr/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/nlmixr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20571 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/nlmixr/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/results_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7225 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/external/rxode/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/rxode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/external/rxode/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.427096 pharmpy-core-0.97.0/src/pharmpy/tools/frem/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/frem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/frem/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/frem/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)    39054 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/frem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/frem/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.431097 pharmpy-core-0.97.0/src/pharmpy/tools/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/funcs/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.431097 pharmpy-core-0.97.0/src/pharmpy/tools/funcs/ml_models/
--rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
--rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/funcs/summarize_individuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.431097 pharmpy-core-0.97.0/src/pharmpy/tools/iivsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/iivsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/iivsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/iivsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.431097 pharmpy-core-0.97.0/src/pharmpy/tools/iovsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/iovsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/iovsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.431097 pharmpy-core-0.97.0/src/pharmpy/tools/linearize/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/linearize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/linearize/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/linearize/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.431097 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.431097 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.431097 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.435097 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/mfl/stringify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.435097 pharmpy-core-0.97.0/src/pharmpy/tools/modelfit/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/modelfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/modelfit/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.435097 pharmpy-core-0.97.0/src/pharmpy/tools/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/modelsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/modelsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/modelsearch/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/psn_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.435097 pharmpy-core-0.97.0/src/pharmpy/tools/qa/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/qa/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    33617 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.435097 pharmpy-core-0.97.0/src/pharmpy/tools/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/ruvsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/ruvsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/ruvsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.435097 pharmpy-core-0.97.0/src/pharmpy/tools/scm/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/scm/psn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27707 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/scm/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.435097 pharmpy-core-0.97.0/src/pharmpy/tools/simeval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/simeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/simeval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.435097 pharmpy-core-0.97.0/src/pharmpy/tools/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/simfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/simfit/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.435097 pharmpy-core-0.97.0/src/pharmpy/tools/structsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/structsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/structsearch/tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/structsearch/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/src/pharmpy/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/src/pharmpy/workflows/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/dispatchers/local_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/src/pharmpy/workflows/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/model_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/model_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/model_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/model_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/src/pharmpy/workflows/tool_database/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/tool_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/tool_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/tool_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/tool_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/src/pharmpy/workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/src/pharmpy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48318 2023-06-28 07:02:54.000000 pharmpy-core-0.97.0/src/pharmpy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    47419 2023-06-28 07:02:54.000000 pharmpy-core-0.97.0/src/pharmpy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 07:02:54.000000 pharmpy-core-0.97.0/src/pharmpy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-28 07:02:54.000000 pharmpy-core-0.97.0/src/pharmpy_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 06:56:11.000000 pharmpy-core-0.97.0/src/pharmpy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-28 07:02:54.000000 pharmpy-core-0.97.0/src/pharmpy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 07:02:54.000000 pharmpy-core-0.97.0/src/pharmpy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/tests/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/deps/test_deps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.439097 pharmpy-core-0.97.0/tests/external/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/external/test_external.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/external/test_nlmixr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/external/test_rxode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.451098 pharmpy-core-0.97.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_evaldesign.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/integration/test_ruvsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.451098 pharmpy-core-0.97.0/tests/internals/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.451098 pharmpy-core-0.97.0/tests/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/internals/fs/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/internals/fs/test_tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.451098 pharmpy-core-0.97.0/tests/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/internals/module/test_lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/internals/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/internals/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.451098 pharmpy-core-0.97.0/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10111 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/model/test_datainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/model/test_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/model/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/model/test_random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/model/test_statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.459099 pharmpy-core-0.97.0/tests/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_blq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)    34423 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_data_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27901 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)    66667 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_odes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_parameter_variability.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/modeling/test_units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.463099 pharmpy-core-0.97.0/tests/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.467100 pharmpy-core-0.97.0/tests/nonmem/output/
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/output/test_nonmem_results_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.471100 pharmpy-core-0.97.0/tests/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_abbreviated.py
--rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_etas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_omega.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_subroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/records/test_theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/test_advan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/test_des.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/test_fcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/test_modelfit_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    35449 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/test_nonmem_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/test_nonmem_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/nonmem/test_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.471100 pharmpy-core-0.97.0/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.471100 pharmpy-core-0.97.0/tests/testdata/frem/
--rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/frem/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.475100 pharmpy-core-0.97.0/tests/testdata/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/DDMODEL00000130
--rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.475100 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.475100 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.479101 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.483101 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/control_stream_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/est_step_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/failed_run.ext
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/failed_run.mod
--rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/no_header_error.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/no_header_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/rounding_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/run_interrupted.ext
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/run_interrupted.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.483101 pharmpy-core-0.97.0/tests/testdata/nonmem/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/fcon/FCON
--rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/fcon/FDATA
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/file.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.387093 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.483101 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/
--rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.483101 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/
--rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.387093 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.483101 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.487101 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/minimal.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.387093 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.487101 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/covariance/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.387093 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/multPROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.387093 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.487101 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.387093 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.387093 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.487101 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
--rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
--rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
--rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
--rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.487101 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.387093 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.491102 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
--rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.491102 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
--rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.495102 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.495102 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
--rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.503103 pharmpy-core-0.97.0/tests/testdata/nonmem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/fviii6.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/fviii6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/fviii6.prn
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox2.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.lst
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.phi
--rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_simulated_log.csv
--rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pef.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pef.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_conc.mod
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_des_assignments.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_dvid.csv
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_dvid.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.coi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.cov
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.lst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.phi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_abbr.mod
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_abbr_comments.mod
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_block.mod
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_etas.mod
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_nm750.mod
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_pd.csv
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_pd.mod
--rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_rate.dta
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.coi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.cor
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.tab
--rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.xml
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.tab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.507103 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/
--rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/boxcox.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/boxcox.lst
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/boxcox.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/boxcox.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/fullblock.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/fullblock.lst
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/fullblock.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/fullblock.phi
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/iov.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/iov.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/iov.mod
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/iov.phi
--rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/resmod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/scm_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/simeval_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/tdist.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/tdist.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/tdist.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/qa/tdist.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.507103 pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mox3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mox3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mox3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mox3.phi
--rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
--rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mytab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.507103 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.507103 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/backward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.511103 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/gofofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/localmin.logf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.511103 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.511103 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.511103 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.511103 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/onlyforward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.511103 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.511103 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/scmplus_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/sdtab1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.515104 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/pheno_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.391093 pharmpy-core-0.97.0/tests/testdata/psn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.515104 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/est_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/est_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/est_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/est_data3.dta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.523105 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/xv_result.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.523105 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.523105 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/frem_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.527105 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
--rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/proposal_density.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.531105 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/command.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.531105 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.531105 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
--rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/results_summary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.531105 pharmpy-core-0.97.0/tests/testdata/psn/resmod_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.531105 pharmpy-core-0.97.0/tests/testdata/psn/resmod_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.531105 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.535106 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.ext
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.phi
--rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
--rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.539106 pharmpy-core-0.97.0/tests/testdata/results/
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/allometry_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/amd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/bootstrap_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/covsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/estmethod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/iivsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/iovsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/linearize_results.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/modelsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/qa_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/ruvsearch_results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.391093 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.391093 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:58:19.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.543106 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.547107 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.547107 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.547107 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.547107 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.551107 pharmpy-core-0.97.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_cdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_crossval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_frem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_linearize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_mfl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_runtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_ruvsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_simeval.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_start_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_structsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_summarize_individuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/tools/test_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.551107 pharmpy-core-0.97.0/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/workflows/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/workflows/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/workflows/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/workflows/test_model_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/workflows/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/workflows/test_tool_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tests/workflows/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-28 06:54:49.000000 pharmpy-core-0.97.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.198306 pharmpy-core-0.98.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    46815 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    48730 2023-07-22 10:50:10.198306 pharmpy-core-0.98.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.102306 pharmpy-core-0.98.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/NONMEM.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/Pharmpy_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/Pharmpy_logo_dark.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.102306 pharmpy-core-0.98.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/_ext/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/_ext/pharmpy_snippet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/allometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/amd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/api_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/api_modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/api_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/api_workflows.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/bootstrap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/cdd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/covsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/crossval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/developers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/estmethod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/frem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/iivsearch.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.102306 pharmpy-core-0.98.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/images/Pharmpy_symbol.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/images/tools.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/iovsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/linearize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/modelfit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16627 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/modelsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/nonmem_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/pharmr_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/plots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/psn_resmod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/psn_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/qa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/ruvsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/scm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/simeval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/docs/using_r.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-22 10:50:10.202306 pharmpy-core-0.98.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3204 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.102306 pharmpy-core-0.98.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.102306 pharmpy-core-0.98.0/src/pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80672 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.102306 pharmpy-core-0.98.0/src/pharmpy/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/deps/altair.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/deps/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/deps/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/deps/sympy_printing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.102306 pharmpy-core-0.98.0/src/pharmpy/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.102306 pharmpy-core-0.98.0/src/pharmpy/internals/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/ds/ordered_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.102306 pharmpy-core-0.98.0/src/pharmpy/internals/expr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/leaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/expr/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/internals/fn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/fn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/fn/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/fn/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/fs/cwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/fs/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/fs/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/fs/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.082306 pharmpy-core-0.98.0/src/pharmpy/internals/graph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/internals/graph/directed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/graph/directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/graph/directed/connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/graph/directed/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/graph/directed/reachability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/module/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/internals/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/parse/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/parse/ignored.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/parse/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/parse/prettyprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/parse/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/parse/treeprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/internals/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/sequence/lcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/internals/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/set/partitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/set/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/internals/unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30947 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/datainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/model/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/distributions/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/distributions/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/model/external/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/model/external/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/fcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/fcon/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/model/external/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/generic/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.106306 pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/model_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/name_mangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/sanity_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.110306 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22606 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/nmtran_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.114306 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/abbreviated_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25255 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/code_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/data_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/etas_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.114306 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/definitions.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/option_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/problem_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/omega_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/problem_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/raw_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/simulation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/sizes_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/subroutine_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/table_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/theta_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68481 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.114306 pharmpy-core-0.98.0/src/pharmpy/model/external/rxode/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/rxode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/rxode/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/external/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74441 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/model/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.114306 pharmpy-core-0.98.0/src/pharmpy/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21351 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51755 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37809 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.118306 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/moxo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/moxo.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.tab
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    47328 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74416 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/odes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34944 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/parameter_variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25760 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/modeling/write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.118306 pharmpy-core-0.98.0/src/pharmpy/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/reporting/altairplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/reporting/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/reporting/custom.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5634 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/reporting/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.118306 pharmpy-core-0.98.0/src/pharmpy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.118306 pharmpy-core-0.98.0/src/pharmpy/tools/allometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/allometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/allometry/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.118306 pharmpy-core-0.98.0/src/pharmpy/tools/amd/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/amd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/amd/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/amd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/amd/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.118306 pharmpy-core-0.98.0/src/pharmpy/tools/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/bootstrap/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/bootstrap/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/bootstrap/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.118306 pharmpy-core-0.98.0/src/pharmpy/tools/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/cdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/cdd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.118306 pharmpy-core-0.98.0/src/pharmpy/tools/covsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/covsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/covsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/covsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.118306 pharmpy-core-0.98.0/src/pharmpy/tools/crossval/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/crossval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/crossval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/estmethod/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/estmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/estmethod/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/estmethod/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/estmethod/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/evaldesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/evaldesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/evaldesign/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/external/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/external/nlmixr/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/nlmixr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20571 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/nlmixr/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/results_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7225 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/external/rxode/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/rxode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/external/rxode/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/frem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/frem/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/frem/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    39054 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/frem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/frem/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/funcs/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/funcs/ml_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/funcs/summarize_individuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/iivsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/iivsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/iivsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/iivsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/iovsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/iovsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/iovsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/linearize/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/linearize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/linearize/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/linearize/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.122306 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/mfl/stringify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/modelfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/modelfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/modelfit/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/modelsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/modelsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/modelsearch/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/psn_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/qa/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33694 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/ruvsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/ruvsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/ruvsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/scm/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/scm/psn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27707 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/scm/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/simeval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/simeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/simeval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/simfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/simfit/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/tools/structsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/structsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/structsearch/pkpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/structsearch/tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/structsearch/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.126306 pharmpy-core-0.98.0/src/pharmpy/workflows/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/dispatchers/local_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/src/pharmpy/workflows/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/model_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/model_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/model_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/model_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/src/pharmpy/workflows/tool_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/tool_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/tool_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/tool_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/tool_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/src/pharmpy/workflows/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/src/pharmpy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48730 2023-07-22 10:50:10.000000 pharmpy-core-0.98.0/src/pharmpy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    47497 2023-07-22 10:50:10.000000 pharmpy-core-0.98.0/src/pharmpy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 10:50:10.000000 pharmpy-core-0.98.0/src/pharmpy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-22 10:50:10.000000 pharmpy-core-0.98.0/src/pharmpy_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 10:43:00.000000 pharmpy-core-0.98.0/src/pharmpy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-22 10:50:10.000000 pharmpy-core-0.98.0/src/pharmpy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 10:50:10.000000 pharmpy-core-0.98.0/src/pharmpy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/tests/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/deps/test_deps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/tests/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/external/test_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/external/test_nlmixr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/external/test_rxode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_evaldesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_ruvsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/integration/test_structsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/tests/internals/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/tests/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/internals/fs/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/internals/fs/test_tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.130306 pharmpy-core-0.98.0/tests/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/internals/module/test_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/internals/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/internals/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.134306 pharmpy-core-0.98.0/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10111 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/model/test_datainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/model/test_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/model/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/model/test_random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/model/test_statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.134306 pharmpy-core-0.98.0/tests/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34423 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_data_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29609 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68275 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_odes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_parameter_variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/modeling/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.134306 pharmpy-core-0.98.0/tests/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.134306 pharmpy-core-0.98.0/tests/nonmem/output/
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/output/test_nonmem_results_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.138306 pharmpy-core-0.98.0/tests/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_abbreviated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_etas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_omega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_subroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/records/test_theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/test_advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/test_fcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/test_modelfit_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35981 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/test_nonmem_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/test_nonmem_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/nonmem/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.138306 pharmpy-core-0.98.0/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.138306 pharmpy-core-0.98.0/tests/testdata/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/frem/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.142306 pharmpy-core-0.98.0/tests/testdata/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/DDMODEL00000130
+-rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.142306 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.142306 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.146306 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.146306 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/control_stream_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/est_step_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/failed_run.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/failed_run.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/no_header_error.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/no_header_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/rounding_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/run_interrupted.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/run_interrupted.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.146306 pharmpy-core-0.98.0/tests/testdata/nonmem/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/fcon/FCON
+-rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/fcon/FDATA
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/file.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.150306 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/
+-rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.150306 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/
+-rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.150306 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.150306 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/minimal.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.150306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/covariance/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/multPROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.150306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.154306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
+-rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.154306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.158306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.158306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
+-rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.158306 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.158306 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.166306 pharmpy-core-0.98.0/tests/testdata/nonmem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/fviii6.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/fviii6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/fviii6.prn
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_simulated_log.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pef.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pef.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_conc.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_des_assignments.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_dvid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_dvid.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_abbr.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_abbr_comments.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_block.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_etas.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_nm750.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_pd.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_pd.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_rate.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.tab
+-rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.tab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/boxcox.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/boxcox.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/boxcox.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/boxcox.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/fullblock.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/fullblock.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/fullblock.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/fullblock.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/iov.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/iov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/iov.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/iov.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/resmod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/scm_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/simeval_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/tdist.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/tdist.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/tdist.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/qa/tdist.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mox3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mox3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mox3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mox3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mytab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/backward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/gofofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/localmin.logf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/onlyforward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.170306 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/scmplus_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/sdtab1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.174306 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/pheno_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/psn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.174306 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/est_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/est_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/est_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/est_data3.dta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.178306 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/xv_result.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.178306 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.178306 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/frem_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.182306 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/proposal_density.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.182306 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/command.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.182306 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.182306 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
+-rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/results_summary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.182306 pharmpy-core-0.98.0/tests/testdata/psn/resmod_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.182306 pharmpy-core-0.98.0/tests/testdata/psn/resmod_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.182306 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.186306 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.190306 pharmpy-core-0.98.0/tests/testdata/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/allometry_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/amd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/bootstrap_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/covsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/estmethod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/iivsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/iovsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/linearize_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/modelsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/qa_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/ruvsearch_results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.190306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.190306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.190306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.094306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.190306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:46:21.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.194306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.194306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.194306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.194306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.194306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.194306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.194306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.194306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.198306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.198306 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
+-rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.198306 pharmpy-core-0.98.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_cdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_crossval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_frem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_mfl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_runtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_ruvsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_simeval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_start_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_structsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_summarize_individuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/tools/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:50:10.198306 pharmpy-core-0.98.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/workflows/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/workflows/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/workflows/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/workflows/test_model_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/workflows/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/workflows/test_tool_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tests/workflows/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-22 10:41:51.000000 pharmpy-core-0.98.0/tox.ini
```

### Comparing `pharmpy-core-0.97.0/AUTHORS.rst` & `pharmpy-core-0.98.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/CHANGELOG.rst` & `pharmpy-core-0.98.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+0.98.0 (2023-07-21)
+-------------------
+
+New features
+============
+
+* Support for multiple doses
+* Add function ``modeling.add_bioavailability``
+* Add function ``modeling.remove_bioavailability``
+* Support for PKPD models in structsearch
+* Option to keep IIVs in IIVSearch
+* Option to test uncertainty methods in Estmethod
+* Autogenerate CMT column
+
+Changes
+=======
+
+* Rename BLQ flag datainfo typ to ``blqdv``
+
 0.97.0 (2023-06-28)
 -------------------
 
 New features
 ============
 
 * Support BLQ transformations in RUVSearch
```

### Comparing `pharmpy-core-0.97.0/CODE_OF_CONDUCT.rst` & `pharmpy-core-0.98.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/LICENSE` & `pharmpy-core-0.98.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/LICENSE.LESSER` & `pharmpy-core-0.98.0/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/MANIFEST.in` & `pharmpy-core-0.98.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/PKG-INFO` & `pharmpy-core-0.98.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.97.0
+Version: 0.98.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -40,14 +40,33 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.98.0 (2023-07-21)
+-------------------
+
+New features
+============
+
+* Support for multiple doses
+* Add function ``modeling.add_bioavailability``
+* Add function ``modeling.remove_bioavailability``
+* Support for PKPD models in structsearch
+* Option to keep IIVs in IIVSearch
+* Option to test uncertainty methods in Estmethod
+* Autogenerate CMT column
+
+Changes
+=======
+
+* Rename BLQ flag datainfo typ to ``blqdv``
+
 0.97.0 (2023-06-28)
 -------------------
 
 New features
 ============
 
 * Support BLQ transformations in RUVSearch
```

### Comparing `pharmpy-core-0.97.0/README.rst` & `pharmpy-core-0.98.0/README.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/NONMEM.rst` & `pharmpy-core-0.98.0/docs/NONMEM.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/Pharmpy_logo.svg` & `pharmpy-core-0.98.0/docs/Pharmpy_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/Pharmpy_logo_dark.svg` & `pharmpy-core-0.98.0/docs/Pharmpy_logo_dark.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/_ext/conversion.py` & `pharmpy-core-0.98.0/docs/_ext/conversion.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/_ext/pharmpy_snippet.py` & `pharmpy-core-0.98.0/docs/_ext/pharmpy_snippet.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/allometry.rst` & `pharmpy-core-0.98.0/docs/allometry.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/amd.rst` & `pharmpy-core-0.98.0/docs/amd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/api.rst` & `pharmpy-core-0.98.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/bootstrap.rst` & `pharmpy-core-0.98.0/docs/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/cdd.rst` & `pharmpy-core-0.98.0/docs/cdd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/cli.rst` & `pharmpy-core-0.98.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/conf.py` & `pharmpy-core-0.98.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'Pharmpy'
 year = '2018-2023'
 authors = ['the Pharmpy development team']
 copyright = '{0}; {1}'.format(year, ', '.join(authors))
-version = release = '0.97.0'
+version = release = '0.98.0'
 html_show_sourcelink = False
 
 pygments_style = 'trac'
 templates_path = ['.']
 
 html_static_path = ['.']
 html_theme = "pydata_sphinx_theme"
```

### Comparing `pharmpy-core-0.97.0/docs/configuration.rst` & `pharmpy-core-0.98.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/contribute.rst` & `pharmpy-core-0.98.0/docs/contribute.rst`

 * *Files 2% similar despite different names*

```diff
@@ -103,21 +103,21 @@
     tox -e py39 -- tests/modeling/test_parameters.py::test_get_thetas
 
 Build and test the documentation
 ********************************
 
 The documentation can be built with::
 
-    tox -e docs
+    tox -e docs-build
 
 The local version of the documentation can now be found in ``dist/docs/``.
 
 Documentation tests are run with::
 
-    tox -e doctest
+    tox -e docs-test
 
 This will test all code given in examples of function documentation and check their output.
 
 Run the integration tests
 *************************
 
 Apart from the unit tests Pharmpy also has a suite of integration tests. The purpose of these
```

### Comparing `pharmpy-core-0.97.0/docs/covsearch.rst` & `pharmpy-core-0.98.0/docs/covsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/crossval.rst` & `pharmpy-core-0.98.0/docs/crossval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/custom.css` & `pharmpy-core-0.98.0/docs/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/data.rst` & `pharmpy-core-0.98.0/docs/data.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/design.rst` & `pharmpy-core-0.98.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/estmethod.rst` & `pharmpy-core-0.98.0/docs/estmethod.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/frem.rst` & `pharmpy-core-0.98.0/docs/frem.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/getting_started.rst` & `pharmpy-core-0.98.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/help_functions.py` & `pharmpy-core-0.98.0/docs/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/iivsearch.rst` & `pharmpy-core-0.98.0/docs/iivsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/images/Pharmpy_symbol.svg` & `pharmpy-core-0.98.0/docs/images/Pharmpy_symbol.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/images/tools.png` & `pharmpy-core-0.98.0/docs/images/tools.png`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/index.rst` & `pharmpy-core-0.98.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/iovsearch.rst` & `pharmpy-core-0.98.0/docs/iovsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/license.rst` & `pharmpy-core-0.98.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/linearize.rst` & `pharmpy-core-0.98.0/docs/linearize.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/model.rst` & `pharmpy-core-0.98.0/docs/model.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/modelfit.rst` & `pharmpy-core-0.98.0/docs/modelfit.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/modeling.rst` & `pharmpy-core-0.98.0/docs/modeling.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/modelsearch.rst` & `pharmpy-core-0.98.0/docs/modelsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/nonmem_plugin.rst` & `pharmpy-core-0.98.0/docs/nonmem_plugin.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/pharmr_logo.svg` & `pharmpy-core-0.98.0/docs/pharmr_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/plots.rst` & `pharmpy-core-0.98.0/docs/plots.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/plugins.rst` & `pharmpy-core-0.98.0/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/projects.rst` & `pharmpy-core-0.98.0/docs/projects.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/qa.rst` & `pharmpy-core-0.98.0/docs/qa.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/ruvsearch.rst` & `pharmpy-core-0.98.0/docs/ruvsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/scm.rst` & `pharmpy-core-0.98.0/docs/scm.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/simeval.rst` & `pharmpy-core-0.98.0/docs/simeval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/tools.rst` & `pharmpy-core-0.98.0/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/docs/using_r.rst` & `pharmpy-core-0.98.0/docs/using_r.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/requirements.txt` & `pharmpy-core-0.98.0/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,83 +4,83 @@
 asttokens==2.2.1
 attrs==23.1.0
 Babel==2.12.1
 backcall==0.2.0
 beautifulsoup4==4.12.2
 bleach==6.0.0
 certifi==2023.5.7
-charset-normalizer==3.1.0
-click==8.1.3
+charset-normalizer==3.2.0
+click==8.1.6
 cloudpickle==2.2.1
 comm==0.1.3
 commonmark==0.9.1
 csscompressor==0.9.5
-dask==2023.6.1
+dask==2023.7.0
 debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
-distributed==2023.6.1
+distributed==2023.7.0
 docutils==0.20.1
 entrypoints==0.4
 executing==1.2.0
 fastjsonschema==2.17.1
 fsspec==2023.6.0
 HeapDict==1.0.1
 idna==3.4
 imagesize==1.4.1
-importlib_metadata==6.7.0
-ipykernel==6.23.3
+importlib_metadata==6.8.0
+ipykernel==6.24.0
 ipython==8.14.0
-ipywidgets==8.0.6
+ipywidgets==8.0.7
 jedi==0.18.2
 Jinja2==3.1.2
 jsonschema==4.17.3
 jupyter-client==8.3.0
 jupyter-core==5.3.1
 jupyter-sphinx==0.4.0
 jupyterlab-pygments==0.2.2
-jupyterlab-widgets==3.0.7
-lark==1.1.5
+jupyterlab-widgets==3.0.8
+lark==1.1.7
 locket==1.0.0
-lxml==4.9.2
+lxml==4.9.3
 MarkupSafe==2.1.3
 matplotlib-inline==0.1.6
 mistune==2.0.5
 mpmath==1.3.0
 msgpack==1.0.5
 nbclient==0.8.0
-nbconvert==7.6.0
-nbformat==5.9.0
+nbconvert==7.7.2
+nbformat==5.9.1
 nest-asyncio==1.5.6
 networkx==3.1
 numexpr==2.8.4
 numpy==1.24.3
 packaging==23.1
 pandas==1.5.3
 pandocfilters==1.5.0
 parso==0.8.3
 partd==1.4.0
 pexpect==4.8.0
 pickleshare==0.7.5
-platformdirs==3.8.0
-prompt-toolkit==3.0.38
+platformdirs==3.9.1
+prompt-toolkit==3.0.39
 psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
 Pygments==2.15.1
 pyreadr==0.4.7
 pyrsistent==0.19.3
 python-dateutil==2.8.2
 pytz==2023.3
 pywin32>=302,!=304; sys_platform == 'win32' and platform_python_implementation != 'PyPy'
-PyYAML==6.0
+PyYAML==6.0.1
 requests==2.31.0
 pyzmq==25.1.0
 rich==13.4.2
-scipy==1.11.0
+scipy==1.11.1
 six==1.16.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 soupsieve==2.4.1
 Sphinx==7.0.1
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
@@ -92,18 +92,18 @@
 symengine==0.10.0
 sympy==1.12
 tblib==2.0.0
 tinycss2==1.2.1
 toolz==0.12.0
 tornado==6.3.2
 traitlets==5.9.0
-urllib3==2.0.3
+urllib3==2.0.4
 wcwidth==0.2.6
 webencodings==0.5.1
-widgetsnbextension==4.0.7
+widgetsnbextension==4.0.8
 zict==3.0.0
-zipp==3.15.0
+zipp==3.16.2
 tflite-runtime==2.12.0; sys_platform == 'linux' and python_version == '3.9'
 tflite_runtime @ https://github.com/hjonnala/snippets/raw/main/wheels/python3.10/tflite_runtime-2.5.0.post1-cp310-cp310-linux_x86_64.whl ; sys_platform == 'linux' and python_version == '3.10'
 --extra-index-url https://google-coral.github.io/py-repo/
 tflite_runtime==2.5.0.post1; sys_platform == 'darwin' and python_version == '3.9'
 tflite_runtime==2.5.0.post1; sys_platform == 'win32' and python_version == '3.9'
```

### Comparing `pharmpy-core-0.97.0/setup.cfg` & `pharmpy-core-0.98.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/setup.py` & `pharmpy-core-0.98.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     txt = re.compile(pat, re.MULTILINE | re.DOTALL).findall(text_str)
     txt = [dedent(block).strip() for block in txt]
     return '\n\n'.join(txt)
 
 
 setup(
     name='pharmpy-core',
-    version='0.97.0',
+    version='0.98.0',
     license='GNU Lesser General Public License v3 (LGPLv3)',
     description='Pharmacometric modeling',
     long_description='%s\n\n%s'
     % (strip_refs(longdesc(read('README.rst'))), strip_refs(read('CHANGELOG.rst'))),
     author='Rikard Nordgren',
     author_email='rikard.nordgren@farmaci.uu.se',
     url='https://pharmpy.github.io',
@@ -77,16 +77,16 @@
         'jsonschema',
         'sphinx',
         'csscompressor',
         'beautifulsoup4',
         'lxml',
         'numpy>=1.17',
         'scipy',
-        'dask>=2022.12.1',
-        'distributed>=2022.12.1',
+        'dask>=2022.12.1, <=2023.7.0',
+        'distributed>=2022.12.1, <=2023.7.0',
         'networkx',
         'appdirs',
         'rich',
         'jupyter-sphinx',
     ],
     extras_require={
         'nlmixr': ["pyreadr"],
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/cli.py` & `pharmpy-core-0.98.0/src/pharmpy/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,15 +659,15 @@
         eps = args.eps
 
     try:
         eta_names = args.eta_names.split(" ")
     except AttributeError:
         eta_names = args.eta_names
 
-    model = set_iiv_on_ruv(model, eps, args.same_eta, eta_names)
+    model = set_iiv_on_ruv(model, list_of_eps=eps, same_eta=args.same_eta, eta_names=eta_names)
 
     write_model_or_dataset(model, model.dataset, path=args.output_file, force=False)
 
 
 def remove_iiv(args):
     """Subcommand to remove IIVs."""
     from pharmpy.modeling import remove_iiv
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/config.py` & `pharmpy-core-0.98.0/src/pharmpy/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/deps/__init__.py` & `pharmpy-core-0.98.0/src/pharmpy/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/deps/altair.py` & `pharmpy-core-0.98.0/src/pharmpy/deps/altair.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/df.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/df.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/ds/ordered_set.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/ds/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/expr/eval.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/expr/eval.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/expr/funcs.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/expr/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/expr/leaves.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/expr/leaves.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/expr/ode.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/expr/ode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/expr/subs.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/expr/subs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/expr/tree.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/expr/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/expr/units.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/expr/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/fn/signature.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/fn/signature.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/fn/type.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/fn/type.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/fs/lock.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/fs/lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/fs/path.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/fs/path.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/fs/tmp.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/fs/tmp.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/graph/directed/connected_components.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/graph/directed/connected_components.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/immutable.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/immutable.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/math.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/module/lazy.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/module/lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/parse/generic.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/parse/generic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/parse/ignored.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/parse/ignored.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from importlib.metadata import version
 from typing import Iterable, Iterator, List, Tuple, Union
 
 from lark import Token, Transformer, Tree
 from lark.tree import Meta
 
 WS = {' ', '\x00', '\t'}
 LF = {'\r', '\n'}
@@ -44,23 +45,33 @@
         i = head
 
 
 def _item_range(x: Union[Tree, Token]) -> Tuple[int, int]:
     if isinstance(x, Tree):
         i = x.meta.start_pos
         j = x.meta.end_pos
+        if version('lark') == '1.1.6':
+            j = _get_new_end_pos(x)
     else:
         i = x.start_pos
         j = x.end_pos
 
     assert isinstance(i, int)
     assert isinstance(j, int)
     return (i, j)
 
 
+def _get_new_end_pos(x):
+    # FIXME: temporary workaround, see https://github.com/lark-parser/lark/issues/1304
+    x = x.children[-1]
+    if isinstance(x, Token):
+        return x.end_pos
+    return _get_new_end_pos(x)
+
+
 def _interleave_ignored(source: str, it: Iterator[Union[Tree, Token]]):
     x = next(it)
     yield x
 
     i = _item_range(x)[1]
 
     x = next(it)
@@ -92,14 +103,17 @@
         new_children = interleave_ignored(self.source, children)
         return Tree(data, new_children, meta)
 
 
 def with_ignored_tokens(source, tree):
     new_tree = InterleaveIgnored(source).transform(tree)
 
+    if version('lark') == '1.1.6' and new_tree.children:
+        new_tree.meta.end_pos = _get_new_end_pos(new_tree)
+
     final_meta = Meta()
     # TODO propagate line/column information
     final_meta.start_pos = 0
     final_meta.end_pos = len(source)
     final_meta.empty = False
 
     final_children: List[Union[Tree, Token]] = (
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/parse/missing.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/parse/missing.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/parse/prettyprint.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/parse/prettyprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/parse/tree.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/parse/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/parse/treeprint.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/parse/treeprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/sequence/lcs.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/sequence/lcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/set/partitions.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/set/partitions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/set/subsets.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/set/subsets.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/internals/unicode.py` & `pharmpy-core-0.98.0/src/pharmpy/internals/unicode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/__init__.py` & `pharmpy-core-0.98.0/src/pharmpy/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/data.py` & `pharmpy-core-0.98.0/src/pharmpy/model/data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/datainfo.py` & `pharmpy-core-0.98.0/src/pharmpy/model/datainfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         'ss',
         'event',
         'covariate',
         'mdv',
         'compartment',
         'admid',
         'lloq',
-        'blq',
+        'blqdv',
     )
     _all_scales = ('nominal', 'ordinal', 'interval', 'ratio')
     _all_dtypes = (
         'int8',
         'int16',
         'int32',
         'int64',
@@ -311,15 +311,15 @@
         ii            Interdose interval
         ss            Steady state dosing
         event         0 = observation
         mdv           0 = DV is observation value, 1 = DV is missing
         admid         Administration ID
         compartment   Compartment information (not yet exactly specified)
         lloq          Lower limit of quantification
-        blq           Below limit of quantification
+        blqdv         Below limit of quantification indicator
         unknown       Unkown type. This will be the default for columns that hasn't been
                       assigned a type
         ============  =============
         """
         return self._type
 
     @property
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/distributions/numeric.py` & `pharmpy-core-0.98.0/src/pharmpy/model/distributions/numeric.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/distributions/symbolic.py` & `pharmpy-core-0.98.0/src/pharmpy/model/distributions/symbolic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/estimation.py` & `pharmpy-core-0.98.0/src/pharmpy/model/estimation.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 class EstimationStep(Immutable):
     """Definition of one estimation operation"""
 
     """Supported estimation methods
     """
     supported_methods = frozenset(('FO', 'FOCE', 'ITS', 'IMPMAP', 'IMP', 'SAEM', 'BAYES'))
     supported_solvers = frozenset(('CVODES', 'DGEAR', 'DVERK', 'IDA', 'LSODA', 'LSODI'))
+    supported_covs = frozenset(('SANDWICH', 'CPG', 'OFIM'))
 
     def __init__(
         self,
         method,
         interaction=False,
-        cov=False,
+        cov=None,
         evaluation=False,
         maximum_evaluations=None,
         laplace=False,
         isample=None,
         niter=None,
         auto=None,
         keep_every_nth_iter=None,
@@ -56,15 +57,15 @@
         self._epsilon_derivatives = epsilon_derivatives
 
     @classmethod
     def create(
         cls,
         method,
         interaction=False,
-        cov=False,
+        cov=None,
         evaluation=False,
         maximum_evaluations=None,
         laplace=False,
         isample=None,
         niter=None,
         auto=None,
         keep_every_nth_iter=None,
@@ -88,14 +89,20 @@
             residuals = ()
         else:
             residuals = tuple(residuals)
         if predictions is None:
             predictions = ()
         else:
             predictions = tuple(predictions)
+        if cov is not None:
+            cov = cov.upper()
+        if not (cov is None or cov in EstimationStep.supported_covs):
+            raise ValueError(
+                f"Unknown cov {cov}. Recognized covs are {sorted(EstimationStep.supported_covs)}."
+            )
         if solver is not None:
             solver = solver.upper()
         if not (solver is None or solver in EstimationStep.supported_solvers):
             raise ValueError(
                 f"Unknown solver {solver}. Recognized solvers are {sorted(EstimationStep.supported_solvers)}."
             )
         if tool_options is None:
@@ -165,15 +172,27 @@
     @property
     def evaluation(self):
         """Only perform model evaluation"""
         return self._evaluation
 
     @property
     def cov(self):
-        """Should the parameter uncertainty be estimated?"""
+        """Method to use when estimating parameter uncertainty
+        Supported methods and their corresponding NMTRAN code:
+
+        +----------------------------+------------------+
+        | Method                     | NMTRAN           |
+        +============================+==================+
+        | Sandwich                   | $COV             |
+        +----------------------------+------------------+
+        | Cross-product gradient     | $COV MATRIX=S    |
+        +----------------------------+------------------+
+        | Observed FIM               | $COV MATRIX=R    |
+        +----------------------------+------------------+
+        """
         return self._cov
 
     @property
     def laplace(self):
         """Use the laplacian method"""
         return self._laplace
 
@@ -314,22 +333,24 @@
 
     @classmethod
     def from_dict(cls, d):
         d['tool_options'] = frozenmapping(d['tool_options'])
         return cls(**d)
 
     def __repr__(self):
+        cov = f"'{self.cov}'" if self.cov is not None else self.cov
+        solver = f"'{self.solver}'" if self.solver is not None else self.solver
         return (
-            f'EstimationStep("{self.method}", interaction={self.interaction}, '
-            f'cov={self.cov}, evaluation={self.evaluation}, '
-            f'maximum_evaluations={self.maximum_evaluations}, laplace={self.laplace}, '
-            f'isample={self.isample}, niter={self.niter}, auto={self.auto}, '
-            f'keep_every_nth_iter={self.keep_every_nth_iter}, solver={self.solver}, '
-            f'solver_rtol={self.solver_rtol}, solver_atol={self.solver_atol}, '
-            f'tool_options={self.tool_options})'
+            f"EstimationStep('{self.method}', interaction={self.interaction}, "
+            f"cov={cov}, evaluation={self.evaluation}, "
+            f"maximum_evaluations={self.maximum_evaluations}, laplace={self.laplace}, "
+            f"isample={self.isample}, niter={self.niter}, auto={self.auto}, "
+            f"keep_every_nth_iter={self.keep_every_nth_iter}, solver={solver}, "
+            f"solver_rtol={self.solver_rtol}, solver_atol={self.solver_atol}, "
+            f"tool_options={self.tool_options})"
         )
 
 
 class EstimationSteps(Sequence, Immutable):
     """A sequence of estimation steps
 
     Parameters
@@ -410,16 +431,16 @@
         -------
         pd.DataFrame
             DataFrame overview
 
         >>> from pharmpy.modeling import load_example_model
         >>> model = load_example_model("pheno")
         >>> model.estimation_steps.to_dataframe()   # doctest: +ELLIPSIS
-          method  interaction   cov  ...  auto keep_every_nth_iter  tool_options
-        0   FOCE         True  True  ...  None                None            {}
+          method  interaction       cov  ...  auto keep_every_nth_iter  tool_options
+        0   FOCE         True  SANDWICH  ...  None                None            {}
         """
         method = [s.method for s in self._steps]
         interaction = [s.interaction for s in self._steps]
         cov = [s.cov for s in self._steps]
         evaluation = [s.evaluation for s in self._steps]
         maximum_evaluations = [s.maximum_evaluations for s in self._steps]
         laplace = [s.laplace for s in self._steps]
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/fcon/model.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/fcon/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/generic/generic.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/generic/generic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/error_model.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/error_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/ini.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/ini.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/model.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/model_block.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/model_block.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nlmixr/sanity_checks.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nlmixr/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/advan.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/advan.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/dataset.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/dataset.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/model.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/nmtran_parser.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/nmtran_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/parsing.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,15 @@
         elif value == '1' or value == 'CONDITIONAL' or value == 'COND':
             name = 'foce'
         else:
             name = value
         interaction = False
         evaluation = False
         maximum_evaluations = None
-        cov = False
+        cov = None
         laplace = False
         isample = None
         niter = None
         auto = None
         keep_every_nth_iter = None
 
         if record.has_option('INTERACTION') or record.has_option('INTER'):
@@ -392,15 +392,15 @@
                 evaluation = True
             else:
                 maximum_evaluations = int(maxeval_opt)
         eval_opt = record.get_option('EONLY')
         if eval_opt is not None and int(eval_opt) == 1:
             evaluation = True
         if covrec:
-            cov = True
+            cov = 'SANDWICH'
         if record.has_option('LAPLACIAN') or record.has_option('LAPLACE'):
             laplace = True
         if record.has_option('ISAMPLE'):
             isample = int(record.get_option('ISAMPLE'))
         if record.has_option('NITER'):
             niter = int(record.get_option('NITER'))
         if record.has_option('AUTO'):
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/abbreviated_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/abbreviated_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/code_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/code_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/data_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/data_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/factory.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/model_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/omega_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/omega_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/option_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/option_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/parsers.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/parsers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/problem_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/problem_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/sizes_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/sizes_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/subroutine_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/subroutine_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/table_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/table_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/records/theta_record.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/records/theta_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/table.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/nonmem/update.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/nonmem/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import re
-import warnings
 from itertools import product
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional
 
 from pharmpy.deps import numpy as np
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy, sympy_printing
@@ -24,15 +23,16 @@
     Parameter,
     Parameters,
     RandomVariables,
     Statements,
     data,
     output,
 )
-from pharmpy.modeling import get_ids, simplify_expression
+from pharmpy.model.model import update_datainfo
+from pharmpy.modeling import get_admid, get_ids, simplify_expression
 
 from .records.parsers import CodeRecordParser
 
 if TYPE_CHECKING:
     from .model import Model
 
 from .nmtran_parser import NMTranControlStream
@@ -369,35 +369,97 @@
 def update_ode_system(model: Model, old: Optional[CompartmentalSystem], new: CompartmentalSystem):
     """Update ODE system
 
     Handle changes from to CompartmentSystem
     """
     if old is None:
         old = CompartmentalSystem(CompartmentalSystemBuilder())
-
     model = update_lag_time(model, old, new)
+    model = update_bio(model, old, new)
+    model, updated_dataset = update_cmt_column(model, old, new)
 
     advan, trans, nonlin, haszo = new_advan_trans(model)
 
     if nonlin or haszo:
         model = to_des(model, new)
     else:
-        if isinstance(new.dosing_compartment.dose, Bolus) and 'RATE' in model.datainfo.names:
+        if isinstance(new.dosing_compartment[0].dose, Bolus) and 'RATE' in model.datainfo.names:
             df = model.dataset.drop(columns=['RATE'])
             model = model.replace(dataset=df)
 
         model = pk_param_conversion(model, advan=advan, trans=trans)
         model = add_needed_pk_parameters(model, advan, trans)
         model = update_subroutines_record(model, advan, trans)
         model = update_model_record(model, advan)
 
         if not is_nonlinear_odes(model):
             model = from_des(model, advan)
 
-    model, updated_dataset = update_infusion(model, old)
+    if not updated_dataset:
+        model, updated_dataset = update_infusion(model, old)
+    else:
+        model, _ = update_infusion(model, old)
+    return model, updated_dataset
+
+
+def update_cmt_column(model, old, new):
+    if model.dataset is not None:
+        if (
+            "admid" in model.datainfo.types
+            and len(model.dataset[model.datainfo.typeix["admid"].names[0]].unique()) != 1
+        ):
+            cs = model.statements.ode_system
+            newmap = new_compartmental_map(cs)
+
+            d = {}
+            for dose_comp in model.statements.ode_system.dosing_compartment:
+                d[dose_comp.dose.admid] = newmap[dose_comp.name]
+
+            cmt_col = get_admid(model)
+            cmt_col = cmt_col.replace(d)
+
+            dataset = model.dataset.copy()
+            dataset['CMT'] = cmt_col
+            di = update_datainfo(model.datainfo, dataset)
+            colinfo = di['CMT'].replace(type='compartment')
+            model = model.replace(datainfo=di.set_column(colinfo), dataset=dataset)
+
+            updated_dataset = True
+        elif "CMT" in model.datainfo.names and len(old.compartment_names) != len(
+            new.compartment_names
+        ):
+            dataset = model.dataset.copy()
+
+            # Make sure column is a number and not string
+            dataset["CMT"] = pd.to_numeric(dataset["CMT"])
+
+            # Differ in amount of compartment -> Change cmt numbering
+            # The cmt number should be the same as the dosing compartment
+            oldmap = model.internals.compartment_map
+            assert oldmap is not None
+            cs = model.statements.ode_system
+            newmap = new_compartmental_map(cs)
+            oldmap = oldmap.copy()
+            remap = create_compartment_remap(oldmap, newmap)
+
+            for dose_comp in old.dosing_compartment:
+                if dose_comp != old.central_compartment:
+                    # Remap oral doses to new dosing compartment
+                    remap[oldmap[dose_comp.name]] = newmap[new.dosing_compartment[0].name]
+
+            dataset = dataset.replace({"CMT": remap})
+            model = model.replace(dataset=dataset)
+
+            updated_dataset = True
+        else:
+            # Could verify that the cmt column is the same
+            updated_dataset = False
+    else:
+        updated_dataset = False
+
     return model, updated_dataset
 
 
 def is_nonlinear_odes(model: Model):
     """Check if ode system is nonlinear"""
     odes = model.statements.ode_system
     M = odes.compartmental_matrix
@@ -410,27 +472,29 @@
     return not all(a == 0 for a in zo)
 
 
 def update_infusion(model: Model, old: ODESystem):
     statements = model.statements
     new = statements.ode_system
     assert new is not None
-    if isinstance(new.dosing_compartment.dose, Infusion) and not statements.find_assignment('D1'):
+    if isinstance(new.dosing_compartment[0].dose, Infusion) and not statements.find_assignment(
+        'D1'
+    ):
         # Handle direct moving of Infusion dose
         statements = statements.subs({'D2': 'D1'})
 
-    if isinstance(new.dosing_compartment.dose, Infusion) and isinstance(
-        old.dosing_compartment.dose, Bolus
+    if isinstance(new.dosing_compartment[0].dose, Infusion) and isinstance(
+        old.dosing_compartment[0].dose, Bolus
     ):
-        dose = new.dosing_compartment.dose
+        dose = new.dosing_compartment[0].dose
         if dose.rate is None:
             # FIXME: Not always D1 here!
             ass = Assignment(sympy.Symbol('D1'), dose.duration)
             cb = CompartmentalSystemBuilder(new)
-            cb.set_dose(new.dosing_compartment, Infusion(dose.amount, duration=ass.symbol))
+            cb.set_dose(new.dosing_compartment[0], Infusion(dose.amount, duration=ass.symbol))
             statements = statements.before_odes + CompartmentalSystem(cb) + statements.after_odes
         else:
             raise NotImplementedError("First order infusion rate is not yet supported")
         statements = statements.before_odes + ass + statements.ode_system + statements.after_odes
         dataset = model.dataset.copy()
         rate = np.where(dataset['AMT'] == 0, 0.0, -2.0)
         dataset['RATE'] = rate
@@ -522,15 +586,15 @@
     newdes = des.from_odes(new, to_odes)
     cs = cs.replace_records([des], [newdes])
     cs = cs.remove_records(model.internals.control_stream.get_records('MODEL'))
     mod = create_record('$MODEL\n')
     cs = cs.insert_record(mod)
     old_mod = mod
     assert isinstance(mod, ModelRecord)
-    dosecmt_name = new.dosing_compartment.name
+    dosecmt_name = new.dosing_compartment[0].name
     for eq in new.eqs:
         name = eq.lhs.args[0].name[2:]
         if name == dosecmt_name:
             dose = True
         else:
             dose = False
         mod = mod.add_compartment(name, dosing=dose)
@@ -573,22 +637,14 @@
 
     if old == new and old_solver == new_solver:
         return model, updated_dataset
 
     if new_odes is not None:
         old_odes = old.ode_system
         if new_odes != old_odes:
-            colnames, drop, _, _ = parse_column_info(model.internals.control_stream)
-            col_dropped = dict(zip(colnames, drop))
-            if 'CMT' in col_dropped.keys() and not col_dropped['CMT']:
-                warnings.warn(
-                    'Compartment structure has been updated, CMT-column '
-                    'in dataset might not be relevant anymore. Check '
-                    'CMT-column or drop column'
-                )
             model, updated_dataset = update_ode_system(model, old_odes, new_odes)
         else:
             if new_solver:
                 if new_solver != old_solver:
                     advan = solver_to_advan(new_solver)
                     subs = model.internals.control_stream.get_records('SUBROUTINES')[0]
                     newsubs = subs.set_advan(advan)
@@ -602,15 +658,14 @@
         keep = []
         for s in main_statements:
             if model.statements.ode_system.t not in s.free_symbols:
                 keep.append(s)
         main_statements = Statements(tuple(keep))
 
     error_statements = model.statements.after_odes
-
     rec = model.internals.control_stream.get_pred_pk_record()
     newrec = rec.update_statements(main_statements.subs(trans), model.random_variables, trans)
     newcs = model.internals.control_stream.replace_records([rec], [newrec])
     model = model.replace(internals=model.internals.replace(control_stream=newcs))
 
     error = model.internals.control_stream.get_error_record()
     if not error and len(error_statements) > 0:
@@ -698,30 +753,53 @@
         cs = cs.replace_records([rec], [new_rec])
         internals = model.internals.replace(control_stream=cs)
         model = model.replace(internals=internals)
     return model
 
 
 def update_lag_time(model: Model, old: CompartmentalSystem, new: CompartmentalSystem):
-    new_dosing = new.dosing_compartment
+    new_dosing = new.dosing_compartment[0]
     new_lag_time = new_dosing.lag_time
-    old_lag_time = old.dosing_compartment.lag_time
+    old_lag_time = old.dosing_compartment[0].lag_time
     if new_lag_time != old_lag_time and new_lag_time != 0:
         ass = Assignment(sympy.Symbol('ALAG1'), new_lag_time)
         cb = CompartmentalSystemBuilder(new)
         cb.set_lag_time(new_dosing, ass.symbol)
         model = model.replace(
             statements=model.statements.before_odes
             + ass
             + CompartmentalSystem(cb)
             + model.statements.after_odes
         )
     return model
 
 
+def update_bio(model, old, new):
+    """
+    Update all bioavailability statements to match the numbering of the
+    compartments in NONMEM.
+    Is based on the order of dosing compartments
+    """
+    newmap = new_compartmental_map(new)
+    for dose in new.dosing_compartment:
+        # If the dose is not already correctly set (i.e dose numbering has
+        # changed), it should be update to match the new number.
+        if (
+            not isinstance(dose.bioavailability, sympy.Number)
+            and dose.bioavailability != f'F{newmap[dose.name]}'
+        ):
+            model = model.replace(
+                statements=model.statements.subs(
+                    {sympy.Symbol(f'{dose.bioavailability}'): sympy.Symbol(f'F{newmap[dose.name]}')}
+                )
+            )
+
+    return model
+
+
 def new_compartmental_map(cs: CompartmentalSystem):
     """Create compartmental map for updated model
     cs - new compartmental system
     """
     compmap = {name: i for i, name in enumerate(cs.compartment_names, start=1)}
     return compmap
 
@@ -755,15 +833,16 @@
     newmap['OUTPUT'] = len(newmap) + 1
     oldmap = oldmap.copy()
     oldmap['OUTPUT'] = len(oldmap) + 1
     remap = create_compartment_remap(oldmap, newmap)
     d = {}
     for old, new in remap.items():
         d[sympy.Symbol(f'S{old}')] = sympy.Symbol(f'S{new}')
-        d[sympy.Symbol(f'F{old}')] = sympy.Symbol(f'F{new}')
+        # FIXME: F should also be moved with dose compartment (?)
+        # d[sympy.Symbol(f'F{old}')] = sympy.Symbol(f'F{new}')
         # FIXME: R, D and ALAG should be moved with dose compartment
         # d[sympy.Symbol(f'R{old}')] = sympy.Symbol(f'R{new}')
         # d[sympy.Symbol(f'D{old}')] = sympy.Symbol(f'D{new}')
         # d[sympy.Symbol(f'ALAG{old}')] = sympy.Symbol(f'ALAG{new}')
         d[sympy.Symbol(f'A({old})')] = sympy.Symbol(f'A({new})')
     if from_advan == 'ADVAN5' or from_advan == 'ADVAN7':
         reverse_map = {v: k for k, v in newmap.items()}
@@ -920,15 +999,15 @@
     return len(odes) == 1
 
 
 def match_advan2(statements):
     odes = statements.ode_system
     if len(odes) != 2:
         return False
-    dosing = odes.dosing_compartment
+    dosing = odes.dosing_compartment[0]
     outflows = odes.get_compartment_outflows(dosing)
     if len(outflows) != 1:
         return False
     central = outflows[0][0]
     central_rate = outflows[0][1]
 
     # Check if rate is depending on CL or V assignments
@@ -947,27 +1026,27 @@
         return False
     return True
 
 
 def match_advan3(odes):
     if len(odes) != 2:
         return False
-    central = odes.dosing_compartment
+    central = odes.dosing_compartment[0]
     bidir = odes.get_bidirectionals(central)
     if len(bidir) != 1:
         return False
     if odes.get_flow(bidir[0], output) != 0:
         return False
     return True
 
 
 def match_advan4(odes):
     if len(odes) != 3:
         return False
-    dosing = odes.dosing_compartment
+    dosing = odes.dosing_compartment[0]
     outflows = odes.get_compartment_outflows(dosing)
     if len(outflows) != 1:
         return False
     central = outflows[0][0]
     bidir = odes.get_bidirectionals(central)
     if len(bidir) != 1:
         return False
@@ -975,15 +1054,15 @@
         return False
     return True
 
 
 def match_advan11(odes):
     if len(odes) != 3:
         return False
-    central = odes.dosing_compartment
+    central = odes.dosing_compartment[0]
     bidir = odes.get_bidirectionals(central)
     if len(bidir) != 2:
         return False
     if (
         odes.get_flow(bidir[0], output) != 0
         or odes.get_flow(bidir[1], output) != 0
         or odes.get_flow(bidir[0], bidir[1]) != 0
@@ -991,15 +1070,15 @@
         return False
     return True
 
 
 def match_advan12(odes):
     if len(odes) != 4:
         return False
-    dosing = odes.dosing_compartment
+    dosing = odes.dosing_compartment[0]
     outflows = odes.get_compartment_outflows(dosing)
     if len(outflows) != 1:
         return False
     central = outflows[0][0]
     bidir = odes.get_bidirectionals(central)
     if len(bidir) != 2:
         return False
@@ -1455,27 +1534,37 @@
     if old_records:
         control_stream = control_stream.replace_records(old_records, new_records)
     else:
         for rec in new_records:
             newrec = create_record(str(rec))
             control_stream = control_stream.insert_record(newrec)
 
-    old_cov = False
+    # Initiate old_cov
+    old_cov = None
     for est in old:
-        old_cov |= est.cov
-    new_cov = False
+        old_cov = est.cov
+
+    # Initiate new_cov
+    new_cov = None
     for est in new:
-        new_cov |= est.cov
-    if not old_cov and new_cov:
+        new_cov = est.cov
+
+    if old_cov is None and new_cov is not None:
         # Add $COV
         last_est_rec = control_stream.get_records('ESTIMATION')[-1]
         idx_cov = control_stream.records.index(last_est_rec)
-        covrec = create_record('$COVARIANCE\n')
+        if new_cov == 'SANDWICH':
+            covrec_ = '$COVARIANCE'
+        elif new_cov == 'CPG':
+            covrec_ = '$COVARIANCE MATRIX=S'
+        elif new_cov == 'OFIM':
+            covrec_ = '$COVARIANCE MATRIX=R'
+        covrec = create_record(f'{covrec_}\n')
         control_stream = control_stream.insert_record(covrec, at_index=idx_cov + 1)
-    elif old_cov and not new_cov:
+    elif old_cov is not None and new_cov is None:
         # Remove $COV
         covrecs = control_stream.get_records('COVARIANCE')
         control_stream = control_stream.remove_records(covrecs)
 
     # Update $TABLE
     # Currently only adds if did not exist before
     cols = set()
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/rxode/model.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/rxode/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/external/utils.py` & `pharmpy-core-0.98.0/src/pharmpy/model/external/utils.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/model.py` & `pharmpy-core-0.98.0/src/pharmpy/model/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/parameters.py` & `pharmpy-core-0.98.0/src/pharmpy/model/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/random_variables.py` & `pharmpy-core-0.98.0/src/pharmpy/model/random_variables.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/results.py` & `pharmpy-core-0.98.0/src/pharmpy/model/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/model/statements.py` & `pharmpy-core-0.98.0/src/pharmpy/model/statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import warnings
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from typing import Iterable, List, Optional, Set, Tuple, Union, overload
 
 import pharmpy.internals.unicode as unicode
 from pharmpy.deps import networkx as nx
 from pharmpy.deps import sympy
@@ -76,14 +77,19 @@
     def create(cls, symbol, expression):
         if isinstance(symbol, str):
             symbol = sympy.Symbol(symbol)
         if not (symbol.is_Symbol or symbol.is_Derivative or symbol.is_Function):
             raise TypeError("symbol of Assignment must be a Symbol or str representing a symbol")
         if isinstance(expression, str):
             expression = parse_expr(expression)
+        # Needed for expression.free_symbols to work
+        if isinstance(expression, float):
+            expression = sympy.Float(expression)
+        if isinstance(expression, int):
+            expression = sympy.Integer(expression)
         return cls(symbol, expression)
 
     def replace(self, **kwargs):
         symbol = kwargs.get('symbol', self._symbol)
         expression = kwargs.get('expression', self._expression)
         return Assignment.create(symbol, expression)
 
@@ -678,15 +684,15 @@
         return atoms
 
     def __eq__(self, other):
         return (
             isinstance(other, CompartmentalSystem)
             and self._t == other._t
             and nx.to_dict_of_dicts(self._g) == nx.to_dict_of_dicts(other._g)
-            and self.dosing_compartment.dose == other.dosing_compartment.dose
+            and self.dosing_compartment == other.dosing_compartment
         )
 
     def __hash__(self):
         return hash((self._t, self._g))
 
     def to_dict(self):
         comps = [comp for comp in self._g.nodes]
@@ -898,32 +904,41 @@
         in_comps = {c for c, _ in self.get_compartment_inflows(comp)}
         return len((out_comps | in_comps) - {output})
 
     @property
     def dosing_compartment(self):
         """The dosing compartment
 
-        A dosing compartment is a compartment that receives an input dose. Only one dose
-        compartment is supported.
+        A dosing compartment is a compartment that receives an input dose. Multiple
+        dose compartments are supported. The order of dose compartments is defined
+        to put the central compartment last.
 
         Returns
         -------
-        Compartment
-            Dosing compartment
+        tuple
+            A tuple of dose compartments
 
         Examples
         --------
         >>> from pharmpy.modeling import load_example_model
         >>> model = load_example_model("pheno")
-        >>> model.statements.ode_system.dosing_compartment
+        >>> model.statements.ode_system.dosing_compartment[0]
         Compartment(CENTRAL, amount=A_CENTRAL, dose=Bolus(AMT, admid=1))
         """
+        dosing_comps = tuple()
         for node in _comps(self._g):
             if node.dose is not None:
-                return node
+                if node.name != self.central_compartment.name:
+                    dosing_comps = (node,) + dosing_comps
+                else:
+                    dosing_comps = dosing_comps + (node,)
+
+        if len(dosing_comps) != 0:
+            return dosing_comps
+
         raise ValueError('No dosing compartment exists')
 
     @property
     def central_compartment(self):
         """The central compartment
 
         The central compartment is defined to be the compartment that has an outward flow
@@ -938,16 +953,17 @@
         --------
         >>> from pharmpy.modeling import load_example_model
         >>> model = load_example_model("pheno")
         >>> model.statements.ode_system.central_compartment
         Compartment(CENTRAL, amount=A_CENTRAL, dose=Bolus(AMT, admid=1))
         """
         try:
-            central = next(self._g.predecessors(output))
-        except StopIteration:
+            # E.g. TMDD models have more than one input
+            central = list(self._g.predecessors(output))[-1]
+        except IndexError:
             raise ValueError('Cannot find central compartment')
         return central
 
     @property
     def peripheral_compartments(self):
         """Find perihperal compartments
 
@@ -993,15 +1009,15 @@
         --------
         >>> from pharmpy.modeling import load_example_model
         >>> model = load_example_model("pheno")
         >>> model.statements.ode_system.find_transit_compartments(model.statements)
         []
         """
         transits = []
-        comp = self.dosing_compartment
+        comp = self.dosing_compartment[0]
         if len(self.get_compartment_inflows(comp)) != 0:
             return transits
         outflows = self.get_compartment_outflows(comp)
         if len(outflows) != 1:
             return transits
         transits.append(comp)
         comp, rate = outflows[0]
@@ -1128,15 +1144,15 @@
         ordered_cmts = self._order_compartments()
         names = [cmt.name for cmt in ordered_cmts]
         return names
 
     def _order_compartments(self):
         """Return list of all compartments in canonical order"""
         try:
-            dosecmt = self.dosing_compartment
+            dosecmt = self.dosing_compartment[0]
         except ValueError:
             # Fallback for cases where no dose is available (yet)
             return list(_comps(self._g))
         # Order compartments
 
         def sortfunc(x):
             a = list(x)
@@ -1193,15 +1209,15 @@
 
         def f_string(comp):
             return f"\nF={comp.bioavailability}" if comp.bioavailability != 1 else ""
 
         def comp_string(comp):
             return comp.name + lag_string(comp) + f_string(comp)
 
-        current = self.dosing_compartment
+        current = self.dosing_compartment[0]
         comp_height = 0
         comp_width = 0
 
         while True:
             bidirects = self.get_bidirectionals(current)
             outflows = self.get_compartment_outflows(current)
             comp_height = max(comp_height, len(bidirects) + 1)
@@ -1216,27 +1232,32 @@
         noutput = len(self.get_compartment_inflows(output))
         have_zo_input = int(not is_zero_matrix(self.zero_order_inputs))
         comp_nrows = comp_height * 2 - 1 + (1 if noutput > 1 else 0)
         nrows = comp_nrows + have_zo_input
         ncols = comp_width * 2
         grid = unicode.Grid(nrows, ncols)
 
-        current = self.dosing_compartment
+        current = self.dosing_compartment[0]
         col = 0
         if comp_nrows == 1 or comp_nrows == 2:
             main_row = 0 + have_zo_input
         else:
             main_row = 2 + have_zo_input
 
         if have_zo_input:
             # Assuming a fully linear layout
             for i, zo in enumerate(self.zero_order_inputs):
                 if zo != 0:
-                    grid.set(0, i * 2, unicode.VerticalArrow(str(zo)))
-
+                    try:
+                        grid.set(0, i * 2, unicode.VerticalArrow(str(zo)))
+                    except IndexError:
+                        warnings.warn(
+                            """The ODE system cannot be printed. Try statements.before_odes
+                            and statements.after_odes instead."""
+                        )
         while True:
             bidirects = self.get_bidirectionals(current)
             outflows = self.get_compartment_outflows(current)
             comp_box = unicode.Box(comp_string(current))
             grid.set(main_row, col, comp_box)
 
             if bidirects:
@@ -1278,15 +1299,15 @@
                 arrow = unicode.VerticalArrow(str(rate))
                 grid.set(main_row + 1, col, arrow)
             col += 2
             current = next_comp
             if not current:
                 break
 
-        dose = self.dosing_compartment.dose
+        dose = self.dosing_compartment[0].dose
         s = str(dose) + '\n' + str(grid).rstrip()
         return s
 
 
 class Compartment:
     """Compartment for a compartmental system
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/__init__.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,20 +17,22 @@
     rename_symbols,
     set_name,
     write_model,
 )
 from .compartments import get_bioavailability, get_lag_times
 from .covariate_effect import add_covariate_effect, has_covariate_effect, remove_covariate_effect
 from .data import (
+    add_admid,
     add_time_after_dose,
     check_dataset,
     deidentify_data,
     drop_columns,
     drop_dropped_columns,
     expand_additional_doses,
+    get_admid,
     get_baselines,
     get_cmt,
     get_concentration_parameters_from_data,
     get_covariate_baselines,
     get_doseid,
     get_doses,
     get_evid,
@@ -87,14 +89,15 @@
     calculate_eta_gradient_expression,
     cleanup_model,
     create_symbol,
     get_dv_symbol,
     get_individual_parameters,
     get_individual_prediction_expression,
     get_observation_expression,
+    get_pd_parameters,
     get_pk_parameters,
     get_population_prediction_expression,
     get_rv_parameters,
     greekify_model,
     has_random_effect,
     is_linearized,
     is_real,
@@ -111,14 +114,15 @@
     calculate_prec_from_corrse,
     calculate_prec_from_cov,
     calculate_se_from_cov,
     calculate_se_from_prec,
 )
 from .metabolite import add_metabolite
 from .odes import (
+    add_bioavailability,
     add_individual_parameter,
     add_lag_time,
     add_peripheral_compartment,
     display_odes,
     find_clearance_parameters,
     find_volume_parameters,
     get_initial_conditions,
@@ -127,14 +131,15 @@
     has_linear_odes,
     has_linear_odes_with_real_eigenvalues,
     has_michaelis_menten_elimination,
     has_mixed_mm_fo_elimination,
     has_odes,
     has_zero_order_absorption,
     has_zero_order_elimination,
+    remove_bioavailability,
     remove_lag_time,
     remove_peripheral_compartment,
     set_bolus_absorption,
     set_first_order_absorption,
     set_first_order_elimination,
     set_initial_condition,
     set_michaelis_menten_elimination,
@@ -202,23 +207,25 @@
 from .tmdd import set_tmdd
 from .units import get_unit_of
 from .write_csv import write_csv
 
 # Must be set directly, otherwise errors about unused imports
 __all__ = [
     'set_direct_effect',
+    'add_admid',
     'add_allometry',
     'add_covariance_step',
     'add_covariate_effect',
     'add_estimation_step',
     'add_effect_compartment',
     'add_iiv',
     'add_individual_parameter',
     'add_iov',
     'add_lag_time',
+    'add_bioavailability',
     'add_metabolite',
     'add_peripheral_compartment',
     'add_pk_iiv',
     'add_population_parameter',
     'add_time_after_dose',
     'append_estimation_step_options',
     'bump_model_number',
@@ -262,14 +269,15 @@
     'evaluate_weighted_residuals',
     'expand_additional_doses',
     'find_clearance_parameters',
     'find_volume_parameters',
     'fix_or_unfix_parameters',
     'fix_parameters',
     'fix_parameters_to',
+    'get_admid',
     'get_baselines',
     'get_bioavailability',
     'get_cmt',
     'get_concentration_parameters_from_data',
     'get_config_path',
     'get_covariate_baselines',
     'get_doses',
@@ -287,14 +295,15 @@
     'get_number_of_individuals',
     'get_number_of_observations',
     'get_number_of_observations_per_individual',
     'get_omegas',
     'get_observations',
     'get_observation_expression',
     'get_pk_parameters',
+    'get_pd_parameters',
     'get_population_prediction_expression',
     'get_rv_parameters',
     'get_sigmas',
     'get_thetas',
     'get_unit_of',
     'get_zero_order_inputs',
     'greekify_model',
@@ -330,14 +339,15 @@
     'rename_symbols',
     'remove_covariance_step',
     'remove_covariate_effect',
     'remove_error_model',
     'remove_estimation_step',
     'remove_iiv',
     'remove_iov',
+    'remove_bioavailability',
     'remove_lag_time',
     'remove_loq_data',
     'remove_peripheral_compartment',
     'remove_unused_parameters_and_rvs',
     'resample_data',
     'sample_parameters_from_covariance_matrix',
     'sample_individual_estimates',
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/allometry.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/basic_models.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/basic_models.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/blq.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/blq.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def transform_blq(model: Model, method: str = 'm4', lloq: Optional[float] = None):
     """Transform for BLQ data
 
     Transform a given model, methods available are m1, m3, and m4 [1]_. Current limits of the
     m3 and m4 method:
 
     * Does not support covariance between epsilons
-    * Only supports additive, proportional, and combined error model
+    * Supports additive, proportional, combined, and power error model
 
     .. [1] Beal SL. Ways to fit a PK model with some data below the quantification
     limit. J Pharmacokinet Pharmacodyn. 2001 Oct;28(5):481-504. doi: 10.1023/a:1012299115260.
     Erratum in: J Pharmacokinet Pharmacodyn 2002 Jun;29(3):309. PMID: 11768292.
 
     Parameters
     ----------
@@ -157,16 +157,16 @@
 
 def get_blq_symb_and_type(model: Model):
     try:
         blq_datainfo = model.datainfo.typeix['lloq']
         return sympy.Symbol(blq_datainfo[0].name), 'lloq'
     except IndexError:
         try:
-            blq_datainfo = model.datainfo.typeix['blq']
-            return sympy.Symbol(blq_datainfo[0].name), 'blq'
+            blq_datainfo = model.datainfo.typeix['blqdv']
+            return sympy.Symbol(blq_datainfo[0].name), 'blqdv'
         except IndexError:
             return sympy.Symbol('LLOQ'), 'lloq'
 
 
 def _has_all_expected_symbs(sset, expected_symbs):
     symb_names = [s.symbol.name for s in sset]
     return all(symb in symb_names for symb in expected_symbs)
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/common.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
     """
     datasymbs = {sympy.Symbol(s) for s in model.datainfo.names}
 
     odes = model.statements.ode_system
 
     # Consider statements that are dependencies of the ode system and y
     if odes:
-        dose_comp = odes.dosing_compartment
+        dose_comp = odes.dosing_compartment[0]
         cb = CompartmentalSystemBuilder(odes)
         cb.set_dose(dose_comp, None)
         cs = CompartmentalSystem(cb)
         statements = model.statements.before_odes + cs + model.statements.after_odes
         ode_deps = statements.dependencies(cs)
     else:
         ode_deps = set()
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/compartments.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/compartments.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/covariate_effect.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/covariate_effect.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,16 +138,16 @@
             - For each additional category:
 
             .. math::
 
                 \\text{coveff} = 1 + \\text{theta}
 
         - Init: :math:`0.001`
-        - Upper: :math:`100,000`
-        - Lower: :math:`-100,000`
+        - Upper: :math:`5`
+        - Lower: :math:`-1`
     - Piecewise linear function/"hockey-stick", continuous covariates only (*piece_lin*)
         - Function:
             - If cov <= median:
 
             .. math::
 
                 \\text{coveff} = 1 + \\text{theta1} * (\\text{cov} - \\text{median})
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/data.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -841,19 +841,95 @@
         pass
     else:
         return model.dataset[eventcols[0].name]
     mdv = get_mdv(model)
     return mdv.rename('EVID')
 
 
+def get_admid(model: Model):
+    """Get the admid from model dataset
+
+    If an administration column is present this will be extracted otherwise
+    an admid column will be created.
+    1 : Oral dose
+    2 : IV dose
+
+    Parameters
+    ----------
+    model : Model
+        Pharmpy model
+
+    Returns
+    -------
+    pd.Series
+        ADMID
+    """
+    di = model.datainfo
+    try:
+        admidcols = di.typeix["admid"]
+    except IndexError:
+        pass
+    else:
+        return model.dataset[admidcols[0].name]
+
+    oral = iv = None
+    odes = model.statements.ode_system
+    names = odes.compartment_names
+    if isinstance(odes, CompartmentalSystem):
+        for dosing in odes.dosing_compartment:
+            if dosing == odes.central_compartment:
+                iv = names.index(dosing.name) + 1
+            else:
+                oral = names.index(dosing.name) + 1
+    adm = get_cmt(model)
+    adm = adm.replace({oral: 1, iv: 2})
+    adm.name = "ADMID"
+    return adm
+
+
+def add_admid(model: Model):
+    """
+    Add an admid column to the model dataset and datainfo. Dependent on the
+    presence of a CMT column in order to add admid correctly.
+    1 : Oral dose
+    2 : IV dose
+
+    Parameters
+    ----------
+    model : Model
+        Pharmpy model
+
+    Returns
+    -------
+    model : Model
+        Pharmpy model
+
+    See also
+    --------
+    get_admid : Get or create an admid column
+    get_cmt : Get or create a cmt column
+    """
+    di = model.datainfo
+    if "admid" not in di.types:
+        adm = get_admid(model)
+        dataset = model.dataset
+        dataset["ADMID"] = adm
+        di = update_datainfo(model.datainfo, dataset)
+        colinfo = di['ADMID'].replace(type='admid')
+        model = model.replace(datainfo=di.set_column(colinfo), dataset=dataset)
+
+    return model.update_source()
+
+
 def get_cmt(model: Model):
     """Get the cmt (compartment) column from the model dataset
 
     If a cmt column is present this will be extracted otherwise
-    a cmt column will be created.
+    a cmt column will be created. If created, multiple dose compartments are
+    not supported.
 
     Parameters
     ----------
     model : Model
         Pharmpy model
 
     Returns
@@ -866,15 +942,15 @@
         cmtcols = di.typeix['compartment']
     except IndexError:
         pass
     else:
         return model.dataset[cmtcols[0].name]
     odes = model.statements.ode_system
     if isinstance(odes, CompartmentalSystem):
-        dosing = odes.dosing_compartment
+        dosing = odes.dosing_compartment[0]
         names = odes.compartment_names
         dose_cmt = names.index(dosing.name) + 1
     else:
         dose_cmt = 1
     cmt = get_evid(model)
     cmt = cmt.replace({1: dose_cmt, 2: 0, 3: 0, 4: dose_cmt})  # Only consider dose/non-dose
     cmt.name = "CMT"
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/error.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -834,25 +834,29 @@
         sympy.Piecewise((sympy.log(y), sympy.Eq(lam, 0)), ((y**lam - 1) / lam, sympy.Ne(lam, 0))),
     )
     model = model.replace(observation_transformation=obs, statements=statements)
 
     return model.update_source()
 
 
-def set_time_varying_error_model(model: Model, cutoff: float, idv: str = 'TIME'):
+def set_time_varying_error_model(
+    model: Model, cutoff: float, idv: str = 'TIME', dv: Union[sympy.Symbol, str, int, None] = None
+):
     """Set a time varying error model per time cutoff
 
     Parameters
     ----------
     model : Model
         Pharmpy model
     cutoff : float
         A value at the given quantile over idv column
     idv : str
         Time or time after dose, default is Time
+    dv : Union[sympy.Symbol, str, int, None]
+        Name or DVID of dependent variable. None for the default (first or only)
 
     Return
     ------
     Model
         Pharmpy model object
 
     Examples
@@ -862,15 +866,16 @@
     >>> model = set_time_varying_error_model(model, cutoff=1.0)
     >>> model.statements.find_assignment("Y")
         ⎧EPS₁⋅W⋅time_varying + F  for TIME < 1.0
         ⎨
     Y = ⎩      EPS₁⋅W + F           otherwise
 
     """
-    y = model.statements.find_assignment('Y')
+    dv = get_dv_symbol(model, dv)
+    y = model.statements.find_assignment(dv)
     idv = parse_expr(idv)
     theta = create_symbol(model, 'time_varying')
     eps = model.random_variables.epsilons
     expr = sympy.Piecewise(
         (
             subs(
                 y.expression,
@@ -1022,14 +1027,15 @@
             ipred = s.symbol
             break
     return ipred
 
 
 def set_iiv_on_ruv(
     model: Model,
+    dv: Union[sympy.Symbol, str, int, None] = None,
     list_of_eps: Optional[Union[List[str], str]] = None,
     same_eta: bool = True,
     eta_names: Optional[Union[List[str], str]] = None,
 ):
     """
     Multiplies epsilons with exponential (new) etas.
 
@@ -1043,14 +1049,16 @@
         Name/names of epsilons to multiply with exponential etas. If None, all epsilons will
         be chosen. None is default.
     same_eta : bool
         Boolean of whether all RUVs from input should use the same new ETA or if one ETA
         should be created for each RUV. True is default.
     eta_names : str, list
         Custom names of new etas. Must be equal to the number epsilons or 1 if same eta.
+    dv : Union[sympy.Symbol, str, int, None]
+        Name or DVID of dependent variable. None for the default (first or only)
 
     Return
     ------
     Model
         Pharmpy model object
 
     Examples
@@ -1082,21 +1090,28 @@
         rvs = rvs + eta
         eta_dict = {e: eta for e in eps}
     else:
         etas = [_create_eta(pset, i + 1, eta_names) for i in range(len(eps))]
         rvs = rvs + etas
         eta_dict = dict(zip(eps, etas))
 
+    dv_symb = get_dv_symbol(model, dv)
+    y = model.statements.find_assignment(dv_symb)
+
     for e in eps:
-        sset = sset.subs(
-            {
-                sympy.Symbol(e.names[0]): sympy.Symbol(e.names[0])
-                * sympy.exp(sympy.Symbol(eta_dict[e].names[0]))
-            }
-        )
+        subs_dict = {
+            sympy.Symbol(e.names[0]): sympy.Symbol(e.names[0])
+            * sympy.exp(sympy.Symbol(eta_dict[e].names[0]))
+        }
+        # FIXME: this is needed if you e.g. have Y and IPRED, with multiple DVs, how should this be handled?
+        if not dv:
+            sset = sset.subs(subs_dict)
+        else:
+            y = y.subs(subs_dict)
+            sset = sset.reassign(y.symbol, y.expression)
 
     model = model.replace(random_variables=rvs, parameters=Parameters.create(pset), statements=sset)
     return model.update_source()
 
 
 def _create_eta(pset, number, eta_names):
     omega = sympy.Symbol(f'IIV_RUV{number}')
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/estimation.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/estimation_steps.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/estimation_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         Pharmpy model object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
     >>> opts = {'NITER': 1000, 'ISAMPLE': 100}
-    >>> model = set_estimation_step(model, "IMP", evaluation=True, tool_options=opts)
+    >>> model = set_estimation_step(model, 'IMP', evaluation=True, tool_options=opts)
     >>> model.estimation_steps[0]   # doctest: +ELLIPSIS
-    EstimationStep("IMP", interaction=True, cov=True, evaluation=True, ..., tool_options=...
+    EstimationStep('IMP', interaction=True, cov='SANDWICH', evaluation=True, ..., tool_options=...
 
     See also
     --------
     add_estimation_step
     remove_estimation_step
     append_estimation_step_options
     add_covariance_step
@@ -82,20 +82,20 @@
         Pharmpy model object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
     >>> opts = {'NITER': 1000, 'ISAMPLE': 100}
-    >>> model = add_estimation_step(model, "IMP", tool_options=opts)
+    >>> model = add_estimation_step(model, 'IMP', tool_options=opts)
     >>> ests = model.estimation_steps
     >>> len(ests)
     2
     >>> ests[1]   # doctest: +ELLIPSIS
-    EstimationStep("IMP", interaction=False, cov=False, ..., tool_options={'NITER': 1000,...
+    EstimationStep('IMP', interaction=False, cov=None, ..., tool_options={'NITER': 1000,...
 
     See also
     --------
     set_estimation_step
     remove_estimation_step
     append_estimation_step_options
     add_covariance_step
@@ -213,49 +213,51 @@
     toolopts.update(tool_options)
     newstep = steps[idx].replace(tool_options=toolopts)
     newsteps = steps[0:idx] + newstep + steps[idx + 1 :]
     model = model.replace(estimation_steps=newsteps)
     return model.update_source()
 
 
-def add_covariance_step(model: Model):
+def add_covariance_step(model: Model, cov: str):
     """Adds covariance step to the final estimation step
 
     Parameters
     ----------
     model : Model
         Pharmpy model
+    cov : str
+        covariance method to use
 
     Returns
     -------
     Model
         Pharmpy model object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
-    >>> model = set_estimation_step(model, 'FOCE', cov=False)
-    >>> model = add_covariance_step(model)
+    >>> model = set_estimation_step(model, 'FOCE', cov=None)
+    >>> model = add_covariance_step(model, 'SANDWICH')
     >>> ests = model.estimation_steps
     >>> ests[0]   # doctest: +ELLIPSIS
-    EstimationStep("FOCE", interaction=True, cov=True, ...)
+    EstimationStep('FOCE', interaction=True, cov='SANDWICH', ...)
 
     See also
     --------
     add_estimation_step
     set_estimation_step
     remove_estimation_step
     append_estimation_step_options
     remove_covariance_step
     set_evaluation_step
 
     """
     steps = model.estimation_steps
-    newstep = steps[-1].replace(cov=True)
+    newstep = steps[-1].replace(cov=f'{cov}')
     newsteps = steps[0:-1] + newstep
     model = model.replace(estimation_steps=newsteps)
     return model.update_source()
 
 
 def remove_covariance_step(model: Model):
     """Removes covariance step to the final estimation step
@@ -273,28 +275,28 @@
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
     >>> model = remove_covariance_step(model)
     >>> ests = model.estimation_steps
     >>> ests[0]   # doctest: +ELLIPSIS
-    EstimationStep("FOCE", interaction=True, cov=False, ...)
+    EstimationStep('FOCE', interaction=True, cov=None, ...)
 
     See also
     --------
     add_estimation_step
     set_estimation_step
     remove_estimation_step
     append_estimation_step_options
     add_covariance_step
     set_evaluation_step
 
     """
     steps = model.estimation_steps
-    newstep = steps[-1].replace(cov=False)
+    newstep = steps[-1].replace(cov=None)
     newsteps = steps[:-1] + newstep
     model = model.replace(estimation_steps=newsteps)
     return model.update_source()
 
 
 def set_evaluation_step(model: Model, idx: int = -1):
     """Set estimation step
@@ -316,15 +318,15 @@
 
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
     >>> model = set_evaluation_step(model)
     >>> model.estimation_steps[0]   # doctest: +ELLIPSIS
-    EstimationStep("FOCE", interaction=True, cov=True, evaluation=True, ...
+    EstimationStep('FOCE', interaction=True, cov='SANDWICH', evaluation=True, ...
 
     See also
     --------
     set_estimation_step
     add_estimation_step
     remove_estimation_step
     append_estimation_step_options
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/evaluation.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/evaluation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/moxo.csv` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/moxo.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/moxo.mod` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/moxo.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.cov` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.datainfo` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.dta` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.ext` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.lst` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.mod` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.phi` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno.tab` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.dta` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.ext` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.lst` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.mod` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/example_models/pheno_linear.phi` & `pharmpy-core-0.98.0/src/pharmpy/modeling/example_models/pheno_linear.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/expressions.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1130,15 +1130,15 @@
         True,
         is_constant,
         contains_theta,
     )
 
 
 def get_pk_parameters(model: Model, kind: str = 'all') -> List[str]:
-    """Retrieves PK parameters in :class:`pharmpy.model`.
+    """Retrieves PK parameters in :class:`pharmpy.model.Model`.
 
     Parameters
     ----------
     model : Model
         Pharmpy model to retrieve the PK parameters from
     kind : str
         The type of parameter to retrieve: 'absorption', 'distribution',
@@ -1171,15 +1171,60 @@
     natural_assignments = _get_natural_assignments(model.statements.before_odes)
     cs_remapped = _remap_compartmental_system(model.statements, natural_assignments)
 
     free_symbols = set(_pk_free_symbols(cs_remapped, kind))
 
     dependency_graph = _dependency_graph(natural_assignments)
 
-    return sorted(map(str, _filter_symbols(dependency_graph, free_symbols)))
+    pk_symbols = _filter_symbols(dependency_graph, free_symbols)
+    if model.statements.ode_system.find_compartment("EFFECT") is not None:
+        pd_symbols = model.statements.ode_system.find_compartment("EFFECT").input.free_symbols
+        pk_symbols = pk_symbols.difference(pd_symbols)
+    return sorted(map(str, pk_symbols))
+
+
+def get_pd_parameters(model: Model) -> List[str]:
+    """Retrieves PD parameters in :class:`pharmpy.model.Model`.
+
+    Parameters
+    ----------
+    model : Model
+        Pharmpy model to retrieve the PD parameters from
+
+    Return
+    ------
+    list[str]
+        A list of the PD parameter names of the given model
+
+    Example
+    -------
+    >>> from pharmpy.modeling import *
+    >>> model = load_example_model("pheno")
+    >>> model = set_direct_effect(model, "linear")
+    >>> get_pd_parameters(model)
+    ['E0', 'S']
+
+    See also
+    --------
+    get_pk_parameters
+
+    """
+    # FIXME: this function needs to be updated. Currently uses fixed parameter names.
+
+    pd_symbols = []
+    sset = model.statements
+    if sympy.Symbol('Y_2') in model.dependent_variables:
+        parameters_in_e = sset.find_assignment('E').free_symbols
+        pk_parameters = get_pk_parameters(model)
+        parameters_in_e = {x for x in parameters_in_e if str(x) not in pk_parameters}
+        pd_symbols = {statement.symbol for statement in sset.before_odes}
+        pd_symbols = pd_symbols.intersection(parameters_in_e)
+        if sset.ode_system.find_compartment("EFFECT") is not None:
+            pd_symbols.add("KE0")
+    return sorted(map(str, pd_symbols))
 
 
 def _get_natural_assignments(before_odes):
     # Return assignments where assignments that are constants (e.g. X=1),
     # single length expressions (e.g. S1=V), and divisions between parameters
     # (e.g. K=CL/V) have been filtered out
     classified_assignments = list(_classify_assignments(list(_assignments(before_odes))))
@@ -1204,16 +1249,16 @@
 def _pk_free_symbols(cs: CompartmentalSystem, kind: str) -> Iterable[sympy.Symbol]:
     if kind == 'all':
         return cs.free_symbols
 
     if kind == 'absorption':
         return (
             []
-            if cs.dosing_compartment == cs.central_compartment
-            else _pk_free_symbols_from_compartment(cs, cs.dosing_compartment)
+            if cs.dosing_compartment[0] == cs.central_compartment
+            else _pk_free_symbols_from_compartment(cs, cs.dosing_compartment[0])
         )
 
     if kind == 'distribution':
         return _pk_free_symbols_from_compartment(cs, cs.central_compartment)
 
     if kind == 'elimination':
         free_symbols = _pk_free_symbols_from_compartment(cs, output)
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/help_functions.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/iterators.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/lrt.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/math.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/metabolite.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/metabolite.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/odes.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/odes.py`

 * *Files 6% similar despite different names*

```diff
@@ -202,14 +202,118 @@
             {sympy.Symbol('KM'), sympy.Symbol('CLMM')}, statements.ode_system
         )
         model = model.replace(statements=statements)
         model = remove_unused_parameters_and_rvs(model)
     return model
 
 
+def add_bioavailability(model: Model, add_parameter: bool = True):
+    """Add bioavailability statement for the first dose compartment of the model.
+    Can be added as a new parameter or otherwise it will be set to 1.
+
+    Parameters
+    ----------
+    model : Model
+        Pharmpy model
+    add_parameter : bool
+        Add new parameter representing bioavailability or not
+
+    Return
+    ------
+    Model
+        Pharmpy model object
+
+    Examples
+    --------
+    >>> from pharmpy.modeling import *
+    >>> model = load_example_model("pheno")
+    >>> model = add_bioavailability(model)
+
+    See also
+    --------
+    remove_bioavailability
+
+    """
+    odes = model.statements.ode_system
+    if odes is None:
+        raise ValueError(f'Model {model.name} has no ODE system')
+
+    dose_comp = odes.dosing_compartment[0]
+    bio = dose_comp.bioavailability
+
+    if isinstance(bio, sympy.Number):
+        # Bio not defined
+        if add_parameter:
+            model, bio_symb = _add_parameter(model, 'BIO', init=float(bio))
+            f_ass = Assignment.create(sympy.Symbol('F_BIO'), bio_symb)
+
+            new_before_odes = model.statements.before_odes + f_ass
+
+        else:
+            # Add as a number
+            bio_ass = Assignment.create(sympy.Symbol("BIO"), sympy.Number(1))
+            f_ass = Assignment.create(sympy.Symbol("F_BIO"), bio_ass.symbol)
+            new_before_odes = bio_ass + model.statements.before_odes + f_ass
+
+        # Add statement to code
+        cb = CompartmentalSystemBuilder(odes)
+        cb.set_bioavailability(dose_comp, f_ass.symbol)
+
+        model = model.replace(
+            statements=(new_before_odes + CompartmentalSystem(cb) + model.statements.after_odes)
+        )
+
+    else:
+        # BIO already defined, leave it alone?
+        pass
+
+    return model.update_source()
+
+
+def remove_bioavailability(model: Model):
+    """Remove bioavailability from the first dose compartment of model.
+
+    Parameters
+    ----------
+    model : Model
+        Pharmpy model
+
+    Return
+    ------
+    Model
+        Pharmpy model object
+
+    Examples
+    --------
+    >>> from pharmpy.modeling import *
+    >>> model = load_example_model("pheno")
+    >>> model = remove_bioavailability(model)
+
+    See also
+    --------
+    set_bioavailability
+    """
+    odes = model.statements.ode_system
+    if odes is None:
+        raise ValueError(f'Model {model.name} has no ODE system')
+    dosing_comp = odes.dosing_compartment[0]
+    bio = dosing_comp.bioavailability
+    if bio:
+        symbols = bio.free_symbols
+        cb = CompartmentalSystemBuilder(odes)
+        cb.set_bioavailability(dosing_comp, sympy.Integer(1))
+        statements = (
+            model.statements.before_odes + CompartmentalSystem(cb) + model.statements.after_odes
+        )
+        statements = statements.remove_symbol_definitions(symbols, statements.ode_system)
+        model = model.replace(statements=statements)
+        model = remove_unused_parameters_and_rvs(model)
+    return model
+
+
 def set_zero_order_elimination(model: Model):
     """Sets elimination to zero order.
 
     Initial estimate for KM is set to 1% of smallest observation.
 
     Parameters
     ----------
@@ -698,14 +802,16 @@
         raise ValueError(f'Model {model.name} has no ODE system')
     transits = cs.find_transit_compartments(statements)
     try:
         n = _as_integer(n)
     except ValueError:
         raise ValueError(f'Number of compartments must be integer: {n}')
 
+    model = remove_lag_time(model)
+
     # Handle keep_depot option
     depot = cs.find_depot(statements)
     mdt_init = None
     mdt_assign = None
     if not keep_depot and depot:
         central = cs.central_compartment
         rate = cs.get_flow(depot, central)
@@ -752,23 +858,25 @@
         else:
             if mdt_init is not None:
                 init = mdt_init
             else:
                 init = _get_absorption_init(model, 'MDT')
             model, mdt_symb = _add_parameter(model, 'MDT', init=init)
         rate = n / mdt_symb
-        dosing_comp = cs.dosing_compartment
+        dosing_comp = cs.dosing_compartment[0]
         comp = dosing_comp
         cb = CompartmentalSystemBuilder(cs)
         while n > 0:
             new_comp = Compartment.create(f'TRANSIT{n}')
             cb.add_compartment(new_comp)
             n -= 1
             cb.add_flow(new_comp, comp, rate)
             comp = new_comp
+        comp = cb.set_bioavailability(comp, dosing_comp.bioavailability)
+        dosing_comp = cb.set_bioavailability(dosing_comp, sympy.Integer(1))
         cb.move_dose(dosing_comp, comp)
         statements = (
             model.statements.before_odes + CompartmentalSystem(cb) + model.statements.after_odes
         )
         model = model.replace(statements=statements)
         model = model.update_source()
     elif len(transits) > n:
@@ -786,15 +894,15 @@
             remaining.remove(trans)
             removed_symbols |= flow.free_symbols
             trans = from_comp
             flow = from_flow
             nremove -= 1
 
         if n == 0:
-            dose = cs.dosing_compartment.dose
+            dose = cs.dosing_compartment[0].dose
             cb.set_dose(destination, dose)
 
         statements = (
             model.statements.before_odes + CompartmentalSystem(cb) + model.statements.after_odes
         )
         model = model.replace(statements=statements)
         model = _update_numerators(model)
@@ -891,15 +999,15 @@
     set_transit_compartments
     remove_lag_time
 
     """
     odes = model.statements.ode_system
     if odes is None:
         raise ValueError(f'Model {model.name} has no ODE system')
-    dosing_comp = odes.dosing_compartment
+    dosing_comp = odes.dosing_compartment[0]
     old_lag_time = dosing_comp.lag_time
     model, mdt_symb = _add_parameter(model, 'MDT', init=_get_absorption_init(model, 'MDT'))
     cb = CompartmentalSystemBuilder(odes)
     cb.set_lag_time(dosing_comp, mdt_symb)
     model = model.replace(
         statements=(
             model.statements.before_odes + CompartmentalSystem(cb) + model.statements.after_odes
@@ -940,15 +1048,15 @@
     add_lag_time
 
 
     """
     odes = model.statements.ode_system
     if odes is None:
         raise ValueError(f'Model {model.name} has no ODE system')
-    dosing_comp = odes.dosing_compartment
+    dosing_comp = odes.dosing_compartment[0]
     lag_time = dosing_comp.lag_time
     if lag_time:
         symbols = lag_time.free_symbols
         cb = CompartmentalSystemBuilder(odes)
         cb.set_lag_time(dosing_comp, sympy.Integer(0))
         statements = (
             model.statements.before_odes + CompartmentalSystem(cb) + model.statements.after_odes
@@ -995,15 +1103,15 @@
     statements = model.statements
     odes = statements.ode_system
     if odes is None:
         raise ValueError(f'Model {model.name} has no ODE system')
     _disallow_infusion(model, odes)
     depot = odes.find_depot(statements)
 
-    dose_comp = odes.dosing_compartment
+    dose_comp = odes.dosing_compartment[0]
     symbols = dose_comp.free_symbols
     dose = dose_comp.dose
     lag_time = dose_comp.lag_time
     if depot:
         to_comp, _ = odes.get_compartment_outflows(depot)[0]
         ka = odes.get_flow(depot, odes.central_compartment)
         assert ka is not None
@@ -1024,15 +1132,15 @@
     model = model.replace(statements=new_statements)
 
     model = remove_unused_parameters_and_rvs(model)
     if not has_zero_order_absorption(model):
         odes = model.statements.ode_system
         assert odes is not None
         model = _add_zero_order_absorption(
-            model, dose.amount, odes.dosing_compartment, 'MAT', lag_time
+            model, dose.amount, odes.dosing_compartment[0], 'MAT', lag_time
         )
         model = model.update_source()
     return model
 
 
 def set_first_order_absorption(model: Model):
     """Set or change to first order absorption rate.
@@ -1069,18 +1177,19 @@
     """
     statements = model.statements
     cs = statements.ode_system
     if cs is None:
         raise ValueError(f'Model {model.name} has no ODE system')
     depot = cs.find_depot(statements)
 
-    dose_comp = cs.dosing_compartment
+    dose_comp = cs.dosing_compartment[0]
     amount = dose_comp.dose.amount
     symbols = dose_comp.free_symbols
     lag_time = dose_comp.lag_time
+    bio = dose_comp.bioavailability
     cb = CompartmentalSystemBuilder(cs)
     if depot and depot == dose_comp:
         dose_comp = cb.set_dose(dose_comp, Bolus(dose_comp.dose.amount))
         dose_comp = cb.set_lag_time(dose_comp, sympy.Integer(0))
     if not depot:
         dose_comp = cb.set_dose(dose_comp, Bolus(amount))
     statements = statements.before_odes + CompartmentalSystem(cb) + statements.after_odes
@@ -1091,15 +1200,15 @@
         mat_assign = statements[mat_idx]
         new_statements = new_statements[0:mat_idx] + mat_assign + new_statements[mat_idx:]
 
     model = model.replace(statements=new_statements)
 
     model = remove_unused_parameters_and_rvs(model)
     if not depot:
-        model, _ = _add_first_order_absorption(model, Bolus(amount), dose_comp, lag_time)
+        model, _ = _add_first_order_absorption(model, Bolus(amount), dose_comp, lag_time, bio)
         model = model.update_source()
     return model
 
 
 def set_bolus_absorption(model: Model):
     """Set or change to bolus absorption rate.
 
@@ -1146,15 +1255,15 @@
         symbols = ka.free_symbols
         statements = statements.before_odes + CompartmentalSystem(cb) + statements.after_odes
         model = model.replace(
             statements=statements.remove_symbol_definitions(symbols, statements.ode_system)
         )
         model = remove_unused_parameters_and_rvs(model)
     if has_zero_order_absorption(model):
-        dose_comp = cs.dosing_compartment
+        dose_comp = cs.dosing_compartment[0]
         old_symbols = dose_comp.free_symbols
         cb = CompartmentalSystemBuilder(cs)
         new_dose = Bolus(dose_comp.dose.amount)
         cb.set_dose(dose_comp, new_dose)
         unneeded_symbols = old_symbols - new_dose.free_symbols
         statements = statements.before_odes + CompartmentalSystem(cb) + statements.after_odes
         model = model.replace(
@@ -1205,30 +1314,30 @@
     statements = model.statements
     cs = statements.ode_system
     if cs is None:
         raise ValueError(f'Model {model.name} has no ODE system')
     _disallow_infusion(model, cs)
     depot = cs.find_depot(statements)
 
-    dose_comp = cs.dosing_compartment
+    dose_comp = cs.dosing_compartment[0]
     have_ZO = has_zero_order_absorption(model)
     if depot and not have_ZO:
         model = _add_zero_order_absorption(model, dose_comp.amount, depot, 'MDT')
     elif not depot and have_ZO:
         model, _ = _add_first_order_absorption(model, dose_comp.dose, dose_comp)
     elif not depot and not have_ZO:
         amount = dose_comp.dose.amount
         model, depot = _add_first_order_absorption(model, Bolus(amount), dose_comp)
         model = _add_zero_order_absorption(model, amount, depot, 'MDT')
     model = model.update_source()
     return model
 
 
 def _disallow_infusion(model, odes):
-    dose_comp = odes.dosing_compartment
+    dose_comp = odes.dosing_compartment[0]
     if isinstance(dose_comp.dose, Infusion):
         if dose_comp.dose.rate is not None:
             ex = dose_comp.dose.rate
         else:
             ex = dose_comp.dose.duration
         assert ex is not None
 
@@ -1259,15 +1368,15 @@
     >>> has_zero_order_absorption(model)
     False
 
     """
     cs = model.statements.ode_system
     if cs is None:
         raise ValueError(f'Model {model.name} has no ODE system')
-    dosing = cs.dosing_compartment
+    dosing = cs.dosing_compartment[0]
     dose = dosing.dose
     if isinstance(dose, Infusion):
         if dose.rate is None:
             value = dose.duration
         else:
             value = dose.rate
         if isinstance(value, sympy.Symbol) or isinstance(value, str):
@@ -1294,35 +1403,39 @@
         model, mat_symb = _add_parameter(
             model, parameter_name, init=_get_absorption_init(model, parameter_name)
         )
     new_dose = Infusion(amount, duration=mat_symb * 2)
     cb = CompartmentalSystemBuilder(model.statements.ode_system)
     cb.set_dose(to_comp, new_dose)
     if lag_time is not None and lag_time != 0:
-        cb.set_lag_time(model.statements.ode_system.dosing_compartment, lag_time)
+        cb.set_lag_time(model.statements.ode_system.dosing_compartment[0], lag_time)
     model = model.replace(
         statements=model.statements.before_odes
         + CompartmentalSystem(cb)
         + model.statements.after_odes
     )
     return model
 
 
-def _add_first_order_absorption(model, dose, to_comp, lag_time=None):
+def _add_first_order_absorption(model, dose, to_comp, lag_time=None, bioavailability=None):
     """Add first order absorption
     Disregards what is currently in the model.
     """
     odes = model.statements.ode_system
     cb = CompartmentalSystemBuilder(odes)
     depot = Compartment.create(
-        'DEPOT', dose=dose, lag_time=sympy.Integer(0) if lag_time is None else lag_time
+        'DEPOT',
+        dose=dose,
+        lag_time=sympy.Integer(0) if lag_time is None else lag_time,
+        bioavailability=sympy.Integer(1) if bioavailability is None else bioavailability,
     )
     cb.add_compartment(depot)
     to_comp = cb.set_dose(to_comp, None)
     to_comp = cb.set_lag_time(to_comp, sympy.Integer(0))
+    to_comp = cb.set_bioavailability(to_comp, sympy.Integer(1))
 
     mat_assign = model.statements.find_assignment('MAT')
     if mat_assign:
         mat_symb = mat_assign.symbol
     else:
         model, mat_symb = _add_parameter(model, 'MAT', _get_absorption_init(model, 'MAT'))
     cb.add_flow(depot, to_comp, 1 / mat_symb)
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/parameter_sampling.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/parameter_variability.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/parameter_variability.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/parameters.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/pd.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/pd.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 )
 
 from .error import set_proportional_error_model
 from .odes import add_individual_parameter, set_initial_estimates
 
 
 def add_effect_compartment(model: Model, expr: str):
-    """Add an effect compartment
+    r"""Add an effect compartment.
+
+    Implemented PD models are:
+
+    * Baseline: :math:`E = E_0`
+    * Linear: :math:`E = E_0 + S \cdot C`
+    * Emax: :math:`E = E_0 + \frac {E_{max} \cdot C } { EC_{50} + C }`
+    * Step effect: :math:`E = \Biggl \lbrace { E_0 \quad  \text{ if C } < 0 \atop E_0 + E_{max} \quad  \text{else}}`
+    * Sigmoidal: :math:`E = \frac {E_{max} C^n} { EC_{50}^n + C^n}`
+    * Log-linear: :math:`E = m \cdot  \text{log}(C + C_0)`
 
     Parameters
     ----------
     model : Model
         Pharmpy model
     expr : str
-        Name of PD effect function. The function can either be
-        * baseline: E = E0
-        * step effect: Emax = theta if C > 0 else 0, E = E0 + Emax
-        * linear: E = E0 + S * C
-        * Emax: E = E0 + Emax * C / (EC50 + C)
-        * sigmoidal: E = Emax * C^n / (EC50^n + C^n)
-        * log-lin: E = m * log(C + C0)
-        Valid strings are: baseline, linear, Emax, sigmoid, step, loglin
+        Name of the PD effect function. Valid names are: baseline, linear, Emax, sigmoid, step, loglin
 
     Return
     ------
     Model
         Pharmpy model object
 
     Examples
@@ -69,40 +71,48 @@
     conc_e = model.statements.ode_system.find_compartment("EFFECT").amount / vc
 
     model = _add_effect(model, expr, conc_e)
     return model
 
 
 def set_direct_effect(model: Model, expr: str):
-    """Add an effect to a model
+    r"""Add an effect to a model.
+
+    Implemented PD models are:
+
+    * Baseline: :math:`E = E_0`
+    * Linear: :math:`E = E_0 + S \cdot C`
+    * Emax: :math:`E = E_0 + \frac {E_{max} \cdot C } { EC_{50} + C }`
+    * Step effect: :math:`E = \Biggl \lbrace { E_0 \quad  \text{ if C } < 0 \atop E_0 + E_{max} \quad  \text{else}}`
+    * Sigmoidal: :math:`E = \frac {E_{max} C^n} { EC_{50}^n + C^n}`
+    * Log-linear: :math:`E = m \cdot  \text{log}(C + C_0)`
 
     Parameters
     ----------
     model : Model
         Pharmpy model
     expr : str
-        Name of PD effect function. The function can either be
-        * baseline: E = E0
-        * step effect: Emax = theta if C > 0 else 0, E = E0 + Emax
-        * linear: E = E0 + S * C
-        * Emax: E = E0 + Emax * C / (EC50 + C)
-        * sigmoidal: E = Emax * C^n / (EC50^n + C^n)
-        * log-lin: E = m * log(C + C0)
-        Valid strings are: baseline, linear, Emax, sigmoid, step, loglin
+        Name of PD effect function. Valid names are: baseline, linear, Emax, sigmoid, step, loglin
 
     Return
     ------
     Model
         Pharmpy model object
 
     Examples
     --------
+    >>> from pharmpy.modeling import *
+    >>> model = load_example_model("pheno")
+    >>> model = set_direct_effect(model, "linear")
+    >>> model.statements.find_assignment("E")
+        A_CENTRAL⋅S
+        ─────────── + E₀
+    E =      V
 
     """
-    # vc = sympy.Symbol("VC") # must be changed later
     vc, cl = _get_central_volume_and_cl(model)
     conc = model.statements.ode_system.central_compartment.amount / vc
 
     model = _add_effect(model, expr, conc)
 
     return model
 
@@ -136,15 +146,15 @@
     elif expr == "linear":
         s = sympy.Symbol("S")  # slope
         model = add_individual_parameter(model, s.name)
         E = Assignment(sympy.Symbol('E'), e0 + s * conc)
     elif expr == "Emax":
         E = Assignment(sympy.Symbol("E"), e0 + emax * conc / (ec50 + conc))
     elif expr == "step":
-        E = Assignment(sympy.Symbol("E"), sympy.Piecewise((0, conc < 0), (emax, True)))
+        E = Assignment(sympy.Symbol("E"), sympy.Piecewise((e0, conc < 0), (e0 + emax, True)))
     elif expr == "sigmoid":
         n = sympy.Symbol("n")  # Hill coefficient
         model = add_individual_parameter(model, n.name)
         model = set_initial_estimates(model, {"POP_n": 1})
         E = Assignment(sympy.Symbol("E"), emax * conc**n / (ec50**n + conc**n))
     elif expr == "loglin":
         m = sympy.Symbol("m")  # slope
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/plots.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/results.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/tmdd.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/tmdd.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,18 @@
         cb.set_input(
             target_comp,
             ksyn * vc
             - kdeg * target_amount
             - (kint - kdeg) * target_amount * lafree_symb / (kd + lafree_symb),
         )
 
+        # FIXME: should others also have flows?
+        central = cb.find_compartment('CENTRAL')
+        cb.add_flow(central, output, lafree_symb * elimination_rate)
+
         lafreef = sympy.Symbol("LAFREEF")
         lafree_final = Assignment(lafreef, lafree_expr)
         before = model.statements.before_odes + (ksyn_ass, kd_ass, lafree_ass)
         after = lafree_final + model.statements.after_odes
         ipred = lafreef / vc
         after = after.reassign(sympy.Symbol('IPRED'), ipred)  # FIXME: Assumes an IPRED
     elif type == 'WAGNER':
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/units.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/modeling/write_csv.py` & `pharmpy-core-0.98.0/src/pharmpy/modeling/write_csv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/reporting/altairplot.py` & `pharmpy-core-0.98.0/src/pharmpy/reporting/altairplot.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/reporting/custom.css` & `pharmpy-core-0.98.0/src/pharmpy/reporting/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/reporting/reporting.py` & `pharmpy-core-0.98.0/src/pharmpy/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/results.py` & `pharmpy-core-0.98.0/src/pharmpy/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/__init__.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/allometry/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/allometry/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/amd/funcs.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/amd/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/amd/run.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/amd/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from .results import AMDResults
 
 
 def run_amd(
     input: Union[Model, Path, str],
     results: Optional[ModelfitResults] = None,
     modeltype: str = 'basic_pk',
-    administraton: str = 'oral',
+    administration: str = 'oral',
     cl_init: float = 0.01,
     vc_init: float = 1.0,
     mat_init: float = 0.1,
     search_space: Optional[str] = None,
     lloq_method: Optional[str] = None,
     lloq_limit: Optional[str] = None,
     order: Optional[List[str]] = None,
@@ -55,15 +55,15 @@
     Parameters
     ----------
     input : Model or Path
         Read model object/Path to a dataset
     results : ModelfitResults
         Reults of input if input is a model
     modeltype : str
-        Type of model to build. Either 'basic_pl' or 'tmdd'
+        Type of model to build. Either 'basic_pk' or 'tmdd'
     administration : str
         Route of administration. Either 'iv' or 'oral'
     cl_init : float
         Initial estimate for the population clearance
     vc_init : float
         Initial estimate for the central compartment population volume
     mat_init : float
@@ -102,14 +102,20 @@
     --------
     run_iiv
     run_tool
 
     """
     from pharmpy.model.external import nonmem  # FIXME We should not depend on NONMEM
 
+    # FIXME: temporary until modeltype and administration is fully supported in e.g. create_start_model
+    if modeltype == 'basic_pk' and administration == 'iv':
+        modeltype = 'pk_iv'
+    elif modeltype == 'basic_pk' and administration == 'oral':
+        modeltype = 'pk_oral'
+
     if type(input) is str:
         from pharmpy.tools.amd.funcs import create_start_model
 
         model = create_start_model(
             input, modeltype=modeltype, cl_init=cl_init, vc_init=vc_init, mat_init=mat_init
         )
         model = convert_model(model, 'nonmem')  # FIXME: Workaround for results retrieval system
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/bootstrap/report.rst` & `pharmpy-core-0.98.0/src/pharmpy/tools/bootstrap/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/bootstrap/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/bootstrap/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/bootstrap/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/bootstrap/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/cdd/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/cdd/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/common.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/covsearch/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/covsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/crossval/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/crossval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/estmethod/algorithms.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/estmethod/algorithms.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,93 +2,95 @@
 
 from pharmpy.modeling import add_estimation_step, remove_estimation_step, set_ode_solver
 from pharmpy.tools.common import update_initial_estimates
 from pharmpy.tools.modelfit import create_fit_workflow
 from pharmpy.workflows import Task, Workflow
 
 
-def exhaustive(methods, solvers):
+def exhaustive(methods, solvers, covs):
     wf = Workflow()
 
     task_start = Task('start', start)
     wf.add_task(task_start)
 
     candidate_no = 1
-    for method, solver in itertools.product(methods, solvers):
-        wf_estmethod = _create_candidate_model_wf(candidate_no, method, solver, update=False)
+    for method, solver, cov in itertools.product(methods, solvers, covs):
+        wf_estmethod = _create_candidate_model_wf(candidate_no, method, solver, cov, update=False)
         wf.insert_workflow(wf_estmethod, predecessors=task_start)
         candidate_no += 1
 
     return wf, None
 
 
-def exhaustive_with_update(methods, solvers):
+def exhaustive_with_update(methods, solvers, covs):
     wf = Workflow()
 
     task_base_model = Task('create_base_model', _create_base_model)
     wf.add_task(task_base_model)
     wf_fit = create_fit_workflow(n=1)
     wf.insert_workflow(wf_fit, predecessors=task_base_model)
     task_base_model_fit = wf.output_tasks
 
     candidate_no = 1
-    for method, solver in itertools.product(methods, solvers):
+    for method, solver, cov in itertools.product(methods, solvers, covs):
         # This is equivalent to the base model
         if not (method == 'FOCE' and solver is None):
             # Create model with original estimates
             wf_estmethod_original = _create_candidate_model_wf(
-                candidate_no, method, solver, update=False
+                candidate_no, method, solver, cov, update=False
             )
             wf.insert_workflow(wf_estmethod_original, predecessors=task_base_model_fit)
             candidate_no += 1
 
         # Create model with updated estimates from FOCE
-        wf_estmethod_update = _create_candidate_model_wf(candidate_no, method, solver, update=True)
+        wf_estmethod_update = _create_candidate_model_wf(
+            candidate_no, method, solver, cov, update=True
+        )
         wf.insert_workflow(wf_estmethod_update, predecessors=task_base_model_fit)
         candidate_no += 1
 
     return wf, task_base_model_fit
 
 
-def exhaustive_only_eval(methods, solvers):
+def exhaustive_only_eval(methods, solvers, covs):
     wf = Workflow()
 
     task_start = Task('start', start)
     wf.add_task(task_start)
 
     candidate_no = 1
-    for method, solver in itertools.product(methods, solvers):
+    for method, solver, cov in itertools.product(methods, solvers, covs):
         wf_estmethod = _create_candidate_model_wf(
-            candidate_no, method, solver, update=False, is_eval_candidate=True
+            candidate_no, method, solver, cov, update=False, is_eval_candidate=True
         )
         wf.insert_workflow(wf_estmethod, predecessors=task_start)
         candidate_no += 1
 
     return wf, None
 
 
 def start(model):
     return model
 
 
-def _create_candidate_model_wf(candidate_no, method, solver, update, is_eval_candidate=False):
+def _create_candidate_model_wf(candidate_no, method, solver, cov, update, is_eval_candidate=False):
     wf = Workflow()
 
     model_name = f'estmethod_run{candidate_no}'
     task_copy = Task('copy_model', _copy_model, model_name)
     wf.add_task(task_copy)
 
     if update:
         task_update_inits = Task('update_inits', update_initial_estimates)
         wf.add_task(task_update_inits, predecessors=task_copy)
         task_prev = task_update_inits
     else:
         task_prev = task_copy
     task_create_candidate = Task(
-        'create_candidate', _create_candidate_model, method, solver, update, is_eval_candidate
+        'create_candidate', _create_candidate_model, method, solver, cov, update, is_eval_candidate
     )
     wf.add_task(task_create_candidate, predecessors=task_prev)
     return wf
 
 
 def _copy_model(name, model):
     return model.replace(name=name)
@@ -108,22 +110,24 @@
         base_model = remove_estimation_step(base_model, 0)
 
     base_model = add_estimation_step(base_model, **est_settings)
     base_model = add_estimation_step(base_model, **eval_settings)
     return base_model
 
 
-def _create_candidate_model(method, solver, update, is_eval_candidate, model):
+def _create_candidate_model(method, solver, cov, update, is_eval_candidate, model):
     est_settings = _create_est_settings(method, is_eval_candidate)
     laplace = True if method == 'LAPLACE' else False
-    eval_settings = _create_eval_settings(laplace)
+    eval_settings = _create_eval_settings(laplace, cov)
 
     eval_method = eval_settings['method']
     model = model.replace(
-        description=_create_description([method, eval_method], solver=solver, update=update)
+        description=_create_description(
+            [method, eval_method], solver=solver, cov=cov, update=update
+        )
     )
 
     while len(model.estimation_steps) > 0:
         model = remove_estimation_step(model, 0)
 
     model = add_estimation_step(model, **est_settings)
     model = add_estimation_step(model, **eval_settings)
@@ -135,46 +139,50 @@
 def _create_est_settings(method, is_eval_candidate=False):
     est_settings = {
         'method': method,
         'interaction': True,
         'laplace': False,
         'auto': True,
         'keep_every_nth_iter': 10,
+        'cov': None,
     }
 
     if method == 'LAPLACE':
         est_settings['method'] = 'FOCE'
         est_settings['laplace'] = True
 
     if is_eval_candidate:
         est_settings['evaluation'] = True
     else:
         est_settings['maximum_evaluations'] = 9999
 
     return est_settings
 
 
-def _create_eval_settings(laplace=False):
+def _create_eval_settings(laplace=False, cov=None):
     eval_settings = {
         'method': 'IMP',
         'interaction': True,
         'evaluation': True,
         'laplace': False,
         'maximum_evaluations': 9999,
         'isample': 10000,
         'niter': 10,
         'keep_every_nth_iter': 10,
+        'cov': cov,
     }
 
     if laplace:
         eval_settings['laplace'] = True
 
     return eval_settings
 
 
-def _create_description(methods, solver, update=False):
+def _create_description(methods, solver, cov, update=False):
     model_description = ','.join(methods)
     if solver:
         model_description += f';{solver}'
+    if cov:
+        model_description += f';{cov}'
     if update:
         model_description += ' (update)'
     return model_description
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/estmethod/report.rst` & `pharmpy-core-0.98.0/src/pharmpy/tools/estmethod/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/estmethod/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/estmethod/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 from pharmpy.tools import summarize_errors, summarize_modelfit_results
 from pharmpy.tools.common import ToolResults
 from pharmpy.tools.modelfit import create_fit_workflow
 from pharmpy.workflows import Task, Workflow
 
 EST_METHODS = ('FOCE', 'FO', 'IMP', 'IMPMAP', 'ITS', 'SAEM', 'LAPLACE', 'BAYES')
 SOLVERS = ('CVODES', 'DGEAR', 'DVERK', 'IDA', 'LSODA', 'LSODI')
+COVS = ('SANDWICH', 'CPG', 'OFIM')
 
 ALGORITHMS = frozenset(['exhaustive', 'exhaustive_with_update', 'exhaustive_only_eval'])
 
 
 def create_workflow(
     algorithm: str,
     methods: Optional[Union[List[str], str]] = None,
     solvers: Optional[Union[List[str], str]] = None,
+    covs: Optional[Union[List[str], str]] = None,
     results: Optional[ModelfitResults] = None,
     model: Optional[Model] = None,
 ):
     """Run estmethod tool.
 
     Parameters
     ----------
@@ -36,14 +38,17 @@
         The algorithm to use (can be 'exhaustive', 'exhaustive_with_update' or 'exhaustive_only_eval')
     methods : list or None
         List of estimation methods to test. Can be specified as 'all', a list of methods, or
         None (to not test any estimation method)
     solvers : list, str or None
         List of solver to test. Can be specified as 'all', a list of solvers, or None (to
         not test any solver)
+    covs : list, str or None
+        List of covariance to test. Can be specified as 'all', a list of covs, or None (to
+        not evaluate any covariance)
     results : ModelfitResults
         Results for model
     model : Model
         Pharmpy model
 
     Returns
     -------
@@ -53,15 +58,18 @@
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> from pharmpy.tools import run_estmethod, load_example_modelfit_results
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> methods = ['imp', 'saem']
-    >>> run_estmethod('reduced', methods=methods, solvers='all', results=results, model=model) # doctest: +SKIP
+    >>> covs = None
+    >>> run_estmethod( # doctest: +SKIP
+    >>>     'reduced', methods=methods, solvers='all', covs=covs, results=results, model=model # doctest: +SKIP
+    >>> ) # doctest: +SKIP
 
     """
     wf = Workflow()
     wf.name = "estmethod"
 
     algorithm_func = getattr(algorithms, algorithm)
 
@@ -72,15 +80,17 @@
 
     wf.add_task(start_task)
 
     if methods is None:
         methods = [model.estimation_steps[-1].method]
 
     wf_algorithm, task_base_model_fit = algorithm_func(
-        _format_input(methods, EST_METHODS), _format_input(solvers, SOLVERS)
+        _format_input(methods, EST_METHODS),
+        _format_input(solvers, SOLVERS),
+        _format_input(covs, COVS),
     )
     wf.insert_workflow(wf_algorithm, predecessors=start_task)
 
     wf_fit = create_fit_workflow(n=len(wf.output_tasks))
     wf.insert_workflow(wf_fit, predecessors=wf.output_tasks)
 
     if task_base_model_fit:
@@ -173,36 +183,39 @@
         dfs[model.name] = df.drop(columns=['tool_options'])
 
     return pd.concat(dfs.values(), keys=dfs.keys())
 
 
 @with_runtime_arguments_type_check
 @with_same_arguments_as(create_workflow)
-def validate_input(algorithm, methods, solvers, model):
+def validate_input(algorithm, methods, solvers, covs, model):
     if solvers is not None and has_linear_odes(model):
         raise ValueError(
             'Invalid input `model`: testing non-linear solvers on linear system is not supported'
         )
 
     if algorithm not in ALGORITHMS:
         raise ValueError(
             f'Invalid `algorithm`: got `{algorithm}`, must be one of {sorted(ALGORITHMS)}.'
         )
 
-    if methods is None and solvers is None:
+    if methods is None and solvers is None and covs is None:
         raise ValueError(
-            'Invalid search space options: please specify at least `methods` or `solvers`'
+            'Invalid search space options: please specify at least one of `methods`, `solvers`, or `covs`'
         )
 
     if methods is not None:
         _validate_search_space(methods, EST_METHODS, 'methods')
 
     if solvers is not None:
         _validate_search_space(solvers, SOLVERS, 'solvers')
 
+    if covs is not None:
+        _validate_search_space(covs, COVS, 'covs')
+
 
 def _validate_search_space(input_search_space, allowed_search_space, option_name):
     if isinstance(input_search_space, str):
         if input_search_space != 'all':
             raise ValueError(
                 f'Invalid `{option_name}`: if option is str it must be `all`, got {input_search_space}'
             )
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/evaldesign/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/evaldesign/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/external/nlmixr/__init__.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/external/nlmixr/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/external/nlmixr/run.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/external/nlmixr/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/__init__.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/config.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/results_file.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/external/nonmem/run.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/external/nonmem/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/external/rxode/__init__.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/external/rxode/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/external/rxode/run.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/external/rxode/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/frem/models.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/frem/models.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/frem/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/frem/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/frem/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/frem/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/funcs/ml.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/funcs/ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite` & `pharmpy-core-0.98.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite` & `pharmpy-core-0.98.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/funcs/summarize_individuals.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/funcs/summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/iivsearch/algorithms.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/iivsearch/algorithms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-from typing import Dict, Tuple
+from typing import Dict, List, Set, Tuple
 
 import pharmpy.tools.modelfit as modelfit
 from pharmpy.internals.expr.subs import subs
 from pharmpy.internals.set.partitions import partitions
 from pharmpy.internals.set.subsets import non_empty_subsets
 from pharmpy.model import Model, RandomVariables
 from pharmpy.modeling import create_joint_distribution, remove_iiv, split_joint_distribution
 from pharmpy.modeling.expressions import get_rv_parameters
 from pharmpy.results import mfr
 from pharmpy.tools.common import update_initial_estimates
 from pharmpy.workflows import Task, Workflow
 
 
-def brute_force_no_of_etas(base_model, index_offset=0):
+def brute_force_no_of_etas(base_model, index_offset=0, keep=[]):
     wf = Workflow()
 
     base_model = base_model.replace(description=create_description(base_model))
 
     iivs = base_model.random_variables.iiv
+    iiv_names = iivs.names
+    if len(keep) > 0:
+        iiv_names = set(iiv_names) - _get_eta_from_parameter(base_model, keep)
 
-    for i, to_remove in enumerate(non_empty_subsets(iivs.names), 1):
+    for i, to_remove in enumerate(non_empty_subsets(iiv_names), 1):
         model_name = f'iivsearch_run{i + index_offset}'
         task_copy = Task('copy', copy, model_name)
         wf.add_task(task_copy)
 
         task_update_inits = Task('update_inits', update_initial_estimates)
         wf.add_task(task_update_inits, predecessors=task_copy)
 
@@ -145,7 +148,18 @@
     return model_copy
 
 
 def update_description(model):
     description = create_description(model)
     model = model.replace(description=description)
     return model
+
+
+def _get_eta_from_parameter(model: Model, parameters: List[str]) -> Set[str]:
+    # returns list of eta names from parameter names
+    iiv_set = set()
+    iiv_names = model.random_variables.names
+    for iiv_name in iiv_names:
+        param = get_rv_parameters(model, iiv_name)
+        if set(param).issubset(parameters) and len(param) > 0:
+            iiv_set.add(iiv_name)
+    return iiv_set
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/iivsearch/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/iivsearch/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Optional, Set, Union
 
 import pharmpy.tools.iivsearch.algorithms as algorithms
 from pharmpy.deps import pandas as pd
 from pharmpy.internals.fn.signature import with_same_arguments_as
 from pharmpy.internals.fn.type import with_runtime_arguments_type_check
 from pharmpy.model import Model
-from pharmpy.modeling import add_pk_iiv, calculate_bic, create_joint_distribution
+from pharmpy.modeling import add_pk_iiv, calculate_bic, create_joint_distribution, has_random_effect
 from pharmpy.modeling.results import RANK_TYPES
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import summarize_modelfit_results
 from pharmpy.tools.common import ToolResults, create_results, update_initial_estimates
 from pharmpy.tools.modelfit import create_fit_workflow
 from pharmpy.workflows import Task, Workflow, call_workflow
 
@@ -31,14 +31,15 @@
 def create_workflow(
     algorithm: str,
     iiv_strategy: str = 'no_add',
     rank_type: str = 'bic',
     cutoff: Optional[Union[float, int]] = None,
     results: Optional[ModelfitResults] = None,
     model: Optional[Model] = None,
+    keep: Optional[List[str]] = [],
 ):
     """Run IIVsearch tool. For more details, see :ref:`iivsearch`.
 
     Parameters
     ----------
     algorithm : str
         Which algorithm to run (brute_force, brute_force_no_of_etas, brute_force_block_structure)
@@ -67,22 +68,24 @@
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> run_iivsearch('brute_force', results=results, model=model)   # doctest: +SKIP
     """
 
     wf = Workflow()
     wf.name = 'iivsearch'
-    start_task = Task('start_iiv', start, model, algorithm, iiv_strategy, rank_type, cutoff)
+    start_task = Task('start_iiv', start, model, algorithm, iiv_strategy, rank_type, cutoff, keep)
     wf.add_task(start_task)
     task_results = Task('results', _results)
     wf.add_task(task_results, predecessors=[start_task])
     return wf
 
 
-def create_algorithm_workflow(input_model, base_model, state, iiv_strategy, rank_type, cutoff):
+def create_algorithm_workflow(
+    input_model, base_model, state, iiv_strategy, rank_type, cutoff, keep
+):
     wf: Workflow[IIVSearchResults] = Workflow()
 
     start_task = Task(f'start_{state.algorithm}', _start_algorithm, base_model)
     wf.add_task(start_task)
 
     if iiv_strategy != 'no_add':
         wf_fit = create_fit_workflow(n=1)
@@ -91,28 +94,31 @@
     else:
         base_model_task = start_task
 
     index_offset = len(
         [model_name for model_name in state.model_names_so_far if 'base' not in model_name]
     )
     algorithm_func = getattr(algorithms, state.algorithm)
-    wf_method = algorithm_func(base_model, index_offset)
+    if state.algorithm == "brute_force_no_of_etas":
+        wf_method = algorithm_func(base_model, index_offset, keep)
+    else:
+        wf_method = algorithm_func(base_model, index_offset)
     wf.insert_workflow(wf_method)
 
     task_result = Task(
         'results', post_process, state, rank_type, cutoff, input_model, base_model.name
     )
 
     post_process_tasks = [base_model_task] + wf.output_tasks
     wf.add_task(task_result, predecessors=post_process_tasks)
 
     return wf
 
 
-def start(context, input_model, algorithm, iiv_strategy, rank_type, cutoff):
+def start(context, input_model, algorithm, iiv_strategy, rank_type, cutoff, keep):
     if iiv_strategy != 'no_add':
         model_iiv = input_model.replace(name='base_model')
         model_iiv = update_initial_estimates(model_iiv)
         base_model = _add_iiv(iiv_strategy, model_iiv)
         base_model = algorithms.update_description(base_model)
     else:
         base_model = input_model
@@ -128,15 +134,15 @@
     last_res = None
     final_model = None
 
     for i, algorithm_cur in enumerate(list_of_algorithms):
         state = State(algorithm_cur, models_set, input_model.name)
         # NOTE Execute algorithm
         wf = create_algorithm_workflow(
-            input_model, base_model, state, iiv_strategy, rank_type, cutoff
+            input_model, base_model, state, iiv_strategy, rank_type, cutoff, keep
         )
         res = call_workflow(wf, f'results_{algorithm}', context)
         # NOTE Append results
         new_models = list(filter(lambda model: model.name not in models_set, res.models))
         models.extend(new_models)
         models_set.update(model.name for model in new_models)
 
@@ -258,14 +264,16 @@
 
 @with_runtime_arguments_type_check
 @with_same_arguments_as(create_workflow)
 def validate_input(
     algorithm,
     iiv_strategy,
     rank_type,
+    model,
+    keep,
 ):
     if algorithm not in IIV_ALGORITHMS:
         raise ValueError(
             f'Invalid `algorithm`: got `{algorithm}`, must be one of {sorted(IIV_ALGORITHMS)}.'
         )
 
     if rank_type not in RANK_TYPES:
@@ -275,11 +283,18 @@
 
     if iiv_strategy not in IIV_STRATEGIES:
         raise ValueError(
             f'Invalid `iiv_strategy`: got `{iiv_strategy}`,'
             f' must be one of {sorted(IIV_STRATEGIES)}.'
         )
 
+    if len(keep) > 0:
+        for parameter in keep:
+            try:
+                has_random_effect(model, parameter, "iiv")
+            except KeyError:
+                raise ValueError(f"Parameter {parameter} has no iiv.")
+
 
 @dataclass(frozen=True)
 class IIVSearchResults(ToolResults):
     pass
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/iovsearch/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/iovsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/linearize/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/linearize/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/linearize/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/linearize/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/absorption.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/covariate.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/elimination.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/peripherals.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/peripherals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/feature/transits.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/filter.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/filter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/grammar.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/grammar.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/helpers.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/interpreter.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/parse.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/definition.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/definition.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/absorption.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/covariate.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/elimination.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/statement/feature/transits.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/statement/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/mfl/stringify.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/mfl/stringify.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/modelfit/__init__.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/modelfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/modelfit/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/modelfit/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/modelsearch/algorithms.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/modelsearch/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/modelsearch/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/modelsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/psn_helpers.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/psn_helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/qa/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/qa/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/rankfuncs.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/reporting.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/reporting.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/run.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,14 +907,16 @@
     >>> summarize_modelfit_results(model.modelfit_results) # doctest: +SKIP
                      description  minimization_successful ...        ofv  ... runtime_total  ...
     pheno PHENOBARB SIMPLE MODEL                     True ... 586.276056  ...           4.0  ...
     """
     if isinstance(results, ModelfitResults):
         results = [results]
 
+    if results is None:
+        raise ValueError('Option `results` is None')
     if all(res is None for res in results):
         raise ValueError('All input results are empty')
 
     summaries = []
 
     for res in results:
         if res is not None:
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/ruvsearch/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/ruvsearch/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/ruvsearch/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/ruvsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/scm/psn_wrapper.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/scm/psn_wrapper.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/scm/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/scm/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/simeval/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/simeval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/simfit/results.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/simfit/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/structsearch/tmdd.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/structsearch/tmdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/structsearch/tool.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/structsearch/tool.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
 
 from pharmpy.deps import numpy as np
+from pharmpy.deps import pandas as pd
 from pharmpy.internals.fn.signature import with_same_arguments_as
 from pharmpy.internals.fn.type import with_runtime_arguments_type_check
 from pharmpy.model import Model
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import summarize_modelfit_results
-from pharmpy.tools.common import ToolResults
+from pharmpy.tools.common import ToolResults, create_results
 from pharmpy.tools.modelfit import create_fit_workflow
 from pharmpy.workflows import Task, Workflow, call_workflow
 
+from .pkpd import create_pkpd_models
 from .tmdd import create_qss_models, create_remaining_models
 
 ROUTES = frozenset(('iv', 'oral'))
-TYPES = frozenset(('tmdd',))
+TYPES = frozenset(('tmdd', 'pkpd'))
 
 
 def create_workflow(
     route: str,
     type: str,
     results: Optional[ModelfitResults] = None,
     model: Optional[Model] = None,
@@ -28,15 +30,15 @@
     """Run the structsearch tool. For more details, see :ref:`structsearch`.
 
     Parameters
     ----------
     route : str
         Route of administration. Either 'pk' or 'oral'
     type : str
-        Type of model. Currently only 'tmdd'
+        Type of model. Currently only 'tmdd' and 'pkpd'
     results : ModelfitResults
         Results for the start model
     model : Model
         Pharmpy start model
 
     Returns
     -------
@@ -50,18 +52,19 @@
     >>> model = load_example_model("pheno")
     >>> results = load_example_modelfit_results("pheno")
     >>> run_structsearch(model_type='tmdd', results=results, model=model)   # doctest: +SKIP
     """
 
     wf = Workflow()
     wf.name = 'structsearch'
-    start_task = Task('run_tmdd', run_tmdd, model)
+    if type == 'tmdd':
+        start_task = Task('run_tmdd', run_tmdd, model)
+    elif type == 'pkpd':
+        start_task = Task('run_pkpd', run_pkpd, model)
     wf.add_task(start_task)
-    results_task = Task('results', _results)
-    wf.add_task(results_task, predecessors=[start_task])
     return wf
 
 
 def run_tmdd(context, model):
     qss_candidate_models = create_qss_models(model)
 
     wf = create_fit_workflow(qss_candidate_models)
@@ -75,21 +78,52 @@
 
     models = create_remaining_models(model, best_qss_model.modelfit_results.parameter_estimates)
     wf2 = create_fit_workflow(models)
     task_results = Task('results', bundle_results)
     wf.add_task(task_results, predecessors=wf2.output_tasks)
     run_models = call_workflow(wf, 'results_remaining', context)
 
-    summary_models = summarize_modelfit_results(
+    summary_input = summarize_modelfit_results(model.modelfit_results)
+    summary_candidates = summarize_modelfit_results(
         [model.modelfit_results for model in qss_run_models + run_models]
     )
 
-    res = StructSearchResults(summary_models=summary_models)
+    return create_results(
+        StructSearchResults,
+        model,
+        model,
+        qss_run_models + run_models,
+        rank_type='bic',
+        cutoff=None,
+        summary_models=pd.concat([summary_input, summary_candidates], keys=[0, 1], names=['step']),
+    )
+
+
+def run_pkpd(context, model):
+    pkpd_models = create_pkpd_models(model, model.modelfit_results.parameter_estimates)
+
+    wf = create_fit_workflow(pkpd_models)
+    task_results = Task('results2', bundle_results)
+    wf.add_task(task_results, predecessors=wf.output_tasks)
+    pkpd_models_fit = call_workflow(wf, 'results_remaining', context)
+
+    summary_input = summarize_modelfit_results(model.modelfit_results)
+    summary_candidates = summarize_modelfit_results(
+        [model.modelfit_results for model in pkpd_models_fit]
+    )
 
-    return res
+    return create_results(
+        StructSearchResults,
+        model,
+        model,
+        list(pkpd_models_fit),
+        rank_type='bic',
+        cutoff=None,
+        summary_models=pd.concat([summary_input, summary_candidates], keys=[0, 1], names=["step"]),
+    )
 
 
 def bundle_results(*args):
     return args
 
 
 def _results(model):
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy/tools/wrap.py` & `pharmpy-core-0.98.0/src/pharmpy/tools/wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/visualization.py` & `pharmpy-core-0.98.0/src/pharmpy/visualization.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/__init__.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/args.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/args.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/call.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/call.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/dispatchers/local_dask.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/dispatchers/local_dask.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/execute.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/execute.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/log.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/log.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/model_database/baseclass.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/model_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/model_database/local_directory.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/model_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/model_database/null_database.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/model_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/optimize.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/optimize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/tool_database/baseclass.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/tool_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/tool_database/local_directory.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/tool_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/tool_database/null_database.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/tool_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy/workflows/workflow.py` & `pharmpy-core-0.98.0/src/pharmpy/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/src/pharmpy_core.egg-info/PKG-INFO` & `pharmpy-core-0.98.0/src/pharmpy_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.97.0
+Version: 0.98.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -40,14 +40,33 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.98.0 (2023-07-21)
+-------------------
+
+New features
+============
+
+* Support for multiple doses
+* Add function ``modeling.add_bioavailability``
+* Add function ``modeling.remove_bioavailability``
+* Support for PKPD models in structsearch
+* Option to keep IIVs in IIVSearch
+* Option to test uncertainty methods in Estmethod
+* Autogenerate CMT column
+
+Changes
+=======
+
+* Rename BLQ flag datainfo typ to ``blqdv``
+
 0.97.0 (2023-06-28)
 -------------------
 
 New features
 ============
 
 * Support BLQ transformations in RUVSearch
```

### Comparing `pharmpy-core-0.97.0/src/pharmpy_core.egg-info/SOURCES.txt` & `pharmpy-core-0.98.0/src/pharmpy_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -338,14 +338,15 @@
 src/pharmpy/tools/scm/psn_wrapper.py
 src/pharmpy/tools/scm/results.py
 src/pharmpy/tools/simeval/__init__.py
 src/pharmpy/tools/simeval/results.py
 src/pharmpy/tools/simfit/__init__.py
 src/pharmpy/tools/simfit/results.py
 src/pharmpy/tools/structsearch/__init__.py
+src/pharmpy/tools/structsearch/pkpd.py
 src/pharmpy/tools/structsearch/tmdd.py
 src/pharmpy/tools/structsearch/tool.py
 src/pharmpy/workflows/__init__.py
 src/pharmpy/workflows/args.py
 src/pharmpy/workflows/call.py
 src/pharmpy/workflows/context.py
 src/pharmpy/workflows/execute.py
@@ -389,14 +390,15 @@
 tests/integration/test_evaldesign.py
 tests/integration/test_fit.py
 tests/integration/test_iivsearch.py
 tests/integration/test_iovsearch.py
 tests/integration/test_modelsearch.py
 tests/integration/test_resume.py
 tests/integration/test_ruvsearch.py
+tests/integration/test_structsearch.py
 tests/internals/test_math.py
 tests/internals/test_parse.py
 tests/internals/fs/test_lock.py
 tests/internals/fs/test_tmp.py
 tests/internals/module/test_lazy.py
 tests/model/__init__.py
 tests/model/test_datainfo.py
```

### Comparing `pharmpy-core-0.97.0/tests/cli/test_cli.py` & `pharmpy-core-0.98.0/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/conftest.py` & `pharmpy-core-0.98.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/external/test_nlmixr.py` & `pharmpy-core-0.98.0/tests/external/test_nlmixr.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/external/test_rxode.py` & `pharmpy-core-0.98.0/tests/external/test_rxode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/conftest.py` & `pharmpy-core-0.98.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_allometry.py` & `pharmpy-core-0.98.0/tests/integration/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_amd.py` & `pharmpy-core-0.98.0/tests/integration/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_bootstrap.py` & `pharmpy-core-0.98.0/tests/integration/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_common.py` & `pharmpy-core-0.98.0/tests/integration/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_covsearch.py` & `pharmpy-core-0.98.0/tests/integration/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_estmethod.py` & `pharmpy-core-0.98.0/tests/integration/test_estmethod.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import pytest
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.tools import run_estmethod
 
 
 @pytest.mark.parametrize(
-    'algorithm, methods, solvers, no_of_candidates, advan_ref',
+    'algorithm, methods, covs, no_of_candidates, advan_ref',
     [
         ('exhaustive', ['foce', 'imp'], None, 2, 'ADVAN2'),
         ('exhaustive_only_eval', ['foce', 'imp'], None, 2, 'ADVAN2'),
+        ('exhaustive', ['foce'], ['sandwich', 'cpg'], 2, 'ADVAN2'),
     ],
 )
 def test_estmethod(
     tmp_path,
     start_model,
     model_count,
     testdata,
     algorithm,
     methods,
-    solvers,
+    covs,
     no_of_candidates,
     advan_ref,
 ):
     with chdir(tmp_path):
-        res = run_estmethod(algorithm, methods=methods, solvers=solvers, model=start_model)
+        res = run_estmethod(algorithm, methods=methods, covs=covs, model=start_model)
 
         assert len(res.summary_tool) == no_of_candidates
         assert len(res.models) == no_of_candidates
         assert advan_ref in res.models[-1].model_code
         rundir = tmp_path / 'estmethod_dir1'
         assert rundir.is_dir()
         assert model_count(rundir) == no_of_candidates
```

### Comparing `pharmpy-core-0.97.0/tests/integration/test_evaldesign.py` & `pharmpy-core-0.98.0/tests/integration/test_evaldesign.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_fit.py` & `pharmpy-core-0.98.0/tests/integration/test_fit.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_iivsearch.py` & `pharmpy-core-0.98.0/tests/integration/test_iivsearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import NormalDistribution
 from pharmpy.modeling import set_seq_zo_fo_absorption
 from pharmpy.tools import fit, retrieve_models, run_iivsearch
 
 
+def test_no_of_etas_keep(tmp_path, model_count, start_model):
+    with chdir(tmp_path):
+        res_keep1 = run_iivsearch(
+            'brute_force_no_of_etas',
+            results=start_model.modelfit_results,
+            model=start_model,
+            keep=["CL"],
+        )
+        no_of_models = 8
+        assert len(res_keep1.summary_models) == no_of_models // 2
+        assert res_keep1.summary_individuals.iloc[-1]['description'] == '[CL]'
+
+
 def test_block_structure(tmp_path, model_count, start_model):
     with chdir(tmp_path):
         res = run_iivsearch(
             'brute_force_block_structure', results=start_model.modelfit_results, model=start_model
         )
 
         no_of_candidate_models = 4
```

### Comparing `pharmpy-core-0.97.0/tests/integration/test_iovsearch.py` & `pharmpy-core-0.98.0/tests/integration/test_iovsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_modelsearch.py` & `pharmpy-core-0.98.0/tests/integration/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_resume.py` & `pharmpy-core-0.98.0/tests/integration/test_resume.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/integration/test_ruvsearch.py` & `pharmpy-core-0.98.0/tests/integration/test_ruvsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/internals/fs/test_lock.py` & `pharmpy-core-0.98.0/tests/internals/fs/test_lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/internals/module/test_lazy.py` & `pharmpy-core-0.98.0/tests/internals/module/test_lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/internals/test_math.py` & `pharmpy-core-0.98.0/tests/internals/test_math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/internals/test_parse.py` & `pharmpy-core-0.98.0/tests/internals/test_parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/model/test_datainfo.py` & `pharmpy-core-0.98.0/tests/model/test_datainfo.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/model/test_estimation.py` & `pharmpy-core-0.98.0/tests/model/test_estimation.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,31 @@
     with pytest.raises(ValueError):
         EstimationStep.create('foce', solver='unknownsolverz')
     steps = EstimationSteps.create()
     assert len(steps) == 0
 
 
 def test_estimation_method():
-    a = EstimationStep.create('foce', cov=True)
+    a = EstimationStep.create('foce', cov='sandwich')
     assert a.method == 'FOCE'
-    assert a.cov
+    assert a.cov == 'SANDWICH'
 
     with pytest.raises(ValueError):
         EstimationStep.create('sklarfs')
 
     a = a.replace(method='fo')
     assert a.method == 'FO'
+    assert a.cov == 'SANDWICH'
 
-    assert a == EstimationStep.create('fo', interaction=False, cov=True)
+    assert a == EstimationStep.create('fo', interaction=False, cov='sandwich')
     assert (
-        repr(a) == 'EstimationStep("FO", interaction=False, cov=True, evaluation=False, '
-        'maximum_evaluations=None, laplace=False, isample=None, niter=None, auto=None, '
-        'keep_every_nth_iter=None, solver=None, solver_rtol=None, solver_atol=None, '
-        'tool_options={})'
+        repr(a) == "EstimationStep('FO', interaction=False, cov='SANDWICH', evaluation=False, "
+        "maximum_evaluations=None, laplace=False, isample=None, niter=None, auto=None, "
+        "keep_every_nth_iter=None, solver=None, solver_rtol=None, solver_atol=None, "
+        "tool_options={})"
     )
 
     with pytest.raises(ValueError):
         EstimationStep.create('fo', maximum_evaluations=0)
 
 
 def test_repr():
@@ -102,15 +103,15 @@
 
 def test_dict():
     a = EstimationStep.create('foce')
     d = a.to_dict()
     assert d == {
         'method': 'FOCE',
         'interaction': False,
-        'cov': False,
+        'cov': None,
         'evaluation': False,
         'maximum_evaluations': None,
         'laplace': False,
         'isample': None,
         'niter': None,
         'auto': None,
         'keep_every_nth_iter': None,
@@ -126,15 +127,15 @@
     s1 = EstimationSteps.create([a, b])
     d = s1.to_dict()
     assert d == {
         'steps': (
             {
                 'method': 'FOCE',
                 'interaction': False,
-                'cov': False,
+                'cov': None,
                 'evaluation': False,
                 'maximum_evaluations': None,
                 'laplace': False,
                 'isample': None,
                 'niter': None,
                 'auto': None,
                 'keep_every_nth_iter': None,
@@ -142,15 +143,15 @@
                 'solver_rtol': None,
                 'solver_atol': None,
                 'tool_options': {},
             },
             {
                 'method': 'FO',
                 'interaction': False,
-                'cov': False,
+                'cov': None,
                 'evaluation': False,
                 'maximum_evaluations': None,
                 'laplace': False,
                 'isample': None,
                 'niter': None,
                 'auto': None,
                 'keep_every_nth_iter': None,
```

### Comparing `pharmpy-core-0.97.0/tests/model/test_model.py` & `pharmpy-core-0.98.0/tests/model/test_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/model/test_parameter.py` & `pharmpy-core-0.98.0/tests/model/test_parameter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/model/test_random_variables.py` & `pharmpy-core-0.98.0/tests/model/test_random_variables.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/model/test_statements.py` & `pharmpy-core-0.98.0/tests/model/test_statements.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,29 @@
     Compartment,
     CompartmentalSystem,
     CompartmentalSystemBuilder,
     Infusion,
     Statements,
     output,
 )
+from pharmpy.modeling import add_effect_compartment, set_first_order_absorption
 
 
 def S(x):
     return sympy.Symbol(x)
 
 
+def test_statements_effect_compartment(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'pheno_pd.mod')
+    model = add_effect_compartment(model, "baseline")
+
+    with pytest.warns(UserWarning):
+        print(model.statements)
+
+
 def test_str(load_model_for_test, testdata):
     s1 = Assignment(S('KA'), S('X') + S('Y'))
     assert str(s1) == 'KA = X + Y'
     s2 = Assignment(S('X2'), sympy.exp('X'))
     a = str(s2).split('\n')
     assert a[0].startswith(' ')
     assert len(a) == 2
@@ -280,15 +289,15 @@
     assert comp.name == 'CENTRAL'
     comp = model.statements.ode_system.find_compartment('NOTINMODEL')
     assert comp is None
 
 
 def test_dosing_compartment(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
-    assert model.statements.ode_system.dosing_compartment.name == 'CENTRAL'
+    assert model.statements.ode_system.dosing_compartment[0].name == 'CENTRAL'
 
 
 def test_central_compartment(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'modeling' / 'pheno_advan2.mod')
     assert model.statements.ode_system.central_compartment.name == 'CENTRAL'
     model = load_model_for_test(testdata / 'nonmem' / 'modeling' / 'pheno_advan5_nodepot.mod')
     assert model.statements.ode_system.central_compartment.name == 'CENTRAL'
@@ -456,7 +465,27 @@
     comp = Compartment.create("CENTRAL", lag_time='LT')
     assert repr(comp) == "Compartment(CENTRAL, amount=A_CENTRAL, lag_time=LT)"
 
 
 def test_compartment_names(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
     assert model.statements.ode_system.compartment_names == ['CENTRAL']
+
+
+def test_assignment_create_numeric(load_model_for_test, testdata):
+    with pytest.raises(AttributeError):
+        Assignment('X', 1).free_symbols
+    assert Assignment.create('X', 1).free_symbols
+    with pytest.raises(AttributeError):
+        Assignment('X', 1.0).free_symbols
+    assert Assignment.create('X', 1.0).free_symbols
+
+
+def test_multi_dose_comp_order(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
+    model = set_first_order_absorption(model)
+
+    ode = model.statements.ode_system
+    cb = CompartmentalSystemBuilder(ode)
+    cb.set_dose(cb.find_compartment("CENTRAL"), cb.find_compartment("DEPOT").dose)
+    ode = CompartmentalSystem(cb)
+    assert ode.dosing_compartment[0].name == "DEPOT"
```

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_allometry.py` & `pharmpy-core-0.98.0/tests/modeling/test_allometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from pharmpy.model import Assignment
-from pharmpy.modeling import add_allometry, add_peripheral_compartment
+from pharmpy.modeling import add_allometry, add_peripheral_compartment, set_tmdd
 
 
 def test_allometry(load_model_for_test, testdata):
     ref_model = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
 
     model = add_allometry(
         ref_model,
@@ -115,7 +115,26 @@
         allometric_variable='WGT',
         reference_value=70,
         parameters=['K'],
         initials=[1],
         lower_bounds=[0],
         upper_bounds=[1],
     )
+
+
+def test_add_allometry_tmdd(pheno_path, load_model_for_test):
+    model = load_model_for_test(pheno_path)
+    model = set_tmdd(model, type="full")
+    add_allometry(
+        model,
+        allometric_variable='WGT',
+        reference_value=70,
+    )
+
+    # FIXME: currently adds to CL and LAFREE, is this correct?
+    model = load_model_for_test(pheno_path)
+    model = set_tmdd(model, type="qss")
+    add_allometry(
+        model,
+        allometric_variable='WGT',
+        reference_value=70,
+    )
```

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_blq.py` & `pharmpy-core-0.98.0/tests/modeling/test_blq.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     model_float = transform_blq(model, lloq=0.1)
 
     assert 'DV.GE.LLOQ' in model_float.model_code
 
     df_blq = model.dataset
     df_blq['BLQ'] = np.random.randint(0, 2, df_blq.shape[0])
     di_blq = update_datainfo(model.datainfo, df_blq)
-    blq_col = di_blq['BLQ'].replace(type='blq')
+    blq_col = di_blq['BLQ'].replace(type='blqdv')
     di_blq = di_blq.set_column(blq_col)
     model_blq = model.replace(dataset=df_blq, datainfo=di_blq)
 
     model_blq_col = transform_blq(model_blq)
 
     assert 'BLQ.EQ.0' in model_blq_col.model_code
```

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_common.py` & `pharmpy-core-0.98.0/tests/modeling/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_covariate_effect.py` & `pharmpy-core-0.98.0/tests/modeling/test_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_data_funcs.py` & `pharmpy-core-0.98.0/tests/modeling/test_data_funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_error.py` & `pharmpy-core-0.98.0/tests/modeling/test_error.py`

 * *Files 3% similar despite different names*

```diff
@@ -842,14 +842,72 @@
 $OMEGA 0.031128  ; IVV
 $SIGMA 0.013241
 $ESTIMATION METHOD=1 INTERACTION
 """
     assert model.model_code == correct
 
 
+def test_set_time_varying_error_model_multiple_dvs(testdata, load_model_for_test):
+    code = """$PROBLEM PHENOBARB SIMPLE MODEL
+$DATA pheno.dta IGNORE=@
+$INPUT ID TIME AMT WGT APGR DV
+$SUBROUTINE ADVAN1 TRANS2
+$PK
+CL=THETA(1)*EXP(ETA(1))
+V=THETA(2)*EXP(ETA(2))
+S1=V
+$ERROR
+IF (DVID.EQ.1) THEN
+    Y = F + F*EPS(1)
+ELSE
+    Y = F + F*EPS(1) + EPS(2)
+END IF
+$THETA (0,0.00469307) ; TVCL
+$THETA (0,1.00916) ; TVV
+$OMEGA 0.0309626  ; IVCL
+$OMEGA 0.031128  ; IVV
+$SIGMA 0.013241
+$SIGMA 0.013241
+$ESTIMATION METHOD=1 INTERACTION
+"""
+    model = read_model_from_string(code)
+    model = set_time_varying_error_model(model, cutoff=1.0, dv=1)
+
+    correct = """$PROBLEM PHENOBARB SIMPLE MODEL
+$DATA pheno.dta IGNORE=@
+$INPUT ID TIME AMT WGT APGR DV
+$SUBROUTINE ADVAN1 TRANS2
+$PK
+CL=THETA(1)*EXP(ETA(1))
+V=THETA(2)*EXP(ETA(2))
+S1=V
+$ERROR
+IF (TIME.LT.1.0) THEN
+    Y_1 = F + EPS(1)*F*THETA(3)
+ELSE
+    Y_1 = F + EPS(1)*F
+END IF
+Y_2 = F + EPS(1)*F + EPS(2)
+IF (DVID.EQ.1) THEN
+    Y = Y_1
+ELSE
+    Y = Y_2
+END IF
+$THETA (0,0.00469307) ; TVCL
+$THETA (0,1.00916) ; TVV
+$THETA  0.1 ; time_varying
+$OMEGA 0.0309626  ; IVCL
+$OMEGA 0.031128  ; IVV
+$SIGMA 0.013241
+$SIGMA 0.013241
+$ESTIMATION METHOD=1 INTERACTION
+"""
+    assert model.model_code == correct
+
+
 @pytest.mark.parametrize(
     'epsilons, same_eta, eta_names, err_ref, omega_ref',
     [
         (
             ['EPS_1'],
             False,
             None,
@@ -925,15 +983,15 @@
         'IPRED=F\nIRES=DV-IPRED', 'IPRED=F+EPS(2)\nIRES=DV-IPRED+EPS(3)', model_str
     )
     model_sigma = re.sub(
         r'\$SIGMA 0.013241', '$SIGMA 0.013241\n$SIGMA 0.1\n$SIGMA 0.1', model_more_eps
     )
     model = create_model_for_test(model_sigma)
 
-    model = set_iiv_on_ruv(model, epsilons, same_eta, eta_names)
+    model = set_iiv_on_ruv(model, list_of_eps=epsilons, same_eta=same_eta, eta_names=eta_names)
 
     assert eta_names is None or eta_names[0] in model.random_variables.etas.names
 
     err_rec = model.internals.control_stream.get_records('ERROR')[0]
 
     assert str(err_rec) == f'$ERROR\n' f'W=F\n' f'{err_ref}' f'IWRES=IRES/W\n\n'
 
@@ -943,14 +1001,31 @@
         f'$OMEGA DIAGONAL(2)\n'
         f' 0.0309626  ;       IVCL\n'
         f' 0.031128  ;        IVV\n\n'
         f'{omega_ref}\n'
     )
 
 
+def test_set_iiv_on_ruv_multiple_dvs(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'models' / 'pheno_dvid.mod')
+    model = set_iiv_on_ruv(model, dv=1)
+    rec = model.internals.control_stream.get_records('ERROR')[0]
+    correct = """$ERROR
+Y_1 = F + EPS(1)*F*EXP(ETA_RV1)
+Y_2 = F + EPS(1)*F + EPS(2)
+
+IF (DVID.EQ.1) THEN
+    Y = Y_1
+ELSE
+    Y = Y_2
+END IF
+"""
+    assert str(rec) == correct
+
+
 @pytest.mark.parametrize(
     'epsilons, err_ref, theta_ref',
     [
         (
             ['EPS_1'],
             'IF (F.EQ.0) F = 2.22500000000000E-307\n'
             'Y = F + EPS(1)*F**THETA(4)\n'
```

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_estimation_steps.py` & `pharmpy-core-0.98.0/tests/modeling/test_estimation_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     model = set_estimation_step(model, method, **kwargs)
     assert model.model_code.split('\n')[-2] == code_ref
 
 
 def test_set_estimation_step_est_middle(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
-    model = set_estimation_step(model, 'FOCE', interaction=True, cov=True, idx=0)
+    model = set_estimation_step(model, 'FOCE', interaction=True, cov='SANDWICH', idx=0)
     assert (
         '$ESTIMATION METHOD=COND INTER MAXEVAL=9990 PRINT=2 POSTHOC\n$COVARIANCE'
         in model.model_code
     )
 
 
 def test_add_estimation_step(testdata, load_model_for_test):
@@ -84,22 +84,26 @@
     assert not model.estimation_steps
     assert model.model_code.split('\n')[-2] == '$SIGMA 1'
 
 
 def test_add_covariance_step(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
     assert len(model.estimation_steps) == 1
-    model = add_covariance_step(model)
+    model = add_covariance_step(model, 'SANDWICH')
     assert len(model.estimation_steps) == 1
     assert model.model_code.split('\n')[-2] == '$COVARIANCE'
+    model = remove_covariance_step(model)
+    model = add_covariance_step(model, 'CPG')
+    assert len(model.estimation_steps) == 1
+    assert model.model_code.split('\n')[-2] == '$COVARIANCE MATRIX=S'
 
 
 def test_remove_covariance_step(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
-    model = add_covariance_step(model)
+    model = add_covariance_step(model, 'SANDWICH')
     assert model.model_code.split('\n')[-2] == '$COVARIANCE'
     model = remove_covariance_step(model)
     assert (
         model.model_code.split('\n')[-2]
         == '$ESTIMATION METHOD=COND INTER MAXEVAL=9990 PRINT=2 POSTHOC'
     )
```

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_evaluate.py` & `pharmpy-core-0.98.0/tests/modeling/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_expressions.py` & `pharmpy-core-0.98.0/tests/modeling/test_expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,35 @@
     NormalDistribution,
     Parameter,
     Parameters,
     RandomVariables,
     Statements,
 )
 from pharmpy.modeling import (
+    add_effect_compartment,
     calculate_epsilon_gradient_expression,
     calculate_eta_gradient_expression,
     cleanup_model,
     display_odes,
     get_dv_symbol,
     get_individual_parameters,
     get_individual_prediction_expression,
     get_observation_expression,
+    get_pd_parameters,
     get_pk_parameters,
     get_population_prediction_expression,
     get_rv_parameters,
     greekify_model,
     has_random_effect,
     is_linearized,
     is_real,
     make_declarative,
     mu_reference_model,
     read_model_from_string,
+    set_direct_effect,
     simplify_expression,
     solve_ode_system,
 )
 
 
 def s(x):
     return sympy.Symbol(x)
@@ -331,14 +334,47 @@
         ('nonmem/modeling/transit_indirect_reabsorption.mod', 'elimination', ['CL']),
     ),
     ids=repr,
 )
 def test_get_pk_parameters(load_model_for_test, testdata, model_path, kind, expected):
     model = load_model_for_test(testdata / model_path)
     assert set(get_pk_parameters(model, kind)) == set(expected)
+    assert 'KE0' not in get_pk_parameters(model)
+
+    pkpd_model = load_model_for_test(testdata / "nonmem" / "pheno_real.mod")
+    pkpd_model = add_effect_compartment(pkpd_model, "linear")
+    assert 'KE0' not in get_pk_parameters(pkpd_model)
+
+
+@pytest.mark.parametrize(
+    ('model_path', 'kind', 'expected'),
+    (
+        ('nonmem/pheno.mod', 'baseline', ['E0']),
+        ('nonmem/pheno.mod', 'linear', ['E0', 'S']),
+        ('nonmem/pheno.mod', 'Emax', ['E0', 'E_max', 'EC_50']),
+        ('nonmem/pheno.mod', 'step', ['E0', 'E_max']),
+        ('nonmem/pheno.mod', 'sigmoid', ['EC_50', 'E_max', 'n']),
+        ('nonmem/pheno.mod', 'loglin', ['E0', 'm']),
+    ),
+    ids=repr,
+)
+def test_get_pd_parameters(load_model_for_test, testdata, model_path, kind, expected):
+    model = load_model_for_test(testdata / model_path)
+    assert set(get_pd_parameters(set_direct_effect(model, kind))) == set(expected)
+    assert set(get_pd_parameters(add_effect_compartment(model, kind))) == set(expected + ["KE0"])
+    assert not set(
+        set(get_pd_parameters(set_direct_effect(model, kind))).intersection(
+            get_pk_parameters(set_direct_effect(model, kind))
+        )
+    )
+    assert not set(
+        set(get_pd_parameters(add_effect_compartment(model, kind))).intersection(
+            get_pk_parameters(add_effect_compartment(model, kind))
+        )
+    )
 
 
 @pytest.mark.parametrize(
     ('model_path', 'level', 'expected'),
     (
         ('nonmem/pheno.mod', 'all', ['CL', 'V']),
         ('nonmem/pheno_real.mod', 'all', ['CL', 'V']),
```

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_help_functions.py` & `pharmpy-core-0.98.0/tests/modeling/test_help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_iterators.py` & `pharmpy-core-0.98.0/tests/modeling/test_iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_lrt.py` & `pharmpy-core-0.98.0/tests/modeling/test_lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_metabolite.py` & `pharmpy-core-0.98.0/tests/modeling/test_metabolite.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_odes.py` & `pharmpy-core-0.98.0/tests/modeling/test_odes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import shutil
 from typing import Iterable
 
 import sympy
 
 from pharmpy.model import Assignment
 from pharmpy.modeling import (
+    add_bioavailability,
     add_lag_time,
     add_peripheral_compartment,
     find_clearance_parameters,
     find_volume_parameters,
     get_initial_conditions,
     get_lag_times,
     get_zero_order_inputs,
@@ -17,25 +18,27 @@
     has_linear_odes,
     has_linear_odes_with_real_eigenvalues,
     has_michaelis_menten_elimination,
     has_mixed_mm_fo_elimination,
     has_odes,
     has_zero_order_absorption,
     has_zero_order_elimination,
+    remove_bioavailability,
     remove_lag_time,
     remove_peripheral_compartment,
     set_bolus_absorption,
     set_first_order_absorption,
     set_first_order_elimination,
     set_initial_condition,
     set_michaelis_menten_elimination,
     set_mixed_mm_fo_elimination,
     set_ode_solver,
     set_peripheral_compartments,
     set_seq_zo_fo_absorption,
+    set_tmdd,
     set_transit_compartments,
     set_zero_order_absorption,
     set_zero_order_elimination,
     set_zero_order_input,
 )
 
 
@@ -1667,14 +1670,37 @@
     model = set_transit_compartments(model, 3)
     model = set_mixed_mm_fo_elimination(model)
     assert 'VC1 =' not in model.model_code
     assert 'CLMM = THETA(6)' in model.model_code
     assert 'CL = THETA(1) * EXP(ETA(1))' in model.model_code
 
 
+def test_bioavailability(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'modeling' / 'pheno_advan1.mod')
+    before = model.model_code
+    model = add_bioavailability(model)
+    assert "POP_BIO" in model.parameters
+    assert model.statements.find_assignment("BIO")
+    assert model.statements.find_assignment("F1")
+
+    model = remove_bioavailability(model)
+    assert model.model_code == before
+
+
+def test_move_bioavailability(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'modeling' / 'pheno_advan1.mod')
+    model = add_bioavailability(model)
+    assert model.statements.ode_system.dosing_compartment[0].bioavailability == sympy.Symbol("F1")
+
+    model = set_first_order_absorption(model)
+    assert model.statements.ode_system.dosing_compartment[0].name == "DEPOT"
+    assert model.statements.ode_system.dosing_compartment[0].bioavailability == sympy.Symbol("F1")
+    assert model.statements.ode_system.find_compartment("CENTRAL").dose is None
+
+
 def test_lag_time(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'modeling' / 'pheno_advan1.mod')
     before = model.model_code
     model = add_lag_time(model)
     correct = '''$PROBLEM PHENOBARB SIMPLE MODEL
 $DATA ../pheno.dta IGNORE=@
 $INPUT ID TIME AMT WGT APGR DV FA1 FA2
@@ -2583,7 +2609,19 @@
 
 def test_find_volume_parameters_github_issues_1053_and_1062_bis(load_example_model_for_test):
     model = load_example_model_for_test('pheno')
     model = add_peripheral_compartment(model)
     model = add_peripheral_compartment(model)
     model = set_michaelis_menten_elimination(model)
     assert find_volume_parameters(model) == _symbols(['V1', 'VP1', 'VP2'])
+
+
+def test_find_clearance_and_volume_parameters_tmdd(load_example_model_for_test):
+    model = load_example_model_for_test('pheno')
+    model = set_tmdd(model, 'full')
+    assert find_clearance_parameters(model) == _symbols(['CL'])
+    assert find_volume_parameters(model) == _symbols(['V'])
+
+    model = load_example_model_for_test('pheno')
+    model = set_tmdd(model, 'qss')
+    assert find_clearance_parameters(model) == _symbols(['CL', 'LAFREE'])
+    assert find_volume_parameters(model) == _symbols(['V'])
```

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_parameter_sampling.py` & `pharmpy-core-0.98.0/tests/modeling/test_parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_parameter_variability.py` & `pharmpy-core-0.98.0/tests/modeling/test_parameter_variability.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_parameters.py` & `pharmpy-core-0.98.0/tests/modeling/test_parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_pd.py` & `pharmpy-core-0.98.0/tests/modeling/test_pd.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         )
         assert model.statements.after_odes[-1] == Assignment(S("Y_2"), e + e * S("epsilon_p"))
         assert model.parameters["POP_n"].init == 1
     elif expr == "step":
         assert model.statements[1] == Assignment(e0, S("POP_E0"))
         assert model.statements[0] == Assignment(emax, S("POP_E_max"))
         assert model.statements.after_odes[-2] == Assignment(
-            e, sympy.Piecewise((0, conc < 0), (emax, True))
+            e, sympy.Piecewise((e0, conc < 0), (e0 + emax, True))
         )
         assert model.statements.after_odes[-1] == Assignment(S("Y_2"), e + e * S("epsilon_p"))
     elif expr == "loglin":
         assert model.statements[1] == Assignment(e0, S("POP_E0"))
         assert model.statements[0] == Assignment(S("m"), S("POP_m"))
         assert model.statements.after_odes[-2] == Assignment(
             e, S("m") * sympy.log(conc + sympy.exp(e0 / S("m")))
```

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_plots.py` & `pharmpy-core-0.98.0/tests/modeling/test_plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_results.py` & `pharmpy-core-0.98.0/tests/modeling/test_results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/modeling/test_tmdd.py` & `pharmpy-core-0.98.0/tests/modeling/test_tmdd.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
         'A_CENTRAL(t)*(-A_TARGET(t)*KON - CL/V) + A_COMPLEX(t)*KOFF'
     )
 
 
 def test_qss(pheno_path, load_model_for_test):
     model = load_model_for_test(pheno_path)
     model = set_tmdd(model, type="qss")
+    assert model.statements.ode_system.eqs[0].rhs == sympy.sympify(
+        '-A_CENTRAL(t)*CL*LAFREE/V - A_TARGET(t)*KINT*LAFREE/(KD + LAFREE) - CL*LAFREE/V'
+    )
 
 
 def test_cr(pheno_path, load_model_for_test):
     model = load_model_for_test(pheno_path)
     model = set_tmdd(model, type="cr")
     assert model.statements.ode_system.eqs[1].rhs == sympy.sympify(
         '(-KINT - KOFF)*A_COMPLEX(t) + (KON*R_0 - KON*A_COMPLEX(t)/V)*A_CENTRAL(t)'
```

### Comparing `pharmpy-core-0.97.0/tests/nonmem/output/test_nonmem_results_file.py` & `pharmpy-core-0.98.0/tests/nonmem/output/test_nonmem_results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_abbreviated.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_abbreviated.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_code.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_code.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_data.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_estimation_record.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_estimation_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_factory.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_model_record.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_omega.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_omega.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_option_record.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_option_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_problem.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_problem.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_sizes.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_sizes.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/records/test_theta.py` & `pharmpy-core-0.98.0/tests/nonmem/records/test_theta.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/test_advan.py` & `pharmpy-core-0.98.0/tests/nonmem/test_advan.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/test_des.py` & `pharmpy-core-0.98.0/tests/nonmem/test_des.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/test_input.py` & `pharmpy-core-0.98.0/tests/nonmem/test_input.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/test_modelfit_results.py` & `pharmpy-core-0.98.0/tests/nonmem/test_modelfit_results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/test_nonmem_model.py` & `pharmpy-core-0.98.0/tests/nonmem/test_nonmem_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import shutil
 
 import pytest
 import sympy
 from sympy import Symbol as symbol
 
+from pharmpy.deps import pandas as pd
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import (
     Assignment,
     EstimationStep,
     EstimationSteps,
     Model,
     ModelSyntaxError,
@@ -24,14 +25,15 @@
     add_iiv,
     add_population_parameter,
     create_joint_distribution,
     remove_iiv,
     set_estimation_step,
     set_initial_condition,
     set_initial_estimates,
+    set_transit_compartments,
     set_zero_order_absorption,
     set_zero_order_elimination,
     set_zero_order_input,
 )
 from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.amd.funcs import create_start_model
 
@@ -564,36 +566,49 @@
     model_ref = transformation(model_ref)
 
     model_des = Model.parse_model_from_string(model_ref.model_code)
 
     assert model_ref.statements.ode_system == model_des.statements.ode_system
 
 
-def test_cmt_warning(load_model_for_test, testdata):
-    model_original = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox1.mod')
+def test_cmt_update(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox1.mod')
+    old_cmt = model.dataset["CMT"]
+    old_cmt = pd.to_numeric(old_cmt)
 
-    model_str = model_original.model_code.replace('CMT=DROP', 'CMT')
-    model = Model.parse_model_from_string(model_str)
-    model = model.replace(datainfo=model.datainfo.replace(path=model_original.datainfo.path))
+    model = set_transit_compartments(model, 2)
+    updated_cmt = model.dataset["CMT"]
 
-    with pytest.raises(UserWarning, match='Compartment structure has been updated'):
-        set_zero_order_absorption(model)
+    assert old_cmt[0] == 1 and updated_cmt[0] == 1
+    assert old_cmt[1] == 2 and updated_cmt[1] == 4
+
+
+def test_zero_order_cmt(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox1.mod')
+    old_cmt = model.dataset["CMT"]
+    old_cmt = pd.to_numeric(old_cmt)
+
+    model = set_zero_order_absorption(model)
+    updated_cmt = model.dataset["CMT"]
+
+    assert old_cmt[0] == 1 and updated_cmt[0] == 1
+    assert old_cmt[1] == 2 and updated_cmt[1] == 1
 
 
 @pytest.mark.parametrize(
     'estcode,est_steps',
     [
         ('$ESTIMATION METH=COND INTERACTION', [EstimationStep.create('foce', interaction=True)]),
         ('$ESTIMATION INTER METH=COND', [EstimationStep.create('foce', interaction=True)]),
         ('$ESTM METH=1 INTERACTION', [EstimationStep.create('foce', interaction=True)]),
         ('$ESTIM METH=1', [EstimationStep.create('foce')]),
         ('$ESTIMA METH=0', [EstimationStep.create('fo')]),
         ('$ESTIMA METH=ZERO', [EstimationStep.create('fo')]),
         ('$ESTIMA INTER', [EstimationStep.create('fo', interaction=True)]),
-        ('$ESTIMA INTER\n$COV', [EstimationStep.create('fo', interaction=True, cov=True)]),
+        ('$ESTIMA INTER\n$COV', [EstimationStep.create('fo', interaction=True, cov='sandwich')]),
         (
             '$ESTIMA METH=COND INTER\n$EST METH=COND',
             [
                 EstimationStep.create('foce', interaction=True),
                 EstimationStep.create('foce', interaction=False),
             ],
         ),
@@ -650,15 +665,17 @@
 
 
 @pytest.mark.parametrize(
     'estcode,kwargs,rec_ref',
     [
         ('$EST METH=COND INTER', {'method': 'fo'}, '$ESTIMATION METHOD=ZERO INTER'),
         ('$EST METH=COND INTER', {'interaction': False}, '$ESTIMATION METHOD=COND'),
-        ('$EST METH=COND INTER', {'cov': True}, '$COVARIANCE'),
+        ('$EST METH=COND INTER', {'cov': 'sandwich'}, '$COVARIANCE'),
+        ('$EST METH=COND INTER', {'cov': 'cpg'}, '$COVARIANCE MATRIX=S'),
+        ('$EST METH=COND INTER', {'cov': 'ofim'}, '$COVARIANCE MATRIX=R'),
         (
             '$EST METH=COND INTER MAXEVAL=99999',
             {'method': 'fo'},
             '$ESTIMATION METHOD=ZERO INTER MAXEVAL=99999',
         ),
         (
             '$EST METH=COND INTER POSTHOC',
```

### Comparing `pharmpy-core-0.97.0/tests/nonmem/test_nonmem_table.py` & `pharmpy-core-0.98.0/tests/nonmem/test_nonmem_table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/test_parser.py` & `pharmpy-core-0.98.0/tests/nonmem/test_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/nonmem/test_read.py` & `pharmpy-core-0.98.0/tests/nonmem/test_read.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/frem/results.json` & `pharmpy-core-0.98.0/tests/testdata/frem/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/DDMODEL00000130` & `pharmpy-core-0.98.0/tests/testdata/nonmem/DDMODEL00000130`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv` & `pharmpy-core-0.98.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml` & `pharmpy-core-0.98.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/errors/control_stream_error.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/errors/control_stream_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/errors/est_step_warning.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/errors/est_step_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/errors/failed_run.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/errors/failed_run.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/errors/no_header_error.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/errors/no_header_error.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/errors/no_header_error.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/errors/no_header_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/errors/rounding_error.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/errors/rounding_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/errors/run_interrupted.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/errors/run_interrupted.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/errors/zero_gradient_error.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/errors/zero_gradient_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/fcon/FCON` & `pharmpy-core-0.98.0/tests/testdata/nonmem/fcon/FCON`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/fcon/FDATA` & `pharmpy-core-0.98.0/tests/testdata/nonmem/fcon/FDATA`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_1transit.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_1transit.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_2transits.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_2transits.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan1.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan11.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan11.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan12.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan12.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan2.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan3.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan4.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/fviii6.datainfo` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/fviii6.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/fviii6.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/fviii6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox1.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox2.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox2.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox2.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox2.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_2comp.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_2comp.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_simulated_log.csv` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_simulated_log.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_simulated_normal.csv` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_simulated_normal.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/mytab_mox2` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pef.csv` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pef.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_des_assignments.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_des_assignments.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_dvid.csv` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_dvid.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_dvid.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_dvid.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.coi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.cor` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_noifs.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_noifs.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_trans1.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_trans1.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/models/pheno_trans1.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/models/pheno_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.datainfo` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_block.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_block.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_etas.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_etas.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_pd.csv` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_pd.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_rate.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_rate.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.coi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.cor` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.tab` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real.xml` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real.xml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/pheno_real_linbase.tab` & `pharmpy-core-0.98.0/tests/testdata/nonmem/pheno_real_linbase.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/add_etas_linbase.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/add_etas_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/add_etas_linbase.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/add_etas_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/add_etas_linbase.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/add_etas_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/add_etas_linbase.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/add_etas_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/boxcox.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/boxcox.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/boxcox.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/boxcox.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/boxcox.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/boxcox.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/boxcox.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/boxcox.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/cdd_results.json` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/fullblock.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/fullblock.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/fullblock.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/fullblock.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/fullblock.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/fullblock.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/fullblock.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/fullblock.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/iov.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/iov.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/iov.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/iov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/iov.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/iov.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/iov.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/iov.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/pheno_linbase.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/resmod_results.json` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/resmod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/scm_results.json` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/scm_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/simeval_results.json` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/simeval_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/tdist.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/tdist.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/tdist.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/tdist.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/tdist.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/tdist.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/qa/tdist.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/qa/tdist.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mox3.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mox3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mox3.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mox3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mox3.mod` & `pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mox3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mox3.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mox3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv` & `pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/ruvsearch/mytab` & `pharmpy-core-0.98.0/tests/testdata/nonmem/ruvsearch/mytab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/localmin.logf` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/localmin.logf`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/meta.yaml` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt` & `pharmpy-core-0.98.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/sdtab1` & `pharmpy-core-0.98.0/tests/testdata/nonmem/sdtab1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.dta` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/pheno.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run1.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run1.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run1.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run1.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run2.cov` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run2.ext` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run2.lst` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/nonmem/secondary_parameters/run2.phi` & `pharmpy-core-0.98.0/tests/testdata/nonmem/secondary_parameters/run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/pheno_data.csv` & `pharmpy-core-0.98.0/tests/testdata/pheno_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/est_data0.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/est_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/est_data1.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/est_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/est_data2.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/est_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/est_data3.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/est_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/meta.yaml` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/pred_data0.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/pred_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/pred_data1.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/pred_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/pred_data2.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/pred_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/pred_data3.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/pred_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt` & `pharmpy-core-0.98.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/frem_dataset.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/frem_results.csv` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/frem_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1.cov` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.cor` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.cov` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.mod` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3.mod` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/meta.yaml` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/proposal_density.cov` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/proposal_density.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt` & `pharmpy-core-0.98.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/results.json` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/qa_dir1/results_summary.yaml` & `pharmpy-core-0.98.0/tests/testdata/psn/qa_dir1/results_summary.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/resmod_dir1/resmod_results.csv` & `pharmpy-core-0.98.0/tests/testdata/psn/resmod_dir1/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/resmod_dir2/resmod_results.csv` & `pharmpy-core-0.98.0/tests/testdata/psn/resmod_dir2/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.cor` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.cov` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.mod` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv` & `pharmpy-core-0.98.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/allometry_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/allometry_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/amd_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/amd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/bootstrap_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/bootstrap_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/cdd_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/covsearch_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/covsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/estmethod_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/estmethod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/iivsearch_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/iivsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/iovsearch_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/iovsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/linearize_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/linearize_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/metadata.json` & `pharmpy-core-0.98.0/tests/testdata/results/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/modelsearch_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/modelsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/qa_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/qa_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/ruvsearch_results.json` & `pharmpy-core-0.98.0/tests/testdata/results/ruvsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/metadata.json` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/results.csv` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/testdata/results/tool_databases/modelsearch/results.json` & `pharmpy-core-0.98.0/tests/testdata/results/tool_databases/modelsearch/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_allometry.py` & `pharmpy-core-0.98.0/tests/tools/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_amd.py` & `pharmpy-core-0.98.0/tests/tools/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_bootstrap.py` & `pharmpy-core-0.98.0/tests/tools/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_cdd.py` & `pharmpy-core-0.98.0/tests/tools/test_cdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_covsearch.py` & `pharmpy-core-0.98.0/tests/tools/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_estmethod.py` & `pharmpy-core-0.98.0/tests/tools/test_estmethod.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import pytest
 
 from pharmpy.tools.estmethod.algorithms import _create_candidate_model
 from pharmpy.tools.estmethod.tool import SOLVERS, create_workflow, validate_input
 
 
 @pytest.mark.parametrize(
-    'algorithm, methods, solvers, no_of_models',
+    'algorithm, methods, solvers, covs, no_of_models',
     [
-        ('exhaustive', ['foce'], None, 1),
-        ('exhaustive', ['foce', 'laplace'], None, 2),
-        ('exhaustive', ['foce', 'imp'], ['lsoda'], 2),
-        ('exhaustive', ['foce'], 'all', len(SOLVERS)),
-        ('exhaustive_with_update', ['foce'], None, 2),
-        ('exhaustive_with_update', ['foce', 'laplace'], None, 4),
-        ('exhaustive_with_update', ['laplace'], None, 3),
-        ('exhaustive_with_update', ['foce'], ['lsoda'], 3),
-        ('exhaustive_with_update', ['foce'], 'all', len(SOLVERS) * 2 + 1),
+        ('exhaustive', ['foce'], None, None, 1),
+        ('exhaustive', ['foce', 'laplace'], None, None, 2),
+        ('exhaustive', ['foce', 'imp'], ['lsoda'], None, 2),
+        ('exhaustive', ['foce'], 'all', None, len(SOLVERS)),
+        ('exhaustive_with_update', ['foce'], None, None, 2),
+        ('exhaustive_with_update', ['foce', 'laplace'], None, None, 4),
+        ('exhaustive_with_update', ['laplace'], None, None, 3),
+        ('exhaustive_with_update', ['foce'], ['lsoda'], None, 3),
+        ('exhaustive_with_update', ['foce'], 'all', None, len(SOLVERS) * 2 + 1),
+        ('exhaustive', ['foce'], None, ['sandwich', 'cpg'], 2),
+        ('exhaustive', ['foce', 'imp'], None, ['sandwich', 'cpg'], 4),
     ],
 )
-def test_algorithm(algorithm, methods, solvers, no_of_models):
-    wf = create_workflow(algorithm, methods=methods, solvers=solvers)
+def test_algorithm(algorithm, methods, solvers, covs, no_of_models):
+    wf = create_workflow(algorithm, methods=methods, solvers=solvers, covs=covs)
     fit_tasks = [task.name for task in wf.tasks if task.name.startswith('run')]
 
     assert len(fit_tasks) == no_of_models
 
 
 @pytest.mark.parametrize(
     'method, est_rec, eval_rec',
@@ -41,15 +43,15 @@
         ),
     ],
 )
 def test_create_est_model(load_model_for_test, pheno_path, method, est_rec, eval_rec):
     model = load_model_for_test(pheno_path)
     assert len(model.estimation_steps) == 1
     est_model = _create_candidate_model(
-        method, None, model=model, update=False, is_eval_candidate=False
+        method, None, None, model=model, update=False, is_eval_candidate=False
     )
     assert len(est_model.estimation_steps) == 2
     assert est_model.model_code.split('\n')[-5] == est_rec
     assert est_model.model_code.split('\n')[-4] == eval_rec
 
 
 @pytest.mark.parametrize(
```

### Comparing `pharmpy-core-0.97.0/tests/tools/test_exports.py` & `pharmpy-core-0.98.0/tests/tools/test_exports.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_frem.py` & `pharmpy-core-0.98.0/tests/tools/test_frem.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_iivsearch.py` & `pharmpy-core-0.98.0/tests/tools/test_iivsearch.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,27 @@
     create_eta_blocks,
 )
 from pharmpy.tools.iivsearch.tool import create_workflow, validate_input
 from pharmpy.workflows import Workflow
 
 
 @pytest.mark.parametrize(
+    'list_of_parameters, expected_values',
+    [([], 3), (['CL'], 1), (["CL", "V"], 0)],
+)
+def test_brute_force_no_of_etas_keep(
+    load_model_for_test, testdata, list_of_parameters, expected_values
+):
+    model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
+    wf = brute_force_no_of_etas(model, keep=list_of_parameters)
+    fit_tasks = [task.name for task in wf.tasks if task.name.startswith('run')]
+    assert len(fit_tasks) == expected_values
+
+
+@pytest.mark.parametrize(
     'list_of_parameters, no_of_models',
     [([], 7), (['QP1'], 15)],
 )
 def test_brute_force_no_of_etas(load_model_for_test, testdata, list_of_parameters, no_of_models):
     model = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox2.mod')
     model = add_peripheral_compartment(model)
     model = add_iiv(model, list_of_parameters, 'add')
```

### Comparing `pharmpy-core-0.97.0/tests/tools/test_iovsearch.py` & `pharmpy-core-0.98.0/tests/tools/test_iovsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_linearize.py` & `pharmpy-core-0.98.0/tests/tools/test_linearize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_mfl.py` & `pharmpy-core-0.98.0/tests/tools/test_mfl.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_ml.py` & `pharmpy-core-0.98.0/tests/tools/test_ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_modelsearch.py` & `pharmpy-core-0.98.0/tests/tools/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_qa.py` & `pharmpy-core-0.98.0/tests/tools/test_qa.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_rankfuncs.py` & `pharmpy-core-0.98.0/tests/tools/test_rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_run.py` & `pharmpy-core-0.98.0/tests/tools/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,14 +384,20 @@
     summary_multest_full_no_res = summarize_modelfit_results(
         [None, mox],
         include_all_estimation_steps=True,
     )
 
     assert summary_multest_full_no_res.loc['mox1', 1]['ofv'] == -624.5229577248352
 
+    with pytest.raises(ValueError, match='Option `results` is None'):
+        summarize_modelfit_results(None)
+
+    with pytest.raises(ValueError, match='All input results are empty'):
+        summarize_modelfit_results([None, None])
+
 
 def test_summarize_modelfit_results_errors(load_model_for_test, testdata, tmp_path, pheno_path):
     with chdir(tmp_path):
         model = read_modelfit_results(pheno_path)
         shutil.copy2(testdata / 'pheno_data.csv', tmp_path)
 
         error_path = testdata / 'nonmem' / 'errors'
```

### Comparing `pharmpy-core-0.97.0/tests/tools/test_runtool.py` & `pharmpy-core-0.98.0/tests/tools/test_runtool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_ruvsearch.py` & `pharmpy-core-0.98.0/tests/tools/test_ruvsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_scm.py` & `pharmpy-core-0.98.0/tests/tools/test_scm.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_start_model.py` & `pharmpy-core-0.98.0/tests/tools/test_start_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     model = create_start_model(path, modeltype='pk_iv')
     sep = model.datainfo.separator
     assert sep == "\\s+"
     assert len(model.dataset.columns) == 8
     assert len(model.parameters) == 6
     assert 'POP_CL' in model.parameters
     assert 'POP_MAT' not in model.parameters
-    assert model.statements.ode_system.dosing_compartment.dose == Bolus.create("AMT")
+    assert model.statements.ode_system.dosing_compartment[0].dose == Bolus.create("AMT")
     model = create_start_model(path, modeltype='pk_oral')
     assert 'IIV_MAT' in model.parameters
     assert 'POP_CL' in model.parameters
     assert 'POP_MAT' in model.parameters
 
     path_2 = testdata / 'nonmem' / 'modeling' / 'pheno_zero_order.csv'
     model = create_start_model(path_2, modeltype='pk_iv')
-    assert model.statements.ode_system.dosing_compartment.dose == Infusion.create(
+    assert model.statements.ode_system.dosing_compartment[0].dose == Infusion.create(
         "AMT", duration="D1"
     )
```

### Comparing `pharmpy-core-0.97.0/tests/tools/test_summarize_individuals.py` & `pharmpy-core-0.98.0/tests/tools/test_summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/tools/test_wrap.py` & `pharmpy-core-0.98.0/tests/tools/test_wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/workflows/test_call.py` & `pharmpy-core-0.98.0/tests/workflows/test_call.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/workflows/test_execute.py` & `pharmpy-core-0.98.0/tests/workflows/test_execute.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/workflows/test_model_database.py` & `pharmpy-core-0.98.0/tests/workflows/test_model_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tests/workflows/test_workflow.py` & `pharmpy-core-0.98.0/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.97.0/tox.ini` & `pharmpy-core-0.98.0/tox.ini`

 * *Files identical despite different names*

