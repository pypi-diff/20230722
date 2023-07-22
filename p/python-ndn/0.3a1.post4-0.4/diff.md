# Comparing `tmp/python-ndn-0.3a1.post4.tar.gz` & `tmp/python_ndn-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ndn-0.3a1.post4.tar", last modified: Mon Jul  5 20:24:33 2021, max compression
+gzip compressed data, was "python_ndn-0.4.tar", max compression
```

## Comparing `python-ndn-0.3a1.post4.tar` & `python_ndn-0.4.tar`

### file list

```diff
@@ -1,97 +1,134 @@
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.399994 python-ndn-0.3a1.post4/
--rw-r--r--   0 cs217a     (501) staff       (20)      187 2020-09-25 00:48:59.000000 python-ndn-0.3a1.post4/AUTHORS.rst
--rw-r--r--   0 cs217a     (501) staff       (20)    10175 2019-11-26 04:57:08.000000 python-ndn-0.3a1.post4/COPYING
--rw-r--r--   0 cs217a     (501) staff       (20)     3971 2021-07-05 20:24:33.400154 python-ndn-0.3a1.post4/PKG-INFO
--rw-r--r--   0 cs217a     (501) staff       (20)      988 2021-04-29 18:37:08.000000 python-ndn-0.3a1.post4/README.rst
--rw-r--r--   0 cs217a     (501) staff       (20)       96 2021-07-02 04:01:59.000000 python-ndn-0.3a1.post4/pyproject.toml
--rw-r--r--   0 cs217a     (501) staff       (20)     1431 2021-07-05 20:24:33.401493 python-ndn-0.3a1.post4/setup.cfg
--rw-r--r--   0 cs217a     (501) staff       (20)       69 2021-07-02 08:34:37.000000 python-ndn-0.3a1.post4/setup.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.352630 python-ndn-0.3a1.post4/src/
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.358610 python-ndn-0.3a1.post4/src/ndn/
--rw-r--r--   0 cs217a     (501) staff       (20)       24 2021-07-02 04:13:19.000000 python-ndn-0.3a1.post4/src/ndn/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)    22914 2021-05-28 09:11:08.000000 python-ndn-0.3a1.post4/src/ndn/app.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.361867 python-ndn-0.3a1.post4/src/ndn/app_support/
--rw-r--r--   0 cs217a     (501) staff       (20)        0 2019-10-02 17:36:51.000000 python-ndn-0.3a1.post4/src/ndn/app_support/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2419 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/app_support/dispatcher.py
--rw-r--r--   0 cs217a     (501) staff       (20)     7122 2020-09-25 17:27:02.000000 python-ndn-0.3a1.post4/src/ndn/app_support/nfd_mgmt.py
--rw-r--r--   0 cs217a     (501) staff       (20)     5095 2021-05-29 09:18:09.000000 python-ndn-0.3a1.post4/src/ndn/app_support/security_v2.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2637 2020-09-25 17:27:17.000000 python-ndn-0.3a1.post4/src/ndn/app_support/segment_fetcher.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.362400 python-ndn-0.3a1.post4/src/ndn/bin/
--rw-r--r--   0 cs217a     (501) staff       (20)        0 2021-07-05 20:02:19.000000 python-ndn-0.3a1.post4/src/ndn/bin/__init__.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.363020 python-ndn-0.3a1.post4/src/ndn/bin/sec/
--rw-r--r--   0 cs217a     (501) staff       (20)      814 2021-07-05 20:06:43.000000 python-ndn-0.3a1.post4/src/ndn/bin/sec/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)       57 2021-07-05 20:07:14.000000 python-ndn-0.3a1.post4/src/ndn/bin/sec/__main__.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.363595 python-ndn-0.3a1.post4/src/ndn/bin/tools/
--rw-r--r--   0 cs217a     (501) staff       (20)      814 2021-07-05 20:06:51.000000 python-ndn-0.3a1.post4/src/ndn/bin/tools/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)       57 2021-07-05 20:07:49.000000 python-ndn-0.3a1.post4/src/ndn/bin/tools/__main__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     4021 2021-07-05 05:03:51.000000 python-ndn-0.3a1.post4/src/ndn/client_conf.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.363871 python-ndn-0.3a1.post4/src/ndn/contrib/
--rw-r--r--   0 cs217a     (501) staff       (20)        0 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post4/src/ndn/contrib/__init__.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.365626 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/
--rw-r--r--   0 cs217a     (501) staff       (20)     1742 2019-10-10 22:49:52.000000 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)    13048 2020-11-15 07:42:05.000000 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/cocoalibs.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2629 2019-10-10 22:49:52.000000 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/cocoatypes.py
--rw-r--r--   0 cs217a     (501) staff       (20)    51363 2020-11-15 07:58:22.000000 python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/runtime.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.372592 python-ndn-0.3a1.post4/src/ndn/encoding/
--rw-r--r--   0 cs217a     (501) staff       (20)      415 2019-09-28 20:57:01.000000 python-ndn-0.3a1.post4/src/ndn/encoding/__init__.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.375365 python-ndn-0.3a1.post4/src/ndn/encoding/name/
--rw-r--r--   0 cs217a     (501) staff       (20)    10641 2020-09-25 17:27:52.000000 python-ndn-0.3a1.post4/src/ndn/encoding/name/Component.py
--rw-r--r--   0 cs217a     (501) staff       (20)     6972 2020-09-25 17:27:57.000000 python-ndn-0.3a1.post4/src/ndn/encoding/name/Name.py
--rw-r--r--   0 cs217a     (501) staff       (20)       32 2019-11-07 04:59:36.000000 python-ndn-0.3a1.post4/src/ndn/encoding/name/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)    19631 2020-09-25 17:28:03.000000 python-ndn-0.3a1.post4/src/ndn/encoding/ndn_format_0_3.py
--rw-r--r--   0 cs217a     (501) staff       (20)     4173 2020-11-16 10:03:22.000000 python-ndn-0.3a1.post4/src/ndn/encoding/ndnlp_v2.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1975 2020-09-25 17:28:10.000000 python-ndn-0.3a1.post4/src/ndn/encoding/signer.py
--rw-r--r--   0 cs217a     (501) staff       (20)    34436 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/encoding/tlv_model.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1899 2020-09-25 17:28:19.000000 python-ndn-0.3a1.post4/src/ndn/encoding/tlv_type.py
--rw-r--r--   0 cs217a     (501) staff       (20)     5007 2020-09-25 17:28:23.000000 python-ndn-0.3a1.post4/src/ndn/encoding/tlv_var.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2725 2020-09-25 17:29:53.000000 python-ndn-0.3a1.post4/src/ndn/name_tree.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.378696 python-ndn-0.3a1.post4/src/ndn/platform/
--rw-r--r--   0 cs217a     (501) staff       (20)       69 2021-07-01 03:36:59.000000 python-ndn-0.3a1.post4/src/ndn/platform/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2100 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/platform/general.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1591 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/platform/linux.py
--rw-r--r--   0 cs217a     (501) staff       (20)     5480 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/platform/osx.py
--rw-r--r--   0 cs217a     (501) staff       (20)     6856 2021-07-05 05:03:42.000000 python-ndn-0.3a1.post4/src/ndn/platform/windows.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.384268 python-ndn-0.3a1.post4/src/ndn/schema/
--rw-r--r--   0 cs217a     (501) staff       (20)        0 2020-09-25 00:48:54.000000 python-ndn-0.3a1.post4/src/ndn/schema/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     3868 2020-09-25 17:33:09.000000 python-ndn-0.3a1.post4/src/ndn/schema/policy.py
--rw-r--r--   0 cs217a     (501) staff       (20)    25245 2021-04-29 18:34:03.000000 python-ndn-0.3a1.post4/src/ndn/schema/schema_tree.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2509 2020-09-25 17:33:19.000000 python-ndn-0.3a1.post4/src/ndn/schema/simple_cache.py
--rw-r--r--   0 cs217a     (501) staff       (20)     7378 2020-09-25 17:38:42.000000 python-ndn-0.3a1.post4/src/ndn/schema/simple_node.py
--rw-r--r--   0 cs217a     (501) staff       (20)     5780 2020-09-25 17:33:30.000000 python-ndn-0.3a1.post4/src/ndn/schema/simple_trust.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2839 2020-09-25 17:39:08.000000 python-ndn-0.3a1.post4/src/ndn/schema/util.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.384978 python-ndn-0.3a1.post4/src/ndn/security/
--rw-r--r--   0 cs217a     (501) staff       (20)      231 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post4/src/ndn/security/__init__.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.387479 python-ndn-0.3a1.post4/src/ndn/security/keychain/
--rw-r--r--   0 cs217a     (501) staff       (20)      244 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post4/src/ndn/security/keychain/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1651 2020-09-25 17:28:38.000000 python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1378 2020-09-25 17:28:43.000000 python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain_digest.py
--rw-r--r--   0 cs217a     (501) staff       (20)    17273 2020-09-25 17:28:47.000000 python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain_sqlite3.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.391054 python-ndn-0.3a1.post4/src/ndn/security/signer/
--rw-r--r--   0 cs217a     (501) staff       (20)      311 2019-10-25 06:53:37.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1390 2020-09-25 17:28:54.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_digest_signer.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2306 2020-09-25 17:29:00.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_ecdsa_signer.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1704 2020-09-25 17:29:03.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_hmac_signer.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1892 2020-09-25 17:29:06.000000 python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_rsa_signer.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.394426 python-ndn-0.3a1.post4/src/ndn/security/tpm/
--rw-r--r--   0 cs217a     (501) staff       (20)       82 2019-10-23 22:58:35.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2376 2020-09-25 17:29:14.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm.py
--rw-r--r--   0 cs217a     (501) staff       (20)    11547 2021-07-05 05:03:42.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_cng.py
--rw-r--r--   0 cs217a     (501) staff       (20)     3760 2020-09-25 17:29:18.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_file.py
--rw-r--r--   0 cs217a     (501) staff       (20)     9692 2021-07-05 05:03:42.000000 python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_osx_keychain.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.396138 python-ndn-0.3a1.post4/src/ndn/security/validator/
--rw-r--r--   0 cs217a     (501) staff       (20)      394 2021-05-29 08:45:36.000000 python-ndn-0.3a1.post4/src/ndn/security/validator/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2341 2020-09-25 17:29:27.000000 python-ndn-0.3a1.post4/src/ndn/security/validator/digest_validator.py
--rw-r--r--   0 cs217a     (501) staff       (20)     3248 2021-05-29 08:56:19.000000 python-ndn-0.3a1.post4/src/ndn/security/validator/known_key_validator.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.397595 python-ndn-0.3a1.post4/src/ndn/transport/
--rw-r--r--   0 cs217a     (501) staff       (20)        0 2019-09-26 07:09:13.000000 python-ndn-0.3a1.post4/src/ndn/transport/__init__.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2413 2020-09-25 17:29:38.000000 python-ndn-0.3a1.post4/src/ndn/transport/dummy_face.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2981 2021-07-05 05:00:49.000000 python-ndn-0.3a1.post4/src/ndn/transport/stream_socket.py
--rw-r--r--   0 cs217a     (501) staff       (20)     2667 2021-03-23 10:53:39.000000 python-ndn-0.3a1.post4/src/ndn/types.py
--rw-r--r--   0 cs217a     (501) staff       (20)     1307 2020-09-25 17:30:01.000000 python-ndn-0.3a1.post4/src/ndn/utils.py
-drwxr-xr-x   0 cs217a     (501) staff       (20)        0 2021-07-05 20:24:33.399727 python-ndn-0.3a1.post4/src/python_ndn.egg-info/
--rw-r--r--   0 cs217a     (501) staff       (20)     3971 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/PKG-INFO
--rw-r--r--   0 cs217a     (501) staff       (20)     2349 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/SOURCES.txt
--rw-r--r--   0 cs217a     (501) staff       (20)        1 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/dependency_links.txt
--rw-r--r--   0 cs217a     (501) staff       (20)       79 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/entry_points.txt
--rw-r--r--   0 cs217a     (501) staff       (20)      116 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/requires.txt
--rw-r--r--   0 cs217a     (501) staff       (20)        4 2021-07-05 20:24:33.000000 python-ndn-0.3a1.post4/src/python_ndn.egg-info/top_level.txt
+-rw-r--r--   0        0        0     2955 2023-07-10 08:50:03.554385 python_ndn-0.4/CHANGELOG.rst
+-rw-r--r--   0        0        0      993 2023-07-10 08:50:03.554121 python_ndn-0.4/README.rst
+-rw-r--r--   0        0        0     2192 2023-07-22 00:46:13.687486 python_ndn-0.4/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-07-22 00:46:13.688673 python_ndn-0.4/src/ndn/__init__.py
+-rw-r--r--   0        0        0    24473 2023-07-10 08:50:05.505075 python_ndn-0.4/src/ndn/app.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:50:05.506803 python_ndn-0.4/src/ndn/app_support/__init__.py
+-rw-r--r--   0        0        0     2419 2023-07-10 08:50:05.506064 python_ndn-0.4/src/ndn/app_support/dispatcher.py
+-rw-r--r--   0        0        0     2552 2023-07-10 08:50:05.550795 python_ndn-0.4/src/ndn/app_support/keychain_register.py
+-rw-r--r--   0        0        0      204 2023-07-10 08:50:05.508336 python_ndn-0.4/src/ndn/app_support/light_versec/__init__.py
+-rw-r--r--   0        0        0     3757 2023-07-10 08:50:05.507778 python_ndn-0.4/src/ndn/app_support/light_versec/binary.py
+-rw-r--r--   0        0        0    13047 2023-07-10 08:50:05.529322 python_ndn-0.4/src/ndn/app_support/light_versec/checker.py
+-rw-r--r--   0        0        0    14856 2023-07-10 08:50:05.508067 python_ndn-0.4/src/ndn/app_support/light_versec/compiler.py
+-rw-r--r--   0        0        0     2025 2023-07-10 08:50:05.528816 python_ndn-0.4/src/ndn/app_support/light_versec/grammar.py
+-rw-r--r--   0        0        0     3531 2023-07-10 08:50:05.529055 python_ndn-0.4/src/ndn/app_support/light_versec/parser.py
+-rw-r--r--   0        0        0     2607 2023-07-10 08:50:05.507403 python_ndn-0.4/src/ndn/app_support/light_versec/validator.py
+-rw-r--r--   0        0        0     9405 2023-07-10 08:50:05.506609 python_ndn-0.4/src/ndn/app_support/nfd_mgmt.py
+-rw-r--r--   0        0        0     5473 2023-07-10 08:50:05.550529 python_ndn-0.4/src/ndn/app_support/security_v2.py
+-rw-r--r--   0        0        0     2637 2023-07-10 08:50:05.529546 python_ndn-0.4/src/ndn/app_support/segment_fetcher.py
+-rw-r--r--   0        0        0      111 2023-07-19 22:10:14.885876 python_ndn-0.4/src/ndn/app_support/svs/__init__.py
+-rw-r--r--   0        0        0     8713 2023-07-20 03:16:10.920599 python_ndn-0.4/src/ndn/app_support/svs/sync.py
+-rw-r--r--   0        0        0     1520 2023-07-19 22:11:17.960417 python_ndn-0.4/src/ndn/app_support/svs/tlv.py
+-rw-r--r--   0        0        0    31698 2023-07-20 03:09:29.230309 python_ndn-0.4/src/ndn/appv2.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:50:05.179183 python_ndn-0.4/src/ndn/bin/__init__.py
+-rw-r--r--   0        0        0     2086 2023-07-10 08:50:05.183054 python_ndn-0.4/src/ndn/bin/nfdc/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-10 08:50:05.184489 python_ndn-0.4/src/ndn/bin/nfdc/__main__.py
+-rw-r--r--   0        0        0     4489 2023-07-10 08:50:05.182388 python_ndn-0.4/src/ndn/bin/nfdc/cmd_get_face.py
+-rw-r--r--   0        0        0     2547 2023-07-10 08:50:05.184810 python_ndn-0.4/src/ndn/bin/nfdc/cmd_get_route.py
+-rw-r--r--   0        0        0     2773 2023-07-10 08:50:05.181888 python_ndn-0.4/src/ndn/bin/nfdc/cmd_get_status.py
+-rw-r--r--   0        0        0     1826 2023-07-10 08:50:05.182806 python_ndn-0.4/src/ndn/bin/nfdc/cmd_get_strategy.py
+-rw-r--r--   0        0        0     1793 2023-07-10 08:50:05.184030 python_ndn-0.4/src/ndn/bin/nfdc/cmd_new_face.py
+-rw-r--r--   0        0        0     1813 2023-07-10 08:50:05.184240 python_ndn-0.4/src/ndn/bin/nfdc/cmd_new_route.py
+-rw-r--r--   0        0        0     3143 2023-07-10 08:50:05.182599 python_ndn-0.4/src/ndn/bin/nfdc/cmd_remove_face.py
+-rw-r--r--   0        0        0     1978 2023-07-10 08:50:05.183774 python_ndn-0.4/src/ndn/bin/nfdc/cmd_remove_route.py
+-rw-r--r--   0        0        0     1676 2023-07-10 08:50:05.182118 python_ndn-0.4/src/ndn/bin/nfdc/cmd_remove_strategy.py
+-rw-r--r--   0        0        0     2383 2023-07-10 08:50:05.183472 python_ndn-0.4/src/ndn/bin/nfdc/cmd_set_strategy.py
+-rw-r--r--   0        0        0     1583 2023-07-10 08:50:05.183259 python_ndn-0.4/src/ndn/bin/nfdc/utils.py
+-rw-r--r--   0        0        0     3256 2023-07-10 08:50:05.163272 python_ndn-0.4/src/ndn/bin/sec/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-10 08:50:05.178263 python_ndn-0.4/src/ndn/bin/sec/__main__.py
+-rw-r--r--   0        0        0     1505 2023-07-10 08:50:05.179030 python_ndn-0.4/src/ndn/bin/sec/cmd_export_cert.py
+-rw-r--r--   0        0        0     4404 2023-07-10 08:50:05.178507 python_ndn-0.4/src/ndn/bin/sec/cmd_get_childitem.py
+-rw-r--r--   0        0        0     2732 2023-07-10 08:50:05.177185 python_ndn-0.4/src/ndn/bin/sec/cmd_get_default.py
+-rw-r--r--   0        0        0     2209 2023-07-10 08:50:05.163027 python_ndn-0.4/src/ndn/bin/sec/cmd_get_signreq.py
+-rw-r--r--   0        0        0     2181 2023-07-10 08:50:05.177504 python_ndn-0.4/src/ndn/bin/sec/cmd_import_cert.py
+-rw-r--r--   0        0        0     2218 2023-07-10 08:50:05.177976 python_ndn-0.4/src/ndn/bin/sec/cmd_init_pib.py
+-rw-r--r--   0        0        0     2735 2023-07-10 08:50:05.177748 python_ndn-0.4/src/ndn/bin/sec/cmd_new_item.py
+-rw-r--r--   0        0        0     1670 2023-07-10 08:50:05.162795 python_ndn-0.4/src/ndn/bin/sec/cmd_remove_item.py
+-rw-r--r--   0        0        0     2032 2023-07-10 08:50:05.178735 python_ndn-0.4/src/ndn/bin/sec/cmd_set_default.py
+-rw-r--r--   0        0        0     4697 2023-07-10 08:50:05.176957 python_ndn-0.4/src/ndn/bin/sec/cmd_sign_cert.py
+-rw-r--r--   0        0        0     3846 2023-07-10 08:50:05.176671 python_ndn-0.4/src/ndn/bin/sec/utils.py
+-rw-r--r--   0        0        0     1650 2023-07-10 08:50:05.160425 python_ndn-0.4/src/ndn/bin/tools/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-10 08:50:05.162289 python_ndn-0.4/src/ndn/bin/tools/__main__.py
+-rw-r--r--   0        0        0     3992 2023-07-10 08:50:05.161373 python_ndn-0.4/src/ndn/bin/tools/cmd_fetch_data.py
+-rw-r--r--   0        0        0     5505 2023-07-10 08:50:05.161610 python_ndn-0.4/src/ndn/bin/tools/cmd_fetch_rdrcontent.py
+-rw-r--r--   0        0        0     3123 2023-07-10 08:50:05.161828 python_ndn-0.4/src/ndn/bin/tools/cmd_serve_data.py
+-rw-r--r--   0        0        0     3991 2023-07-10 08:50:05.162059 python_ndn-0.4/src/ndn/bin/tools/cmd_serve_rdrcontent.py
+-rw-r--r--   0        0        0     4359 2023-07-10 08:50:05.505389 python_ndn-0.4/src/ndn/client_conf.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:50:05.466460 python_ndn-0.4/src/ndn/contrib/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-10 08:50:05.475398 python_ndn-0.4/src/ndn/contrib/boost_info/__init__.py
+-rw-r--r--   0        0        0     4376 2023-07-10 08:50:05.480808 python_ndn-0.4/src/ndn/contrib/boost_info/parser.py
+-rw-r--r--   0        0        0     1545 2023-07-10 08:50:05.437050 python_ndn-0.4/src/ndn/contrib/cocoapy/LICENSE
+-rw-r--r--   0        0        0     1742 2023-07-10 08:50:05.437862 python_ndn-0.4/src/ndn/contrib/cocoapy/__init__.py
+-rw-r--r--   0        0        0    13048 2023-07-10 08:50:05.437460 python_ndn-0.4/src/ndn/contrib/cocoapy/cocoalibs.py
+-rw-r--r--   0        0        0     2629 2023-07-10 08:50:05.466259 python_ndn-0.4/src/ndn/contrib/cocoapy/cocoatypes.py
+-rw-r--r--   0        0        0    51669 2023-07-10 08:50:05.465985 python_ndn-0.4/src/ndn/contrib/cocoapy/runtime.py
+-rw-r--r--   0        0        0      415 2023-07-10 08:50:05.318553 python_ndn-0.4/src/ndn/encoding/__init__.py
+-rw-r--r--   0        0        0    11959 2023-07-10 08:50:05.389853 python_ndn-0.4/src/ndn/encoding/name/Component.py
+-rw-r--r--   0        0        0     7581 2023-07-10 08:50:05.389573 python_ndn-0.4/src/ndn/encoding/name/Name.py
+-rw-r--r--   0        0        0       32 2023-07-10 08:50:05.372309 python_ndn-0.4/src/ndn/encoding/name/__init__.py
+-rw-r--r--   0        0        0    19369 2023-07-10 08:50:05.318329 python_ndn-0.4/src/ndn/encoding/ndn_format_0_3.py
+-rw-r--r--   0        0        0    19733 2023-07-10 08:50:05.371084 python_ndn-0.4/src/ndn/encoding/ndn_format_0_3_2017.py
+-rw-r--r--   0        0        0     4542 2023-07-10 08:50:05.390554 python_ndn-0.4/src/ndn/encoding/ndnlp_v2.py
+-rw-r--r--   0        0        0     1975 2023-07-10 08:50:05.390266 python_ndn-0.4/src/ndn/encoding/signer.py
+-rw-r--r--   0        0        0    40835 2023-07-18 20:27:44.076488 python_ndn-0.4/src/ndn/encoding/tlv_model.py
+-rw-r--r--   0        0        0     1863 2023-07-10 08:50:05.317508 python_ndn-0.4/src/ndn/encoding/tlv_type.py
+-rw-r--r--   0        0        0     5007 2023-07-10 08:50:05.371671 python_ndn-0.4/src/ndn/encoding/tlv_var.py
+-rw-r--r--   0        0        0     3325 2023-07-10 08:50:05.551121 python_ndn-0.4/src/ndn/name_tree.py
+-rw-r--r--   0        0        0       69 2023-07-10 08:50:05.307485 python_ndn-0.4/src/ndn/platform/__init__.py
+-rw-r--r--   0        0        0     2100 2023-07-10 08:50:05.316774 python_ndn-0.4/src/ndn/platform/general.py
+-rw-r--r--   0        0        0     1591 2023-07-10 08:50:05.316340 python_ndn-0.4/src/ndn/platform/linux.py
+-rw-r--r--   0        0        0     5480 2023-07-10 08:50:05.316556 python_ndn-0.4/src/ndn/platform/osx.py
+-rw-r--r--   0        0        0     6856 2023-07-10 08:50:05.316097 python_ndn-0.4/src/ndn/platform/windows.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:50:05.482665 python_ndn-0.4/src/ndn/schema/__init__.py
+-rw-r--r--   0        0        0     3868 2023-07-10 08:50:05.482488 python_ndn-0.4/src/ndn/schema/policy.py
+-rw-r--r--   0        0        0    25245 2023-07-10 08:50:05.482228 python_ndn-0.4/src/ndn/schema/schema_tree.py
+-rw-r--r--   0        0        0     2509 2023-07-10 08:50:05.504473 python_ndn-0.4/src/ndn/schema/simple_cache.py
+-rw-r--r--   0        0        0     7378 2023-07-10 08:50:05.481681 python_ndn-0.4/src/ndn/schema/simple_node.py
+-rw-r--r--   0        0        0     5780 2023-07-10 08:50:05.481415 python_ndn-0.4/src/ndn/schema/simple_trust.py
+-rw-r--r--   0        0        0     2839 2023-07-10 08:50:05.481957 python_ndn-0.4/src/ndn/schema/util.py
+-rw-r--r--   0        0        0      231 2023-07-10 08:50:05.273651 python_ndn-0.4/src/ndn/security/__init__.py
+-rw-r--r--   0        0        0      365 2023-07-10 08:50:05.279726 python_ndn-0.4/src/ndn/security/keychain/__init__.py
+-rw-r--r--   0        0        0     3227 2023-07-10 08:50:05.306401 python_ndn-0.4/src/ndn/security/keychain/keychain.py
+-rw-r--r--   0        0        0     1378 2023-07-10 08:50:05.306639 python_ndn-0.4/src/ndn/security/keychain/keychain_digest.py
+-rw-r--r--   0        0        0    23951 2023-07-10 08:50:05.306873 python_ndn-0.4/src/ndn/security/keychain/keychain_sqlite3.py
+-rw-r--r--   0        0        0      451 2023-07-10 08:50:05.186930 python_ndn-0.4/src/ndn/security/signer/__init__.py
+-rw-r--r--   0        0        0     1833 2023-07-10 08:50:05.222941 python_ndn-0.4/src/ndn/security/signer/ed25519_signer.py
+-rw-r--r--   0        0        0     1249 2023-07-10 08:50:05.186519 python_ndn-0.4/src/ndn/security/signer/null_signer.py
+-rw-r--r--   0        0        0     1699 2023-07-10 08:50:05.187337 python_ndn-0.4/src/ndn/security/signer/sha256_digest_signer.py
+-rw-r--r--   0        0        0     2346 2023-07-10 08:50:05.186075 python_ndn-0.4/src/ndn/security/signer/sha256_ecdsa_signer.py
+-rw-r--r--   0        0        0     1744 2023-07-10 08:50:05.222705 python_ndn-0.4/src/ndn/security/signer/sha256_hmac_signer.py
+-rw-r--r--   0        0        0     1932 2023-07-10 08:50:05.222489 python_ndn-0.4/src/ndn/security/signer/sha256_rsa_signer.py
+-rw-r--r--   0        0        0       82 2023-07-10 08:50:05.247384 python_ndn-0.4/src/ndn/security/tpm/__init__.py
+-rw-r--r--   0        0        0     2436 2023-07-10 08:50:05.272878 python_ndn-0.4/src/ndn/security/tpm/tpm.py
+-rw-r--r--   0        0        0    11724 2023-07-10 08:50:05.247003 python_ndn-0.4/src/ndn/security/tpm/tpm_cng.py
+-rw-r--r--   0        0        0     3905 2023-07-10 08:50:05.273401 python_ndn-0.4/src/ndn/security/tpm/tpm_file.py
+-rw-r--r--   0        0        0     9869 2023-07-10 08:50:05.273113 python_ndn-0.4/src/ndn/security/tpm/tpm_osx_keychain.py
+-rw-r--r--   0        0        0      473 2023-07-10 08:50:05.226690 python_ndn-0.4/src/ndn/security/validator/__init__.py
+-rw-r--r--   0        0        0     4836 2023-07-10 08:50:05.226218 python_ndn-0.4/src/ndn/security/validator/cascade_validator.py
+-rw-r--r--   0        0        0     2341 2023-07-10 08:50:05.246218 python_ndn-0.4/src/ndn/security/validator/digest_validator.py
+-rw-r--r--   0        0        0     4934 2023-07-10 08:50:05.226454 python_ndn-0.4/src/ndn/security/validator/known_key_validator.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:50:05.130789 python_ndn-0.4/src/ndn/transport/__init__.py
+-rw-r--r--   0        0        0     2453 2023-07-10 08:50:05.130183 python_ndn-0.4/src/ndn/transport/dummy_face.py
+-rw-r--r--   0        0        0     1452 2023-07-10 08:50:05.159717 python_ndn-0.4/src/ndn/transport/face.py
+-rw-r--r--   0        0        0     1309 2023-07-10 08:50:05.130388 python_ndn-0.4/src/ndn/transport/ip_face.py
+-rw-r--r--   0        0        0     7208 2023-07-10 08:50:05.158986 python_ndn-0.4/src/ndn/transport/ndn_dpdk.py
+-rw-r--r--   0        0        0     3834 2023-07-10 08:50:05.130653 python_ndn-0.4/src/ndn/transport/nfd_registerer.py
+-rw-r--r--   0        0        0     1173 2023-07-10 08:50:05.159232 python_ndn-0.4/src/ndn/transport/prefix_registerer.py
+-rw-r--r--   0        0        0     2628 2023-07-10 08:50:05.129974 python_ndn-0.4/src/ndn/transport/stream_face.py
+-rw-r--r--   0        0        0     2679 2023-07-10 08:50:05.159490 python_ndn-0.4/src/ndn/transport/udp_face.py
+-rw-r--r--   0        0        0     3964 2023-07-10 08:50:05.390854 python_ndn-0.4/src/ndn/types.py
+-rw-r--r--   0        0        0     1307 2023-07-10 08:50:05.504759 python_ndn-0.4/src/ndn/utils.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:50:03.371646 python_ndn-0.4/tests/__init__.py
+-rw-r--r--   0        0        0    14092 2023-07-10 08:50:03.423241 python_ndn-0.4/tests/encoding/name_test.py
+-rw-r--r--   0        0        0    19664 2023-07-10 08:50:03.423920 python_ndn-0.4/tests/encoding/ndn_format_0_3_test.py
+-rw-r--r--   0        0        0     2016 2023-07-10 08:50:03.373047 python_ndn-0.4/tests/encoding/ndnlp_v2_test.py
+-rw-r--r--   0        0        0     6921 2023-07-10 08:50:03.423656 python_ndn-0.4/tests/encoding/tlv_model_test.py
+-rw-r--r--   0        0        0     3779 2023-07-10 08:50:03.372201 python_ndn-0.4/tests/encoding/tlv_var_test.py
+-rw-r--r--   0        0        0     2848 2023-07-10 08:50:03.424147 python_ndn-0.4/tests/face_test.py
+-rw-r--r--   0        0        0    12293 2023-07-10 08:50:03.346660 python_ndn-0.4/tests/integration/app_test.py
+-rw-r--r--   0        0        0    12681 2023-07-10 08:50:03.347100 python_ndn-0.4/tests/integration/app_v2_test.py
+-rw-r--r--   0        0        0     3100 2023-07-10 08:50:03.371472 python_ndn-0.4/tests/integration/keychain_test.py
+-rw-r--r--   0        0        0     2565 2023-07-10 08:50:03.334652 python_ndn-0.4/tests/misc/boost_info_test.py
+-rw-r--r--   0        0        0    13905 2023-07-10 08:50:03.334402 python_ndn-0.4/tests/misc/light_versec_test.py
+-rw-r--r--   0        0        0    14359 2023-07-10 08:50:03.336245 python_ndn-0.4/tests/security/signer_test.py
+-rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 python_ndn-0.4/PKG-INFO
```

### Comparing `python-ndn-0.3a1.post4/README.rst` & `python_ndn-0.4/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 |Test Badge|
 |Code Size|
 |Release Badge|
 |Doc Badge|
 
 A Named Data Networking client library with AsyncIO support in Python 3.
 
-It supports Python >=3.7 and PyPy3 >=7.1.1.
+It supports Python >=3.10 and PyPy3.10 >=7.3.12.
 
 Please see our documentation_ if you have any issues.
 
 .. |Test Badge| image:: https://github.com/named-data/python-ndn/workflows/test/badge.svg
     :target: https://github.com/named-data/python-ndn
     :alt: Test Status
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/app.py` & `python_ndn-0.4/src/ndn/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import struct
 import logging
 import asyncio as aio
 from typing import Optional, Any, Awaitable, Coroutine, Tuple, List
 from .utils import gen_nonce
 from .encoding import BinaryStr, TypeNumber, LpTypeNumber, parse_interest, \
     parse_tl_num, parse_data, DecodeError, Name, NonStrictName, MetaInfo, \
-    make_data, InterestParam, make_interest, FormalName, SignaturePtrs, parse_lp_packet
-from .security import Keychain, sha256_digest_checker, params_sha256_checker
-from .transport.stream_socket import Face
+    make_data, InterestParam, make_interest, FormalName, SignaturePtrs, parse_lp_packet, Component
+from .security import Keychain, sha256_digest_checker, params_sha256_checker, NullSigner
+from .transport.face import Face
 from .app_support.nfd_mgmt import make_command, parse_response
 from .name_tree import NameTrie, InterestTreeNode, PrefixTreeNode
 from .types import NetworkError, InterestTimeout, Validator, Route, InterestCanceled, \
     InterestNack, ValidationFailure
 from .client_conf import read_client_conf, default_face, default_keychain
 
 
@@ -70,15 +70,16 @@
     async def _receive(self, typ: int, data: BinaryStr):
         """
         Pipeline when a packet is received.
 
         :param typ: the Type.
         :param data: the Value of the packet with TL.
         """
-        logging.debug('Packet received %s, %s' % (typ, bytes(data)))
+        # if logging.getLogger().isEnabledFor(logging.DEBUG):
+        #     logging.debug('Packet received %s, %s' % (typ, bytes(data)))
         if typ == LpTypeNumber.LP_PACKET:
             try:
                 nack_reason, fragment = parse_lp_packet(data, with_tl=True)
             except (DecodeError, TypeError, ValueError, struct.error):
                 logging.warning('Unable to decode received packet')
                 return
             data = fragment
@@ -88,32 +89,35 @@
 
         if nack_reason is not None:
             try:
                 name, _, _, _ = parse_interest(data, with_tl=True)
             except (DecodeError, TypeError, ValueError, struct.error):
                 logging.warning('Unable to decode the fragment of LpPacket')
                 return
-            logging.debug('NetworkNack received %s, reason=%s' % (Name.to_str(name), nack_reason))
+            if logging.getLogger().isEnabledFor(logging.DEBUG):
+                logging.debug('NetworkNack received %s, reason=%s' % (Name.to_str(name), nack_reason))
             self._on_nack(name, nack_reason)
         else:
             if typ == TypeNumber.INTEREST:
                 try:
                     name, param, app_param, sig = parse_interest(data, with_tl=True)
                 except (DecodeError, TypeError, ValueError, struct.error):
                     logging.warning('Unable to decode received packet')
                     return
-                logging.debug('Interest received %s' % Name.to_str(name))
+                if logging.getLogger().isEnabledFor(logging.DEBUG):
+                    logging.debug('Interest received %s' % Name.to_str(name))
                 await self._on_interest(name, param, app_param, sig, raw_packet=data)
             elif typ == TypeNumber.DATA:
                 try:
                     name, meta_info, content, sig = parse_data(data, with_tl=True)
                 except (DecodeError, TypeError, ValueError, struct.error):
                     logging.warning('Unable to decode received packet')
                     return
-                logging.debug('Data received %s' % Name.to_str(name))
+                if logging.getLogger().isEnabledFor(logging.DEBUG):
+                    logging.debug('Data received %s' % Name.to_str(name))
                 await self._on_data(name, meta_info, content, sig, raw_packet=data)
             else:
                 logging.warning('Unable to decode received packet')
 
     def put_raw_packet(self, data: BinaryStr):
         r"""
         Send a raw Data packet.
@@ -133,15 +137,17 @@
         :param name: the Name.
         :type name: :any:`NonStrictName`
         :param content: the Content.
         :type content: Optional[:any:`BinaryStr`]
         :param kwargs: :ref:`label-keyword-arguments`.
         :return: TLV encoded Data packet.
         """
-        if 'signer' in kwargs:
+        if kwargs.get('no_signature', False):
+            signer = NullSigner()
+        elif 'signer' in kwargs:
             signer = kwargs['signer']
         else:
             signer = self.keychain.get_signer(kwargs)
         if 'meta_info' in kwargs:
             meta_info = kwargs['meta_info']
         else:
             meta_info = MetaInfo.from_dict(kwargs)
@@ -219,39 +225,45 @@
                              interest_param: InterestParam,
                              raw_interest: BinaryStr,
                              validator: Optional[Validator] = None,
                              need_raw_packet: bool = False
                              ) -> Coroutine[Any, None, Tuple[FormalName, MetaInfo, Optional[BinaryStr]]]:
         final_name = Name.normalize(final_name)
         future = aio.get_running_loop().create_future()
-        node = self._int_tree.setdefault(final_name, InterestTreeNode())
-        node.append_interest(future, interest_param)
+        if Component.get_type(final_name[-1]) == Component.TYPE_IMPLICIT_SHA256:
+            node_name = final_name[:-1]
+            implicit_sha256 = Component.get_value(final_name[-1])
+        else:
+            node_name = final_name
+            implicit_sha256 = b''
+        node = self._int_tree.setdefault(node_name, InterestTreeNode())
+        node.append_interest(future, interest_param, implicit_sha256)
         self.face.send(raw_interest)
-        return self._wait_for_data(future, interest_param.lifetime, final_name, node, validator, need_raw_packet)
+        return self._wait_for_data(future, interest_param.lifetime, node_name, node, validator, need_raw_packet)
 
-    async def _wait_for_data(self, future: aio.Future, lifetime: int, name: FormalName,
+    async def _wait_for_data(self, future: aio.Future, lifetime: int, node_name: FormalName,
                              node: InterestTreeNode, validator: Validator, need_raw_packet: bool):
         lifetime = 100 if lifetime is None else lifetime
         try:
-            name, meta_info, content, sig, raw_packet = await aio.wait_for(future, timeout=lifetime/1000.0)
+            data_name, meta_info, content, sig, raw_packet = await aio.wait_for(future, timeout=lifetime/1000.0)
         except aio.TimeoutError:
             if node.timeout(future):
-                del self._int_tree[name]
+                del self._int_tree[node_name]
             raise InterestTimeout()
         except aio.CancelledError:
             raise InterestCanceled()
         if validator is None:
             validator = self.data_validator
-        if await validator(name, sig):
+        if await validator(data_name, sig):
             if need_raw_packet:
-                return name, meta_info, content, raw_packet
+                return data_name, meta_info, content, raw_packet
             else:
-                return name, meta_info, content
+                return data_name, meta_info, content
         else:
-            raise ValidationFailure(name, meta_info, content)
+            raise ValidationFailure(data_name, meta_info, content, sig)
 
     async def main_loop(self, after_start: Awaitable = None) -> bool:
         """
         The main loop of NDNApp.
 
         :param after_start: the coroutine to start after connection to NFD is established.
         :return: ``True`` if the connection is shutdown not by ``Ctrl+C``.
@@ -271,15 +283,15 @@
 
         try:
             await self.face.open()
         except (FileNotFoundError, ConnectionError, OSError, PermissionError):
             if after_start:
                 if isinstance(after_start, Coroutine):
                     after_start.close()
-                elif isinstance(after_start, aio.Task) or isinstance(after_start, aio.Future):
+                elif isinstance(after_start, (aio.Task, aio.Future)):
                     after_start.cancel()
             raise
         task = aio.create_task(starting_task())
         logging.debug('Connected to NFD node, start running...')
         try:
             await self.face.run()
             ret = True
@@ -356,14 +368,25 @@
             .. code-block:: python3
 
                 app = NDNApp()
 
                 @app.route('/example/rpc')
                 def on_interest(name: FormalName, param: InterestParam, app_param):
                     pass
+
+        .. note::
+            The route function must be a normal function instead of an ``async`` one.
+            This is on purpose, because an Interest is supposed to be replied ASAP,
+            even it cannot finish the request in time.
+            To provide some feedback, a better practice is replying with an Application NACK
+            (or some equivalent Data packet saying the operation cannot be finished in time).
+            If you want to use ``await`` in the handler, please use ``asyncio.create_task`` to create a new coroutine.
+
+        .. note::
+            Currently, python-ndn does not handle PIT Tokens.
         """
         name = Name.normalize(name)
 
         def decorator(func: Route):
             self._autoreg_routes.append((name, func, validator, need_raw_packet, need_sig_ptrs))
             if self.face.running:
                 aio.create_task(self.register(name, func, validator, need_raw_packet, need_sig_ptrs))
@@ -397,23 +420,25 @@
         name = Name.normalize(name)
         if func is not None:
             self.set_interest_filter(name, func, validator, need_raw_packet, need_sig_ptrs)
 
         # Fix the issue that NFD only allows one packet signed by a specific key for a timestamp number
         async with self._prefix_register_semaphore:
             try:
-                _, _, reply = await self.express_interest(make_command('rib', 'register', name=name), lifetime=1000)
+                _, _, reply = await self.express_interest(
+                    name=make_command('rib', 'register', self.face, name=name),
+                    lifetime=1000)
                 ret = parse_response(reply)
                 if ret['status_code'] != 200:
                     logging.error(f'Registration for {Name.to_str(name)} failed: '
-                                  f'{ret["status_code"]} {bytes(ret["status_text"]).decode()}')
+                                  f'{ret["status_code"]} {ret["status_text"]}')
                     return False
                 else:
                     logging.debug(f'Registration for {Name.to_str(name)} succeeded: '
-                                  f'{ret["status_code"]} {bytes(ret["status_text"]).decode()}')
+                                  f'{ret["status_code"]} {ret["status_text"]}')
                     return True
             except (InterestNack, InterestTimeout, InterestCanceled, ValidationFailure) as e:
                 logging.error(f'Registration for {Name.to_str(name)} failed: {e.__class__.__name__}')
                 return False
 
     async def unregister(self, name: NonStrictName) -> bool:
         """
@@ -421,15 +446,15 @@
 
         :param name: the Name prefix.
         :type name: :any:`NonStrictName`
         """
         name = Name.normalize(name)
         del self._prefix_tree[name]
         try:
-            await self.express_interest(make_command('rib', 'unregister', name=name), lifetime=1000)
+            await self.express_interest(make_command('rib', 'unregister', self.face, name=name), lifetime=1000)
             return True
         except (InterestNack, InterestTimeout, InterestCanceled, ValidationFailure):
             return False
 
     def set_interest_filter(self, name: NonStrictName, func: Route,
                             validator: Optional[Validator] = None, need_raw_packet: bool = False,
                             need_sig_ptrs: bool = False):
@@ -491,24 +516,28 @@
         if node.callback is None:
             logging.warning('No callback: %s' % name)
             return
         if app_param is not None or sig.signature_info is not None:
             if not await params_sha256_checker(name, sig):
                 logging.warning('Drop malformed Interest: %s' % name)
                 return
-        if sig.signature_info is not None:
-            validator = node.validator if node.validator else self.int_validator
-            valid = await validator(name, sig)
-        else:
-            valid = True
-        if not valid:
-            logging.warning('Drop unvalidated Interest: %s' % name)
-            return
-        if node.extra_param:
-            kwargs = {}
-            if node.extra_param.get('raw_packet', False):
-                kwargs['raw_packet'] = raw_packet
-            if node.extra_param.get('sig_ptrs', False):
-                kwargs['sig_ptrs'] = sig
-            node.callback(name, param, app_param, **kwargs)
-        else:
-            node.callback(name, param, app_param)
+
+        # In case the validator blocks the pipeline, create a task
+        async def submit_interest():
+            if sig.signature_info is not None:
+                validator = node.validator if node.validator else self.int_validator
+                valid = await validator(name, sig)
+            else:
+                valid = True
+            if not valid:
+                logging.warning('Drop unvalidated Interest: %s' % name)
+                return
+            if node.extra_param:
+                kwargs = {}
+                if node.extra_param.get('raw_packet', False):
+                    kwargs['raw_packet'] = raw_packet
+                if node.extra_param.get('sig_ptrs', False):
+                    kwargs['sig_ptrs'] = sig
+                node.callback(name, param, app_param, **kwargs)
+            else:
+                node.callback(name, param, app_param)
+        aio.create_task(submit_interest())
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/app_support/dispatcher.py` & `python_ndn-0.4/src/ndn/app_support/dispatcher.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/app_support/security_v2.py` & `python_ndn-0.4/src/ndn/app_support/security_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     SignatureInfo, TypeNumber, RepeatedField, IncludeBase, MetaInfo, VarBinaryStr,\
     get_tl_num_size, write_tl_num, parse_and_check_tl, FormalName
 from ..encoding.ndn_format_0_3 import DataPacketValue
 
 
 KEY_COMPONENT = Component.from_str('KEY')
 SELF_COMPONENT = Component.from_str('self')
+SIGN_REQ_COMPONENT = Component.from_str('cert-request')
 
 
 class SecurityV2TypeNumber:
     VALIDITY_PERIOD = 0xFD
     NOT_BEFORE = 0xFE
     NOT_AFTER = 0xFF
     ADDITIONAL_DESCRIPTION = 0x0102
@@ -108,17 +109,24 @@
     write_tl_num(len(value) - shrink_size, buf, type_len)
     buf[type_len + size_len:] = memoryview(value)[0:len(value) - shrink_size]
     return cert_name, buf
 
 
 def self_sign(key_name, pub_key, signer) -> Tuple[FormalName, VarBinaryStr]:
     end_time = datetime.utcnow()
-    end_time.replace(year=end_time.year + 20)
+    end_time = end_time.replace(year=end_time.year + 20)
     return new_cert(key_name, SELF_COMPONENT, pub_key, signer,
                     datetime.fromisoformat('1970-01-01T00:00:00'), end_time)
 
 
-def derive_cert(key_name, issuer_id, pub_key, signer, start_time, expire_sec):
+def sign_req(key_name, pub_key, signer) -> Tuple[FormalName, VarBinaryStr]:
+    start_time = datetime.utcnow()
+    end_time = start_time + timedelta(days=10)
+    return new_cert(key_name, SIGN_REQ_COMPONENT, pub_key, signer,
+                    datetime.utcnow(), end_time)
+
+
+def derive_cert(key_name, issuer_id, pub_key, signer, start_time, expire_sec) -> Tuple[FormalName, VarBinaryStr]:
     end_time = start_time + timedelta(seconds=expire_sec)
     if isinstance(issuer_id, str):
         issuer_id = Component.from_str(issuer_id)
     return new_cert(key_name, issuer_id, pub_key, signer, start_time, end_time)
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/app_support/segment_fetcher.py` & `python_ndn-0.4/src/ndn/app_support/segment_fetcher.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/client_conf.py` & `python_ndn-0.4/src/ndn/client_conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import os
 import sys
 from configparser import ConfigParser
+from urllib.parse import urlparse
 from .platform import Platform
 from .security import TpmFile, Keychain, KeychainSqlite3
-from .transport.stream_socket import Face, UnixFace, TcpFace
+from .transport.face import Face
+from .transport.stream_face import UnixFace, TcpFace
+from .transport.udp_face import UdpFace
+from .transport.prefix_registerer import PrefixRegisterer
+from .transport.nfd_registerer import NfdRegister
 if sys.platform == 'darwin':
     from .security.tpm.tpm_osx_keychain import TpmOsxKeychain
 if sys.platform == 'win32':
     from .security.tpm.tpm_cng import TpmCng
 
 
 def read_client_conf():
@@ -36,38 +41,38 @@
                 return p
         return ''
 
     def resolve_location(item: str, value: str) -> str:
         nonlocal path
         sp = value.split(':')
         if len(sp) == 1:
-            schema = value
+            scheme = value
             loc = ''
         else:
-            schema, loc = sp
+            scheme, loc = sp
         if not loc or not os.path.exists(loc):
             if loc and (path is not None):
                 loc = os.path.join(os.path.dirname(path), loc)
             if not loc or not os.path.exists(loc):
                 if item == 'pib':
                     paths = Platform().default_pib_paths()
                 else:
                     paths = Platform().default_tpm_paths()
                 for p_str in paths:
                     p = os.path.expandvars(p_str)
                     if os.path.exists(p):
                         loc = p
                         break
-        return ':'.join((schema, loc))
+        return ':'.join((scheme, loc))
 
     path = get_path()
     ret = {
         'transport': Platform().default_transport(),
-        'pib': Platform().default_pib_schema(),
-        'tpm': Platform().default_tpm_schema()
+        'pib': Platform().default_pib_scheme(),
+        'tpm': Platform().default_tpm_scheme()
     }
     if path:
         parser = ConfigParser()
         text = '[DEFAULT]\n'
         with open(path) as f:
             text += f.read()
         parser.read_string(text)
@@ -83,38 +88,42 @@
             pass
     for key in ['pib', 'tpm']:
         ret[key] = resolve_location(key, ret[key])
     return ret
 
 
 def default_keychain(pib: str, tpm: str) -> Keychain:
-    pib_schema, pib_loc = pib.split(':', 1)
-    tpm_schema, tpm_loc = tpm.split(':', 1)
-    if tpm_schema == 'tpm-file':
+    pib_scheme, pib_loc = pib.split(':', 1)
+    tpm_scheme, tpm_loc = tpm.split(':', 1)
+    if tpm_scheme == 'tpm-file':
         tpm = TpmFile(tpm_loc)
-    elif tpm_schema == 'tpm-osxkeychain':
+    elif tpm_scheme == 'tpm-osxkeychain':
         tpm = TpmOsxKeychain()
-    elif tpm_schema == 'tpm-cng':
+    elif tpm_scheme == 'tpm-cng':
         tpm = TpmCng()
     else:
-        raise ValueError(f'Unrecognized tpm schema: {tpm}')
-    if pib_schema == 'pib-sqlite3':
+        raise ValueError(f'Unrecognized tpm scheme: {tpm}')
+    if pib_scheme == 'pib-sqlite3':
         pib = KeychainSqlite3(os.path.join(pib_loc, 'pib.db'), tpm)
     else:
-        raise ValueError(f'Unrecognized pib schema: {pib}')
+        raise ValueError(f'Unrecognized pib scheme: {pib}')
     return pib
 
 
 def default_face(face: str) -> Face:
-    schema, uri = face.split('://')
-    if schema == 'unix':
-        return UnixFace(uri)
-    elif schema == 'tcp' or schema == 'tcp4':
-        if uri.find(':') >= 0:
-            host, port = uri.split(':')
-            port = port
-        else:
-            host = uri
-            port = 6363
-        return TcpFace(host, int(port))
+    url = urlparse(face)
+    scheme = url.scheme
+    if scheme == 'unix':
+        return UnixFace(url.path)
+    host, port = url.hostname, url.port
+    if not port:
+        port = 6363
+    if scheme == 'tcp' or scheme == 'tcp4' or scheme == 'tcp6':
+        return TcpFace(host, port)
+    elif scheme == 'udp' or scheme == 'udp4' or scheme == 'udp6':
+        return UdpFace(host, int(port))
     else:
         raise ValueError(f'Unrecognized face: {face}')
+
+
+def default_registerer() -> PrefixRegisterer:
+    return NfdRegister()
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/__init__.py` & `python_ndn-0.4/src/ndn/contrib/cocoapy/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/cocoalibs.py` & `python_ndn-0.4/src/ndn/contrib/cocoapy/cocoalibs.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/cocoatypes.py` & `python_ndn-0.4/src/ndn/contrib/cocoapy/cocoatypes.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/contrib/cocoapy/runtime.py` & `python_ndn-0.4/src/ndn/contrib/cocoapy/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from ctypes import *
 from ctypes import util
 
 from .cocoatypes import *
 
 __LP64__ = (8*struct.calcsize("P") == 64)
 __i386__ = (platform.machine() == 'i386')
+__arm64__ = (platform.machine() == 'arm64')
 
 if sizeof(c_void_p) == 4:
     c_ptrdiff_t = c_int32
 elif sizeof(c_void_p) == 8:
     c_ptrdiff_t = c_int64
 
 ######################################################################
@@ -125,17 +126,19 @@
 objc.class_getIvarLayout.restype = c_char_p
 objc.class_getIvarLayout.argtypes = [c_void_p]
 
 # IMP class_getMethodImplementation(Class cls, SEL name)
 objc.class_getMethodImplementation.restype = c_void_p
 objc.class_getMethodImplementation.argtypes = [c_void_p, c_void_p]
 
-# IMP class_getMethodImplementation_stret(Class cls, SEL name)
-objc.class_getMethodImplementation_stret.restype = c_void_p
-objc.class_getMethodImplementation_stret.argtypes = [c_void_p, c_void_p]
+if not __arm64__:
+    # marked as OBJC_ARM64_UNAVAILABLE
+    # IMP class_getMethodImplementation_stret(Class cls, SEL name)
+    objc.class_getMethodImplementation_stret.restype = c_void_p
+    objc.class_getMethodImplementation_stret.argtypes = [c_void_p, c_void_p]
 
 # const char * class_getName(Class cls)
 objc.class_getName.restype = c_char_p
 objc.class_getName.argtypes = [c_void_p]
 
 # objc_property_t class_getProperty(Class cls, const char *name)
 objc.class_getProperty.restype = c_void_p
@@ -274,22 +277,28 @@
 objc.objc_getProtocol.restype = c_void_p
 objc.objc_getProtocol.argtypes = [c_char_p]
 
 # You should set return and argument types depending on context.
 # id objc_msgSend(id theReceiver, SEL theSelector, ...)
 # id objc_msgSendSuper(struct objc_super *super, SEL op,  ...)
 
-# void objc_msgSendSuper_stret(struct objc_super *super, SEL op, ...)
-objc.objc_msgSendSuper_stret.restype = None
-
-# double objc_msgSend_fpret(id self, SEL op, ...)
-# objc.objc_msgSend_fpret.restype = c_double
-
-# void objc_msgSend_stret(void * stretAddr, id theReceiver, SEL theSelector,  ...)
-objc.objc_msgSend_stret.restype = None
+if not __arm64__:
+    # marked as OBJC_ARM64_UNAVAILABLE
+    # void objc_msgSendSuper_stret(struct objc_super *super, SEL op, ...)
+    objc.objc_msgSendSuper_stret.restype = None
+
+if not __arm64__:
+    # marked as OBJC_ARM64_UNAVAILABLE
+    # double objc_msgSend_fpret(id self, SEL op, ...)
+    objc.objc_msgSend_fpret.restype = c_double
+
+if not __arm64__:
+    # marked as OBJC_ARM64_UNAVAILABLE
+    # void objc_msgSend_stret(void * stretAddr, id theReceiver, SEL theSelector,  ...)
+    objc.objc_msgSend_stret.restype = None
 
 # void objc_registerClassPair(Class cls)
 objc.objc_registerClassPair.restype = None
 objc.objc_registerClassPair.argtypes = [c_void_p]
 
 # void objc_removeAssociatedObjects(id object)
 objc.objc_removeAssociatedObjects.restype = None
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/encoding/name/Component.py` & `python_ndn-0.4/src/ndn/encoding/name/Component.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,19 +50,19 @@
 """The character set for NameComponent, which is unreserved characters + {'=', '%'}"""
 
 TYPE_INVALID = 0x00
 TYPE_GENERIC = 0x08
 TYPE_IMPLICIT_SHA256 = 0x01
 TYPE_PARAMETERS_SHA256 = 0x02
 TYPE_KEYWORD = 0x20
-TYPE_SEGMENT = 0x21
-TYPE_BYTE_OFFSET = 0x22
-TYPE_VERSION = 0x23
-TYPE_TIMESTAMP = 0x24
-TYPE_SEQUENCE_NUM = 0x25
+TYPE_SEGMENT = 0x32
+TYPE_BYTE_OFFSET = 0x34
+TYPE_VERSION = 0x36
+TYPE_TIMESTAMP = 0x38
+TYPE_SEQUENCE_NUM = 0x3A
 
 ALTERNATE_URI_TYPE = {
     TYPE_SEGMENT: 'seg={}',
     TYPE_BYTE_OFFSET: 'off={}',
     TYPE_VERSION: 'v={}',
     TYPE_TIMESTAMP: 't={}',
     TYPE_SEQUENCE_NUM: 'seq={}'
@@ -72,23 +72,27 @@
     'seg': TYPE_SEGMENT,
     'off': TYPE_BYTE_OFFSET,
     'v': TYPE_VERSION,
     't': TYPE_TIMESTAMP,
     'seq': TYPE_SEQUENCE_NUM,
 }
 
+MAX_COMPONENT_TYPE_VALUE = 65535
+
 
 def from_bytes(val: BinaryStr, typ: int = TYPE_GENERIC) -> bytearray:
     """
     Construct a Component from bytes by adding a type and length.
 
     :param val: the value of the component.
     :param typ: the type of the component. :const:`TYPE_GENERIC` by default.
     :return: the component.
     """
+    if typ <= 0 or typ > MAX_COMPONENT_TYPE_VALUE:
+        raise ValueError(f'Type number {typ} not in range 0<T<=65535.')
     size_typ = get_tl_num_size(typ)
     size_len = get_tl_num_size(len(val))
     ret = bytearray(size_typ + size_len + len(val))
     write_tl_num(typ, ret, 0)
     write_tl_num(len(val), ret, size_typ)
     ret[size_typ+size_len:] = val
     return ret
@@ -115,32 +119,32 @@
         .. note::
             Additional periods are not allowed here. To create a zero-size Component, just pass
             an empty string ``''`` in.
 
     :return: the component.
     :raises ValueError: the string is not a legal URI.
     """
-    def raise_except():
-        raise ValueError(f'{val} is not a legal Name.')
+    def raise_except(explain=''):
+        raise ValueError(f'{val} is not a legal NameComponent: {explain}')
 
     # Check empty string
     if not val:
         return bytearray(b'\x08\x00')
 
     percent_cnt = 0
     type_offset = None
     # Check charset
     for i, ch in enumerate(val):
         if ch not in CHARSET:
-            raise_except()
+            raise_except(f'Unrecognized char {ch} for NameComponent.')
         if ch == '%':
             percent_cnt += 1
         if ch == "=":
             if type_offset is not None:
-                raise_except()
+                raise_except('Multiple TLV types are present.')
             else:
                 type_offset = i
     # Get Type
     typ = TYPE_GENERIC
     if type_offset is not None:
         try:
             typ_str = val[:type_offset]
@@ -150,23 +154,25 @@
             elif typ_str == 'params-sha256':
                 return from_bytes(bytearray.fromhex(val[type_offset + 1:]), TYPE_PARAMETERS_SHA256)
             elif typ_str in ALTERNATE_URI_STR:
                 return from_number(int(val[type_offset + 1:]), ALTERNATE_URI_STR[typ_str])
             # General case
             else:
                 typ = int(typ_str)
-        except ValueError:
-            raise_except()
+        except ValueError as e:
+            raise_except(f'Unable to parse Component type: {e}')
+        if typ <= 0 or typ > MAX_COMPONENT_TYPE_VALUE:
+            raise_except(f'Type number {typ} not in range 0<T<=65535.')
     else:
         typ = TYPE_GENERIC
         type_offset = -1
     # Alloc buf
     length = len(val) - type_offset - 1 - 2 * percent_cnt
     if length < 0:
-        raise_except()
+        raise_except('Too many %%%%% in the Component.')
     size_typ = get_tl_num_size(typ)
     size_len = get_tl_num_size(length)
     ret = bytearray(size_typ + size_len + length)
     view = memoryview(ret)
     write_tl_num(typ, ret, 0)
     write_tl_num(length, ret, size_typ)
 
@@ -182,16 +188,16 @@
             view[pos] = int(val[i+1:i+3], 16)
             return 3
 
     while i < len(val):
         try:
             i += encode()
             pos += 1
-        except IndexError:
-            raise_except()
+        except IndexError as e:
+            raise_except(repr(e))
     return ret
 
 
 def from_number(val: int, typ: int) -> bytearray:
     """
     Construct a Component from an integer.
 
@@ -312,14 +318,44 @@
                 return ret
             else:
                 return f"%{val:02X}"
 
         return ret + "".join(decode(val) for val in component[offset:])
 
 
+def to_canonical_uri(component: BinaryStr) -> str:
+    """
+    Convert a Component into a canonical URI string without naming conventions.
+    Returns an empty string ``''`` for a 0-size Component.
+
+    :param component: the component.
+    :return: a canonical URI string.
+    """
+    offset = 0
+    typ, sz = parse_tl_num(component, offset)
+    offset += sz
+    length, sz = parse_tl_num(component, offset)
+    offset += sz
+    if len(component) != length + offset:
+        raise ValueError(f'{component} is malformed.')
+
+    ret = ""
+    if typ != TYPE_GENERIC:
+        ret = f"{typ}="
+
+    def decode(val: int) -> str:
+        ret = chr(val)
+        if ret in CHARSET and ret not in {'%', '='}:
+            return ret
+        else:
+            return f"%{val:02X}"
+
+    return ret + "".join(decode(val) for val in component[offset:])
+
+
 def to_number(component: BinaryStr) -> int:
     """
     Take the number encoded in the component out.
 
     :param component: the component.
     :return: an integer, which is the value of the component.
     """
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/encoding/name/Name.py` & `python_ndn-0.4/src/ndn/encoding/name/Name.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,34 @@
     name = normalize(name)
     ret = '/' + '/'.join(Component.to_str(comp) for comp in name)
     if name and name[-1] == b'\x08\x00':
         ret += '/'
     return ret
 
 
+def to_canonical_uri(name: NonStrictName) -> str:
+    r"""
+    Convert an NDN Name to a canonical URI string without naming conventions.
+
+    :param name: the input NDN Name.
+    :type name: :any:`NonStrictName`
+    :return: the canonical URI.
+
+    :examples:
+        >>> from ndn.encoding.name import Name
+        >>> Name.to_canonical_uri('Σπυρίδων')
+        '/%CE%A3%CF%80%CF%85%CF%81%CE%AF%CE%B4%CF%89%CE%BD'
+    """
+    name = normalize(name)
+    ret = '/' + '/'.join(Component.to_canonical_uri(comp) for comp in name)
+    if name and name[-1] == b'\x08\x00':
+        ret += '/'
+    return ret
+
+
 def from_bytes(buf: BinaryStr) -> FormalName:
     r"""
     Decode the Name from its TLV encoded form.
 
     :param buf: encoded Name.
     :return: Decoded Name.
     :rtype: :any:`FormalName`
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/encoding/ndn_format_0_3.py` & `python_ndn-0.4/src/ndn/encoding/ndn_format_0_3_2017.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,29 +95,31 @@
     NACK = 3
 
 
 class SignatureType:
     r"""
     Numbers used in SignatureType.
 
-    =================   ==============================================
+    =================   ==================================================
     Type                Description
-    =================   ==============================================
+    =================   ==================================================
     NOT_SIGNED          Not signed
     DIGEST_SHA256       SHA-256 digest (only for integrity protection)
     SHA256_WITH_RSA     RSA signature over a SHA-256 digest
     SHA256_WITH_ECDSA   An ECDSA signature over a SHA-256 digest
     HMAC_WITH_SHA256    SHA256 hash-based message authentication codes
-    =================   ==============================================
+    NULL                An empty signature for testing and experimentation
+    =================   ==================================================
     """
     NOT_SIGNED = None
     DIGEST_SHA256 = 0
     SHA256_WITH_RSA = 1
     SHA256_WITH_ECDSA = 3
     HMAC_WITH_SHA256 = 4
+    NULL = 200
 
 
 class KeyLocator(TlvModel):
     name = NameField()
     key_digest = BytesField(TypeNumber.KEY_DIGEST)
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/encoding/ndnlp_v2.py` & `python_ndn-0.4/src/ndn/encoding/ndnlp_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,29 +16,30 @@
 # limitations under the License.
 # -----------------------------------------------------------------------------
 from typing import Optional
 from .tlv_type import BinaryStr, VarBinaryStr
 from .tlv_var import parse_and_check_tl
 from .tlv_model import TlvModel, UintField, BytesField, ModelField, BoolField, DecodeError
 
-__all__ = ['LpTypeNumber', 'NackReason', 'parse_network_nack', 'make_network_nack', 'parse_lp_packet']
+__all__ = ['LpTypeNumber', 'NackReason', 'parse_network_nack', 'make_network_nack', 'parse_lp_packet',
+           'parse_lp_packet_v2']
 
 
 class LpTypeNumber:
     FRAGMENT = 0x50
     SEQUENCE = 0x51
     FRAG_INDEX = 0x52
     FRAG_COUNT = 0x53
     HOP_COUNT = 0x54
     PIT_TOKEN = 0x62
     LP_PACKET = 0x64
     NACK = 0x0320
     NACK_REASON = 0x0321
+    INCOMING_FACE_ID = 0x032C
     NEXT_HOP_FACE_ID = 0x0330
-    INCOMING_FACE_ID = 0x0331
     CACHE_POLICY = 0x0334
     CACHE_POLICY_TYPE = 0x0335
     CONGESTION_MARK = 0x0340
     ACK = 0x0344
     TX_SEQUENCE = 0x0348
     NON_DISCOVERY = 0x034C
     PREFIX_ANNOUNCEMENT = 0x0350
@@ -60,16 +61,16 @@
 
 
 class LpPacketValue(TlvModel):
     frag_index = UintField(LpTypeNumber.FRAG_INDEX)
     frag_count = UintField(LpTypeNumber.FRAG_COUNT)
     pit_token = BytesField(LpTypeNumber.PIT_TOKEN)
     nack = ModelField(LpTypeNumber.NACK, NetworkNack)
-    next_hop_face_id = UintField(LpTypeNumber.NEXT_HOP_FACE_ID)
     incoming_face_id = UintField(LpTypeNumber.INCOMING_FACE_ID)
+    next_hop_face_id = UintField(LpTypeNumber.NEXT_HOP_FACE_ID)
     cache_policy = ModelField(LpTypeNumber.CACHE_POLICY, CachePolicy)
     congestion_mark = UintField(LpTypeNumber.CONGESTION_MARK)
     tx_sequence = BytesField(LpTypeNumber.TX_SEQUENCE)
     ack = BytesField(LpTypeNumber.ACK)
     non_discovery = BoolField(LpTypeNumber.NON_DISCOVERY)
     prefix_announcement = BytesField(LpTypeNumber.PREFIX_ANNOUNCEMENT)
 
@@ -84,26 +85,38 @@
     """
     Parse an LpPacket, return NackReason (if exists) and the fragment.
 
     :param wire: an LpPacket.
     :param with_tl: if `wire` has the TL fields.
     :return: a tuple of NackReason and Fragment.
     """
+    ret = parse_lp_packet_v2(wire, with_tl)
+    if ret.nack is not None:
+        return ret.nack.nack_reason, ret.fragment
+    else:
+        return None, ret.fragment
+
+
+def parse_lp_packet_v2(wire: BinaryStr, with_tl: bool = True) -> LpPacketValue:
+    """
+    Parse an LpPacket, return NackReason (if exists) and the fragment.
+
+    :param wire: an LpPacket.
+    :param with_tl: if `wire` has the TL fields.
+    :return: LpPacketValue.
+    """
     if with_tl:
         wire = parse_and_check_tl(wire, LpTypeNumber.LP_PACKET)
     markers = {}
     ret = LpPacketValue.parse(wire, markers, ignore_critical=True)
 
     if ret.frag_index is not None or ret.frag_count is not None:
         raise DecodeError('NDNLP fragmentation is not implemented yet.')
 
-    if ret.nack is not None:
-        return ret.nack.nack_reason, ret.fragment
-    else:
-        return None, ret.fragment
+    return ret
 
 
 def parse_network_nack(wire: BinaryStr, with_tl: bool = True) -> (Optional[int], Optional[BinaryStr]):
     if with_tl:
         wire = parse_and_check_tl(wire, LpTypeNumber.LP_PACKET)
     markers = {}
     ret = LpPacketValue.parse(wire, markers, ignore_critical=True)
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/encoding/signer.py` & `python_ndn-0.4/src/ndn/encoding/signer.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/encoding/tlv_model.py` & `python_ndn-0.4/src/ndn/encoding/tlv_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import abc
 import struct
+from enum import Enum, Flag
 from typing import Optional, Type, List, Iterable
 from functools import reduce
 from .tlv_type import BinaryStr, VarBinaryStr, is_binary_str
 from .tlv_var import write_tl_num, parse_tl_num, get_tl_num_size
 from .name import Name, Component
 
 
 __all__ = ['DecodeError', 'TlvModel', 'ProcedureArgument', 'OffsetMarker', 'UintField', 'BoolField',
-           'NameField', 'BytesField', 'ModelField', 'RepeatedField', 'IncludeBase', 'IncludeBaseError']
+           'NameField', 'BytesField', 'ModelField', 'RepeatedField', 'IncludeBase', 'IncludeBaseError',
+           'MapField']
 
 
 class DecodeError(Exception):
     """
     Raised when there is a critical field (Type is odd) that is unrecognized, redundant or out-of-order.
     """
     pass
@@ -282,43 +284,80 @@
     Type: :class:`int`
 
     Its Length is 1, 2, 4 or 8 when present.
 
     :ivar fixed_len: the fixed value for Length if it's not ``None``.
         Only 1, 2, 4 and 8 are acceptable.
     :vartype fixed_len: int
+    :ivar val_base_type: the base type of the value of the field.
+        Can be int (default), an Enum or a Flag type.
     """
-    def __init__(self, type_num: int, default=None, fixed_len: int = None):
+    def __init__(self, type_num: int, default=None, fixed_len: int = None,
+                 val_base_type=int):
         super().__init__(type_num, default)
         if fixed_len not in {None, 1, 2, 4, 8}:
             raise ValueError("Uint's length should be 1, 2, 4, 8 or None")
+        if not issubclass(val_base_type, (Flag, Enum, int)):
+            raise TypeError("Uint's base class should be int, an Enum, or a Flag")
         self.fixed_len = fixed_len
+        self.val_base_type = val_base_type
+
+    def __set__(self, instance, value):
+        """
+        Set the value of this uint field.
+        Will try to convert ``value`` into ``int``.
+
+        :param instance: the instance whose field is being set.
+        :param value: the new value.
+        """
+        if not isinstance(value, int) and value is not None:
+            if isinstance(value, (Flag, Enum)):
+                value = value.value
+            else:
+                raise TypeError(f"Cannot convert {value} into a uint field.")
+        instance.__dict__[self.name] = value
+
+    def __get__(self, instance, owner):
+        """
+        Get the value of this uint field in a specific instance.
+        Convert the value into the given ``val_base_type``.
+
+        :param instance: the instance that this field is being accessed through.
+        :param owner: the owner class of this field.
+        :return: the value of this field.
+        """
+        if instance is None:
+            return self
+        value = self.get_value(instance)
+        if value is not None:
+            return self.val_base_type(value)
+        else:
+            return None
 
     def encoded_length(self, val, markers: dict) -> int:
         if val is None:
             return 0
+        if not isinstance(val, int) or val < 0:
+            raise TypeError(f'{self.name}=f{val} is not a legal uint')
+        tl_size = get_tl_num_size(self.type_num) + 1
+        if self.fixed_len is not None:
+            ret = self.fixed_len
         else:
-            if not isinstance(val, int) or val < 0:
-                raise TypeError(f'{self.name}=f{val} is not a legal uint')
-            tl_size = get_tl_num_size(self.type_num) + 1
-            if self.fixed_len is not None:
-                ret = self.fixed_len
+            if val <= 0xFF:
+                ret = 1
+            elif val <= 0xFFFF:
+                ret = 2
+            elif val <= 0xFFFFFFFF:
+                ret = 4
             else:
-                if val <= 0xFF:
-                    ret = 1
-                elif val <= 0xFFFF:
-                    ret = 2
-                elif val <= 0xFFFFFFFF:
-                    ret = 4
-                else:
-                    ret = 8
-            if val >= 0x100 ** ret:
-                raise ValueError(f'{val} cannot be encoded into {ret} bytes')
-            markers[f'{self.name}##encoded_length'] = ret
-            return ret + tl_size
+                ret = 8
+        if val >= 0x100 ** ret:
+            raise ValueError(f'{val} cannot be encoded into {ret} bytes')
+        markers[f'{self.name}##encoded_length'] = ret
+        return ret + tl_size
 
     def encode_into(self, val, markers: dict, wire: VarBinaryStr, offset: int) -> int:
         if val is None:
             return 0
         tl_size = get_tl_num_size(self.type_num) + 1
         length = markers[f'{self.name}##encoded_length']
         offset += write_tl_num(self.type_num, wire, offset)
@@ -550,16 +589,16 @@
 
 class NameField(Field):
     """
     NDN Name field. Its Type is always :any:`Name.TYPE_NAME`.
 
     Type: :any:`NonStrictName`
     """
-    def __init__(self, default=None):
-        super().__init__(Name.TYPE_NAME, default)
+    def __init__(self, default=None, type_number=Name.TYPE_NAME):
+        super().__init__(type_number, default)
 
     def encoded_length(self, val, markers: dict) -> int:
         if val is None:
             return 0
         name = val
         if isinstance(name, str):
             name = Name.from_str(name)
@@ -599,49 +638,70 @@
 
 class BytesField(Field):
     r"""
     Field for ``*OCTET``.
 
     Type: :any:`BinaryStr`
 
+    :ivar is_string: If the value is a UTF-8 string. False by default.
+
     .. note::
-        Do not assign it with a :class:`str`.
+        Do not assign it with a :class:`str` if ``is_string`` is False.
     """
+    def __init__(self, type_num: int, default=None, is_string: bool = False):
+        super().__init__(type_num, default)
+        self.is_string = is_string
+
+    def __set__(self, instance, value):
+        instance.__dict__[self.name] = value
+
+    def __get__(self, instance, owner):
+        if instance is None:
+            return self
+        value = self.get_value(instance)
+        return value
+
     def encoded_length(self, val, markers: dict) -> int:
         if val is None:
             return 0
         tl_size = get_tl_num_size(self.type_num) + get_tl_num_size(len(val))
         return tl_size + len(val)
 
     def encode_into(self, val, markers: dict, wire: VarBinaryStr, offset: int) -> int:
         if val is None:
             return 0
         else:
+            if isinstance(val, str):
+                val = val.encode('utf-8')
             origin_offset = offset
             offset += write_tl_num(self.type_num, wire, offset)
             offset += write_tl_num(len(val), wire, offset)
             wire[offset:offset+len(val)] = val
             offset += len(val)
             return offset - origin_offset
 
     def parse_from(self, instance, markers: dict, wire: BinaryStr, offset: int, length: int, offset_btl: int):
-        return memoryview(wire)[offset:offset+length]
+        ret = memoryview(wire)[offset:offset+length]
+        if self.is_string:
+            return bytes(ret).decode('utf-8')
+        else:
+            return ret
 
 
 class TlvModel(metaclass=TlvModelMeta):
     r"""
     Used to describe a TLV format.
 
     :ivar _encoded_fields: a list of :any:`Field` in order.
     :vartype _encoded_fields: List[Field]
     """
     _encoded_fields: List[Field]
 
     def __repr__(self):
-        values = ', '.join(f'{field.name}={field.get_value(self).__repr__()}' for field in self._encoded_fields)
+        values = ', '.join(f'{field.name}={field.__get__(self, None).__repr__()}' for field in self._encoded_fields)
         return f'{self.__class__.__name__}({values})'
 
     def __eq__(self, other):
         """
         Compare two TlvModels
 
         :param other: the other TlvModel to compare with.
@@ -658,21 +718,28 @@
 
         :param dict_factory: class of dict.
         :return: the dict.
         """
         result = []
         for field in self._encoded_fields:
             if isinstance(field, ModelField):
-                result.append((field.name, field.get_value(self).asdict()))
+                result.append((field.name, field.__get__(self, None).asdict()))
             elif isinstance(field, RepeatedField):
                 result.append((field.name, field.aslist(self)))
+            elif isinstance(field, MapField):
+                result.append((field.name, field.asdict(self)))
             elif isinstance(field, BytesField):
-                result.append((field.name, bytes(field.get_value(self))))
+                val = field.__get__(self, None)
+                if isinstance(val, str):
+                    result.append((field.name, val))
+                else:
+                    # memoryview, bytearray, bytes
+                    result.append((field.name, bytes(val)))
             else:
-                result.append((field.name, field.get_value(self)))
+                result.append((field.name, field.__get__(self, None)))
         return dict_factory(result)
 
     def encoded_length(self, markers: Optional[dict] = None) -> int:
         """
         Get the encoded Length of this TlvModel.
 
         :param markers: encoding marker variables.
@@ -751,19 +818,33 @@
                 i += 1
             if i < len(ret._encoded_fields):
                 # If found
                 # First process skipped fields
                 for j in range(field_pos, i):
                     ret._encoded_fields[j].skipping_process(markers, wire, offset_btl)
                 # Parse that field
-                val = ret._encoded_fields[i].parse_from(ret, markers, wire, offset, length, offset_btl)
-                ret._encoded_fields[i].__set__(ret, val)
+                cur_field = ret._encoded_fields[i]
+                val = cur_field.parse_from(ret, markers, wire, offset, length, offset_btl)
+                cur_field.__set__(ret, val)
                 # Set next field
-                if isinstance(ret._encoded_fields[i], RepeatedField):
+                if isinstance(cur_field, RepeatedField):
+                    field_pos = i
+                elif isinstance(cur_field, MapField):
+                    # Parse the value part for a map
                     field_pos = i
+                    offset += length
+
+                    offset_btl = offset
+                    typ, size_typ = parse_tl_num(wire, offset)
+                    offset += size_typ
+                    length, size_len = parse_tl_num(wire, offset)
+                    offset += size_len
+
+                    val = cur_field.parse_value(ret, markers, wire, offset, length, offset_btl)
+                    cur_field.__set__(ret, val)
                 else:
                     field_pos = i + 1
             else:
                 # If not found
                 if (typ & 1) == 1 and not ignore_critical:
                     raise DecodeError(f'a critical field of type {typ} is unrecognized, redundant or out-of-order')
             offset += length
@@ -890,15 +971,99 @@
         self.element_type.name = f'{self.name}[{len(lst)}]'
         new_ele = self.element_type.parse_from(instance, markers, wire, offset, length, offset_btl)
         lst.append(new_ele)
         return lst
 
     def aslist(self, instance):
         ret = []
-        for x in self.get_value(instance):
+        for x in self.__get__(instance, None):
             if isinstance(x, TlvModel):
                 ret.append(x.asdict())
             elif isinstance(x, memoryview):
                 ret.append(bytes(x))
             else:
                 ret.append(x)
         return ret
+
+
+class MapField(Field):
+    r"""
+    Field for an unordered string or int map of a specific type.
+    All elements will be directly encoded into TLV wire in order, sharing the same Type.
+    The ``type_num`` of ``element_type`` is used.
+
+    Type: :class:`list`
+
+    :vartype value_type: :any:`Field`
+    :ivar value_type: the type of values in the dict.
+
+        .. warning::
+
+            Please always create a new :any:`Field` instance.
+            Don't use an existing one.
+    """
+
+    def __init__(self, key_type: Field, value_type: Field):
+        # default should be None here to prevent unintended modification
+        if not isinstance(key_type, BytesField) and not isinstance(key_type, UintField):
+            raise TypeError('MapField only supports string and uint to be keys')
+        super().__init__(key_type.type_num, None)
+        self.key_type = key_type
+        self.value_type = value_type
+
+    def get_value(self, instance):
+        if self.name not in instance.__dict__:
+            instance.__dict__[self.name] = {}
+        return instance.__dict__[self.name]
+
+    def encoded_length(self, val, markers: dict) -> int:
+        if not val:
+            return 0
+
+        ret = 0
+        for i, (key, val) in enumerate(val.items()):
+            self.key_type.name = f'{self.name}[{i}#k]'
+            ret += self.key_type.encoded_length(key, markers)
+            self.value_type.name = f'{self.name}[{i}#v]'
+            ret += self.value_type.encoded_length(val, markers)
+
+        return ret
+
+    def encode_into(self, val, markers: dict, wire: VarBinaryStr, offset: int) -> int:
+        if val is None:
+            return 0
+        else:
+            origin_offset = offset
+            for i, (key, val) in enumerate(val.items()):
+                self.key_type.name = f'{self.name}[{i}#k]'
+                offset += self.key_type.encode_into(key, markers, wire, offset)
+                self.value_type.name = f'{self.name}[{i}#v]'
+                offset += self.value_type.encode_into(val, markers, wire, offset)
+            return offset - origin_offset
+
+    def parse_from(self, instance, markers: dict, wire: BinaryStr, offset: int, length: int, offset_btl: int):
+        # parse_from only parses keys and will not update the value
+        dct = self.get_value(instance)
+        self.key_type.name = f'{self.name}[{len(dct)}#k]'
+        new_key = self.key_type.parse_from(instance, markers, wire, offset, length, offset_btl)
+        markers[f'{self.name}#last_key'] = new_key
+        return dct
+
+    def parse_value(self, instance, markers: dict, wire: BinaryStr, offset: int, length: int, offset_btl: int):
+        # parse_value parses the value associated with the key last parsed.
+        dct = self.get_value(instance)
+        last_key = markers.get(f'{self.name}#last_key')
+        self.value_type.name = f'{self.name}[{len(dct)}#v]'
+        val = self.value_type.parse_from(instance, markers, wire, offset, length, offset_btl)
+        dct[last_key] = val
+        return dct
+
+    def asdict(self, instance):
+        ret = {}
+        for key, val in self.__get__(instance, None).items():
+            if isinstance(val, TlvModel):
+                ret[key] = val.asdict()
+            elif isinstance(val, memoryview):
+                ret[key] = bytes(val)
+            else:
+                ret[key] = val
+        return ret
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/encoding/tlv_type.py` & `python_ndn-0.4/src/ndn/encoding/tlv_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 def is_binary_str(var):
     r"""
     Check whether var is of type BinaryStr.
 
     :param var: The variable to check.
     :return: ``True`` if var is a :any:`BinaryStr`.
     """
-    return isinstance(var, bytes) or isinstance(var, bytearray) or isinstance(var, memoryview)
+    return isinstance(var, (bytes, bytearray, memoryview))
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/encoding/tlv_var.py` & `python_ndn-0.4/src/ndn/encoding/tlv_var.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/name_tree.py` & `python_ndn-0.4/src/ndn/name_tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,63 +12,85 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import asyncio as aio
+import dataclasses as dc
+from hashlib import sha256
+from typing import Optional
 from pygtrie import Trie
-from typing import List, Optional, Tuple, Dict
-from .encoding import InterestParam, FormalName
-from .types import InterestNack, Validator, Route
+from .encoding import InterestParam, FormalName, BinaryStr
+from .types import InterestNack, Validator, Route, DataTuple
 
 
 class NameTrie(Trie):
     def _path_from_key(self, key: FormalName) -> FormalName:
         # bytes(x) will copy x if x is memoryview or bytearray but will not copy bytes
         return [x if isinstance(x, memoryview) and x.readonly else bytes(x)
                 for x in key]
 
     def _key_from_path(self, path: FormalName) -> FormalName:
         return path
 
 
+@dc.dataclass
+class PendingIntEntry:
+    future: aio.Future
+    lifetime: int
+    can_be_prefix: bool
+    must_be_fresh: bool
+    implicit_sha256: BinaryStr = b''
+
+
 class InterestTreeNode:
-    pending_list: List[Tuple[aio.Future, int, bool, bool]] = None
+    pending_list: list[PendingIntEntry]
 
     def __init__(self):
         self.pending_list = []
 
-    def append_interest(self, future: aio.Future, param: InterestParam):
-        self.pending_list.append((future, param.lifetime, param.can_be_prefix, param.must_be_fresh))
+    def append_interest(self, future: aio.Future, param: InterestParam, implicit_sha256: BinaryStr):
+        self.pending_list.append(
+            PendingIntEntry(future, param.lifetime,
+                            param.can_be_prefix, param.must_be_fresh, implicit_sha256))
 
     def nack_interest(self, nack_reason: int) -> bool:
-        for future, _, _, _ in self.pending_list:
-            future.set_exception(InterestNack(nack_reason))
+        for entry in self.pending_list:
+            entry.future.set_exception(InterestNack(nack_reason))
         return True
 
-    def satisfy(self, data, is_prefix: bool) -> bool:
-        exact_match_interest = False
-        for future, _, can_be_prefix, _ in self.pending_list:
-            if can_be_prefix or not is_prefix:
-                future.set_result(data)
+    def satisfy(self, data: DataTuple, is_prefix: bool) -> bool:
+        unsatisfied_entries = []
+        raw_packet = data[4]
+        for entry in self.pending_list:
+            if entry.can_be_prefix or not is_prefix:
+                if len(entry.implicit_sha256) > 0:
+                    data_sha256 = sha256(raw_packet).digest()
+                    passed = data_sha256 == entry.implicit_sha256
+                else:
+                    passed = True
+            else:
+                passed = False
+            if passed:
+                entry.future.set_result(data)
             else:
-                exact_match_interest = True
-        if exact_match_interest:
-            self.pending_list = [ele for ele in self.pending_list if not ele[2]]
+                unsatisfied_entries.append(entry)
+        if unsatisfied_entries:
+            self.pending_list = unsatisfied_entries
             return False
         else:
             return True
 
     def timeout(self, future: aio.Future):
-        self.pending_list = [ele for ele in self.pending_list if ele[0] is not future]
+        self.pending_list = [ele for ele in self.pending_list if ele.future is not future]
         return not self.pending_list
 
     def cancel(self):
-        for future, _, _, _ in self.pending_list:
-            future.cancel()
+        for entry in self.pending_list:
+            entry.future.cancel()
 
 
 class PrefixTreeNode:
     callback: Route = None
     validator: Optional[Validator] = None
-    extra_param: Dict = None
+    extra_param: dict = None
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/platform/general.py` & `python_ndn-0.4/src/ndn/platform/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,23 @@
         pass
 
     @abc.abstractmethod
     def default_transport(self) -> str:
         pass
 
     @abc.abstractmethod
-    def default_pib_schema(self) -> str:
+    def default_pib_scheme(self) -> str:
         pass
 
     @abc.abstractmethod
     def default_pib_paths(self) -> List[str]:
         pass
 
     @abc.abstractmethod
-    def default_tpm_schema(self) -> str:
+    def default_tpm_scheme(self) -> str:
         pass
 
     @abc.abstractmethod
     def default_tpm_paths(self) -> List[str]:
         pass
 
     @abc.abstractmethod
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/platform/linux.py` & `python_ndn-0.4/src/ndn/platform/linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,21 @@
                 '/usr/local/etc/ndn/client.conf',
                 '/opt/local/etc/ndn/client.conf',
                 '/etc/ndn/client.conf']
 
     def default_transport(self):
         return 'unix:///run/nfd.sock'
 
-    def default_pib_schema(self):
+    def default_pib_scheme(self):
         return 'pib-sqlite3'
 
     def default_pib_paths(self):
         return [os.path.expanduser(r'~/.ndn')]
 
-    def default_tpm_schema(self):
+    def default_tpm_scheme(self):
         return 'tpm-file'
 
     def default_tpm_paths(self):
         return [os.path.expanduser(r'~/.ndn/ndnsec-key-file')]
 
     async def open_unix_connection(self, path=None):
         return await aio.open_unix_connection(path)
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/platform/osx.py` & `python_ndn-0.4/src/ndn/platform/osx.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,21 +119,21 @@
                 '/usr/local/etc/ndn/client.conf',
                 '/opt/local/etc/ndn/client.conf',
                 '/etc/ndn/client.conf']
 
     def default_transport(self):
         return 'unix:///var/run/nfd.sock'
 
-    def default_pib_schema(self):
+    def default_pib_scheme(self):
         return 'pib-sqlite3'
 
     def default_pib_paths(self):
         return [os.path.expanduser(r'~/.ndn')]
 
-    def default_tpm_schema(self):
+    def default_tpm_scheme(self):
         return 'tpm-osxkeychain'
 
     def default_tpm_paths(self):
         return [os.path.expanduser(r'~/.ndn/ndnsec-key-file')]
 
     async def open_unix_connection(self, path=None):
         return await aio.open_unix_connection(path)
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/platform/windows.py` & `python_ndn-0.4/src/ndn/platform/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,22 @@
                 os.path.expandvars(r'%USERPROFILE%\ndn\client.conf'),
                 os.path.expandvars(r'%ALLUSERSPROFILE%\ndn\client.conf')]
 
     def default_transport(self):
         # Note: %TEMP% won't be redirected even when the executable is a MSIX/MicrosoftStore app
         return 'unix://' + os.path.expandvars(r'%TEMP%\nfd.sock')
 
-    def default_pib_schema(self):
+    def default_pib_scheme(self):
         return 'pib-sqlite3'
 
     def default_pib_paths(self):
         return [os.path.expandvars(r'%LOCALAPPDATA%\ndn'),
                 os.path.expandvars(r'%USERPROFILE%\ndn')]
 
-    def default_tpm_schema(self):
+    def default_tpm_scheme(self):
         return 'tpm-cng'
 
     def default_tpm_paths(self):
         return [os.path.expandvars(r'%LOCALAPPDATA%\ndn\ndnsec-key-file'),
                 os.path.expandvars(r'%USERPROFILE%\ndn\ndnsec-key-file')]
 
     @staticmethod
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/schema/policy.py` & `python_ndn-0.4/src/ndn/schema/policy.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/schema/schema_tree.py` & `python_ndn-0.4/src/ndn/schema/schema_tree.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/schema/simple_cache.py` & `python_ndn-0.4/src/ndn/schema/simple_cache.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/schema/simple_node.py` & `python_ndn-0.4/src/ndn/schema/simple_node.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/schema/simple_trust.py` & `python_ndn-0.4/src/ndn/schema/simple_trust.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/schema/util.py` & `python_ndn-0.4/src/ndn/schema/util.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain.py` & `python_ndn-0.4/src/ndn/security/keychain/keychain_digest.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,31 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
-import abc
-import collections
+from .keychain import Keychain
 from typing import Dict, Any
+from ..signer.sha256_digest_signer import DigestSha256Signer
 
 
-class Keychain(collections.abc.Mapping):
+class KeychainDigest(Keychain):
     """
-    The abstract Keychain class, derived from :class:`collections.abc.Mapping`.
-    It behaves like an immutable dict from :any:`FormalName` to Identity.
-    The implementation of Identity varies with concrete implementations.
-    Generally, its methods should also accept :any:`NonStrictName` as inputs.
-    This includes operators such as ``in`` and ``[]``.
+    A signer which has no Identity and always returns a SHA-256 digest signer.
     """
-    # __getitem__ will be called extra times, but there is no need to optimize for performance
-    @abc.abstractmethod
     def get_signer(self, sign_args: Dict[str, Any]):
-        """
-        Get a signer from sign_args.
+        if sign_args.get('no_signature', False):
+            return None
+        else:
+            return DigestSha256Signer()
 
-        :param sign_args: the signing arguments provided by the application.
-        :return: a signer.
-        :rtype: :any:`Signer`
-        """
-        pass
+    def __iter__(self):
+        return None
+
+    def __len__(self) -> int:
+        return 0
+
+    def __getitem__(self, name):
+        raise KeyError(name)
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/keychain/keychain_sqlite3.py` & `python_ndn-0.4/src/ndn/security/keychain/keychain_sqlite3.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -----------------------------------------------------------------------------
-# Copyright (C) 2019-2020 The python-ndn authors
+# Copyright (C) 2019-2022 The python-ndn authors
 #
 # This file is part of python-ndn.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -11,27 +11,168 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
+from __future__ import annotations
+import logging
+import os
 import sqlite3
-from typing import Iterator
-from dataclasses import dataclass
-from typing import Dict, Any, Mapping
+from typing import Iterator, Any
 from ...encoding import FormalName, BinaryStr, NonStrictName, Name
 from ...app_support.security_v2 import self_sign
 from ..signer.sha256_digest_signer import DigestSha256Signer
 from ..tpm.tpm import Tpm
-from .keychain import Keychain
+from .keychain import Keychain, AbstractCertificate, AbstractKey, AbstractIdentity
 
 
-@dataclass
-class Certificate:
+INITIALIZE_SQL = """
+CREATE TABLE IF NOT EXISTS
+  tpmInfo(
+    tpm_locator           BLOB
+  );
+CREATE TABLE IF NOT EXISTS
+  identities(
+    id                    INTEGER PRIMARY KEY,
+    identity              BLOB NOT NULL,
+    is_default            INTEGER DEFAULT 0
+  );
+CREATE UNIQUE INDEX IF NOT EXISTS
+  identityIndex ON identities(identity);
+CREATE TRIGGER IF NOT EXISTS
+  identity_default_before_insert_trigger
+  BEFORE INSERT ON identities
+  FOR EACH ROW
+  WHEN NEW.is_default=1
+  BEGIN
+    UPDATE identities SET is_default=0;
+  END;
+CREATE TRIGGER IF NOT EXISTS
+  identity_default_after_insert_trigger
+  AFTER INSERT ON identities
+  FOR EACH ROW
+  WHEN NOT EXISTS
+    (SELECT id
+       FROM identities
+       WHERE is_default=1)
+  BEGIN
+    UPDATE identities
+      SET is_default=1
+      WHERE identity=NEW.identity;
+  END;
+CREATE TRIGGER IF NOT EXISTS
+  identity_default_update_trigger
+  BEFORE UPDATE ON identities
+  FOR EACH ROW
+  WHEN NEW.is_default=1 AND OLD.is_default=0
+  BEGIN
+    UPDATE identities SET is_default=0;
+  END;
+CREATE TABLE IF NOT EXISTS
+  keys(
+    id                    INTEGER PRIMARY KEY,
+    identity_id           INTEGER NOT NULL,
+    key_name              BLOB NOT NULL,
+    key_bits              BLOB NOT NULL,
+    is_default            INTEGER DEFAULT 0,
+    FOREIGN KEY(identity_id)
+      REFERENCES identities(id)
+      ON DELETE CASCADE
+      ON UPDATE CASCADE
+  );
+CREATE UNIQUE INDEX IF NOT EXISTS
+  keyIndex ON keys(key_name);
+CREATE TRIGGER IF NOT EXISTS
+  key_default_before_insert_trigger
+  BEFORE INSERT ON keys
+  FOR EACH ROW
+  WHEN NEW.is_default=1
+  BEGIN
+    UPDATE keys
+      SET is_default=0
+      WHERE identity_id=NEW.identity_id;
+  END;
+CREATE TRIGGER IF NOT EXISTS
+  key_default_after_insert_trigger
+  AFTER INSERT ON keys
+  FOR EACH ROW
+  WHEN NOT EXISTS
+    (SELECT id
+       FROM keys
+       WHERE is_default=1
+         AND identity_id=NEW.identity_id)
+  BEGIN
+    UPDATE keys
+      SET is_default=1
+      WHERE key_name=NEW.key_name;
+  END;
+CREATE TRIGGER IF NOT EXISTS
+  key_default_update_trigger
+  BEFORE UPDATE ON keys
+  FOR EACH ROW
+  WHEN NEW.is_default=1 AND OLD.is_default=0
+  BEGIN
+    UPDATE keys
+      SET is_default=0
+      WHERE identity_id=NEW.identity_id;
+  END;
+CREATE TABLE IF NOT EXISTS
+  certificates(
+    id                    INTEGER PRIMARY KEY,
+    key_id                INTEGER NOT NULL,
+    certificate_name      BLOB NOT NULL,
+    certificate_data      BLOB NOT NULL,
+    is_default            INTEGER DEFAULT 0,
+    FOREIGN KEY(key_id)
+      REFERENCES keys(id)
+      ON DELETE CASCADE
+      ON UPDATE CASCADE
+  );
+CREATE UNIQUE INDEX IF NOT EXISTS
+  certIndex ON certificates(certificate_name);
+CREATE TRIGGER IF NOT EXISTS
+  cert_default_before_insert_trigger
+  BEFORE INSERT ON certificates
+  FOR EACH ROW
+  WHEN NEW.is_default=1
+  BEGIN
+    UPDATE certificates
+      SET is_default=0
+      WHERE key_id=NEW.key_id;
+  END;
+CREATE TRIGGER IF NOT EXISTS
+  cert_default_after_insert_trigger
+  AFTER INSERT ON certificates
+  FOR EACH ROW
+  WHEN NOT EXISTS
+    (SELECT id
+       FROM certificates
+       WHERE is_default=1
+         AND key_id=NEW.key_id)
+  BEGIN
+    UPDATE certificates
+      SET is_default=1
+      WHERE certificate_name=NEW.certificate_name;
+  END;
+CREATE TRIGGER IF NOT EXISTS
+  cert_default_update_trigger
+  BEFORE UPDATE ON certificates
+  FOR EACH ROW
+  WHEN NEW.is_default=1 AND OLD.is_default=0
+  BEGIN
+    UPDATE certificates
+      SET is_default=0
+      WHERE key_id=NEW.key_id;
+  END;
+"""
+
+
+class Certificate(AbstractCertificate):
     """
     A dataclass for a Certificate.
 
     :ivar id: its id in the database.
     :vartype id: int
     :ivar key: the Name of the associated Key.
     :vartype key: :any:`FormalName`
@@ -39,21 +180,40 @@
     :vartype name: :any:`FormalName`
     :ivar data: the content.
     :vartype data: bytes
     :ivar is_default: whether this is the default Identity.
     :vartype is_default: bool
     """
     id: int
-    key: FormalName
-    name: FormalName
-    data: BinaryStr
+    _key: FormalName
+    _name: FormalName
+    _data: BinaryStr
     is_default: bool
 
+    @property
+    def name(self) -> FormalName:
+        return self._name
+
+    @property
+    def key(self) -> FormalName:
+        return self._key
+
+    @property
+    def data(self) -> BinaryStr:
+        return self._data
+
+    def __init__(self, row_id: int, key: FormalName, name: FormalName, data: BinaryStr, is_default: bool):
+        self.id = row_id
+        self._key = key
+        self._name = name
+        self._data = data
+        self.is_default = is_default
+
 
-class Key(Mapping[FormalName, Certificate]):
+class Key(AbstractKey):
     """
     A Key. It behaves like an immutable ``dict`` from :any:`FormalName` to :any:`Certificate`.
 
     :ivar row_id: its id in the database.
     :vartype row_id: int
     :ivar identity: the Name of the associated Identity.
     :vartype identity: :any:`FormalName`.
@@ -61,25 +221,37 @@
     :vartype name: :any:`FormalName`
     :ivar key_bits: the key bits of the public key.
     :vartype key_bits: bytes
     :ivar is_default: whether this is the default Identity.
     :vartype is_default: bool
     """
     row_id: int
-    identity: FormalName
-    name: FormalName
-    key_bits: BinaryStr
+    _identity: FormalName
+    _name: FormalName
+    _key_bits: BinaryStr
     is_default: bool
 
+    @property
+    def key_bits(self) -> BinaryStr:
+        return self._key_bits
+
+    @property
+    def name(self) -> FormalName:
+        return self._name
+
+    @property
+    def identity(self) -> FormalName:
+        return self._identity
+
     def __init__(self, pib, identity, row_id, name, key_bits, is_default):
         self.pib = pib
-        self.identity = identity
+        self._identity = identity
         self.row_id = row_id
-        self.name = name
-        self.key_bits = key_bits
+        self._name = name
+        self._key_bits = key_bits
         self.is_default = is_default
 
     def __len__(self) -> int:
         cursor = self.pib.conn.execute('SELECT count(*) FROM keys WHERE identity_id=?', (self.row_id,))
         ret = cursor.fetchone()[0]
         cursor.close()
         return ret
@@ -89,15 +261,15 @@
         sql = 'SELECT id, certificate_name, certificate_data, is_default FROM certificates WHERE certificate_name=?'
         cursor = self.pib.conn.execute(sql, (name,))
         data = cursor.fetchone()
         if not data:
             raise KeyError(name)
         row_id, cert_name, cert_data, is_default = data
         cursor.close()
-        return Certificate(id=row_id, key=self.name, name=cert_name, data=cert_data, is_default=is_default != 0)
+        return Certificate(row_id=row_id, key=self._name, name=cert_name, data=cert_data, is_default=is_default != 0)
 
     def __iter__(self) -> Iterator[FormalName]:
         cursor = self.pib.conn.execute('SELECT certificate_name FROM certificates WHERE key_id=?', (self.row_id,))
         while True:
             name = cursor.fetchone()
             if not name:
                 break
@@ -145,36 +317,40 @@
                'FROM certificates WHERE is_default=1 AND key_id=?')
         cursor = self.pib.conn.execute(sql, (self.row_id,))
         data = cursor.fetchone()
         if not data:
             raise KeyError('No default certificate')
         row_id, cert_name, cert_data, is_default = data
         cursor.close()
-        return Certificate(id=row_id, key=self.name, name=cert_name, data=cert_data, is_default=is_default != 0)
+        return Certificate(row_id=row_id, key=self._name, name=cert_name, data=cert_data, is_default=is_default != 0)
 
 
-class Identity(Mapping[FormalName, Key]):
+class Identity(AbstractIdentity):
     """
     An Identity. It behaves like an immutable ``dict`` from :any:`FormalName` to :any:`Key`.
 
     :ivar row_id: its id in the database.
     :vartype row_id: int
     :ivar name: its Name.
     :vartype name: :any:`FormalName`
     :ivar is_default: whether this is the default Identity.
     :vartype is_default: bool
     """
     row_id: int
-    name: FormalName
+    _name: FormalName
     is_default: bool
 
+    @property
+    def name(self) -> FormalName:
+        return self._name
+
     def __init__(self, pib, row_id, name, is_default):
         self.pib = pib
         self.row_id = row_id
-        self.name = name
+        self._name = name
         self.is_default = is_default
 
     def __len__(self) -> int:
         cursor = self.pib.conn.execute('SELECT count(*) FROM keys WHERE identity_id=?', (self.row_id,))
         ret = cursor.fetchone()[0]
         cursor.close()
         return ret
@@ -184,15 +360,15 @@
         cursor = self.pib.conn.execute('SELECT id, key_name, key_bits, is_default FROM keys WHERE key_name=?',
                                        (name,))
         data = cursor.fetchone()
         if not data:
             raise KeyError(name)
         row_id, key_name, key_bits, is_default = data
         cursor.close()
-        return Key(self.pib, self.name, row_id, Name.from_bytes(key_name), key_bits, is_default != 0)
+        return Key(self.pib, self._name, row_id, Name.from_bytes(key_name), key_bits, is_default != 0)
 
     def __iter__(self) -> Iterator[FormalName]:
         cursor = self.pib.conn.execute('SELECT key_name FROM keys WHERE identity_id=?', (self.row_id,))
         while True:
             name = cursor.fetchone()
             if not name:
                 break
@@ -211,15 +387,15 @@
     def new_key(self, key_type: str) -> Key:
         """
         Create a new key with default arguments.
 
         :param key_type: the type of the Key. Can be ``ec`` or ``rsa``.
         :return: the new Key.
         """
-        return self.pib.new_key(self.name, key_type=key_type)
+        return self.pib.new_key(self._name, key_type=key_type)
 
     def has_default_key(self) -> bool:
         """
         Whether it has a default Key.
 
         :return: ``True`` if there is one.
         """
@@ -248,15 +424,15 @@
         sql = 'SELECT id, key_name, key_bits, is_default FROM keys WHERE is_default=1 AND identity_id=?'
         cursor = self.pib.conn.execute(sql, (self.row_id,))
         data = cursor.fetchone()
         if not data:
             raise KeyError('No default key')
         row_id, key_name, key_bits, is_default = data
         cursor.close()
-        return Key(self.pib, self.name, row_id, Name.from_bytes(key_name), key_bits, is_default != 0)
+        return Key(self.pib, self._name, row_id, Name.from_bytes(key_name), key_bits, is_default != 0)
 
 
 class KeychainSqlite3(Keychain):
     r"""
     Store public infomation in a Sqlite3 database and private keys in a TPM.
 
     :ivar path: the path to the database. The default path is ``~/.ndn/pib.db``.
@@ -267,14 +443,35 @@
     :vartype tpm_locator: str
     """
     tpm: Tpm
     path: str
     tpm_locator: str
     _signer_cache: dict
 
+    @staticmethod
+    def initialize(path: str, tpm_scheme: str, tpm_path: str = '') -> bool:
+        if os.path.exists(path):
+            logging.fatal(f'PIB database {path} already exists.')
+            return False
+        # Make sure the directory exists
+        base_dir = os.path.dirname(path)
+        os.makedirs(base_dir, exist_ok=True)
+        # Create an empty folder if the scheme is file
+        if tpm_scheme == 'tpm-file':
+            if not tpm_path:
+                tpm_path = os.path.join(base_dir, 'ndnsec-key-file')
+            os.makedirs(tpm_path, exist_ok=True)
+        # Create sqlite3 database
+        conn = sqlite3.connect(path)
+        conn.executescript(INITIALIZE_SQL)
+        conn.execute('INSERT INTO tpmInfo (tpm_locator) VALUES (?)', (f'{tpm_scheme}:{tpm_path}'.encode(),))
+        conn.commit()
+        conn.close()
+        return True
+
     def __init__(self, path: str, tpm: Tpm):
         self.path = path
         self.conn = sqlite3.connect(path)
         cursor = self.conn.execute('SELECT tpm_locator FROM tpmInfo')
         self.tpm_locator = cursor.fetchone()[0]
         cursor.close()
         self.tpm = tpm
@@ -373,68 +570,92 @@
             self.conn.execute('INSERT INTO identities (identity) VALUES (?)', (name,))
             self.conn.commit()
             self.new_key(name)
         if not self.has_default_identity():
             self.set_default_identity(name)
         return self[name]
 
+    def __del__(self):
+        if self.conn is not None:
+            self.shutdown()
+
     def shutdown(self):
         """
         Close the connection.
         """
         self.conn.close()
+        self.conn = None
 
     def del_identity(self, name: NonStrictName):
         """
         Delete a specific Identity.
 
         :param name: the Identity Name.
         :type name: :any:`NonStrictName`
         """
         name = Name.to_bytes(name)
         for key_name in self[name]:
-            self.tpm.delete_key(key_name)
+            self.del_key(key_name)
         self.conn.execute('DELETE FROM identities WHERE identity=?', (name,))
         self.conn.commit()
         self._signer_cache = {}
 
-    def get_signer(self, sign_args: Dict[str, Any]):
-        if sign_args.pop('no_signature', False):
+    def get_signer(self, sign_args: dict[str, Any]):
+        if sign_args.get('no_signature', False):
             return None
-        if sign_args.pop('digest_sha256', False):
+        if sign_args.get('digest_sha256', False):
             return DigestSha256Signer()
-        key_name = sign_args.pop('key', None)
-        if not key_name:
-            id_name = sign_args.pop('identity', None)
-            if id_name:
-                if isinstance(id_name, Identity):
-                    identity = id_name
+        cert_name = sign_args.get('cert', None)
+        if not cert_name:
+            key_name = sign_args.get('key', None)
+            if not key_name:
+                id_name = sign_args.get('identity', None)
+                if id_name:
+                    if isinstance(id_name, Identity):
+                        identity = id_name
+                    else:
+                        identity = self[id_name]
                 else:
-                    identity = self[id_name]
+                    identity = self.default_identity()
+                key = identity.default_key()
+                cert_name = key.default_cert().name
+                key_name = key.name
+            elif isinstance(key_name, Key):
+                cert_name = key_name.default_cert().name
+                key_name = key_name.name
             else:
-                identity = self.default_identity()
-            key_name = identity.default_key().name
-        elif isinstance(key_name, Key):
-            key_name = key_name.name
-        key_name_bytes = Name.to_bytes(key_name)
-        signer = self._signer_cache.get(key_name_bytes, None)
+                id_name = key_name[:-2]
+                cert_name = self[id_name][key_name].default_cert().name
+        elif isinstance(cert_name, Certificate):
+            cert_name = cert_name.name
+            key_name = cert_name[:-2]
+        else:
+            key_name = cert_name[:-2]
+        key_locator_name = sign_args.get('key_locator', None)
+        if not key_locator_name:
+            key_locator_name = cert_name
+        key_locator_bytes = Name.to_bytes(key_locator_name)
+        signer = self._signer_cache.get(key_locator_bytes, None)
         if not signer:
-            signer = self.tpm.get_signer(key_name)
-            self._signer_cache[key_name_bytes] = signer
+            signer = self.tpm.get_signer(key_name, key_locator_name)
+            self._signer_cache[key_locator_bytes] = signer
         return signer
 
     def del_key(self, name: NonStrictName):
         """
         Delete a specific Key.
 
         :param name: the Key Name.
         :type name: :any:`NonStrictName`
         """
         formal_name = Name.normalize(name)
         name = Name.to_bytes(name)
+        id_name = formal_name[:-2]
+        key = self[id_name][formal_name]
+        self.conn.execute('DELETE FROM certificates WHERE key_id=?', (key.row_id,))
         self.conn.execute('DELETE FROM keys WHERE key_name=?', (name,))
         self.conn.commit()
         self.tpm.delete_key(formal_name)
         self._signer_cache = {}
 
     def del_cert(self, name: NonStrictName):
         """
@@ -485,7 +706,15 @@
                           'VALUES ((SELECT id FROM keys WHERE key_name=?), ?, ?)',
                           (key_name, cert_name, bytes(cert_data)))
         self.conn.commit()
 
         if not identity.has_default_key():
             identity.set_default_key(key_name)
         return identity[key_name]
+
+    def import_cert(self, key_name: NonStrictName, cert_name: NonStrictName, cert_data: BinaryStr):
+        key_name = Name.to_bytes(key_name)
+        cert_name = Name.to_bytes(cert_name)
+        self.conn.execute('INSERT INTO certificates (key_id, certificate_name, certificate_data)'
+                          'VALUES ((SELECT id FROM keys WHERE key_name=?), ?, ?)',
+                          (key_name, cert_name, bytes(cert_data)))
+        self.conn.commit()
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_digest_signer.py` & `python_ndn-0.4/src/ndn/security/signer/null_signer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -----------------------------------------------------------------------------
-# Copyright (C) 2019-2020 The python-ndn authors
+# Copyright (C) 2019-2021 The python-ndn authors
 #
 # This file is part of python-ndn.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -12,25 +12,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 from typing import List
-from Cryptodome.Hash import SHA256
 from ...encoding import Signer, SignatureType, VarBinaryStr
 
 
-class DigestSha256Signer(Signer):
+class NullSigner(Signer):
     def write_signature_info(self, signature_info):
-        signature_info.signature_type = SignatureType.DIGEST_SHA256
+        signature_info.signature_type = SignatureType.NULL
         signature_info.key_locator = None
 
     def get_signature_value_size(self):
-        return 32
+        return 0
 
     def write_signature_value(self, wire: VarBinaryStr, contents: List[VarBinaryStr]) -> int:
-        h = SHA256.new()
-        for blk in contents:
-            h.update(blk)
-        wire[:] = h.digest()
-        return 32
+        wire[:] = b''
+        return 0
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_ecdsa_signer.py` & `python_ndn-0.4/src/ndn/security/signer/sha256_ecdsa_signer.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,35 +20,35 @@
 from Cryptodome.PublicKey import ECC
 from Cryptodome.Signature import DSS
 from ...encoding import Signer, SignatureType, KeyLocator, NonStrictName, VarBinaryStr
 
 
 class Sha256WithEcdsaSigner(Signer):
     # SHA256 doesn't work for P-384 and P-521
-    key_name: NonStrictName
+    key_locator_name: NonStrictName
     key_der: bytes
     curve_bit: int
     key_size: int
 
-    def __init__(self, key_name: NonStrictName, key_der: Union[bytes, str]):
-        self.key_name = key_name
+    def __init__(self, key_locator_name: NonStrictName, key_der: Union[bytes, str]):
+        self.key_locator_name = key_locator_name
         self.key_der = key_der
         self.key = ECC.import_key(self.key_der)
         curve = self.key.curve
         if curve[-2:] == 'r1' or curve[-2:] == 'v1':
             self.curve_bit = int(curve[-5:-2])
         else:
             self.curve_bit = int(curve[-3:])
         self.key_size = (self.curve_bit * 2 + 7) // 8
         self.key_size += self.key_size % 2
 
     def write_signature_info(self, signature_info):
         signature_info.signature_type = SignatureType.SHA256_WITH_ECDSA
         signature_info.key_locator = KeyLocator()
-        signature_info.key_locator.name = self.key_name
+        signature_info.key_locator.name = self.key_locator_name
 
     def get_signature_value_size(self):
         return self.key_size + 8
 
     def write_signature_value(self, wire: VarBinaryStr, contents: List[VarBinaryStr]) -> int:
         h = SHA256.new()
         for blk in contents:
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_hmac_signer.py` & `python_ndn-0.4/src/ndn/security/signer/ed25519_signer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -----------------------------------------------------------------------------
-# Copyright (C) 2019-2020 The python-ndn authors
+# Copyright (C) 2019-2022 The python-ndn authors
 #
 # This file is part of python-ndn.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -11,34 +11,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
-from typing import List
-from Cryptodome.Hash import SHA256, HMAC
-from ...encoding import Signer, SignatureType, KeyLocator, NonStrictName, VarBinaryStr
+from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
+from ...encoding import Signer, SignatureType, KeyLocator, NonStrictName, VarBinaryStr, BinaryStr
 
 
-class HmacSha256Signer(Signer):
-    key_name: NonStrictName
-    key_bytes: bytes
-
-    def __init__(self, key_name: NonStrictName, key_bytes: bytes):
-        self.key_name = key_name
-        self.key_bytes = key_bytes
+class Ed25519Signer(Signer):
+    key_locator_name: NonStrictName
+
+    def __init__(self, key_locator_name: NonStrictName, key_bits: BinaryStr):
+        self.key_locator_name = key_locator_name
+        self.key = Ed25519PrivateKey.from_private_bytes(key_bits)
 
     def write_signature_info(self, signature_info):
-        signature_info.signature_type = SignatureType.HMAC_WITH_SHA256
+        signature_info.signature_type = SignatureType.ED25519
         signature_info.key_locator = KeyLocator()
-        signature_info.key_locator.name = self.key_name
+        signature_info.key_locator.name = self.key_locator_name
 
     def get_signature_value_size(self):
-        return 32
+        return 64
 
-    def write_signature_value(self, wire: VarBinaryStr, contents: List[VarBinaryStr]) -> int:
-        h = HMAC.new(self.key_bytes, digestmod=SHA256)
-        for blk in contents:
-            h.update(blk)
-        wire[:] = h.digest()
-        return 32
+    def write_signature_value(self, wire: VarBinaryStr, contents: list[VarBinaryStr]) -> int:
+        # Copying is needed as cryptography library only support bytes
+        c = b''.join(bytes(blk) for blk in contents)
+        signature = self.key.sign(c)
+        wire[:] = signature
+        return len(signature)
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/signer/sha256_rsa_signer.py` & `python_ndn-0.4/src/ndn/security/signer/sha256_digest_signer.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,38 +11,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
-from typing import List, Union
+from typing import List
 from Cryptodome.Hash import SHA256
-from Cryptodome.PublicKey import RSA
-from Cryptodome.Signature import pkcs1_15
-from ...encoding import Signer, SignatureType, KeyLocator, NonStrictName, VarBinaryStr
+from ...encoding import Signer, SignatureType, VarBinaryStr
+from ...utils import timestamp, gen_nonce_64
 
 
-class Sha256WithRsaSigner(Signer):
-    key_name: NonStrictName
-    key_der: bytes
-
-    def __init__(self, key_name: NonStrictName, key_der: Union[str, bytes]):
-        self.key_name = key_name
-        self.key_der = key_der
-        self.key = RSA.import_key(self.key_der)
+class DigestSha256Signer(Signer):
+    for_interest: bool
+
+    def __init__(self, for_interest: bool = False):
+        self.for_interest = for_interest
 
     def write_signature_info(self, signature_info):
-        signature_info.signature_type = SignatureType.SHA256_WITH_RSA
-        signature_info.key_locator = KeyLocator()
-        signature_info.key_locator.name = self.key_name
+        signature_info.signature_type = SignatureType.DIGEST_SHA256
+        signature_info.key_locator = None
+        if self.for_interest:
+            signature_info.signature_time = timestamp()
+            signature_info.signature_nonce = gen_nonce_64()
 
     def get_signature_value_size(self):
-        return self.key.size_in_bytes()
+        return 32
 
     def write_signature_value(self, wire: VarBinaryStr, contents: List[VarBinaryStr]) -> int:
         h = SHA256.new()
         for blk in contents:
             h.update(blk)
-        signature = pkcs1_15.new(self.key).sign(h)
-        wire[:] = signature
-        return len(signature)
+        wire[:] = h.digest()
+        return 32
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm.py` & `python_ndn-0.4/src/ndn/security/tpm/tpm.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import abc
-from typing import Tuple
+from typing import Tuple, Optional
 from Cryptodome.Hash import SHA256
 from Cryptodome.Random import get_random_bytes
 from ...app_support.security_v2 import KEY_COMPONENT
 from ...encoding import Signer, NonStrictName, BinaryStr, FormalName, Component
 
 
 class Tpm(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def get_signer(self, key_name: NonStrictName) -> Signer:
+    def get_signer(self, key_name: NonStrictName, key_locator_name: Optional[NonStrictName] = None) -> Signer:
         pass
 
     @abc.abstractmethod
     def generate_key(self, id_name: FormalName, key_type: str = 'rsa', **kwargs) -> Tuple[FormalName, BinaryStr]:
         pass
 
     @abc.abstractmethod
@@ -37,16 +37,16 @@
         pass
 
     @abc.abstractmethod
     def delete_key(self, key_name: FormalName):
         pass
 
     def construct_key_name(self, id_name: FormalName, pub_key: BinaryStr, **kwargs) -> FormalName:
-        key_id = kwargs.pop('key_id', None)
-        key_id_type = kwargs.pop('key_id_type', 'random')
+        key_id = kwargs.get('key_id', None)
+        key_id_type = kwargs.get('key_id_type', 'random')
         if not key_id:
             if key_id_type == 'random':
                 while True:
                     key_id = Component.from_bytes(get_random_bytes(8))
                     if not self.key_exist(id_name + [KEY_COMPONENT, key_id]):
                         break
             elif key_id_type == 'sha256':
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_cng.py` & `python_ndn-0.4/src/ndn/security/tpm/tpm_cng.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import sys
 import ctypes as c
 import logging
-from typing import Tuple
+from typing import Tuple, Optional
 from Cryptodome.PublicKey import ECC, RSA
 from Cryptodome.Util.asn1 import DerSequence
 from ndn.encoding import FormalName, BinaryStr
 
 from ...encoding import Signer, NonStrictName, SignatureType, KeyLocator, Name
 from .tpm import Tpm
 if sys.platform == 'win32':
     from ...platform.windows import Cng, ReleaseGuard
 
 
 class CngSigner(Signer):
-    def __init__(self, key_name: NonStrictName, sig_len, key_type, h_key):
+    def __init__(self, key_locator_name: NonStrictName, sig_len, key_type, h_key):
         self.h_key = h_key
-        self.key_name = key_name
+        self.key_locator_name = key_locator_name
         if key_type == "RSA":
             self.key_type = SignatureType.SHA256_WITH_RSA
             self.sig_len = sig_len
         elif key_type == "ECDSA":
             self.key_type = SignatureType.SHA256_WITH_ECDSA
             self.sig_len = sig_len + 8
         else:
             raise ValueError(f'Unrecognized key type {key_type}')
 
     def write_signature_info(self, signature_info):
         signature_info.signature_type = self.key_type
         signature_info.key_locator = KeyLocator()
-        signature_info.key_locator.name = self.key_name
+        signature_info.key_locator.name = self.key_locator_name
 
     def get_signature_value_size(self):
         return self.sig_len
 
     def __del__(self):
         Cng().ncrypt.NCryptFreeObject(self.h_key)
 
@@ -174,18 +174,20 @@
         status = cng.ncrypt.NCryptGetProperty(h_key, c.c_wchar_p('AlgorithmName'), c.pointer(key_type), cb_property,
                                               c.pointer(cb_property), 0)
         if not cng.nt_success(status):
             raise OSError(f'Error {status} returned by NCryptGetProperty', status)
 
         return key_type.value, sig_len.value, h_key
 
-    def get_signer(self, key_name: NonStrictName) -> Signer:
+    def get_signer(self, key_name: NonStrictName, key_locator_name: Optional[NonStrictName] = None) -> Signer:
         name_hash = Name.to_bytes(key_name).hex()
         key_type, sig_len, h_key = self._get_key(name_hash)
-        return CngSigner(key_name, sig_len, key_type, h_key)
+        if key_locator_name is None:
+            key_locator_name = key_name
+        return CngSigner(key_locator_name, sig_len, key_type, h_key)
 
     def key_exist(self, key_name: FormalName) -> bool:
         try:
             name_hash = Name.to_bytes(key_name).hex()
             self._get_key(name_hash)
             return True
         except KeyError:
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_file.py` & `python_ndn-0.4/src/ndn/security/tpm/tpm_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import os
 from base64 import b64decode, b64encode
 from hashlib import sha256
-from typing import Tuple
+from typing import Tuple, Optional
 from Cryptodome.PublicKey import RSA, ECC
 from ...encoding import Signer, NonStrictName, Name, BinaryStr, FormalName
 from ..signer.sha256_rsa_signer import Sha256WithRsaSigner
 from ..signer.sha256_ecdsa_signer import Sha256WithEcdsaSigner
 from .tpm import Tpm
 
 
@@ -36,25 +36,27 @@
     def _to_file_name(key_name: bytes):
         return sha256(key_name).digest().hex() + '.privkey'
 
     @staticmethod
     def _base64_newline(src: bytes):
         return b'\n'.join(src[i*64:i*64+64] for i in range((len(src) + 63) // 64))
 
-    def get_signer(self, key_name: NonStrictName) -> Signer:
+    def get_signer(self, key_name: NonStrictName, key_locator_name: Optional[NonStrictName] = None) -> Signer:
         key_name = Name.to_bytes(key_name)
+        if key_locator_name is None:
+            key_locator_name = key_name
         file_name = os.path.join(self.path, self._to_file_name(key_name))
         if not os.path.exists(file_name):
             raise KeyError(key_name)
         with open(file_name, 'rb') as f:
             key_b64 = f.read()
         key_der = b64decode(key_b64)
         for signer in [Sha256WithRsaSigner, Sha256WithEcdsaSigner]:
             try:
-                return signer(key_name, key_der)
+                return signer(key_locator_name, key_der)
             except ValueError:
                 pass
         raise ValueError('Key format is not supported')
 
     def key_exist(self, key_name: FormalName) -> bool:
         key_name = Name.encode(key_name)
         file_name = os.path.join(self.path, self._to_file_name(key_name))
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/tpm/tpm_osx_keychain.py` & `python_ndn-0.4/src/ndn/security/tpm/tpm_osx_keychain.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,44 +13,44 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import sys
 import logging
-from typing import Tuple
+from typing import Tuple, Optional
 from ctypes import c_void_p, pointer, c_int
 from Cryptodome.Hash import SHA256
 from Cryptodome.PublicKey import RSA, ECC
 from ...encoding import Signer, NonStrictName, Name, SignatureType, KeyLocator, BinaryStr, FormalName
 from .tpm import Tpm
 if sys.platform == 'darwin':
     from ...contrib.cocoapy import cf, CFSTR, ObjCInstance, cfstring_to_string, cfnumber_to_number, kCFNumberIntType
     from ...platform.osx import OsxSec, ReleaseGuard
 
 
 class OsxSigner(Signer):
-    def __init__(self, key_name: NonStrictName, key_bits, key_type, key_ref):
+    def __init__(self, key_locator_name: NonStrictName, key_bits, key_type, key_ref):
         self.key_ref = key_ref
-        self.key_name = key_name
+        self.key_locator_name = key_locator_name
         if key_type == cfstring_to_string(OsxSec().kSecAttrKeyTypeRSA):
             self.key_type = SignatureType.SHA256_WITH_RSA
             self.key_size = key_bits // 8
         elif key_type == cfstring_to_string(OsxSec().kSecAttrKeyTypeECSECPrimeRandom):
             self.key_type = SignatureType.SHA256_WITH_ECDSA
             self.key_size = (key_bits * 2 + 7) // 8
             self.key_size += self.key_size % 2
             self.key_size += 8
         else:
             raise ValueError(f'Unrecognized key type {key_type}')
 
     def write_signature_info(self, signature_info):
         signature_info.signature_type = self.key_type
         signature_info.key_locator = KeyLocator()
-        signature_info.key_locator.name = self.key_name
+        signature_info.key_locator.name = self.key_locator_name
 
     def get_signature_value_size(self):
         return self.key_size
 
     def __del__(self):
         cf.CFRelease(self.key_ref)
 
@@ -100,17 +100,19 @@
                 raise RuntimeError(f"Error happened when searching specific key {key_name}")
 
             key_type = cfstring_to_string(cf.CFDictionaryGetValue(g.dic, sec.kSecAttrKeyType))
             key_bits = cfnumber_to_number(cf.CFDictionaryGetValue(g.dic, sec.kSecAttrKeySizeInBits))
             key_ref = cf.CFRetain(cf.CFDictionaryGetValue(g.dic, sec.kSecValueRef))
         return key_type, key_bits, key_ref
 
-    def get_signer(self, key_name: NonStrictName) -> Signer:
+    def get_signer(self, key_name: NonStrictName, key_locator_name: Optional[NonStrictName] = None) -> Signer:
         key_type, key_bits, key_ref = self._get_key(key_name)
-        return OsxSigner(key_name, key_bits, key_type, key_ref)
+        if key_locator_name is None:
+            key_locator_name = key_name
+        return OsxSigner(key_locator_name, key_bits, key_type, key_ref)
 
     def key_exist(self, key_name: FormalName) -> bool:
         try:
             self._get_key(key_name)
             return True
         except KeyError:
             return False
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/security/validator/digest_validator.py` & `python_ndn-0.4/src/ndn/security/validator/digest_validator.py`

 * *Files identical despite different names*

### Comparing `python-ndn-0.3a1.post4/src/ndn/transport/dummy_face.py` & `python_ndn-0.4/src/ndn/transport/dummy_face.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
 import asyncio as aio
+
 from ndn.encoding import parse_tl_num
-from ndn.transport.stream_socket import Face
+from ndn.transport.face import Face
 
 
 class DummyFace(Face):
     app = None
 
     def __init__(self, test_func):
         super().__init__()
@@ -42,14 +43,17 @@
             self.event.set()
 
     async def run(self):
         await self.test_func(self)
         if self.app:
             self.app.shutdown()
 
+    def isLocalFace(self):
+        return True
+
     async def consume_output(self, expected_output, timeout=0.01):
         self.expected_len = len(expected_output)
         if len(self.output_buf) < self.expected_len:
             await aio.wait_for(self.event.wait(), timeout)
         self.expected_len = 2 ** 32
         self.event.clear()
         assert self.output_buf == expected_output
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/transport/stream_socket.py` & `python_ndn-0.4/src/ndn/transport/stream_face.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,44 +11,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -----------------------------------------------------------------------------
-import io
 import abc
 import asyncio as aio
-from typing import Optional, Callable, Coroutine, Any
-from ..encoding.tlv_var import read_tl_num_from_stream
-from ..platform import Platform
-
-
-class Face(metaclass=abc.ABCMeta):
-    running: bool = False
-    callback: Callable[[int, bytes], Coroutine[Any, None, None]] = None
-
-    def __init__(self):
-        self.running = False
-
-    @abc.abstractmethod
-    async def open(self):
-        pass
-
-    @abc.abstractmethod
-    def shutdown(self):
-        pass
+import io
+from typing import Optional
 
-    @abc.abstractmethod
-    def send(self, data: bytes):
-        pass
+from ndn.transport.ip_face import IpFace
 
-    @abc.abstractmethod
-    async def run(self):
-        pass
+from ..encoding.tlv_var import read_tl_num_from_stream
+from ..platform import Platform
+from .face import Face
 
 
 class StreamFace(Face, metaclass=abc.ABCMeta):
     reader: Optional[aio.StreamReader] = None
     writer: Optional[aio.StreamWriter] = None
 
     def shutdown(self):
@@ -81,16 +61,19 @@
         if path:
             self.path = path
 
     async def open(self):
         self.reader, self.writer = await Platform().open_unix_connection(self.path)
         self.running = True
 
+    def isLocalFace(self):
+        return True
+
 
-class TcpFace(StreamFace):
+class TcpFace(StreamFace, IpFace):
     host: str = '127.0.0.1'
     port: int = 6363
 
     def __init__(self, host: str = '', port: int = 0):
         super().__init__()
         if host:
             self.host = host
```

### Comparing `python-ndn-0.3a1.post4/src/ndn/utils.py` & `python_ndn-0.4/src/ndn/utils.py`

 * *Files identical despite different names*

