# Comparing `tmp/uploadserver-4.2.0.tar.gz` & `tmp/uploadserver-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadserver-4.2.0.tar", last modified: Sun Mar 12 17:02:22 2023, max compression
+gzip compressed data, was "uploadserver-5.0.0.tar", last modified: Sat Jul 22 20:07:33 2023, max compression
```

## Comparing `uploadserver-4.2.0.tar` & `uploadserver-5.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2023-03-12 17:02:22.038292 uploadserver-4.2.0/
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)     1066 2023-03-11 20:39:09.000000 uploadserver-4.2.0/LICENSE
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)     7647 2023-03-12 17:02:22.038292 uploadserver-4.2.0/PKG-INFO
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)     7186 2023-03-11 20:39:09.000000 uploadserver-4.2.0/README.md
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)       38 2023-03-12 17:02:22.038292 uploadserver-4.2.0/setup.cfg
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)      678 2023-03-12 16:55:41.000000 uploadserver-4.2.0/setup.py
-drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2023-03-12 17:02:22.038292 uploadserver-4.2.0/uploadserver/
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)    18055 2023-03-12 16:54:07.000000 uploadserver-4.2.0/uploadserver/__init__.py
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)       72 2023-03-11 20:39:09.000000 uploadserver-4.2.0/uploadserver/__main__.py
-drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2023-03-12 17:02:22.038292 uploadserver-4.2.0/uploadserver.egg-info/
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)     7647 2023-03-12 17:02:22.000000 uploadserver-4.2.0/uploadserver.egg-info/PKG-INFO
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)      220 2023-03-12 17:02:22.000000 uploadserver-4.2.0/uploadserver.egg-info/SOURCES.txt
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)        1 2023-03-12 17:02:22.000000 uploadserver-4.2.0/uploadserver.egg-info/dependency_links.txt
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)       13 2023-03-12 17:02:22.000000 uploadserver-4.2.0/uploadserver.egg-info/top_level.txt
+drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2023-07-22 20:07:33.439986 uploadserver-5.0.0/
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)     1066 2023-03-11 20:39:09.000000 uploadserver-5.0.0/LICENSE
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)     7226 2023-07-22 20:07:33.438986 uploadserver-5.0.0/PKG-INFO
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)     6765 2023-07-21 01:39:15.000000 uploadserver-5.0.0/README.md
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)       38 2023-07-22 20:07:33.439986 uploadserver-5.0.0/setup.cfg
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)      758 2023-07-22 20:03:59.000000 uploadserver-5.0.0/setup.py
+drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2023-07-22 20:07:33.438986 uploadserver-5.0.0/uploadserver/
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)    13441 2023-07-21 02:52:06.000000 uploadserver-5.0.0/uploadserver/__init__.py
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)       72 2023-03-11 20:39:09.000000 uploadserver-5.0.0/uploadserver/__main__.py
+drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2023-07-22 20:07:33.438986 uploadserver-5.0.0/uploadserver.egg-info/
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)     7226 2023-07-22 20:07:33.000000 uploadserver-5.0.0/uploadserver.egg-info/PKG-INFO
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)      259 2023-07-22 20:07:33.000000 uploadserver-5.0.0/uploadserver.egg-info/SOURCES.txt
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)        1 2023-07-22 20:07:33.000000 uploadserver-5.0.0/uploadserver.egg-info/dependency_links.txt
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)       51 2023-07-22 20:07:33.000000 uploadserver-5.0.0/uploadserver.egg-info/entry_points.txt
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)       13 2023-07-22 20:07:33.000000 uploadserver-5.0.0/uploadserver.egg-info/top_level.txt
```

### Comparing `uploadserver-4.2.0/LICENSE` & `uploadserver-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uploadserver-4.2.0/PKG-INFO` & `uploadserver-5.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: uploadserver
-Version: 4.2.0
+Version: 5.0.0
 Summary: Python's http.server extended to include a file upload page
 Home-page: https://github.com/Densaugeo/uploadserver
 Author: Densaugeo
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # uploadserver
 
 Python's http.server extended to include a file upload page
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://mit-license.org/)
 [![Build Status](https://travis-ci.com/Densaugeo/uploadserver.svg?branch=master)](https://travis-ci.com/github/Densaugeo/uploadserver)
 
 ## Supported Platforms
 
 | Platform | Supported? | Notes |
 |-|-|-|
-| Python 3.6+ | Yes | Tested on 3.6 through 3.12 every release. |
+| Python 3.8+ | Yes | Tested on 3.8 through 3.12 every release. |
+| Python 3.6-3.7 | No | Was supported by previous versions. |
 | Python 3.5- | No | |
 | Linux | Yes | Tested on Fedora and Ubuntu every release. |
 | Windows | Yes | Occasional manual testing. Haven't noticed any obvious problems. |
 | Mac | No idea | I don't have a Mac. Idk if it works or not. |
 
 ## Installation
 
@@ -73,30 +74,14 @@
 python3 -m uploadserver --basic-auth-upload hello:world
 ~~~
 
 The same as above, but authentication is only required for upload operations.
 
 If both --basic-auth and --basic-auth-upload are specified, first one will be used for downloads and the second one for uploads.
 
-## Token Option (deprecated, will be removed in future)
-
-Run with a simple token.
-~~~
-python3 -m uploadserver -t helloworld
-~~~
-
-Now you can upload a file with the token. For example:
-~~~
-curl -X POST http://127.0.0.1:8000/upload -F 'files=@token-example.txt' -F 'token=helloworld'
-~~~
-
-Uploads without the token will be rejected. Tokens can be stolen if sent in plain HTTP, so this option is best used with HTTPS.
-
-Note: The server cannot check the token until after a file has been transferred, due to the way HTML form uploads are formatted, which creates a DoS vulnerability. If this is a concern, use mTLS for client authentication instead of relying on tokens.
-
 ## Theme Option
 
 The upload page supports a dark mode for showing white text on black background. If no option is specified, the color scheme is chosen from the client’s browser’s preference (which typically matches their operating system’s setting, if light or dark mode is supported by the OS). To enforce the light or dark theme, the CLI parameter `--theme` can be used:
 ~~~
 python3 -m uploadserver --theme light
 ~~~
 or
@@ -136,14 +121,19 @@
 
 # Connect as a client
 curl -X POST https://localhost:8000/upload --insecure --cert client.pem -F files=@mtls-example.txt
 ~~~
 
 Note: This uses a self-signed server certificate which clients such as web browser and cURL will warn about. Most browsers will allow you to proceed after adding an exception, and cURL will work if given the -k/--insecure option. Using your own certificate from a certificate authority will avoid these warnings.
 
+## Breaking Changes in 5.0.0
+
+- Support for Python 3.6-7 dropped.
+- `--token` option removed (use `--basic-auth` or `--basic-auth-upload` instead).
+
 ## Breaking Changes in 4.0.0
 
 - By default, uploaded files which have the same name as an existing file are renamed. To restore the previous behavior of overwriting them, pass `--allowreplace`.
 - File uploads with no files in them are rejected with 400 Bad Request instead of 500 Internal Server Error, with a more informative error message.
 - Handling of large uploads has been improved. Theoretically this should not cause any breaking changes, but filesystems are black magic and should be viewed with suspicion.
 
 ## Breaking Changes in 3.0.0
@@ -169,8 +159,8 @@
 
 Thanks to NteRySin for several improvements including mTLS support and refactoring to support use by other modules.
 
 Thanks to marvinruder for work on the upload progress indicator, theme option, and pre-validation of tokens before upload.
 
 Thanks to shuangye for finding an easy way to handle large file uploads, and improved handling of filename collisions.
 
-Thanks to abbbe for adding HTTP basic auth.
+Thanks to abbbe for adding HTTP basic auth (has now replaced the token option).
```

### Comparing `uploadserver-4.2.0/README.md` & `uploadserver-5.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://mit-license.org/)
 [![Build Status](https://travis-ci.com/Densaugeo/uploadserver.svg?branch=master)](https://travis-ci.com/github/Densaugeo/uploadserver)
 
 ## Supported Platforms
 
 | Platform | Supported? | Notes |
 |-|-|-|
-| Python 3.6+ | Yes | Tested on 3.6 through 3.12 every release. |
+| Python 3.8+ | Yes | Tested on 3.8 through 3.12 every release. |
+| Python 3.6-3.7 | No | Was supported by previous versions. |
 | Python 3.5- | No | |
 | Linux | Yes | Tested on Fedora and Ubuntu every release. |
 | Windows | Yes | Occasional manual testing. Haven't noticed any obvious problems. |
 | Mac | No idea | I don't have a Mac. Idk if it works or not. |
 
 ## Installation
 
@@ -59,30 +60,14 @@
 python3 -m uploadserver --basic-auth-upload hello:world
 ~~~
 
 The same as above, but authentication is only required for upload operations.
 
 If both --basic-auth and --basic-auth-upload are specified, first one will be used for downloads and the second one for uploads.
 
-## Token Option (deprecated, will be removed in future)
-
-Run with a simple token.
-~~~
-python3 -m uploadserver -t helloworld
-~~~
-
-Now you can upload a file with the token. For example:
-~~~
-curl -X POST http://127.0.0.1:8000/upload -F 'files=@token-example.txt' -F 'token=helloworld'
-~~~
-
-Uploads without the token will be rejected. Tokens can be stolen if sent in plain HTTP, so this option is best used with HTTPS.
-
-Note: The server cannot check the token until after a file has been transferred, due to the way HTML form uploads are formatted, which creates a DoS vulnerability. If this is a concern, use mTLS for client authentication instead of relying on tokens.
-
 ## Theme Option
 
 The upload page supports a dark mode for showing white text on black background. If no option is specified, the color scheme is chosen from the client’s browser’s preference (which typically matches their operating system’s setting, if light or dark mode is supported by the OS). To enforce the light or dark theme, the CLI parameter `--theme` can be used:
 ~~~
 python3 -m uploadserver --theme light
 ~~~
 or
@@ -122,14 +107,19 @@
 
 # Connect as a client
 curl -X POST https://localhost:8000/upload --insecure --cert client.pem -F files=@mtls-example.txt
 ~~~
 
 Note: This uses a self-signed server certificate which clients such as web browser and cURL will warn about. Most browsers will allow you to proceed after adding an exception, and cURL will work if given the -k/--insecure option. Using your own certificate from a certificate authority will avoid these warnings.
 
+## Breaking Changes in 5.0.0
+
+- Support for Python 3.6-7 dropped.
+- `--token` option removed (use `--basic-auth` or `--basic-auth-upload` instead).
+
 ## Breaking Changes in 4.0.0
 
 - By default, uploaded files which have the same name as an existing file are renamed. To restore the previous behavior of overwriting them, pass `--allowreplace`.
 - File uploads with no files in them are rejected with 400 Bad Request instead of 500 Internal Server Error, with a more informative error message.
 - Handling of large uploads has been improved. Theoretically this should not cause any breaking changes, but filesystems are black magic and should be viewed with suspicion.
 
 ## Breaking Changes in 3.0.0
@@ -155,8 +145,8 @@
 
 Thanks to NteRySin for several improvements including mTLS support and refactoring to support use by other modules.
 
 Thanks to marvinruder for work on the upload progress indicator, theme option, and pre-validation of tokens before upload.
 
 Thanks to shuangye for finding an easy way to handle large file uploads, and improved handling of filename collisions.
 
-Thanks to abbbe for adding HTTP basic auth.
+Thanks to abbbe for adding HTTP basic auth (has now replaced the token option).
```

### Comparing `uploadserver-4.2.0/setup.py` & `uploadserver-5.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='uploadserver',
-    version='4.2.0',
+    version='5.0.0',
     author='Densaugeo',
     author_email='author@example.com',
     description='Python\'s http.server extended to include a file upload page',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Densaugeo/uploadserver',
-    packages=setuptools.find_packages(),
+    packages=['uploadserver'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
+    entry_points = {
+        'console_scripts': ['uploadserver=uploadserver:main'],
+    }
 )
```

### Comparing `uploadserver-4.2.0/uploadserver/__init__.py` & `uploadserver-5.0.0/uploadserver/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,43 @@
 import http.server, http, cgi, pathlib, sys, argparse, ssl, os, builtins
-import tempfile, base64, binascii
+import tempfile, base64, binascii, functools, contextlib
 
 # Does not seem to do be used, but leaving this import out causes uploadserver to not receive IPv4 requests when
 # started with default options under Windows
-import socket 
+import socket
 
-if sys.version_info.major > 3 or sys.version_info.minor >= 7:
-    import functools
-
-if sys.version_info.major > 3 or sys.version_info.minor >= 8:
-    import contextlib
-
-CSS = {
-    'light': '',
-    'auto': '''<style type="text/css">
-@media (prefers-color-scheme: dark) {
-  body {
-    background-color: #000;
-    color: #fff;
-  }
-}
-</style>''',
-    'dark': '''<style type="text/css">
-body {
-  background-color: #000;
-  color: #fff;
-}
-</style>'''
+COLOR_SCHEME = {
+    'light': 'light',
+    'auto': 'light dark',
+    'dark': 'dark',
 }
 
 def get_upload_page(theme):
     return bytes('''<!DOCTYPE html>
 <html>
 <head>
 <title>File Upload</title>
-<meta name="viewport" content="width=device-width, user-scalable=no" />''' \
-    + CSS.get(theme) + '''
+<meta name="viewport" content="width=device-width, user-scalable=no" />
+<meta name="color-scheme" content="''' + COLOR_SCHEME.get(theme) + '''">
 </head>
 <body>
 <h1>File Upload</h1>
 <form action="upload" method="POST" enctype="multipart/form-data">
 <input name="files" type="file" multiple />
 <br />
 <br />
-Token (only needed if server was started with token option): <input name="token" type="text" />
-<br />
-<br />
 <input type="submit" />
 </form>
-<p id="deprecation-notice"></p>
 <p id="task"></p>
 <p id="status"></p>
 </body>
 <script>
-document.getElementsByName('token')[0].value=localStorage.token || ''
-
 document.getElementsByTagName('form')[0].addEventListener('submit', async e => {
   e.preventDefault()
   
-  if(e.target.token.value) {
-    document.getElementById('deprecation-notice').textContent = 'NOTICE: Token will be deprecated in a future release, please configure the server to use the new HTTP basic auth options instead'
-  }
-  
-  localStorage.token = e.target.token.value
-  
-  const tokenValidationFormData = new FormData()
-  tokenValidationFormData.append('token', e.target.token.value)
-  
-  let tokenValidationResponse;
-  try {
-    tokenValidationResponse = await fetch('/upload/validateToken', { method: 'POST', body: tokenValidationFormData})
-  } catch (e) {
-    tokenValidationResponse = {
-      ok: false,
-      status: "Token validation unsuccessful",
-      statusText: e.message,
-    }
-  }
-  
-  if (!tokenValidationResponse.ok) {
-    let message = `${tokenValidationResponse.status}: ${tokenValidationResponse.statusText}`
-    document.getElementById('status').textContent = message
-    console.log(tokenValidationResponse)
-    return
-  }
-  message = `Success: ${tokenValidationResponse.statusText}`
   const uploadFormData = new FormData(e.target)
   const filenames = uploadFormData.getAll('files').map(v => v.name).join(', ')
   const uploadRequest = new XMLHttpRequest()
   uploadRequest.open(e.target.method, e.target.action)
   uploadRequest.timeout = 3600000
   
   uploadRequest.onreadystatechange = () => {
@@ -136,25 +85,14 @@
     (base, ext) = os.path.splitext(path)
     for i in range(1, sys.maxsize):
         renamed_path = f'{base} ({i}){ext}'
         if not os.path.exists(renamed_path):
             return renamed_path
     raise FileExistsError(f'File {path} already exists.')
 
-def validate_token(handler):
-    form = PersistentFieldStorage(fp=handler.rfile, headers=handler.headers, environ={'REQUEST_METHOD': 'POST'})
-    if args.token:
-        # server started with token.
-        if 'token' not in form or form['token'].value != args.token:
-            # no token or token error
-            handler.log_message('Token rejected (bad token)')
-            return (http.HTTPStatus.FORBIDDEN, 'Token is enabled on this server, and your token is missing or wrong')
-        return (http.HTTPStatus.NO_CONTENT, 'Token validation successful (good token)')
-    return (http.HTTPStatus.NO_CONTENT, 'Token validation successful (no token required)')
-
 def receive_upload(handler):
     result = (http.HTTPStatus.INTERNAL_SERVER_ERROR, 'Server error')
     name_conflict = False
     
     form = PersistentFieldStorage(fp=handler.rfile, headers=handler.headers, environ={'REQUEST_METHOD': 'POST'})
     if 'files' not in form:
         return (http.HTTPStatus.BAD_REQUEST, 'Field "files" not found')
@@ -168,22 +106,14 @@
     
     for field in fields:
         if field.file and field.filename:
             filename = pathlib.Path(field.filename).name
         else:
             filename = None
         
-        if args.token:
-            # server started with token.
-            if 'token' not in form or form['token'].value != args.token:
-                # no token or token error
-                handler.log_message('Upload of "{}" rejected (bad token)'.format(filename))
-                result = (http.HTTPStatus.FORBIDDEN, 'Token is enabled on this server, and your token is missing or wrong')
-                continue # continue so if a multiple file upload is rejected, each file will be logged
-        
         if filename:
             destination = pathlib.Path(args.directory) / filename
             if os.path.exists(destination):
                 if args.allow_replace and os.path.isfile(destination):
                     os.remove(destination)
                 else:
                     destination = auto_rename(destination)
@@ -226,15 +156,15 @@
 
 def check_http_authentication(handler):
     """
         This function should be called in at the beginning of HTTP method handler.
         It validates Authorization header and sends back 401 response on failure.
         It returns False if this happens.
     """
-    if handler.path in ['/upload', '/upload/validateToken']:
+    if handler.path == '/upload':
         auth = args.basic_auth or args.basic_auth_upload
     else:
         auth = args.basic_auth
     
     # If no auth settings apply, check always passes
     if not auth: return True
     
@@ -256,19 +186,17 @@
             send_upload_page(self)
         else:
             super().do_GET()
     
     def do_POST(self):
         if not check_http_authentication(self): return
         
-        if self.path in ['/upload', '/upload/validateToken']:
-            if self.path == '/upload/validateToken':
-                result = validate_token(self)
-            elif self.path == '/upload':
-                result = receive_upload(self)
+        if self.path == '/upload':
+            result = receive_upload(self)
+            
             if result[0] < http.HTTPStatus.BAD_REQUEST:
                 self.send_response(result[0], result[1])
                 self.end_headers()
             else:
                 self.send_error(result[0], result[1])
         else:
             self.send_error(http.HTTPStatus.NOT_FOUND, 'Can only POST/PUT to /upload')
@@ -284,19 +212,17 @@
             send_upload_page(self)
         else:
             super().do_GET()
     
     def do_POST(self):
         if not check_http_authentication(self): return
         
-        if self.path in ['/upload', '/upload/validateToken']:
-            if self.path == '/upload/validateToken':
-                result = validate_token(self)
-            elif self.path == '/upload':
-                result = receive_upload(self)
+        if self.path == '/upload':
+            result = receive_upload(self)
+            
             if result[0] < http.HTTPStatus.BAD_REQUEST:
                 self.send_response(result[0], result[1])
                 self.end_headers()
             else:
                 self.send_error(result[0], result[1])
         else:
             super().do_POST()
@@ -353,107 +279,74 @@
 
 def serve_forever():
     # Verify arguments in case the method was called directly
     assert hasattr(args, 'port') and type(args.port) is int
     assert hasattr(args, 'cgi') and type(args.cgi) is bool
     assert hasattr(args, 'allow_replace') and type(args.allow_replace) is bool
     assert hasattr(args, 'bind')
-    assert hasattr(args, 'token')
     assert hasattr(args, 'theme')
     assert hasattr(args, 'server_certificate')
     assert hasattr(args, 'client_certificate')
     assert hasattr(args, 'basic_auth')
     assert hasattr(args, 'basic_auth_upload')
     assert hasattr(args, 'directory') and type(args.directory) is str
     
     if args.cgi:
         handler_class = CGIHTTPRequestHandler
-    elif sys.version_info.major == 3 and sys.version_info.minor < 7:
-        handler_class = SimpleHTTPRequestHandler
     else:
         handler_class = functools.partial(SimpleHTTPRequestHandler, directory=args.directory)
     
     print('File upload available at /upload')
     
-    if sys.version_info.major == 3 and sys.version_info.minor < 8:
-        # The only difference in http.server.test() between Python 3.6 and 3.7 is the default value of ServerClass
-        if sys.version_info.minor < 7:
-            from http.server import HTTPServer as DefaultHTTPServer
-        else:
-            from http.server import ThreadingHTTPServer as DefaultHTTPServer
-        
-        class CustomHTTPServer(DefaultHTTPServer):
-            def server_bind(self):
-                bind = super().server_bind()
-                if args.server_certificate:
-                    self.socket = ssl_wrap(self.socket)
-                return bind
-        server_class = CustomHTTPServer
-    else:
-        class DualStackServer(http.server.ThreadingHTTPServer):
-            def server_bind(self):
-                # suppress exception when protocol is IPv4
-                with contextlib.suppress(Exception):
-                    self.socket.setsockopt(
-                        socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
-                bind = super().server_bind()
-                if args.server_certificate:
-                    self.socket = ssl_wrap(self.socket)
-                return bind
-        server_class = DualStackServer
+    class DualStackServer(http.server.ThreadingHTTPServer):
+        def server_bind(self):
+            # suppress exception when protocol is IPv4
+            with contextlib.suppress(Exception):
+                self.socket.setsockopt(
+                    socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
+            bind = super().server_bind()
+            if args.server_certificate:
+                self.socket = ssl_wrap(self.socket)
+            return bind
+    server_class = DualStackServer
     
     intercept_first_print()
     http.server.test(
         HandlerClass=handler_class,
         ServerClass=server_class,
         port=args.port,
         bind=args.bind,
     )
 
 def main():
     global args
     
-    # In Python 3.8, http.server.test() was altered to use None instead of '' as the default for its bind parameter
-    if sys.version_info.major == 3 and sys.version_info.minor < 8:
-        bind_default = ''
-    else:
-        bind_default = None
-    
     parser = argparse.ArgumentParser()
     parser.add_argument('port', type=int, default=8000, nargs='?',
         help='Specify alternate port [default: 8000]')
     parser.add_argument('--cgi', action='store_true',
         help='Run as CGI Server')
     parser.add_argument('--allow-replace', action='store_true', default=False,
         help='Replace existing file if uploaded file has the same name. Auto rename by default.')
-    parser.add_argument('--bind', '-b', default=bind_default, metavar='ADDRESS',
+    parser.add_argument('--bind', '-b', metavar='ADDRESS',
         help='Specify alternate bind address [default: all interfaces]')
-    parser.add_argument('--token', '-t', type=str,
-        help='Specify alternate token [default: \'\']')
+    parser.add_argument('--directory', '-d', default=os.getcwd(),
+        help='Specify alternative directory [default:current directory]')
     parser.add_argument('--theme', type=str, default='auto',
         choices=['light', 'auto', 'dark'], help='Specify a light or dark theme for the upload page [default: auto]')
     parser.add_argument('--server-certificate', '--certificate', '-c',
         help='Specify HTTPS server certificate to use [default: none]')
     parser.add_argument('--client-certificate',
         help='Specify HTTPS client certificate to accept for mutual TLS [default: none]')
     parser.add_argument('--basic-auth',
         help='Specify user:pass for basic authentication (downloads and uploads)')
     parser.add_argument('--basic-auth-upload',
         help='Specify user:pass for basic authentication (uploads only)')
     
-    # Directory option was added to http.server in Python 3.7
-    if sys.version_info.major > 3 or sys.version_info.minor >= 7:
-        parser.add_argument('--directory', '-d', default=os.getcwd(),
-            help='Specify alternative directory [default:current directory]')
-    
     args = parser.parse_args()
     if not hasattr(args, 'directory'): args.directory = os.getcwd()
     
-    if args.token:
-        print('WARNING: Token will be deprecated in a future release, please use the new '
-            'HTTP basic auth options instead')
-    
     if args.basic_auth and args.basic_auth_upload:
         print('Cannot set both --basic--auth and --basic-auth-upload')
         sys.exit(6)
     
     serve_forever()
```

### Comparing `uploadserver-4.2.0/uploadserver.egg-info/PKG-INFO` & `uploadserver-5.0.0/uploadserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: uploadserver
-Version: 4.2.0
+Version: 5.0.0
 Summary: Python's http.server extended to include a file upload page
 Home-page: https://github.com/Densaugeo/uploadserver
 Author: Densaugeo
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # uploadserver
 
 Python's http.server extended to include a file upload page
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://mit-license.org/)
 [![Build Status](https://travis-ci.com/Densaugeo/uploadserver.svg?branch=master)](https://travis-ci.com/github/Densaugeo/uploadserver)
 
 ## Supported Platforms
 
 | Platform | Supported? | Notes |
 |-|-|-|
-| Python 3.6+ | Yes | Tested on 3.6 through 3.12 every release. |
+| Python 3.8+ | Yes | Tested on 3.8 through 3.12 every release. |
+| Python 3.6-3.7 | No | Was supported by previous versions. |
 | Python 3.5- | No | |
 | Linux | Yes | Tested on Fedora and Ubuntu every release. |
 | Windows | Yes | Occasional manual testing. Haven't noticed any obvious problems. |
 | Mac | No idea | I don't have a Mac. Idk if it works or not. |
 
 ## Installation
 
@@ -73,30 +74,14 @@
 python3 -m uploadserver --basic-auth-upload hello:world
 ~~~
 
 The same as above, but authentication is only required for upload operations.
 
 If both --basic-auth and --basic-auth-upload are specified, first one will be used for downloads and the second one for uploads.
 
-## Token Option (deprecated, will be removed in future)
-
-Run with a simple token.
-~~~
-python3 -m uploadserver -t helloworld
-~~~
-
-Now you can upload a file with the token. For example:
-~~~
-curl -X POST http://127.0.0.1:8000/upload -F 'files=@token-example.txt' -F 'token=helloworld'
-~~~
-
-Uploads without the token will be rejected. Tokens can be stolen if sent in plain HTTP, so this option is best used with HTTPS.
-
-Note: The server cannot check the token until after a file has been transferred, due to the way HTML form uploads are formatted, which creates a DoS vulnerability. If this is a concern, use mTLS for client authentication instead of relying on tokens.
-
 ## Theme Option
 
 The upload page supports a dark mode for showing white text on black background. If no option is specified, the color scheme is chosen from the client’s browser’s preference (which typically matches their operating system’s setting, if light or dark mode is supported by the OS). To enforce the light or dark theme, the CLI parameter `--theme` can be used:
 ~~~
 python3 -m uploadserver --theme light
 ~~~
 or
@@ -136,14 +121,19 @@
 
 # Connect as a client
 curl -X POST https://localhost:8000/upload --insecure --cert client.pem -F files=@mtls-example.txt
 ~~~
 
 Note: This uses a self-signed server certificate which clients such as web browser and cURL will warn about. Most browsers will allow you to proceed after adding an exception, and cURL will work if given the -k/--insecure option. Using your own certificate from a certificate authority will avoid these warnings.
 
+## Breaking Changes in 5.0.0
+
+- Support for Python 3.6-7 dropped.
+- `--token` option removed (use `--basic-auth` or `--basic-auth-upload` instead).
+
 ## Breaking Changes in 4.0.0
 
 - By default, uploaded files which have the same name as an existing file are renamed. To restore the previous behavior of overwriting them, pass `--allowreplace`.
 - File uploads with no files in them are rejected with 400 Bad Request instead of 500 Internal Server Error, with a more informative error message.
 - Handling of large uploads has been improved. Theoretically this should not cause any breaking changes, but filesystems are black magic and should be viewed with suspicion.
 
 ## Breaking Changes in 3.0.0
@@ -169,8 +159,8 @@
 
 Thanks to NteRySin for several improvements including mTLS support and refactoring to support use by other modules.
 
 Thanks to marvinruder for work on the upload progress indicator, theme option, and pre-validation of tokens before upload.
 
 Thanks to shuangye for finding an easy way to handle large file uploads, and improved handling of filename collisions.
 
-Thanks to abbbe for adding HTTP basic auth.
+Thanks to abbbe for adding HTTP basic auth (has now replaced the token option).
```

