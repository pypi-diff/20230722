# Comparing `tmp/manticore-0.3.8.dev230721.tar.gz` & `tmp/manticore-0.3.8.dev230722.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manticore-0.3.8.dev230721.tar", last modified: Fri Jul 21 12:53:59 2023, max compression
+gzip compressed data, was "dist/manticore-0.3.8.dev230722.tar", last modified: Sat Jul 22 12:43:52 2023, max compression
```

## Comparing `manticore-0.3.8.dev230721.tar` & `manticore-0.3.8.dev230722.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/
--rw-r--r--   0 runner    (1001) docker     (122)    15363 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12497 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8393 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/binary/
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/binary/binary.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    49622 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/manticore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/core/parser/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)    28116 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/core/smtlib/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/smtlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17980 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/smtlib/constraints.py
--rw-r--r--   0 runner    (1001) docker     (122)    44912 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/smtlib/expression.py
--rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/smtlib/operators.py
--rw-r--r--   0 runner    (1001) docker     (122)    39663 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/smtlib/solver.py
--rw-r--r--   0 runner    (1001) docker     (122)    38537 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/smtlib/visitors.py
--rw-r--r--   0 runner    (1001) docker     (122)    23618 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/state.py
--rw-r--r--   0 runner    (1001) docker     (122)    10874 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/state_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    16180 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)    20267 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/core/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/ethereum/
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14383 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/abi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5031 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/abitypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5299 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     4572 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    39008 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/detectors.py
--rw-r--r--   0 runner    (1001) docker     (122)    81041 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/manticore.py
--rw-r--r--   0 runner    (1001) docker     (122)     8264 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/parsetab.py
--rw-r--r--   0 runner    (1001) docker     (122)    11447 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/plugins.py
--rw-r--r--   0 runner    (1001) docker     (122)    14652 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/solidity.py
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/state.py
--rw-r--r--   0 runner    (1001) docker     (122)    19857 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/ethereum/verifier.py
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/native/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/native/cpu/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   163406 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cpu/aarch64.py
--rw-r--r--   0 runner    (1001) docker     (122)    41088 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cpu/abstractcpu.py
--rw-r--r--   0 runner    (1001) docker     (122)    62492 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cpu/arm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7715 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cpu/bitwise.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cpu/cpufactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cpu/disasm.py
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cpu/register.py
--rw-r--r--   0 runner    (1001) docker     (122)   255150 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/cpu/x86.py
--rw-r--r--   0 runner    (1001) docker     (122)    18111 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/manticore.py
--rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/mappings.py
--rw-r--r--   0 runner    (1001) docker     (122)    56205 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     9960 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     6100 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/plugins.py
--rw-r--r--   0 runner    (1001) docker     (122)    13875 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/state.py
--rw-r--r--   0 runner    (1001) docker     (122)    10474 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/native/state_merging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/platforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18558 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/platforms/cgcrandom.py
--rw-r--r--   0 runner    (1001) docker     (122)    40996 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/platforms/decree.py
--rw-r--r--   0 runner    (1001) docker     (122)   126684 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/platforms/evm.py
--rw-r--r--   0 runner    (1001) docker     (122)   145626 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (122)    39079 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/platforms/linux_syscall_stubs.py
--rw-r--r--   0 runner    (1001) docker     (122)    35214 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/platforms/linux_syscalls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/platforms/platform.py
--rw-r--r--   0 runner    (1001) docker     (122)    17265 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/platforms/wasm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/command_line.py
--rw-r--r--   0 runner    (1001) docker     (122)    11075 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    19441 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/emulate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     7679 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/event.py
--rw-r--r--   0 runner    (1001) docker     (122)    11226 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/fallback_emulator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6517 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/install_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)     6282 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/utils/nointerrupt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore/wasm/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/wasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      734 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/wasm/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    53332 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/wasm/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)     8530 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/wasm/manticore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/wasm/state.py
--rw-r--r--   0 runner    (1001) docker     (122)    76013 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/wasm/structure.py
--rw-r--r--   0 runner    (1001) docker     (122)    12023 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/manticore/wasm/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15363 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2534 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/manticore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 12:53:59.000000 manticore-0.3.8.dev230721/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2664 2023-07-21 12:53:52.000000 manticore-0.3.8.dev230721/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/
+-rw-r--r--   0 runner    (1001) docker     (122)    15363 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12497 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8393 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/binary/
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/binary/binary.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49622 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/manticore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28116 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/core/smtlib/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/smtlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17980 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/smtlib/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44912 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/smtlib/expression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/smtlib/operators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39663 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/smtlib/solver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38537 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/smtlib/visitors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23618 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10874 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/state_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16180 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20267 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/core/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/ethereum/
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14383 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/abi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5031 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/abitypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5299 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4572 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39008 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    81041 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/manticore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8264 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/parsetab.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11447 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14652 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/solidity.py
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19857 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/ethereum/verifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/native/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/native/cpu/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   163406 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cpu/aarch64.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41088 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cpu/abstractcpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    62492 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cpu/arm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7715 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cpu/bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cpu/cpufactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cpu/disasm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cpu/register.py
+-rw-r--r--   0 runner    (1001) docker     (122)   255150 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/cpu/x86.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18111 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/manticore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56205 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9960 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6100 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13875 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10474 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/native/state_merging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/platforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18558 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/platforms/cgcrandom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40996 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/platforms/decree.py
+-rw-r--r--   0 runner    (1001) docker     (122)   126684 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/platforms/evm.py
+-rw-r--r--   0 runner    (1001) docker     (122)   145626 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39079 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/platforms/linux_syscall_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35214 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/platforms/linux_syscalls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/platforms/platform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17265 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/platforms/wasm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11075 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19441 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/emulate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7679 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11226 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/fallback_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6517 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/install_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6282 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/utils/nointerrupt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore/wasm/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/wasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      734 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/wasm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53332 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/wasm/executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8530 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/wasm/manticore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/wasm/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    76013 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/wasm/structure.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12023 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/manticore/wasm/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15363 2023-07-22 12:43:51.000000 manticore-0.3.8.dev230722/manticore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2534 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/manticore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 12:43:51.000000 manticore-0.3.8.dev230722/manticore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-22 12:43:51.000000 manticore-0.3.8.dev230722/manticore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-22 12:43:51.000000 manticore-0.3.8.dev230722/manticore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-22 12:43:51.000000 manticore-0.3.8.dev230722/manticore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-22 12:43:52.000000 manticore-0.3.8.dev230722/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2664 2023-07-22 12:43:47.000000 manticore-0.3.8.dev230722/setup.py
```

### Comparing `manticore-0.3.8.dev230721/PKG-INFO` & `manticore-0.3.8.dev230722/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manticore
-Version: 0.3.8.dev230721
+Version: 0.3.8.dev230722
 Summary: Manticore is a symbolic execution tool for analysis of binaries and smart contracts.
 Home-page: https://github.com/trailofbits/manticore
 Author: Trail of Bits
 License: UNKNOWN
 Description: # :warning: Project is in Maintenance Mode :warning:
         
         This project is no longer internally developed and maintained. However, we are happy to review and accept small, well-written pull requests by the community. We will only consider bug fixes and minor enhancements.
```

### Comparing `manticore-0.3.8.dev230721/README.md` & `manticore-0.3.8.dev230722/README.md`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/__main__.py` & `manticore-0.3.8.dev230722/manticore/__main__.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/binary/__init__.py` & `manticore-0.3.8.dev230722/manticore/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/binary/binary.py` & `manticore-0.3.8.dev230722/manticore/binary/binary.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/manticore.py` & `manticore-0.3.8.dev230722/manticore/core/manticore.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/parser/parser.py` & `manticore-0.3.8.dev230722/manticore/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/plugin.py` & `manticore-0.3.8.dev230722/manticore/core/plugin.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/smtlib/constraints.py` & `manticore-0.3.8.dev230722/manticore/core/smtlib/constraints.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/smtlib/expression.py` & `manticore-0.3.8.dev230722/manticore/core/smtlib/expression.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/smtlib/operators.py` & `manticore-0.3.8.dev230722/manticore/core/smtlib/operators.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/smtlib/solver.py` & `manticore-0.3.8.dev230722/manticore/core/smtlib/solver.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/smtlib/visitors.py` & `manticore-0.3.8.dev230722/manticore/core/smtlib/visitors.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/state.py` & `manticore-0.3.8.dev230722/manticore/core/state.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/state_pb2.py` & `manticore-0.3.8.dev230722/manticore/core/state_pb2.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/worker.py` & `manticore-0.3.8.dev230722/manticore/core/worker.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/core/workspace.py` & `manticore-0.3.8.dev230722/manticore/core/workspace.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/__init__.py` & `manticore-0.3.8.dev230722/manticore/ethereum/__init__.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/abi.py` & `manticore-0.3.8.dev230722/manticore/ethereum/abi.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/abitypes.py` & `manticore-0.3.8.dev230722/manticore/ethereum/abitypes.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/account.py` & `manticore-0.3.8.dev230722/manticore/ethereum/account.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/cli.py` & `manticore-0.3.8.dev230722/manticore/ethereum/cli.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/detectors.py` & `manticore-0.3.8.dev230722/manticore/ethereum/detectors.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/manticore.py` & `manticore-0.3.8.dev230722/manticore/ethereum/manticore.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/parsetab.py` & `manticore-0.3.8.dev230722/manticore/ethereum/parsetab.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/plugins.py` & `manticore-0.3.8.dev230722/manticore/ethereum/plugins.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/solidity.py` & `manticore-0.3.8.dev230722/manticore/ethereum/solidity.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/state.py` & `manticore-0.3.8.dev230722/manticore/ethereum/state.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/ethereum/verifier.py` & `manticore-0.3.8.dev230722/manticore/ethereum/verifier.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/exceptions.py` & `manticore-0.3.8.dev230722/manticore/exceptions.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/cli.py` & `manticore-0.3.8.dev230722/manticore/native/cli.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/cpu/aarch64.py` & `manticore-0.3.8.dev230722/manticore/native/cpu/aarch64.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/cpu/abstractcpu.py` & `manticore-0.3.8.dev230722/manticore/native/cpu/abstractcpu.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/cpu/arm.py` & `manticore-0.3.8.dev230722/manticore/native/cpu/arm.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/cpu/bitwise.py` & `manticore-0.3.8.dev230722/manticore/native/cpu/bitwise.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/cpu/cpufactory.py` & `manticore-0.3.8.dev230722/manticore/native/cpu/cpufactory.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/cpu/disasm.py` & `manticore-0.3.8.dev230722/manticore/native/cpu/disasm.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/cpu/register.py` & `manticore-0.3.8.dev230722/manticore/native/cpu/register.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/cpu/x86.py` & `manticore-0.3.8.dev230722/manticore/native/cpu/x86.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/manticore.py` & `manticore-0.3.8.dev230722/manticore/native/manticore.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/mappings.py` & `manticore-0.3.8.dev230722/manticore/native/mappings.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/memory.py` & `manticore-0.3.8.dev230722/manticore/native/memory.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/models.py` & `manticore-0.3.8.dev230722/manticore/native/models.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/plugins.py` & `manticore-0.3.8.dev230722/manticore/native/plugins.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/state.py` & `manticore-0.3.8.dev230722/manticore/native/state.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/native/state_merging.py` & `manticore-0.3.8.dev230722/manticore/native/state_merging.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/platforms/cgcrandom.py` & `manticore-0.3.8.dev230722/manticore/platforms/cgcrandom.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/platforms/decree.py` & `manticore-0.3.8.dev230722/manticore/platforms/decree.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/platforms/evm.py` & `manticore-0.3.8.dev230722/manticore/platforms/evm.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/platforms/linux.py` & `manticore-0.3.8.dev230722/manticore/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/platforms/linux_syscall_stubs.py` & `manticore-0.3.8.dev230722/manticore/platforms/linux_syscall_stubs.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/platforms/linux_syscalls.py` & `manticore-0.3.8.dev230722/manticore/platforms/linux_syscalls.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/platforms/platform.py` & `manticore-0.3.8.dev230722/manticore/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/platforms/wasm.py` & `manticore-0.3.8.dev230722/manticore/platforms/wasm.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/command_line.py` & `manticore-0.3.8.dev230722/manticore/utils/command_line.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/config.py` & `manticore-0.3.8.dev230722/manticore/utils/config.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/deprecated.py` & `manticore-0.3.8.dev230722/manticore/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/emulate.py` & `manticore-0.3.8.dev230722/manticore/utils/emulate.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/enums.py` & `manticore-0.3.8.dev230722/manticore/utils/enums.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/event.py` & `manticore-0.3.8.dev230722/manticore/utils/event.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/fallback_emulator.py` & `manticore-0.3.8.dev230722/manticore/utils/fallback_emulator.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/helpers.py` & `manticore-0.3.8.dev230722/manticore/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/install_helper.py` & `manticore-0.3.8.dev230722/manticore/utils/install_helper.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/log.py` & `manticore-0.3.8.dev230722/manticore/utils/log.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/utils/nointerrupt.py` & `manticore-0.3.8.dev230722/manticore/utils/nointerrupt.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/wasm/cli.py` & `manticore-0.3.8.dev230722/manticore/wasm/cli.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/wasm/executor.py` & `manticore-0.3.8.dev230722/manticore/wasm/executor.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/wasm/manticore.py` & `manticore-0.3.8.dev230722/manticore/wasm/manticore.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/wasm/state.py` & `manticore-0.3.8.dev230722/manticore/wasm/state.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/wasm/structure.py` & `manticore-0.3.8.dev230722/manticore/wasm/structure.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore/wasm/types.py` & `manticore-0.3.8.dev230722/manticore/wasm/types.py`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore.egg-info/PKG-INFO` & `manticore-0.3.8.dev230722/manticore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manticore
-Version: 0.3.8.dev230721
+Version: 0.3.8.dev230722
 Summary: Manticore is a symbolic execution tool for analysis of binaries and smart contracts.
 Home-page: https://github.com/trailofbits/manticore
 Author: Trail of Bits
 License: UNKNOWN
 Description: # :warning: Project is in Maintenance Mode :warning:
         
         This project is no longer internally developed and maintained. However, we are happy to review and accept small, well-written pull requests by the community. We will only consider bug fixes and minor enhancements.
```

### Comparing `manticore-0.3.8.dev230721/manticore.egg-info/SOURCES.txt` & `manticore-0.3.8.dev230722/manticore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/manticore.egg-info/requires.txt` & `manticore-0.3.8.dev230722/manticore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `manticore-0.3.8.dev230721/setup.py` & `manticore-0.3.8.dev230722/setup.py`

 * *Files identical despite different names*

