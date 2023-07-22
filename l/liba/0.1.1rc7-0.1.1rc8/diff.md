# Comparing `tmp/liba-0.1.1rc7.tar.gz` & `tmp/liba-0.1.1rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liba-0.1.1rc7.tar", last modified: Mon Jul 17 07:25:36 2023, max compression
+gzip compressed data, was "liba-0.1.1rc8.tar", last modified: Sat Jul 22 14:07:52 2023, max compression
```

## Comparing `liba-0.1.1rc7.tar` & `liba-0.1.1rc8.tar`

### file list

```diff
@@ -1,104 +1,103 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.330217 liba-0.1.1rc7/
--rwxrwxrwx   0 root         (0) root         (0)       87 2023-07-17 02:44:36.000000 liba-0.1.1rc7/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     5842 2023-07-17 07:25:36.330217 liba-0.1.1rc7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3891 2023-07-17 07:11:16.000000 liba-0.1.1rc7/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.180407 liba-0.1.1rc7/include/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.235634 liba-0.1.1rc7/include/a/
--rwxrwxrwx   0 root         (0) root         (0)    32982 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/a.h
--rwxrwxrwx   0 root         (0) root         (0)     9676 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/avl.h
--rwxrwxrwx   0 root         (0) root         (0)    11237 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/buf.h
--rwxrwxrwx   0 root         (0) root         (0)    12768 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/complex.h
--rwxrwxrwx   0 root         (0) root         (0)     1984 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/crc.h
--rwxrwxrwx   0 root         (0) root         (0)     1436 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/fuzzy.h
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.243615 liba-0.1.1rc7/include/a/host/
--rwxrwxrwx   0 root         (0) root         (0)      714 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/host/a.h
--rwxrwxrwx   0 root         (0) root         (0)    10052 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/host/que.h
--rwxrwxrwx   0 root         (0) root         (0)     8714 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/host/str.h
--rwxrwxrwx   0 root         (0) root         (0)    13007 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/host/vec.h
--rwxrwxrwx   0 root         (0) root         (0)    13397 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/host/vector.h
--rwxrwxrwx   0 root         (0) root         (0)     2097 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/hpf.h
--rwxrwxrwx   0 root         (0) root         (0)    14161 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/list.h
--rwxrwxrwx   0 root         (0) root         (0)     2025 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/lpf.h
--rwxrwxrwx   0 root         (0) root         (0)     8962 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/math.h
--rwxrwxrwx   0 root         (0) root         (0)     3387 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/mf.h
--rwxrwxrwx   0 root         (0) root         (0)   111612 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/notefreqs.h
--rwxrwxrwx   0 root         (0) root         (0)     3135 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/oop.h
--rwxrwxrwx   0 root         (0) root         (0)     2279 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/operator.h
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.246606 liba-0.1.1rc7/include/a/pid/
--rwxrwxrwx   0 root         (0) root         (0)     7360 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/pid/fuzzy.h
--rwxrwxrwx   0 root         (0) root         (0)     4398 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/pid/neuron.h
--rwxrwxrwx   0 root         (0) root         (0)     4407 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/pid.h
--rwxrwxrwx   0 root         (0) root         (0)     1313 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/poly.h
--rwxrwxrwx   0 root         (0) root         (0)    12530 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/polytrack.h
--rwxrwxrwx   0 root         (0) root         (0)     1773 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/rbf.h
--rwxrwxrwx   0 root         (0) root         (0)     9960 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/rbt.h
--rwxrwxrwx   0 root         (0) root         (0)     7032 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/slist.h
--rwxrwxrwx   0 root         (0) root         (0)     2212 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/tf.h
--rwxrwxrwx   0 root         (0) root         (0)     1610 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/utf.h
--rwxrwxrwx   0 root         (0) root         (0)     8015 2023-07-17 07:11:16.000000 liba-0.1.1rc7/include/a/version.h
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.252541 liba-0.1.1rc7/liba.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5842 2023-07-17 07:25:36.000000 liba-0.1.1rc7/liba.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1589 2023-07-17 07:25:36.000000 liba-0.1.1rc7/liba.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-17 07:25:36.000000 liba-0.1.1rc7/liba.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-07-17 07:25:36.000000 liba-0.1.1rc7/liba.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       92 2023-07-17 02:44:36.000000 liba-0.1.1rc7/pyproject.toml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.183784 liba-0.1.1rc7/python/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.256527 liba-0.1.1rc7/python/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.286469 liba-0.1.1rc7/python/src/a/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/__init__.pxd
--rwxrwxrwx   0 root         (0) root         (0)     1387 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/crc.pxd
--rwxrwxrwx   0 root         (0) root         (0)     3055 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/crc.pxi
--rwxrwxrwx   0 root         (0) root         (0)      209 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/math.pxd
--rwxrwxrwx   0 root         (0) root         (0)     1122 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/math.pxi
--rwxrwxrwx   0 root         (0) root         (0)      686 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/mf.pxd
--rwxrwxrwx   0 root         (0) root         (0)     2453 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/mf.pxi
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.292504 liba-0.1.1rc7/python/src/a/pid/
--rwxrwxrwx   0 root         (0) root         (0)     1700 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/pid/fuzzy.pxd
--rwxrwxrwx   0 root         (0) root         (0)     4476 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/pid/fuzzy.pxi
--rwxrwxrwx   0 root         (0) root         (0)      951 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/pid/neuron.pxd
--rwxrwxrwx   0 root         (0) root         (0)     3430 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/pid/neuron.pxi
--rwxrwxrwx   0 root         (0) root         (0)      945 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/pid.pxd
--rwxrwxrwx   0 root         (0) root         (0)     2435 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/pid.pxi
--rwxrwxrwx   0 root         (0) root         (0)      465 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/poly.pxd
--rwxrwxrwx   0 root         (0) root         (0)      722 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/poly.pxi
--rwxrwxrwx   0 root         (0) root         (0)     1681 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/polytrack.pxd
--rwxrwxrwx   0 root         (0) root         (0)     6340 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/polytrack.pxi
--rwxrwxrwx   0 root         (0) root         (0)      531 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/tf.pxd
--rwxrwxrwx   0 root         (0) root         (0)     1297 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/tf.pxi
--rwxrwxrwx   0 root         (0) root         (0)      308 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/version.pxd
--rwxrwxrwx   0 root         (0) root         (0)      591 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a/version.pxi
--rwxrwxrwx   0 root         (0) root         (0)  1351218 2023-07-17 07:12:57.000000 liba-0.1.1rc7/python/src/a.c
--rwxrwxrwx   0 root         (0) root         (0)     1080 2023-07-17 07:11:16.000000 liba-0.1.1rc7/python/src/a.pyx
--rwxrwxrwx   0 root         (0) root         (0)      592 2023-07-17 07:25:36.332213 liba-0.1.1rc7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     5271 2023-07-17 07:11:16.000000 liba-0.1.1rc7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.318249 liba-0.1.1rc7/src/
--rwxrwxrwx   0 root         (0) root         (0)     2650 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/a.c
--rwxrwxrwx   0 root         (0) root         (0)    25489 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/avl.c
--rwxrwxrwx   0 root         (0) root         (0)     4647 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/buf.c
--rwxrwxrwx   0 root         (0) root         (0)    24361 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/complex.c
--rwxrwxrwx   0 root         (0) root         (0)      668 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/complex.h
--rwxrwxrwx   0 root         (0) root         (0)     5952 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/crc.c
--rwxrwxrwx   0 root         (0) root         (0)      824 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/fuzzy.c
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.324232 liba-0.1.1rc7/src/host/
--rwxrwxrwx   0 root         (0) root         (0)      539 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/host/a.c
--rwxrwxrwx   0 root         (0) root         (0)     9452 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/host/que.c
--rwxrwxrwx   0 root         (0) root         (0)     5596 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/host/str.c
--rwxrwxrwx   0 root         (0) root         (0)     6818 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/host/vec.c
--rwxrwxrwx   0 root         (0) root         (0)     8156 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/host/vector.c
--rwxrwxrwx   0 root         (0) root         (0)     5704 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/math.c
--rwxrwxrwx   0 root         (0) root         (0)      257 2023-07-17 02:44:36.000000 liba-0.1.1rc7/src/math.h
--rwxrwxrwx   0 root         (0) root         (0)     2371 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/mf.c
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 07:25:36.329246 liba-0.1.1rc7/src/pid/
--rwxrwxrwx   0 root         (0) root         (0)     6695 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/pid/fuzzy.c
--rwxrwxrwx   0 root         (0) root         (0)      648 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/pid/fuzzy.h
--rwxrwxrwx   0 root         (0) root         (0)     3725 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/pid/neuron.c
--rwxrwxrwx   0 root         (0) root         (0)      876 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/pid/neuron.h
--rwxrwxrwx   0 root         (0) root         (0)     4886 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/pid.c
--rwxrwxrwx   0 root         (0) root         (0)      888 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/pid.h
--rwxrwxrwx   0 root         (0) root         (0)     1451 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/poly.c
--rwxrwxrwx   0 root         (0) root         (0)     7824 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/polytrack.c
--rwxrwxrwx   0 root         (0) root         (0)     2815 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/rbf.c
--rwxrwxrwx   0 root         (0) root         (0)    24599 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/rbt.c
--rwxrwxrwx   0 root         (0) root         (0)     1417 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/tf.c
--rwxrwxrwx   0 root         (0) root         (0)     2990 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/utf.c
--rwxrwxrwx   0 root         (0) root         (0)     1232 2023-07-17 07:11:16.000000 liba-0.1.1rc7/src/version.c
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.148629 liba-0.1.1rc8/
+-rwxrwxrwx   0 root         (0) root         (0)       87 2023-07-17 02:44:36.000000 liba-0.1.1rc8/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     5842 2023-07-22 14:07:52.148629 liba-0.1.1rc8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3891 2023-07-17 07:11:16.000000 liba-0.1.1rc8/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.005064 liba-0.1.1rc8/include/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.055415 liba-0.1.1rc8/include/a/
+-rwxrwxrwx   0 root         (0) root         (0)    34182 2023-07-22 14:04:05.000000 liba-0.1.1rc8/include/a/a.h
+-rwxrwxrwx   0 root         (0) root         (0)     9676 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/avl.h
+-rwxrwxrwx   0 root         (0) root         (0)    11237 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/buf.h
+-rwxrwxrwx   0 root         (0) root         (0)    12768 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/complex.h
+-rwxrwxrwx   0 root         (0) root         (0)     1984 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/crc.h
+-rwxrwxrwx   0 root         (0) root         (0)     1436 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/fuzzy.h
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.062854 liba-0.1.1rc8/include/a/host/
+-rwxrwxrwx   0 root         (0) root         (0)      714 2023-07-17 07:11:16.000000 liba-0.1.1rc8/include/a/host/a.h
+-rwxrwxrwx   0 root         (0) root         (0)    10052 2023-07-17 07:11:16.000000 liba-0.1.1rc8/include/a/host/que.h
+-rwxrwxrwx   0 root         (0) root         (0)     8714 2023-07-17 07:11:16.000000 liba-0.1.1rc8/include/a/host/str.h
+-rwxrwxrwx   0 root         (0) root         (0)    13007 2023-07-17 07:11:16.000000 liba-0.1.1rc8/include/a/host/vec.h
+-rwxrwxrwx   0 root         (0) root         (0)    13397 2023-07-17 07:11:16.000000 liba-0.1.1rc8/include/a/host/vector.h
+-rwxrwxrwx   0 root         (0) root         (0)     2097 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/hpf.h
+-rwxrwxrwx   0 root         (0) root         (0)    14161 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/list.h
+-rwxrwxrwx   0 root         (0) root         (0)     2025 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/lpf.h
+-rwxrwxrwx   0 root         (0) root         (0)     8461 2023-07-22 14:04:05.000000 liba-0.1.1rc8/include/a/math.h
+-rwxrwxrwx   0 root         (0) root         (0)     3387 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/mf.h
+-rwxrwxrwx   0 root         (0) root         (0)   111612 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/notefreqs.h
+-rwxrwxrwx   0 root         (0) root         (0)     3135 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/oop.h
+-rwxrwxrwx   0 root         (0) root         (0)     2279 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/operator.h
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.066845 liba-0.1.1rc8/include/a/pid/
+-rwxrwxrwx   0 root         (0) root         (0)     7360 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/pid/fuzzy.h
+-rwxrwxrwx   0 root         (0) root         (0)     4398 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/pid/neuron.h
+-rwxrwxrwx   0 root         (0) root         (0)     4407 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/pid.h
+-rwxrwxrwx   0 root         (0) root         (0)     1311 2023-07-22 14:04:05.000000 liba-0.1.1rc8/include/a/poly.h
+-rwxrwxrwx   0 root         (0) root         (0)    12530 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/polytrack.h
+-rwxrwxrwx   0 root         (0) root         (0)     1773 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/rbf.h
+-rwxrwxrwx   0 root         (0) root         (0)     9960 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/rbt.h
+-rwxrwxrwx   0 root         (0) root         (0)     7032 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/slist.h
+-rwxrwxrwx   0 root         (0) root         (0)     2212 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/tf.h
+-rwxrwxrwx   0 root         (0) root         (0)     1610 2023-07-17 07:30:14.000000 liba-0.1.1rc8/include/a/utf.h
+-rwxrwxrwx   0 root         (0) root         (0)     8015 2023-07-22 14:04:05.000000 liba-0.1.1rc8/include/a/version.h
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.072908 liba-0.1.1rc8/liba.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5842 2023-07-22 14:07:51.000000 liba-0.1.1rc8/liba.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1567 2023-07-22 14:07:51.000000 liba-0.1.1rc8/liba.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-22 14:07:51.000000 liba-0.1.1rc8/liba.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-07-22 14:07:51.000000 liba-0.1.1rc8/liba.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       92 2023-07-17 02:44:36.000000 liba-0.1.1rc8/pyproject.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.009081 liba-0.1.1rc8/python/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.077885 liba-0.1.1rc8/python/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.105434 liba-0.1.1rc8/python/src/a/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-17 07:30:14.000000 liba-0.1.1rc8/python/src/a/__init__.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     1387 2023-07-17 07:30:14.000000 liba-0.1.1rc8/python/src/a/crc.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     3135 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a/crc.pxi
+-rwxrwxrwx   0 root         (0) root         (0)      209 2023-07-17 07:11:16.000000 liba-0.1.1rc8/python/src/a/math.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      686 2023-07-17 07:11:16.000000 liba-0.1.1rc8/python/src/a/mf.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     2493 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a/mf.pxi
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.110463 liba-0.1.1rc8/python/src/a/pid/
+-rwxrwxrwx   0 root         (0) root         (0)     1700 2023-07-17 07:30:14.000000 liba-0.1.1rc8/python/src/a/pid/fuzzy.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     4663 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a/pid/fuzzy.pxi
+-rwxrwxrwx   0 root         (0) root         (0)      951 2023-07-17 07:30:14.000000 liba-0.1.1rc8/python/src/a/pid/neuron.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     3621 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a/pid/neuron.pxi
+-rwxrwxrwx   0 root         (0) root         (0)      945 2023-07-17 07:30:14.000000 liba-0.1.1rc8/python/src/a/pid.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     2552 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a/pid.pxi
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a/poly.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      796 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a/poly.pxi
+-rwxrwxrwx   0 root         (0) root         (0)     1681 2023-07-17 07:11:16.000000 liba-0.1.1rc8/python/src/a/polytrack.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     6485 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a/polytrack.pxi
+-rwxrwxrwx   0 root         (0) root         (0)      531 2023-07-17 07:30:14.000000 liba-0.1.1rc8/python/src/a/tf.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     1410 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a/tf.pxi
+-rwxrwxrwx   0 root         (0) root         (0)      308 2023-07-17 07:11:16.000000 liba-0.1.1rc8/python/src/a/version.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      591 2023-07-17 07:11:16.000000 liba-0.1.1rc8/python/src/a/version.pxi
+-rwxrwxrwx   0 root         (0) root         (0)  2699593 2023-07-22 14:07:51.000000 liba-0.1.1rc8/python/src/a.c
+-rwxrwxrwx   0 root         (0) root         (0)     7261 2023-07-22 14:04:05.000000 liba-0.1.1rc8/python/src/a.pyx
+-rwxrwxrwx   0 root         (0) root         (0)      592 2023-07-22 14:07:52.149659 liba-0.1.1rc8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     5271 2023-07-17 07:11:16.000000 liba-0.1.1rc8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.136247 liba-0.1.1rc8/src/
+-rwxrwxrwx   0 root         (0) root         (0)     2636 2023-07-22 14:04:05.000000 liba-0.1.1rc8/src/a.c
+-rwxrwxrwx   0 root         (0) root         (0)    25489 2023-07-17 07:30:14.000000 liba-0.1.1rc8/src/avl.c
+-rwxrwxrwx   0 root         (0) root         (0)     4647 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/buf.c
+-rwxrwxrwx   0 root         (0) root         (0)    24361 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/complex.c
+-rwxrwxrwx   0 root         (0) root         (0)      668 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/complex.h
+-rwxrwxrwx   0 root         (0) root         (0)     5952 2023-07-17 07:30:14.000000 liba-0.1.1rc8/src/crc.c
+-rwxrwxrwx   0 root         (0) root         (0)      824 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/fuzzy.c
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.141685 liba-0.1.1rc8/src/host/
+-rwxrwxrwx   0 root         (0) root         (0)      539 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/host/a.c
+-rwxrwxrwx   0 root         (0) root         (0)     9452 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/host/que.c
+-rwxrwxrwx   0 root         (0) root         (0)     5548 2023-07-22 14:04:05.000000 liba-0.1.1rc8/src/host/str.c
+-rwxrwxrwx   0 root         (0) root         (0)     6820 2023-07-22 14:04:05.000000 liba-0.1.1rc8/src/host/vec.c
+-rwxrwxrwx   0 root         (0) root         (0)     8158 2023-07-22 14:04:05.000000 liba-0.1.1rc8/src/host/vector.c
+-rwxrwxrwx   0 root         (0) root         (0)     5704 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/math.c
+-rwxrwxrwx   0 root         (0) root         (0)      257 2023-07-17 02:44:36.000000 liba-0.1.1rc8/src/math.h
+-rwxrwxrwx   0 root         (0) root         (0)     2371 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/mf.c
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-22 14:07:52.147633 liba-0.1.1rc8/src/pid/
+-rwxrwxrwx   0 root         (0) root         (0)     6715 2023-07-22 14:04:05.000000 liba-0.1.1rc8/src/pid/fuzzy.c
+-rwxrwxrwx   0 root         (0) root         (0)      648 2023-07-22 13:55:07.000000 liba-0.1.1rc8/src/pid/fuzzy.h
+-rwxrwxrwx   0 root         (0) root         (0)     3725 2023-07-17 07:30:14.000000 liba-0.1.1rc8/src/pid/neuron.c
+-rwxrwxrwx   0 root         (0) root         (0)      876 2023-07-17 07:30:14.000000 liba-0.1.1rc8/src/pid/neuron.h
+-rwxrwxrwx   0 root         (0) root         (0)     4886 2023-07-17 07:30:14.000000 liba-0.1.1rc8/src/pid.c
+-rwxrwxrwx   0 root         (0) root         (0)      868 2023-07-22 14:04:05.000000 liba-0.1.1rc8/src/pid.h
+-rwxrwxrwx   0 root         (0) root         (0)     1452 2023-07-22 14:04:05.000000 liba-0.1.1rc8/src/poly.c
+-rwxrwxrwx   0 root         (0) root         (0)     7824 2023-07-17 07:30:14.000000 liba-0.1.1rc8/src/polytrack.c
+-rwxrwxrwx   0 root         (0) root         (0)     2815 2023-07-17 07:30:14.000000 liba-0.1.1rc8/src/rbf.c
+-rwxrwxrwx   0 root         (0) root         (0)    24599 2023-07-17 07:30:14.000000 liba-0.1.1rc8/src/rbt.c
+-rwxrwxrwx   0 root         (0) root         (0)     1417 2023-07-17 07:30:14.000000 liba-0.1.1rc8/src/tf.c
+-rwxrwxrwx   0 root         (0) root         (0)     2990 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/utf.c
+-rwxrwxrwx   0 root         (0) root         (0)     1232 2023-07-17 07:11:16.000000 liba-0.1.1rc8/src/version.c
```

### Comparing `liba-0.1.1rc7/PKG-INFO` & `liba-0.1.1rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liba
-Version: 0.1.1rc7
+Version: 0.1.1rc8
 Summary: An algorithm library based on C/C++ language
 Home-page: https://github.com/tqfx/liba.git
 Author: tqfx
 Author-email: tqfx@foxmail.com
 License: MPL-2.0
 Description: # An algorithm library {#mainpage}
```

### Comparing `liba-0.1.1rc7/README.md` & `liba-0.1.1rc8/README.md`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/a.h` & `liba-0.1.1rc8/include/a/a.h`

 * *Files 5% similar despite different names*

```diff
@@ -271,28 +271,31 @@
 #include <float.h>
 
 /*!
  @addtogroup A algorithm library
  @{
 */
 
+/*! assert a build-time dependency, as an expression */
+#define A_ASSERT_BUILD(x) (sizeof(char[1 - 2 * !(x)]) - 1)
+
 #if defined(__cplusplus)
 #define a_cast_r(T, x) reinterpret_cast<T>(x)
 #define a_cast_d(T, x) dynamic_cast<T>(x)
 #define a_cast_s(T, x) static_cast<T>(x)
 #define a_cast_c(T, x) const_cast<T>(x)
 #else /* !__cplusplus */
 #define a_cast_r(T, x) ((T)(x))
 #define a_cast_d(T, x) ((T)(x))
 #define a_cast_s(T, x) ((T)(x))
 #define a_cast_c(T, x) ((T)(x))
 #endif /* __cplusplus */
-#define A_CASE_3(a, b, c) a##b##c
-#define A_CASE_2(a, b) a##b
-#define A_CASE_1(a) #a
+#define A_CAST_3(a, b, c) a##b##c
+#define A_CAST_2(a, b) a##b
+#define A_CAST_1(a) #a
 
 #if defined(__cplusplus) && defined(A_HAVE_NULLPTR)
 #define A_NULL nullptr
 #else /* !__cplusplus */
 #define A_NULL NULL
 #endif /* __cplusplus */
 
@@ -600,21 +603,21 @@
 
 #define A_F16_NNAN A_U16_C(0xFE00)
 #define A_F16_PNAN A_U16_C(0x7E00)
 #define A_F16_NINF A_U16_C(0xFC00)
 #define A_F16_PINF A_U16_C(0x7C00)
 
 #define A_F32_T float
-#define A_F32_C(X) A_CASE_2(X, F)
-#define A_F32_F(F) A_CASE_2(F, f)
-#define A_F32_F1(F, a) A_CASE_2(F, f)(a)
-#define A_F32_F2(F, a, b) A_CASE_2(F, f)(a, b)
-#define A_F32_F3(F, a, b, c) A_CASE_2(F, f)(a, b, c)
+#define A_F32_C(X) A_CAST_2(X, F)
+#define A_F32_F(F) A_CAST_2(F, f)
+#define A_F32_F1(F, a) A_CAST_2(F, f)(a)
+#define A_F32_F2(F, a, b) A_CAST_2(F, f)(a, b)
+#define A_F32_F3(F, a, b, c) A_CAST_2(F, f)(a, b, c)
 #if defined(A_HAVE_VARIADIC_MACROS)
-#define A_F32_FN(F, ...) A_CASE_2(F, f)(__VA_ARGS__)
+#define A_F32_FN(F, ...) A_CAST_2(F, f)(__VA_ARGS__)
 #endif /* A_HAVE_VARIADIC_MACROS */
 #define A_F32_DIG FLT_DIG
 #define A_F32_EPSILON FLT_EPSILON
 #define A_F32_MANT_DIG FLT_MANT_DIG
 #define A_F32_MAX FLT_MAX
 #define A_F32_MAX_10_EXP FLT_MAX_10_EXP
 #define A_F32_MAX_EXP FLT_MAX_EXP
@@ -699,24 +702,24 @@
 #define A_FLOAT_MIN FLT_MIN
 #define A_FLOAT_MIN_10_EXP FLT_MIN_10_EXP
 #define A_FLOAT_MIN_EXP FLT_MIN_EXP
 
 /*!
  expands to a floating-point constant expression having the value specified by its argument and the type \ref a_float_t
 */
-#define A_FLOAT_C(X) A_CASE_2(X, F)
+#define A_FLOAT_C(X) A_CAST_2(X, F)
 /*!
  expands to a floating-point function expression having the value specified by its argument and the type \ref a_float_t
 */
-#define A_FLOAT_F(F) A_CASE_2(F, f)
-#define A_FLOAT_F1(F, a) A_CASE_2(F, f)(a)
-#define A_FLOAT_F2(F, a, b) A_CASE_2(F, f)(a, b)
-#define A_FLOAT_F3(F, a, b, c) A_CASE_2(F, f)(a, b, c)
+#define A_FLOAT_F(F) A_CAST_2(F, f)
+#define A_FLOAT_F1(F, a) A_CAST_2(F, f)(a)
+#define A_FLOAT_F2(F, a, b) A_CAST_2(F, f)(a, b)
+#define A_FLOAT_F3(F, a, b, c) A_CAST_2(F, f)(a, b, c)
 #if defined(A_HAVE_VARIADIC_MACROS)
-#define A_FLOAT_FN(F, ...) A_CASE_2(F, f)(__VA_ARGS__)
+#define A_FLOAT_FN(F, ...) A_CAST_2(F, f)(__VA_ARGS__)
 #endif /* A_HAVE_VARIADIC_MACROS */
 
 /*! format constants for the fprintf family of functions */
 #define A_FLOAT_PRI(F, C) "%" F C
 /*! format constants for the fscanf family of functions */
 #define A_FLOAT_SCN(F, C) "%" F C
 
@@ -767,24 +770,24 @@
 #define A_FLOAT_MIN LDBL_MIN
 #define A_FLOAT_MIN_10_EXP LDBL_MIN_10_EXP
 #define A_FLOAT_MIN_EXP LDBL_MIN_EXP
 
 /*!
  expands to a floating-point constant expression having the value specified by its argument and the type \ref a_float_t
 */
-#define A_FLOAT_C(X) A_CASE_2(X, L)
+#define A_FLOAT_C(X) A_CAST_2(X, L)
 /*!
  expands to a floating-point function expression having the value specified by its argument and the type \ref a_float_t
 */
-#define A_FLOAT_F(F) A_CASE_2(F, l)
-#define A_FLOAT_F1(F, a) A_CASE_2(F, l)(a)
-#define A_FLOAT_F2(F, a, b) A_CASE_2(F, l)(a, b)
-#define A_FLOAT_F3(F, a, b, c) A_CASE_2(F, l)(a, b, c)
+#define A_FLOAT_F(F) A_CAST_2(F, l)
+#define A_FLOAT_F1(F, a) A_CAST_2(F, l)(a)
+#define A_FLOAT_F2(F, a, b) A_CAST_2(F, l)(a, b)
+#define A_FLOAT_F3(F, a, b, c) A_CAST_2(F, l)(a, b, c)
 #if defined(A_HAVE_VARIADIC_MACROS)
-#define A_FLOAT_FN(F, ...) A_CASE_2(F, l)(__VA_ARGS__)
+#define A_FLOAT_FN(F, ...) A_CAST_2(F, l)(__VA_ARGS__)
 #endif /* A_HAVE_VARIADIC_MACROS */
 
 /*! format constants for the fprintf family of functions */
 #define A_FLOAT_PRI(F, C) "%" F "L" C
 /*! format constants for the fscanf family of functions */
 #define A_FLOAT_SCN(F, C) "%" F "L" C
 
@@ -843,25 +846,48 @@
     char *str;
 #if defined(A_FLOAT_TYPE) && (A_FLOAT_TYPE + 0 < A_FLOAT_EXTEND)
     a_float_t f;
 #endif /* A_FLOAT_TYPE */
 } a_cast_u;
 
 /*!
- @brief size of memory that alignment is specified by alignment
- @param base specifies the alignment that is a power of two
- @param size number of bytes to allocate
+ @brief square of x, \f$ x^2 \f$
+*/
+#define A_SQ(x) ((x) * (x))
+
+/*!
+ @brief minimum value between x and y
+*/
+#define A_MIN(x, y) (((x) < (y)) ? (x) : (y))
+
+/*!
+ @brief maximum value between x and y
+*/
+#define A_MAX(x, y) (((x) > (y)) ? (x) : (y))
+
+/*!
+ @brief absolute value of x, \f$ |x| \f$
+*/
+#define A_ABS(x) ((x) < 0 ? -(x) : (x))
+
+/*!
+ @brief signum function, \f$ \texttt{sgn}{x}=\begin{cases}+1&x>0\\0&0\\-1&x<0\end{cases} \f$
+*/
+#define A_SGN(x) ((0 < (x)) - ((x) < 0))
+
+/*!
+ @brief saturation value of x, \f$ \texttt{sat}(x,min,max)=\begin{cases}min&min>x\\max&x>max\\x&else\end{cases} \f$
 */
-#define a_align(base, size) ((a_cast_s(a_size_t, size) + (base)-1) & ~((base)-1))
+#define A_SAT(x, min, max) ((min) < (x) ? (x) < (max) ? (x) : (max) : (min))
 
 /*!
- @brief count of an array buffer
- @param array must be an array variable
+ @brief number of elements in a visible array
+ @param array must be a visible array
 */
-#define a_count_of(array) (sizeof(array) / sizeof(*(array)))
+#define a_array_n(array) (sizeof(array) / sizeof(*(array)))
 
 /*!
  @brief offset of a structure member
  @param type structure type
  @param member member variable
 */
 #if defined(offsetof)
@@ -875,14 +901,34 @@
  @param ptr pointer to a member variable
  @param type structure type
  @param member member variable
 */
 #define a_container_of(ptr, type, member) a_cast_r(type *, a_cast_r(a_uptr_t, ptr) - a_offsetof(type, member))
 
 /*!
+ @brief round down size "n" to be a multiple of "a"
+*/
+#define a_size_down(a, n) (a_cast_s(a_size_t, n) & ~a_cast_s(a_size_t, (a)-1))
+
+/*!
+ @brief round up size "n" to be a multiple of "a"
+*/
+#define a_size_up(a, n) ((a_cast_s(a_size_t, n) + (a)-1) & ~a_cast_s(a_size_t, (a)-1))
+
+/*!
+ @brief round pointer "p" down to the closest "a"-aligned address <= "p"
+*/
+#define a_align_down(a, p) a_cast_r(void *, a_cast_r(a_uptr_t, p) & ~a_cast_s(a_uptr_t, (a)-1))
+
+/*!
+ @brief round pointer "p" up to the closest "a"-aligned address >= "p"
+*/
+#define a_align_up(a, p) a_cast_r(void *, (a_cast_r(a_uptr_t, p) + (a)-1) & ~a_cast_s(a_uptr_t, (a)-1))
+
+/*!
  @brief iterate from 0 to n and not include n
  @param I index type of the iteration
  @param i index variable of the iteration
  @param n final value of the iteration
 */
 #define a_forenum(I, i, n) for (I i = 0; i < (n); ++i)
```

### Comparing `liba-0.1.1rc7/include/a/avl.h` & `liba-0.1.1rc8/include/a/avl.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/buf.h` & `liba-0.1.1rc8/include/a/buf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/complex.h` & `liba-0.1.1rc8/include/a/complex.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/crc.h` & `liba-0.1.1rc8/include/a/crc.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/fuzzy.h` & `liba-0.1.1rc8/include/a/fuzzy.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/host/a.h` & `liba-0.1.1rc8/include/a/host/a.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/host/que.h` & `liba-0.1.1rc8/include/a/host/que.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/host/str.h` & `liba-0.1.1rc8/include/a/host/str.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/host/vec.h` & `liba-0.1.1rc8/include/a/host/vec.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/host/vector.h` & `liba-0.1.1rc8/include/a/host/vector.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/hpf.h` & `liba-0.1.1rc8/include/a/hpf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/list.h` & `liba-0.1.1rc8/include/a/list.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/lpf.h` & `liba-0.1.1rc8/include/a/lpf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/math.h` & `liba-0.1.1rc8/include/a/math.h`

 * *Files 2% similar despite different names*

```diff
@@ -38,34 +38,14 @@
 /*! \f$ \frac{2}{\sqrt{\pi}} \f$ */
 #define A_2_SQRTPI 1.12837916709551257390
 /*! \f$ \sqrt{2} \f$ */
 #define A_SQRT2 1.41421356237309504880
 /*! \f$ \frac{1}{\sqrt{2}}=\frac{\sqrt{2}}{2} \f$ */
 #define A_SQRT1_2 0.707106781186547524401
 
-/*!
- @brief square of x, \f$ x^2 \f$
-*/
-#define A_SQ(x) ((x) * (x))
-
-/*!
- @brief absolute value of x, \f$ |x| \f$
-*/
-#define A_ABS(x) ((x) < 0 ? -(x) : (x))
-
-/*!
- @brief signum function, \f$ \texttt{sgn}{x}=\begin{cases}+1&x>0\\0&0\\-1&x<0\end{cases} \f$
-*/
-#define A_SGN(x) ((0 < (x)) - ((x) < 0))
-
-/*!
- @brief saturation value of x, \f$ \texttt{sat}(x,min,max)=\begin{cases}min&min>x\\max&x>max\\x&else\end{cases} \f$
-*/
-#define A_SAT(x, min, max) ((min) < (x) ? (x) < (max) ? (x) : (max) : (min))
-
 #if defined(__cplusplus)
 extern "C" {
 #endif /* __cplusplus */
 
 A_EXTERN a_f32_t a_f32_hypot(a_f32_t x, a_f32_t y);
 A_EXTERN a_f64_t a_f64_hypot(a_f64_t x, a_f64_t y);
```

### Comparing `liba-0.1.1rc7/include/a/mf.h` & `liba-0.1.1rc8/include/a/mf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/notefreqs.h` & `liba-0.1.1rc8/include/a/notefreqs.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/oop.h` & `liba-0.1.1rc8/include/a/oop.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/operator.h` & `liba-0.1.1rc8/include/a/operator.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/pid/fuzzy.h` & `liba-0.1.1rc8/include/a/pid/fuzzy.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/pid/neuron.h` & `liba-0.1.1rc8/include/a/pid/neuron.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/pid.h` & `liba-0.1.1rc8/include/a/pid.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/poly.h` & `liba-0.1.1rc8/include/a/poly.h`

 * *Files 17% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 */
 
 #if defined(__cplusplus)
 extern "C" {
 #endif /* __cplusplus */
 
 /*!
- @brief convert between \f$ \sum_{i=0}^{n}a_{i}x^{i} \f$ and \f$ \sum_{i=0}^{n}a_{i}x^{n-i} \f$
+ @brief swap between \f$ \sum_{i=0}^{n}a_{i}x^{i} \f$ and \f$ \sum_{i=0}^{n}a_{i}x^{n-i} \f$
 */
-A_EXTERN a_float_t *a_poly_inv(a_float_t *a, a_size_t n);
+A_EXTERN a_float_t *a_poly_swap(a_float_t *a, a_size_t n);
 
 /*!
  @brief horner function for polynomial \f$ \sum_{i=0}^{n}a_{i}x^{i} \f$
  \f[
   \left\{\begin{array}{l}
   S_n = a_n\\
   S_i = xS_{i+1} + a_i,\quad(i=n-1,n-2,\cdots,1,0)\\
```

### Comparing `liba-0.1.1rc7/include/a/polytrack.h` & `liba-0.1.1rc8/include/a/polytrack.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/rbf.h` & `liba-0.1.1rc8/include/a/rbf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/rbt.h` & `liba-0.1.1rc8/include/a/rbt.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/slist.h` & `liba-0.1.1rc8/include/a/slist.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/tf.h` & `liba-0.1.1rc8/include/a/tf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/utf.h` & `liba-0.1.1rc8/include/a/utf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/include/a/version.h` & `liba-0.1.1rc8/include/a/version.h`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 #undef patch
 
 /*! algorithm library version tweak */
 #ifndef A_VERSION_TWEAK
 #define A_VERSION_TWEAK A_U64_C(0)
 #endif /* A_VERSION_TWEAK */
 
-#define A_VERSION_TOSTR(X) A_CASE_1(X)
+#define A_VERSION_TOSTR(X) A_CAST_1(X)
 /*! algorithm library version string */
 #ifndef A_VERSION
 #define A_VERSION A_VERSION_TOSTR(A_VERSION_MAJOR) "." A_VERSION_TOSTR(A_VERSION_MINOR) "." A_VERSION_TOSTR(A_VERSION_PATCH)
 #endif /* A_VERSION */
 
 #if defined(__cplusplus)
 #define A_VERSION_C(maj, min, pat) a::version(maj, min, pat)
```

### Comparing `liba-0.1.1rc7/liba.egg-info/PKG-INFO` & `liba-0.1.1rc8/liba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liba
-Version: 0.1.1rc7
+Version: 0.1.1rc8
 Summary: An algorithm library based on C/C++ language
 Home-page: https://github.com/tqfx/liba.git
 Author: tqfx
 Author-email: tqfx@foxmail.com
 License: MPL-2.0
 Description: # An algorithm library {#mainpage}
```

### Comparing `liba-0.1.1rc7/liba.egg-info/SOURCES.txt` & `liba-0.1.1rc8/liba.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 liba.egg-info/top_level.txt
 python/src/a.c
 python/src/a.pyx
 python/src/a/__init__.pxd
 python/src/a/crc.pxd
 python/src/a/crc.pxi
 python/src/a/math.pxd
-python/src/a/math.pxi
 python/src/a/mf.pxd
 python/src/a/mf.pxi
 python/src/a/pid.pxd
 python/src/a/pid.pxi
 python/src/a/poly.pxd
 python/src/a/poly.pxi
 python/src/a/polytrack.pxd
```

### Comparing `liba-0.1.1rc7/python/src/a/__init__.pxd` & `liba-0.1.1rc8/python/src/a/__init__.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/python/src/a/crc.pxd` & `liba-0.1.1rc8/python/src/a/crc.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/python/src/a/crc.pxi` & `liba-0.1.1rc8/python/src/a/crc.pxi`

 * *Files 12% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 cdef class crc8:
     POLY = A_CRC8_POLY
     INIT = A_CRC8_INIT
     cdef array table
-    @property
-    def table(self):
-        return self.table
-    def __cinit__(self, poly: a_u8_t = A_CRC8_POLY, high = False):
-        self.table = u8s([0] * A_CRC_SIZ)
+    property table:
+        def __get__(self):
+            return self.table
+    def __init__(self, poly: a_u8_t = A_CRC8_POLY, high = False):
+        self.table = u8.array([0] * A_CRC_SIZ)
         if high:
             a_crc8h_init(<a_u8_t *>self.table.data.as_voidptr, poly)
         else:
             a_crc8l_init(<a_u8_t *>self.table.data.as_voidptr, poly)
     def __call__(self, data: bytes, init: a_u8_t = A_CRC8_INIT) -> a_u8_t:
         return a_crc8(<a_u8_t *>self.table.data.as_voidptr, <const void *>data, len(data), init)
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 cdef class crc16:
     POLY = A_CRC16_POLY
     INIT = A_CRC16_INIT
     cdef array table
-    @property
-    def table(self):
-        return self.table
+    property table:
+        def __get__(self):
+            return self.table
     cdef a_u16_t (*f)(const a_u16_t *, const void *, a_size_t, a_u16_t)
-    def __cinit__(self, poly: a_u16_t = A_CRC16_POLY, high = False):
-        self.table = u16s([0] * A_CRC_SIZ)
+    def __init__(self, poly: a_u16_t = A_CRC16_POLY, high = False):
+        self.table = u16.array([0] * A_CRC_SIZ)
         if high:
             self.f = a_crc16h
             a_crc16h_init(<a_u16_t *>self.table.data.as_voidptr, poly)
         else:
             self.f = a_crc16l
             a_crc16l_init(<a_u16_t *>self.table.data.as_voidptr, poly)
     def __call__(self, data: bytes, init: a_u16_t = A_CRC16_INIT) -> a_u16_t:
@@ -41,20 +41,20 @@
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 cdef class crc32:
     POLY = A_CRC32_POLY
     INIT = A_CRC32_INIT
     cdef array table
-    @property
-    def table(self):
-        return self.table
+    property table:
+        def __get__(self):
+            return self.table
     cdef a_u32_t (*f)(const a_u32_t *, const void *, a_size_t, a_u32_t)
-    def __cinit__(self, poly: a_u32_t = A_CRC32_POLY, high = False):
-        self.table = u32s([0] * A_CRC_SIZ)
+    def __init__(self, poly: a_u32_t = A_CRC32_POLY, high = False):
+        self.table = u32.array([0] * A_CRC_SIZ)
         if high:
             self.f = a_crc32h
             a_crc32h_init(<a_u32_t *>self.table.data.as_voidptr, poly)
         else:
             self.f = a_crc32l
             a_crc32l_init(<a_u32_t *>self.table.data.as_voidptr, poly)
     def __call__(self, data: bytes, init: a_u32_t = A_CRC32_INIT) -> a_u32_t:
@@ -62,20 +62,20 @@
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 cdef class crc64:
     POLY = A_CRC64_POLY
     INIT = A_CRC64_INIT
     cdef array table
-    @property
-    def table(self):
-        return self.table
+    property table:
+        def __get__(self):
+            return self.table
     cdef a_u64_t (*f)(const a_u64_t *, const void *, a_size_t, a_u64_t)
-    def __cinit__(self, poly: a_u64_t = A_CRC64_POLY, high = False):
-        self.table = u64s([0] * A_CRC_SIZ)
+    def __init__(self, poly: a_u64_t = A_CRC64_POLY, high = False):
+        self.table = u64.array([0] * A_CRC_SIZ)
         if high:
             self.f = a_crc64h
             a_crc64h_init(<a_u64_t *>self.table.data.as_voidptr, poly)
         else:
             self.f = a_crc64l
             a_crc64l_init(<a_u64_t *>self.table.data.as_voidptr, poly)
     def __call__(self, data: bytes, init: a_u64_t = A_CRC64_INIT) -> a_u64_t:
```

### Comparing `liba-0.1.1rc7/python/src/a/mf.pxd` & `liba-0.1.1rc8/python/src/a/mf.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/python/src/a/mf.pxi` & `liba-0.1.1rc8/python/src/a/mf.pxi`

 * *Files 8% similar despite different names*

```diff
@@ -9,69 +9,69 @@
     GBELL = A_MF_GBELL
     SIG   = A_MF_SIG
     TRAP  = A_MF_TRAP
     TRI   = A_MF_TRI
     Z     = A_MF_Z
     @staticmethod
     def __call__(e: a_mf_e, x, a):
-        cdef array d = floats(a)
-        cdef a_float_t *v = <a_float_t *>d.data.as_voidptr
+        cdef array f = float.array(a)
+        cdef a_float_t *v = <a_float_t *>f.data.as_voidptr
         if iterable(x):
-            y = floats(x)
+            y = float.array(x)
             for i, it in enumerate(x):
                 y[i] = a_mf(e, it, v)
             return y
         return a_mf(e, x, v)
     @staticmethod
     def gauss(x, sigma: a_float_t, c: a_float_t):
         '''Gaussian membership function'''
         if iterable(x):
-            y = floats(x)
+            y = float.array(x)
             for i, it in enumerate(x):
                 y[i] = a_mf_gauss(it, sigma, c)
             return y
         return a_mf_gauss(x, sigma, c)
     @staticmethod
     def gbell(x, a: a_float_t, b: a_float_t, c: a_float_t):
         '''Generalized bell-shaped membership function'''
         if iterable(x):
-            y = floats(x)
+            y = float.array(x)
             for i, it in enumerate(x):
                 y[i] = a_mf_gbell(it, a, b, c)
             return y
         return a_mf_gbell(x, a, b, c)
     @staticmethod
     def sig(x, a: a_float_t, c: a_float_t):
         '''Sigmoidal membership function'''
         if iterable(x):
-            y = floats(x)
+            y = float.array(x)
             for i, it in enumerate(x):
                 y[i] = a_mf_sig(it, a, c)
             return y
         return a_mf_sig(x, a, c)
     @staticmethod
     def trap(x, a: a_float_t, b: a_float_t, c: a_float_t, d: a_float_t):
         '''Trapezoidal membership function'''
         if iterable(x):
-            y = floats(x)
+            y = float.array(x)
             for i, it in enumerate(x):
                 y[i] = a_mf_trap(it, a, b, c, d)
             return y
         return a_mf_trap(x, a, b, c, d)
     @staticmethod
     def tri(x, a: a_float_t, b: a_float_t, c: a_float_t):
         '''Triangular membership function'''
         if iterable(x):
-            y = floats(x)
+            y = float.array(x)
             for i, it in enumerate(x):
                 y[i] = a_mf_tri(it, a, b, c)
             return y
         return a_mf_tri(x, a, b, c)
     @staticmethod
     def z(x, a: a_float_t, b: a_float_t):
         '''Z-shaped membership function'''
         if iterable(x):
-            y = floats(x)
+            y = float.array(x)
             for i, it in enumerate(x):
                 y[i] = a_mf_z(it, a, b)
             return y
         return a_mf_z(x, a, b)
```

### Comparing `liba-0.1.1rc7/python/src/a/pid/fuzzy.pxd` & `liba-0.1.1rc8/python/src/a/pid/fuzzy.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/python/src/a/pid/fuzzy.pxi` & `liba-0.1.1rc8/python/src/a/pid/fuzzy.pxi`

 * *Files 14% similar despite different names*

```diff
@@ -29,19 +29,19 @@
         if sum:
             self.ctx.pid.mode = A_PID_POS
         else:
             self.ctx.pid.mode = A_PID_INC
         a_pid_fuzzy_set_op(&self.ctx, A_PID_FUZZY_EQU)
     def rule(self, me, mec, mkp, mki, mkd):
         '''set rule base for fuzzy PID controller'''
-        self.me = floats((col for row in me for col in row))
-        self.mec = floats((col for row in mec for col in row))
-        self.mkp = floats((col for row in mkp for col in row))
-        self.mki = floats((col for row in mki for col in row))
-        self.mkd = floats((col for row in mkd for col in row))
+        self.me = float.array((col for row in me for col in row))
+        self.mec = float.array((col for row in mec for col in row))
+        self.mkp = float.array((col for row in mkp for col in row))
+        self.mki = float.array((col for row in mki for col in row))
+        self.mkd = float.array((col for row in mkd for col in row))
         a_pid_fuzzy_rule(&self.ctx, <unsigned int>len(me),
                          <a_float_t *>self.me.data.as_voidptr,
                          <a_float_t *>self.mec.data.as_voidptr,
                          <a_float_t *>self.mkp.data.as_voidptr,
                          <a_float_t *>self.mki.data.as_voidptr,
                          <a_float_t *>self.mkd.data.as_voidptr)
         return self
@@ -64,67 +64,60 @@
     def __dealloc__(self):
         '''terminate function for fuzzy PID controller'''
         PyMem_Free(self.ptr)
     def zero(self):
         '''zero clear function for fuzzy PID controller'''
         a_pid_fuzzy_zero(&self.ctx)
         return self
-    @property
-    def kp(self) -> a_float_t:
-        return self.ctx.kp
-    @kp.setter
-    def kp(self, kp: a_float_t):
-        self.ctx.pid.kp = kp
-        self.ctx.kp = kp
-    @property
-    def ki(self) -> a_float_t:
-        return self.ctx.ki
-    @ki.setter
-    def ki(self, ki: a_float_t):
-        self.ctx.pid.ki = ki
-        self.ctx.ki = ki
-    @property
-    def kd(self) -> a_float_t:
-        return self.ctx.kd
-    @kd.setter
-    def kd(self, kd: a_float_t):
-        self.ctx.pid.kd = kd
-        self.ctx.kd = kd
-    @property
-    def summax(self) -> a_float_t:
-        return self.ctx.pid.summax
-    @summax.setter
-    def summax(self, summax: a_float_t):
-        self.ctx.pid.summax = summax
-    @property
-    def outmax(self) -> a_float_t:
-        return self.ctx.pid.outmax
-    @outmax.setter
-    def outmax(self, outmax: a_float_t):
-        self.ctx.pid.outmax = outmax
-    @property
-    def outmin(self) -> a_float_t:
-        return self.ctx.pid.outmin
-    @outmin.setter
-    def outmin(self, outmin: a_float_t):
-        self.ctx.pid.outmin = outmin
-    @property
-    def out(self) -> a_float_t:
-        return self.ctx.pid.out.f
-    @property
-    def fdb(self) -> a_float_t:
-        return self.ctx.pid.fdb.f
-    @property
-    def err(self) -> a_float_t:
-        return self.ctx.pid.err.f
-    @property
-    def mode(self) -> int:
-        return self.ctx.pid.mode
-    @mode.setter
-    def mode(self, mode: int):
-        self.ctx.pid.mode = mode
-    @property
-    def col(self) -> int:
-        return self.ctx.col
-    @property
-    def buf(self) -> int:
-        return self.ctx.buf
+    property kp:
+        def __get__(self) -> a_float_t:
+            return self.ctx.kp
+        def __set__(self, kp: a_float_t):
+            self.ctx.pid.kp = kp
+            self.ctx.kp = kp
+    property ki:
+        def __get__(self) -> a_float_t:
+            return self.ctx.ki
+        def __set__(self, ki: a_float_t):
+            self.ctx.pid.ki = ki
+            self.ctx.ki = ki
+    property kd:
+        def __get__(self) -> a_float_t:
+            return self.ctx.kd
+        def __set__(self, kd: a_float_t):
+            self.ctx.pid.kd = kd
+            self.ctx.kd = kd
+    property summax:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.summax
+        def __set__(self, summax: a_float_t):
+            self.ctx.pid.summax = summax
+    property outmax:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.outmax
+        def __set__(self, outmax: a_float_t):
+            self.ctx.pid.outmax = outmax
+    property outmin:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.outmin
+        def __set__(self, outmin: a_float_t):
+            self.ctx.pid.outmin = outmin
+    property out:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.out.f
+    property fdb:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.fdb.f
+    property err:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.err.f
+    property mode:
+        def __get__(self) -> int:
+            return self.ctx.pid.mode
+        def __set__(self, mode: int):
+            self.ctx.pid.mode = mode
+    property col:
+        def __get__(self) -> int:
+            return self.ctx.col
+    property buf:
+        def __get__(self) -> int:
+            return self.ctx.buf
```

### Comparing `liba-0.1.1rc7/python/src/a/pid/neuron.pxd` & `liba-0.1.1rc8/python/src/a/pid/neuron.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/python/src/a/pid/neuron.pxi` & `liba-0.1.1rc8/python/src/a/pid/neuron.pxi`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from neuron cimport *
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 cdef class pid_neuron:
     '''single neuron proportional integral derivative controller'''
     cdef a_pid_neuron_s ctx
-    def __cinit__(self, a_float_t min = -A_FLOAT_INF, a_float_t max = +A_FLOAT_INF, a_float_t sum = 0):
+    def __init__(self, a_float_t min = -A_FLOAT_INF, a_float_t max = +A_FLOAT_INF, a_float_t sum = 0):
         self.ctx.pid.summax = sum
         self.ctx.pid.outmax = max
         self.ctx.pid.outmin = min
         a_pid_neuron_init(&self.ctx, 0)
         if sum:
             self.ctx.pid.mode = A_PID_POS
         else:
@@ -26,85 +26,74 @@
     def __call__(self, set: a_float_t, fdb: a_float_t) -> a_float_t:
         '''calculate function for single neuron PID controller'''
         return a_pid_neuron_outf(&self.ctx, set, fdb)
     def zero(self):
         '''zero clear function for single neuron PID controller'''
         a_pid_neuron_zero(&self.ctx)
         return self
-    @property
-    def kp(self) -> a_float_t:
-        return self.ctx.pid.kp
-    @kp.setter
-    def kp(self, kp: a_float_t):
-        self.ctx.pid.kp = kp
-    @property
-    def ki(self) -> a_float_t:
-        return self.ctx.pid.ki
-    @ki.setter
-    def ki(self, ki: a_float_t):
-        self.ctx.pid.ki = ki
-    @property
-    def kd(self) -> a_float_t:
-        return self.ctx.pid.kd
-    @kd.setter
-    def kd(self, kd: a_float_t):
-        self.ctx.pid.kd = kd
-    @property
-    def summax(self) -> a_float_t:
-        return self.ctx.pid.summax
-    @summax.setter
-    def summax(self, summax: a_float_t):
-        self.ctx.pid.summax = summax
-    @property
-    def outmax(self) -> a_float_t:
-        return self.ctx.pid.outmax
-    @outmax.setter
-    def outmax(self, outmax: a_float_t):
-        self.ctx.pid.outmax = outmax
-    @property
-    def outmin(self) -> a_float_t:
-        return self.ctx.pid.outmin
-    @outmin.setter
-    def outmin(self, outmin: a_float_t):
-        self.ctx.pid.outmin = outmin
-    @property
-    def out(self) -> a_float_t:
-        return self.ctx.pid.out.f
-    @property
-    def fdb(self) -> a_float_t:
-        return self.ctx.pid.fdb.f
-    @property
-    def err(self) -> a_float_t:
-        return self.ctx.pid.err.f
-    @property
-    def mode(self) -> int:
-        return self.ctx.pid.mode
-    @mode.setter
-    def mode(self, mode: int):
-        self.ctx.pid.mode = mode
-    @property
-    def ec(self) -> a_float_t:
-        return self.ctx.ec.f
-    @property
-    def wp(self) -> a_float_t:
-        return self.ctx.wp.f
-    @wp.setter
-    def wp(self, wp: a_float_t):
-        self.ctx.wp.f = wp
-    @property
-    def wi(self) -> a_float_t:
-        return self.ctx.wi.f
-    @wi.setter
-    def wi(self, wi: a_float_t):
-        self.ctx.wi.f = wi
-    @property
-    def wd(self) -> a_float_t:
-        return self.ctx.wd.f
-    @wd.setter
-    def wd(self, wd: a_float_t):
-        self.ctx.wd.f = wd
-    @property
-    def k(self) -> a_float_t:
-        return self.ctx.k
-    @k.setter
-    def k(self, k: a_float_t):
-        self.ctx.k = k
+    property kp:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.kp
+        def __set__(self, kp: a_float_t):
+            self.ctx.pid.kp = kp
+    property ki:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.ki
+        def __set__(self, ki: a_float_t):
+            self.ctx.pid.ki = ki
+    property kd:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.kd
+        def __set__(self, kd: a_float_t):
+            self.ctx.pid.kd = kd
+    property summax:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.summax
+        def __set__(self, summax: a_float_t):
+            self.ctx.pid.summax = summax
+    property outmax:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.outmax
+        def __set__(self, outmax: a_float_t):
+            self.ctx.pid.outmax = outmax
+    property outmin:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.outmin
+        def __set__(self, outmin: a_float_t):
+            self.ctx.pid.outmin = outmin
+    property out:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.out.f
+    property fdb:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.fdb.f
+    property err:
+        def __get__(self) -> a_float_t:
+            return self.ctx.pid.err.f
+    property mode:
+        def __get__(self) -> int:
+            return self.ctx.pid.mode
+        def __set__(self, mode: int):
+            self.ctx.pid.mode = mode
+    property ec:
+        def __get__(self) -> a_float_t:
+            return self.ctx.ec.f
+    property wp:
+        def __get__(self) -> a_float_t:
+            return self.ctx.wp.f
+        def __set__(self, wp: a_float_t):
+            self.ctx.wp.f = wp
+    property wi:
+        def __get__(self) -> a_float_t:
+            return self.ctx.wi.f
+        def __set__(self, wi: a_float_t):
+            self.ctx.wi.f = wi
+    property wd:
+        def __get__(self) -> a_float_t:
+            return self.ctx.wd.f
+        def __set__(self, wd: a_float_t):
+            self.ctx.wd.f = wd
+    property k:
+        def __get__(self) -> a_float_t:
+            return self.ctx.k
+        def __set__(self, k: a_float_t):
+            self.ctx.k = k
```

### Comparing `liba-0.1.1rc7/python/src/a/pid.pxd` & `liba-0.1.1rc8/python/src/a/pid.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/python/src/a/poly.pxi` & `liba-0.1.1rc8/python/src/a/poly.pxi`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from a.poly cimport *
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 def poly_eval(x, *a):
-    d, n = floats(a), len(a)
-    cdef a_float_t *p = <a_float_t *>d.data.as_voidptr
+    cdef array y
+    cdef array f = float.array(a)
+    cdef a_float_t *p = <a_float_t *>f.data.as_voidptr
     if iterable(x):
-        y = floats(x)
-        a_poly_evaln(p, n, <a_float_t *>y.data.as_voidptr, len(x), <a_float_t *>y.data.as_voidptr)
+        y = float.array(x)
+        a_poly_evaln(p, len(a), <a_float_t *>y.data.as_voidptr, len(x), <a_float_t *>y.data.as_voidptr)
         return y
-    return a_poly_eval(p, n, x)
+    return a_poly_eval(p, len(a), x)
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 def poly_evar(x, *a):
-    d, n = floats(a), len(a)
-    cdef a_float_t *p = <a_float_t *>d.data.as_voidptr
+    cdef array y
+    cdef array f = float.array(a)
+    cdef a_float_t *p = <a_float_t *>f.data.as_voidptr
     if iterable(x):
-        y = floats(x)
-        a_poly_evarn(p, n, <a_float_t *>y.data.as_voidptr, len(x), <a_float_t *>y.data.as_voidptr)
+        y = float.array(x)
+        a_poly_evarn(p, len(a), <a_float_t *>y.data.as_voidptr, len(x), <a_float_t *>y.data.as_voidptr)
         return y
-    return a_poly_evar(p, n, x)
+    return a_poly_evar(p, len(a), x)
```

### Comparing `liba-0.1.1rc7/python/src/a/polytrack.pxd` & `liba-0.1.1rc8/python/src/a/polytrack.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/python/src/a/polytrack.pxi` & `liba-0.1.1rc8/python/src/a/polytrack.pxi`

 * *Files 12% similar despite different names*

```diff
@@ -1,170 +1,170 @@
 from a.polytrack cimport *
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 cdef class polytrack3:
     '''cubic polynomial trajectory'''
     cdef a_polytrack3_s ctx
-    def __cinit__(self, a_float_t t0, a_float_t t1, a_float_t q0, a_float_t q1, a_float_t v0 = 0, a_float_t v1 = 0):
+    def __init__(self, a_float_t t0, a_float_t t1, a_float_t q0, a_float_t q1, a_float_t v0 = 0, a_float_t v1 = 0):
         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
     def gen(self, a_float_t t0, a_float_t t1, a_float_t q0, a_float_t q1, a_float_t v0 = 0, a_float_t v1 = 0):
         '''generation function'''
         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
     def __call__(self, dt):
         '''calculate all'''
         cdef a_float_t out[3]
         if iterable(dt):
-            p = floats(dt)
-            v = floats(dt)
-            a = floats(dt)
+            p = float.array(dt)
+            v = float.array(dt)
+            a = float.array(dt)
             for i, it in enumerate(dt):
                 a_polytrack3_out(&self.ctx, it, out)
                 p[i] = out[0]
                 v[i] = out[1]
                 a[i] = out[2]
             return p, v, a
         a_polytrack3_out(&self.ctx, dt, out)
         return out[0], out[1], out[2]
     def pos(self, dt):
         '''calculate position'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack3_pos(&self.ctx, it)
             return out
         return a_polytrack3_pos(&self.ctx, dt)
     def vel(self, dt):
         '''calculate velocity'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack3_vel(&self.ctx, it)
             return out
         return a_polytrack3_vel(&self.ctx, dt)
     def acc(self, dt):
         '''calculate acceleration'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack3_acc(&self.ctx, it)
             return out
         return a_polytrack3_acc(&self.ctx, dt)
-    @property
-    def k(self):
-        return self.ctx.k
+    property k:
+        def __get__(self):
+            return self.ctx.k
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 cdef class polytrack5:
     '''quintic polynomial trajectory'''
     cdef a_polytrack5_s ctx
-    def __cinit__(self, a_float_t t0, a_float_t t1, a_float_t q0, a_float_t q1, a_float_t v0 = 0, a_float_t v1 = 0, a_float_t a0 = 0, a_float_t a1 = 0):
+    def __init__(self, a_float_t t0, a_float_t t1, a_float_t q0, a_float_t q1, a_float_t v0 = 0, a_float_t v1 = 0, a_float_t a0 = 0, a_float_t a1 = 0):
         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
     def gen(self, a_float_t t0, a_float_t t1, a_float_t q0, a_float_t q1, a_float_t v0 = 0, a_float_t v1 = 0, a_float_t a0 = 0, a_float_t a1 = 0):
         '''generation function'''
         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
     def __call__(self, dt):
         '''calculate all'''
         cdef a_float_t out[3]
         if iterable(dt):
-            p = floats(dt)
-            v = floats(dt)
-            a = floats(dt)
+            p = float.array(dt)
+            v = float.array(dt)
+            a = float.array(dt)
             for i, it in enumerate(dt):
                 a_polytrack5_out(&self.ctx, it, out)
                 p[i] = out[0]
                 v[i] = out[1]
                 a[i] = out[2]
             return p, v, a
         a_polytrack5_out(&self.ctx, dt, out)
         return out[0], out[1], out[2]
     def pos(self, dt):
         '''calculate position'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack5_pos(&self.ctx, it)
             return out
         return a_polytrack5_pos(&self.ctx, dt)
     def vel(self, dt):
         '''calculate velocity'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack5_vel(&self.ctx, it)
             return out
         return a_polytrack5_vel(&self.ctx, dt)
     def acc(self, dt):
         '''calculate acceleration'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack5_acc(&self.ctx, it)
             return out
         return a_polytrack5_acc(&self.ctx, dt)
-    @property
-    def k(self):
-        return self.ctx.k
+    property k:
+        def __get__(self):
+            return self.ctx.k
 
 @cython.wraparound(False)
 @cython.boundscheck(False)
 cdef class polytrack7:
     '''hepta polynomial trajectory'''
     cdef a_polytrack7_s ctx
-    def __cinit__(self, a_float_t t0, a_float_t t1, a_float_t q0, a_float_t q1, a_float_t v0 = 0, a_float_t v1 = 0, a_float_t a0 = 0, a_float_t a1 = 0, a_float_t j0 = 0, a_float_t j1 = 0):
+    def __init__(self, a_float_t t0, a_float_t t1, a_float_t q0, a_float_t q1, a_float_t v0 = 0, a_float_t v1 = 0, a_float_t a0 = 0, a_float_t a1 = 0, a_float_t j0 = 0, a_float_t j1 = 0):
         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
     def gen(self, a_float_t t0, a_float_t t1, a_float_t q0, a_float_t q1, a_float_t v0 = 0, a_float_t v1 = 0, a_float_t a0 = 0, a_float_t a1 = 0, a_float_t j0 = 0, a_float_t j1 = 0):
         '''generation function'''
         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
     def __call__(self, dt):
         '''calculate all'''
         cdef a_float_t out[4]
         if iterable(dt):
-            p = floats(dt)
-            v = floats(dt)
-            a = floats(dt)
-            j = floats(dt)
+            p = float.array(dt)
+            v = float.array(dt)
+            a = float.array(dt)
+            j = float.array(dt)
             for i, it in enumerate(dt):
                 a_polytrack7_out(&self.ctx, it, out)
                 p[i] = out[0]
                 v[i] = out[1]
                 a[i] = out[2]
                 j[i] = out[3]
             return p, v, a, j
         a_polytrack7_out(&self.ctx, dt, out)
         return out[0], out[1], out[2], out[3]
     def pos(self, dt):
         '''calculate position'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack7_pos(&self.ctx, it)
             return out
         return a_polytrack7_pos(&self.ctx, dt)
     def vel(self, dt):
         '''calculate velocity'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack7_vel(&self.ctx, it)
             return out
         return a_polytrack7_vel(&self.ctx, dt)
     def acc(self, dt):
         '''calculate acceleration'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack7_acc(&self.ctx, it)
             return out
         return a_polytrack7_acc(&self.ctx, dt)
     def jer(self, dt):
         '''calculate jerk'''
         if iterable(dt):
-            out = floats(dt)
+            out = float.array(dt)
             for i, it in enumerate(dt):
                 out[i] = a_polytrack7_jer(&self.ctx, it)
             return out
         return a_polytrack7_jer(&self.ctx, dt)
-    @property
-    def k(self):
-        return self.ctx.k
+    property k:
+        def __get__(self):
+            return self.ctx.k
```

### Comparing `liba-0.1.1rc7/python/src/a/tf.pxd` & `liba-0.1.1rc8/python/src/a/tf.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/python/src/a/tf.pxi` & `liba-0.1.1rc8/python/src/a/tf.pxi`

 * *Files 26% similar despite different names*

```diff
@@ -9,35 +9,33 @@
         '''calculate function for transfer function'''
         return a_tf_iter(&self.ctx, x)
     def zero(self):
         '''zero clear function for transfer function'''
         a_tf_zero(&self.ctx)
         return self
     cdef array input
-    @property
-    def input(self):
-        return self.input
+    property input:
+        def __get__(self):
+            return self.input
     cdef array _num
-    @property
-    def num(self):
-        return self._num
-    @num.setter
-    def num(self, num):
-        self._num = floats(num)
-        self.input = floats(num)
-        a_tf_set_num(&self.ctx, <unsigned int>len(num), <a_float_t *>self._num.data.as_voidptr, <a_float_t *>self.input.data.as_voidptr)
+    property num:
+        def __get__(self):
+            return self._num
+        def __set__(self, num):
+            self._num = float.array(num)
+            self.input = float.array(num)
+            a_tf_set_num(&self.ctx, <unsigned int>len(num), <a_float_t *>self._num.data.as_voidptr, <a_float_t *>self.input.data.as_voidptr)
     cdef array output
-    @property
-    def output(self):
-        return self.output
+    property output:
+        def __get__(self):
+            return self.output
     cdef array _den
-    @property
-    def den(self):
-        return self._den
-    @den.setter
-    def den(self, den):
-        self._den = floats(den)
-        self.output = floats(den)
-        a_tf_set_den(&self.ctx, <unsigned int>len(den), <a_float_t *>self._den.data.as_voidptr, <a_float_t *>self.output.data.as_voidptr)
-    def __cinit__(self, num, den):
-        self.num = num
-        self.den = den
+    property den:
+        def __get__(self):
+            return self._den
+        def __set__(self, den):
+            self._den = float.array(den)
+            self.output = float.array(den)
+            a_tf_set_den(&self.ctx, <unsigned int>len(den), <a_float_t *>self._den.data.as_voidptr, <a_float_t *>self.output.data.as_voidptr)
+    def __init__(self, num, den):
+        tf.num.__set__(self, num)
+        tf.den.__set__(self, den)
```

### Comparing `liba-0.1.1rc7/python/src/a/version.pxi` & `liba-0.1.1rc8/python/src/a/version.pxi`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/setup.cfg` & `liba-0.1.1rc8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = liba
-version = 0.1.1-rc7
+version = 0.1.1-rc8
 url = https://github.com/tqfx/liba.git
 author = tqfx
 author_email = tqfx@foxmail.com
 classifiers = 
 	Programming Language :: C
 	Programming Language :: C++
 	Programming Language :: Cython
```

### Comparing `liba-0.1.1rc7/setup.py` & `liba-0.1.1rc8/setup.py`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/a.c` & `liba-0.1.1rc8/src/a.c`

 * *Files 6% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     }
     return val;
 }
 
 void a_float_save(a_float_t *const array_p, a_size_t const array_n,
                   a_float_t const *const cache_p, a_size_t const cache_n)
 {
-    a_size_t const n = cache_n < array_n ? cache_n : array_n;
+    a_size_t const n = A_MIN(cache_n, array_n);
     for (a_size_t i = array_n, j = array_n - n; j;)
     {
         array_p[--i] = array_p[--j];
     }
     for (a_size_t i = 0; i != n; ++i)
     {
         array_p[i] = cache_p[i];
```

### Comparing `liba-0.1.1rc7/src/avl.c` & `liba-0.1.1rc8/src/avl.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/buf.c` & `liba-0.1.1rc8/src/buf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/complex.c` & `liba-0.1.1rc8/src/complex.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/complex.h` & `liba-0.1.1rc8/src/complex.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/crc.c` & `liba-0.1.1rc8/src/crc.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/fuzzy.c` & `liba-0.1.1rc8/src/fuzzy.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/host/a.c` & `liba-0.1.1rc8/src/host/a.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/host/que.c` & `liba-0.1.1rc8/src/host/que.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/host/str.c` & `liba-0.1.1rc8/src/host/str.c`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     ctx->_mem = 0;
 }
 
 int a_str_init(a_str_s *const ctx, void const *const pdata, a_size_t const nbyte)
 {
     ctx->_num = nbyte;
     ctx->_mem = nbyte + 1;
-    ctx->_mem = a_align(sizeof(void *), ctx->_mem);
+    ctx->_mem = a_size_up(sizeof(void *), ctx->_mem);
     ctx->_ptr = (char *)a_alloc(A_NULL, ctx->_mem);
     if (a_unlikely(ctx->_ptr == A_NULL))
     {
         return A_FAILURE;
     }
     if (pdata && nbyte)
     {
@@ -86,16 +86,15 @@
 }
 
 int a_str_cmp(a_str_s const *const lhs, a_str_s const *const rhs)
 {
     int ok = 0;
     if (lhs->_ptr && rhs->_ptr)
     {
-        a_size_t const num = lhs->_num < rhs->_num ? lhs->_num : rhs->_num;
-        ok = memcmp(lhs->_ptr, rhs->_ptr, num);
+        ok = memcmp(lhs->_ptr, rhs->_ptr, A_MIN(lhs->_num, rhs->_num));
     }
     if (ok)
     {
         return ok;
     }
     if (lhs->_num == rhs->_num)
     {
@@ -103,15 +102,15 @@
     }
     return lhs->_num < rhs->_num ? -1 : +1;
 }
 
 int a_str_alloc_(a_str_s *const ctx, a_size_t mem)
 {
     char *str;
-    mem = a_align(sizeof(void *), mem);
+    mem = a_size_up(sizeof(void *), mem);
     str = (char *)a_alloc(ctx->_ptr, mem);
     if (a_unlikely(!str && mem))
     {
         return A_FAILURE;
     }
     ctx->_ptr = str;
     ctx->_mem = mem;
```

### Comparing `liba-0.1.1rc7/src/host/vec.c` & `liba-0.1.1rc8/src/host/vec.c`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     if (ctx->_mem <= num)
     {
         a_size_t mem = ctx->_mem;
         do
         {
             mem += (mem >> 1) + 1;
         } while (mem < num);
-        a_size_t const siz = a_align(sizeof(void *), ctx->_siz * mem);
+        a_size_t const siz = a_size_up(sizeof(void *), ctx->_siz * mem);
         void *ptr = a_alloc(ctx->_ptr, siz);
         if (a_unlikely(ptr == A_NULL))
         {
             return A_FAILURE;
         }
         ctx->_mem = mem;
         ctx->_ptr = ptr;
```

### Comparing `liba-0.1.1rc7/src/host/vector.c` & `liba-0.1.1rc8/src/host/vector.c`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         a_size_t mem = ctx->_mem;
         do
         {
             mem += (mem >> 1) + 1;
         } while (mem < num);
         a_size_t const mem_ = mem * ctx->_siz;
         a_size_t const num_ = ctx->_num * ctx->_siz;
-        a_size_t const size = a_align(sizeof(void *), mem_);
+        a_size_t const size = a_size_up(sizeof(void *), mem_);
         void *const head = a_alloc(ctx->_head, size);
         if (a_unlikely(head == A_NULL))
         {
             return A_FAILURE;
         }
         ctx->_mem = mem;
         ctx->_head = head;
```

### Comparing `liba-0.1.1rc7/src/math.c` & `liba-0.1.1rc8/src/math.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/mf.c` & `liba-0.1.1rc8/src/mf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/pid/fuzzy.c` & `liba-0.1.1rc8/src/pid/fuzzy.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #define LIBA_PID_FUZZY_C
 #include "fuzzy.h"
+#include "a/math.h"
 
 a_float_t a_pid_fuzzy_op_or(a_float_t const l, a_float_t const r) { return l + r - l * r; }
 
 a_float_t a_pid_fuzzy_op_and(a_float_t const l, a_float_t const r) { return l * r; }
 
 a_float_t a_pid_fuzzy_op_equ(a_float_t const l, a_float_t const r)
 {
```

### Comparing `liba-0.1.1rc7/src/pid/fuzzy.h` & `liba-0.1.1rc8/src/pid/fuzzy.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/pid/neuron.c` & `liba-0.1.1rc8/src/pid/neuron.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/pid/neuron.h` & `liba-0.1.1rc8/src/pid/neuron.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/pid.c` & `liba-0.1.1rc8/src/pid.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/pid.h` & `liba-0.1.1rc8/src/pid.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #ifndef PID_H
 #define PID_H
 
 #include "a/pid.h"
-#include "a/math.h"
 
 #define A_PID_CHAN(ctx)     \
     do                      \
     {                       \
         (ctx)->out.p = out; \
         (ctx)->fdb.p = fdb; \
         (ctx)->tmp.p = tmp; \
```

### Comparing `liba-0.1.1rc7/src/poly.c` & `liba-0.1.1rc8/src/poly.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "a/poly.h"
 
-a_float_t *a_poly_inv(a_float_t *const a, a_size_t const n)
+a_float_t *a_poly_swap(a_float_t *const a, a_size_t const n)
 {
     for (a_float_t t[1], *l = a, *r = a + n - 1, *m = a + (n >> 1); l < m; ++l, --r)
     {
         *t = *l;
         *l = *r;
         *r = *t;
     }
```

### Comparing `liba-0.1.1rc7/src/polytrack.c` & `liba-0.1.1rc8/src/polytrack.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/rbf.c` & `liba-0.1.1rc8/src/rbf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/rbt.c` & `liba-0.1.1rc8/src/rbt.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/tf.c` & `liba-0.1.1rc8/src/tf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/utf.c` & `liba-0.1.1rc8/src/utf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc7/src/version.c` & `liba-0.1.1rc8/src/version.c`

 * *Files identical despite different names*

