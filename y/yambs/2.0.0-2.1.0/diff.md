# Comparing `tmp/yambs-2.0.0.tar.gz` & `tmp/yambs-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-2.0.0.tar", last modified: Mon Jul 17 06:21:32 2023, max compression
+gzip compressed data, was "yambs-2.1.0.tar", last modified: Sat Jul 22 21:05:46 2023, max compression
```

## Comparing `yambs-2.0.0.tar` & `yambs-2.1.0.tar`

### file list

```diff
@@ -1,97 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 06:20:21.000000 yambs-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-17 06:21:32.823221 yambs-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-17 06:20:21.000000 yambs-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-17 06:20:21.000000 yambs-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:21:32.823221 yambs-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-17 06:20:21.000000 yambs-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.815221 yambs-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-17 06:20:21.000000 yambs-2.0.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 06:20:21.000000 yambs-2.0.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.815221 yambs-2.0.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/includes/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/CommonConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/targets_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/variants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.691005 yambs-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-22 21:04:27.000000 yambs-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-22 21:05:46.691005 yambs-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-22 21:04:27.000000 yambs-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-22 21:04:27.000000 yambs-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 21:05:46.691005 yambs-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-22 21:04:27.000000 yambs-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.679005 yambs-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-22 21:04:27.000000 yambs-2.1.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-22 21:04:27.000000 yambs-2.1.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.683005 yambs-2.1.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.683005 yambs-2.1.0/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.683005 yambs-2.1.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/commands/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.683005 yambs-2.1.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.683005 yambs-2.1.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.683005 yambs-2.1.0/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/includes/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.687005 yambs-2.1.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/CommonConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.687005 yambs-2.1.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.687005 yambs-2.1.0/yambs/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.687005 yambs-2.1.0/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.687005 yambs-2.1.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.687005 yambs-2.1.0/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/generate/variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.687005 yambs-2.1.0/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.687005 yambs-2.1.0/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-22 21:04:27.000000 yambs-2.1.0/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:05:46.683005 yambs-2.1.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-22 21:05:46.000000 yambs-2.1.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-22 21:05:46.000000 yambs-2.1.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 21:05:46.000000 yambs-2.1.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-22 21:05:46.000000 yambs-2.1.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-22 21:05:46.000000 yambs-2.1.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 21:05:46.000000 yambs-2.1.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-2.0.0/LICENSE` & `yambs-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/PKG-INFO` & `yambs-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.0.0
+Version: 2.1.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=002bf1ec758c597d37da825e56ca08c0
+    hash=0f4386a6affa598c310b2ec58d5f608f
     =====================================
 -->
 
-# yambs ([2.0.0](https://pypi.org/project/yambs/))
+# yambs ([2.1.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.0.0/README.md` & `yambs-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=002bf1ec758c597d37da825e56ca08c0
+    hash=0f4386a6affa598c310b2ec58d5f608f
     =====================================
 -->
 
-# yambs ([2.0.0](https://pypi.org/project/yambs/))
+# yambs ([2.1.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.0.0/pyproject.toml` & `yambs-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "2.0.0"
+version = "2.1.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-2.0.0/setup.py` & `yambs-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/tests/test_entry.py` & `yambs-2.1.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/aggregation/__init__.py` & `yambs-2.1.0/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/app.py` & `yambs-2.1.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/commands/all.py` & `yambs-2.1.0/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/commands/common.py` & `yambs-2.1.0/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/commands/dist.py` & `yambs-2.1.0/yambs/commands/dist.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from argparse import Namespace as _Namespace
 from pathlib import Path
 from shutil import copytree, rmtree
 from tempfile import TemporaryDirectory
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
+from vcorelib.io import ARBITER
 from vcorelib.paths import create_hex_digest
 
 # internal
 from yambs.commands.common import add_config_arg
 from yambs.config.common import CommonConfig
-from yambs.dist import copy_source_tree, make_archives
+from yambs.dist import copy_source_tree, dist_metadata, make_archives
 
 
 def dist_cmd(args: _Namespace) -> int:
     """Execute the dist command."""
 
     config = CommonConfig.load(path=args.config, root=args.dir)
 
@@ -33,14 +34,17 @@
 
         if args.sources:
             copytree(config.src_root, base)
         else:
             base.mkdir()
             copy_source_tree(config, base)
 
+        # Add JSON metadata.
+        ARBITER.encode(base.joinpath("dist.json"), dist_metadata())
+
         # Remove and re-create the dist directory.
         dist = config.dist_root
         rmtree(dist, ignore_errors=True)
         dist.mkdir()
 
         make_archives(path, config)
```

### Comparing `yambs-2.0.0/yambs/commands/gen.py` & `yambs-2.1.0/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/commands/native.py` & `yambs-2.1.0/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/commands/uf2conv.py` & `yambs-2.1.0/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/config/__init__.py` & `yambs-2.1.0/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/config/board.py` & `yambs-2.1.0/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/config/common.py` & `yambs-2.1.0/yambs/config/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/includes/chips.yaml` & `yambs-2.1.0/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/includes/infineon.yaml` & `yambs-2.1.0/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/includes/microchip.yaml` & `yambs-2.1.0/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/native.yaml` & `yambs-2.1.0/yambs/data/native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/schemas/Chip.yaml` & `yambs-2.1.0/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/schemas/Config.yaml` & `yambs-2.1.0/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/schemas/Native.yaml` & `yambs-2.1.0/yambs/data/schemas/Native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/schemas/config_common.yaml` & `yambs-2.1.0/yambs/data/schemas/config_common.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/templates/native_rules.ninja.j2` & `yambs-2.1.0/yambs/data/templates/native_rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/templates/rules.ninja.j2` & `yambs-2.1.0/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/data/uf2families.json` & `yambs-2.1.0/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/dist/__init__.py` & `yambs-2.1.0/yambs/dist/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 A module implementing interfaces for facilitating project distribution.
 """
 
 # built-in
 from pathlib import Path
 from shutil import copy2, copytree, make_archive
+from typing import Any, Dict
 
 # third-party
 from vcorelib.paths.context import in_dir
 
 # internal
+from yambs import VERSION
 from yambs.config.common import CommonConfig
 
 ARCHIVES = [
     ("tar.gz", "gztar"),
     ("tar.xz", "xztar"),
     ("zip", "zip"),
 ]
@@ -59,7 +61,12 @@
         + [root.joinpath(x) for x in config.data.get("extra_dist", [])]
         if x and x.exists()
     ]:
         if item.is_dir():
             copytree(item, dest.joinpath(item.name))
         else:
             copy2(item, dest.joinpath(item.name))
+
+
+def dist_metadata() -> Dict[str, Any]:
+    """Get metadata for packaged distributions."""
+    return {"yambs_version": VERSION}
```

### Comparing `yambs-2.0.0/yambs/entry.py` & `yambs-2.1.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/environment/__init__.py` & `yambs-2.1.0/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/environment/native.py` & `yambs-2.1.0/yambs/environment/native.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,18 +116,22 @@
             stream.write(linesep + linesep)
 
         line = "build ${variant}_apps: phony "
         offset = " " * len(line)
 
         elfs_list = list(elfs.values())
 
-        # Also update the static library (if necessary) when linking
-        # applications.
+        # Add a phony target for creating a static library.
         if outputs:
-            elfs_list.append(self.write_static_library_rule(stream, outputs))
+            stream.write(
+                "build ${variant}_lib: phony "
+                + str(self.write_static_library_rule(stream, outputs))
+                + linesep
+                + linesep
+            )
 
         stream.write(line + str(elfs_list[0]))
         for elf in elfs_list[1:]:
             write_continuation(stream, offset)
             stream.write(str(elf))
         stream.write(linesep)
```

### Comparing `yambs-2.0.0/yambs/generate/__init__.py` & `yambs-2.1.0/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/generate/architectures.py` & `yambs-2.1.0/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/generate/boards.py` & `yambs-2.1.0/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/generate/chips.py` & `yambs-2.1.0/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/generate/common.py` & `yambs-2.1.0/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/generate/ninja/__init__.py` & `yambs-2.1.0/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/generate/ninja/format.py` & `yambs-2.1.0/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/generate/toolchains.py` & `yambs-2.1.0/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/generate/variants.py` & `yambs-2.1.0/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/schemas.py` & `yambs-2.1.0/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/translation/__init__.py` & `yambs-2.1.0/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs/uf2/__init__.py` & `yambs-2.1.0/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.0.0/yambs.egg-info/PKG-INFO` & `yambs-2.1.0/yambs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.0.0
+Version: 2.1.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=002bf1ec758c597d37da825e56ca08c0
+    hash=0f4386a6affa598c310b2ec58d5f608f
     =====================================
 -->
 
-# yambs ([2.0.0](https://pypi.org/project/yambs/))
+# yambs ([2.1.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.0.0/yambs.egg-info/SOURCES.txt` & `yambs-2.1.0/yambs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 yambs/data/schemas/CommonConfig.yaml
 yambs/data/schemas/Config.yaml
 yambs/data/schemas/Native.yaml
 yambs/data/schemas/Toolchain.yaml
 yambs/data/schemas/Variant.yaml
 yambs/data/schemas/config_common.yaml
 yambs/data/schemas/entry_common.yaml
-yambs/data/schemas/targets_common.yaml
 yambs/data/schemas/toolchain_common.yaml
 yambs/data/templates/all.ninja.j2
 yambs/data/templates/architecture.ninja.j2
 yambs/data/templates/board.ninja.j2
 yambs/data/templates/build.ninja.j2
 yambs/data/templates/chip.ld.j2
 yambs/data/templates/chip.ninja.j2
```

