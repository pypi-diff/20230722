# Comparing `tmp/aiodnsbl-0.1.1.tar.gz` & `tmp/aiodnsbl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodnsbl-0.1.1.tar", max compression
+gzip compressed data, was "aiodnsbl-1.0.0.tar", max compression
```

## Comparing `aiodnsbl-0.1.1.tar` & `aiodnsbl-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1070 2021-08-22 06:46:45.002704 aiodnsbl-0.1.1/LICENSE
--rw-r--r--   0        0        0     2154 2021-08-24 09:56:46.661735 aiodnsbl-0.1.1/README.md
--rw-r--r--   0        0        0      230 2021-10-08 21:44:25.940575 aiodnsbl-0.1.1/aiodnsbl/__init__.py
--rw-r--r--   0        0        0     5247 2021-08-24 13:25:32.674824 aiodnsbl-0.1.1/aiodnsbl/checker.py
--rw-r--r--   0        0        0      837 2021-08-24 09:49:01.964381 aiodnsbl-0.1.1/aiodnsbl/providers.py
--rw-r--r--   0        0        0      860 2021-10-08 21:44:25.942620 aiodnsbl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3033 2021-10-08 21:44:57.393551 aiodnsbl-0.1.1/setup.py
--rw-r--r--   0        0        0     2890 2021-10-08 21:44:57.393817 aiodnsbl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-22 05:55:23.298871 aiodnsbl-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2155 2023-07-22 05:55:23.298871 aiodnsbl-1.0.0/README.md
+-rw-r--r--   0        0        0      149 2023-07-22 05:55:23.298871 aiodnsbl-1.0.0/aiodnsbl/__init__.py
+-rw-r--r--   0        0        0     5183 2023-07-22 05:55:23.298871 aiodnsbl-1.0.0/aiodnsbl/checker.py
+-rw-r--r--   0        0        0      815 2023-07-22 05:55:23.298871 aiodnsbl-1.0.0/aiodnsbl/providers.py
+-rw-r--r--   0        0        0     1109 2023-07-22 05:55:42.811141 aiodnsbl-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 aiodnsbl-1.0.0/PKG-INFO
```

### Comparing `aiodnsbl-0.1.1/LICENSE` & `aiodnsbl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodnsbl-0.1.1/README.md` & `aiodnsbl-1.0.0/README.md`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -68,8 +68,8 @@
     # ['b.barracudacentral.org', 'bl.spamcop.net', 'dnsbl.sorbs.net', 'ips.backscatterer.org', ...]
     print([provider.host for provider in res.detected_by])
     # ['b.barracudacentral.org', 'dnsbl.sorbs.net', 'spam.dnsbl.sorbs.net', 'zen.spamhaus.org']
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
-```
+```
```

### Comparing `aiodnsbl-0.1.1/aiodnsbl/checker.py` & `aiodnsbl-1.0.0/aiodnsbl/checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,20 @@
     except ValueError:
         return False
 
 
 @functools.lru_cache(maxsize=256)
 def normalize_domain(value: str) -> str:
     value = value.lower()
-
     return idna.encode(value).decode()
 
 
-# regex taken from https://regexr.com/3abjr
+# https://regex101.com/r/vdrgm7/1
 DOMAIN_REGEX = re.compile(
-    r"^((?!-))(xn--)?[a-z0-9][a-z0-9-_]{0,61}[a-z0-9]{0,1}\.(xn--)?([a-z0-9\-]{1,61}|[a-z0-9-]{1,30}\.[a-z]{2,})$"
+    r"^(((?!-))(xn--|_{1,1})?[a-z0-9-]{0,61}[a-z0-9]{1,1}\.)*(xn--[a-z0-9][a-z0-9\-]{0,60}|[a-z0-9-]{1,30}\.[a-z]{2,})$"
 )
 
 
 @functools.lru_cache(maxsize=256)
 def is_domain(value: str) -> bool:
     value = normalize_domain(value)
     return DOMAIN_REGEX.match(value) is not None
@@ -130,44 +129,40 @@
         # select providers
         selected_providers: List[Provider] = []
         request_type = detect_request_type(request)
         for provider in self.providers:
             if provider.support_type == request_type:
                 selected_providers.append(provider)
 
-        tasks = []
-        for provider in selected_providers:
-            tasks.append(self.dnsbl_request(request, provider))
-
+        tasks = [
+            self.dnsbl_request(request, provider) for provider in selected_providers
+        ]
         responses = await asyncio.gather(*tasks)
         return DNSBLResult(address=request, responses=responses)
 
     async def check(self, request: str) -> DNSBLResult:
         return await self.check_async(request)
 
     async def bulk_check(self, requests: List[str]) -> List[DNSBLResult]:
-        tasks = []
-        for request in requests:
-            tasks.append(self.check_async(request))
-
+        tasks = [self.check_async(request) for request in requests]
         return await asyncio.gather(*tasks)
 
 
 class DNSBLChecker(BaseDNSBLChecker):
     def prepare_query(self, request: str) -> str:
         # check a request as an IP address
         if is_ip_address(request):
             address = ipaddress.ip_address(request)
             if address.version == 4:
                 return ".".join(reversed(request.split(".")))
 
             if address.version == 6:
                 # according to RFC: https://tools.ietf.org/html/rfc5782#section-2.4
                 request_stripped = request.replace(":", "")
-                return ".".join(reversed([x for x in request_stripped]))
+                return ".".join(reversed(list(request_stripped)))
 
             raise ValueError("Unknown ip version")
 
         domain = normalize_domain(request)
         if not is_domain(domain):
             raise ValueError(f"Should be a valid domain, got {domain}")
```

### Comparing `aiodnsbl-0.1.1/aiodnsbl/providers.py` & `aiodnsbl-1.0.0/aiodnsbl/providers.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 class Provider:
     host: str
     support_type: str = "ip"
 
 
 _BASE_PROVIDERS = [
     "b.barracudacentral.org",
-    "bl.spamcop.net",
     "dnsbl.sorbs.net",
     "ips.backscatterer.org",
     "psbl.surriel.com",
     "sbl.spamhaus.org",
     "spam.dnsbl.sorbs.net",
     "ubl.unsubscore.com",
     "xbl.spamhaus.org",
```

### Comparing `aiodnsbl-0.1.1/setup.py` & `aiodnsbl-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,95 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aiodnsbl
+Version: 1.0.0
+Summary: Async DNSBL lists checker
+Home-page: https://github.com/ninoseki/aiodnsbl
+License: MIT
+Author: Manabu Niseki
+Author-email: manabu.niseki@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiodns (>=3.0,<4.0)
+Requires-Dist: idna (>=3.4,<4.0)
+Project-URL: Repository, https://github.com/ninoseki/aiodnsbl
+Description-Content-Type: text/markdown
 
-packages = \
-['aiodnsbl']
+# aiodnsbl
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/aiodnsbl.svg)](https://badge.fury.io/py/aiodnsbl)
+[![Python CI](https://github.com/ninoseki/aiodnsbl/actions/workflows/test.yml/badge.svg)](https://github.com/ninoseki/aiodnsbl/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/ninoseki/aiodnsbl/badge.svg?branch=main)](https://coveralls.io/github/ninoseki/aiodnsbl?branch=main)
 
-install_requires = \
-['aiodns>=3.0.0,<4.0.0', 'idna>=3.2,<4.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=4.8.1,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'aiodnsbl',
-    'version': '0.1.1',
-    'description': 'Async DNSBL lists checker',
-    'long_description': '# aiodnsbl\n\n[![PyPI version](https://badge.fury.io/py/aiodnsbl.svg)](https://badge.fury.io/py/aiodnsbl)\n[![Python CI](https://github.com/ninoseki/aiodnsbl/actions/workflows/test.yml/badge.svg)](https://github.com/ninoseki/aiodnsbl/actions/workflows/test.yml)\n[![Coverage Status](https://coveralls.io/repos/github/ninoseki/aiodnsbl/badge.svg?branch=main)](https://coveralls.io/github/ninoseki/aiodnsbl?branch=main)\n\n[DNSBL](https://en.wikipedia.org/wiki/DNSBL) lists checker based on [aiodns](https://github.com/saghul/aiodns). Checks if an IP or a domain is listed on anti-spam DNS blacklists.\n\n## Notes\n\nThis is a fork of [pydnsbl](https://github.com/dmippolitov/pydnsbl).\n\nKey differences:\n\n- Fully type annotated\n- No sync wrapper (async only)\n- No category classification\n\n## Installation\n\n```bash\npip install aiodnsbl\n```\n\n## Usage\n\n```python\nimport asyncio\n\nfrom aiodnsbl import DNSBLChecker\n\n\nloop = asyncio.get_event_loop()\n\nchecker = DNSBLChecker()\n\n# Check IP\nloop.run_until_complete(checker.check("8.8.8.8"))\n# <DNSBLResult: 8.8.8.8  (0/10)>\nloop.run_until_complete(checker.check("68.128.212.240"))\n# <DNSBLResult: 68.128.212.240 [BLACKLISTED] (4/10)>\n\n# Check domain\nloop.run_until_complete(checker.check("example.com"))\n# <DNSBLResult: example.com  (0/4)>\n\n# Bulk check\nloop.run_until_complete(\n    checker.bulk_check(["example.com", "8.8.8.8", "68.128.212.240"])\n)\n# [<DNSBLResult: example.com  (0/4)>, <DNSBLResult: 8.8.8.8  (0/10)>, <DNSBLResult: 68.128.212.240 [BLACKLISTED] (4/10)>]\n```\n\n```python\nimport asyncio\n\nfrom aiodnsbl import DNSBLChecker\n\n\nasync def main():\n    checker = DNSBLChecker()\n    res = await checker.check("68.128.212.240")\n    print(res)\n    # <DNSBLResult: 68.128.212.240 [BLACKLISTED] (4/10)>\n    print(res.blacklisted)\n    # True\n    print([provider.host for provider in res.providers])\n    # [\'b.barracudacentral.org\', \'bl.spamcop.net\', \'dnsbl.sorbs.net\', \'ips.backscatterer.org\', ...]\n    print([provider.host for provider in res.detected_by])\n    # [\'b.barracudacentral.org\', \'dnsbl.sorbs.net\', \'spam.dnsbl.sorbs.net\', \'zen.spamhaus.org\']\n\n\nloop = asyncio.get_event_loop()\nloop.run_until_complete(main())\n```',
-    'author': 'Manabu Niseki',
-    'author_email': 'manabu.niseki@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ninoseki/aiodnsbl',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+[DNSBL](https://en.wikipedia.org/wiki/DNSBL) lists checker based on [aiodns](https://github.com/saghul/aiodns). Checks if an IP or a domain is listed on anti-spam DNS blacklists.
 
+## Notes
+
+This is a fork of [pydnsbl](https://github.com/dmippolitov/pydnsbl).
+
+Key differences:
+
+- Fully type annotated
+- No sync wrapper (async only)
+- No category classification
+
+## Installation
+
+```bash
+pip install aiodnsbl
+```
+
+## Usage
+
+```python
+import asyncio
+
+from aiodnsbl import DNSBLChecker
+
+
+loop = asyncio.get_event_loop()
+
+checker = DNSBLChecker()
+
+# Check IP
+loop.run_until_complete(checker.check("8.8.8.8"))
+# <DNSBLResult: 8.8.8.8  (0/10)>
+loop.run_until_complete(checker.check("68.128.212.240"))
+# <DNSBLResult: 68.128.212.240 [BLACKLISTED] (4/10)>
+
+# Check domain
+loop.run_until_complete(checker.check("example.com"))
+# <DNSBLResult: example.com  (0/4)>
+
+# Bulk check
+loop.run_until_complete(
+    checker.bulk_check(["example.com", "8.8.8.8", "68.128.212.240"])
+)
+# [<DNSBLResult: example.com  (0/4)>, <DNSBLResult: 8.8.8.8  (0/10)>, <DNSBLResult: 68.128.212.240 [BLACKLISTED] (4/10)>]
+```
+
+```python
+import asyncio
+
+from aiodnsbl import DNSBLChecker
+
+
+async def main():
+    checker = DNSBLChecker()
+    res = await checker.check("68.128.212.240")
+    print(res)
+    # <DNSBLResult: 68.128.212.240 [BLACKLISTED] (4/10)>
+    print(res.blacklisted)
+    # True
+    print([provider.host for provider in res.providers])
+    # ['b.barracudacentral.org', 'bl.spamcop.net', 'dnsbl.sorbs.net', 'ips.backscatterer.org', ...]
+    print([provider.host for provider in res.detected_by])
+    # ['b.barracudacentral.org', 'dnsbl.sorbs.net', 'spam.dnsbl.sorbs.net', 'zen.spamhaus.org']
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
 
-setup(**setup_kwargs)
```

