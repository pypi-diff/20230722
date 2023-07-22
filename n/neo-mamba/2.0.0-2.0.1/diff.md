# Comparing `tmp/neo-mamba-2.0.0.tar.gz` & `tmp/neo-mamba-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo-mamba-2.0.0.tar", last modified: Wed Jul  5 17:21:02 2023, max compression
+gzip compressed data, was "neo-mamba-2.0.1.tar", last modified: Sat Jul 22 11:33:48 2023, max compression
```

## Comparing `neo-mamba-2.0.0.tar` & `neo-mamba-2.0.1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.726175 neo-mamba-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.730175 neo-mamba-2.0.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/advanced.md
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/home.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/mamba-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/smart-contracts.md
--rw-r--r--   0 runner    (1001) docker     (123)    26776 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/wrapper-hierarchy.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.730175 neo-mamba-2.0.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/examples/shared/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/coz-wallet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/default.neo-express
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.nef
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.nef
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/examples/shared/nep11-token/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/compile_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/go.mod
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/go.sum
--rwxr-xr-x   0 runner    (1001) docker     (123)     2042 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/nep11-token.manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/nep11-token.nef
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/nft.go
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/nft.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/examples/shared/nep17-token/
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.nef
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/register-candidate.invoke
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/setup-neoxp-for-tests.batch
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/user-wallet.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/neo3/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/neo3/api/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/helpers/signing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/helpers/txbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/helpers/unwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    45820 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/noderpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    56625 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/callflags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/findoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/nef.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/core/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/core/cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/cryptography/bloomfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/cryptography/ecc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/cryptography/merkletree.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/types/uint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/network/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/network/convenience/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/flightinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18614 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/nodemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/nodeweight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/requestinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/syncmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/ipfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    27799 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/neo3/network/payloads/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/address.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/extensible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    27818 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/relaycache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    26371 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/neo3/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/scrypt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/neo_mamba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-05 17:21:02.750176 neo-mamba-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/api/test_noderpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_callflags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_contractstate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20522 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_nef.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_biginteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/network/convenience/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/convenience/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/convenience/test_nodemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/convenience/test_syncmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/convenience/test_various.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_ipfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    61223 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_witnessrules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/test_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/wallet/rc2-wallet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/wallet/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/wallet/test_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.097331 neo-mamba-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-22 11:33:48.097331 neo-mamba-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.053331 neo-mamba-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.061331 neo-mamba-2.0.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/docs/source/advanced.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/docs/source/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/docs/source/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/docs/source/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/docs/source/mamba-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/docs/source/smart-contracts.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26776 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/docs/source/wrapper-hierarchy.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.053331 neo-mamba-2.0.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.065331 neo-mamba-2.0.1/examples/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/coz-wallet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/default.neo-express
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.069331 neo-mamba-2.0.1/examples/shared/deploy-update-destroy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v1.manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v1.nef
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v2.manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v2.nef
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.069331 neo-mamba-2.0.1/examples/shared/nep11-token/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep11-token/compile_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep11-token/go.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep11-token/go.sum
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2042 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep11-token/nep11-token.manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep11-token/nep11-token.nef
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep11-token/nft.go
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep11-token/nft.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.069331 neo-mamba-2.0.1/examples/shared/nep17-token/
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep17-token/nep17token.manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep17-token/nep17token.nef
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/nep17-token/nep17token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/register-candidate.invoke
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/setup-neoxp-for-tests.batch
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/examples/shared/user-wallet.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.069331 neo-mamba-2.0.1/neo3/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.073331 neo-mamba-2.0.1/neo3/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.073331 neo-mamba-2.0.1/neo3/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/api/helpers/signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/api/helpers/txbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/api/helpers/unwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45820 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/api/noderpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56625 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.073331 neo-mamba-2.0.1/neo3/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/contracts/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/contracts/callflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/contracts/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/contracts/findoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/contracts/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/contracts/nef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/contracts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.077331 neo-mamba-2.0.1/neo3/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.077331 neo-mamba-2.0.1/neo3/core/cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/cryptography/bloomfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/cryptography/ecc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/cryptography/merkletree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.077331 neo-mamba-2.0.1/neo3/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/types/uint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.081331 neo-mamba-2.0.1/neo3/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.081331 neo-mamba-2.0.1/neo3/network/convenience/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/convenience/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/convenience/flightinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18614 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/convenience/nodemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/convenience/nodeweight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/convenience/requestinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/convenience/syncmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/ipfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27799 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.085331 neo-mamba-2.0.1/neo3/network/payloads/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/extensible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27818 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/payloads/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/network/relaycache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26371 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.085331 neo-mamba-2.0.1/neo3/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/wallet/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/wallet/scrypt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/wallet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/wallet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/neo3/wallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.085331 neo-mamba-2.0.1/neo_mamba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-22 11:33:48.000000 neo-mamba-2.0.1/neo_mamba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-22 11:33:48.000000 neo-mamba-2.0.1/neo_mamba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 11:33:48.000000 neo-mamba-2.0.1/neo_mamba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 11:33:47.000000 neo-mamba-2.0.1/neo_mamba.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-22 11:33:48.000000 neo-mamba-2.0.1/neo_mamba.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 11:33:48.000000 neo-mamba-2.0.1/neo_mamba.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-22 11:33:48.097331 neo-mamba-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.085331 neo-mamba-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.089331 neo-mamba-2.0.1/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/api/test_noderpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.089331 neo-mamba-2.0.1/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/contracts/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/contracts/test_callflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/contracts/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/contracts/test_contractstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20522 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/contracts/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/contracts/test_nef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/contracts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.089331 neo-mamba-2.0.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/core/test_biginteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/core/test_cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/core/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/core/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/core/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.093331 neo-mamba-2.0.1/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.093331 neo-mamba-2.0.1/tests/network/convenience/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/convenience/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/convenience/test_nodemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/convenience/test_syncmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/convenience/test_various.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/test_ipfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61223 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/network/test_witnessrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/test_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:48.097331 neo-mamba-2.0.1/tests/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/wallet/rc2-wallet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/wallet/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-22 11:33:27.000000 neo-mamba-2.0.1/tests/wallet/test_wallet.py
```

### Comparing `neo-mamba-2.0.0/CHANGELOG.rst` & `neo-mamba-2.0.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/LICENSE.md` & `neo-mamba-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/Makefile` & `neo-mamba-2.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/PKG-INFO` & `neo-mamba-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-mamba
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python SDK for the NEO 3 blockchain
 Home-page: https://github.com/CityOfZion/neo-mamba
 Author: Erik van den Brink
 Author-email: erik@coz.io
 Maintainer: Erik van den Brink
 Maintainer-email: erik@coz.io
 License: MIT License
```

### Comparing `neo-mamba-2.0.0/README.rst` & `neo-mamba-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/docs/source/faq.md` & `neo-mamba-2.0.1/docs/source/faq.md`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/docs/source/getting-started.md` & `neo-mamba-2.0.1/docs/source/getting-started.md`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/docs/source/home.html` & `neo-mamba-2.0.1/docs/source/home.html`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/docs/source/mamba-logo.png` & `neo-mamba-2.0.1/docs/source/mamba-logo.png`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/docs/source/smart-contracts.md` & `neo-mamba-2.0.1/docs/source/smart-contracts.md`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/docs/source/wrapper-hierarchy.png` & `neo-mamba-2.0.1/docs/source/wrapper-hierarchy.png`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/__init__.py` & `neo-mamba-2.0.1/examples/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/coz-wallet.json` & `neo-mamba-2.0.1/examples/shared/coz-wallet.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/default.neo-express` & `neo-mamba-2.0.1/examples/shared/default.neo-express`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.manifest.json` & `neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v1.manifest.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.py` & `neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v1.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.manifest.json` & `neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v2.manifest.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.py` & `neo-mamba-2.0.1/examples/shared/deploy-update-destroy/contract_v2.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/nep11-token/nep11-token.manifest.json` & `neo-mamba-2.0.1/examples/shared/nep11-token/nep11-token.manifest.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/nep11-token/nep11-token.nef` & `neo-mamba-2.0.1/examples/shared/nep11-token/nep11-token.nef`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/nep11-token/nft.go` & `neo-mamba-2.0.1/examples/shared/nep11-token/nft.go`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/nep11-token/nft.yml` & `neo-mamba-2.0.1/examples/shared/nep11-token/nft.yml`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.manifest.json` & `neo-mamba-2.0.1/examples/shared/nep17-token/nep17token.manifest.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.nef` & `neo-mamba-2.0.1/examples/shared/nep17-token/nep17token.nef`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.py` & `neo-mamba-2.0.1/examples/shared/nep17-token/nep17token.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/examples/shared/user-wallet.json` & `neo-mamba-2.0.1/examples/shared/user-wallet.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/api/helpers/signing.py` & `neo-mamba-2.0.1/neo3/api/helpers/signing.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/api/helpers/txbuilder.py` & `neo-mamba-2.0.1/neo3/api/helpers/txbuilder.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/api/helpers/unwrap.py` & `neo-mamba-2.0.1/neo3/api/helpers/unwrap.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/api/noderpc.py` & `neo-mamba-2.0.1/neo3/api/noderpc.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/api/wrappers.py` & `neo-mamba-2.0.1/neo3/api/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         self.notification_processor = None
 
     def __call__(self, *args, **kwargs):
         pass
 
 
 _DEFAULT_MAINNET_RPC = "http://seed1.neo.org:10332"
-_DEFAULT_TESTNET_RPC = "http://seed1t5.neo.org:10332"
+_DEFAULT_TESTNET_RPC = "http://seed1t5.neo.org:20332"
 
 SigningPair: TypeAlias = tuple[signing.SigningFunction, verification.Signer]
 
 
 @dataclass
 class InvokeReceipt(Generic[ReturnType]):
     """
```

### Comparing `neo-mamba-2.0.0/neo3/contracts/abi.py` & `neo-mamba-2.0.1/neo3/contracts/abi.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/contracts/callflags.py` & `neo-mamba-2.0.1/neo3/contracts/callflags.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/contracts/contract.py` & `neo-mamba-2.0.1/neo3/contracts/contract.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/contracts/findoptions.py` & `neo-mamba-2.0.1/neo3/contracts/findoptions.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/contracts/manifest.py` & `neo-mamba-2.0.1/neo3/contracts/manifest.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/contracts/nef.py` & `neo-mamba-2.0.1/neo3/contracts/nef.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/contracts/utils.py` & `neo-mamba-2.0.1/neo3/contracts/utils.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/core/cryptography/__init__.py` & `neo-mamba-2.0.1/neo3/core/cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/core/cryptography/bloomfilter.py` & `neo-mamba-2.0.1/neo3/core/cryptography/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/core/cryptography/ecc.py` & `neo-mamba-2.0.1/neo3/core/cryptography/ecc.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/core/cryptography/merkletree.py` & `neo-mamba-2.0.1/neo3/core/cryptography/merkletree.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/core/serialization.py` & `neo-mamba-2.0.1/neo3/core/serialization.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/core/types/uint.py` & `neo-mamba-2.0.1/neo3/core/types/uint.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/core/utils.py` & `neo-mamba-2.0.1/neo3/core/utils.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/capabilities.py` & `neo-mamba-2.0.1/neo3/network/capabilities.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/convenience/flightinfo.py` & `neo-mamba-2.0.1/neo3/network/convenience/flightinfo.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/convenience/nodemanager.py` & `neo-mamba-2.0.1/neo3/network/convenience/nodemanager.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/convenience/nodeweight.py` & `neo-mamba-2.0.1/neo3/network/convenience/nodeweight.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/convenience/requestinfo.py` & `neo-mamba-2.0.1/neo3/network/convenience/requestinfo.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/convenience/syncmanager.py` & `neo-mamba-2.0.1/neo3/network/convenience/syncmanager.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/ipfilter.py` & `neo-mamba-2.0.1/neo3/network/ipfilter.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/message.py` & `neo-mamba-2.0.1/neo3/network/message.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/node.py` & `neo-mamba-2.0.1/neo3/network/node.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/address.py` & `neo-mamba-2.0.1/neo3/network/payloads/address.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/block.py` & `neo-mamba-2.0.1/neo3/network/payloads/block.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/consensus.py` & `neo-mamba-2.0.1/neo3/network/payloads/consensus.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/extensible.py` & `neo-mamba-2.0.1/neo3/network/payloads/extensible.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/filter.py` & `neo-mamba-2.0.1/neo3/network/payloads/filter.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/inventory.py` & `neo-mamba-2.0.1/neo3/network/payloads/inventory.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/ping.py` & `neo-mamba-2.0.1/neo3/network/payloads/ping.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/transaction.py` & `neo-mamba-2.0.1/neo3/network/payloads/transaction.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/verification.py` & `neo-mamba-2.0.1/neo3/network/payloads/verification.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/payloads/version.py` & `neo-mamba-2.0.1/neo3/network/payloads/version.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/network/relaycache.py` & `neo-mamba-2.0.1/neo3/network/relaycache.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/settings.py` & `neo-mamba-2.0.1/neo3/settings.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/singleton.py` & `neo-mamba-2.0.1/neo3/singleton.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/vm.py` & `neo-mamba-2.0.1/neo3/vm.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/wallet/account.py` & `neo-mamba-2.0.1/neo3/wallet/account.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/wallet/scrypt_parameters.py` & `neo-mamba-2.0.1/neo3/wallet/scrypt_parameters.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/wallet/utils.py` & `neo-mamba-2.0.1/neo3/wallet/utils.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo3/wallet/wallet.py` & `neo-mamba-2.0.1/neo3/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/neo_mamba.egg-info/PKG-INFO` & `neo-mamba-2.0.1/neo_mamba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-mamba
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python SDK for the NEO 3 blockchain
 Home-page: https://github.com/CityOfZion/neo-mamba
 Author: Erik van den Brink
 Author-email: erik@coz.io
 Maintainer: Erik van den Brink
 Maintainer-email: erik@coz.io
 License: MIT License
```

### Comparing `neo-mamba-2.0.0/neo_mamba.egg-info/SOURCES.txt` & `neo-mamba-2.0.1/neo_mamba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/setup.cfg` & `neo-mamba-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.0.0
+current_version = 2.0.1
 commit = True
 tag = True
 
 [metadata]
 name = neo-mamba
 version = attr: neo3.__version__
 description = Python SDK for the NEO 3 blockchain
```

### Comparing `neo-mamba-2.0.0/tests/api/test_noderpc.py` & `neo-mamba-2.0.1/tests/api/test_noderpc.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/api/test_wrappers.py` & `neo-mamba-2.0.1/tests/api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/contracts/test_abi.py` & `neo-mamba-2.0.1/tests/contracts/test_abi.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/contracts/test_callflags.py` & `neo-mamba-2.0.1/tests/contracts/test_callflags.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/contracts/test_contract.py` & `neo-mamba-2.0.1/tests/contracts/test_contract.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/contracts/test_contractstate.py` & `neo-mamba-2.0.1/tests/contracts/test_contractstate.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/contracts/test_manifest.py` & `neo-mamba-2.0.1/tests/contracts/test_manifest.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/contracts/test_nef.py` & `neo-mamba-2.0.1/tests/contracts/test_nef.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/contracts/test_utils.py` & `neo-mamba-2.0.1/tests/contracts/test_utils.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/core/test_biginteger.py` & `neo-mamba-2.0.1/tests/core/test_biginteger.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/core/test_cryptography.py` & `neo-mamba-2.0.1/tests/core/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/core/test_serialization.py` & `neo-mamba-2.0.1/tests/core/test_serialization.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/core/test_types.py` & `neo-mamba-2.0.1/tests/core/test_types.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/core/test_utils.py` & `neo-mamba-2.0.1/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/convenience/test_nodemanager.py` & `neo-mamba-2.0.1/tests/network/convenience/test_nodemanager.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/convenience/test_syncmanager.py` & `neo-mamba-2.0.1/tests/network/convenience/test_syncmanager.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/convenience/test_various.py` & `neo-mamba-2.0.1/tests/network/convenience/test_various.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/test_capabilities.py` & `neo-mamba-2.0.1/tests/network/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/test_ipfilter.py` & `neo-mamba-2.0.1/tests/network/test_ipfilter.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/test_issues.py` & `neo-mamba-2.0.1/tests/network/test_issues.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/test_message.py` & `neo-mamba-2.0.1/tests/network/test_message.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/test_node.py` & `neo-mamba-2.0.1/tests/network/test_node.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/test_payloads.py` & `neo-mamba-2.0.1/tests/network/test_payloads.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/network/test_witnessrules.py` & `neo-mamba-2.0.1/tests/network/test_witnessrules.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/test_vm.py` & `neo-mamba-2.0.1/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/wallet/rc2-wallet.json` & `neo-mamba-2.0.1/tests/wallet/rc2-wallet.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/wallet/test_account.py` & `neo-mamba-2.0.1/tests/wallet/test_account.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-2.0.0/tests/wallet/test_wallet.py` & `neo-mamba-2.0.1/tests/wallet/test_wallet.py`

 * *Files identical despite different names*

