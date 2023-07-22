# Comparing `tmp/Louie-1.1.tar.gz` & `tmp/Louie-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Louie-1.1.tar", last modified: Mon Jan 30 19:53:57 2006, max compression, from Unix
+gzip compressed data, was "dist/Louie-2.0.tar", last modified: Mon Sep  9 15:36:56 2019, max compression
```

## Comparing `Louie-1.1.tar` & `Louie-2.0.tar`

### file list

```diff
@@ -1,38 +1,29 @@
-drwxr-xr-x   0 gldnspud  (1000) gldnspud  (1000)        0 2006-01-30 19:53:57.000000 Louie-1.1/
-drwxr-xr-x   0 gldnspud  (1000) gldnspud  (1000)        0 2006-01-30 19:53:57.000000 Louie-1.1/doc/
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      231 2005-11-30 16:15:12.000000 Louie-1.1/doc/contributors.txt
-drwxr-xr-x   0 gldnspud  (1000) gldnspud  (1000)        0 2006-01-30 19:53:57.000000 Louie-1.1/doc/template/
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     3692 2005-11-30 16:36:32.000000 Louie-1.1/doc/template/layout.html
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     2111 2005-11-30 16:36:32.000000 Louie-1.1/doc/template/layout.css
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     3948 2005-11-30 16:36:32.000000 Louie-1.1/doc/template/almodovar.css
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     2011 2005-12-19 15:17:39.000000 Louie-1.1/doc/index.txt
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     2393 2005-11-30 16:28:22.000000 Louie-1.1/doc/about.txt
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     1385 2005-12-19 15:17:09.000000 Louie-1.1/doc/changes.txt
-drwxr-xr-x   0 gldnspud  (1000) gldnspud  (1000)        0 2006-01-30 19:53:57.000000 Louie-1.1/louie/
-drwxr-xr-x   0 gldnspud  (1000) gldnspud  (1000)        0 2006-01-30 19:53:57.000000 Louie-1.1/louie/test/
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)        0 2005-11-29 19:50:19.000000 Louie-1.1/louie/test/fixture.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     4927 2005-12-06 14:37:36.000000 Louie-1.1/louie/test/test_dispatcher.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)       86 2005-11-29 19:50:19.000000 Louie-1.1/louie/test/conftest.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      767 2005-11-29 19:50:19.000000 Louie-1.1/louie/test/test_robustapply.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     2162 2005-11-29 19:50:19.000000 Louie-1.1/louie/test/test_saferef.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     4035 2006-01-30 19:44:48.000000 Louie-1.1/louie/test/test_plugin.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)        0 2005-11-29 19:50:19.000000 Louie-1.1/louie/test/__init__.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      577 2006-01-30 19:44:48.000000 Louie-1.1/louie/error.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     1183 2005-11-29 19:50:19.000000 Louie-1.1/louie/sender.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     2148 2005-11-30 17:44:41.000000 Louie-1.1/louie/robustapply.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)    19674 2005-12-19 15:34:32.000000 Louie-1.1/louie/dispatcher.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     7099 2005-12-06 14:37:37.000000 Louie-1.1/louie/saferef.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      918 2005-12-09 21:50:47.000000 Louie-1.1/louie/__init__.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      663 2005-11-29 19:50:19.000000 Louie-1.1/louie/signal.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      113 2006-01-30 19:44:48.000000 Louie-1.1/louie/version.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     3250 2006-01-30 19:44:48.000000 Louie-1.1/louie/plugin.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      936 2006-01-30 19:53:57.000000 Louie-1.1/PKG-INFO
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      595 2006-01-30 19:50:08.000000 Louie-1.1/setup.cfg
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     1324 2005-12-19 15:30:22.000000 Louie-1.1/setup.py
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)     8189 2005-11-29 22:10:34.000000 Louie-1.1/ez_setup.py
-drwxr-xr-x   0 gldnspud  (1000) gldnspud  (1000)        0 2006-01-30 19:53:57.000000 Louie-1.1/Louie.egg-info/
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      936 2006-01-30 19:53:57.000000 Louie-1.1/Louie.egg-info/PKG-INFO
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)      646 2006-01-30 19:53:57.000000 Louie-1.1/Louie.egg-info/SOURCES.txt
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)        6 2006-01-30 19:53:57.000000 Louie-1.1/Louie.egg-info/top_level.txt
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)        0 2006-01-30 19:37:31.000000 Louie-1.1/Louie.egg-info/not-zip-safe
--rw-r--r--   0 gldnspud  (1000) gldnspud  (1000)       13 2006-01-30 19:53:57.000000 Louie-1.1/Louie.egg-info/requires.txt
+drwxr-xr-x   0 gldnspud   (501) staff       (20)        0 2019-09-09 15:36:56.000000 Louie-2.0/
+drwxr-xr-x   0 gldnspud   (501) staff       (20)        0 2019-09-09 15:36:56.000000 Louie-2.0/Louie.egg-info/
+-rw-r--r--   0 gldnspud   (501) staff       (20)     1297 2019-09-09 15:36:55.000000 Louie-2.0/Louie.egg-info/PKG-INFO
+-rw-r--r--   0 gldnspud   (501) staff       (20)      501 2019-09-09 15:36:55.000000 Louie-2.0/Louie.egg-info/SOURCES.txt
+-rw-r--r--   0 gldnspud   (501) staff       (20)        1 2019-09-09 15:36:55.000000 Louie-2.0/Louie.egg-info/dependency_links.txt
+-rw-r--r--   0 gldnspud   (501) staff       (20)        0 2019-09-09 15:36:55.000000 Louie-2.0/Louie.egg-info/not-zip-safe
+-rw-r--r--   0 gldnspud   (501) staff       (20)        6 2019-09-09 15:36:55.000000 Louie-2.0/Louie.egg-info/top_level.txt
+-rw-r--r--   0 gldnspud   (501) staff       (20)     1297 2019-09-09 15:36:56.000000 Louie-2.0/PKG-INFO
+-rw-r--r--   0 gldnspud   (501) staff       (20)      644 2019-09-09 15:36:55.000000 Louie-2.0/README.rst
+drwxr-xr-x   0 gldnspud   (501) staff       (20)        0 2019-09-09 15:36:56.000000 Louie-2.0/louie/
+-rw-r--r--   0 gldnspud   (501) staff       (20)      866 2019-09-09 15:36:55.000000 Louie-2.0/louie/__init__.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)    19420 2019-09-09 15:36:55.000000 Louie-2.0/louie/dispatcher.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)      569 2019-09-09 15:36:55.000000 Louie-2.0/louie/error.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)     3217 2019-09-09 15:36:55.000000 Louie-2.0/louie/plugin.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)     2144 2019-09-09 15:36:55.000000 Louie-2.0/louie/robustapply.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)     8296 2019-09-09 15:36:55.000000 Louie-2.0/louie/saferef.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)     1156 2019-09-09 15:36:55.000000 Louie-2.0/louie/sender.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)      655 2019-09-09 15:36:55.000000 Louie-2.0/louie/signal.py
+drwxr-xr-x   0 gldnspud   (501) staff       (20)        0 2019-09-09 15:36:56.000000 Louie-2.0/louie/test/
+-rw-r--r--   0 gldnspud   (501) staff       (20)        0 2019-09-09 15:36:55.000000 Louie-2.0/louie/test/__init__.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)       85 2019-09-09 15:36:55.000000 Louie-2.0/louie/test/conftest.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)        0 2019-09-09 15:36:55.000000 Louie-2.0/louie/test/fixture.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)     5786 2019-09-09 15:36:55.000000 Louie-2.0/louie/test/test_dispatcher.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)     4017 2019-09-09 15:36:55.000000 Louie-2.0/louie/test/test_plugin.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)      706 2019-09-09 15:36:55.000000 Louie-2.0/louie/test/test_robustapply.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)     2071 2019-09-09 15:36:55.000000 Louie-2.0/louie/test/test_saferef.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)      111 2019-09-09 15:36:55.000000 Louie-2.0/louie/version.py
+-rw-r--r--   0 gldnspud   (501) staff       (20)       38 2019-09-09 15:36:56.000000 Louie-2.0/setup.cfg
+-rw-r--r--   0 gldnspud   (501) staff       (20)      802 2019-09-09 15:36:55.000000 Louie-2.0/setup.py
```

### Comparing `Louie-1.1/louie/test/test_dispatcher.py` & `Louie-2.0/louie/test/test_dispatcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import gc
 import unittest
 
 import louie
 from louie import dispatcher
 
 
 def x(a):
@@ -9,146 +10,178 @@
 
 
 class Dummy(object):
     pass
 
 
 class Callable(object):
-
     def __call__(self, a):
         return a
 
     def a(self, a):
         return a
 
 
 class TestDispatcher(unittest.TestCase):
-
     def setUp(self):
         louie.reset()
 
     def _isclean(self):
         """Assert that everything has been cleaned up automatically"""
         assert len(dispatcher.senders_back) == 0, dispatcher.senders_back
         assert len(dispatcher.connections) == 0, dispatcher.connections
         assert len(dispatcher.senders) == 0, dispatcher.senders
-    
+
     def test_Exact(self):
         a = Dummy()
-        signal = 'this'
+        signal = "this"
         louie.connect(x, signal, a)
         expected = [(x, a)]
-        result = louie.send('this', a, a=a)
-        assert result == expected, (
-            "Send didn't return expected result:\n\texpected:%s\n\tgot:%s"
-            % (expected, result))
+        result = louie.send(signal, a, a=a)
+        assert (
+            result == expected
+        ), f"Send didn't return expected result:\n\texpected:{expected}\n\tgot:{result}"
         louie.disconnect(x, signal, a)
         assert len(list(louie.get_all_receivers(a, signal))) == 0
         self._isclean()
-        
+
     def test_AnonymousSend(self):
         a = Dummy()
-        signal = 'this'
+        signal = "this"
         louie.connect(x, signal)
         expected = [(x, a)]
         result = louie.send(signal, None, a=a)
-        assert result == expected, (
-            "Send didn't return expected result:\n\texpected:%s\n\tgot:%s"
-            % (expected, result))
+        assert (
+            result == expected
+        ), f"Send didn't return expected result:\n\texpected:{expected}\n\tgot:{result}"
         louie.disconnect(x, signal)
         assert len(list(louie.get_all_receivers(None, signal))) == 0
         self._isclean()
-        
+
     def test_AnyRegistration(self):
         a = Dummy()
-        signal = 'this'
+        signal = "this"
         louie.connect(x, signal, louie.Any)
         expected = [(x, a)]
-        result = louie.send('this', object(), a=a)
-        assert result == expected, (
-            "Send didn't return expected result:\n\texpected:%s\n\tgot:%s"
-            % (expected, result))
+        result = louie.send(signal, object(), a=a)
+        assert (
+            result == expected
+        ), f"Send didn't return expected result:\n\texpected:{expected}\n\tgot:{result}"
         louie.disconnect(x, signal, louie.Any)
         expected = []
-        result = louie.send('this', object(), a=a)
-        assert result == expected, (
-            "Send didn't return expected result:\n\texpected:%s\n\tgot:%s"
-            % (expected, result))
+        result = louie.send(signal, object(), a=a)
+        assert (
+            result == expected
+        ), f"Send didn't return expected result:\n\texpected:{expected}\n\tgot:{result}"
         assert len(list(louie.get_all_receivers(louie.Any, signal))) == 0
         self._isclean()
-        
+
     def test_AllRegistration(self):
         a = Dummy()
-        signal = 'this'
+        signal = "this"
         louie.connect(x, louie.All, a)
         expected = [(x, a)]
-        result = louie.send('this', a, a=a)
-        assert result == expected, (
-            "Send didn't return expected result:\n\texpected:%s\n\tgot:%s"
-            % (expected, result))
+        result = louie.send(signal, a, a=a)
+        assert (
+            result == expected
+        ), f"Send didn't return expected result:\n\texpected:{expected}\n\tgot:{result}"
         louie.disconnect(x, louie.All, a)
         assert len(list(louie.get_all_receivers(a, louie.All))) == 0
         self._isclean()
-        
+
+    def test_receiver_disconnects_itself(self):
+        disconnect_receiver1 = []
+        signal = "this"
+
+        def receiver1():
+            if disconnect_receiver1:
+                louie.disconnect(receiver1, signal)
+            return 1
+
+        def receiver2():
+            return 2
+
+        louie.connect(receiver1, signal)
+        louie.connect(receiver2, signal)
+        # Try without disconnecting; we'll get two responses.
+        result = louie.send(signal)
+        assert result == [(receiver1, 1), (receiver2, 2)]
+        # We should also get two responses when first receiver disconnects.
+        disconnect_receiver1.append(True)
+        result = louie.send(signal)
+        assert result == [(receiver1, 1), (receiver2, 2)]
+        # Then the next time around should have no receiver1.
+        result = louie.send(signal)
+        assert result == [(receiver2, 2)]
+
     def test_GarbageCollected(self):
         a = Callable()
         b = Dummy()
-        signal = 'this'
+        signal = "this"
         louie.connect(a.a, signal, b)
         expected = []
         del a
-        result = louie.send('this', b, a=b)
-        assert result == expected, (
-            "Send didn't return expected result:\n\texpected:%s\n\tgot:%s"
-            % (expected, result))
-        assert len(list(louie.get_all_receivers(b, signal))) == 0, (
-            "Remaining handlers: %s" % (louie.get_all_receivers(b, signal),))
+        gc.collect()
+        result = louie.send(signal, b, a=b)
+        assert (
+            result == expected
+        ), f"Send didn't return expected result:\n\texpected:{expected}\n\tgot:{result}"
+        assert (
+            len(list(louie.get_all_receivers(b, signal))) == 0
+        ), f"Remaining handlers: {louie.get_all_receivers(b, signal)}"
         self._isclean()
-        
+
     def test_GarbageCollectedObj(self):
         class x:
             def __call__(self, a):
                 return a
+
         a = Callable()
         b = Dummy()
-        signal = 'this'
+        signal = "this"
         louie.connect(a, signal, b)
         expected = []
         del a
-        result = louie.send('this', b, a=b)
-        assert result == expected, (
-            "Send didn't return expected result:\n\texpected:%s\n\tgot:%s"
-            % (expected, result))
-        assert len(list(louie.get_all_receivers(b, signal))) == 0, (
-            "Remaining handlers: %s" % (louie.get_all_receivers(b, signal),))
+        gc.collect()
+        result = louie.send(signal, b, a=b)
+        assert (
+            result == expected
+        ), f"Send didn't return expected result:\n\texpected:{expected}\n\tgot:{result}"
+        assert (
+            len(list(louie.get_all_receivers(b, signal))) == 0
+        ), f"Remaining handlers: {louie.get_all_receivers(b, signal)}"
         self._isclean()
 
     def test_MultipleRegistration(self):
         a = Callable()
         b = Dummy()
-        signal = 'this'
+        signal = "this"
         louie.connect(a, signal, b)
         louie.connect(a, signal, b)
         louie.connect(a, signal, b)
         louie.connect(a, signal, b)
         louie.connect(a, signal, b)
         louie.connect(a, signal, b)
-        result = louie.send('this', b, a=b)
+        result = louie.send(signal, b, a=b)
         assert len(result) == 1, result
-        assert len(list(louie.get_all_receivers(b, signal))) == 1, (
-            "Remaining handlers: %s" % (louie.get_all_receivers(b, signal),))
+        assert (
+            len(list(louie.get_all_receivers(b, signal))) == 1
+        ), f"Remaining handlers: {louie.get_all_receivers(b, signal)}"
         del a
         del b
         del result
+        gc.collect()
         self._isclean()
 
     def test_robust(self):
         """Test the sendRobust function."""
+
         def fails():
-            raise ValueError('this')
+            raise ValueError("this")
+
         a = object()
-        signal = 'this'
+        signal = "this"
         louie.connect(fails, louie.All, a)
-        result = louie.send_robust('this', a, a=a)
+        result = louie.send_robust(signal, a, a=a)
         err = result[0][1]
         assert isinstance(err, ValueError)
-        assert err.args == ('this', )
+        assert err.args == ("this",)
```

### Comparing `Louie-1.1/louie/test/test_robustapply.py` & `Louie-2.0/louie/test/test_robustapply.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 
 
 def two_arguments(blah, other):
     pass
 
 
 class TestRobustApply(unittest.TestCase):
-    
     def test_01(self):
         robust_apply(no_argument, no_argument)
-        
+
     def test_02(self):
-        self.assertRaises(TypeError, robust_apply, no_argument, no_argument,
-                          'this' )
-        
+        self.assertRaises(TypeError, robust_apply, no_argument, no_argument, "this")
+
     def test_03(self):
         self.assertRaises(TypeError, robust_apply, one_argument, one_argument)
-        
+
     def test_04(self):
         """Raise error on duplication of a particular argument"""
-        self.assertRaises(TypeError, robust_apply, one_argument, one_argument,
-                          'this', blah='that')
-
+        self.assertRaises(
+            TypeError, robust_apply, one_argument, one_argument, "this", blah="that"
+        )
```

### Comparing `Louie-1.1/louie/test/test_saferef.py` & `Louie-2.0/louie/test/test_saferef.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,81 +3,80 @@
 from louie.saferef import safe_ref
 
 
 class _Sample1(object):
     def x(self):
         pass
 
-    
+
 def _sample2(obj):
     pass
 
 
 class _Sample3(object):
     def __call__(self, obj):
         pass
 
-    
+
 class TestSaferef(unittest.TestCase):
 
     # XXX: The original tests had a test for closure, and it had an
     # off-by-one problem, perhaps due to scope issues.  It has been
     # removed from this test suite.
-    
+
     def setUp(self):
         ts = []
         ss = []
-        for x in xrange(5000):
+        self.closure_count = 0
+        self.ts = ts
+        self.ss = ss
+        for x in range(5000):
             t = _Sample1()
             ts.append(t)
             s = safe_ref(t.x, self._closure)
             ss.append(s)
         ts.append(_sample2)
         ss.append(safe_ref(_sample2, self._closure))
-        for x in xrange(30):
+        for x in range(30):
             t = _Sample3()
             ts.append(t)
             s = safe_ref(t, self._closure)
             ss.append(s)
-        self.ts = ts
-        self.ss = ss
-        self.closure_count = 0
-        
+
     def tearDown(self):
-        if hasattr(self, 'ts'):
+        if hasattr(self, "ts"):
             del self.ts
-        if hasattr(self, 'ss'):
+        if hasattr(self, "ss"):
             del self.ss
-        
+
     def test_In(self):
         """Test the `in` operator for safe references (cmp)"""
         for t in self.ts[:50]:
             assert safe_ref(t.x) in self.ss
-            
+
     def test_Valid(self):
         """Test that the references are valid (return instance methods)"""
         for s in self.ss:
             assert s()
-            
+
     def test_ShortCircuit(self):
         """Test that creation short-circuits to reuse existing references"""
         sd = {}
         for s in self.ss:
             sd[s] = 1
         for t in self.ts:
-            if hasattr(t, 'x'):
-                assert sd.has_key(safe_ref(t.x))
+            if hasattr(t, "x"):
+                assert safe_ref(t.x) in sd
             else:
-                assert sd.has_key(safe_ref(t))
-                
+                assert safe_ref(t) in sd
+
     def test_Representation(self):
         """Test that the reference object's representation works
 
         XXX Doesn't currently check the results, just that no error
             is raised
         """
         repr(self.ss[-1])
-        
+
     def _closure(self, ref):
         """Dumb utility mechanism to increment deletion counter"""
         self.closure_count += 1
-
```

### Comparing `Louie-1.1/louie/test/test_plugin.py` & `Louie-2.0/louie/test/test_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 """Louie plugin tests."""
 
-import unittest
-
 import louie
 
 try:
     import qt
-    if not hasattr(qt.qApp, 'for_testing'):
+
+    if not hasattr(qt.qApp, "for_testing"):
         _app = qt.QApplication([])
         _app.for_testing = True
         qt.qApp = _app
 except ImportError:
     qt = None
 
 
 class ReceiverBase(object):
-
     def __init__(self):
         self.args = []
         self.live = True
 
     def __call__(self, arg):
         self.args.append(arg)
 
+
 class Receiver1(ReceiverBase):
     pass
 
+
 class Receiver2(ReceiverBase):
     pass
 
 
 class Plugin1(louie.Plugin):
-
     def is_live(self, receiver):
         """ReceiverBase instances are only live if their `live`
         attribute is True"""
         if isinstance(receiver, ReceiverBase):
             return receiver.live
         return True
 
 
 class Plugin2(louie.Plugin):
-
     def is_live(self, receiver):
         """Pretend all Receiver2 instances are not live."""
         if isinstance(receiver, Receiver2):
             return False
         return True
 
 
@@ -57,89 +55,92 @@
     # XXX: Move these tests into test cases so we can use unittest's
     # 'assertRaises' method.
     try:
         louie.install_plugin(plugin1b)
     except louie.error.PluginTypeError:
         pass
     else:
-        raise Exception('PluginTypeError not raised')
+        raise Exception("PluginTypeError not raised")
 
 
 def test_is_live():
     louie.reset()
     # Create receivers.
     receiver1a = Receiver1()
     receiver1b = Receiver1()
     receiver2a = Receiver2()
     receiver2b = Receiver2()
     # Connect signals.
-    louie.connect(receiver1a, 'sig')
-    louie.connect(receiver1b, 'sig')
-    louie.connect(receiver2a, 'sig')
-    louie.connect(receiver2b, 'sig')
+    louie.connect(receiver1a, "sig")
+    louie.connect(receiver1b, "sig")
+    louie.connect(receiver2a, "sig")
+    louie.connect(receiver2b, "sig")
     # Check reception without plugins.
-    louie.send('sig', arg='foo')
-    assert receiver1a.args == ['foo']
-    assert receiver1b.args == ['foo']
-    assert receiver2a.args == ['foo']
-    assert receiver2b.args == ['foo']
+    louie.send("sig", arg="foo")
+    assert receiver1a.args == ["foo"]
+    assert receiver1b.args == ["foo"]
+    assert receiver2a.args == ["foo"]
+    assert receiver2b.args == ["foo"]
     # Install plugin 1.
     plugin1 = Plugin1()
     louie.install_plugin(plugin1)
     # Make some receivers not live.
     receiver1a.live = False
     receiver2b.live = False
     # Check reception.
-    louie.send('sig', arg='bar')
-    assert receiver1a.args == ['foo']
-    assert receiver1b.args == ['foo', 'bar']
-    assert receiver2a.args == ['foo', 'bar']
-    assert receiver2b.args == ['foo']
+    louie.send("sig", arg="bar")
+    assert receiver1a.args == ["foo"]
+    assert receiver1b.args == ["foo", "bar"]
+    assert receiver2a.args == ["foo", "bar"]
+    assert receiver2b.args == ["foo"]
     # Remove plugin 1, install plugin 2.
     plugin2 = Plugin2()
     louie.remove_plugin(plugin1)
     louie.install_plugin(plugin2)
     # Check reception.
-    louie.send('sig', arg='baz')
-    assert receiver1a.args == ['foo', 'baz']
-    assert receiver1b.args == ['foo', 'bar', 'baz']
-    assert receiver2a.args == ['foo', 'bar']
-    assert receiver2b.args == ['foo']
+    louie.send("sig", arg="baz")
+    assert receiver1a.args == ["foo", "baz"]
+    assert receiver1b.args == ["foo", "bar", "baz"]
+    assert receiver2a.args == ["foo", "bar"]
+    assert receiver2b.args == ["foo"]
     # Install plugin 1 alongside plugin 2.
     louie.install_plugin(plugin1)
     # Check reception.
-    louie.send('sig', arg='fob')
-    assert receiver1a.args == ['foo', 'baz']
-    assert receiver1b.args == ['foo', 'bar', 'baz', 'fob']
-    assert receiver2a.args == ['foo', 'bar']
-    assert receiver2b.args == ['foo']
-    
+    louie.send("sig", arg="fob")
+    assert receiver1a.args == ["foo", "baz"]
+    assert receiver1b.args == ["foo", "bar", "baz", "fob"]
+    assert receiver2a.args == ["foo", "bar"]
+    assert receiver2b.args == ["foo"]
+
 
 if qt is not None:
+
     def test_qt_plugin():
         louie.reset()
+
         # Create receivers.
         class Receiver(qt.QWidget):
             def __init__(self):
                 qt.QObject.__init__(self)
                 self.args = []
+
             def receive(self, arg):
                 self.args.append(arg)
+
         receiver1 = Receiver()
         receiver2 = Receiver()
         # Connect signals.
-        louie.connect(receiver1.receive, 'sig')
-        louie.connect(receiver2.receive, 'sig')
+        louie.connect(receiver1.receive, "sig")
+        louie.connect(receiver2.receive, "sig")
         # Destroy receiver2 so only a shell is left.
         receiver2.close(True)
         # Check reception without plugins.
-        louie.send('sig', arg='foo')
-        assert receiver1.args == ['foo']
-        assert receiver2.args == ['foo']
+        louie.send("sig", arg="foo")
+        assert receiver1.args == ["foo"]
+        assert receiver2.args == ["foo"]
         # Install plugin.
         plugin = louie.QtWidgetPlugin()
         louie.install_plugin(plugin)
         # Check reception with plugins.
-        louie.send('sig', arg='bar')
-        assert receiver1.args == ['foo', 'bar']
-        assert receiver2.args == ['foo']
-
+        louie.send("sig", arg="bar")
+        assert receiver1.args == ["foo", "bar"]
+        assert receiver2.args == ["foo"]
```

### Comparing `Louie-1.1/louie/error.py` & `Louie-2.0/louie/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 class LouieError(Exception):
     """Base class for all Louie errors"""
 
 
 class DispatcherError(LouieError):
     """Base class for all Dispatcher errors"""
-    
+
 
 class DispatcherKeyError(KeyError, DispatcherError):
     """Error raised when unknown (sender, signal) specified"""
-    
+
 
 class DispatcherTypeError(TypeError, DispatcherError):
     """Error raised when inappropriate signal-type specified (None)"""
 
 
 class PluginTypeError(TypeError, LouieError):
     """Error raise when trying to install more than one plugin of a
```

### Comparing `Louie-1.1/louie/sender.py` & `Louie-2.0/louie/sender.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 """Sender classes."""
 
 
 class _SENDER(type):
     """Base metaclass for sender classes."""
 
     def __str__(cls):
-        return '<Sender: %s>' % (cls.__name__, )
+        return f"<Sender: {cls.__name__}>"
 
 
-class Any(object):
+class Any(object, metaclass=_SENDER):
     """Used to represent either 'any sender'.
 
     The Any class can be used with connect, disconnect, send, or
     sendExact to denote that the sender paramater should react to any
     sender, not just a particular sender.
     """
 
-    __metaclass__ = _SENDER
 
-
-class Anonymous(object):
+class Anonymous(object, metaclass=_SENDER):
     """Singleton used to signal 'anonymous sender'.
 
     The Anonymous class is used to signal that the sender of a message
     is not specified (as distinct from being 'any sender').
     Registering callbacks for Anonymous will only receive messages
     sent without senders.  Sending with anonymous will only send
     messages to those receivers registered for Any or Anonymous.
 
     Note: The default sender for connect is Any, while the default
     sender for send is Anonymous.  This has the effect that if you do
     not specify any senders in either function then all messages are
     routed as though there was a single sender (Anonymous) being used
     everywhere.
     """
-
-    __metaclass__ = _SENDER
-
```

### Comparing `Louie-1.1/louie/robustapply.py` & `Louie-2.0/louie/robustapply.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 """Robust apply mechanism.
 
 Provides a function 'call', which can sort out what arguments a given
 callable object can take, and subset the given arguments to match only
 those which are acceptable.
 """
 
+IM_FUNC = "__func__"
+FUNC_CODE = "__code__"
+
+
 def function(receiver):
     """Get function-like callable object for given receiver.
 
     returns (function_or_method, codeObject, fromMethod)
 
     If fromMethod is true, then the callable already has its first
     argument bound.
     """
-    if hasattr(receiver, '__call__'):
-        # receiver is a class instance; assume it is callable.
-        # Reassign receiver to the actual method that will be called.
-        c = receiver.__call__
-        if hasattr(c, 'im_func') or hasattr(c, 'im_code'):
-            receiver = c
-    if hasattr(receiver, 'im_func'):
-        # receiver is an instance-method.
-        return receiver, receiver.im_func.func_code, 1
-    elif not hasattr(receiver, 'func_code'):
-        raise ValueError(
-            'unknown reciever type %s %s' % (receiver, type(receiver)))
-    return receiver, receiver.func_code, 0
+    if hasattr(receiver, IM_FUNC):
+        # Instance method.
+        im_func = getattr(receiver, IM_FUNC)
+        func_code = getattr(im_func, FUNC_CODE)
+        return receiver, func_code, True
+    elif hasattr(receiver, FUNC_CODE):
+        func_code = getattr(receiver, FUNC_CODE)
+        return receiver, func_code, False
+    elif hasattr(receiver, "__call__"):
+        return function(receiver.__call__)
+    else:
+        raise ValueError(f"unknown reciever type {receiver} {type(receiver)}")
 
 
 def robust_apply(receiver, signature, *arguments, **named):
     """Call receiver with arguments and appropriate subset of named.
     ``signature`` is the callable used to determine the call signature
     of the receiver, in case ``receiver`` is a callable wrapper of the
     actual receiver."""
     signature, code_object, startIndex = function(signature)
     acceptable = code_object.co_varnames[
-        startIndex + len(arguments):
-        code_object.co_argcount
-        ]
-    for name in code_object.co_varnames[
-        startIndex:startIndex + len(arguments)
-        ]:
-        if named.has_key(name):
+        startIndex + len(arguments) : code_object.co_argcount
+    ]
+    for name in code_object.co_varnames[startIndex : startIndex + len(arguments)]:
+        if name in named:
             raise TypeError(
-                'Argument %r specified both positionally '
-                'and as a keyword for calling %r'
-                % (name, signature)
-                )
+                f"Argument {name!r} specified both positionally "
+                f"and as a keyword for calling {signature!r}"
+            )
     if not (code_object.co_flags & 8):
-        # fc does not have a **kwds type parameter, therefore 
+        # fc does not have a **kwds type parameter, therefore
         # remove unacceptable arguments.
-        for arg in named.keys():
+        # have to make this a list type in python3 as dicts cant be
+        # modified in place, producing RuntimeError
+        for arg in list(named.keys()):
             if arg not in acceptable:
                 del named[arg]
     return receiver(*arguments, **named)
-
-
```

### Comparing `Louie-1.1/louie/dispatcher.py` & `Louie-2.0/louie/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,72 +4,68 @@
 core logic for the system.
 
 Internal attributes:
 
 - ``WEAKREF_TYPES``: Tuple of types/classes which represent weak
   references to receivers, and thus must be dereferenced on retrieval
   to retrieve the callable object
-        
+
 - ``connections``::
 
     { senderkey (id) : { signal : [receivers...] } }
-    
+
 - ``senders``: Used for cleaning up sender references on sender
   deletion::
 
     { senderkey (id) : weakref(sender) }
-    
+
 - ``senders_back``: Used for cleaning up receiver references on receiver
   deletion::
 
     { receiverkey (id) : [senderkey (id)...] }
 """
 
-import os
 import weakref
 
-try:
-    set
-except NameError:
-    from sets import Set as set, ImmutableSet as frozenset
-
-from louie import error
-from louie import robustapply
-from louie import saferef
-from louie.sender import Any, Anonymous
+from louie import error, robustapply, saferef
+from louie.sender import Anonymous, Any
 from louie.signal import All
 
-
 # Support for statistics.
 if __debug__:
+    import os
+
     connects = 0
     disconnects = 0
     sends = 0
 
     def print_stats():
-        print ('\n'
-               'Louie connects: %i\n'
-               'Louie disconnects: %i\n'
-               'Louie sends: %i\n'
-               '\n') % (connects, disconnects, sends)
+        print(
+            "\n"
+            f"Louie connects: {connects}\n"
+            f"Louie disconnects: {disconnects}\n"
+            f"Louie sends: {sends}\n"
+            "\n"
+        )
 
-    if 'PYDISPATCH_STATS' in os.environ:
+    if "PYDISPATCH_STATS" in os.environ:
         import atexit
-        atexit.register(print_stats)
 
+        atexit.register(print_stats)
 
 
 WEAKREF_TYPES = (weakref.ReferenceType, saferef.BoundMethodWeakref)
 
 
 connections = {}
 senders = {}
 senders_back = {}
 plugins = []
 
+
 def reset():
     """Reset the state of Louie.
 
     Useful during unit testing.  Should be avoided otherwise.
     """
     global connections, senders, senders_back, plugins
     connections = {}
@@ -83,148 +79,149 @@
 
     - ``receiver``: A callable Python object which is to receive
       messages/signals/events.  Receivers must be hashable objects.
 
       If weak is ``True``, then receiver must be weak-referencable (more
       precisely ``saferef.safe_ref()`` must be able to create a
       reference to the receiver).
-    
+
       Receivers are fairly flexible in their specification, as the
       machinery in the ``robustapply`` module takes care of most of the
       details regarding figuring out appropriate subsets of the sent
       arguments to apply to a given receiver.
 
       Note: If ``receiver`` is itself a weak reference (a callable), it
       will be de-referenced by the system's machinery, so *generally*
       weak references are not suitable as receivers, though some use
       might be found for the facility whereby a higher-level library
       passes in pre-weakrefed receiver references.
 
     - ``signal``: The signal to which the receiver should respond.
-    
+
       If ``All``, receiver will receive all signals from the indicated
       sender (which might also be ``All``, but is not necessarily
       ``All``).
-        
+
       Otherwise must be a hashable Python object other than ``None``
       (``DispatcherError`` raised on ``None``).
-        
+
     - ``sender``: The sender to which the receiver should respond.
-    
+
       If ``Any``, receiver will receive the indicated signals from any
       sender.
-        
+
       If ``Anonymous``, receiver will only receive indicated signals
       from ``send``/``send_exact`` which do not specify a sender, or
       specify ``Anonymous`` explicitly as the sender.
 
       Otherwise can be any python object.
-        
+
     - ``weak``: Whether to use weak references to the receiver.
-      
+
       By default, the module will attempt to use weak references to
       the receiver objects.  If this parameter is ``False``, then strong
       references will be used.
 
     Returns ``None``, may raise ``DispatcherTypeError``.
     """
     if signal is None:
         raise error.DispatcherTypeError(
-            'Signal cannot be None (receiver=%r sender=%r)'
-            % (receiver, sender))
+            f"Signal cannot be None (receiver={receiver!r} sender={sender!r})"
+        )
     if weak:
         receiver = saferef.safe_ref(receiver, on_delete=_remove_receiver)
     senderkey = id(sender)
-    if connections.has_key(senderkey):
+    if senderkey in connections:
         signals = connections[senderkey]
     else:
         connections[senderkey] = signals = {}
     # Keep track of senders for cleanup.
     # Is Anonymous something we want to clean up?
     if sender not in (None, Anonymous, Any):
+
         def remove(object, senderkey=senderkey):
             _remove_sender(senderkey=senderkey)
+
         # Skip objects that can not be weakly referenced, which means
         # they won't be automatically cleaned up, but that's too bad.
         try:
             weak_sender = weakref.ref(sender, remove)
             senders[senderkey] = weak_sender
-        except:
+        except Exception:
             pass
     receiver_id = id(receiver)
     # get current set, remove any current references to
     # this receiver in the set, including back-references
-    if signals.has_key(signal):
+    if signal in signals:
         receivers = signals[signal]
         _remove_old_back_refs(senderkey, signal, receiver, receivers)
     else:
         receivers = signals[signal] = []
     try:
         current = senders_back.get(receiver_id)
         if current is None:
             senders_back[receiver_id] = current = []
         if senderkey not in current:
             current.append(senderkey)
-    except:
+    except Exception:
         pass
     receivers.append(receiver)
     # Update stats.
     if __debug__:
         global connects
         connects += 1
 
 
 def disconnect(receiver, signal=All, sender=Any, weak=True):
     """Disconnect ``receiver`` from ``sender`` for ``signal``.
 
     - ``receiver``: The registered receiver to disconnect.
-    
+
     - ``signal``: The registered signal to disconnect.
-    
+
     - ``sender``: The registered sender to disconnect.
-    
+
     - ``weak``: The weakref state to disconnect.
 
     ``disconnect`` reverses the process of ``connect``, the semantics for
     the individual elements are logically equivalent to a tuple of
     ``(receiver, signal, sender, weak)`` used as a key to be deleted
     from the internal routing tables.  (The actual process is slightly
     more complex but the semantics are basically the same).
 
     Note: Using ``disconnect`` is not required to cleanup routing when
     an object is deleted; the framework will remove routes for deleted
     objects automatically.  It's only necessary to disconnect if you
     want to stop routing to a live object.
-        
+
     Returns ``None``, may raise ``DispatcherTypeError`` or
     ``DispatcherKeyError``.
     """
     if signal is None:
         raise error.DispatcherTypeError(
-            'Signal cannot be None (receiver=%r sender=%r)'
-            % (receiver, sender))
+            f"Signal cannot be None (receiver={receiver!r} sender={sender!r})"
+        )
     if weak:
         receiver = saferef.safe_ref(receiver)
     senderkey = id(sender)
     try:
         signals = connections[senderkey]
         receivers = signals[signal]
     except KeyError:
         raise error.DispatcherKeyError(
-            'No receivers found for signal %r from sender %r' 
-            % (signal, sender)
-            )
+            f"No receivers found for signal {signal!r} from sender {sender!r}"
+        )
     try:
         # also removes from receivers
         _remove_old_back_refs(senderkey, signal, receiver, receivers)
     except ValueError:
         raise error.DispatcherKeyError(
-            'No connection to receiver %s for signal %s from sender %s'
-            % (receiver, signal, sender)
-            )
+            f"No connection to receiver {receiver!r} "
+            f"for signal {signal!r} from sender {sender!r}"
+        )
     _cleanup_connections(senderkey, signal)
     # Update stats.
     if __debug__:
         global disconnects
         disconnects += 1
 
 
@@ -265,15 +262,15 @@
             live = True
             for plugin in plugins:
                 if not plugin.is_live(receiver):
                     live = False
                     break
             if live:
                 yield receiver
-            
+
 
 def get_all_receivers(sender=Any, signal=All):
     """Get list of all receivers from global tables.
 
     This gets all receivers which should receive the given signal from
     sender, each receiver should be produced only once by the
     resulting generator.
@@ -284,33 +281,36 @@
         get_receivers(sender, signal),
         # Add receivers that receive *all* signals from *this* sender.
         get_receivers(sender, All),
         # Add receivers that receive *this* signal from *any* sender.
         get_receivers(Any, signal),
         # Add receivers that receive *all* signals from *any* sender.
         get_receivers(Any, All),
-        ):
-        for receiver in receivers:
-            if receiver: # filter out dead instance-method weakrefs
+    ):
+        # Make a copy of each list so it's immutable within the context
+        # of this function, even if a receiver calls disconnect() or any
+        # other function that changes a list of receivers.
+        for receiver in list(receivers):
+            if receiver:  # filter out dead instance-method weakrefs
                 try:
-                    if not receiver in yielded:
+                    if receiver not in yielded:
                         yielded.add(receiver)
                         yield receiver
                 except TypeError:
                     # dead weakrefs raise TypeError on hash...
                     pass
 
 
 def send(signal=All, sender=Anonymous, *arguments, **named):
     """Send ``signal`` from ``sender`` to all connected receivers.
-    
+
     - ``signal``: (Hashable) signal value; see ``connect`` for details.
 
     - ``sender``: The sender of the signal.
-    
+
       If ``Any``, only receivers registered for ``Any`` will receive the
       message.
 
       If ``Anonymous``, only receivers registered to receive messages
       from ``Anonymous`` or ``Any`` will receive the message.
 
       Otherwise can be any Python object (normally one registered with
@@ -337,20 +337,16 @@
     responses = []
     for receiver in live_receivers(get_all_receivers(sender, signal)):
         # Wrap receiver using installed plugins.
         original = receiver
         for plugin in plugins:
             receiver = plugin.wrap_receiver(receiver)
         response = robustapply.robust_apply(
-            receiver, original,
-            signal=signal,
-            sender=sender,
-            *arguments,
-            **named
-            )
+            receiver, original, signal=signal, sender=sender, *arguments, **named
+        )
         responses.append((receiver, response))
     # Update stats.
     if __debug__:
         global sends
         sends += 1
     return responses
 
@@ -362,19 +358,15 @@
     # Return a list of tuple pairs [(receiver, response), ... ].
     responses = []
     for receiver in live_receivers(get_all_receivers(sender, signal)):
         # Wrap receiver using installed plugins.
         original = receiver
         for plugin in plugins:
             receiver = plugin.wrap_receiver(receiver)
-        response = robustapply.robust_apply(
-            receiver, original,
-            *arguments,
-            **named
-            )
+        response = robustapply.robust_apply(receiver, original, *arguments, **named)
         responses.append((receiver, response))
     # Update stats.
     if __debug__:
         global sends
         sends += 1
     return responses
 
@@ -389,32 +381,28 @@
     responses = []
     for receiver in live_receivers(get_receivers(sender, signal)):
         # Wrap receiver using installed plugins.
         original = receiver
         for plugin in plugins:
             receiver = plugin.wrap_receiver(receiver)
         response = robustapply.robust_apply(
-            receiver, original,
-            signal=signal,
-            sender=sender,
-            *arguments,
-            **named
-            )
+            receiver, original, signal=signal, sender=sender, *arguments, **named
+        )
         responses.append((receiver, response))
     return responses
-    
+
 
 def send_robust(signal=All, sender=Anonymous, *arguments, **named):
     """Send ``signal`` from ``sender`` to all connected receivers catching
     errors
 
     - ``signal``: (Hashable) signal value, see connect for details
 
     - ``sender``: The sender of the signal.
-    
+
       If ``Any``, only receivers registered for ``Any`` will receive the
       message.
 
       If ``Anonymous``, only receivers registered to receive messages
       from ``Anonymous`` or ``Any`` will receive the message.
 
       Otherwise can be any Python object (normally one registered with
@@ -441,40 +429,36 @@
     responses = []
     for receiver in live_receivers(get_all_receivers(sender, signal)):
         original = receiver
         for plugin in plugins:
             receiver = plugin.wrap_receiver(receiver)
         try:
             response = robustapply.robust_apply(
-                receiver, original,
-                signal=signal,
-                sender=sender,
-                *arguments,
-                **named
-                )
-        except Exception, err:
+                receiver, original, signal=signal, sender=sender, *arguments, **named
+            )
+        except Exception as err:
             responses.append((receiver, err))
         else:
             responses.append((receiver, response))
     return responses
 
 
 def _remove_receiver(receiver):
     """Remove ``receiver`` from connections."""
     if not senders_back:
         # During module cleanup the mapping will be replaced with None.
         return False
     backKey = id(receiver)
     for senderkey in senders_back.get(backKey, ()):
         try:
-            signals = connections[senderkey].keys()
+            signals = list(connections[senderkey].keys())
         except KeyError:
             pass
         else:
-            for signal in signals:
+            for signal in list(signals):
                 try:
                     receivers = connections[senderkey][signal]
                 except KeyError:
                     pass
                 else:
                     try:
                         receivers.remove(receiver)
@@ -482,21 +466,21 @@
                         pass
                 _cleanup_connections(senderkey, signal)
     try:
         del senders_back[backKey]
     except KeyError:
         pass
 
-            
+
 def _cleanup_connections(senderkey, signal):
     """Delete empty signals for ``senderkey``. Delete ``senderkey`` if
     empty."""
     try:
         receivers = connections[senderkey][signal]
-    except:
+    except Exception:
         pass
     else:
         if not receivers:
             # No more connected receivers. Therefore, remove the signal.
             try:
                 signals = connections[senderkey]
             except KeyError:
@@ -511,30 +495,30 @@
 def _remove_sender(senderkey):
     """Remove ``senderkey`` from connections."""
     _remove_back_refs(senderkey)
     try:
         del connections[senderkey]
     except KeyError:
         pass
-    # Senderkey will only be in senders dictionary if sender 
+    # Senderkey will only be in senders dictionary if sender
     # could be weakly referenced.
     try:
         del senders[senderkey]
-    except:
+    except Exception:
         pass
 
 
 def _remove_back_refs(senderkey):
     """Remove all back-references to this ``senderkey``."""
     try:
         signals = connections[senderkey]
     except KeyError:
         signals = None
     else:
-        for signal, receivers in signals.iteritems():
+        for signal, receivers in list(signals.items()):
             for receiver in receivers:
                 _kill_back_ref(receiver, senderkey)
 
 
 def _remove_old_back_refs(senderkey, signal, receiver, receivers):
     """Kill old ``senders_back`` references from ``receiver``.
 
@@ -551,37 +535,35 @@
         return False
     else:
         old_receiver = receivers[index]
         del receivers[index]
         found = 0
         signals = connections.get(signal)
         if signals is not None:
-            for sig, recs in connections.get(signal, {}).iteritems():
+            for sig, recs in list(connections.get(signal, {}).items()):
                 if sig != signal:
                     for rec in recs:
                         if rec is old_receiver:
                             found = 1
                             break
         if not found:
             _kill_back_ref(old_receiver, senderkey)
             return True
         return False
-        
-        
+
+
 def _kill_back_ref(receiver, senderkey):
     """Do actual removal of back reference from ``receiver`` to
     ``senderkey``."""
     receiverkey = id(receiver)
     senders = senders_back.get(receiverkey, ())
     while senderkey in senders:
         try:
             senders.remove(senderkey)
-        except:
+        except Exception:
             break
     if not senders:
         try:
             del senders_back[receiverkey]
         except KeyError:
             pass
     return True
-
-
```

### Comparing `Louie-1.1/louie/saferef.py` & `Louie-2.0/louie/saferef.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,90 @@
 """Refactored 'safe reference from dispatcher.py"""
 
-import weakref
+import collections
 import traceback
+import weakref
+from functools import total_ordering
 
 
 def safe_ref(target, on_delete=None):
     """Return a *safe* weak reference to a callable target.
 
     - ``target``: The object to be weakly referenced, if it's a bound
       method reference, will create a BoundMethodWeakref, otherwise
       creates a simple weakref.
-        
+
     - ``on_delete``: If provided, will have a hard reference stored to
       the callable to be called after the safe reference goes out of
       scope with the reference object, (either a weakref or a
       BoundMethodWeakref) as argument.
     """
-    if hasattr(target, 'im_self'):
-        if target.im_self is not None:
+    if hasattr(target, "im_self"):
+        if target.__self__ is not None:
             # Turn a bound method into a BoundMethodWeakref instance.
             # Keep track of these instances for lookup by disconnect().
-            assert hasattr(target, 'im_func'), (
-                "safe_ref target %r has im_self, but no im_func, "
+            assert hasattr(target, "im_func"), (
+                f"safe_ref target {target!r} has im_self, but no im_func, "
                 "don't know how to create reference"
-                % target
-                )
+            )
+            reference = BoundMethodWeakref(target=target, on_delete=on_delete)
+            return reference
+
+    if hasattr(target, "__self__"):
+        if target.__self__ is not None:
+            assert hasattr(target, "__func__"), (
+                f"safe_ref target {target!r} has __self__, but no __func__, "
+                "don't know how to create reference"
+            )
             reference = BoundMethodWeakref(target=target, on_delete=on_delete)
             return reference
-    if callable(on_delete):
+
+    if hasattr(on_delete, "__call__"):
         return weakref.ref(target, on_delete)
     else:
         return weakref.ref(target)
-    
 
+
+@total_ordering
 class BoundMethodWeakref(object):
     """'Safe' and reusable weak references to instance methods.
 
     BoundMethodWeakref objects provide a mechanism for referencing a
     bound method without requiring that the method object itself
     (which is normally a transient object) is kept alive.  Instead,
     the BoundMethodWeakref object keeps weak references to both the
     object and the function which together define the instance method.
 
     Attributes:
-    
+
     - ``key``: The identity key for the reference, calculated by the
       class's calculate_key method applied to the target instance method.
 
     - ``deletion_methods``: Sequence of callable objects taking single
       argument, a reference to this object which will be called when
       *either* the target object or target function is garbage
       collected (i.e. when this object becomes invalid).  These are
       specified as the on_delete parameters of safe_ref calls.
 
     - ``weak_self``: Weak reference to the target object.
 
     - ``weak_func``: Weak reference to the target function.
 
     Class Attributes:
-        
+
     - ``_all_instances``: Class attribute pointing to all live
       BoundMethodWeakref objects indexed by the class's
       calculate_key(target) method applied to the target objects.
       This weak value dictionary is used to short-circuit creation so
       that multiple references to the same (object, function) pair
       produce the same BoundMethodWeakref instance.
     """
-    
+
     _all_instances = weakref.WeakValueDictionary()
-    
+
     def __new__(cls, target, on_delete=None, *arguments, **named):
         """Create new instance or return current instance.
 
         Basically this method of construction allows us to
         short-circuit creation of references to already- referenced
         instance methods.  The key corresponding to the target is
         calculated, and if there is already an existing reference,
@@ -94,76 +106,97 @@
     def __init__(self, target, on_delete=None):
         """Return a weak-reference-like instance for a bound method.
 
         - ``target``: The instance-method target for the weak reference,
           must have im_self and im_func attributes and be
           reconstructable via the following, which is true of built-in
           instance methods::
-            
+
             target.im_func.__get__( target.im_self )
 
         - ``on_delete``: Optional callback which will be called when
           this weak reference ceases to be valid (i.e. either the
           object or the function is garbage collected).  Should take a
           single argument, which will be passed a pointer to this
           object.
         """
-        def remove(weak, self=self):
+
+        def remove(weak, self_=self):
             """Set self.isDead to True when method or instance is destroyed."""
-            methods = self.deletion_methods[:]
-            del self.deletion_methods[:]
+            methods = self_.deletion_methods[:]
+            del self_.deletion_methods[:]
             try:
-                del self.__class__._all_instances[self.key]
+                del self_.__class__._all_instances[self_.key]
             except KeyError:
                 pass
             for function in methods:
                 try:
-                    if callable(function):
-                        function(self)
+                    if isinstance(function, collections.Callable):
+                        function(self_)
                 except Exception:
                     try:
                         traceback.print_exc()
-                    except AttributeError, e:
-                        print ('Exception during saferef %s '
-                               'cleanup function %s: %s' % (self, function, e))
+                    except AttributeError as e:
+                        print(
+                            f"Exception during saferef {self_} "
+                            f"cleanup function {function}: {e}"
+                        )
+
         self.deletion_methods = [on_delete]
         self.key = self.calculate_key(target)
-        self.weak_self = weakref.ref(target.im_self, remove)
-        self.weak_func = weakref.ref(target.im_func, remove)
-        self.self_name = str(target.im_self)
-        self.func_name = str(target.im_func.__name__)
-        
+        try:
+            self.weak_self = weakref.ref(target.__self__, remove)
+            self.weak_func = weakref.ref(target.__func__, remove)
+            self.self_name = str(target.__self__)
+            self.__name__ = str(target.__func__.__name__)
+        except AttributeError:
+            self.weak_self = weakref.ref(target.__self__, remove)
+            self.weak_func = weakref.ref(target.__func__, remove)
+            self.self_name = str(target.__self__)
+            self.__name__ = str(target.__func__.__name__)
+
+    @classmethod
     def calculate_key(cls, target):
         """Calculate the reference key for this reference.
 
         Currently this is a two-tuple of the id()'s of the target
         object and the target function respectively.
         """
-        return (id(target.im_self), id(target.im_func))
-    calculate_key = classmethod(calculate_key)
-    
+        return id(target.__self__), id(target.__func__)
+
     def __str__(self):
         """Give a friendly representation of the object."""
-        return "%s(%s.%s)" % (
-            self.__class__.__name__,
-            self.self_name,
-            self.func_name,
-            )
-    
+        return f"{self.__class__.__name__}({self.self_name}.{self.__name__})"
+
     __repr__ = __str__
-    
-    def __nonzero__(self):
+
+    def __bool__(self):
         """Whether we are still a valid reference."""
         return self() is not None
 
-    def __cmp__(self, other):
+    def __eq__(self, other):
+        """Compare with another reference."""
+        if not isinstance(other, self.__class__):
+            return self.__class__ is type(other)
+        else:
+            return self.key == other.key
+
+    def __ne__(self, other):
+        """Compare with another reference."""
+        if not isinstance(other, self.__class__):
+            return self.__class__ is not type(other)
+        else:
+            return self.key != other.key
+
+    def __lt__(self, other):
         """Compare with another reference."""
         if not isinstance(other, self.__class__):
-            return cmp(self.__class__, type(other))
-        return cmp(self.key, other.key)
+            return self.__class__ < type(other)
+        else:
+            return self.key < other.key
 
     def __call__(self):
         """Return a strong reference to the bound method.
 
         If the target cannot be retrieved, then will return None,
         otherwise returns a bound instance method for our object and
         function.
@@ -173,7 +206,10 @@
         """
         target = self.weak_self()
         if target is not None:
             function = self.weak_func()
             if function is not None:
                 return function.__get__(target)
         return None
+
+    def __hash__(self):
+        return hash(self.key)
```

### Comparing `Louie-1.1/louie/signal.py` & `Louie-2.0/louie/signal.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 """
 
 
 class _SIGNAL(type):
     """Base metaclass for signal classes."""
 
     def __str__(cls):
-        return '<Signal: %s>' % (cls.__name__, )
+        return f"<Signal: {cls.__name__}>"
 
 
-class Signal(object):
-
-    __metaclass__ = _SIGNAL
+class Signal(object, metaclass=_SIGNAL):
+    pass
 
 
 class All(Signal):
     """Used to represent 'all signals'.
 
     The All class can be used with connect, disconnect, send, or
     sendExact to denote that the signal should react to all signals,
     not just a particular signal.
     """
-
```

### Comparing `Louie-1.1/louie/plugin.py` & `Louie-2.0/louie/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Common plugins for Louie."""
 
-from louie import dispatcher
-from louie import error
+from louie import dispatcher, error
 
 
 def install_plugin(plugin):
     cls = plugin.__class__
     for p in dispatcher.plugins:
         if p.__class__ is cls:
-            raise error.PluginTypeError(
-                'Plugin of type %r already installed.' % cls)
+            raise error.PluginTypeError(f"Plugin of type {cls!r} already installed.")
     dispatcher.plugins.append(plugin)
 
+
 def remove_plugin(plugin):
     dispatcher.plugins.remove(plugin)
 
 
 class Plugin(object):
     """Base class for Louie plugins.
 
@@ -62,19 +61,19 @@
             self.is_live = self._is_live_no_qt
         else:
             self.qt = qt
 
     def is_live(self, receiver):
         """If receiver is a method on a QWidget, only return True if
         it hasn't been destroyed."""
-        if (hasattr(receiver, 'im_self') and
-            isinstance(receiver.im_self, self.qt.QWidget)
-            ):
+        if hasattr(receiver, "im_self") and isinstance(
+            receiver.__self__, self.qt.QWidget
+        ):
             try:
-                receiver.im_self.x()
+                receiver.__self__.x()
             except RuntimeError:
                 return False
         return True
 
     def _is_live_no_qt(self, receiver):
         return True
 
@@ -89,20 +88,23 @@
     """
 
     def __init__(self):
         # Don't import reactor ourselves, but make access to it
         # easier.
         from twisted import internet
         from twisted.internet.defer import Deferred
+
         self._internet = internet
         self._Deferred = Deferred
 
     def wrap_receiver(self, receiver):
         def wrapper(*args, **kw):
             d = self._Deferred()
+
             def called(dummy):
                 return receiver(*args, **kw)
+
             d.addCallback(called)
             self._internet.reactor.callLater(0, d.callback, None)
             return d
-        return wrapper
 
+        return wrapper
```

