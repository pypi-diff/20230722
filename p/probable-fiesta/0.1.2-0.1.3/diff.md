# Comparing `tmp/probable_fiesta-0.1.2.tar.gz` & `tmp/probable_fiesta-0.1.3.tar.gz`

## Comparing `probable_fiesta-0.1.2.tar` & `probable_fiesta-0.1.3.tar`

### file list

```diff
@@ -1,80 +1,153 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/env
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/requirements.txt
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tox.ini
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/.github/workflows/python_app.yml
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/.github/workflows/python_publish.yml
--rwxr-xr-x   0        0        0      587 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/scripts/build_install.sh
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/scripts/build_publish.sh
--rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/scripts/run_tests.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/scripts/templater.sh
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/scripts/test_coverage.sh
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/app/__init__.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/app/builder/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/app/builder/app_abstract_machine.py
--rw-r--r--   0        0        0    10326 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/app/builder/app_builder.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/app/builder/context.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/app/builder/context_builder.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/app/builder/context_factory.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/app/builder/context_holder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/cli/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/cli/builder/my_args_parser.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/cli/builder/parser.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/cli/builder/parser_builder.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/cli/builder/parser_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/command/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/command/builder/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/command/builder/command.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/command/builder/command_builder.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/command/builder/command_factory.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/command/builder/command_queue.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/command/builder/command_queue_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/config/_init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/config/default_config.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/config/module_config.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/config/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/config/builder/__init__.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/config/builder/config.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/config/builder/config_builder.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/config/builder/config_builder_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/logger/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/logger/logger_module.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/logger/logging_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/logger/builder/__init__.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/logger/builder/logger.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/logger/builder/logger_abstract_machine.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/logger/builder/logger_builder.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/logger/builder/logger_factory.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/run/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/src/probable_fiesta/run/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/__init__py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/test_main_app.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/test_v1.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/app/builder/__init__.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/app/builder/test_app_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/cli/builder/__init__.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/cli/builder/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/command/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/command/builder/__init__.py
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/command/builder/test_command.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/command/builder/test_command_builder.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/command/builder/test_command_factory.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/command/builder/test_command_queue.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/config/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/config/builder/__init__.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/config/builder/test_config.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/config/builder/test_config_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/logger/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/logger/builder/__init__.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/logger/builder/test_logger.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/tests/logger/builder/test_logger_factory.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/LICENSE
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/hatch.toml
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 probable_fiesta-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.env
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/env
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tox.ini
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.github/workflows/python_app.yml
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/README.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/.gitignore
+-rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0    18544 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_0293064cae6f51b1_args_parse_py.html
+-rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_0293064cae6f51b1_args_parser_factory_py.html
+-rw-r--r--   0        0        0    17408 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_0293064cae6f51b1_parser_builder_py.html
+-rw-r--r--   0        0        0    29534 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_309aba7555c96ec5_logger_abstract_machine_py.html
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_309aba7555c96ec5_logger_factory_py.html
+-rw-r--r--   0        0        0    32638 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_309aba7555c96ec5_logger_py.html
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_3b40d2e1b447d1de___about___py.html
+-rw-r--r--   0        0        0    45718 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_app_abstract_machine_py.html
+-rw-r--r--   0        0        0    58461 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_app_builder_py.html
+-rw-r--r--   0        0        0    16956 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_app_py.html
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_context_factory_py.html
+-rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_context_holder_py.html
+-rw-r--r--   0        0        0     9775 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_context_py.html
+-rw-r--r--   0        0        0    56232 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_my_app_builder_py.html
+-rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_5c9f86e17f38c9da_test_logger_factory_py.html
+-rw-r--r--   0        0        0    33986 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_5c9f86e17f38c9da_test_logger_py.html
+-rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_7a0574776d91e073_test_app_builder_py.html
+-rw-r--r--   0        0        0    14310 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_7a0574776d91e073_test_app_py.html
+-rw-r--r--   0        0        0    20353 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_7a0574776d91e073_test_my_app_builder_py.html
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_929858da485d1af8_logging_config_py.html
+-rw-r--r--   0        0        0    38348 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_9610c8957119e03c_main_py.html
+-rw-r--r--   0        0        0    17287 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_a44f0ac069e85531_test_main_app_py.html
+-rw-r--r--   0        0        0    14163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_a44f0ac069e85531_test_v1_py.html
+-rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_b5ab6064aa946d24_v1_py.html
+-rw-r--r--   0        0        0    38305 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_config_builder_py.html
+-rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_config_factory_py.html
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_default_config_py.html
+-rw-r--r--   0        0        0    12207 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_variables_py.html
+-rw-r--r--   0        0        0    32979 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_builder_py.html
+-rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_factory_py.html
+-rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_py.html
+-rw-r--r--   0        0        0    31733 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_queue_py.html
+-rw-r--r--   0        0        0    16599 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_builder_py.html
+-rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_factory_py.html
+-rw-r--r--   0        0        0    29275 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_py.html
+-rw-r--r--   0        0        0    24515 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_queue_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/status.json
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/style.css
+-rwxr-xr-x   0        0        0      587 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/build_install.sh
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/build_publish.sh
+-rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/run_tests.sh
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/templater.sh
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/test_coverage.sh
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/__init__.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/app_abstract_machine.py
+-rw-r--r--   0        0        0    10852 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/app_builder.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/command_context_factory.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_builder.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_factory.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_holder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/my_args_parser.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser_builder.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/__init__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_builder.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_factory.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_queue.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_queue_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/_init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/default_config.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/module_config.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/builder/__init__.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config_builder.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config_builder_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/logger_module.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/logging_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/__init__.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_abstract_machine.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_builder.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_factory.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/run/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/run/main.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/__about__.py.j2
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/hatch.toml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/hatch.toml.j2
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/make_skeleton.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/pyproject.toml
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/pyproject.toml.j2
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/run___init__.py.j2
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/tox.ini
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/tox.ini.j2
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/write_templates.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/cli/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/run/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/run/main.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/test_main_app.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/test_v1.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/app/builder/__init__.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/app/builder/test_app_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/cli/builder/__init__.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/cli/builder/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/__init__.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command_builder.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command_context_factory.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command_factory.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command_queue.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/config/builder/__init__.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/config/builder/test_config.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/config/builder/test_config_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/logger/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/logger/builder/__init__.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/logger/builder/test_logger.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/logger/builder/test_logger_factory.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/hatch.toml
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/PKG-INFO
```

### Comparing `probable_fiesta-0.1.2/requirements.txt` & `probable_fiesta-0.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/.github/workflows/python_app.yml` & `probable_fiesta-0.1.3/.github/workflows/python_app.yml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/.github/workflows/python_publish.yml` & `probable_fiesta-0.1.3/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/scripts/build_install.sh` & `probable_fiesta-0.1.3/scripts/build_install.sh`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/app/main.py` & `probable_fiesta-0.1.3/src/probable_fiesta/app/main.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/app/builder/app_abstract_machine.py` & `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/app_abstract_machine.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/app/builder/app_builder.py` & `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/app_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 """App builder module."""
 from ...cli.builder.parser import Parser
 from .context_holder import ContextHolder
 
+from ...logger.builder.logger_abstract_machine import LoggerMachine
+
+machine = LoggerMachine()
+SYSTEM_LOG = machine.make_logger(
+    type=LoggerMachine.Available.DEFAULT,
+    name="system",
+    level="INFO",
+    fmt="simple",
+    directory="logs",
+)
+
 
 class App:
     def __init__(self):
         # properties
         self.name = None
         self.args_parser = None
         self.arguments = None
@@ -13,14 +24,15 @@
         self.context = None  # context_holder
         # internal properties
         self.valid = False
         self.error = None
         self.run_history = []
         self.cleaned_args = {}
         self.executables = []  # commands to be run from args
+        self.output = None
 
     def __str__(self):
         return f"App: {self.__dict__}"
 
     def validate(self):
         local_valid = True
 
@@ -65,59 +77,65 @@
     def run(self, name=None):
         if not self.valid:
             print("App is not valid.\nTrying to run anyway.")
             # print(self.context)
             if name is None:
                 # Running without cleaned arguments that match context
                 for name in self.context.context_holder.keys():
-                    context = self.context.context_holder[name]
-                    context_run = context.command_queue.run_all()
-                    context_run_history = context_run.get_history()
-                    self.context_run_history.append(context_run_history)
+                    context = self.context.context_holder[name].command_queue.run_all()
+                    self.output = context  # Add this line
+                    print(
+                        "DEBUG: Context name:", name
+                    )  # Add this print statement for debugging
+                    print("DEBUG: CommandQueue object:", context)  # Change this line
+                    self.output = context_run.get_output()
                 return self
-            command_queue = self.context.context_holder[name].command_queue.run_all()
-            self.run_history.append(command_queue.get_history())
+            context_run = self.context.context_holder[name].command_queue.run_all()
+            self.run_history.append(context_run.get_history())
             return self
 
         # print("App is valid")
+
         # Run all commands from cleaned arguments that match context
         if name is None:
             for name in self.cleaned_args.keys():
                 if name in self.executables:
                     if name in self.context.context_holder.keys():
                         # print("Running command from args: ", name)
                         context_run = self.context.context_holder[
                             name
                         ].command_queue.run_all()
                         self.run_history.append(context_run.get_history())
+                        # Add the following line to store the output after appending to run_history
+                        self.output = context_run.get_output()
             return self
 
         # print("Running one command for context: ", name)
         context_run = self.context.context_holder[name].command_queue.run_all()
         self.run_history.append(context_run.get_history())
         return self
 
     def get_run_history(self):
         if len(self.run_history) == 0:
             print("No run history found")
-            return
+            return []
         if len(self.run_history) == 1:
             return self.run_history[0]
         return self.run_history
 
     def clear_run_history(self):
         self.run_history = []
         return self
 
     def get_arg(self, name):
         try:
             # dotenv is in uppercase
             found_arg = self.config.get_setting(name.upper())
         except KeyError:
-            # print("No dotenv config set for: ", name)
+            SYSTEM_LOG.warning("No dotenv config set for: ", name)
             found_arg = None
         # flags have priority
         if name.lower() in self.cleaned_args.keys():
             found_arg = self.cleaned_args[name.lower()]
         return found_arg
 
 
@@ -151,14 +169,17 @@
     def build(self):
         return self.app
 
     def validate(self):
         self.app.validate()
         return self
 
+    def get_output(self):
+        return self.output
+
 
 class AppContextBuilder(AppBuilder):
     def __init__(self, app):
         super().__init__(app)
 
     def add_context(self, context):
         if self.app.context is None:
@@ -210,22 +231,20 @@
         self.app.cleaned_args = self.clean_arg_function(arguments)
         return self
 
     def set_executables(self, executables: list):
         self.app.executables = executables
         return self
 
+    # TODO: This method needs work
     @staticmethod
     def map_short_flags(arguments, parsed_args):
         for arg in parsed_args.keys():
             clean = arg.split("_")[-1]
-            print(clean)
-            print(arguments)
             if clean in arguments:
-                print("HERE")
                 # update dictionary with long flag
                 arguments[arg] = arguments.pop(clean)
         return arguments
 
     @staticmethod
     def clean_arg_function(arguments: list) -> dict:
         cleaned_args = {}
@@ -277,15 +296,14 @@
                     else:  # 0 or less
                         arg_dict[clean_arg(args_list.pop())] = None
                 args_list.append(arg)
             else:
                 argv_list.append(arg)
 
         if len(args_list) > 1:
-            print("Many args_list: ", args_list)
             for x in args_list:
                 arg_dict[clean_arg(x)] = None
             # Use the last one as the remainder for argv_list
             if len(argv_list) > 1:
                 arg_dict[clean_arg(args_list.pop())] = [x for x in argv_list.pop()]
             elif len(argv_list) == 1:
                 arg_dict[clean_arg(args_list.pop())] = argv_list.pop()
@@ -298,15 +316,14 @@
                 arg_dict[clean_arg(args_list.pop())] = [x for x in argv_list.pop()]
             elif len(argv_list) == 1:
                 arg_dict[clean_arg(args_list.pop())] = argv_list.pop()
             else:  # 0 or less
                 arg_dict[clean_arg(args_list.pop())] = None
 
         else:
-            print("No args_list: ", args_list)
             for x in argv_list:
                 arg_dict[clean_arg(x)] = None
 
         return arg_dict
 
 
 class MyAppConfigBuilder(AppBuilder):
```

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/app/builder/context.py` & `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """App context class."""
+from ...command.builder.command_queue import CommandQueue
+
 
 class Context:
     def __init__(self, name=None, command_queue=None):
         self.name = name
-        self.command_queue = command_queue
+        if command_queue is None:
+            self.command_queue = CommandQueue()
+        else:
+            self.command_queue = command_queue
 
     def __str__(self):
         return f"Context: {self.__dict__}"
 
     @staticmethod
     def new_context(name=None, command_queue=None):
         return Context(name, command_queue)
 
-    class Factory():
+    class Factory:
         @staticmethod
         def new_context(name=None, command_queue=None):
             return Context(name, command_queue)
 
-    factory = Factory()
+    factory = Factory()
```

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/app/builder/context_builder.py` & `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/app/builder/context_factory.py` & `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 """Context Factory class."""
 from .context import Context
 from ...command.builder.command_queue import CommandQueue
 from ...command.builder.command_factory import CommandFactory
 
+
 class ContextFactory:
     @staticmethod
     def new_context(name=None, command_queue=None):
+        if command_queue is None:
+            command_queue = CommandQueue()
         return Context(name, command_queue)
 
     @staticmethod
     def new_context_one_new_command(context_name, command_name, function, *args):
         cq = CommandQueue.new(CommandFactory.new_command(command_name, function, *args))
         context = ContextFactory.new_context(context_name, cq)
         return context
 
     @staticmethod
     def new_context_one_command(context_name, command):
         cq = CommandQueue.new(command)
         context = ContextFactory.new_context(context_name, cq)
-        return context
+        return context
+
+    @staticmethod
+    def new_context_piped_commands(context_name, commands):
+        cq = CommandQueue()
+        for command in commands:
+            cq.add_command(command)
+        context = ContextFactory.new_context(context_name, cq)
+        return context
```

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/app/builder/context_holder.py` & `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_holder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/cli/builder/my_args_parser.py` & `probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/my_args_parser.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/cli/builder/parser.py` & `probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/cli/builder/parser_builder.py` & `probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/cli/builder/parser_factory.py` & `probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/command/builder/command.py` & `probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-"""Command class."""
 class Command:
-
     def __init__(self, name, function, *args):
         self.name = name
         self.function = function
         self.args = args
 
     def __str__(self):
         return f"Command: {self.__dict__}"
 
-    def invoke(self):
+    def invoke(self, input=None):
         if self.function is not None and self.args is not None:
-            if self.args[0] is not None:
+            if input is not None:
+                return self.function(input, *self.args)
+            else:
                 return self.function(*self.args)
-            return self.function()
-        #elif self.function is not None and self.args is None:
-            #return self.function()
         return None
 
-    class Factory():
-
+    class Factory:
         @staticmethod
         def new_command(name, function, *args):
             return Command(name, function, *args)
-    
+
     factory = Factory()
```

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/command/builder/command_builder.py` & `probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """CommandBuilder class."""
 
 from .command_queue import CommandQueue
 
-class CommandBuilder:
 
+class CommandBuilder:
     def __init__(self, command_queue=None):
         if command_queue is not None:
             self.command_queue = command_queue
         else:
             self.command_queue = CommandQueue()
 
     def __str__(self):
@@ -16,16 +16,16 @@
     @property
     def queue(self):
         return CommandBuilderQueue(self.command_queue)
 
     def build(self):
         return self.command_queue
 
-class CommandBuilderQueue(CommandBuilder):
 
+class CommandBuilderQueue(CommandBuilder):
     def __init__(self, command_queue):
         super().__init__(command_queue)
 
     def add_new_command(self, name, function, args=None):
         self.command_queue.add_new_command(name, function, args)
         return self
 
@@ -96,8 +96,14 @@
     def add_command_factories(self, command_factories):
         for command_factory in command_factories:
             self.add_command_factory(command_factory)
         return self
 
     def add_command_builder_factory(self, command_builder_factory):
         self.command_queue.add_command_queue(command_builder_factory.build())
-        return self
+        return self
+
+    def run_piped_commands(self, commands):
+        input_data = None
+        for command in commands:
+            input_data = self.command_queue.run_command(command, input_data)
+        return input_data
```

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/config/module_config.py` & `probable_fiesta-0.1.3/src/probable_fiesta/config/module_config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/config/variables.py` & `probable_fiesta-0.1.3/src/probable_fiesta/config/variables.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/config/builder/config.py` & `probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/config/builder/config_builder.py` & `probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from ...logger.builder.logger_factory import LoggerFactory
 from .config import Config
 
-class ConfigBuilder():
+
+class ConfigBuilder:
     def __init__(self, config=None):
         if config is None:
             self.config = Config()
         else:
             self.config = config
-    
+
     def __str__(self):
         return f"ConfigBuilder: {self.config.__dict__}"
 
     @property
     def package(self):
         return ConfigPackage(self.config)
 
@@ -26,26 +27,28 @@
     @property
     def dotenv(self):
         return ConfigDotEnv(self.config)
 
     def build(self):
         return self.config
 
+
 class ConfigPackage(ConfigBuilder):
     def __init__(self, config):
         super().__init__(config)
 
     def set_package_name(self, name):
-        self.config.package['name'] = name
+        self.config.package["name"] = name
         return self
 
     def set_root_dir(self, directory):
-        self.config.package['root_directory'] = directory
+        self.config.package["root_directory"] = directory
         return self
 
+
 class ConfigLogger(ConfigBuilder):
     def __init__(self, config):
         super().__init__(config)
 
     def set_logger_level(self, level):
         self.config.logger = level
         return self
@@ -83,31 +86,42 @@
         self.config.variables.update(variables)
         return self
 
     def get_from_module_config(self):
         self.config.variables.update(self.config.variables.module_config)
         return self
 
+
 class ConfigDotEnv(ConfigBuilder):
     def __init__(self, config):
         super().__init__(config)
 
-    def load_dotenv(self):
+    def load_dotenv(self, path=".env"):
         try:
             import dotenv as _dotenv
         except ImportError:
             print("Warning: dotenv package not installed.")
-            self.dotenv = None
-        if _dotenv is not None:
-            _dotenv.load_dotenv()
-        return self
-    
-    def get_var(self, var_name):
-        import os
-        if os.getenv(var_name) is not None:
-            self.config.parsed_dotenv[var_name] = os.getenv(var_name)
+        else:
+            self._dotenv = _dotenv
+            self.parse_vars(path)
         return self
 
+    def parse_vars(self, path):
+        try:
+            with open(path) as f:
+                for line in f:
+                    key, value = line.strip().split("=", 1)
+                    self.config.parsed_dotenv[key] = value
+        except IOError:
+            print(f"Warning: Unable to open .env file at {path}")
+        except ValueError:
+            print(f"Warning: Unable to parse line in .env file: {line}")
+
     def set_vars(self, vars):
         for var in vars:
             self.get_var(var)
-        return self
+        return self
+
+    def get_var(self, var_name):
+        if var_name in self.config.parsed_dotenv:
+            return self.config.parsed_dotenv[var_name]
+        return None
```

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/config/builder/config_builder_factory.py` & `probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config_builder_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/logger/logging_config.py` & `probable_fiesta-0.1.3/src/probable_fiesta/logger/logging_config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/logger/builder/logger_abstract_machine.py` & `probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_abstract_machine.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,68 @@
 from abc import ABC
 from enum import Enum, auto
 
 from .logger_factory import LoggerFactory
 
+
 class AbstractLogger(ABC):
     def create_logger(self):
-        pass
+        raise NotImplementedError
+
 
 class LoggerDefault(AbstractLogger):
     def create_logger(self):
-        pass
+        raise NotImplementedError
+
 
 class LoggerFlask(AbstractLogger):
     def create_logger(self):
-        pass
+        raise NotImplementedError
+
 
 class LoggerAbstractFactory(ABC):
-    def create_logger(self, name, level, fmt, directory):
-        pass
-    def create_logger(self, app, name, level, fmt, directory):
-        pass
+    def create_default_logger(self, name, level, fmt, directory):
+        raise NotImplementedError
+
+    def create_flask_logger(self, app, name, level, fmt, directory):
+        raise NotImplementedError
+
 
 class DefaultFactory(LoggerAbstractFactory):
-    def create_logger(self, name, level, fmt, directory):
-        print("Creating default logger")
+    def create_default_logger(self, name, level, fmt, directory):
+        # print("Creating default logger")
         logger = LoggerFactory().new_logger_get_logger(name, level, fmt, directory)
         return logger
 
+
 class FlaskFactory(LoggerAbstractFactory):
-    def create_logger(self, app, name, level, fmt, directory):
-        print("Creating flask logger")
+    def create_flask_logger(self, app, name, level, fmt, directory):
+        # print("Creating flask logger")
         logger = LoggerFactory().new_logger_flask(app, name, level, fmt, directory)
         return logger
 
+
 class LoggerMachine:
     class Available(Enum):
         DEFAULT = auto()
         FLASK = auto()
-    
-    factories = []
-    initialized = False
-
-    def __init__(self):
-        if not self.initialized:
-            self.initialized = True
-            for d in self.Available:
-                name = d.name[0] +  d.name[1:].lower()
-                factory_name = name + "Factory"
-                factory_instance = eval(factory_name)()
-                self.factories.append((name, factory_instance))
+
+    factories = {Available.DEFAULT: DefaultFactory(), Available.FLASK: FlaskFactory()}
 
     def __str__(self):
-        return f"LoggerMachine: Available loggers: {self.factories}"
+        return f"LoggerMachine: Available loggers: {list(self.factories.keys())}"
 
-    def prepare_logger(self):
-        print("Available apps:")
-        for f in self.factories:
-            print(f[0])
-        s = input(f'Please pick app (0-{len(self.factories)-1}):')
-        idx = int(s)
-        return self.factories[idx][1].get()
-
-    def make_logger(self, type, app=None, name=None, level=None, fmt=None, directory=None):
-        if type == 'default':
-            return DefaultFactory().create_logger(name, level, fmt, directory)
-        elif type == 'flask':
-            return FlaskFactory().create_logger(app, name, level, fmt, directory)
+    def make_logger(
+        self, type, app=None, name=None, level=None, fmt=None, directory=None
+    ):
+        if type in self.factories:
+            if type == LoggerMachine.Available.DEFAULT:
+                return self.factories[type].create_default_logger(
+                    name, level, fmt, directory
+                )
+            elif type == LoggerMachine.Available.FLASK:
+                return self.factories[type].create_flask_logger(
+                    app, name, level, fmt, directory
+                )
         else:
             print("Invalid logger type")
             return None
-
-def make_logger(type, app=None, name=None, level=None, fmt=None, directory=None):
-    if type == 'default':
-        return DefaultFactory().create_logger(name, level, fmt, directory)
-    elif type == 'flask':
-        return FlaskFactory().create_logger(app, name, level, fmt, directory)
-    else:
-        print("Invalid logger type")
-        return None
```

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/logger/builder/logger_builder.py` & `probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 from .logger import Logger
+from .logger import LoggerFactory
+
 
 class LoggerBuilder:
     def __init__(self, logger=None):
         if logger is None:
-            self.logger = Logger().new()
+            self.logger = Logger.factory.new_logger()
         else:
-            self.logger = logger().new().set_logger(logger)
+            self.logger = logger
 
     def __str__(self):
         return f"LoggerBuilder: {self.__dict__}"
 
     @property
     def logger(self):
-        return LoggerBuilderLogger(self.logger)
+        return self._logger
+
+    @logger.setter
+    def logger(self, logger):
+        self._logger = logger
 
     def build(self):
         return self.logger
 
+
 class LoggerBuilderLogger(LoggerBuilder):
     def __init__(self, logger):
         super().__init__(logger)
 
-    def get_logger_flask_application(self, application, name=None, level=None, fmt=None, directory=None, filename=None):
-        _file_handler = self.logger.Factory.new_logger_handler(name, level, fmt, directory, filename)
-        if not self.logger.file_handler:
-            print("File handler not set")
-        application.logger.add_handler = self.logger.file_handler
-        yield application
-
-    def get_logger_default(self, name=None, level=None, fmt=None, directory=None, filename=None):
+    def get_logger_flask_application(
+        self,
+        application,
+        name=None,
+        level=None,
+        fmt=None,
+        directory=None,
+        filename=None,
+    ):
+        _file_handler = Logger.factory.new_file_handler(name, level, fmt, directory)
+        application.logger.addHandler(_file_handler)
+        return application
+
+    def get_logger_default(
+        self, name=None, level=None, fmt=None, directory=None, filename=None
+    ):
         print("Getting default logger")
-        self.logger = self.logger.Factory.new_logger(name, level, fmt, directory, filename)
-        return self
+        self.logger = LoggerFactory.new_logger_default(name, level, fmt, directory)
+        return self
```

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/logger/builder/logger_factory.py` & `probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from .logger import Logger
 from ...config.variables import LoggerDef
 
+
 class LoggerFactory:
     @staticmethod
     def new_logger(name=None, level=None, fmt=None, directory=None):
-        return Logger.new(name, level, fmt, directory)
+        return Logger.factory.new_logger(name, level, fmt, directory)
 
     @staticmethod
     def new_logger_get_logger(name=None, level=None, fmt=None, directory=None):
         return Logger.new_get_logger(name, level, fmt, directory)
 
     @staticmethod
     def new_logger_default(name=None, level=None, fmt=None, directory=None):
-        directory = directory
         if not directory:
-            directory = LoggerDef.ROOT_DIR+'/logger'
+            directory = LoggerDef.ROOT_DIR + "/logger"
         if not fmt:
             fmt = LoggerDef.FORMAT
-        return Logger.new(name, level, fmt, directory) 
+        return Logger.new_get_logger(name, level, fmt, directory)
 
     @staticmethod
     def new_logger_flask(app, name, level, fmt, directory):
-        file_handler = Logger.Factory.create_file_handler(name, level, fmt, directory)
+        file_handler = Logger.factory.new_file_handler(name, level, fmt, directory)
         app.logger.addHandler(file_handler)
-        return app.logger
+        return app.logger
```

### Comparing `probable_fiesta-0.1.2/src/probable_fiesta/run/__init__.py` & `probable_fiesta-0.1.3/src/probable_fiesta/run/__init__.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/test_v1.py` & `probable_fiesta-0.1.3/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/app/builder/test_app_builder.py` & `probable_fiesta-0.1.3/tests/app/builder/test_app_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/cli/builder/test_parser.py` & `probable_fiesta-0.1.3/tests/cli/builder/test_parser.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/command/builder/test_command.py` & `probable_fiesta-0.1.3/tests/command/builder/test_command.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/command/builder/test_command_builder.py` & `probable_fiesta-0.1.3/tests/command/builder/test_command_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/command/builder/test_command_factory.py` & `probable_fiesta-0.1.3/tests/command/builder/test_command_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/command/builder/test_command_queue.py` & `probable_fiesta-0.1.3/tests/command/builder/test_command_queue.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/config/builder/test_config.py` & `probable_fiesta-0.1.3/tests/config/builder/test_config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/config/builder/test_config_builder.py` & `probable_fiesta-0.1.3/tests/config/builder/test_config_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/logger/builder/test_logger.py` & `probable_fiesta-0.1.3/tests/logger/builder/test_logger.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/tests/logger/builder/test_logger_factory.py` & `probable_fiesta-0.1.3/tests/logger/builder/test_logger_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/.gitignore` & `probable_fiesta-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/LICENSE` & `probable_fiesta-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/README.md` & `probable_fiesta-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/hatch.toml` & `probable_fiesta-0.1.3/hatch.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/pyproject.toml` & `probable_fiesta-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.2/PKG-INFO` & `probable_fiesta-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probable_fiesta
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Core Package.
 Project-URL: Homepage, https://github.com/sergio-munoz/probable_fiesta/
 Project-URL: Bug Tracker, https://github.com/sergio-munoz/probable_fiesta/issues
 Project-URL: Documentation, https://github.com/sergio-munoz/probable_fiesta#readme
 Project-URL: Issues, https://github.com/sergio-munoz/probable_fiesta/issues
 Project-URL: Source, https://github.com/sergio-munoz/probable_fiesta
 Author-email: Sergio Munoz <sergio.munoz@pubnub.com>
```

