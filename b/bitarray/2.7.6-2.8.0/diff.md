# Comparing `tmp/bitarray-2.7.6.tar.gz` & `tmp/bitarray-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitarray-2.7.6.tar", last modified: Sat Jun 24 21:19:34 2023, max compression
+gzip compressed data, was "bitarray-2.8.0.tar", last modified: Sat Jul 22 05:53:27 2023, max compression
```

## Comparing `bitarray-2.7.6.tar` & `bitarray-2.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:19:34.746963 bitarray-2.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-24 21:19:23.000000 bitarray-2.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-06-24 21:19:34.742963 bitarray-2.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31369 2023-06-24 21:19:23.000000 bitarray-2.7.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:19:34.742963 bitarray-2.7.6/bitarray/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   116910 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/_bitarray.c
--rw-r--r--   0 runner    (1001) docker     (123)    62914 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/_util.c
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/bitarray.h
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/pythoncapi_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)   164453 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/test_bitarray.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/test_data.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    88048 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-24 21:19:23.000000 bitarray-2.7.6/bitarray/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:19:34.742963 bitarray-2.7.6/bitarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-06-24 21:19:34.000000 bitarray-2.7.6/bitarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-24 21:19:34.000000 bitarray-2.7.6/bitarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:19:34.000000 bitarray-2.7.6/bitarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:19:34.000000 bitarray-2.7.6/bitarray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 21:19:34.000000 bitarray-2.7.6/bitarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:19:34.746963 bitarray-2.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-24 21:19:23.000000 bitarray-2.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:53:27.087148 bitarray-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-22 05:53:19.000000 bitarray-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32782 2023-07-22 05:53:27.087148 bitarray-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31705 2023-07-22 05:53:19.000000 bitarray-2.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:53:27.087148 bitarray-2.8.0/bitarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   123740 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/_bitarray.c
+-rw-r--r--   0 runner    (1001) docker     (123)    62925 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/_util.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/bitarray.h
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/pythoncapi_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)   172338 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/test_bitarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/test_data.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    87968 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-22 05:53:19.000000 bitarray-2.8.0/bitarray/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:53:27.087148 bitarray-2.8.0/bitarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32782 2023-07-22 05:53:27.000000 bitarray-2.8.0/bitarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-22 05:53:27.000000 bitarray-2.8.0/bitarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 05:53:27.000000 bitarray-2.8.0/bitarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 05:53:26.000000 bitarray-2.8.0/bitarray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 05:53:27.000000 bitarray-2.8.0/bitarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 05:53:27.087148 bitarray-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-22 05:53:19.000000 bitarray-2.8.0/setup.py
```

### Comparing `bitarray-2.7.6/LICENSE` & `bitarray-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.6/PKG-INFO` & `bitarray-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitarray
-Version: 2.7.6
+Version: 2.8.0
 Summary: efficient arrays of booleans -- C extension
 Home-page: https://github.com/ilanschnell/bitarray
 Author: Ilan Schnell
 Author-email: ilanschnell@gmail.com
 License: PSF
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Development Status :: 6 - Mature
@@ -86,28 +86,28 @@
 
 Once you have installed the package, you may want to test it:
 
 .. code-block:: shell-session
 
     $ python -c 'import bitarray; bitarray.test()'
     bitarray is installed in: /Users/ilan/bitarray/bitarray
-    bitarray version: 2.7.6
+    bitarray version: 2.8.0
     sys.version: 3.11.0 (main, Oct 25 2022) [Clang 14.0.4]
     sys.prefix: /Users/ilan/Mini3/envs/py311
     pointer size: 64 bit
     sizeof(size_t): 8
     sizeof(bitarrayobject): 80
     __clang__ or __GNUC__ defined: 1
     PY_LITTLE_ENDIAN (use word shift): 1
     DEBUG: 0
     .........................................................................
     .........................................................................
     ................................................................
     ----------------------------------------------------------------------
-    Ran 468 tests in 0.460s
+    Ran 485 tests in 0.465s
 
     OK
 
 The ``test()`` function is part of the API.  It will return
 a ``unittest.runner.TextTestResult`` object, such that one can verify that
 all tests ran successfully by:
 
@@ -203,14 +203,18 @@
 
     >>> a = bitarray(30)
     >>> a[:] = 0         # set all elements to 0 - equivalent to a.setall(0)
     >>> a[10:25] = 1     # set elements in range(10, 25) to 1
     >>> a
     bitarray('000000000011111111111111100000')
 
+As of bitarray version 2.8, indices may also be lists of arbitrary
+indices (like in NumPy), or bitarrays that are treated as masks,
+see `Bitarray indexing <https://github.com/ilanschnell/bitarray/blob/master/doc/indexing.rst>`__.
+
 
 Bitwise operators
 -----------------
 
 Bitarray objects support the bitwise operators ``~``, ``&``, ``|``, ``^``,
 ``<<``, ``>>`` (as well as their in-place versions ``&=``, ``|=``, ``^=``,
 ``<<=``, ``>>=``).  The behavior is very much what one would expect:
@@ -430,15 +434,15 @@
         ...
     TypeError: frozenbitarray is immutable
 
 
 Reference
 =========
 
-bitarray version: 2.7.6 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
+bitarray version: 2.8.0 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
 
 In the following, ``item`` and ``value`` are usually a single bit -
 an integer 0 or 1.
 
 
 The bitarray object:
 --------------------
@@ -498,15 +502,16 @@
    7. number of buffer exports
 
 
 ``bytereverse(start=0, stop=<end of buffer>, /)``
    For each byte in byte-range(start, stop) reverse the bit order in-place.
    The start and stop indices are given in terms of bytes (not bits).
    Also note that this method only changes the buffer; it does not change the
-   endianness of the bitarray object.
+   endianness of the bitarray object.  Padbits are left unchanged such that
+   two consecutive calls will always leave the bitarray unchanged.
 
    New in version 2.2.5: optional start and stop arguments.
 
 
 ``clear()``
    Remove all items from the bitarray.
```

### Comparing `bitarray-2.7.6/README.rst` & `bitarray-2.8.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -59,28 +59,28 @@
 
 Once you have installed the package, you may want to test it:
 
 .. code-block:: shell-session
 
     $ python -c 'import bitarray; bitarray.test()'
     bitarray is installed in: /Users/ilan/bitarray/bitarray
-    bitarray version: 2.7.6
+    bitarray version: 2.8.0
     sys.version: 3.11.0 (main, Oct 25 2022) [Clang 14.0.4]
     sys.prefix: /Users/ilan/Mini3/envs/py311
     pointer size: 64 bit
     sizeof(size_t): 8
     sizeof(bitarrayobject): 80
     __clang__ or __GNUC__ defined: 1
     PY_LITTLE_ENDIAN (use word shift): 1
     DEBUG: 0
     .........................................................................
     .........................................................................
     ................................................................
     ----------------------------------------------------------------------
-    Ran 468 tests in 0.460s
+    Ran 485 tests in 0.465s
 
     OK
 
 The ``test()`` function is part of the API.  It will return
 a ``unittest.runner.TextTestResult`` object, such that one can verify that
 all tests ran successfully by:
 
@@ -176,14 +176,18 @@
 
     >>> a = bitarray(30)
     >>> a[:] = 0         # set all elements to 0 - equivalent to a.setall(0)
     >>> a[10:25] = 1     # set elements in range(10, 25) to 1
     >>> a
     bitarray('000000000011111111111111100000')
 
+As of bitarray version 2.8, indices may also be lists of arbitrary
+indices (like in NumPy), or bitarrays that are treated as masks,
+see `Bitarray indexing <https://github.com/ilanschnell/bitarray/blob/master/doc/indexing.rst>`__.
+
 
 Bitwise operators
 -----------------
 
 Bitarray objects support the bitwise operators ``~``, ``&``, ``|``, ``^``,
 ``<<``, ``>>`` (as well as their in-place versions ``&=``, ``|=``, ``^=``,
 ``<<=``, ``>>=``).  The behavior is very much what one would expect:
@@ -403,15 +407,15 @@
         ...
     TypeError: frozenbitarray is immutable
 
 
 Reference
 =========
 
-bitarray version: 2.7.6 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
+bitarray version: 2.8.0 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
 
 In the following, ``item`` and ``value`` are usually a single bit -
 an integer 0 or 1.
 
 
 The bitarray object:
 --------------------
@@ -471,15 +475,16 @@
    7. number of buffer exports
 
 
 ``bytereverse(start=0, stop=<end of buffer>, /)``
    For each byte in byte-range(start, stop) reverse the bit order in-place.
    The start and stop indices are given in terms of bytes (not bits).
    Also note that this method only changes the buffer; it does not change the
-   endianness of the bitarray object.
+   endianness of the bitarray object.  Padbits are left unchanged such that
+   two consecutive calls will always leave the bitarray unchanged.
 
    New in version 2.2.5: optional start and stop arguments.
 
 
 ``clear()``
    Remove all items from the bitarray.
```

### Comparing `bitarray-2.7.6/bitarray/__init__.py` & `bitarray-2.8.0/bitarray/__init__.py`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.6/bitarray/__init__.pyi` & `bitarray-2.8.0/bitarray/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2021 - 2023, Ilan Schnell; All Rights Reserved
 #
 # This stub, as well as util.pyi, are tested with Python 3.9 and mypy 0.950
 
-from collections.abc import Iterable, Iterator
+from collections.abc import Iterable, Iterator, Sequence
 from unittest.runner import TextTestResult
 
 from typing import Any, BinaryIO, Dict, Union, overload
 
 
 CodeDict = Dict[Any, bitarray]
 BytesLike = Union[bytes, Iterable[int]]
@@ -82,20 +82,20 @@
                one: bytes = ...) -> bytes: ...
 
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[int]: ...
     @overload
     def __getitem__(self, i: int) -> int: ...
     @overload
-    def __getitem__(self, s: slice) -> bitarray: ...
+    def __getitem__(self, s: Union[slice, Sequence]) -> bitarray: ...
     @overload
-    def __setitem__(self, i: Union[int, slice], o: int) -> None: ...
+    def __setitem__(self, i: Union[int, slice, Sequence], o: int) -> None: ...
     @overload
-    def __setitem__(self, s: slice, o: bitarray) -> None: ...
-    def __delitem__(self, i: Union[int, slice]) -> None: ...
+    def __setitem__(self, s: Union[slice, Sequence] , o: bitarray) -> None: ...
+    def __delitem__(self, i: Union[int, slice, Sequence]) -> None: ...
 
     def __add__(self, other: bitarray) -> bitarray: ...
     def __iadd__(self, other: bitarray) -> bitarray: ...
     def __mul__(self, n: int) -> bitarray: ...
     def __imul__(self, n: int) -> bitarray: ...
     def __rmul__(self, n: int) -> bitarray: ...
```

### Comparing `bitarray-2.7.6/bitarray/_bitarray.c` & `bitarray-2.8.0/bitarray/_bitarray.c`

 * *Files 3% similar despite different names*

```diff
@@ -882,15 +882,16 @@
 
 PyDoc_STRVAR(bytereverse_doc,
 "bytereverse(start=0, stop=<end of buffer>, /)\n\
 \n\
 For each byte in byte-range(start, stop) reverse the bit order in-place.\n\
 The start and stop indices are given in terms of bytes (not bits).\n\
 Also note that this method only changes the buffer; it does not change the\n\
-endianness of the bitarray object.");
+endianness of the bitarray object.  Padbits are left unchanged such that\n\
+two consecutive calls will always leave the bitarray unchanged.");
 
 
 static PyObject *
 bitarray_buffer_info(bitarrayobject *self)
 {
     PyObject *res, *ptr;
 
@@ -1935,63 +1936,169 @@
     (objobjproc) bitarray_contains,             /* sq_contains */
     (binaryfunc) bitarray_inplace_concat,       /* sq_inplace_concat */
     (ssizeargfunc) bitarray_inplace_repeat,     /* sq_inplace_repeat */
 };
 
 /* ----------------------- bitarray_as_mapping ------------------------- */
 
+/* return new bitarray with item in self, specified by slice */
+static PyObject *
+getslice(bitarrayobject *self, PyObject *slice)
+{
+    Py_ssize_t start, stop, step, slicelength;
+    PyObject *res;
+
+    assert(PySlice_Check(slice));
+    if (PySlice_GetIndicesEx(slice, self->nbits,
+                             &start, &stop, &step, &slicelength) < 0)
+        return NULL;
+
+    res = newbitarrayobject(Py_TYPE(self), slicelength, self->endian);
+    if (res == NULL)
+        return NULL;
+
+#define rr  ((bitarrayobject *) res)
+    if (step == 1) {
+        copy_n(rr, 0, self, start, slicelength);
+    }
+    else {
+        Py_ssize_t i, j;
+
+        for (i = 0, j = start; i < slicelength; i++, j += step)
+            setbit(rr, i, getbit(self, j));
+    }
+#undef rr
+    return res;
+}
+
+static int
+check_mask_length(bitarrayobject *self, bitarrayobject *mask)
+{
+    if (self->nbits != mask->nbits) {
+        PyErr_Format(PyExc_IndexError, "bitarray length is %zd, but "
+                     "mask has length %zd", self->nbits, mask->nbits);
+        return -1;
+    }
+    return 0;
+}
+
+/* return a new bitarray with items from 'self' masked by bitarray 'mask' */
+static PyObject *
+getmasked(bitarrayobject *self, bitarrayobject *mask)
+{
+    PyObject *res;
+    Py_ssize_t i, j, n;
+
+    if (check_mask_length(self, mask) < 0)
+        return NULL;
+
+    n = count(mask, 0, mask->nbits);
+    res = newbitarrayobject(Py_TYPE(self), n, self->endian);
+    if (res == NULL)
+        return NULL;
+
+    for (i = j = 0; i < mask->nbits; i++) {
+        if (getbit(mask, i))
+            setbit((bitarrayobject *) res, j++, getbit(self, i));
+    }
+    assert(j == n);
+    return res;
+}
+
+/* Return j-th item from sequence.  The item is considered an index into
+   an array with given length, and is normalized a pythonic manner.
+   On failure, an exception is set and -1 is returned. */
+static Py_ssize_t
+index_from_seq(PyObject *sequence, Py_ssize_t j, Py_ssize_t length)
+{
+    PyObject *item;
+    Py_ssize_t i;
+
+    if ((item = PySequence_GetItem(sequence, j)) == NULL)
+        return -1;
+
+    i = PyNumber_AsSsize_t(item, PyExc_IndexError);
+    Py_DECREF(item);
+    if (i == -1 && PyErr_Occurred())
+        return -1;
+    if (i < 0)
+        i += length;
+    if (i < 0 || i >= length) {
+        PyErr_SetString(PyExc_IndexError, "bitarray index out of range");
+        return -1;
+    }
+    return i;
+}
+
+/* return a new bitarray with items from 'self' listed by
+   sequence (of indices) 'seq' */
+static PyObject *
+getsequence(bitarrayobject *self, PyObject *seq)
+{
+    PyObject *res;
+    Py_ssize_t i, j, n;
+
+    n = PySequence_Size(seq);
+    res = newbitarrayobject(Py_TYPE(self), n, self->endian);
+    if (res == NULL)
+        return NULL;
+
+    for (j = 0; j < n; j++) {
+        if ((i = index_from_seq(seq, j, self->nbits)) < 0) {
+            Py_DECREF(res);
+            return NULL;
+        }
+        setbit((bitarrayobject *) res, j, getbit(self, i));
+    }
+    return res;
+}
+
+static int
+subscr_seq_check(PyObject *item)
+{
+    if (PyTuple_Check(item)) {
+        PyErr_SetString(PyExc_TypeError, "multiple dimensions not supported");
+        return -1;
+    }
+    if (PySequence_Check(item))
+        return 0;
+
+    PyErr_Format(PyExc_TypeError, "bitarray indices must be integers, "
+                 "slices or sequences, not '%s'", Py_TYPE(item)->tp_name);
+    return -1;
+}
+
 static PyObject *
 bitarray_subscr(bitarrayobject *self, PyObject *item)
 {
     if (PyIndex_Check(item)) {
         Py_ssize_t i;
 
         i = PyNumber_AsSsize_t(item, PyExc_IndexError);
         if (i == -1 && PyErr_Occurred())
             return NULL;
         if (i < 0)
             i += self->nbits;
         return bitarray_item(self, i);
     }
 
-    if (PySlice_Check(item)) {
-        Py_ssize_t start, stop, step, slicelength;
-        PyObject *res;
+    if (PySlice_Check(item))
+        return getslice(self, item);
 
-        if (PySlice_GetIndicesEx(item, self->nbits,
-                                 &start, &stop, &step, &slicelength) < 0)
-            return NULL;
-
-        res = newbitarrayobject(Py_TYPE(self), slicelength, self->endian);
-        if (res == NULL)
-            return NULL;
+    if (bitarray_Check(item))
+        return getmasked(self, (bitarrayobject *) item);
 
-#define rr  ((bitarrayobject *) res)
-        if (step == 1) {
-            copy_n(rr, 0, self, start, slicelength);
-        }
-        else {
-            Py_ssize_t i, j;
-
-            for (i = 0, j = start; i < slicelength; i++, j += step)
-                setbit(rr, i, getbit(self, j));
-        }
-#undef rr
-        return res;
-    }
+    if (subscr_seq_check(item) < 0)
+        return NULL;
 
-    return PyErr_Format(PyExc_TypeError,
-                        "bitarray indices must be integers or slices, not %s",
-                        Py_TYPE(item)->tp_name);
+    return getsequence(self, item);
 }
 
 /* The following functions, namely setslice_bitarray(), setslice_bool() and
-   delslice(), are called from bitarray_ass_subscr().  Having all this
-   functionality inside bitarray_ass_subscr() would make the function
-   incomprehensibly long. */
+   delslice(), are called from assign_slice(). */
 
 /* set items in self, specified by slice, to other bitarray */
 static int
 setslice_bitarray(bitarrayobject *self, PyObject *slice,
                   bitarrayobject *other)
 {
     Py_ssize_t start, stop, step, slicelength, increase;
@@ -2104,14 +2211,168 @@
             if ((i - start) % step != 0)
                 setbit(self, j++, getbit(self, i));
         }
     }
     return delete_n(self, stop - slicelength, slicelength);
 }
 
+/* assign slice of bitarray self to value */
+static int
+assign_slice(bitarrayobject *self, PyObject *slice, PyObject *value)
+{
+    if (value == NULL)
+        return delslice(self, slice);
+
+    if (bitarray_Check(value))
+        return setslice_bitarray(self, slice, (bitarrayobject *) value);
+
+    if (PyIndex_Check(value))
+        return setslice_bool(self, slice, value);
+
+    PyErr_Format(PyExc_TypeError,
+                 "bitarray or int expected for slice assignment, not '%s'",
+                 Py_TYPE(value)->tp_name);
+    return -1;
+}
+
+/* delete items in self, specified by mask */
+static int
+delmask(bitarrayobject *self, bitarrayobject *mask)
+{
+    Py_ssize_t n = 0, i;
+
+    if (check_mask_length(self, mask) < 0)
+        return -1;
+
+    for (i = 0; i < mask->nbits; i++) {
+        if (getbit(mask, i) == 0)  /* set items we want to keep */
+            setbit(self, n++, getbit(self, i));
+    }
+    assert(self == mask || n == mask->nbits - count(mask, 0, mask->nbits));
+
+    return resize(self, n);
+}
+
+/* assign mask of bitarray self to value */
+static int
+assign_mask(bitarrayobject *self, bitarrayobject *mask, PyObject *value)
+{
+    if (value == NULL)
+        return delmask(self, mask);
+
+    PyErr_SetString(PyExc_NotImplementedError, "masked assignment "
+                    "not implemented - use bitwise operations");
+    return -1;
+}
+
+/* assign sequence (of indices) of bitarray self to Boolean value */
+static int
+setseq_bool(bitarrayobject *self, PyObject *seq, PyObject *value)
+{
+    Py_ssize_t n, i, j;
+    int vi;
+
+    if (!conv_pybit(value, &vi))
+        return -1;
+
+    n = PySequence_Size(seq);
+    for (j = 0; j < n; j++) {
+        if ((i = index_from_seq(seq, j, self->nbits)) < 0)
+            return -1;
+        setbit(self, i, vi);
+    }
+    return 0;
+}
+
+/* assign sequence (of indices) of bitarray self to bitarray */
+static int
+setseq_bitarray(bitarrayobject *self, PyObject *seq, bitarrayobject *other)
+{
+    Py_ssize_t n, i, j;
+    int other_copied = 0, res = -1;
+
+    n = PySequence_Size(seq);
+    if (n != other->nbits) {
+        PyErr_Format(PyExc_ValueError, "attempt to assign sequence of "
+                     "size %zd to bitarray of size %zd",
+                     n, other->nbits);
+        return -1;
+    }
+    /* Make a copy of other, in case the buffers overlap.  This is obviously
+       the case when self and other are the same object, but can also happen
+       when the two bitarrays share memory. */
+    if (buffers_overlap(self, other)) {
+        other = (bitarrayobject *) bitarray_copy(other);
+        if (other == NULL)
+            return -1;
+        other_copied = 1;
+    }
+
+    for (j = 0; j < n; j++) {
+        if ((i = index_from_seq(seq, j, self->nbits)) < 0)
+            goto error;
+        setbit(self, i, getbit(other, j));
+    }
+    res = 0;
+ error:
+    if (other_copied)
+        Py_DECREF(other);
+    return res;
+}
+
+/* delete items in self, specified by sequence of indices */
+static int
+delsequence(bitarrayobject *self, PyObject *seq)
+{
+    bitarrayobject *mask;  /* temporary bitarray masking items to remove */
+    Py_ssize_t nseq, i, j;
+    int res = -1;
+
+    nseq = PySequence_Size(seq);
+    if (nseq == 0)   /* shortcut - sequence is empty - nothing to delete */
+        return 0;
+
+    /* create mask bitarray - note that it's endianness is irrelevant */
+    mask = (bitarrayobject *) newbitarrayobject(&Bitarray_Type, self->nbits,
+                                                ENDIAN_LITTLE);
+    if (mask == NULL)
+        return -1;
+    memset(mask->ob_item, 0x00, (size_t) Py_SIZE(mask));
+
+    /* set indices from sequence in mask */
+    for (j = 0; j < nseq; j++) {
+        if ((i = index_from_seq(seq, j, self->nbits)) < 0)
+            goto error;
+        setbit(mask, i, 1);
+    }
+    res = delmask(self, mask);  /* do actual work here */
+ error:
+    Py_DECREF(mask);
+    return res;
+}
+
+/* assign sequence (of indices) of bitarray self to value */
+static int
+assign_sequence(bitarrayobject *self, PyObject *seq, PyObject *value)
+{
+    if (value == NULL)
+        return delsequence(self, seq);
+
+    if (bitarray_Check(value))
+        return setseq_bitarray(self, seq, (bitarrayobject *) value);
+
+    if (PyIndex_Check(value))
+        return setseq_bool(self, seq, value);
+
+    PyErr_Format(PyExc_TypeError,
+                 "bitarray or int expected for sequence assignment, not '%s'",
+                 Py_TYPE(value)->tp_name);
+    return -1;
+}
+
 static int
 bitarray_ass_subscr(bitarrayobject *self, PyObject *item, PyObject *value)
 {
     RAISE_IF_READONLY(self, -1);
 
     if (PyIndex_Check(item)) {
         Py_ssize_t i;
@@ -2120,34 +2381,24 @@
         if (i == -1 && PyErr_Occurred())
             return -1;
         if (i < 0)
             i += self->nbits;
         return bitarray_ass_item(self, i, value);
     }
 
-    if (PySlice_Check(item)) {
-        if (value == NULL)
-            return delslice(self, item);
+    if (PySlice_Check(item))
+        return assign_slice(self, item, value);
 
-        if (bitarray_Check(value))
-            return setslice_bitarray(self, item, (bitarrayobject *) value);
+    if (bitarray_Check(item))
+        return assign_mask(self, (bitarrayobject *) item, value);
 
-        if (PyIndex_Check(value))
-            return setslice_bool(self, item, value);
-
-        PyErr_Format(PyExc_TypeError,
-                     "bitarray or int expected for slice assignment, not %s",
-                     Py_TYPE(value)->tp_name);
+    if (subscr_seq_check(item) < 0)
         return -1;
-    }
 
-    PyErr_Format(PyExc_TypeError,
-                 "bitarray indices must be integers or slices, not %s",
-                 Py_TYPE(item)->tp_name);
-    return -1;
+    return assign_sequence(self, item, value);
 }
 
 static PyMappingMethods bitarray_as_mapping = {
     (lenfunc) bitarray_len,
     (binaryfunc) bitarray_subscr,
     (objobjargproc) bitarray_ass_subscr,
 };
@@ -2398,15 +2649,15 @@
                     variable length encoding and decoding
  **************************************************************************/
 
 static int
 check_codedict(PyObject *codedict)
 {
     if (!PyDict_Check(codedict)) {
-        PyErr_Format(PyExc_TypeError, "dict expected, got %s",
+        PyErr_Format(PyExc_TypeError, "dict expected, got '%s'",
                      Py_TYPE(codedict)->tp_name);
         return -1;
     }
     if (PyDict_Size(codedict) == 0) {
         PyErr_SetString(PyExc_ValueError, "non-empty dict expected");
         return -1;
     }
@@ -3405,14 +3656,15 @@
     /* bytes (for pickling) - must have head byte (0x00 .. 0x07) */
     if (PyBytes_Check(initial) && PyBytes_GET_SIZE(initial) > 0) {
         char head = *PyBytes_AS_STRING(initial);
         if ((head & 0xf8) == 0)
             return newbitarray_from_pickle(type, initial, endian_str);
     }
 
+    /* bitarray: use its endianness (when endian argument missing) */
     if (bitarray_Check(initial) && endian_str == NULL)
         endian = ((bitarrayobject *) initial)->endian;
 
     /* leave remaining type dispatch to extend method */
     result = newbitarrayobject(type, 0, endian);
     if (result == NULL)
         return NULL;
```

### Comparing `bitarray-2.7.6/bitarray/_util.c` & `bitarray-2.8.0/bitarray/_util.c`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 {
     int t;
 
     t = PyObject_IsInstance(obj, bitarray_type_obj);
     if (t < 0)
         return -1;
     if (t == 0) {
-        PyErr_Format(PyExc_TypeError, "bitarray expected, not %s",
+        PyErr_Format(PyExc_TypeError, "bitarray expected, not '%s'",
                      Py_TYPE(obj)->tp_name);
         return -1;
     }
     return 0;
 }
 
 /* return new bitarray of length `nbits` (with uninitialized buffer) and
@@ -1820,15 +1820,15 @@
 static PyObject *
 chdi_new(PyObject *module, PyObject *args)
 {
     PyObject *a, *count, *symbol;
     Py_ssize_t count_sum;
     chdi_obj *it;       /* iterator object to be returned */
 
-    if (!PyArg_ParseTuple(args, "O!OO:count_n",
+    if (!PyArg_ParseTuple(args, "O!OO:canonical_decode",
                           bitarray_type_obj, &a, &count, &symbol))
         return NULL;
     if (!PySequence_Check(count))
         return PyErr_Format(PyExc_TypeError, "count expected to be sequence, "
                             "got '%s'", Py_TYPE(count)->tp_name);
 
     symbol = PySequence_Fast(symbol, "symbol not iterable");
```

### Comparing `bitarray-2.7.6/bitarray/bitarray.h` & `bitarray-2.8.0/bitarray/bitarray.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
    Copyright (c) 2008 - 2023, Ilan Schnell; All Rights Reserved
    bitarray is published under the PSF license.
 
    Author: Ilan Schnell
 */
-#define BITARRAY_VERSION  "2.7.6"
+#define BITARRAY_VERSION  "2.8.0"
 
 #ifdef STDC_HEADERS
 #include <stddef.h>
 #else  /* !STDC_HEADERS */
 #ifdef HAVE_SYS_TYPES_H
 #include <sys/types.h>      /* For size_t */
 #endif /* HAVE_SYS_TYPES_H */
```

### Comparing `bitarray-2.7.6/bitarray/pythoncapi_compat.h` & `bitarray-2.8.0/bitarray/pythoncapi_compat.h`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.6/bitarray/test_bitarray.py` & `bitarray-2.8.0/bitarray/test_bitarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import re
 import os
 import sys
 import platform
 import unittest
 import shutil
 import tempfile
-from random import randint
+from random import randint, shuffle
 
 # imports needed inside tests
 import array
 import copy
 import itertools
 import mmap
 import pickle
@@ -883,15 +883,14 @@
         self.assertEQUAL(a[8:], bitarray('00001'))
         self.assertEQUAL(a[7:], bitarray('100001'))
         self.assertEQUAL(a[:8], bitarray('01001111'))
         self.assertEQUAL(a[::-1], bitarray('10000111 10010'))
         self.assertEQUAL(a[:8:-1], bitarray('1000'))
 
         self.assertRaises(ValueError, a.__getitem__, slice(None, None, 0))
-        self.assertRaises(TypeError, a.__getitem__, (1, 2))
 
     def test_getslice_random(self):
         for a in self.randombitarrays(start=1):
             aa = a.tolist()
             la = len(a)
             for _ in range(10):
                 step = self.rndsliceidx(la) or None
@@ -1246,32 +1245,30 @@
     def test_setslice_bool_simple(self):
         for _ in range(100):
             N = randint(100, 2000)
             s = slice(randint(0, 20), randint(N - 20, N), randint(1, 20))
             a = zeros(N)
             a[s] = 1
             b = zeros(N)
-            for i in range(s.start, s.stop, s.step):
-                b[i] = 1
+            b[list(range(s.start, s.stop, s.step))] = 1
             self.assertEqual(a, b)
 
     def test_setslice_bool_range(self):
         N = 200
         a = bitarray(N, self.random_endian())
         b = bitarray(N)
         for step in range(-N - 1, N):
             if step == 0:
                 continue
             v = randint(0, 1)
             a.setall(not v)
             a[::step] = v
 
             b.setall(not v)
-            for i in range(0, N, abs(step)):
-                b[i] = v
+            b[list(range(0, N, abs(step)))] = v
             if step < 0:
                 b.reverse()
             self.assertEqual(a, b)
 
     def test_setslice_bool_random(self):
         N = 100
         a = bitarray(N)
@@ -1418,14 +1415,227 @@
             del lst[::step]
             self.assertEqual(a.tolist(), lst)
 
 tests.append(SliceTests)
 
 # ---------------------------------------------------------------------------
 
+class MaskedIndexTests(unittest.TestCase, Util):
+
+    def test_get_basic(self):
+        a =    bitarray('1001001')
+        mask = bitarray('1010111')
+        self.assertEqual(a[mask], bitarray('10001'))
+        self.assertRaises(IndexError, a.__getitem__, bitarray('1011'))
+
+    def test_get_random(self):
+        for a in self.randombitarrays():
+            n = len(a)
+            self.assertEqual(a[a], a.count() * bitarray('1'))
+
+            mask = zeros(n)
+            self.assertEqual(a[mask], bitarray())
+
+            mask.setall(1)
+            self.assertEqual(a[mask], a)
+
+            mask = urandom(n)
+            res = bitarray(a[i] for i in range(n) if mask[i])
+            self.assertEqual(a[mask], res)
+
+    def test_set_basic(self):
+        a =    bitarray('1001001')
+        mask = bitarray('1010111')
+        self.assertRaises(NotImplementedError, a.__setitem__, mask, 1)
+
+    def test_del_basic(self):
+        a =    bitarray('1001001')
+        mask = bitarray('1010111')
+        del a[mask]
+        self.assertEqual(a, bitarray('01'))
+        self.assertRaises(IndexError, a.__delitem__, bitarray('101'))
+
+    def test_del_random(self):
+        for a in self.randombitarrays():
+            n = len(a)
+            b = a.copy()
+            # mask has only zeros - nothing will be removed
+            mask = zeros(n)
+            del b[mask]
+            self.assertEqual(b, a)
+
+            b = a.copy()
+            # mask has only ones - everything will be removed
+            mask.setall(1)
+            del b[mask]
+            self.assertEqual(b, bitarray())
+
+            b = a.copy()
+            # mask is bitarray itself - all 1 items are removed -
+            # only all the 0's remain
+            del b[b]
+            self.assertEqual(b, zeros(a.count(0)))
+
+            b = a.copy()
+            mask = urandom(n)
+            res = bitarray(a[i] for i in range(n) if not mask[i])
+            del b[mask]
+            self.assertEqual(b, res)
+            # `del a[mask]` is equivalent to the in-place version of
+            # selecting the reverse mask `a = a[~mask]`
+            self.assertEqual(a[~mask], b)
+
+tests.append(MaskedIndexTests)
+
+# ---------------------------------------------------------------------------
+
+class SequenceIndexTests(unittest.TestCase, Util):
+
+    def test_get_basic(self):
+        a = bitarray('00110101 00')
+        self.assertEqual(a[[2, 4, -3, 9]], bitarray('1010'))
+        self.assertEqual(a[71 * [2, 4, 7]], 71 * bitarray('101'))
+        self.assertEqual(a[[-1]], bitarray('0'))
+        self.assertEqual(a[[]], bitarray())
+        self.assertRaises(IndexError, a.__getitem__, [1, 10])
+        self.assertRaises(IndexError, a.__getitem__, [-11])
+
+    def test_get_types(self):
+        a = bitarray('11001101 01')
+        lst = [1, 3, -2]
+        for b in [lst, array.array('i', lst)]:
+            self.assertEqual(a[b], bitarray('100'))
+        lst[2] += len(a)
+        self.assertEqual(a[bytearray(lst)], bitarray('100'))
+        if is_py3k:
+            self.assertEqual(a[bytes(lst)], bitarray('100'))
+
+        self.assertRaises(TypeError, a.__getitem__, [2, "B"])
+        self.assertRaises(TypeError, a.__getitem__, [2, 1.2])
+        self.assertRaises(TypeError, a.__getitem__, tuple(lst))
+
+    def test_get_random(self):
+        for a in self.randombitarrays():
+            n = len(a)
+            lst = [randint(0, n - 1) for _ in range(n // 2)]
+            b = a[lst]
+            self.assertEqual(b, bitarray(a[i] for i in lst))
+            self.assertEqual(b.endian(), a.endian())
+
+    def test_set_bool_basic(self):
+        a = zeros(10)
+        a[[2, 3, 5, 7]] = 1
+        self.assertEqual(a, bitarray('00110101 00'))
+        a[[]] = 1
+        self.assertEqual(a, bitarray('00110101 00'))
+        a[[-1]] = True
+        self.assertEqual(a, bitarray('00110101 01'))
+        a[[3, -1]] = 0
+        self.assertEqual(a, bitarray('00100101 00'))
+        self.assertRaises(IndexError, a.__setitem__, [1, 10], 0)
+        self.assertRaises(ValueError, a.__setitem__, [1], 2)
+        self.assertRaises(TypeError, a.__setitem__, [1], "A")
+        self.assertRaises(TypeError, a.__setitem__, (3, -1))
+        self.assertRaises(TypeError, a.__setitem__, a)
+
+    def test_set_bool_random(self):
+        for a in self.randombitarrays():
+            n = len(a)
+            lst = [randint(0, n - 1) for _ in range(n // 2)]
+            b = a.copy()
+            for v in 0, 1:
+                a[lst] = v
+                for i in lst:
+                    b[i] = v
+                self.assertEqual(a, b)
+
+    def test_set_bitarray_basic(self):
+        a = zeros(10)
+        a[[2, 3, 5, 7]] = bitarray('1101')
+        self.assertEqual(a, bitarray('00110001 00'))
+        a[[]] = bitarray()
+        self.assertEqual(a, bitarray('00110001 00'))
+        a[[5, -1]] = bitarray('11')
+        self.assertEqual(a, bitarray('00110101 01'))
+        self.assertRaises(IndexError, a.__setitem__, [1, 10], bitarray('11'))
+        self.assertRaises(ValueError, a.__setitem__, [1], bitarray())
+        msg = "attempt to assign sequence of size 2 to bitarray of size 3"
+        self.assertRaisesMessage(ValueError, msg,
+                                 a.__setitem__, [1, 2], bitarray('001'))
+
+    def test_set_bitarray_random(self):
+        for a in self.randombitarrays():
+            n = len(a)
+            lst = [randint(0, n - 1) for _ in range(n // 2)]
+            c = urandom(len(lst))
+            b = a.copy()
+
+            a[lst] = c
+            for i, j in enumerate(lst):
+                b[j] = c[i]
+            self.assertEqual(a, b)
+
+    def test_set_bitarray_random_self(self):
+        for a in self.randombitarrays():
+            lst = list(range(len(a)))
+            shuffle(lst)
+            b = a.copy()
+            c = a.copy()
+
+            a[lst] = a
+            for i, j in enumerate(lst):
+                b[j] = c[i]
+            self.assertEqual(a, b)
+
+    def test_del_basic(self):
+        a = bitarray('00110101 00')
+        #               ^ ^  ^  ^
+        del a[[2, 4, 7, 9]]
+        self.assertEqual(a, bitarray('001100'))
+        del a[[]]  # delete nothing
+        self.assertEqual(a, bitarray('001100'))
+        a = bitarray('00110101 00')
+        del a[71 * [2, 4, 7, 9]]
+        self.assertEqual(a, bitarray('001100'))
+        self.assertRaises(IndexError, a.__delitem__, [1, 10])
+        self.assertRaises(TypeError, a.__delitem__, (1, 3))
+
+    def test_delitems_random(self):
+        for a in self.randombitarrays():
+            n = len(a)
+            lst = [randint(0, n - 1) for _ in range(n // 2)]
+            b = a.copy()
+            c = a.copy()
+            del a[lst]
+            for i in sorted(set(lst), reverse=True):
+                del b[i]
+            self.assertEqual(a, b)
+
+            lst = list(range(n))
+            shuffle(lst)
+            del c[lst]
+            self.assertEqual(len(c), 0)
+
+    def test_type_messages(self):
+        for item, msg in [
+                (tuple([1, 2]), "multiple dimensions not supported"),
+                (None, "bitarray indices must be integers, slices or "
+                       "sequences, not 'NoneType'"),
+                (0.12, "bitarray indices must be integers, slices or "
+                       "sequences, not 'float'"),
+        ]:
+            a = bitarray('10111')
+            self.assertRaisesMessage(TypeError, msg, a.__getitem__, item)
+            self.assertRaisesMessage(TypeError, msg, a.__setitem__, item, 1)
+            self.assertRaisesMessage(TypeError, msg, a.__delitem__, item)
+
+tests.append(SequenceIndexTests)
+
+# ---------------------------------------------------------------------------
+
 class MiscTests(unittest.TestCase, Util):
 
     def test_instancecheck(self):
         a = bitarray('011')
         self.assertIsInstance(a, bitarray)
         self.assertFalse(isinstance(a, str))
 
@@ -2746,25 +2956,31 @@
     def test_setall_random(self):
         for a in self.randombitarrays():
             val = randint(0, 1)
             a.setall(val)
             self.assertEqual(a, bitarray(len(a) * [val]))
             self.check_obj(a)
 
-    def test_bytereverse_explicit_all(self):
+tests.append(MethodTests)
+
+# ---------------------------------------------------------------------------
+
+class ByteReverseTests(unittest.TestCase, Util):
+
+    def test_explicit_all(self):
         for x, y in [('', ''),
                      ('11101101', '10110111'),
                      ('00000001', '10000000'),
                      ('11011111 00100000 00011111',
                       '11111011 00000100 11111000')]:
             a = bitarray(x)
             a.bytereverse()
             self.assertEqual(a, bitarray(y))
 
-    def test_bytereverse_explicit_range(self):
+    def test_explicit_range(self):
         a = bitarray('11100000 00000011 00111111 11111000')
         a.bytereverse(0, 1)  # reverse byte 0
         self.assertEqual(a, bitarray('00000111 00000011 00111111 11111000'))
         a.bytereverse(1, -1)  # reverse bytes 1 and 2
         self.assertEqual(a, bitarray('00000111 11000000 11111100 11111000'))
         a.bytereverse(2)  # reverse bytes 2 till end of buffer
         self.assertEqual(a, bitarray('00000111 11000000 00111111 00011111'))
@@ -2778,27 +2994,36 @@
         self.assertEqual(a, bitarray('11100000 00000011 00111111 11111000'))
 
         self.assertRaises(IndexError, a.bytereverse, -5)
         self.assertRaises(IndexError, a.bytereverse, 0, -5)
         self.assertRaises(IndexError, a.bytereverse, 5)
         self.assertRaises(IndexError, a.bytereverse, 0, 5)
 
-    def test_bytereverse_byte(self):
+    def test_byte(self):
         for i in range(256):
             a = bitarray()
             a.frombytes(bytearray([i]))
             self.assertEqual(len(a), 8)
             b = a.copy()
             b.bytereverse()
             self.assertEqual(b, a[::-1])
             a.reverse()
             self.assertEqual(b, a)
             self.check_obj(b)
 
-    def test_bytereverse_random(self):
+    def test_consecutive(self):
+        for a in self.randombitarrays():
+            b = a.copy()
+            # two consecutive calls to .bytereverse() leave the bitarray
+            # unchanged (even when the length is not a multiple of 8).
+            a.bytereverse()
+            a.bytereverse()
+            self.assertEQUAL(a, b)
+
+    def test_random(self):
         t = bitarray(endian=self.random_endian())
         t.frombytes(bytearray(range(256)))
         t.bytereverse()
         table = t.tobytes()  # translation table
         self.assertEqual(table[:9], b'\x00\x80\x40\xc0\x20\xa0\x60\xe0\x10')
 
         for n in range(100):
@@ -2807,23 +3032,23 @@
             j = randint(0, n)  # stop
             b = a.copy()
             memoryview(b)[i:j] = b.tobytes()[i:j].translate(table)
             a.bytereverse(i, j)
             self.assertEQUAL(a, b)
             self.check_obj(a)
 
-    def test_bytereverse_endian(self):
+    def test_endian(self):
         for n in range(20):
             a = urandom(8 * n, self.random_endian())
             b = a.copy()
             a.bytereverse()
             a = bitarray(a, self.opposite_endian(a.endian()))
             self.assertEqual(a.tobytes(), b.tobytes())
 
-tests.append(MethodTests)
+tests.append(ByteReverseTests)
 
 # ---------------------------------------------------------------------------
 
 class CountTests(unittest.TestCase, Util):
 
     def test_basic(self):
         a = bitarray('10011')
@@ -2858,16 +3083,15 @@
                 self.assertEqual(a.count(v), ref)
                 self.assertEqual(a.count(v, n, -n - 1, -1), ref)
 
     def test_sparse(self):
         N = 65536
         a = zeros(N)
         indices = set(randint(0, N - 1) for _ in range(256))
-        for i in indices:
-            a[i] = 1
+        a[list(indices)] = 1
         self.assertEqual(a.count(1), len(indices))
         self.assertEqual(a.count(0), N - len(indices))
 
         for _ in range(100):
             i = randint(0, N - 1)
             j = randint(i, N - 1)
             cnt = sum(1 for k in indices if i <= k < j)
@@ -3198,21 +3422,19 @@
             self.assertEqual(a.search(b), res)
             self.assertEqual(list(a.itersearch(b)), res)
 
     def test_bool_random(self):
         for a in self.randombitarrays():
             b = a.copy()
             b.setall(0)
-            for i in a.itersearch(1):
-                b[i] = 1
+            b[a.search(1)] = 1
             self.assertEQUAL(b, a)
 
             b.setall(1)
-            for i in a.itersearch(0):
-                b[i] = 0
+            b[a.search(0)] = 0
             self.assertEQUAL(b, a)
 
             s = set(a.search(0) + a.search(1))
             self.assertEqual(len(s), len(a))
 
     def test_random(self):
         for a in self.randombitarrays():
```

### Comparing `bitarray-2.7.6/bitarray/test_util.py` & `bitarray-2.8.0/bitarray/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,16 +315,15 @@
                 j = None
             self.assertEqual(i, j)
 
     def test_random_start_stop(self):
         n = 2000
         a = zeros(n)
         indices = [randint(0, n - 1) for _ in range(100)]
-        for i in indices:
-            a[i] = 1
+        a[indices] = 1
         for _ in range(100):
             start = randint(0, n)
             stop = randint(0, n)
             filtered = [i for i in indices if i >= start and i < stop]
             ref = max(filtered) if filtered else -1
             try:
                 res = rindex(a, 1, start, stop)
@@ -335,16 +334,15 @@
     def test_many_set(self):
         for _ in range(10):
             n = randint(1, 10000)
             v = randint(0, 1)
             a = bitarray(n)
             a.setall(not v)
             lst = [randint(0, n - 1) for _ in range(100)]
-            for i in lst:
-                a[i] = v
+            a[lst] = v
             self.assertEqual(rindex(a, v), max(lst))
 
     def test_one_set(self):
         for _ in range(10):
             N = randint(1, 10000)
             a = bitarray(N)
             a.setall(0)
@@ -1339,16 +1337,15 @@
         for n in range(1, 32):
             positions = os.urandom(n)
             b = bytearray([0x02, 0x00, 0x01, 0xa0 + n])
             b.extend(positions)
             b.append(0)  # stop byte
 
             a.setall(0)
-            for p in positions:
-                a[p] = 1
+            a[positions] = 1
             self.assertEqual(sc_decode(b), a)
 
             # in order to recreate the block sc_encode generates, we need
             # a sorted list of the positions with no duplicates
             lst = sorted(set(positions))
             b = bytearray([0x02, 0x00, 0x01, 0xa0 + len(lst)])
             b.extend(lst)
```

### Comparing `bitarray-2.7.6/bitarray/util.py` & `bitarray-2.8.0/bitarray/util.py`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.6/bitarray/util.pyi` & `bitarray-2.8.0/bitarray/util.pyi`

 * *Files identical despite different names*

### Comparing `bitarray-2.7.6/bitarray.egg-info/PKG-INFO` & `bitarray-2.8.0/bitarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitarray
-Version: 2.7.6
+Version: 2.8.0
 Summary: efficient arrays of booleans -- C extension
 Home-page: https://github.com/ilanschnell/bitarray
 Author: Ilan Schnell
 Author-email: ilanschnell@gmail.com
 License: PSF
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Development Status :: 6 - Mature
@@ -86,28 +86,28 @@
 
 Once you have installed the package, you may want to test it:
 
 .. code-block:: shell-session
 
     $ python -c 'import bitarray; bitarray.test()'
     bitarray is installed in: /Users/ilan/bitarray/bitarray
-    bitarray version: 2.7.6
+    bitarray version: 2.8.0
     sys.version: 3.11.0 (main, Oct 25 2022) [Clang 14.0.4]
     sys.prefix: /Users/ilan/Mini3/envs/py311
     pointer size: 64 bit
     sizeof(size_t): 8
     sizeof(bitarrayobject): 80
     __clang__ or __GNUC__ defined: 1
     PY_LITTLE_ENDIAN (use word shift): 1
     DEBUG: 0
     .........................................................................
     .........................................................................
     ................................................................
     ----------------------------------------------------------------------
-    Ran 468 tests in 0.460s
+    Ran 485 tests in 0.465s
 
     OK
 
 The ``test()`` function is part of the API.  It will return
 a ``unittest.runner.TextTestResult`` object, such that one can verify that
 all tests ran successfully by:
 
@@ -203,14 +203,18 @@
 
     >>> a = bitarray(30)
     >>> a[:] = 0         # set all elements to 0 - equivalent to a.setall(0)
     >>> a[10:25] = 1     # set elements in range(10, 25) to 1
     >>> a
     bitarray('000000000011111111111111100000')
 
+As of bitarray version 2.8, indices may also be lists of arbitrary
+indices (like in NumPy), or bitarrays that are treated as masks,
+see `Bitarray indexing <https://github.com/ilanschnell/bitarray/blob/master/doc/indexing.rst>`__.
+
 
 Bitwise operators
 -----------------
 
 Bitarray objects support the bitwise operators ``~``, ``&``, ``|``, ``^``,
 ``<<``, ``>>`` (as well as their in-place versions ``&=``, ``|=``, ``^=``,
 ``<<=``, ``>>=``).  The behavior is very much what one would expect:
@@ -430,15 +434,15 @@
         ...
     TypeError: frozenbitarray is immutable
 
 
 Reference
 =========
 
-bitarray version: 2.7.6 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
+bitarray version: 2.8.0 -- `change log <https://github.com/ilanschnell/bitarray/blob/master/doc/changelog.rst>`__
 
 In the following, ``item`` and ``value`` are usually a single bit -
 an integer 0 or 1.
 
 
 The bitarray object:
 --------------------
@@ -498,15 +502,16 @@
    7. number of buffer exports
 
 
 ``bytereverse(start=0, stop=<end of buffer>, /)``
    For each byte in byte-range(start, stop) reverse the bit order in-place.
    The start and stop indices are given in terms of bytes (not bits).
    Also note that this method only changes the buffer; it does not change the
-   endianness of the bitarray object.
+   endianness of the bitarray object.  Padbits are left unchanged such that
+   two consecutive calls will always leave the bitarray unchanged.
 
    New in version 2.2.5: optional start and stop arguments.
 
 
 ``clear()``
    Remove all items from the bitarray.
```

### Comparing `bitarray-2.7.6/setup.py` & `bitarray-2.8.0/setup.py`

 * *Files identical despite different names*

