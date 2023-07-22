# Comparing `tmp/fidel-0.0.8.tar.gz` & `tmp/fidel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fidel-0.0.8.tar", last modified: Sat Jul 22 15:32:06 2023, max compression
+gzip compressed data, was "fidel-0.0.9.tar", last modified: Sat Jul 22 16:37:44 2023, max compression
```

## Comparing `fidel-0.0.8.tar` & `fidel-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.975965 fidel-0.0.8/
--rw-rw-rw-   0        0        0    35823 2022-12-08 01:49:24.000000 fidel-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5256 2023-07-22 15:32:06.973962 fidel-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4741 2023-07-22 15:11:54.000000 fidel-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-22 15:32:06.975965 fidel-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-07-22 15:30:16.000000 fidel-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.692793 fidel-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.732836 fidel-0.0.8/src/fidel/
--rw-rw-rw-   0        0        0       63 2023-07-21 19:08:53.000000 fidel-0.0.8/src/fidel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.969973 fidel-0.0.8/src/fidel/data/
--rw-rw-rw-   0        0        0   857510 2022-12-15 22:19:26.000000 fidel-0.0.8/src/fidel/data/word_list.txt
--rw-rw-rw-   0        0        0     2746 2023-07-22 14:38:47.000000 fidel-0.0.8/src/fidel/main.py
-drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.967738 fidel-0.0.8/src/fidel.egg-info/
--rw-rw-rw-   0        0        0     5256 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 16:37:44.716838 fidel-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2022-12-08 01:49:24.000000 fidel-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5249 2023-07-22 16:37:44.714843 fidel-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4734 2023-07-22 16:19:47.000000 fidel-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-22 16:37:44.716838 fidel-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-07-22 16:34:51.000000 fidel-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 16:37:44.035537 fidel-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 16:37:44.272001 fidel-0.0.9/src/fidel/
+-rw-rw-rw-   0        0        0        0 2023-07-22 14:39:48.000000 fidel-0.0.9/src/fidel/README.md
+-rw-rw-rw-   0        0        0       63 2023-07-21 19:08:53.000000 fidel-0.0.9/src/fidel/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-07-22 16:28:27.000000 fidel-0.0.9/src/fidel/a.py
+drwxrwxrwx   0        0        0        0 2023-07-22 16:37:44.357088 fidel-0.0.9/src/fidel/data/
+-rw-rw-rw-   0        0        0   857510 2022-12-15 22:19:26.000000 fidel-0.0.9/src/fidel/data/word_list.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 16:37:44.438719 fidel-0.0.9/src/fidel/helpers/
+drwxrwxrwx   0        0        0        0 2023-07-22 16:37:44.466806 fidel-0.0.9/src/fidel/helpers/__pycache__/
+-rw-rw-rw-   0        0        0     1524 2023-07-22 14:24:06.000000 fidel-0.0.9/src/fidel/helpers/__pycache__/filter.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1181 2023-07-22 13:10:47.000000 fidel-0.0.9/src/fidel/helpers/filter.py
+-rw-rw-rw-   0        0        0     2752 2023-07-22 16:27:53.000000 fidel-0.0.9/src/fidel/main.py
+drwxrwxrwx   0        0        0        0 2023-07-22 16:37:44.542974 fidel-0.0.9/src/fidel/utilities/
+drwxrwxrwx   0        0        0        0 2023-07-22 16:37:44.657994 fidel-0.0.9/src/fidel/utilities/__pycache__/
+-rw-rw-rw-   0        0        0     2310 2023-07-22 12:19:26.000000 fidel-0.0.9/src/fidel/utilities/__pycache__/dictionary.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1950 2023-07-22 14:24:06.000000 fidel-0.0.9/src/fidel/utilities/__pycache__/word.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3092 2023-07-22 12:16:52.000000 fidel-0.0.9/src/fidel/utilities/dictionary.py
+-rw-rw-rw-   0        0        0     3667 2023-07-22 14:31:31.000000 fidel-0.0.9/src/fidel/utilities/word.py
+drwxrwxrwx   0        0        0        0 2023-07-22 16:37:44.342806 fidel-0.0.9/src/fidel.egg-info/
+-rw-rw-rw-   0        0        0     5249 2023-07-22 16:37:43.000000 fidel-0.0.9/src/fidel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-07-22 16:37:44.000000 fidel-0.0.9/src/fidel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 16:37:43.000000 fidel-0.0.9/src/fidel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-22 16:37:43.000000 fidel-0.0.9/src/fidel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-22 16:37:43.000000 fidel-0.0.9/src/fidel.egg-info/top_level.txt
```

### Comparing `fidel-0.0.8/LICENSE` & `fidel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fidel-0.0.8/PKG-INFO` & `fidel-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: fidel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package that can change Amharic language that written in English alphabet to Amharic alphabet character.
 Author: Niftalem Yeneneh
 Author-email: ny.dev0.em@gmail.com
 Keywords: python,amharic,english to amharic,ethiopia,translate,fidel
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # **Fidel / ፊደል**
 ## What is **Fidel / ፊደል** ?
 **Fidel** is a python package that can change Amharic language that written in English alphabet to Amharic alphabet character. <br>
 **| For example: abebe beso bela -> አበበ በሶ በላ**
-#
+
 
 ## **Dependencies**
 * [Symspellpy](https://github.com/mammothb/symspellpy)
-#
+
 
 ## **Installation** 
 ```
 pip install fidel
 ```
 ## **Upgrade**
 ```
 pip install --upgrade fidel
 ```
 #
 
-
 ## **Usage**
 
 ### **Basic Usage**
 ``` python
 from fidel import Translate
 text = "bexam xru sew new"
 translated = Translate(text).translate()
@@ -107,15 +106,15 @@
 reversed = Reverse(text, symbol=True) # The default symbol value is True 
 print(reversed)
 ```
 output
 ```
 betam xru sew nw.
 ```
-#
+
 
 ## **Rules** 
 There are some **rules** that should be apply when writing the text.
  1. For **1st alphabets (ለግዕዝ)** use "e" example: "le" - ለ
  2. For **2nd alphabets (ለካእብ)** use "u" example: "lu" - ሉ
  3. For **3rd alphabets (ለሳልስ)** use "i" example: "li" - ሊ
  4. For **4rh alphabets (ለራዕብ)** use "a" example: "la" - ላ
@@ -145,8 +144,8 @@
 |  phe  |  phu  |  phi  |  pha  |  phie   |  ph  |  pho  |
 |  **ፐ**  |  **ፑ**  |  **ፒ**  |  **ፓ**  |  **ፔ**   |  **ፕ**  |  **ፖ**  |
 |  pe  |  pu |  pi  |  pa  |  pie   |  p  |  po  |
 
 **Addition** <br>
 |Alphabets |ሸ| ኘ| ዥ| ጸ| 
 |-----|-----|-----|-----|------|
-|Prefix |sh |gn |zh| ts|
+|Prefix |sh |gn |zh| ts|
```

### Comparing `fidel-0.0.8/README.md` & `fidel-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # **Fidel / ፊደል**
 ## What is **Fidel / ፊደል** ?
 **Fidel** is a python package that can change Amharic language that written in English alphabet to Amharic alphabet character. <br>
 **| For example: abebe beso bela -> አበበ በሶ በላ**
-#
+
 
 ## **Dependencies**
 * [Symspellpy](https://github.com/mammothb/symspellpy)
-#
+
 
 ## **Installation** 
 ```
 pip install fidel
 ```
 ## **Upgrade**
 ```
 pip install --upgrade fidel
 ```
 #
 
-
 ## **Usage**
 
 ### **Basic Usage**
 ``` python
 from fidel import Translate
 text = "bexam xru sew new"
 translated = Translate(text).translate()
@@ -96,15 +95,15 @@
 reversed = Reverse(text, symbol=True) # The default symbol value is True 
 print(reversed)
 ```
 output
 ```
 betam xru sew nw.
 ```
-#
+
 
 ## **Rules** 
 There are some **rules** that should be apply when writing the text.
  1. For **1st alphabets (ለግዕዝ)** use "e" example: "le" - ለ
  2. For **2nd alphabets (ለካእብ)** use "u" example: "lu" - ሉ
  3. For **3rd alphabets (ለሳልስ)** use "i" example: "li" - ሊ
  4. For **4rh alphabets (ለራዕብ)** use "a" example: "la" - ላ
@@ -134,8 +133,8 @@
 |  phe  |  phu  |  phi  |  pha  |  phie   |  ph  |  pho  |
 |  **ፐ**  |  **ፑ**  |  **ፒ**  |  **ፓ**  |  **ፔ**   |  **ፕ**  |  **ፖ**  |
 |  pe  |  pu |  pi  |  pa  |  pie   |  p  |  po  |
 
 **Addition** <br>
 |Alphabets |ሸ| ኘ| ዥ| ጸ| 
 |-----|-----|-----|-----|------|
-|Prefix |sh |gn |zh| ts|
+|Prefix |sh |gn |zh| ts|
```

### Comparing `fidel-0.0.8/setup.py` & `fidel-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Python package that can change Amharic language that written in English alphabet to Amharic alphabet character.'
 
 setup(
     name="fidel",
     version=VERSION,
     author="Niftalem Yeneneh",
     author_email="ny.dev0.em@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=['fidel'],
     package_dir={'': 'src'},
-    package_data={'': ['data/*.txt']},
+    package_data={'': ['**']},
     install_requires=["symspellpy == 6.7.1" ],
     keywords=['python', 'amharic', 'english to amharic', 'ethiopia', 'translate', 'fidel']
 )
```

### Comparing `fidel-0.0.8/src/fidel/data/word_list.txt` & `fidel-0.0.9/src/fidel/data/word_list.txt`

 * *Files identical despite different names*

### Comparing `fidel-0.0.8/src/fidel/main.py` & `fidel-0.0.9/src/fidel/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fidel.utilities.word import sep_words
+from fidel.utilities.dictionary import sep_words
 from symspellpy import SymSpell, Verbosity
 from fidel.utilities.dictionary import dict
 from fidel.helpers.filter import filter_symbol
 import os
 
 PROJECT_DIR = os.path.dirname(__file__)
```

### Comparing `fidel-0.0.8/src/fidel.egg-info/PKG-INFO` & `fidel-0.0.9/src/fidel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: fidel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package that can change Amharic language that written in English alphabet to Amharic alphabet character.
 Author: Niftalem Yeneneh
 Author-email: ny.dev0.em@gmail.com
 Keywords: python,amharic,english to amharic,ethiopia,translate,fidel
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # **Fidel / ፊደል**
 ## What is **Fidel / ፊደል** ?
 **Fidel** is a python package that can change Amharic language that written in English alphabet to Amharic alphabet character. <br>
 **| For example: abebe beso bela -> አበበ በሶ በላ**
-#
+
 
 ## **Dependencies**
 * [Symspellpy](https://github.com/mammothb/symspellpy)
-#
+
 
 ## **Installation** 
 ```
 pip install fidel
 ```
 ## **Upgrade**
 ```
 pip install --upgrade fidel
 ```
 #
 
-
 ## **Usage**
 
 ### **Basic Usage**
 ``` python
 from fidel import Translate
 text = "bexam xru sew new"
 translated = Translate(text).translate()
@@ -107,15 +106,15 @@
 reversed = Reverse(text, symbol=True) # The default symbol value is True 
 print(reversed)
 ```
 output
 ```
 betam xru sew nw.
 ```
-#
+
 
 ## **Rules** 
 There are some **rules** that should be apply when writing the text.
  1. For **1st alphabets (ለግዕዝ)** use "e" example: "le" - ለ
  2. For **2nd alphabets (ለካእብ)** use "u" example: "lu" - ሉ
  3. For **3rd alphabets (ለሳልስ)** use "i" example: "li" - ሊ
  4. For **4rh alphabets (ለራዕብ)** use "a" example: "la" - ላ
@@ -145,8 +144,8 @@
 |  phe  |  phu  |  phi  |  pha  |  phie   |  ph  |  pho  |
 |  **ፐ**  |  **ፑ**  |  **ፒ**  |  **ፓ**  |  **ፔ**   |  **ፕ**  |  **ፖ**  |
 |  pe  |  pu |  pi  |  pa  |  pie   |  p  |  po  |
 
 **Addition** <br>
 |Alphabets |ሸ| ኘ| ዥ| ጸ| 
 |-----|-----|-----|-----|------|
-|Prefix |sh |gn |zh| ts|
+|Prefix |sh |gn |zh| ts|
```

