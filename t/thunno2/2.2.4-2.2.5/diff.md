# Comparing `tmp/thunno2-2.2.4.tar.gz` & `tmp/thunno2-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.2.4.tar", last modified: Sat Jul 22 09:35:31 2023, max compression
+gzip compressed data, was "thunno2-2.2.5.tar", last modified: Sat Jul 22 10:08:15 2023, max compression
```

## Comparing `thunno2-2.2.4.tar` & `thunno2-2.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:35:31.115307 thunno2-2.2.4/
--rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 09:35:31.115200 thunno2-2.2.4/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-07-22 09:35:31.115340 thunno2-2.2.4/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.4/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:35:31.114532 thunno2-2.2.4/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.4/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.4/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.4/thunno2/canvas.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.4/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    57155 2023-07-02 13:06:12.000000 thunno2-2.2.4/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.4/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.4/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7303 2023-06-03 14:35:27.000000 thunno2-2.2.4/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    58811 2023-07-13 18:38:48.000000 thunno2-2.2.4/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    33317 2023-07-22 09:29:18.000000 thunno2-2.2.4/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    25968 2023-07-22 09:29:18.000000 thunno2-2.2.4/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-07-02 13:16:10.000000 thunno2-2.2.4/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    86420 2023-07-13 18:37:15.000000 thunno2-2.2.4/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4505 2023-06-24 09:12:25.000000 thunno2-2.2.4/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-07-22 09:34:42.000000 thunno2-2.2.4/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:35:31.115059 thunno2-2.2.4/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      459 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       53 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 10:08:15.700202 thunno2-2.2.5/
+-rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 10:08:15.700042 thunno2-2.2.5/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-07-22 10:08:15.700234 thunno2-2.2.5/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.5/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 10:08:15.699338 thunno2-2.2.5/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.5/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.5/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.5/thunno2/canvas.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.5/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    57155 2023-07-02 13:06:12.000000 thunno2-2.2.5/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.5/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.5/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7303 2023-06-03 14:35:27.000000 thunno2-2.2.5/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    58811 2023-07-13 18:38:48.000000 thunno2-2.2.5/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    34295 2023-07-22 09:41:31.000000 thunno2-2.2.5/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    26469 2023-07-22 09:41:31.000000 thunno2-2.2.5/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-07-02 13:16:10.000000 thunno2-2.2.5/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    86420 2023-07-13 18:37:15.000000 thunno2-2.2.5/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4505 2023-06-24 09:12:25.000000 thunno2-2.2.5/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-07-22 10:07:49.000000 thunno2-2.2.5/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 10:08:15.699862 thunno2-2.2.5/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 10:08:15.000000 thunno2-2.2.5/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      459 2023-07-22 10:08:15.000000 thunno2-2.2.5/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-07-22 10:08:15.000000 thunno2-2.2.5/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       53 2023-07-22 10:08:15.000000 thunno2-2.2.5/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-07-22 10:08:15.000000 thunno2-2.2.5/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.2.4/PKG-INFO` & `thunno2-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.4
+Version: 2.2.5
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.4.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.5.tar.gz
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
 Keywords: golfing,code-golf,language
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `thunno2-2.2.4/setup.py` & `thunno2-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/autoexplanation.py` & `thunno2-2.2.5/thunno2/autoexplanation.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/canvas.py` & `thunno2-2.2.5/thunno2/canvas.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/codepage.py` & `thunno2-2.2.5/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/commands.py` & `thunno2-2.2.5/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/constants.py` & `thunno2-2.2.5/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/dictionary.py` & `thunno2-2.2.5/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/flags.py` & `thunno2-2.2.5/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/helpers.py` & `thunno2-2.2.5/thunno2/helpers.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/interpreter.py` & `thunno2-2.2.5/thunno2/interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,15 +154,14 @@
                     ctx.stack.push(value)
         elif desc in (
             "number",
             "string",
             "one character",
             "two characters",
             "three characters",
-            "list",
         ):
             ctx.stack.push(info)
         elif desc == "lowercase alphabetic compression":
             base255_number = decompress(info, "“")
             decompressed_string = to_custom_base_string(
                 " " + string.ascii_lowercase, base255_number
             )
@@ -466,46 +465,58 @@
         elif desc == "print without popping":
             print((ctx.stack.copy() + ctx.other_il + [0])[0])
             ctx.implicit_print = False
         elif desc == "print each":
             for i in listify(next(ctx.stack.rmv(1))):
                 print(i)
             ctx.implicit_print = False
+        elif desc == "list":
+            old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
+            r = []
+            for j in info:
+                ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
+                run(j, context=context, iteration_index=iteration_index)
+                r.append(next(ctx.stack.rmv(1)))
+            ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
+            ctx.stack.push(r)
         elif desc == "map":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
                 run(info, context=j, iteration_index=i)
                 r.append(next(ctx.stack.rmv(1)))
+            ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
             ctx.stack.push(r)
         elif desc == "filter":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
                 run(info, context=j, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 if z:
                     r.append(j)
+            ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
             ctx.stack.push(r)
         elif desc == "sort by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
                 run(info, context=j, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 r.append((j, z))
+            ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
             try:
                 sorted_list = sorted(r, key=lambda t: t[-1])
                 ctx.stack.push([p for p, q in sorted_list])
             except:
                 ctx.stack.push(x)
         elif desc == "group by":
             a = next(ctx.stack.rmv(1))
@@ -513,14 +524,15 @@
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
                 run(info, context=j, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 r.append((j, z))
+            ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
             try:
                 d = []
                 for val, key in r:
                     for k, (i, j) in enumerate(d):
                         if key == i:
                             d[k][1].append(val)
                             break
@@ -537,14 +549,15 @@
                 ctx.stack = Stack(copy.deepcopy(old_stack))
                 run(info, context=r[-1], iteration_index=i)
                 k = (ctx.stack + ctx.other_il + [0])[0]
                 r.append(k)
                 if r[-1] == r[-2]:
                     break
                 i += 1
+            ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
             ctx.stack.push(r[1:])
         elif desc == "first n integers":
             a = next(ctx.stack.rmv(1))
             try:
                 x = int(a)
             except:
                 x = 1
@@ -555,27 +568,29 @@
                 ctx.stack = Stack(copy.deepcopy(old_stack))
                 ctx.stack.push(i)
                 run(info, context=i, iteration_index=i - 1)
                 k = next(ctx.stack.rmv(1))
                 if k:
                     r.append(i)
                 i += 1
+            ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
             ctx.stack.push(r)
         elif desc == "cumulative reduce by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             if x:
                 r = [x.pop(0)]
                 for i, j in enumerate(x):
                     ctx.stack = Stack(copy.deepcopy(old_stack))
                     ctx.stack.push(r[-1])
                     ctx.stack.push(j)
                     run(info, context=j, iteration_index=i)
                     r.append(next(ctx.stack.rmv(1)))
+                ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
                 ctx.stack.push(r)
             else:
                 ctx.stack.push([])
         elif desc == "single function reduce by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
@@ -634,14 +649,15 @@
                 r = [x.pop(0)]
                 for i, j in enumerate(x):
                     ctx.stack = Stack(copy.deepcopy(old_stack))
                     ctx.stack.push(r[-1])
                     ctx.stack.push(j)
                     run(info, context=j, iteration_index=i)
                     r.append(next(ctx.stack.rmv(1)))
+                ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
                 ctx.stack.push(r[-1])
             else:
                 ctx.stack.push([])
         elif desc == "for loop":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             for i, j in enumerate(x):
```

### Comparing `thunno2-2.2.4/thunno2/lexer.py` & `thunno2-2.2.5/thunno2/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,42 +278,55 @@
                 or (x[2] not in dictionary_codepage)
                 or (nxt not in dictionary_codepage)
             ):
                 ret.append(("ʋ" + x, "three characters", x))
             else:
                 index += 1
                 ret.append(("ʋ" + x + nxt, "two words dictionary compression", x + nxt))
+        # elif char == "[":
+        #     s = char
+        #     index += 1
+        #     try:
+        #         in_string = ""
+        #         nests = 1
+        #         while nests:
+        #             c = code[index]
+        #             s += c
+        #             if in_string == "" and c in ('"', "'"):
+        #                 in_string = c
+        #             elif in_string != "" and c == in_string:
+        #                 if code[index - 1] != "\\":
+        #                     in_string = ""
+        #             if in_string == "":
+        #                 if c == "[":
+        #                     nests += 1
+        #                 elif c == "]":
+        #                     nests -= 1
+        #             index += 1
+        #     except:
+        #         s += "]"
+        #     try:
+        #         ret.append((s, "list", eval(s)))
+        #     except:
+        #         ret.append((s, "list", s))
+        # elif char == "]":
+        #     ret.append(("]", "list", []))
         elif char == "[":
-            s = char
-            index += 1
-            try:
-                in_string = ""
-                nests = 1
-                while nests:
-                    c = code[index]
-                    s += c
-                    if in_string == "" and c in ('"', "'"):
-                        in_string = c
-                    elif in_string != "" and c == in_string:
-                        if code[index - 1] != "\\":
-                            in_string = ""
-                    if in_string == "":
-                        if c == "[":
-                            nests += 1
-                        elif c == "]":
-                            nests -= 1
-                    index += 1
-            except:
-                s += "]"
+            r = []
+            i, x = tokenise(code[index + 1 :], expected_end=";]")
+            index += i + 1
+            r.append(x)
             try:
-                ret.append((s, "list", eval(s)))
+                while code[index] == ";":
+                    i, x = tokenise(code[index + 1 :], expected_end=";]")
+                    index += i + 1
+                    r.append(x)
             except:
-                ret.append((s, "list", s))
-        elif char == "]":
-            ret.append(("]", "list", []))
+                pass
+            ret.append((char, "list", r))
         elif char == "#":
             index += 1
             try:
                 if code[index] == " ":
                     while code[index] not in "¶\n":
                         index += 1
                 elif code[index] == "{":
```

### Comparing `thunno2-2.2.4/thunno2/run.py` & `thunno2-2.2.5/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/tests.py` & `thunno2-2.2.5/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2/tokens.py` & `thunno2-2.2.5/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.4/thunno2.egg-info/PKG-INFO` & `thunno2-2.2.5/thunno2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.4
+Version: 2.2.5
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.4.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.5.tar.gz
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
 Keywords: golfing,code-golf,language
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

