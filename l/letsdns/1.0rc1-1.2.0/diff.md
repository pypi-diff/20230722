# Comparing `tmp/letsdns-1.0rc1.tar.gz` & `tmp/letsdns-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsdns-1.0rc1.tar", last modified: Sat Apr  9 16:08:15 2022, max compression
+gzip compressed data, was "letsdns-1.2.0.tar", last modified: Sat Jul 22 00:03:15 2023, max compression
```

## Comparing `letsdns-1.0rc1.tar` & `letsdns-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2022-04-09 16:08:15.290328 letsdns-1.0rc1/
--rw-r--r--   0 ralph      (501) staff       (20)    35149 2022-01-10 09:27:40.000000 letsdns-1.0rc1/LICENSE
--rw-r--r--   0 ralph      (501) staff       (20)     1258 2022-04-09 16:08:15.290506 letsdns-1.0rc1/PKG-INFO
--rw-r--r--   0 ralph      (501) staff       (20)      476 2022-04-08 22:56:36.000000 letsdns-1.0rc1/README.md
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2022-04-09 16:08:15.286221 letsdns-1.0rc1/letsdns/
--rw-r--r--   0 ralph      (501) staff       (20)      764 2022-04-09 16:04:10.000000 letsdns-1.0rc1/letsdns/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     1707 2022-04-08 15:24:50.000000 letsdns-1.0rc1/letsdns/__main__.py
--rw-r--r--   0 ralph      (501) staff       (20)     3633 2022-03-07 20:55:43.000000 letsdns-1.0rc1/letsdns/action.py
--rw-r--r--   0 ralph      (501) staff       (20)     3991 2022-04-09 09:53:28.000000 letsdns-1.0rc1/letsdns/configuration.py
--rw-r--r--   0 ralph      (501) staff       (20)     2346 2022-04-03 13:25:33.000000 letsdns-1.0rc1/letsdns/core.py
--rw-r--r--   0 ralph      (501) staff       (20)     2150 2022-02-09 13:14:40.000000 letsdns-1.0rc1/letsdns/crypto.py
--rw-r--r--   0 ralph      (501) staff       (20)     5669 2022-04-03 15:21:34.000000 letsdns-1.0rc1/letsdns/hetznerapi.py
--rw-r--r--   0 ralph      (501) staff       (20)     2429 2022-04-03 15:21:34.000000 letsdns-1.0rc1/letsdns/liveupdate.py
--rw-r--r--   0 ralph      (501) staff       (20)     1675 2022-04-03 15:21:34.000000 letsdns-1.0rc1/letsdns/nsupdate.py
--rw-r--r--   0 ralph      (501) staff       (20)     2531 2022-04-09 14:22:42.000000 letsdns-1.0rc1/letsdns/tlsa.py
--rw-r--r--   0 ralph      (501) staff       (20)     2455 2022-04-03 15:21:34.000000 letsdns-1.0rc1/letsdns/util.py
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2022-04-09 16:08:15.287982 letsdns-1.0rc1/letsdns.egg-info/
--rw-r--r--   0 ralph      (501) staff       (20)     1258 2022-04-09 16:08:14.000000 letsdns-1.0rc1/letsdns.egg-info/PKG-INFO
--rw-r--r--   0 ralph      (501) staff       (20)      580 2022-04-09 16:08:15.000000 letsdns-1.0rc1/letsdns.egg-info/SOURCES.txt
--rw-r--r--   0 ralph      (501) staff       (20)        1 2022-04-09 16:08:14.000000 letsdns-1.0rc1/letsdns.egg-info/dependency_links.txt
--rw-r--r--   0 ralph      (501) staff       (20)       50 2022-04-09 16:08:15.000000 letsdns-1.0rc1/letsdns.egg-info/entry_points.txt
--rw-r--r--   0 ralph      (501) staff       (20)       32 2022-04-09 16:08:15.000000 letsdns-1.0rc1/letsdns.egg-info/requires.txt
--rw-r--r--   0 ralph      (501) staff       (20)       14 2022-04-09 16:08:15.000000 letsdns-1.0rc1/letsdns.egg-info/top_level.txt
--rw-r--r--   0 ralph      (501) staff       (20)       93 2022-04-03 12:58:41.000000 letsdns-1.0rc1/pyproject.toml
--rw-r--r--   0 ralph      (501) staff       (20)      897 2022-04-09 16:08:15.291275 letsdns-1.0rc1/setup.cfg
-drwxr-xr-x   0 ralph      (501) staff       (20)        0 2022-04-09 16:08:15.289997 letsdns-1.0rc1/tests/
--rw-r--r--   0 ralph      (501) staff       (20)     1720 2022-04-03 15:21:34.000000 letsdns-1.0rc1/tests/__init__.py
--rw-r--r--   0 ralph      (501) staff       (20)     1101 2022-03-07 15:29:37.000000 letsdns-1.0rc1/tests/actions.py
--rw-r--r--   0 ralph      (501) staff       (20)     3567 2022-04-03 13:25:33.000000 letsdns-1.0rc1/tests/test_action.py
--rw-r--r--   0 ralph      (501) staff       (20)     1852 2022-04-03 15:21:34.000000 letsdns-1.0rc1/tests/test_config.py
--rw-r--r--   0 ralph      (501) staff       (20)     1275 2022-04-03 15:21:34.000000 letsdns-1.0rc1/tests/test_hetzner.py
--rw-r--r--   0 ralph      (501) staff       (20)     4238 2022-04-09 14:22:42.000000 letsdns-1.0rc1/tests/test_tlsa.py
--rw-r--r--   0 ralph      (501) staff       (20)     1398 2022-04-03 15:21:34.000000 letsdns-1.0rc1/tests/test_util.py
+drwx------   0 ralph      (501) staff       (20)        0 2023-07-22 00:03:15.839229 letsdns-1.2.0/
+-rw-r--r--   0 ralph      (501) staff       (20)    35149 2022-01-10 09:27:40.000000 letsdns-1.2.0/LICENSE
+-rw-------   0 ralph      (501) staff       (20)     1238 2023-07-22 00:03:15.839544 letsdns-1.2.0/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      481 2023-01-13 18:37:38.000000 letsdns-1.2.0/README.md
+drwx------   0 ralph      (501) staff       (20)        0 2023-07-22 00:03:15.833857 letsdns-1.2.0/letsdns/
+-rw-------   0 ralph      (501) staff       (20)      768 2023-07-21 23:57:30.000000 letsdns-1.2.0/letsdns/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1712 2023-01-13 18:35:00.000000 letsdns-1.2.0/letsdns/__main__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     3638 2023-01-13 18:35:00.000000 letsdns-1.2.0/letsdns/action.py
+-rw-r--r--   0 ralph      (501) staff       (20)     3996 2023-01-13 18:35:00.000000 letsdns-1.2.0/letsdns/configuration.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2351 2023-01-13 18:35:00.000000 letsdns-1.2.0/letsdns/core.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2155 2023-01-13 18:35:00.000000 letsdns-1.2.0/letsdns/crypto.py
+-rw-r--r--   0 ralph      (501) staff       (20)     5674 2023-01-13 18:35:00.000000 letsdns-1.2.0/letsdns/hetznerapi.py
+-rw-------   0 ralph      (501) staff       (20)     2630 2023-07-21 23:57:31.000000 letsdns-1.2.0/letsdns/liveupdate.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1680 2023-01-13 18:35:00.000000 letsdns-1.2.0/letsdns/nsupdate.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2536 2023-01-13 18:35:00.000000 letsdns-1.2.0/letsdns/tlsa.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2462 2023-01-13 18:35:00.000000 letsdns-1.2.0/letsdns/util.py
+drwx------   0 ralph      (501) staff       (20)        0 2023-07-22 00:03:15.836239 letsdns-1.2.0/letsdns.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)     1238 2023-07-22 00:03:15.000000 letsdns-1.2.0/letsdns.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)      580 2023-07-22 00:03:15.000000 letsdns-1.2.0/letsdns.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2023-07-22 00:03:15.000000 letsdns-1.2.0/letsdns.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       50 2023-07-22 00:03:15.000000 letsdns-1.2.0/letsdns.egg-info/entry_points.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       32 2023-07-22 00:03:15.000000 letsdns-1.2.0/letsdns.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        8 2023-07-22 00:03:15.000000 letsdns-1.2.0/letsdns.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       93 2022-04-03 12:58:41.000000 letsdns-1.2.0/pyproject.toml
+-rw-------   0 ralph      (501) staff       (20)      950 2023-07-22 00:03:15.840394 letsdns-1.2.0/setup.cfg
+drwx------   0 ralph      (501) staff       (20)        0 2023-07-22 00:03:15.838905 letsdns-1.2.0/tests/
+-rw-r--r--   0 ralph      (501) staff       (20)     1725 2023-01-13 18:34:18.000000 letsdns-1.2.0/tests/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1106 2023-01-13 18:34:18.000000 letsdns-1.2.0/tests/actions.py
+-rw-r--r--   0 ralph      (501) staff       (20)     3572 2023-01-13 18:34:18.000000 letsdns-1.2.0/tests/test_action.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1912 2023-01-13 18:34:18.000000 letsdns-1.2.0/tests/test_config.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1280 2023-01-13 18:34:18.000000 letsdns-1.2.0/tests/test_hetzner.py
+-rw-r--r--   0 ralph      (501) staff       (20)     4310 2023-01-13 18:34:18.000000 letsdns-1.2.0/tests/test_tlsa.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1403 2023-01-13 18:34:18.000000 letsdns-1.2.0/tests/test_util.py
```

### Comparing `letsdns-1.0rc1/LICENSE` & `letsdns-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `letsdns-1.0rc1/PKG-INFO` & `letsdns-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: letsdns
-Version: 1.0rc1
+Version: 1.2.0
 Summary: Manage DANE TLSA records in DNS servers
 Home-page: https://letsdns.org
 Author: Ralph Seichter
 Author-email: author@letsdns.org
-License: UNKNOWN
 Project-URL: Documentation, https://letsdns.org
 Project-URL: Source, https://github.com/LetsDNS/letsdns
 Project-URL: Tracker, https://github.com/LetsDNS/letsdns/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -24,10 +22,8 @@
 
 Manage DANE TLSA records in DNS servers. Supports multiple domains with multiple TLS certificates each. LetsDNS can be
 invoked manually, from cron jobs, or called in hook functions of ACME-clients like [dehydrated](https://dehydrated.io)
 or [certbot](https://eff-certbot.readthedocs.io).
 
 Documentation is available on the [LetsDNS homepage](https://letsdns.org/).
 
-Copyright © 2022 Ralph Seichter. Hosted on [GitHub](https://github.com/LetsDNS/letsdns).
-
-
+Copyright © 2022-2023 Ralph Seichter. Hosted on [GitHub](https://github.com/LetsDNS/letsdns).
```

### Comparing `letsdns-1.0rc1/letsdns/__init__.py` & `letsdns-1.2.0/letsdns/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright © 2022 Ralph Seichter
+Copyright © 2022-2023 Ralph Seichter
 
 This file is part of LetsDNS.
 
 LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 General Public License as published by the Free Software Foundation, either version 3 of the
 License, or (at your option) any later version.
 
@@ -12,8 +12,8 @@
 General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with LetsDNS.
 If not, see <https://www.gnu.org/licenses/>.
 """
 HOMEPAGE = 'https://letsdns.org/'
 IDENTIFIER = 'letsdns'
-VERSION = '1.0.rc1'
+VERSION = '1.2.0'
```

### Comparing `letsdns-1.0rc1/letsdns/__main__.py` & `letsdns-1.2.0/letsdns/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/letsdns/action.py` & `letsdns-1.2.0/letsdns/action.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/letsdns/configuration.py` & `letsdns-1.2.0/letsdns/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/letsdns/core.py` & `letsdns-1.2.0/letsdns/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/letsdns/crypto.py` & `letsdns-1.2.0/letsdns/crypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/letsdns/hetznerapi.py` & `letsdns-1.2.0/letsdns/hetznerapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/letsdns/liveupdate.py` & `letsdns-1.2.0/letsdns/liveupdate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
@@ -14,14 +14,15 @@
 # If not, see <https://www.gnu.org/licenses/>.
 import json
 from _socket import gethostbyname
 from logging import debug
 
 from dns import query
 from dns import rcode
+from dns import tsig
 from dns import tsigkeyring
 from dns.message import Message
 from dns.update import Update
 
 from letsdns.action import Action
 from letsdns.configuration import Config
 from letsdns.tlsa import rdata_action_lifecycle
@@ -33,21 +34,23 @@
     @classmethod
     def lifecycle(cls, conf: Config, action: Action) -> int:
         return rdata_action_lifecycle(conf, action)
 
     def execute(self, conf: Config, *args, **kwargs) -> int:
         """Update DNS record using the dnspython library. Return 0 to indicate success."""
         zone = conf.get_mandatory('domain')
+        keyalgorithm = conf.get('key_algorithm', tsig.default_algorithm)
         path = conf.get('keyfile')
         if path:
+            debug(f'Key file: {path} (TSIG algorithm: {keyalgorithm})')
             with open(path, 'r') as f:
                 keyring = tsigkeyring.from_text(json.load(f))
         else:  # pragma: no cover
             keyring = None
-        update = Update(zone=zone, keyring=keyring)
+        update = Update(zone=zone, keyalgorithm=keyalgorithm, keyring=keyring)
         for port in conf.get_tcp_ports():
             name = record_name(conf, port)
             update.delete(name)
             dataset = kwargs['dataset']
             if len(dataset) > 0:
                 update.replace(name, dataset)
             nameserver = gethostbyname(conf.get_mandatory('nameserver'))
```

### Comparing `letsdns-1.0rc1/letsdns/nsupdate.py` & `letsdns-1.2.0/letsdns/nsupdate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/letsdns/tlsa.py` & `letsdns-1.2.0/letsdns/tlsa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/letsdns/util.py` & `letsdns-1.2.0/letsdns/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
@@ -43,14 +43,15 @@
     f = s[:1].lower()
     t = '1ty'.find(f)
     return t >= 0
 
 
 def getenv(name: str, default=None, debug_env=True):
     """Return environment variable value if available, otherwise return the default value.
+
     Args:
         name: Environment variable name.
         default: Default value.
         debug_env: Debug variable name/value.
     """
     if name in os.environ:
         value = os.environ[name]
```

### Comparing `letsdns-1.0rc1/letsdns.egg-info/PKG-INFO` & `letsdns-1.2.0/letsdns.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: letsdns
-Version: 1.0rc1
+Version: 1.2.0
 Summary: Manage DANE TLSA records in DNS servers
 Home-page: https://letsdns.org
 Author: Ralph Seichter
 Author-email: author@letsdns.org
-License: UNKNOWN
 Project-URL: Documentation, https://letsdns.org
 Project-URL: Source, https://github.com/LetsDNS/letsdns
 Project-URL: Tracker, https://github.com/LetsDNS/letsdns/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -24,10 +22,8 @@
 
 Manage DANE TLSA records in DNS servers. Supports multiple domains with multiple TLS certificates each. LetsDNS can be
 invoked manually, from cron jobs, or called in hook functions of ACME-clients like [dehydrated](https://dehydrated.io)
 or [certbot](https://eff-certbot.readthedocs.io).
 
 Documentation is available on the [LetsDNS homepage](https://letsdns.org/).
 
-Copyright © 2022 Ralph Seichter. Hosted on [GitHub](https://github.com/LetsDNS/letsdns).
-
-
+Copyright © 2022-2023 Ralph Seichter. Hosted on [GitHub](https://github.com/LetsDNS/letsdns).
```

### Comparing `letsdns-1.0rc1/letsdns.egg-info/SOURCES.txt` & `letsdns-1.2.0/letsdns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `letsdns-1.0rc1/setup.cfg` & `letsdns-1.2.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 [metadata]
 author = Ralph Seichter
 author_email = author@letsdns.org
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.7
 	Topic :: System :: Systems Administration
 	Topic :: Utilities
 description = Manage DANE TLSA records in DNS servers
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = letsdns
 project_urls = 
 	Documentation = https://letsdns.org
 	Source = https://github.com/LetsDNS/letsdns
 	Tracker = https://github.com/LetsDNS/letsdns/issues
 url = https://letsdns.org
-version = 1.0.rc1
+version = 1.2.0
 
 [options]
 install_requires = 
 	cryptography
 	dnspython
 	requests
 packages = find:
 python_requires = >=3.7
 
 [options.entry_points]
 console_scripts = 
 	letsdns = letsdns.__main__:main
 
+[options.packages.find]
+exclude = tests*
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `letsdns-1.0rc1/tests/__init__.py` & `letsdns-1.2.0/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright © 2022 Ralph Seichter
+Copyright © 2022-2023 Ralph Seichter
 
 This file is part of LetsDNS.
 
 LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 General Public License as published by the Free Software Foundation, either version 3 of the
 License, or (at your option) any later version.
```

### Comparing `letsdns-1.0rc1/tests/actions.py` & `letsdns-1.2.0/tests/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/tests/test_action.py` & `letsdns-1.2.0/tests/test_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/tests/test_config.py` & `letsdns-1.2.0/tests/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
 # LetsDNS is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with LetsDNS.
 # If not, see <https://www.gnu.org/licenses/>.
+import filecmp
 import logging
 import os
-import subprocess
 from configparser import NoOptionError
 from tempfile import NamedTemporaryFile
 
 import tests
 from letsdns.configuration import Config
 from letsdns.configuration import log_level
 
@@ -30,22 +30,23 @@
             log_level()
 
     def test_loglevel_good(self):
         os.environ['LOG_LEVEL'] = 'FATAL'
         self.assertEqual(logging.FATAL, log_level())
 
     def test_dump(self):
-        conf = Config()
-        conf.init()
+        c = Config()
+        c.init()
         f = NamedTemporaryFile(mode='wt', delete=False)
-        conf.dump(f)
+        c.dump(f)
         f.close()
-        diff = subprocess.run(['diff', 'dump-expected', f.name])
+        p = os.path.join(os.path.dirname(__file__), 'dump-expected')
+        x = filecmp.cmp(p, f.name, shallow=False)
         os.unlink(f.name)
-        self.assertEqual(0, diff.returncode)
+        self.assertTrue(x, msg='Dumped content differs')
 
     def test_get_domain(self):
         self.c.active_section = 'DEFAULT'
         with self.assertRaises(NoOptionError):
             self.c.get_domain()
 
     def test_options(self):
```

### Comparing `letsdns-1.0rc1/tests/test_hetzner.py` & `letsdns-1.2.0/tests/test_hetzner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `letsdns-1.0rc1/tests/test_tlsa.py` & `letsdns-1.2.0/tests/test_tlsa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
@@ -51,14 +51,15 @@
         self.c.active_section = 'tlsa'
         rd = from_text(RdataClass.IN, RdataType.TLSA, tok='3 1 1 1234')
         ds = Rdataset(RdataClass.IN, RdataType.TLSA, ttl=3)
         ds.add(rd)
         rc = self.update.execute(self.c, name='test', dataset=ds)
         self.assertEqual(0, rc)
 
+    @skipUnless(ENABLE_LIVEUPDATE_TESTS, 'online tests disabled')
     def test_bad_ttl(self):
         self.c.active_section = 'bad_ttl'
         rd = from_text(RdataClass.IN, RdataType.TLSA, tok='2 0 1 abcd')
         ds = Rdataset(RdataClass.IN, RdataType.TLSA, ttl=-3)
         ds.add(rd)
         with self.assertRaises(struct.error):
             self.update.execute(self.c, name='test', dataset=ds)
```

### Comparing `letsdns-1.0rc1/tests/test_util.py` & `letsdns-1.2.0/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Ralph Seichter
+# Copyright © 2022-2023 Ralph Seichter
 #
 # This file is part of LetsDNS.
 #
 # LetsDNS is free software: you can redistribute it and/or modify it under the terms of the GNU
 # General Public License as published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

