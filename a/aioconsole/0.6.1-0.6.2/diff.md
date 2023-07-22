# Comparing `tmp/aioconsole-0.6.1.tar.gz` & `tmp/aioconsole-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioconsole-0.6.1.tar", last modified: Sat Mar  4 10:45:25 2023, max compression
+gzip compressed data, was "aioconsole-0.6.2.tar", last modified: Sat Jul 22 15:20:27 2023, max compression
```

## Comparing `aioconsole-0.6.1.tar` & `aioconsole-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:45:25.972683 aioconsole-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35120 2023-03-04 10:45:24.000000 aioconsole-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-03-04 10:45:25.972683 aioconsole-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-03-04 10:45:24.000000 aioconsole-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:45:25.972683 aioconsole-0.6.1/aioconsole/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/apython.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/rlwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-03-04 10:45:24.000000 aioconsole-0.6.1/aioconsole/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 10:45:25.972683 aioconsole-0.6.1/aioconsole.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-03-04 10:45:25.000000 aioconsole-0.6.1/aioconsole.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-04 10:45:25.000000 aioconsole-0.6.1/aioconsole.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 10:45:25.000000 aioconsole-0.6.1/aioconsole.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-04 10:45:25.000000 aioconsole-0.6.1/aioconsole.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-04 10:45:25.000000 aioconsole-0.6.1/aioconsole.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-04 10:45:25.972683 aioconsole-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-04 10:45:24.000000 aioconsole-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:20:27.495530 aioconsole-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-07-22 15:20:26.000000 aioconsole-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-22 15:20:27.495530 aioconsole-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-22 15:20:26.000000 aioconsole-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:20:27.491530 aioconsole-0.6.2/aioconsole/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/apython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/rlwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-22 15:20:26.000000 aioconsole-0.6.2/aioconsole/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:20:27.495530 aioconsole-0.6.2/aioconsole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-22 15:20:27.000000 aioconsole-0.6.2/aioconsole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-22 15:20:27.000000 aioconsole-0.6.2/aioconsole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:20:27.000000 aioconsole-0.6.2/aioconsole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-22 15:20:27.000000 aioconsole-0.6.2/aioconsole.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 15:20:27.000000 aioconsole-0.6.2/aioconsole.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-22 15:20:27.495530 aioconsole-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-22 15:20:26.000000 aioconsole-0.6.2/setup.py
```

### Comparing `aioconsole-0.6.1/LICENSE` & `aioconsole-0.6.2/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <http://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `aioconsole-0.6.1/PKG-INFO` & `aioconsole-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aioconsole
-Version: 0.6.1
+Version: 0.6.2
 Summary: Asynchronous console and interfaces for asyncio
 Home-page: https://github.com/vxgmichel/aioconsole
 Author: Vincent Michel
 Author-email: vxgmichel@gmail.com
 License: GPLv3
 Download-URL: https://pypi.org/project/aioconsole/
 Description: aioconsole
```

### Comparing `aioconsole-0.6.1/README.rst` & `aioconsole-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `aioconsole-0.6.1/aioconsole/__init__.py` & `aioconsole-0.6.2/aioconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.6.1/aioconsole/apython.py` & `aioconsole-0.6.2/aioconsole/apython.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 
     if (
         namespace.readline
         and not namespace.serve
         and compat.platform != "win32"
         and load_readline()
     ):
-
         # Run python interactive hook in order to configure binding and history support
         interactive_hook = getattr(sys, "__interactivehook__", None)
         if interactive_hook:
             try:
                 interactive_hook()
             except Exception as exc:
                 warnings.warn(f"Interactive hook failed: {exc!r}", stacklevel=2)
```

### Comparing `aioconsole-0.6.1/aioconsole/command.py` & `aioconsole-0.6.2/aioconsole/command.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.6.1/aioconsole/console.py` & `aioconsole-0.6.2/aioconsole/console.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.6.1/aioconsole/events.py` & `aioconsole-0.6.2/aioconsole/events.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.6.1/aioconsole/execute.py` & `aioconsole-0.6.2/aioconsole/execute.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.6.1/aioconsole/rlwrap.py` & `aioconsole-0.6.2/aioconsole/rlwrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
     # Run background task
     with ThreadPoolExecutor(1) as executor:
         future = executor.submit(wait_for_prompt, source, dest, prompt_control)
 
         # Loop over prompts
         while process.poll() is None:
-
             # Get prompt
             try:
                 prompt = future.result()
             except KeyboardInterrupt:
                 process.send_signal(signal.SIGINT)
                 continue
             except EOFError:
```

### Comparing `aioconsole-0.6.1/aioconsole/server.py` & `aioconsole-0.6.2/aioconsole/server.py`

 * *Files identical despite different names*

### Comparing `aioconsole-0.6.1/aioconsole/stream.py` & `aioconsole-0.6.2/aioconsole/stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def is_pipe_transport_compatible(pipe):
     if compat.platform == "win32":
         return False
     try:
         fileno = pipe.fileno()
-    except OSError:
+    except (OSError, AttributeError):
         return False
     mode = os.fstat(fileno).st_mode
     is_char = stat.S_ISCHR(mode)
     is_fifo = stat.S_ISFIFO(mode)
     is_socket = stat.S_ISSOCK(mode)
     if not (is_char or is_fifo or is_socket):
         return False
@@ -90,15 +90,14 @@
         # Call the parent
         super().connection_lost(exc)
         # Restore the inner state
         self.__dict__.update(state)
 
 
 class StandardStreamReader(asyncio.StreamReader):
-
     __del__ = protect_standard_streams
 
     async def readuntil(self, separator=b"\n"):
         # Re-implement `readuntil` to work around self._limit.
         # The limit is still useful to prevent the internal buffer
         # from growing too large when it's not necessary, but it
         # needs to be disabled when the user code is purposely
@@ -112,15 +111,14 @@
                     del self._buffer[: e.consumed + len(separator)]
                     self._maybe_resume_transport()
                     return bytes(chunk)
                 await self._wait_for_data("readuntil")
 
 
 class StandardStreamWriter(asyncio.StreamWriter):
-
     __del__ = protect_standard_streams
 
     def write(self, data):
         if isinstance(data, str):
             data = data.encode()
         super().write(data)
 
@@ -133,22 +131,28 @@
         self.stream = stream
         self.eof = False
 
     def at_eof(self):
         return self.eof
 
     async def readline(self):
-        data = await run_as_daemon(self.stream.readline)
+        try:
+            data = await run_as_daemon(self.stream.readline)
+        except AttributeError:
+            raise RuntimeError("ainput(): lost sys.stdin")
         if isinstance(data, str):
             data = data.encode()
         self.eof = not data
         return data
 
     async def read(self, n=-1):
-        data = await run_as_daemon(self.stream.read, n)
+        try:
+            data = await run_as_daemon(self.stream.read, n)
+        except AttributeError:
+            raise RuntimeError("ainput(): lost sys.stdin")
         if isinstance(data, str):
             data = data.encode()
         self.eof = not data
         return data
 
     def __aiter__(self):
         return self
@@ -253,16 +257,15 @@
 
 async def get_standard_streams(*, cache={}, use_stderr=False, loop=None):
     if loop is None:
         loop = asyncio.get_event_loop()
     args = sys.stdin, sys.stdout, sys.stderr
     key = args, loop
     if cache.get(key) is None:
-        connection = create_standard_streams(*args, loop=loop)
-        cache[key] = await connection
+        cache[key] = await create_standard_streams(*args, loop=loop)
     in_reader, out_writer, err_writer = cache[key]
     return in_reader, err_writer if use_stderr else out_writer
 
 
 async def ainput(prompt="", *, streams=None, use_stderr=False, loop=None):
     """Asynchronous equivalent to *input*."""
     # Get standard streams
```

### Comparing `aioconsole-0.6.1/aioconsole.egg-info/PKG-INFO` & `aioconsole-0.6.2/aioconsole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aioconsole
-Version: 0.6.1
+Version: 0.6.2
 Summary: Asynchronous console and interfaces for asyncio
 Home-page: https://github.com/vxgmichel/aioconsole
 Author: Vincent Michel
 Author-email: vxgmichel@gmail.com
 License: GPLv3
 Download-URL: https://pypi.org/project/aioconsole/
 Description: aioconsole
```

### Comparing `aioconsole-0.6.1/setup.py` & `aioconsole-0.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.10
 Programming Language :: Python :: 3 :: Only
 """.splitlines()
 
 setup(
     name="aioconsole",
-    version="0.6.1",
+    version="0.6.2",
     packages=["aioconsole"],
     entry_points={"console_scripts": ["apython = aioconsole:run_apython"]},
     setup_requires=["pytest-runner" if TESTING else ""],
     tests_require=[
         "pytest",
         "pytest-asyncio",
         "pytest-cov",
```

