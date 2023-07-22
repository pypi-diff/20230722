# Comparing `tmp/klongpy-0.3.78.tar.gz` & `tmp/klongpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.3.78.tar", last modified: Thu Jul  6 16:14:57 2023, max compression
+gzip compressed data, was "klongpy-0.4.0.tar", last modified: Sat Jul 22 00:22:54 2023, max compression
```

## Comparing `klongpy-0.3.78.tar` & `klongpy-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.452793 klongpy-0.3.78/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.78/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    12794 2023-07-06 16:14:57.452793 klongpy-0.3.78/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    12259 2023-07-06 15:05:05.000000 klongpy-0.3.78/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.448794 klongpy-0.3.78/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.78/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.3.78/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.3.78/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    25913 2023-07-06 16:14:39.000000 klongpy-0.3.78/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    30733 2023-06-30 23:35:49.000000 klongpy-0.3.78/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20366 2023-07-06 15:05:05.000000 klongpy-0.3.78/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.3.78/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    16345 2023-07-06 16:14:39.000000 klongpy-0.3.78/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.78/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.78/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.448794 klongpy-0.3.78/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    12794 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-06 16:14:57.000000 klongpy-0.3.78/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.448794 klongpy-0.3.78/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6736 2023-07-06 15:05:05.000000 klongpy-0.3.78/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-06 16:14:57.452793 klongpy-0.3.78/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-07-06 16:14:39.000000 klongpy-0.3.78/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-06 16:14:57.452793 klongpy-0.3.78/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.3.78/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.78/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    23466 2023-07-06 15:05:05.000000 klongpy-0.3.78/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.3.78/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2780 2023-06-29 18:49:02.000000 klongpy-0.3.78/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.3.78/tests/test_join_over.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.78/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.78/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.78/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    13952 2023-07-06 16:14:39.000000 klongpy-0.3.78/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.3.78/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.4.0/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    19806 2023-07-22 00:22:54.762551 klongpy-0.4.0/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    19252 2023-07-22 00:22:29.000000 klongpy-0.4.0/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.4.0/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.4.0/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.4.0/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    26102 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/core.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30678 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20527 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.4.0/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    16759 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    15722 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/sys_fn_ipc.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.4.0/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1558 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/klongpy/web/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       99 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/web/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4721 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/web/sys_fn_web.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    19806 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      687 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      231 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7493 2023-07-22 00:22:29.000000 klongpy-0.4.0/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-22 00:22:54.762551 klongpy-0.4.0/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1136 2023-07-22 00:22:29.000000 klongpy-0.4.0/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.4.0/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.4.0/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    24124 2023-07-22 00:22:29.000000 klongpy-0.4.0/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.4.0/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2780 2023-06-29 18:49:02.000000 klongpy-0.4.0/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.4.0/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.4.0/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.4.0/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.4.0/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14714 2023-07-22 00:22:29.000000 klongpy-0.4.0/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.4.0/tests/test_util.py
```

### Comparing `klongpy-0.3.78/LICENSE` & `klongpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/PKG-INFO` & `klongpy-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,84 @@
-Metadata-Version: 2.1
-Name: klongpy
-Version: 0.3.78
-Summary: Python implementation of Klong language.
-Author: Brian Guarraci
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: cupy
-Provides-Extra: cuda12x
-Provides-Extra: cuda11x
-Provides-Extra: cuda111
-Provides-Extra: cuda110
-Provides-Extra: cuda102
-Provides-Extra: rocm-5-0
-Provides-Extra: rocm-4-3
-Provides-Extra: repl
-License-File: LICENSE
-
 
 ![Unit Tests](https://github.com/briangu/klongpy/workflows/Unit%20Tests/badge.svg)
 
 # KlongPy
 
-KlongPy is a vectorized port of [Klong](https://t3x.org/klong), making it a blazingly fast [array language](https://en.wikipedia.org/wiki/Array_programming) that supports direct Python integration.
+If you're intrigued by the world of [array languages](https://en.wikipedia.org/wiki/Array_programming) and love Python's versatility, meet KlongPy. This project marries the two, bringing Klong's elegant, terse syntax and the computational power of array programming to Python.
 
-[NumPy](https://numpy.org/) is used as the runtime target because it itself is an [Iverson Ghost](https://analyzethedatanotthedrivel.org/2018/03/31/NumPy-another-iverson-ghost/), or rather a descendent of APL, making the mapping from Klong to NumPy *relatively* straightforward.
+Born from the lineage of the [Klong](https://t3x.org/klong) array language, KlongPy leverages [NumPy](https://numpy.org/), an [Iverson Ghost](https://analyzethedatanotthedrivel.org/2018/03/31/NumPy-another-iverson-ghost/) that traces its roots back to APL, as its runtime target. This paves a relatively seamless path for mapping Klong constructs to NumPy, unleashing the performance benefits of this efficient, data-crunching Python library.
 
-Using NumPy also means that, via [CuPy](https://github.com/cupy/cupy), both CPU and GPU backends are supported (where possible, see Status section).
+The charm of KlongPy? It integrates Python's extensive library ecosystem right into the Klong language. Whether it's feeding your machine learning model with Klong-processed data or mixing and matching Klong with other Python libraries for your data analysis workflow, KlongPy has you covered. And, with [CuPy](https://github.com/cupy/cupy) in play, you have the flexibility of both CPU and GPU backends at your disposal.
 
+The project builds upon the work of [Nils M Holm](https://t3x.org), the creator of the Klong language, who has written a comprehensive [Klong Book](https://t3x.org/klong/book.html) for anyone interested in diving deeper. In short, if you're a data scientist, researcher, or just a programming language enthusiast, KlongPy may just be the next thing you want to check out.
 
-Klong was created by Nils M Holm and he has also written a [Klong Book](https://t3x.org/klong/book.html).
+# Overview
 
+KlongPy is a powerful language for high performance data analysis and distributed computing. Some of its main features include:
 
-# Related
+* Simplicity: KlongPy is based on Klong, a concise, expressive, and easy-to-understand array programming language. Its simple syntax and rich feature set make it an excellent tool for data scientists and engineers.
+* Speed: KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
+* Inter-Process Communication (IPC): KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
+* Array Programming: KlongPy supports array programming, which makes it a great tool for mathematical and scientific computing. You can manipulate entire arrays of data at once, enabling efficient data analysis and manipulation.
+* Compatibility: KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
 
- * [Klupyter - KlongPy in Jupyter Notebooks](https://github.com/briangu/klupyter)
- * [Advent Of Code '22](https://github.com/briangu/aoc/tree/main/22)
- * [Example Ticker Plant with streaming and dataframes](https://github.com/briangu/kdfs)
+At its heart, KlongPy is about infusing Python's flexibility with the compact Klong array language, allowing you to tap into the performance of NumPy while writing code that's concise and powerful. 
 
+Consider this simple Klong expression that computes an array's average: (+/a)%#a. Decoded, it means "sum of 'a' divided by the length of 'a'", as read from right to left.
 
-# Overview
+Below, we define the function 'avg' and apply it to the array of 1 million integers (as defined by !1000000)
+
+Let's try this in the KlongPy REPL:
 
-KlongPy brings together the Klong terse array language notation with the performance of NumPy.  I wanted to use Klong but I also wanted it to be a fast as possible.  Bonus is the ability to mix Klong with Python libraries making it easy to pick and choose the tools as appropriate.
+```Bash
+$ rlwrap kgpy
+
+Welcome to KlongPy REPL v0.3.78
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-d or ]q to quit
 
-Here's simple example of mixing Python and KlongPy to compute average of a 1B entry array.
+?> avg::{(+/x)%#x}
+:monad
+?> avg(!1000000)
+499999.5
+```
 
-To get an idea of what the following examples are about, let's first look at how average is computed in Klong. Assume 'a' represents an array, and we want to compute the average of 'a'.
+Now let's time it (first, right it once, then 100 times):
 
 ```
-(+/a)%#a
+?> ]T avg(!1000000)
+total: 0.0032962500117719173 per: 0.0032962500117719173
+?> ]T:100 avg(!1000000)
+total: 0.10882879211567342 per: 0.0010882879211567343
 ```
 
-This directly translates into (from right to left): length of x (#a) divides sum over x (+/a).
+We can also import Python modules to use directly in Klong language.  
 
-Now, with that in hand, we can try it in the REPL.  First we'll make a function called 'avg' and then find the average over the range 0..99 inclusive (!100).  Note, functions in Klong require the parameter names to be x, y, and z.
+Here we import the standard Python math library and redefine avg to use 'fsum':
 
 ```
-Welcome to KlongPy REPL
-author: Brian Guarraci
-repo  : https://github.com/briangu/klongpy
-crtl-c to quit
-
-?> avg::{(+/x)%#x}
+?> .py("math")
+1
+?> favg::{fsum(x)%#x}
 :monad
-?> avg(!100)
-49.49999999999999
+?> favg(!1000000)
+499999.5
 ```
 
-Now let's time it using the REPL system command ]T, which uses the Python timeit facility.  First, we'll run it once and see it takes about 374us, then we'll run it 100 times.
+Notice that using fsum is slower than using Klong '+/'.  This is because the '+/' operation is vectorized while fsum is not.
 
 ```
-?> ]T avg(!100)
-0.0003741057589650154
-?> ]T:100 avg(!100)
-0.01385202500387095
+?> ]T favg(!1000000)
+total: 0.050078875152394176 per: 0.050078875152394176
+?> ]T:100 favg(!1000000)
+total: 2.93945804098621 per: 0.029394580409862103
 ```
 
-Let's use Klong from Python:
+To use KlongPy within Python, here's a basic outline:
 
 ```python
 from klongpy import KlongInterpreter
 
 # instantiate the KlongPy interpeter
 klong = KlongInterpreter()
 
@@ -94,15 +90,15 @@
 
 # reference the 'avg' function in Klong interpeter and call it directly from Python.
 r = klong['avg'](data)
 
 print(f"avg={np.round(r,6)}")
 ```
 
-Let's compare CPU vs GPU backends:
+And let's run a performance comparison between CPU and GPU backends:
 
 ```python
 import time
 from klongpy.backend import np
 from klongpy import KlongInterpreter
 
 klong = KlongInterpreter()
@@ -125,19 +121,21 @@
 Run (GPU)
 
     $ USE_GPU=1 python3 tests/perf_avg.py
     avg=0.500015 in 0.027818 seconds
 
 # Python integration
 
-KlongPy supports direct Python integration, making it easy to mix Klong with Python and use it in the most suitable scenarios.  For example, KlongPy can be part of an ML/Pandas workflow or be part of the website backend.
+Seamlessly blending Klong and Python is the cornerstone of KlongPy, enabling you to utilize each language where it shines brightest. For instance, you can integrate KlongPy into your ML/Pandas workflows, or deploy it as a powerhouse driving your website backend.
+
+The charm of KlongPy lies in its dictionary-like interpreter that hosts the current KlongPy state, making it incredibly simple to extend KlongPy with custom functions and shuttle data in and out of the interpreter.
 
-Extending KlongPy with custom functions and moving data in / out of the KlongPy interpeter is easy since the interpreter operates as a dictionary. The dictionary contents are the current KlongPy state.
+Imagine your data processed elsewhere, just set it into KlongPy and watch as the Klong language works its magic, accessing and manipulating your data with effortless ease. Even more, Python lambdas or functions can directly be exposed as Klong functions, adding an array of powerful tools to your Klong arsenal.
 
-Data generated elsewhere can be set in KlongPy and seamlessly accessed and processed via Klong language.  Also, Python lambdas or functions may be exposed directly as Klong functions, allowing easy extensions to the Klong language.
+KlongPy indeed is a force multiplier, amplifying the power of your data operations.
 
 ## Function example
 
 Call a Python function from Klong:
 
 ```python
 from klongpy import KlongInterpreter
@@ -153,19 +151,17 @@
 from klongpy import KlongInterpreter
 klong = KlongInterpreter()
 klong("f::{(x*1000) + y - z}")
 r = klong['f'](3, 10, 20)
 assert r == 2990
 ```
 
-As you can see, it's easy to interop with Python and Klong allowing the best tool for the job.
-
 ## Data example
 
-Since the Klong interpreter context is basically a dictionary, you can store values there for access in Klong:
+Since the Klong interpreter context is dictionary-like, you can store values there for access in Klong:
 
 ```python
 data = np.arange(10*9)
 klong['data'] = data
 r = klong('1+data')
 assert r == 1 + data
 ```
@@ -176,15 +172,17 @@
 klong('Q::1+data')
 Q = klong['Q']
 print(Q)
 ```
 
 ## Python library access
 
-In order to simplify Klong development, Python functions can be easily added to support common operations:
+Python functions, including lambdas, can be easily added to support common operations.  
+
+In order to be consistent with Klong language, the paramters of Python functions may have at most three paramters and they must be x, y, and z.
 
 ```Python
 from datetime import datetime
 from klongpy import KlongInterpreter
 klong = KlongInterpreter()
 klong['strptime'] = lambda x: datetime.strptime(x, "%d %B, %Y")
 klong("""
@@ -221,15 +219,15 @@
 ```
 called from KlongPy: 2018-06-21 00:00:00
 called from KlongPy: {'timestamp': datetime.datetime(2018, 6, 21, 0, 0)}
 ```
 
 ## Loading Python Modules directly into KlongPy
 
-KlongPy has the powerful ability to load Python modules directly. This can be extremely useful when you want to utilize the functionality offered by various Python libraries, and seamlessly integrate them into your KlongPy programs.
+KlongPy has the powerful ability to load Python modules directly. This can be extremely useful when you want to utilize the functionality offered by various Python libraries, and seamlessly integrate them into your KlongPy programs.  
 
 Here is an example of how you can load a Python module into KlongPy:
 
 ```bash
 $ rlwrap kgpy
 
 Welcome to KlongPy REPL v0.3.76
@@ -237,16 +235,21 @@
 repo  : https://github.com/briangu/klongpy
 crtl-d or ]q to quit
 
 ?> .py("math")
 1
 ?> sqrt(64)
 8.0
+?> fsum(!100)
+4950.0
 ```
 
+In order to keep consistency with Klong 3-parameter function rules, KlongPy will attempt to remap loaded functions to use the x,y and z convention.  For example, in the Python math module, fsum is defined as fsum(seq), so KlongPy remaps this to fsum(x) so that it works within the runtime.
+
+
 ## Loading Custom Python Modules
 
 Custom modules can be written for KlongPy in the same way as any Python module, the main
 difference is that they don't need to be installed (e.g. via pip).
 
 Simply create a directory with a __init__.py and appropriate files, as in:
 
@@ -300,14 +303,99 @@
 
 klong = KlongInterpreter()
 klong['df'] = {col: np.array(df[col]) for col in df.columns}
 klong('df?"Name"') # ==> ['Alice', 'Bob', 'Charlie', 'David']
 klong('df?"Age"')  # ==> [25, 30, 35, 40]
 ```
 
+# Inter-Process Communication (IPC) Capabilities
+
+KlongPy has powerful Inter-Process Communication (IPC) features that enable it to connect and interact with remote KlongPy instances. This includes executing commands, retrieving or storing data, and even defining functions remotely. These new capabilities are available via two new functions: .cli() and .clid().
+
+## The .cli() Function
+
+The .cli() function creates an IPC client. You can pass it either an integer (interpreted as a port on "localhost:<port>"), a string (interpreted as a host address "<host>:<port>"), or a remote dictionary (which shares the network connection and returns a remote function).
+
+Use .cli() to evaluate commands on a remote KlongPy server, define functions, perform calculations, or retrieve values. You can also pass it a symbol to retrieve a value or a function from the remote server.
+
+Here are some examples:
+
+```
+?> f = .cli(8888)
+?> f("avg::{(+/x)%#x}")   
+?> f("avg(!100)")        
+```
+
+Using remote function proxies, you can reference a remotely defined function and call it as if it were local:
+
+```
+?> q::f(:avg)
+?> q(!100)
+49.5 
+```
+
+## The .clid() Function
+
+As seen in Python interop examples, the KlongPy context is effectively a dictionary.  The .clid() function creates an IPC client that treats the remote KlongPy context as a dictionary, allowing you to set/get values on the remote instance.  Combined with the remote function capabilities, the remote dictionary makes it easy to interact with remote KlongPy instances.
+
+Here are some examples:
+
+```
+?> d = .clid(8888)
+?> d,[:foo 2]             
+?> d,[:bar "hello"]       
+?> d,:fn,{x+1}            
+```
+
+These powerful capabilities allow for more effective use of distributed computing resources. Please be aware of potential security issues, as you are allowing a remote server to execute potentially arbitrary commands from your client. Always secure your connections and validate your commands to avoid potential attacks.
+
+## Remote Function Proxies and Enumeration
+
+Another powerful feature of KlongPy's IPC capabilities is the use of remote function proxies. These function proxies behave as if they were local functions, but are actually executed on a remote server. You can easily create these function proxies using .cli() or .clid(), and then use them as you would any other function.
+
+One of the most powerful aspects of these remote function proxies is that they can be stored in an array and then enumerated. When you do this, KlongPy will execute each function in turn with the specified parameters.
+
+For example, suppose you have created three remote function proxies:
+
+```
+?> d::.clid(8888)
+?> d,:avg,{(+/x)%#x}
+?> d,:sum,{(+/x)}
+?> d,:max,{(x@>x)@0}
+?> a = d?:avg
+?> b = d?:sum
+?> c = d?:max
+```
+
+You can then call each of these functions with the same parameter by using enumeration:
+
+```
+?> {x@,!100}'[a b c]
+[  49.5 4950.    99. ]
+```
+
+In this example, KlongPy will execute each function with the range 0-99 as a parameter, and then store the results in the results array. The :avg function will calculate the average of the numbers, the :sum function will add them up, and the :max function will return the largest number in the range.
+
+This makes it easy to perform multiple operations on the same data set, or to compare the results of different functions. It's another way that KlongPy's IPC capabilities can enhance your data analysis and distributed computing tasks.
+
+## Closing Remote Function Proxies
+
+Closing remote connections is done with the .clic() command.  Once it is closed, all proxies that shared that connection are now disconnected as well.
+
+```
+?> f::.cli(8888)
+?> .clic(f)
+1
+```
+
+## Synchronization
+
+While the IPC server I/O is async, the KlongPy interpreter is single-threaded.  All remote operations are synchronous to make it easy to use remote operations as part of a normal workflow.  Of course, when calling over to another KlongPy instance, you have no idea what state that instance is in, but within the calling instance operations will be sequential.
+
+
 # Performance
 
 The Klong language is simple, so the overhead is low.  The bulk of the compute time will likely be spent in NumPy doing actual work.
 
 Here's a contrived rough benchmark to show the magnitude differences between Python, KlongPy (CPU + GPU) and Numpy (CPU).
 
 **Spoiler**: GPU-backed KlongPy is about 790x faster than naive Python and 36x faster than NumPy-backed KlongPy.
@@ -391,62 +479,72 @@
     $ python3 setup.py develop
 
 
 # REPL
 
 KlongPy has a REPL similar to Klong's REPL.
 
-    $ pip3 install klongpy[repl]
-    $ rlwrap kgpy
+```bash
+$ pip3 install klongpy[repl]
+$ rlwrap kgpy
+
+Welcome to KlongPy REPL
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-c to quit
 
-    Welcome to KlongPy REPL
-    author: Brian Guarraci
-    repo  : https://github.com/briangu/klongpy
-    crtl-c to quit
-
-    ?> 1+1
-    2
-    >? "hello, world!"
-    hello, world!
-    ?> prime::{&/x!:\2+!_x^1%2}
-    :monad
-    ?> prime(4)
-    0
-    ?> prime(251)
-    1
-    ?> ]T prime(251)
-    0.0005430681630969048
+?> 1+1
+2
+>? "hello, world!"
+hello, world!
+?> prime::{&/x!:\2+!_x^1%2}
+:monad
+?> prime(4)
+0
+?> prime(251)
+1
+?> ]T prime(251)
+total: 0.0004914579913020134 per: 0.0004914579913020134
+```
 
 Read about the [prime example here](https://t3x.org/klong/prime.html).
 
 
 # Status
 
-KlongPy aims to be a complete implementation of klong.  It currently passes all of the integration tests provided by klong.
+KlongPy aims to be a complete implementation of klong.  It currently passes all of the integration tests provided by klong as well as additional suites.
 
 Since CuPy is [not 100% compatible with NumPy](https://docs.cupy.dev/en/stable/user_guide/difference.html), there are currently some gaps in KlongPy between the two backends.  Notably, strings are supported in CuPy arrays so KlongPy GPU support currently is limited to math.
 
 Primary ongoing work includes:
 
+* Add IPC capabilities so to enable inter-KlongPy commoncation
 * Actively switch between CuPy and NumPy when incompatibilities are present
     * Work on CuPy kernels is in this branch: _cupy_reduce_kernels
 * Additional syntax error help
 * Additional tests to
     * ensure proper vectorization
     * increase Klong grammar coverage
 * Make REPL (kgpy) compatible with original Klong (kg) REPL
 
+
 # Differences from Klong
 
-While KlongPy aims to be 100% compatible with Klong language, the KlongPy system has different goals:
+While KlongPy aims to be 100% compatible with Klong language, the KlongPy system has some differences:
 
     * Infinite precision: The main difference in this implementation of Klong is the lack of infinite precision.  By using NumPy we are restricted to doubles.
     * Python integration: Most notably, the ".py" command allows direct import of Python modules into the current Klong context.
     * IPC - KlongPy will support IPC between KlongPy processes, allowing one KlongPy process to interact with other KlongPy processes over the network.
 
+# Related
+
+ * [Klupyter - KlongPy in Jupyter Notebooks](https://github.com/briangu/klupyter)
+ * [Advent Of Code '22](https://github.com/briangu/aoc/tree/main/22)
+ * [Example Ticker Plant with streaming and dataframes](https://github.com/briangu/kdfs)
+
 
 # Running tests
 
 ```bash
 python3 -m unittest
 ```
```

### Comparing `klongpy-0.3.78/klongpy/adverbs.py` & `klongpy-0.4.0/klongpy/adverbs.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/klongpy/backend.py` & `klongpy-0.4.0/klongpy/backend.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/klongpy/core.py` & `klongpy-0.4.0/klongpy/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,32 @@
         return f":{super().__str__()}"
     def __eq__(self, o):
         return isinstance(o,KGSym) and self.__str__() == o.__str__()
     def __hash__(self):
         return super().__hash__()
 
 
+def get_fn_arity_str(arity):
+    if arity == 0:
+        return ":nilad"
+    elif arity == 1:
+        return ":monad"
+    elif arity == 2:
+        return ":dyad"
+    return ":triad"
+
+
 class KGFn:
     def __init__(self, a, args, arity):
         self.a = a
         self.args = args
         self.arity = arity
 
     def __str__(self):
-        if self.arity == 0:
-            return ":nilad"
-        elif self.arity == 1:
-            return ":monad"
-        elif self.arity == 2:
-            return ":dyad"
-        return ":triad"
+        return get_fn_arity_str(self.arity)
 
     def is_op(self):
         return isinstance(self.a,KGOp)
 
     def is_adverb_chain(self):
         return isinstance(self.a,list) and isinstance(self.a[0],KGAdverb)
 
@@ -49,15 +53,16 @@
 
     def __call__(self, *args, **kwargs):
         fn_args = [np.asarray(x) if isinstance(x, list) else x for x in args]
         return self.klong.call(KGCall(self.fn.a, [*fn_args], self.fn.arity))
 
 
 class KGCall(KGFn):
-    pass
+    def __str__(self):
+        return self.a.__str__() if issubclass(type(self.a), KGLambda) else super().__str__()
 
 
 class KGOp:
     def __init__(self, a, arity):
         self.a = a
         self.arity = arity
 
@@ -95,24 +100,27 @@
     lambda x,y: x + y
     lambda klong, x: klong(x)
 
     """
     def __init__(self, fn):
         self.fn = fn
         params = inspect.signature(self.fn, follow_wrapped=True).parameters
-        self.args = [x for x in params if x in reserved_fn_args]
+        self.args = [reserved_fn_symbol_map[x] for x in reserved_fn_args if x in params]
         self.provide_klong = 'klong' in params
 
     def __call__(self, klong, ctx):
-        params = [ctx[reserved_fn_symbol_map[x]] for x in reserved_fn_args[:len(self.args)]]
+        params = [ctx[x] for x in self.args]
         return self.fn(klong, *params) if self.provide_klong else self.fn(*params)
 
     def get_arity(self):
         return len(self.args)
 
+    def __str__(self):
+        return get_fn_arity_str(self.get_arity())
+
 
 class KGChannelDir(Enum):
     INPUT=1
     OUTPUT=2
 
 
 class KGChannel:
```

### Comparing `klongpy-0.3.78/klongpy/dyads.py` & `klongpy-0.4.0/klongpy/dyads.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,17 +161,17 @@
                     [1 2 3 4 5]@[1 2 3]  -->  [2 3 4]
                     [1 2 3 4 5]@[0 0 0]  -->  [1 1 1]
                   "hello world"@[3 7 2]  -->  "lol"
                                {x}@:foo  -->  :foo
                          {y+x*x}@[2 3]   -->  7
 
     """
-    if isinstance(a, (KGFn, KGSym)):
-        # TODO: fix arity
-        return klong.eval(KGCall(a, b.tolist() if np.isarray(b) else b, arity=2))
+    if isinstance(a, (KGFn, KGSym)) or issubclass(type(a), KGLambda):
+        b = [x for x in b] if np.isarray(b) else b
+        return klong.eval(KGCall(a, b, arity=1))
     j = isinstance(a,str)
     a = str_to_chr_arr(a) if j else a
     if is_list(b):
         if is_empty(b):
             r = np.asarray([])
         else:
             # TODO: return None for missing keys? or raise?
@@ -305,16 +305,16 @@
                             ""?""  -->  [0]
                       :{[1 []]}?1  -->  []
 
     """
     if isinstance(a,str):
         return np.asarray([m.start() for m in re.finditer(f"(?={b})", a)])
     elif is_dict(a):
-        # NOTE: we don't use get or np.inf because value may be 0 or None
-        return a[b] if b in a else np.inf # TODO: use undefined type
+        v = a.get(b)
+        return np.inf if v is None else v
     if is_list(b):
         return np.asarray([i for i,x in enumerate(a) if kg_equal(x,b)])
     return np.where(np.asarray(a) == b)[0]
 
 
 def eval_dyad_form(a, b):
     """
```

### Comparing `klongpy-0.3.78/klongpy/interpreter.py` & `klongpy-0.4.0/klongpy/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 from collections import deque
 
 from .adverbs import get_adverb_fn
 from .core import *
 from .dyads import create_dyad_functions
 from .monads import create_monad_functions
 from .sys_fn import create_system_functions
+from .sys_fn_ipc import create_system_functions_ipc
 from .sys_var import *
 from .utils import ReadonlyDict
 
 
 def set_context_var(d, sym, v):
     """
     Sets a context variable, wrapping Python lambda/functions as appropriate.
     """
     assert isinstance(sym, KGSym)
     if callable(v):
-        x = KGLambda(v)
+        x = v if issubclass(type(v), KGLambda) else KGLambda(v)
         v = KGCall(x,args=None,arity=x.get_arity())
     d[sym] = v
 
 
 class KGModule(dict):
     """
     A module class that is used for optimizing when to scan for namespaced keys.
@@ -119,14 +120,15 @@
 def create_system_contexts():
     cin = eval_sys_var_cin()
     cout = eval_sys_var_cout()
     cerr = eval_sys_var_cerr()
 
     sys_d = {}
     add_system_functions(sys_d, create_system_functions())
+    add_system_functions(sys_d, create_system_functions_ipc())
     set_context_var(sys_d, KGSym('.e'), eval_sys_var_epsilon()) # TODO: this is probably a bug that this can't be a lambda
     set_context_var(sys_d, KGSym('.cin'), cin)
     set_context_var(sys_d, KGSym('.cout'), cout)
     set_context_var(sys_d, KGSym('.cerr'), cerr)
 
     sys_var = {}
     set_context_var(sys_var, KGSym('.sys.cin'), cin)
@@ -513,15 +515,15 @@
                     ctx[q] = q
                 f = f[1:]
 
         ctx[reserved_dot_f_symbol] = f
 
         self._context.push(ctx)
         try:
-            return f(self, self._context) if isinstance(f, KGLambda) else self.call(f)
+            return f(self, self._context) if issubclass(type(f), KGLambda) else self.call(f)
         finally:
             self._context.pop()
 
     def call(self, x):
         """
 
         Invoke a Klong program (as produced by prog()), causing functions to be called and evaluated.
```

### Comparing `klongpy-0.3.78/klongpy/monads.py` & `klongpy-0.4.0/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/klongpy/sys_fn.py` & `klongpy-0.4.0/klongpy/sys_fn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 import errno
 import importlib.util
+import inspect
 import os
 import random
 import subprocess
 import sys
 import time
 
 from .core import KGChannel, KGChannelDir, is_empty, kg_read, kg_write, safe_eq, reserved_fn_args
@@ -313,67 +314,73 @@
             module = None
             try:
                 pardir = os.path.dirname(x)
                 sys.path.insert(0,pardir)
                 module_name = os.path.basename(os.path.normpath(x))
                 module = importlib.import_module(module_name)
             except Exception as e:
-                print(e)
+                print(f".py: {e}")
                 raise e
             finally:
                 sys.path.pop(0)
         else:
             raise FileNotFoundError("Not a valid Python module (missing __init__.py): {x}")
     elif os.path.isfile(x):
         module_name = os.path.dirname(x)
         location = x
         spec = importlib.util.spec_from_file_location(module_name, location=location)
         module = importlib.util.module_from_spec(spec)
         try:
             spec.loader.exec_module(module)
         except Exception as e:
-            print(e)
+            print(f".py: {e}")
             raise RuntimeError("module could not be imported: {x}")
     else:
         if (spec := importlib.util.find_spec(x)) is not None:
             module = importlib.util.module_from_spec(spec)
             try:
                 spec.loader.exec_module(module)
             except Exception as e:
-                print(e)
+                print(f".py: {e}")
                 raise RuntimeError("module could not be imported: {x}")
     try:
-        import_items = filter(lambda p: not p[0].startswith("__"), module.__dict__.items())
+        klong_exports = module.__dict__.get("klong_exports")
+        if klong_exports is None:
+            import_items = filter(lambda p: not (p[0].startswith("__")), module.__dict__.items())
+        else:
+            import_items = klong_exports.items()
         if import_items is not None:
             ctx = klong._context.pop()
             try:
-                import inspect
-
                 for p,q in import_items:
+                    if not callable(q):
+                        continue
                     try:
                         args = inspect.signature(q, follow_wrapped=True).parameters
-                        if len(args) > len(reserved_fn_args):
-                            print("skipping {p} - too many paramters {len(args)}")
-                        if reserved_fn_args[0] not in args:
-                            print("remapping {p} using reserved parameter names")
-                            n_args = len(args)
+                        n_args = len(args)
+                        provide_klong = 'klong' in args
+                        n_args = n_args - (1 if provide_klong else 0)
+                        if n_args > len(reserved_fn_args):
+                            print(f".py: skipping {p} - too many paramters: {n_args}")
+                        if n_args > 0 and reserved_fn_args[0] not in args:
+                            print(f".py: remapping {p} using reserved parameter names")
                             if n_args == 3:
                                 q = lambda x,y,z,f=q: f(x,y,z)
                             elif n_args == 2:
                                 q = lambda x,y,f=q: f(x,y)
                             elif n_args == 1:
                                 q = lambda x,f=q: f(x)
                         klong[p] = q
                     except Exception as e:
-                        print(e)
+                        print(f".py: {e}")
             finally:
                 klong._context.push(ctx)
             return 1
     except Exception as e:
-        print(e)
+        print(f".py: {e}")
         raise RuntimeError("failed to load module: {x}")
 
 
 def eval_sys_random_number():
     """
 
         .rn()                                            [Random-Number]
```

### Comparing `klongpy-0.3.78/klongpy/sys_var.py` & `klongpy-0.4.0/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/klongpy.egg-info/SOURCES.txt` & `klongpy-0.4.0/klongpy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 klongpy/adverbs.py
 klongpy/backend.py
 klongpy/core.py
 klongpy/dyads.py
 klongpy/interpreter.py
 klongpy/monads.py
 klongpy/sys_fn.py
+klongpy/sys_fn_ipc.py
 klongpy/sys_var.py
 klongpy/utils.py
 klongpy.egg-info/PKG-INFO
 klongpy.egg-info/SOURCES.txt
 klongpy.egg-info/dependency_links.txt
 klongpy.egg-info/requires.txt
 klongpy.egg-info/top_level.txt
+klongpy/web/__init__.py
+klongpy/web/sys_fn_web.py
 scripts/kgpy
 tests/test_accel.py
 tests/test_examples.py
 tests/test_extra_suite.py
 tests/test_fn.py
 tests/test_interop.py
 tests/test_join_over.py
```

### Comparing `klongpy-0.3.78/scripts/kgpy` & `klongpy-0.4.0/scripts/kgpy`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/python3
 
 import argparse
+import asyncio
 import os
 import sys
 import timeit
 
+import colorama
 import pkg_resources
-from colorama import Fore, init
 
 from klongpy import KlongInterpreter
 
-
 """
 
     KlongPy REPL: See https://t3x.org/klong/klong-ref.txt.html for additional details.
 
 """
 
 def sys_cmd_shell(klong, cmd):
@@ -129,16 +129,15 @@
 
         For one iteration, it's possible this Klong timeit is more accurate than the native Python timeit due to overhead.
 
         Note: Added in KlongPy.
 
     """
     n = int(cmd[3:cmd.index(" ")]) if cmd[2] == ":" else 1
-    prog = klong.prog(cmd[cmd.index(" "):])
-    r = timeit.timeit(lambda k=klong,p=prog: k.eval(p), number=n)
+    r = timeit.timeit(lambda k=klong,p=cmd[cmd.index(" "):]: k(p), number=n)
     return f"total: {r} per: {r/n}"
 
 
 def create_sys_cmd_functions():
     def _get_name(s):
         s = s.strip()
         x = s.index(']')+1
@@ -151,110 +150,127 @@
         fn = getattr(m,x)
         name = _get_name(fn.__doc__)
         registry[name] = fn 
 
     return registry
 
 
-success = lambda input: f"{Fore.GREEN}{input}"
-failure = lambda input: f"{Fore.RED}{input}"
+success = lambda input: f"{colorama.Fore.GREEN}{input}"
+failure = lambda input: f"{colorama.Fore.RED}{input}"
 
 
-def repl_eval(klong, p, verbose=False):
+def repl_eval(klong, p, verbose=True):
     try:
         r = klong(p)
         r = r if r is None else success(r)
     except Exception as e:
         r = failure(f"Error: {e.args}")
         if verbose:
             import traceback
-            traceback.print_exc(e)
-    return r
+            traceback.print_exception(type(e), e, e.__traceback__)
 
+    return r
 
-# https://dev.to/amal/building-the-python-repl-3468
-def repl(klong=None):
 
+def show_repl_header(ipc_addr=None):
     print()
-    print(f"{Fore.GREEN}Welcome to KlongPy REPL v{pkg_resources.get_distribution('klongpy').version}")
-    print(f"{Fore.BLUE}author: Brian Guarraci")
-    print(f"{Fore.BLUE}repo  : https://github.com/briangu/klongpy")
-    print(f"{Fore.YELLOW}crtl-d or ]q to quit")
+    print(f"{colorama.Fore.GREEN}Welcome to KlongPy REPL v{pkg_resources.get_distribution('klongpy').version}")
+    print(f"{colorama.Fore.GREEN}author: Brian Guarraci")
+    print(f"{colorama.Fore.GREEN}repo  : https://github.com/briangu/klongpy")
+    print(f"{colorama.Fore.YELLOW}crtl-d or ]q to quit")
     print()
+    if ipc_addr:
+        print(f"{colorama.Fore.RED}Running IPC server at {ipc_addr}")
+        print()
 
-    init(autoreset=True)
 
-    sys_cmds = create_sys_cmd_functions()
+def get_input():
+    return input("?> ")
 
-    klong = klong or KlongInterpreter()
-    while True:
-        try:
-            s = input("?> ")
-            if len(s) == 0:
-                continue
-            if s.startswith("]"):
-                if s[1] in sys_cmds:
-                    r = sys_cmds[s[1]](klong, s)
-                else:
-                    print(f"unkown system command: ]{s[1]}")
+
+class ConsoleInputHandler:
+    @staticmethod
+    async def input_producer(loop, klong, verbose=False):
+        sys_cmds = create_sys_cmd_functions()
+
+        while True:
+            try:
+                s = await loop.run_in_executor(None, get_input)
+                if len(s) == 0:
                     continue
-            else:
-                r = repl_eval(klong, s)
-            if r is not None:
-                print(r)
-        except EOFError:
-            print("\rbye!")
-            break
-        except KeyboardInterrupt:
-            print(failure("\nkg: error: interrupted"))
-        except Exception as e:
-            print(failure(f"Error: {e.args}"))
-            import traceback
-            traceback.print_exc(e)
+                if s.startswith("]"):
+                    if s[1] in sys_cmds:
+                        r = sys_cmds[s[1]](klong, s)
+                    else:
+                        print(f"unkown system command: ]{s[1]}")
+                        continue
+                else:
+                    r = repl_eval(klong, s, verbose=verbose)
+                if r is not None:
+                    print(r)
+            except EOFError:
+                print("\rbye!")
+                loop.stop()
+                break
+            except KeyboardInterrupt:
+                print(failure("\nkg: error: interrupted"))
+            except Exception as e:
+                print(failure(f"Error: {e.args}"))
+                import traceback
+                traceback.print_exc(e)
 
 
 def run_file(fname):
     with open(fname, "r") as f:
         return klong(f.read())
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         prog='KlongPy',
         description='KlongPy REPL',
         epilog='For help, go to https://github.com/briangu/klongpy')
     parser.add_argument('-e', '--expr', help='evaluate expression, no interactive mode')
     parser.add_argument('-l', '--load', help='load program from file')
-    parser.add_argument('-p', '--run', help='run program from file')
+    parser.add_argument('-s', '--server', help='start the IPC server', type=str)
     parser.add_argument('-t', '--test', help='test program from file')
+    parser.add_argument('-v', '--verbose', help='enable verbose output', action="store_true")
     parser.add_argument('filename', nargs='?', help='filename to be run if no flags are specified')
 
     args = parser.parse_args()
 
     if args.expr:
         print(KlongInterpreter()(args.expr))
         exit()
 
     klong = KlongInterpreter()
+    loop = asyncio.get_event_loop()
+    run_repl = False
 
-    if args.load:
-        print(f"Loading: {args.load}")
-        with open(args.load, "r") as f:
-            klong(f.read())
-        repl(klong)
-    elif args.run:
-        print(f"Running: {args.run}")
-        with open(args.run, "r") as f:
-            klong(f.read())
+    if args.server:
+        r = klong(f".srv({args.server})")
+        if r == 0:
+            print(f"Failed to start server")
     elif args.test:
         print(f"Test: {args.test}")
         with open(args.test, "r") as f:
             for x in f.readlines():
                 x = x.strip()
                 if len(x) == 0 or x.startswith(":"):
                     continue
                 print(x)
                 klong(x)
-    elif args.filename:
+    
+    if args.filename:
         run_file(args.filename)
     else:
-        repl()
+        run_repl = True
+
+    if run_repl:
+        if args.load:
+            print(f"Loading: {args.load}")
+            with open(args.load, "r") as f:
+                klong(f.read())
+        colorama.init(autoreset=True)
+        show_repl_header(args.server)
+        loop.create_task(ConsoleInputHandler.input_producer(loop, klong, args.verbose))
+        loop.run_forever()
```

### Comparing `klongpy-0.3.78/setup.py` & `klongpy-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
-    packages=['klongpy'],
-    version='0.3.78',
+    packages=['klongpy', 'klongpy.web'],
+    version='0.4.0',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -27,12 +27,13 @@
         'cuda11x': ["cupy-cuda11x"],
         'cuda111': ["cupy-cuda111"],
         'cuda110': ["cupy-cuda110"],
         'cuda102': ["cupy-cuda102"],
         'rocm-5-0': ["cupy-rocm-5-0"],
         'rocm-4-3': ["cupy-rocm-4-3"],
         'repl': ["colorama"],
+        'web': ["aiohttp"]
     },
     include_package_data=True,
     test_suite='tests',
     scripts=['scripts/kgpy']
 )
```

### Comparing `klongpy-0.3.78/tests/test_accel.py` & `klongpy-0.4.0/tests/test_accel.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/tests/test_examples.py` & `klongpy-0.4.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/tests/test_extra_suite.py` & `klongpy-0.4.0/tests/test_extra_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,37 @@
 
 # add tests not included in the original kg suite
 class TestExtraCoreSuite(unittest.TestCase):
 
     def assert_eval_cmp(self, a, b, klong=None):
         self.assertTrue(eval_cmp(a, b, klong=klong))
 
+    @unittest.skip
+    def test_join_two_dict(self):
+        klong = KlongInterpreter()
+        klong("b:::{[1 2]}")
+        klong("c:::{[3 4]}")
+        r = klong("b,c")
+        self.assertEqual(r, {1: 2, 3: 4})
+
+    @unittest.skip
+    def test_nested_dict(self):
+        klong = KlongInterpreter()
+        klong('c:::{["GET" :{["/" 2]}]}')
+        r = klong('(c?"GET")?"/"')
+        self.assertEqual(r, 2)
+
+    def test_apply_range(self):
+        klong = KlongInterpreter()
+        r = klong("{x}@,!100")
+        self.assertTrue(kg_equal(r, np.arange(100)))
+        klong("avg::{(+/x)%#x}")
+        r = klong("avg@,!100")
+        self.assertEqual(r,49.5)
+
     def test_eval_quote_string(self):
         klong = KlongInterpreter()
         r = klong(':"hello"')
         self.assertTrue(r is None)
 
     def test_array_identity(self):
         klong = KlongInterpreter()
```

### Comparing `klongpy-0.3.78/tests/test_fn.py` & `klongpy-0.4.0/tests/test_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/tests/test_interop.py` & `klongpy-0.4.0/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/tests/test_join_over.py` & `klongpy-0.4.0/tests/test_join_over.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/tests/test_prog.py` & `klongpy-0.4.0/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/tests/test_suite.py` & `klongpy-0.4.0/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/tests/test_suite_file.py` & `klongpy-0.4.0/tests/test_suite_file.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.78/tests/test_sys_fn.py` & `klongpy-0.4.0/tests/test_sys_fn.py`

 * *Files 8% similar despite different names*

```diff
@@ -228,27 +228,42 @@
         tests.append(os.path.join(plugins_dir, "greetings/__init__.py"))
         tests.append(os.path.join(plugins_dir, "greetings/hello_world.py"))
         tests.append("greetings")
         try:
             sys.path.append(plugins_dir)
             for fpath in tests:
                 klong = KlongInterpreter()
-                r = klong(f'.py("{fpath}")')
-                self.assertEqual(r,1)
-                r = klong('hello()')
-                self.assertEqual(r,"world!")
+                self.assertEqual(klong(f'.py("{fpath}")'),1)
+
+                self.assertEqual(klong('nilad()'),"hello, world!")
+                self.assertEqual(klong('monad(1)'),"1+1")
+                self.assertEqual(klong('dyad(1;2)'),"1*2+1")
+                self.assertEqual(klong('triad(1;2;3)'),"1*2+3+1")
+                self.assertEqual(klong('knilad()'),4)
+                self.assertEqual(klong('kmonad(1)'),2)
+                self.assertEqual(klong('kdyad(1;2)'),1*2+1)
+                self.assertEqual(klong('ktriad(1;2;3)'),1*2+3+1)
+
                 if fpath.endswith("hello_world.py"):
                     r = klong['not_exported']
                     self.assertTrue(r is not None)
                 else:
                     with self.assertRaises(KeyError):
                         klong['not_exported']
         finally:
             sys.path.pop()
 
+    def test_sys_python_load_custom_export(self):
+        tests_dir = os.path.dirname(os.path.abspath(__file__))
+        plugins_dir = os.path.join(tests_dir, "plugins")
+        fpath = os.path.join(plugins_dir, "custom_export")
+        klong = KlongInterpreter()
+        self.assertEqual(klong(f'.py("{fpath}")'),1)
+        self.assertEqual(klong('.hello()'),"hello, world!")
+
     def test_eval_sys_random_number(self):
         r = eval_sys_random_number()
         r2 = eval_sys_random_number()
         i = 0
         while r == r2 and i < 3:
             i += 1
             r2 = eval_sys_random_number()
```

### Comparing `klongpy-0.3.78/tests/test_util.py` & `klongpy-0.4.0/tests/test_util.py`

 * *Files identical despite different names*

