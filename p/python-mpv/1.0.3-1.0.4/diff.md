# Comparing `tmp/python-mpv-1.0.3.tar.gz` & `tmp/python-mpv-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mpv-1.0.3.tar", last modified: Mon Feb 27 09:31:30 2023, max compression
+gzip compressed data, was "python-mpv-1.0.4.tar", last modified: Sat Jul 22 14:19:03 2023, max compression
```

## Comparing `python-mpv-1.0.3.tar` & `python-mpv-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2023-02-27 09:31:30.520204 python-mpv-1.0.3/
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    18092 2023-02-26 12:13:42.000000 python-mpv-1.0.3/LICENSE.GPL
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    26530 2023-02-26 12:13:42.000000 python-mpv-1.0.3/LICENSE.LGPL
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    15415 2023-02-27 09:31:30.520204 python-mpv-1.0.3/PKG-INFO
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    14207 2023-02-27 09:26:59.000000 python-mpv-1.0.3/README.rst
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    88054 2023-02-27 09:26:59.000000 python-mpv-1.0.3/mpv.py
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)     1304 2023-02-27 09:31:22.000000 python-mpv-1.0.3/pyproject.toml
-drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2023-02-27 09:31:30.520204 python-mpv-1.0.3/python_mpv.egg-info/
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)    15415 2023-02-27 09:31:30.000000 python-mpv-1.0.3/python_mpv.egg-info/PKG-INFO
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)      244 2023-02-27 09:31:30.000000 python-mpv-1.0.3/python_mpv.egg-info/SOURCES.txt
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)        1 2023-02-27 09:31:30.000000 python-mpv-1.0.3/python_mpv.egg-info/dependency_links.txt
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)       45 2023-02-27 09:31:30.000000 python-mpv-1.0.3/python_mpv.egg-info/requires.txt
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)        4 2023-02-27 09:31:30.000000 python-mpv-1.0.3/python_mpv.egg-info/top_level.txt
--rw-r--r--   0 jaseg     (1000) jaseg     (1000)       38 2023-02-27 09:31:30.520204 python-mpv-1.0.3/setup.cfg
-drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2023-02-27 09:31:30.520204 python-mpv-1.0.3/tests/
--rwxr-xr-x   0 jaseg     (1000) jaseg     (1000)    31814 2023-02-27 09:26:59.000000 python-mpv-1.0.3/tests/test_mpv.py
+drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2023-07-22 14:19:03.739394 python-mpv-1.0.4/
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    18092 2023-02-26 12:13:42.000000 python-mpv-1.0.4/LICENSE.GPL
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    26530 2023-02-26 12:13:42.000000 python-mpv-1.0.4/LICENSE.LGPL
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    15415 2023-07-22 14:19:03.739394 python-mpv-1.0.4/PKG-INFO
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    14207 2023-02-27 09:26:59.000000 python-mpv-1.0.4/README.rst
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    88231 2023-07-22 14:04:17.000000 python-mpv-1.0.4/mpv.py
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)     1309 2023-07-22 14:18:58.000000 python-mpv-1.0.4/pyproject.toml
+drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2023-07-22 14:19:03.739394 python-mpv-1.0.4/python_mpv.egg-info/
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)    15415 2023-07-22 14:19:03.000000 python-mpv-1.0.4/python_mpv.egg-info/PKG-INFO
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)      244 2023-07-22 14:19:03.000000 python-mpv-1.0.4/python_mpv.egg-info/SOURCES.txt
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)        1 2023-07-22 14:19:03.000000 python-mpv-1.0.4/python_mpv.egg-info/dependency_links.txt
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)       50 2023-07-22 14:19:03.000000 python-mpv-1.0.4/python_mpv.egg-info/requires.txt
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)        4 2023-07-22 14:19:03.000000 python-mpv-1.0.4/python_mpv.egg-info/top_level.txt
+-rw-r--r--   0 jaseg     (1000) jaseg     (1000)       38 2023-07-22 14:19:03.739394 python-mpv-1.0.4/setup.cfg
+drwxr-xr-x   0 jaseg     (1000) jaseg     (1000)        0 2023-07-22 14:19:03.739394 python-mpv-1.0.4/tests/
+-rwxr-xr-x   0 jaseg     (1000) jaseg     (1000)    31867 2023-07-22 14:03:02.000000 python-mpv-1.0.4/tests/test_mpv.py
```

### Comparing `python-mpv-1.0.3/LICENSE.GPL` & `python-mpv-1.0.4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `python-mpv-1.0.3/LICENSE.LGPL` & `python-mpv-1.0.4/LICENSE.LGPL`

 * *Files identical despite different names*

### Comparing `python-mpv-1.0.3/PKG-INFO` & `python-mpv-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mpv
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python interface to the mpv media player
 Author-email: jaseg <mpv@jaseg.de>
 License: GPLv2+ or LGPLv2.1+
 Project-URL: homepage, https://github.com/jaseg/python-mpv
 Keywords: mpv,library,video,audio,player,display,multimedia
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications
```

### Comparing `python-mpv-1.0.3/README.rst` & `python-mpv-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `python-mpv-1.0.3/mpv.py` & `python-mpv-1.0.4/mpv.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 #
 # This library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
 # warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License and the GNU
 # Lesser General Public License for more details.
 #
 # You can find copies of the GPLv2 and LGPLv2.1 licenses in the project repository's LICENSE.GPL and LICENSE.LGPL files.
 
+__version__ = '1.0.4'
+
 from ctypes import *
 import ctypes.util
 import threading
 import queue
 import os
 import sys
 from warnings import warn
@@ -437,17 +439,22 @@
         return self._level.decode("utf-8")
 
     @property
     def text(self):
         return lazy_decoder(self._text)
 
 class MpvEventEndFile(Structure):
-    _fields_ = [('reason', c_int),
-                ('error', c_int)]
-
+    _fields_ = [
+        ('reason', c_int),
+        ('error', c_int),
+        ('playlist_entry_id', c_ulonglong),
+        ('playlist_insert_id', c_ulonglong),
+        ('playlist_insert_num_entries', c_int),
+    ]
+    
     EOF                 = 0
     RESTARTED           = 1
     ABORTED             = 2
     QUIT                = 3
     ERROR               = 4
     REDIRECT            = 5
 
@@ -1442,15 +1449,15 @@
         """Mapped mpv rescan-external-files command, see man mpv(1)."""
         self.command('rescan-external-files', mode)
 
     def discnav(self, command):
         """Mapped mpv discnav command, see man mpv(1)."""
         self.command('discnav', command)
 
-    def mouse(x, y, button=None, mode='single'):
+    def mouse(self, x, y, button=None, mode='single'):
         """Mapped mpv mouse command, see man mpv(1)."""
         if button is None:
             self.command('mouse', x, y, mode)
         else:
             self.command('mouse', x, y, button, mode)
 
     def keypress(self, name):
```

### Comparing `python-mpv-1.0.3/pyproject.toml` & `python-mpv-1.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['mpv']
 
 [project]
 name = "python-mpv"
-version = "v1.0.3"
+version = "v1.0.4"
 description = "A python interface to the mpv media player"
 readme = "README.rst"
 authors = [{name = "jaseg", email = "mpv@jaseg.de"}]
 license = {text = "GPLv2+ or LGPLv2.1+"}
 requires-python = ">=3.7"
 keywords = ['mpv', 'library', 'video', 'audio', 'player', 'display', 'multimedia']
 classifiers = [
@@ -32,8 +32,8 @@
 ]
 
 [project.urls]
 homepage = "https://github.com/jaseg/python-mpv"
 
 [project.optional-dependencies]
 screenshot_raw = ["Pillow"]
-test = ['xvfbwrapper']
+test = ['PyVirtualDisplay']
```

### Comparing `python-mpv-1.0.3/python_mpv.egg-info/PKG-INFO` & `python-mpv-1.0.4/python_mpv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mpv
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python interface to the mpv media player
 Author-email: jaseg <mpv@jaseg.de>
 License: GPLv2+ or LGPLv2.1+
 Project-URL: homepage, https://github.com/jaseg/python-mpv
 Keywords: mpv,library,video,audio,player,display,multimedia
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications
```

### Comparing `python-mpv-1.0.3/tests/test_mpv.py` & `python-mpv-1.0.4/tests/test_mpv.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 os.environ["PATH"] = os.path.dirname(__file__) + os.pathsep + os.environ["PATH"]
 
 import mpv
 
 
 if os.name == 'nt':
-  Xvfb = mock.Mock()
+  Display = mock.Mock()
   testvo='gpu'
 
 else:
-  from xvfbwrapper import Xvfb
+  from pyvirtualdisplay import Display
   testvo='x11'
 
 
 TESTVID = os.path.join(os.path.dirname(__file__), 'test.webm')
 TESTSRT = os.path.join(os.path.dirname(__file__), 'sub_test.srt')
 MPV_ERRORS = [ l(ec) for ec, l in mpv.ErrorCode.EXCEPTION_DICT.items() if l ]
 SKIP_TESTS = os.environ.get('PY_MPV_SKIP_TESTS', '').split()
@@ -50,15 +50,15 @@
     def do_print(level, prefix, text):
         td = time.time() - start_time
         print('{:.3f} [{}] {}: {}'.format(td, level, prefix, text), flush=True)
 
 
 class MpvTestCase(unittest.TestCase):
     def setUp(self):
-        self.disp = Xvfb()
+        self.disp = Display()
         self.disp.start()
         self.m = mpv.MPV(vo=testvo, loglevel='debug', log_handler=timed_print())
 
     def tearDown(self):
         self.m.terminate()
         self.disp.stop()
 
@@ -440,15 +440,15 @@
         handler2.assert_has_calls([ mock.call() ])
 
 
 class TestStreams(unittest.TestCase):
     def test_python_stream(self):
         handler = mock.Mock()
 
-        disp = Xvfb()
+        disp = Display()
         disp.start()
         m = mpv.MPV(vo=testvo)
         def cb(evt):
             handler(evt.as_dict(decoder=mpv.lazy_decoder))
         m.register_event_callback(cb)
 
         @m.python_stream('foo')
@@ -498,15 +498,15 @@
     def test_custom_stream(self):
         handler = mock.Mock()
         fail_mock = mock.Mock(side_effect=ValueError)
         stream_mock = mock.Mock()
         stream_mock.seek = mock.Mock(return_value=0)
         stream_mock.read = mock.Mock(return_value=b'')
 
-        disp = Xvfb()
+        disp = Display()
         disp.start()
         m = mpv.MPV(vo=testvo, video=False)
         def cb(evt):
             handler(evt.as_dict(decoder=mpv.lazy_decoder))
         m.register_event_callback(cb)
 
         m.register_stream_protocol('pythonfail', fail_mock)
@@ -532,15 +532,15 @@
         stream_mock.read.assert_called()
         handler.assert_any_call({'event': 'end-file', 'reason': 'error', 'playlist_entry_id': 3, 'file_error': 'unrecognized file format'})
 
         m.terminate()
         disp.stop()
 
     def test_stream_open_exception(self):
-        disp = Xvfb()
+        disp = Display()
         disp.start()
         m = mpv.MPV(vo=testvo, video=False)
 
         @m.register_stream_protocol('raiseerror')
         def open_fn(uri):
             raise SystemError()
 
@@ -568,15 +568,15 @@
         try:
             assert result.result()
         finally:
             m.terminate()
             disp.stop()
 
     def test_python_stream_exception(self):
-        disp = Xvfb()
+        disp = Display()
         disp.start()
         m = mpv.MPV(vo=testvo)
 
         @m.python_stream('foo')
         def foo_gen():
             with open(TESTVID, 'rb') as f:
                 yield f.read(100)
@@ -606,15 +606,15 @@
         try:
             assert result.result()
         finally:
             m.terminate()
             disp.stop()
 
     def test_stream_open_forward(self):
-        disp = Xvfb()
+        disp = Display()
         disp.start()
         m = mpv.MPV(vo=testvo, video=False)
 
         @m.register_stream_protocol('raiseerror')
         def open_fn(uri):
             raise ValueError()
 
@@ -688,15 +688,15 @@
             ], any_order=True)
         time.sleep(1)
         handler.reset_mock()
         m.terminate()
         handler.assert_not_called()
 
     def test_wait_for_property_negative(self):
-        self.disp = Xvfb()
+        self.disp = Display()
         self.disp.start()
         m = mpv.MPV(vo=testvo)
         m.play(TESTVID)
         result = Future()
         def run():
             nonlocal self
             result.set_running_or_notify_cancel()
@@ -711,15 +711,15 @@
         m.terminate()
         time.sleep(1)
         t.join()
         self.disp.stop()
         assert result.result()
 
     def test_wait_for_property_positive(self):
-        self.disp = Xvfb()
+        self.disp = Display()
         self.disp.start()
         handler = mock.Mock()
         m = mpv.MPV(vo=testvo)
         m.play(TESTVID)
         def run():
             nonlocal self
             m.wait_for_property('mute')
@@ -731,15 +731,15 @@
         t.join()
         m.terminate()
         time.sleep(1)
         handler.assert_called()
         self.disp.stop()
 
     def test_wait_for_event(self):
-        self.disp = Xvfb()
+        self.disp = Display()
         self.disp.start()
         m = mpv.MPV(vo=testvo)
         m.play(TESTVID)
         result = Future()
         def run():
             nonlocal self
             result.set_running_or_notify_cancel()
@@ -753,29 +753,29 @@
         time.sleep(1)
         m.terminate()
         t.join()
         self.disp.stop()
         assert result.result()
 
     def test_wait_for_property_shutdown(self):
-        self.disp = Xvfb()
+        self.disp = Display()
         self.disp.start()
         m = mpv.MPV(vo=testvo)
         m.play(TESTVID)
         with self.assertRaises(mpv.ShutdownError):
             # level_sensitive=false needed to prevent get_property on dead
             # handle
             with m.prepare_and_wait_for_property('mute', level_sensitive=False):
                 m.terminate()
         time.sleep(1)
         self.disp.stop()
 
     @unittest.skipIf('test_wait_for_property_event_overflow' in SKIP_TESTS, reason="kills X-Server first")
     def test_wait_for_property_event_overflow(self):
-        self.disp = Xvfb()
+        self.disp = Display()
         self.disp.start()
         m = mpv.MPV(vo=testvo)
         m.play(TESTVID)
         with self.assertRaises(mpv.EventOverflowError):
             # level_sensitive=false needed to prevent get_property on dead
             # handle
             with m.prepare_and_wait_for_property('mute', cond=lambda val: time.sleep(0.001)):
@@ -788,37 +788,37 @@
                     except:
                         pass
         m.terminate()
         time.sleep(1)
         self.disp.stop()
 
     def test_wait_for_event_shutdown(self):
-        self.disp = Xvfb()
+        self.disp = Display()
         self.disp.start()
         m = mpv.MPV(vo=testvo)
         m.play(TESTVID)
         with self.assertRaises(mpv.ShutdownError):
             with m.prepare_and_wait_for_event('seek'):
                 m.terminate()
         self.disp.stop()
 
     def test_wait_for_shutdown(self):
-        self.disp = Xvfb()
+        self.disp = Display()
         self.disp.start()
         m = mpv.MPV(vo=testvo)
         m.play(TESTVID)
         with self.assertRaises(mpv.ShutdownError):
             with m.prepare_and_wait_for_event(None) as result:
                 m.terminate()
             result.result()
         self.disp.stop()
 
     def test_log_handler(self):
         handler = mock.Mock()
-        self.disp = Xvfb()
+        self.disp = Display()
         self.disp.start()
         m = mpv.MPV(vo=testvo, log_handler=handler)
         m.play(TESTVID)
         # Wait for playback to start
         m.wait_until_playing(timeout=2)
         m.command("print-text", 'This is a python-mpv test')
         m.wait_for_playback()
```

