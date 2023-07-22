# Comparing `tmp/jfricas-1.0.0.tar.gz` & `tmp/jfricas-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jfricas-1.0.0.tar", last modified: Tue Jul 21 23:41:41 2020, max compression
+gzip compressed data, was "jfricas-2.0.0.tar", last modified: Sat Jul 22 13:38:11 2023, max compression
```

## Comparing `jfricas-1.0.0.tar` & `jfricas-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 hemmecke  (1000) hemmecke  (1000)        0 2020-07-21 23:41:41.000000 jfricas-1.0.0/
--rw-------   0 hemmecke  (1000) hemmecke  (1000)     1316 2020-07-21 23:41:41.000000 jfricas-1.0.0/PKG-INFO
-drwx------   0 hemmecke  (1000) hemmecke  (1000)        0 2020-07-21 23:41:41.000000 jfricas-1.0.0/jfricas.egg-info/
--rw-------   0 hemmecke  (1000) hemmecke  (1000)     1316 2020-07-21 23:41:40.000000 jfricas-1.0.0/jfricas.egg-info/PKG-INFO
--rw-------   0 hemmecke  (1000) hemmecke  (1000)        1 2020-07-21 23:41:40.000000 jfricas-1.0.0/jfricas.egg-info/dependency_links.txt
--rw-------   0 hemmecke  (1000) hemmecke  (1000)        1 2020-07-21 20:13:22.000000 jfricas-1.0.0/jfricas.egg-info/not-zip-safe
--rw-------   0 hemmecke  (1000) hemmecke  (1000)      288 2020-07-21 23:41:41.000000 jfricas-1.0.0/jfricas.egg-info/SOURCES.txt
--rw-------   0 hemmecke  (1000) hemmecke  (1000)        8 2020-07-21 23:41:40.000000 jfricas-1.0.0/jfricas.egg-info/top_level.txt
--rw-------   0 hemmecke  (1000) hemmecke  (1000)       17 2020-07-21 23:41:40.000000 jfricas-1.0.0/jfricas.egg-info/requires.txt
--rw-------   0 hemmecke  (1000) hemmecke  (1000)       64 2020-07-21 17:43:00.000000 jfricas-1.0.0/MANIFEST.in
-drwx------   0 hemmecke  (1000) hemmecke  (1000)        0 2020-07-21 23:41:41.000000 jfricas-1.0.0/jfricas/
--rw-------   0 hemmecke  (1000) hemmecke  (1000)     9664 2020-07-21 23:16:42.000000 jfricas-1.0.0/jfricas/webspad.lisp
--rw-------   0 hemmecke  (1000) hemmecke  (1000)        0 2020-07-21 20:22:50.000000 jfricas-1.0.0/jfricas/__init__.py
--rw-------   0 hemmecke  (1000) hemmecke  (1000)    20245 2020-07-21 23:41:06.000000 jfricas-1.0.0/jfricas/fricaskernel.py
--rw-------   0 hemmecke  (1000) hemmecke  (1000)     2094 2020-07-21 23:41:06.000000 jfricas-1.0.0/setup.py
--rw-------   0 hemmecke  (1000) hemmecke  (1000)     1516 2020-06-16 22:07:01.000000 jfricas-1.0.0/LICENSE
--rw-------   0 hemmecke  (1000) hemmecke  (1000)      538 2020-07-21 23:41:06.000000 jfricas-1.0.0/README.rst
--rw-------   0 hemmecke  (1000) hemmecke  (1000)       38 2020-07-21 23:41:41.000000 jfricas-1.0.0/setup.cfg
+drwx------   0 hemmecke  (1000) hemmecke  (1000)        0 2023-07-22 13:38:11.755011 jfricas-2.0.0/
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)     1516 2023-07-17 20:52:00.000000 jfricas-2.0.0/LICENSE
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)       64 2020-07-21 17:43:00.000000 jfricas-2.0.0/MANIFEST.in
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)     1123 2023-07-22 13:38:11.755011 jfricas-2.0.0/PKG-INFO
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)      538 2023-07-17 20:31:24.000000 jfricas-2.0.0/README.rst
+drwx------   0 hemmecke  (1000) hemmecke  (1000)        0 2023-07-22 13:38:11.751010 jfricas-2.0.0/jfricas/
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)        0 2021-04-17 15:48:16.000000 jfricas-2.0.0/jfricas/__init__.py
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)    20246 2023-07-17 20:00:36.000000 jfricas-2.0.0/jfricas/fricaskernel.py
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)     8649 2023-06-29 21:56:05.000000 jfricas-2.0.0/jfricas/webspad.lisp
+drwx------   0 hemmecke  (1000) hemmecke  (1000)        0 2023-07-22 13:38:11.751010 jfricas-2.0.0/jfricas.egg-info/
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)     1123 2023-07-22 13:38:11.000000 jfricas-2.0.0/jfricas.egg-info/PKG-INFO
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)      288 2023-07-22 13:38:11.000000 jfricas-2.0.0/jfricas.egg-info/SOURCES.txt
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)        1 2023-07-22 13:38:11.000000 jfricas-2.0.0/jfricas.egg-info/dependency_links.txt
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)        1 2022-06-20 06:59:30.000000 jfricas-2.0.0/jfricas.egg-info/not-zip-safe
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)       17 2023-07-22 13:38:11.000000 jfricas-2.0.0/jfricas.egg-info/requires.txt
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)        8 2023-07-22 13:38:11.000000 jfricas-2.0.0/jfricas.egg-info/top_level.txt
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)       38 2023-07-22 13:38:11.755011 jfricas-2.0.0/setup.cfg
+-rw-------   0 hemmecke  (1000) hemmecke  (1000)     2094 2023-07-17 20:01:56.000000 jfricas-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jfricas-1.0.0/PKG-INFO` & `jfricas-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: jfricas
-Version: 1.0.0
+Version: 2.0.0
 Summary: FriCAS Jupyter Kernel.
 Home-page: http://github.com/fricas/jfricas
 Author: Kurt Pagani, Ralf Hemmecke
 Author-email: jfricas@hemmecke.org
 License: BSD
-Description: ===============================
-        FriCAS Jupyter Kernel (jfricas)
-        ===============================
-        
-        This project implements a Jupyter kernel for `FriCAS`_ .
-        
-        Documentation: https://jfricas.readthedocs.io
-        
-        Git repository: https://github.com/fricas/jfricas
-        
-        :Authors:
-            Ralf Hemmecke,
-            Kurt Pagani
-        
-            (and sundry other good-natured folks)
-        
-        :Version: 1.0.0 (22-Jul-2020)
-        
-        :License: `Simplified BSD License`_
-        
-        
-        .. _FriCAS: https://github.com/fricas/fricas
-        .. _Simplified BSD License: https://github.com/fricas/jfricas/blob/master/LICENSE
-        
 Keywords: fricas,jupyter,computer_algebra
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+===============================
+FriCAS Jupyter Kernel (jfricas)
+===============================
+
+This project implements a Jupyter kernel for `FriCAS`_ .
+
+Documentation: https://jfricas.readthedocs.io
+
+Git repository: https://github.com/fricas/jfricas
+
+:Authors:
+    Ralf Hemmecke,
+    Kurt Pagani
+
+    (and sundry other good-natured folks)
+
+:Version: 2.0.0 (22-Jul-2023)
+
+:License: `Simplified BSD License`_
+
+
+.. _FriCAS: https://github.com/fricas/fricas
+.. _Simplified BSD License: https://github.com/fricas/jfricas/blob/master/LICENSE
```

### Comparing `jfricas-1.0.0/jfricas.egg-info/PKG-INFO` & `jfricas-2.0.0/jfricas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: jfricas
-Version: 1.0.0
+Version: 2.0.0
 Summary: FriCAS Jupyter Kernel.
 Home-page: http://github.com/fricas/jfricas
 Author: Kurt Pagani, Ralf Hemmecke
 Author-email: jfricas@hemmecke.org
 License: BSD
-Description: ===============================
-        FriCAS Jupyter Kernel (jfricas)
-        ===============================
-        
-        This project implements a Jupyter kernel for `FriCAS`_ .
-        
-        Documentation: https://jfricas.readthedocs.io
-        
-        Git repository: https://github.com/fricas/jfricas
-        
-        :Authors:
-            Ralf Hemmecke,
-            Kurt Pagani
-        
-            (and sundry other good-natured folks)
-        
-        :Version: 1.0.0 (22-Jul-2020)
-        
-        :License: `Simplified BSD License`_
-        
-        
-        .. _FriCAS: https://github.com/fricas/fricas
-        .. _Simplified BSD License: https://github.com/fricas/jfricas/blob/master/LICENSE
-        
 Keywords: fricas,jupyter,computer_algebra
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+===============================
+FriCAS Jupyter Kernel (jfricas)
+===============================
+
+This project implements a Jupyter kernel for `FriCAS`_ .
+
+Documentation: https://jfricas.readthedocs.io
+
+Git repository: https://github.com/fricas/jfricas
+
+:Authors:
+    Ralf Hemmecke,
+    Kurt Pagani
+
+    (and sundry other good-natured folks)
+
+:Version: 2.0.0 (22-Jul-2023)
+
+:License: `Simplified BSD License`_
+
+
+.. _FriCAS: https://github.com/fricas/fricas
+.. _Simplified BSD License: https://github.com/fricas/jfricas/blob/master/LICENSE
```

### Comparing `jfricas-1.0.0/jfricas/webspad.lisp` & `jfricas-2.0.0/jfricas/webspad.lisp`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 ;;; (a) makes a webserver (Hunchentoot) available,
 ;;; (b) extends/modifies some FriCAS (package "BOOT") behavior,
 ;;; (c) provides functions (package "webspad") that take a multiline
 ;;;     (FriCAS) code string, send it to FriCAS and catch the
 ;;;     FriCAS output.
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
-;;; Load the Hunchentoot webserver.
-;;; https://edicl.github.io/hunchentoot/
-(require :asdf)
-(require :hunchentoot)
-
-;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;;; BOOT is a Package in FriCAS.
 ;;  This part adds a few functions to the BOOT package of FriCAS
 ;;; to make the FriCAS output contain a number of markers (via the
 ;;; |$ioHook| facility) that make parsing of the output easier.
 ;;; Furthermore, it contains a function, interpret-block, which
 ;;; interprets a (potentially multiline) block of code.
 
@@ -62,16 +56,16 @@
 
 (defun ws-fmt (marker)
   (|sayMSG| (format nil "--FORMAT:~A:~D" marker boot::|$IOindex|)))
 
 (setf |$ioHook|
       (lambda (x &optional args)
         (cond
-;         ((eq x '|startAlgebraOutput|) (ws-fmt "BEG:Algebra"))
-;         ((eq x '|endOfAlgebraOutput|) (ws-fmt "END:Algebra"))
+         ((eq x '|startAlgebraOutput|) (ws-fmt "BEG:Algebra"))
+         ((eq x '|endOfAlgebraOutput|) (ws-fmt "END:Algebra"))
          ((eq x '|startPatternMsg|)    (ws-fmt "BEG:ERROR"))
          ((eq x '|endPatternMsg|)      (ws-fmt "END:ERROR"))
          ((eq x '|startKeyedMsg|)
           (cond
            ((eq (car args) 'S2GL0012) (ws-fmt "BEG:Type"))
            ((eq (car args) 'S2GL0013) (ws-fmt "BEG:Time"))
            ((eq (car args) 'S2GL0014) (ws-fmt "BEG:TypeTime"))
@@ -82,61 +76,36 @@
            ((eq (car args) 'S2GL0012) (ws-fmt "END:Type"))
            ((eq (car args) 'S2GL0013) (ws-fmt "END:Time"))
            ((eq (car args) 'S2GL0014) (ws-fmt "END:TypeTime"))
            ((eq (car args) 'S2GL0016) (ws-fmt "END:Storage"))
            ('T                        (ws-fmt "END:KeyedMsg"))))
         )))
 
-;;; Override a FriCAS function in order to remove the equation number.
-(DEFUN |mathprintWithNumber| (|x|)
-  (PROG ()
-    (RETURN
-     (PROGN
-      ;(|ioHook| '|startAlgebraOutput|)
-      (|saySpadMsg| '|--FORMAT:BEG:Algebra|)
-      (|maprin| (|outputTran2| |x|))
-      (|saySpadMsg| '|--FORMAT:END:Algebra|)
-      ;(|ioHook| '|endOfAlgebraOutput|)
-      ))))
-
-;;; interpret-block takes a code string that is interpreted as if it
-;;; comes from a .input file.
-(DEFUN |interpret-block| (|code|)
-  (PROG (|$ncMsgList| |$erMsgToss| |$lastPos| |$EchoLines| |st|)
-    (DECLARE (SPECIAL |$ncMsgList| |$erMsgToss| |$lastPos| |$EchoLines|))
-    (RETURN
-     (PROGN
-      (SETQ |$EchoLines| NIL)
-      (SETQ |$lastPos| |$nopos|)
-      (SETQ |$erMsgToss| NIL)
-      (SETQ |$ncMsgList| NIL)
-      (SETQ |st| (MAKE-STRING-INPUT-STREAM |code|))
-      (|intloopInclude0| |st| '|webspad| 0)))))
-
 ;;; Following function calls FriCAS for evaluation of code and returns
 ;;; true if ther is an error and nil otherwise.
 (defun |webspad-parseAndEvalStr| (code)
 ;  (setf |$printTypeIfTrue| T)    ; Make sure we get "Type:" line.
 ;  (setf |$printTimeIfTrue| T)    ; Make sure we get "Time:" line.
   (setf |$printStorageIfTrue| T) ; Make sure we get "Storage:" line.
   (setf |$fortranFormat| NIL)    ; we don't want Fortran output
   (setf |$htmlFormat| NIL)       ; we don't want Html output
   (setf |$openMathFormat| NIL)   ; we don't want OpenMath output
   (setf |$MARGIN| 0)             ; we don't want indentation
+  (setf |$print_equatnum| NIL)   ; we don't want indentation
 
   ;;; code might consist of multiple lines (i.e. contain newline
   ;;; characters)
-  (eq (catch 'SPAD_READER (catch '|top_level| (|interpret-block| code)))
+  (eq (catch 'SPAD_READER (catch '|top_level| (|interpret_block| code)))
       '|restart|))
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 
 (defpackage webspad
     (:use common-lisp)
-    (:documentation "see docs"))
+    (:documentation "see source code"))
 
 (in-package :webspad)
 
 ;;; The function webspad-eval is called from the Jupyter notebook via
 ;;; fricaskernel.py and the Hunchentoot webserver. It receives the
 ;;; code of a cell as input. Before this code is sent to FriCAS, all
 ;;; relevant streams that FriCAS writes to are stored and replaced by
@@ -144,14 +113,17 @@
 ;;; the output is fetched and the saved stream are restored.
 
 (defstruct r
   (stdout    "" :type string)
   (error?    "" :type string)
   (input     "" :type string))
 
+;;; One stream that catches all output.
+(defvar webspad-stream (make-string-output-stream))
+
 (defun webspad-eval (input)
   (let* (
         ;;; store original input argument
          (data (make-r :input input))
          ;;; Because we want to read from the fricas streams via
          ;;; get-output-stream-string, we must make sure that the
          ;;; streams are created via make-string-output-stream.
@@ -162,33 +134,32 @@
          (s-formatted (if formattedp boot::|$formattedOutputStream|))
          (s-stdout    boot::*standard-output*)
          (s-stderr    boot::*error-output*)
          (s-algebra   boot::|$algebraOutputStream|)
          (s-tex       boot::|$texOutputStream|)
          (s-mathml    boot::|$mathmlOutputStream|)
          (s-texmacs   boot::|$texmacsOutputStream|)
-         (s           nil))
+         (boot::*OBEY-STDOUT* T)
+         (*standard-output* webspad-stream)
+         (*error-output* *standard-output*)
+         (s           (boot::|mkOutputConsoleStream|))) ; use *standard-output*
 
     ;;; create empty streams
-    (setf boot::*standard-output*        (make-string-output-stream))
-    (setf boot::*error-output*           boot::*standard-output*)
-    (setf s (boot::|mkOutputConsoleStream|))
     (setf boot::|$algebraOutputStream|   s)
     (setf boot::|$texOutputStream|       s)
     (setf boot::|$mathmlOutputStream|    s)
     (setf boot::|$texmacsOutputStream|   s)
     (if formattedp (setf boot::|$formattedOutputStream| s))
 
     ;;; eval and return true if there was an error
     (setf (r-error? data) (if (boot::|webspad-parseAndEvalStr| input) "T" "F"))
 
     (setf (r-stdout data) (get-output-stream-string boot::*standard-output*))
     (if formattedp (setf boot::|$formattedOutputStream| s-formatted))
-    (setf boot::*standard-output*        s-stdout)
-    (setf boot::*error-output*           s-stderr)
+
     (setf boot::|$algebraOutputStream|   s-algebra)
     (setf boot::|$texOutputStream|       s-tex)
     (setf boot::|$mathmlOutputStream|    s-mathml)
     (setf boot::|$texmacsOutputStream|   s-texmacs)
 
     ;;; return the data record
     data))
```

### Comparing `jfricas-1.0.0/jfricas/fricaskernel.py` & `jfricas-2.0.0/jfricas/fricaskernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from ipykernel.kernelbase import Kernel
 from subprocess import Popen, run, PIPE, STDOUT
 import requests
 import json
 import os
 
-__version__ = '1.0.0'
+__version__ = '2.0.0'
 
 ###################################################################
 # BEGIN user configuration options
 ###################################################################
 shell_timeout = 15 # Timeout for shell commands in secs.
 shell_result = None # store last sh result in python
 shell_result_fricas = '__shell_result:=["{0}"]' # store sh result in FriCAS
@@ -169,15 +169,15 @@
         # (a) All whitespace is remove from the end of a line.
         # (b) A line ending in _ (underscore) makes the next line
         #     belonging to the same block.
         # (c) A line starting with a non-whitespace character begins
         #     a new input block.
         # (d) All lines that begin with a space character are associated
         #     with the current block.
-        # Then we handle one block afte the other.
+        # Then we handle one block after the other.
         lines = code.split('\n')
         blocks = []
         block = ""
         for line in lines:
             line = line.rstrip()
             if not block:
                 block = line
```

### Comparing `jfricas-1.0.0/setup.py` & `jfricas-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 kernel_srcdir = 'jfricas/kspec'
 kernel_name = 'jfricas'
-kernel_version = '1.0.0'
+kernel_version = '2.0.0'
 ldescr = readme()
 
 setup(name=kernel_name,
       version=kernel_version,
       description='FriCAS Jupyter Kernel.',
       long_description=ldescr,
       long_description_content_type='text/x-rst',
```

### Comparing `jfricas-1.0.0/LICENSE` & `jfricas-2.0.0/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2019-2020, FriCAS Team.
+Copyright (c) 2019-2023, FriCAS Team.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `jfricas-1.0.0/README.rst` & `jfricas-2.0.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 
 :Authors:
     Ralf Hemmecke,
     Kurt Pagani
 
     (and sundry other good-natured folks)
 
-:Version: 1.0.0 (22-Jul-2020)
+:Version: 2.0.0 (22-Jul-2023)
 
 :License: `Simplified BSD License`_
 
 
 .. _FriCAS: https://github.com/fricas/fricas
 .. _Simplified BSD License: https://github.com/fricas/jfricas/blob/master/LICENSE
```

