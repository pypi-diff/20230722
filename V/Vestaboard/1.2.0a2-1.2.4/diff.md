# Comparing `tmp/Vestaboard-1.2.0a2.tar.gz` & `tmp/Vestaboard-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vestaboard-1.2.0a2.tar", last modified: Mon Aug  1 00:00:15 2022, max compression
+gzip compressed data, was "Vestaboard-1.2.4.tar", last modified: Sat Jul 22 01:06:12 2023, max compression
```

## Comparing `Vestaboard-1.2.0a2.tar` & `Vestaboard-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 ShaneSutro   (501) staff       (20)        0 2022-08-01 00:00:15.805480 Vestaboard-1.2.0a2/
--rw-r--r--   0 ShaneSutro   (501) staff       (20)     1068 2021-02-09 00:42:34.000000 Vestaboard-1.2.0a2/LICENSE
--rw-r--r--   0 ShaneSutro   (501) staff       (20)    12077 2022-08-01 00:00:15.804654 Vestaboard-1.2.0a2/PKG-INFO
--rw-r--r--   0 ShaneSutro   (501) staff       (20)    11508 2022-07-29 22:10:23.000000 Vestaboard-1.2.0a2/README.md
-drwxr-xr-x   0 ShaneSutro   (501) staff       (20)        0 2022-08-01 00:00:15.799244 Vestaboard-1.2.0a2/Vestaboard.egg-info/
--rw-r--r--   0 ShaneSutro   (501) staff       (20)    12077 2022-08-01 00:00:15.000000 Vestaboard-1.2.0a2/Vestaboard.egg-info/PKG-INFO
--rw-r--r--   0 ShaneSutro   (501) staff       (20)      457 2022-08-01 00:00:15.000000 Vestaboard-1.2.0a2/Vestaboard.egg-info/SOURCES.txt
--rw-r--r--   0 ShaneSutro   (501) staff       (20)        1 2022-08-01 00:00:15.000000 Vestaboard-1.2.0a2/Vestaboard.egg-info/dependency_links.txt
--rw-r--r--   0 ShaneSutro   (501) staff       (20)        9 2022-08-01 00:00:15.000000 Vestaboard-1.2.0a2/Vestaboard.egg-info/requires.txt
--rw-r--r--   0 ShaneSutro   (501) staff       (20)       11 2022-08-01 00:00:15.000000 Vestaboard-1.2.0a2/Vestaboard.egg-info/top_level.txt
--rw-r--r--   0 ShaneSutro   (501) staff       (20)       38 2022-08-01 00:00:15.805846 Vestaboard-1.2.0a2/setup.cfg
--rw-r--r--   0 ShaneSutro   (501) staff       (20)      817 2022-07-31 23:54:05.000000 Vestaboard-1.2.0a2/setup.py
-drwxr-xr-x   0 ShaneSutro   (501) staff       (20)        0 2022-08-01 00:00:15.802474 Vestaboard-1.2.0a2/vestaboard/
--rw-r--r--   0 ShaneSutro   (501) staff       (20)    17191 2022-07-31 23:21:13.000000 Vestaboard-1.2.0a2/vestaboard/__init__.py
--rw-r--r--   0 ShaneSutro   (501) staff       (20)     2046 2022-07-30 18:58:31.000000 Vestaboard-1.2.0a2/vestaboard/characters.py
--rw-r--r--   0 ShaneSutro   (501) staff       (20)     4445 2022-07-31 22:13:19.000000 Vestaboard-1.2.0a2/vestaboard/formatter.py
--rw-r--r--   0 ShaneSutro   (501) staff       (20)      268 2022-07-31 22:26:58.000000 Vestaboard-1.2.0a2/vestaboard/vbUrls.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2023-07-22 01:06:12.151247 Vestaboard-1.2.4/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1068 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/LICENSE
+-rw-rw-r--   0 travis    (1000) travis    (1000)    17564 2023-07-22 01:06:12.151247 Vestaboard-1.2.4/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)    17016 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/README.md
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2023-07-22 01:06:12.151247 Vestaboard-1.2.4/Vestaboard.egg-info/
+-rw-rw-r--   0 travis    (1000) travis    (1000)    17564 2023-07-22 01:06:12.000000 Vestaboard-1.2.4/Vestaboard.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)      398 2023-07-22 01:06:12.000000 Vestaboard-1.2.4/Vestaboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2023-07-22 01:06:12.000000 Vestaboard-1.2.4/Vestaboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        9 2023-07-22 01:06:12.000000 Vestaboard-1.2.4/Vestaboard.egg-info/requires.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)       11 2023-07-22 01:06:12.000000 Vestaboard-1.2.4/Vestaboard.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)       38 2023-07-22 01:06:12.151247 Vestaboard-1.2.4/setup.cfg
+-rw-rw-r--   0 travis    (1000) travis    (1000)      816 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/setup.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2023-07-22 01:06:12.151247 Vestaboard-1.2.4/tests/
+-rw-rw-r--   0 travis    (1000) travis    (1000)    14769 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/tests/test_formatting.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    10592 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/tests/test_init.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4445 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/tests/test_localApi.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2582 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/tests/test_readWrite.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      270 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/tests/test_urls.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2023-07-22 01:06:12.151247 Vestaboard-1.2.4/vestaboard/
+-rw-rw-r--   0 travis    (1000) travis    (1000)    19863 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/vestaboard/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2098 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/vestaboard/characters.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     8359 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/vestaboard/formatter.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      268 2023-07-22 01:05:09.000000 Vestaboard-1.2.4/vestaboard/vbUrls.py
```

### Comparing `Vestaboard-1.2.0a2/LICENSE` & `Vestaboard-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Vestaboard-1.2.0a2/setup.py` & `Vestaboard-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Vestaboard",
-    version="1.2.0a2",
+    version="1.2.4",
     author="Shane Sutro",
     author_email="shane@shanesutro.com",
     description="A Vestaboard Wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/SonicRift/Vestaboard.git",
+    url="https://github.com/ShaneSutro/Vestaboard.git",
     packages=setuptools.find_packages(),
     license="MIT",
     install_requires=[
         'requests'
     ],
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `Vestaboard-1.2.0a2/vestaboard/__init__.py` & `Vestaboard-1.2.4/vestaboard/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 """Vestaboard Module
 
 A lightweight wrapper for Vestaboard
 
 Board - Class
 Installable - Class
 """
+import warnings
+import json
 import requests
 from vestaboard.formatter import Formatter
 import vestaboard.vbUrls as vbUrls
-import warnings
-import json
-import os
 
 
 class Board:
     def __init__(
         self,
         installable=False,
         apiKey=False,
         apiSecret=False,
         subscriptionId=False,
         localApi: dict = None,
         readWrite: bool = False,
+        validateKey: bool = False,
     ):
         """
         Returns an instance of Board().
 
         Args:
         installable - an instance of installable()
         apiKey - your Vestaboard API Key
         apiSecret - your Vestaboard API Secret
         subscriptionId - your Subscription ID (this can be obtained for you by creating a new installable() instance)
+        readWrite - pass True to create a new instance of Read/Write Board
+        validateKey - Read/Write & Local API only - sends a GET request to validate the API key and raises an error if the key is invalid
 
         Keyword Args:
         localApi = {
           'key': str - your local API key
           'ip': str - your boards local IP address
           'useSavedToken': bool - use saved token instead of provided key and IP
           'saveToken': bool - used alongside the enablement token to store your credentials. Defaults to True
@@ -49,14 +51,15 @@
                 f'Expected the first argument passed to be an instance of Installable, but instead got {type(installable)}. If you are not trying to pass an Installable, specify the name of the arguments, or pass "None" as the first argument.'
             )
 
         self.localOptions = localApi
         self.localKey = ""
         self.localIP = ""
         self.readWrite = readWrite
+        self.validateKey = validateKey
 
         if self.localOptions is not None:
             if self.checkAndEnableLocalAPI():
                 return
             if len(self.localOptions) < 2:
                 if (
                     "useSavedToken" in self.localOptions
@@ -66,73 +69,104 @@
                     self.localKey = token[0]
                     self.localIP = token[1]
                 else:
                     raise ValueError(
                         "Either the local API key or your board's IP address was not provided. If you have saved credentials, pass `useSavedToken` to use those credentials instead."
                     )
             else:
-                self.localKey = localApi["key"]
-                self.localIP = localApi["ip"]
+                if (
+                    "useSavedToken" in self.localOptions
+                    and self.localOptions["useSavedToken"]
+                ):
+                    token = get_local_token()
+                    self.localKey = token[0]
+                    self.localIP = token[1]
+                    if "ip" in self.localOptions and self.localOptions["ip"]:
+                        self.localIP = self.localOptions["ip"]
+                else:
+                    self.localKey = localApi["key"]
+                    self.localIP = localApi["ip"]
+            if self.validateKey:
+                self.read()
             return
 
         if not installable:  # check for cred file
             if readWrite:
                 if not apiKey:
                     try:
                         creds = get_creds()
                         if len(creds) < 2:
                             raise ValueError(
                                 "You must supply a read/write enabled API key to use readWrite mode, or instantiate an Installable in readWrite mode to store your credentials."
                             )
-                        else:
-                            self.apiKey = creds[0]
-                    except FileNotFoundError as e:
+                        self.apiKey = creds[0]
+                        if self.validateKey:
+                            self.read()
+                    except FileNotFoundError as exc:
                         raise FileNotFoundError(
                             "I couldn't find any saved credentials, and no API key was provided.\nTo use readWrite mode, you must supply a read/write enabled API key, or instantiate an Installable in readWrite mode."
-                        ) from e
+                        ) from exc
                 else:
                     self.apiKey = apiKey
+                    if self.validateKey:
+                        self.read()
                     return
             if not apiKey or not apiSecret or not subscriptionId:
                 try:
                     creds = get_creds()
                     if len(creds) == 3:
                         self.apiKey = creds[0]
                         self.apiSecret = creds[1]
                         self.subscriptionId = creds[2]
                     elif len(creds) < 3 or len(creds) > 3:
                         raise ValueError(
                             "Credentials have been saved, but one or more are missing. Create a new installable and pass in saveCredentials=True, or pass in all three parameters when initializing a new Board."
                         )
-                except FileNotFoundError as e:
+                except FileNotFoundError as exc:
                     raise ValueError(
                         "You must create an installable first or save credentials by passing saveCredentials=True into installable()."
-                    ) from e
+                    ) from exc
             else:
                 self.apiKey = apiKey
                 self.apiSecret = apiSecret
                 self.subscriptionId = subscriptionId
         else:
             self.apiKey = installable.apiKey
             self.apiSecret = installable.apiSecret
             self.subscriptionId = installable.subscriptionId or subscriptionId
 
     def post(self, text):
         if self.localOptions:
             self._post_local(text)
             return
 
+        if self.readWrite:
+            if not isinstance(text, str):
+                raise ValueError(
+                    "The `post()` method expects a plain string - if your characters are already converted, use the `raw()` method instead."
+                )
+            headers = {"X-Vestaboard-Read-Write-Key": self.apiKey}
+            fm = Formatter()
+            self.raw(
+                fm.convertPlainText(text, justify="left", useVestaboardCentering=True)
+            )
+            return
+
         headers = {
             "X-Vestaboard-Api-Key": self.apiKey,
             "X-Vestaboard-Api-Secret": self.apiSecret,
         }
         finalText = Formatter()._standard(text)
-        requests.post(
-            vbUrls.post.format(self.subscriptionId), headers=headers, json=finalText
+        req = requests.post(
+            vbUrls.post.format(self.subscriptionId),
+            headers=headers,
+            json=finalText,
+            timeout=5,
         )
+        req.raise_for_status()
 
     def raw(self, charList: list, pad=None):
         """
         Posts already-formatted characters to the board.
 
         Keyword arguments:
 
@@ -180,57 +214,61 @@
             self._raw_local(finalText["characters"])
         elif self.readWrite and self.apiKey:
             headers = {"X-Vestaboard-Read-Write-Key": self.apiKey}
             requests.post(
                 vbUrls.readWrite,
                 headers=headers,
                 data=json.dumps(finalText["characters"]),
+                timeout=5,
             )
         else:
             headers = {
                 "X-Vestaboard-Api-Key": self.apiKey,
                 "X-Vestaboard-Api-Secret": self.apiSecret,
             }
             requests.post(
-                vbUrls.post.format(self.subscriptionId), headers=headers, json=finalText
+                vbUrls.post.format(self.subscriptionId),
+                headers=headers,
+                json=finalText,
+                timeout=5,
             )
 
     def _enableLocalApi(
         self, enablementKey: str = "", boardIP: str = "", saveToFile: bool = True
     ):
         headers = {"X-Vestaboard-Local-Api-Enablement-Token": enablementKey}
         try:
             response = requests.post(
-                vbUrls.enableLocal.format(boardIP), headers=headers
+                vbUrls.enableLocal.format(boardIP), headers=headers, timeout=5
             )
             if not response.ok:
                 print(
                     "Looks like that didn't work. The Vestaboard returned the following message:\n",
                     response.text,
                 )
             else:
                 parsed = response.json()
                 self.localOptions = {"useSavedToken": True}
                 self.localIP = boardIP
                 self.localKey = parsed["apiKey"]
                 print("Success! Here's your local API token:\n", parsed["apiKey"])
                 if saveToFile:
-                    with open("./local.txt", "w") as local:
+                    with open("./local.txt", "w", encoding="UTF-8") as local:
                         local.write(parsed["apiKey"])
                         local.write("\n")
                         local.write(boardIP)
                         print(
                             "Saved to ./local.txt! This instance of Board can now be used with the local API, or pass the `localApi={'useSavedToken': True}` when instantiating a new Board to use your saved credentials."
                         )
                         local.close()
         except OSError as e:
             raise ConnectionError(
                 "I couldn't connect to your board. Are you on the same network as the board you're trying to connect to?",
                 e,
-            )
+            ) from e
 
     def checkAndEnableLocalAPI(self):
         if "enablementToken" not in self.localOptions:
             return False
         elif "ip" not in self.localOptions:
             raise ValueError(
                 "Looks like you're trying to enable your board's local API, but your board's IP was not passed in.\nSupply both the enablement token from Vestaboard and your board's local IP address and try again with just the key and IP."
@@ -247,69 +285,83 @@
             )
             return True
         self._enableLocalApi(
             self.localOptions["enablementToken"], self.localOptions["ip"]
         )
         return True
 
-    def read(self, options: dict = {}):
+    def read(self, options: dict = None):
+        if options is None:
+            options = {}
         if not self.readWrite:
-            if self.localOptions is None or "useSavedToken" not in self.localOptions:
+            if self.localOptions is None or (
+                "useSavedToken" not in self.localOptions
+                and "key" not in self.localOptions
+            ):
                 raise ValueError(
                     '.read() is only available when using local API or by using a read/write enabled API key.\nPass "readWrite=True" along with your apiKey to enable readWrite mode.'
                 )
         if self.localIP and self.localKey:
             localHeader = {"X-Vestaboard-Local-Api-Key": self.localKey}
             res = requests.get(
-                vbUrls.postLocal.format(self.localIP), headers=localHeader
+                vbUrls.postLocal.format(self.localIP), headers=localHeader, timeout=5
             )
+            res.raise_for_status()
+            if res.text == "" and not self.validateKey:
+                warnings.warn(
+                    "The request succeeded, but I didn't get any text back from your board. If your board is currently displaying a message and this is unexpected, ensure you are using a valid local API key rather than a regular API key from Vestaboard's website."
+                )
+                return
+            elif res.text == "" and self.validateKey:
+                warnings.warn(
+                    "This API key appears to be invalid; I recieved an empty string from your board. If your board is not currently blank, double check your API key, or pass in your enablement token again to get a new API key."
+                )
+                return
             response_text = res.json()["message"]
         elif self.readWrite and self.apiKey:
             readWriteHeader = {"X-Vestaboard-Read-Write-Key": self.apiKey}
-            res = requests.get(vbUrls.readWrite, headers=readWriteHeader)
+            print("Getting board message")
+            res = requests.get(vbUrls.readWrite, headers=readWriteHeader, timeout=5)
+            res.raise_for_status()
             response_text = json.loads(res.json()["currentMessage"]["layout"])
         if "print" in options and options["print"]:
             print(res.json())
         if "convert" in options and options["convert"]:
             if "normalize" in options and options["normalize"]:
                 converted = Formatter()._reverse_convert(response_text, normalize=True)
                 return converted
             else:
                 converted = Formatter()._reverse_convert(response_text)
                 return converted
+        if self.validateKey:
+            print("Your API key appears to be valid!")
         return res.json()
 
     def _post_local(self, text):
-        print(
-            "Feature coming soon! For now, you can pass a pre-formatted message to your board by using the Board().raw() method."
-        )
-        return
-        print(self.localIP)
-        print(self.localKey)
         localHeader = {"X-Vestaboard-Local-Api-Key": self.localKey}
-        textArr = []
-        f = Formatter()
-        for i in range(0, 6):
-            textArr.append(f.convertLine(text))
-        finalText = f._raw(textArr)
-        print(finalText)
+        fm = Formatter()
+        convertedByDefault = fm.convertPlainText(text)
         res = requests.post(
             vbUrls.postLocal.format(self.localIP),
             headers=localHeader,
-            data=json.dumps(textArr),
+            data=json.dumps(convertedByDefault),
+            timeout=5,
         )
+        res.raise_for_status()
         print(res.text)
 
     def _raw_local(self, chars):
         localHeader = {"X-Vestaboard-Local-Api-Key": self.localKey}
         res = requests.post(
             vbUrls.postLocal.format(self.localIP),
             headers=localHeader,
             data=json.dumps(chars),
+            timeout=5,
         )
+        res.raise_for_status()
 
 
 class Installable:
     def __init__(
         self, apiKey=False, apiSecret=False, getSubscription=True, saveCredentials=True
     ):
         """
@@ -327,15 +379,15 @@
         self.apiSecret = apiSecret
         self.saveCredentials = saveCredentials
         if not apiKey or not apiSecret:
             raise ValueError(
                 "Installables must have an apiKey and apiSecret parameter."
             )
         if saveCredentials and apiKey and apiSecret:
-            with open("./credentials.txt", "w") as cred:
+            with open("./credentials.txt", "w", encoding="UTF-8") as cred:
                 cred.write(apiKey + "\n")
                 cred.write(apiSecret + "\n")
                 cred.close()
         if getSubscription:
             self.subscriptionId = self.get_subscriptions(saveCredentials)[0]["_id"]
         else:
             self.subscriptionId = False
@@ -345,44 +397,45 @@
             raise ValueError(
                 "There are no keys set. Call Installable(apiKey= apiSecret=) with your installable keys."
             )
         headers = {
             "X-Vestaboard-Api-Key": self.apiKey,
             "X-Vestaboard-Api-Secret": self.apiSecret,
         }
-        response = requests.get(vbUrls.subscription, headers=headers)
+        response = requests.get(vbUrls.subscription, headers=headers, timeout=5)
+        response.raise_for_status()
         if self.saveCredentials or save and response.status_code == 200:
-            with open("./credentials.txt", "a") as cred:
+            with open("./credentials.txt", "a", encoding="UTF-8") as cred:
                 cred.write(response.json()["subscriptions"][0]["_id"] + "\n")
                 cred.close()
 
         print("Subscription id(s):", response.json()["subscriptions"])
         return response.json()["subscriptions"]
 
 
 def get_creds():
-    with open("./credentials.txt", "r") as cred:
+    with open("./credentials.txt", "r", encoding="UTF-8") as cred:
         creds = cred.read().splitlines()
         return creds
 
 
 def get_local_token():
     try:
-        with open("./local.txt", "r") as local:
+        with open("./local.txt", "r", encoding="UTF-8") as local:
             token = local.read().splitlines()
             if len(token) == 0:
                 raise ValueError(
                     "Either your local token or IP was not passed in, and there's nothing stored.\nEither pass in a value for `localKey` and `localIP`, or store a copy of your local key and IP with the name 'local.txt.' Don't forget to include your board's IP address on line 2."
                 )
             elif len(token) == 1:
                 raise ValueError(
                     "Your local.txt file is missing either the local key or your board's IP address. Ensure your key is on line 1 and your IP is on line 2 and try again."
                 )
             elif len(token) > 2:
                 raise ValueError(
                     "Your local.txt file contains more than your key and IP (or has more than two lines of text). Please remove the extra key or line and try again. Your local.txt file should contain only the local key and board IP address, each on their own line."
                 )
             return (token[0], token[1])
-    except FileNotFoundError:
+    except FileNotFoundError as exc:
         raise FileNotFoundError(
             "I couldn't find any stored tokens. If you have already enabled your board's local API, you can pass in your board's IP and token in via the `localApi` dict, or pass in just the enablement token to get and store a new API token."
-        )
+        ) from exc
```

