# Comparing `tmp/nopasaran-0.2.8.tar.gz` & `tmp/nopasaran-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.2.8.tar", last modified: Wed Jul 12 13:04:24 2023, max compression
+gzip compressed data, was "nopasaran-0.2.9.tar", last modified: Sat Jul 22 09:50:00 2023, max compression
```

## Comparing `nopasaran-0.2.8.tar` & `nopasaran-0.2.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 13:04:16.000000 nopasaran-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-12 13:04:24.588588 nopasaran-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-12 13:04:16.000000 nopasaran-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/controllers/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/controllers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/controllers/protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/control_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/definitions/transitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/errors/parsing_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/action_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/condition_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/ipsec_tunnels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/machines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/machines/action_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/machines/state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/parsers/interpreter_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/parsers/state_machine_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/nopasaran/primitives/action_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/action_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/control_channel_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/data_channel_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/data_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/dns_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/event_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/io_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/ip_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/nested_machine_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/tcp_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/action_primitives/udp_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/nopasaran/primitives/condition_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/condition_primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/condition_primitives/condition_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/condition_primitives/variable_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/nopasaran/primitives/transition_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/transition_primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/transition_primitives/assignment_transitions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/primitives/transition_primitives/transition_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/nopasaran/sniffers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/sniffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-12 13:04:16.000000 nopasaran-0.2.8/nopasaran/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.584588 nopasaran-0.2.8/nopasaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 13:04:24.000000 nopasaran-0.2.8/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:04:24.588588 nopasaran-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-12 13:04:23.000000 nopasaran-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:24.588588 nopasaran-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:04:16.000000 nopasaran-0.2.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.704595 nopasaran-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-22 09:49:52.000000 nopasaran-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-22 09:50:00.704595 nopasaran-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-22 09:49:52.000000 nopasaran-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.688595 nopasaran-0.2.9/nopasaran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.692595 nopasaran-0.2.9/nopasaran/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/controllers/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/controllers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/controllers/protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.692595 nopasaran-0.2.9/nopasaran/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/definitions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/definitions/control_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/definitions/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/definitions/transitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.692595 nopasaran-0.2.9/nopasaran/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/errors/parsing_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.692595 nopasaran-0.2.9/nopasaran/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/interpreters/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/interpreters/action_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/interpreters/condition_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/interpreters/interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.696595 nopasaran-0.2.9/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.696595 nopasaran-0.2.9/nopasaran/machines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/machines/action_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/machines/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.696595 nopasaran-0.2.9/nopasaran/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/parsers/interpreter_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/parsers/state_machine_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.696595 nopasaran-0.2.9/nopasaran/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.700595 nopasaran-0.2.9/nopasaran/primitives/action_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/action_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/control_channel_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/data_channel_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/data_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19650 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/dns_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/event_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/io_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/ip_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/nested_machine_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/tcp_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/action_primitives/udp_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.700595 nopasaran-0.2.9/nopasaran/primitives/condition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/condition_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/condition_primitives/condition_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/condition_primitives/variable_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.704595 nopasaran-0.2.9/nopasaran/primitives/transition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/transition_primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/transition_primitives/assignment_transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/primitives/transition_primitives/transition_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.704595 nopasaran-0.2.9/nopasaran/sniffers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-22 09:49:52.000000 nopasaran-0.2.9/nopasaran/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.688595 nopasaran-0.2.9/nopasaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-22 09:50:00.000000 nopasaran-0.2.9/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-22 09:50:00.000000 nopasaran-0.2.9/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 09:50:00.000000 nopasaran-0.2.9/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 09:50:00.000000 nopasaran-0.2.9/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-22 09:50:00.000000 nopasaran-0.2.9/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-22 09:50:00.000000 nopasaran-0.2.9/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 09:50:00.704595 nopasaran-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-22 09:49:59.000000 nopasaran-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:50:00.704595 nopasaran-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:49:52.000000 nopasaran-0.2.9/tests/__init__.py
```

### Comparing `nopasaran-0.2.8/LICENSE` & `nopasaran-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/PKG-INFO` & `nopasaran-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.8
+Version: 0.2.9
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.8/README.md` & `nopasaran-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/__main__.py` & `nopasaran-0.2.9/nopasaran/__main__.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/controllers/controller.py` & `nopasaran-0.2.9/nopasaran/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/controllers/factory.py` & `nopasaran-0.2.9/nopasaran/controllers/factory.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/controllers/protocol.py` & `nopasaran-0.2.9/nopasaran/controllers/protocol.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/decorators.py` & `nopasaran-0.2.9/nopasaran/decorators.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/definitions/control_channel.py` & `nopasaran-0.2.9/nopasaran/definitions/control_channel.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/errors/parsing_error.py` & `nopasaran-0.2.9/nopasaran/errors/parsing_error.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.2.9/nopasaran/interpreters/action_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/interpreters/condition_interpreter.py` & `nopasaran-0.2.9/nopasaran/interpreters/condition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/interpreters/interpreter.py` & `nopasaran-0.2.9/nopasaran/interpreters/interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.2.9/nopasaran/interpreters/transition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.2.9/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/machines/action_queue.py` & `nopasaran-0.2.9/nopasaran/machines/action_queue.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/machines/state_machine.py` & `nopasaran-0.2.9/nopasaran/machines/state_machine.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.2.9/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/parsers/state_machine_parser.py` & `nopasaran-0.2.9/nopasaran/parsers/state_machine_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/primitives/action_primitives/action_primitives.py` & `nopasaran-0.2.9/nopasaran/primitives/action_primitives/action_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/primitives/action_primitives/control_channel_primitives.py` & `nopasaran-0.2.9/nopasaran/primitives/action_primitives/control_channel_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/primitives/action_primitives/data_channel_primitives.py` & `nopasaran-0.2.9/nopasaran/primitives/action_primitives/data_channel_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/primitives/action_primitives/data_manipulation.py` & `nopasaran-0.2.9/nopasaran/primitives/action_primitives/data_manipulation.py`

 * *Files 13% similar despite different names*

```diff
@@ -104,8 +104,39 @@
             outputs (List[str]): The list of output variable names.
             
             state_machine: The state machine object.
 
         Returns:
             None
         """
-        state_machine.get_variable_value(inputs[0]).pop(0)
+        state_machine.get_variable_value(inputs[0]).pop(0)
+
+
+    @staticmethod
+    @parsing_decorator(input_args=1, output_args=1)
+    def get_first_element(inputs, outputs, state_machine):
+        """
+        Get the first element from a list stored in the machine's state.
+
+        Number of input arguments: 1
+
+        Number of output arguments: 1
+
+        Optional input arguments: No
+
+        Optional output arguments: No
+
+        Args:
+            inputs (List[str]): The list of input variable names. It contains one mandatory input argument,
+                which is the name of a variable representing the list.
+
+            outputs (List[str]): The list of output variable names. It contains one mandatory output argument,
+                which is the name of the variable to store the first element.
+
+            state_machine: The state machine object.
+
+        Returns:
+            None
+        """
+        input_list = state_machine.get_variable_value(inputs[0])
+        first_element = input_list[0]
+        state_machine.set_variable_value(outputs[0], first_element)
```

### Comparing `nopasaran-0.2.8/nopasaran/primitives/action_primitives/event_primitives.py` & `nopasaran-0.2.9/nopasaran/primitives/action_primitives/event_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/primitives/action_primitives/io_primitives.py` & `nopasaran-0.2.9/nopasaran/primitives/action_primitives/io_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/primitives/action_primitives/nested_machine_utils.py` & `nopasaran-0.2.9/nopasaran/primitives/action_primitives/nested_machine_utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/primitives/action_primitives/tcp_primitives.py` & `nopasaran-0.2.9/nopasaran/primitives/action_primitives/tcp_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/primitives/condition_primitives/variable_comparisons.py` & `nopasaran-0.2.9/nopasaran/primitives/condition_primitives/variable_comparisons.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/primitives/transition_primitives/assignment_transitions.py` & `nopasaran-0.2.9/nopasaran/primitives/transition_primitives/assignment_transitions.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran/sniffers/sniffer.py` & `nopasaran-0.2.9/nopasaran/sniffers/sniffer.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.2.9/nopasaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.8
+Version: 0.2.9
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.8/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.2.9/nopasaran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.8/setup.py` & `nopasaran-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 # Version will automatically be updated when pushed on the main branch
 setup(
     name="nopasaran",
-    version='0.2.8',
+    version='0.2.9',
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
```

