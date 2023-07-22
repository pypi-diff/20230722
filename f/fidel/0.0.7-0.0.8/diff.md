# Comparing `tmp/fidel-0.0.7.tar.gz` & `tmp/fidel-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fidel-0.0.7.tar", last modified: Thu Dec 15 23:33:55 2022, max compression
+gzip compressed data, was "fidel-0.0.8.tar", last modified: Sat Jul 22 15:32:06 2023, max compression
```

## Comparing `fidel-0.0.7.tar` & `fidel-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0 ny        (1000) ny        (1000)        0 2022-12-15 23:33:54.987679 fidel-0.0.7/
--rwxrwxrwx   0 ny        (1000) ny        (1000)    35823 2022-12-08 01:49:24.000000 fidel-0.0.7/LICENSE
--rwxrwxrwx   0 ny        (1000) ny        (1000)     3984 2022-12-15 23:33:54.986696 fidel-0.0.7/PKG-INFO
--rwxrwxrwx   0 ny        (1000) ny        (1000)     3616 2022-12-15 21:30:36.000000 fidel-0.0.7/README.md
--rwxrwxrwx   0 ny        (1000) ny        (1000)       38 2022-12-15 23:33:54.987679 fidel-0.0.7/setup.cfg
--rwxrwxrwx   0 ny        (1000) ny        (1000)      857 2022-12-15 22:48:21.000000 fidel-0.0.7/setup.py
-drwxrwxrwx   0 ny        (1000) ny        (1000)        0 2022-12-15 23:33:54.834936 fidel-0.0.7/src/
-drwxrwxrwx   0 ny        (1000) ny        (1000)        0 2022-12-15 23:33:54.909096 fidel-0.0.7/src/fidel/
--rwxrwxrwx   0 ny        (1000) ny        (1000)       38 2022-12-15 15:07:04.000000 fidel-0.0.7/src/fidel/__init__.py
-drwxrwxrwx   0 ny        (1000) ny        (1000)        0 2022-12-15 23:33:54.957953 fidel-0.0.7/src/fidel/data/
--rwxrwxrwx   0 ny        (1000) ny        (1000)   857510 2022-12-15 22:19:26.000000 fidel-0.0.7/src/fidel/data/word_list.txt
--rwxrwxrwx   0 ny        (1000) ny        (1000)     2832 2022-12-15 15:40:43.000000 fidel-0.0.7/src/fidel/dictionary.py
--rwxrwxrwx   0 ny        (1000) ny        (1000)     2207 2022-12-15 23:32:54.000000 fidel-0.0.7/src/fidel/translate.py
--rwxrwxrwx   0 ny        (1000) ny        (1000)     3378 2022-12-15 15:44:25.000000 fidel-0.0.7/src/fidel/word.py
-drwxrwxrwx   0 ny        (1000) ny        (1000)        0 2022-12-15 23:33:54.954054 fidel-0.0.7/src/fidel.egg-info/
--rwxrwxrwx   0 ny        (1000) ny        (1000)     3984 2022-12-15 23:33:53.000000 fidel-0.0.7/src/fidel.egg-info/PKG-INFO
--rwxrwxrwx   0 ny        (1000) ny        (1000)      306 2022-12-15 23:33:53.000000 fidel-0.0.7/src/fidel.egg-info/SOURCES.txt
--rwxrwxrwx   0 ny        (1000) ny        (1000)        1 2022-12-15 23:33:53.000000 fidel-0.0.7/src/fidel.egg-info/dependency_links.txt
--rwxrwxrwx   0 ny        (1000) ny        (1000)       18 2022-12-15 23:33:53.000000 fidel-0.0.7/src/fidel.egg-info/requires.txt
--rwxrwxrwx   0 ny        (1000) ny        (1000)        6 2022-12-15 23:33:53.000000 fidel-0.0.7/src/fidel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.975965 fidel-0.0.8/
+-rw-rw-rw-   0        0        0    35823 2022-12-08 01:49:24.000000 fidel-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5256 2023-07-22 15:32:06.973962 fidel-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4741 2023-07-22 15:11:54.000000 fidel-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-22 15:32:06.975965 fidel-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-07-22 15:30:16.000000 fidel-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.692793 fidel-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.732836 fidel-0.0.8/src/fidel/
+-rw-rw-rw-   0        0        0       63 2023-07-21 19:08:53.000000 fidel-0.0.8/src/fidel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.969973 fidel-0.0.8/src/fidel/data/
+-rw-rw-rw-   0        0        0   857510 2022-12-15 22:19:26.000000 fidel-0.0.8/src/fidel/data/word_list.txt
+-rw-rw-rw-   0        0        0     2746 2023-07-22 14:38:47.000000 fidel-0.0.8/src/fidel/main.py
+drwxrwxrwx   0        0        0        0 2023-07-22 15:32:06.967738 fidel-0.0.8/src/fidel.egg-info/
+-rw-rw-rw-   0        0        0     5256 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-22 15:32:06.000000 fidel-0.0.8/src/fidel.egg-info/top_level.txt
```

### Comparing `fidel-0.0.7/LICENSE` & `fidel-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fidel-0.0.7/PKG-INFO` & `fidel-0.0.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,152 @@
-Metadata-Version: 2.1
-Name: fidel
-Version: 0.0.7
-Summary: Python package that can change Amharic language that written in English alphabet to Amharic alphabet character.
-Author: Niftalem Yeneneh
-Author-email: n.y.official.em@gmail.com
-Keywords: python,amharic,english to amharic,ethiopia,translate,fidel
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# **Fidel / ፊደል**
-## What is **Fidel / ፊደል** ?
-**Fidel** is a python package that can change Amharic language that written in English alphabet to Amharic alphabet character. <br>
-**| For example: abebe beso bela -> አበበ በሶ በላ**
-#
-
-## **Dependencies**
-* [Symspellpy](https://github.com/mammothb/symspellpy)
-#
-
-## **Installation** 
-```
-pip install fidel
-```
-#
-
-## **Usage**
-
-### **Without Autocorrect**
-``` python
-from fidel import Translate
-text = "bexam xru sew new"
-trans_word = Translate(text=text,AutoCorrect=False).translate()
-print(trans_word)
-```
-output
-```
-በጣም ጥሩ ሰው ነው
-```
-
-### **Autocorrect Mode**
-``` python
-from fidel import Translate
-text = "betam tiru sew nw"
-trans_word = Translate(text=text,AutoCorrect=False).translate()
-corrected_word = Translate(text=text,AutoCorrect=True).translate()
-print(f"translated : {trans_word}")
-print(f"corrected_word : {corrected_word}")
-```
-output
-```
-translated : በታም ቲሩ ሰው ንው
-corrected_word : በጣም ጥሩ ሰው ነው
-```
-#
-
-## **Rules** 
-There are some **rules** that should be apply when writing the text
- 1. For **1st alphabets (ለግዕዝ)** use "e" example: "le" - ለ
- 2. For **2nd alphabets (ለካእብ)** use "u" example: "lu" - ሉ
- 3. For **3rd alphabets (ለሳልስ)** use "i" example: "li" - ሊ
- 4. For **4rh alphabets (ለራዕብ)** use "a" example: "la" - ላ
- 5. For **5th alphabets (ለሀምስ)** use "ie" example: "lie" - ሌ
- 6. For **6th alphabets (ለሳድስ)** use only vowel example: "l" - ል
- 7. For **7th alphabets (ለሳብዕ)** use "o" example: "lo" - ሎ
- 8. For **8th alphabets(ለዲቃላ ቃላት)** use "ua" example: "ua" -  ሏ 
-
-**Note** The above rules may violate for some alphabets family check out ambiguous alphabets.
-## **Ambiguous alphabets**
-
-| ግዕዝ | ካእብ | ሳልስ | ራዕብ | ሀምስ | ሳድስ | ሳብዕ |
-|-----|-----|-----|-----|------|-----|-----|
-|  **ሀ**  |  **ሁ**  |  **ሂ**  |  **ሀ**  |  **ሄ**   |  **ህ**  |  **ሆ**  |
-| ha  | hu  | hi  | ha  | hie  |  h  |  ho |
-|  **አ**  |  **ኡ**  |  **ኢ**  |  **ኣ**  |  **ኤ**   |  **እ**  |  **ኦ**  |
-|  a  |  u  |  i  |  a   |  ie  |  e  |  o  |
-|  **ተ**  |  **ቱ**  |  **ቲ**  |  **ታ**  |  **ቴ**   |  **ት**  |  **ቶ**  |
-|  te |  tu  |  ti  |  ta  |  tie   |  t  |  to  |
-|  **ጠ**  |  **ጡ**  |  **ጢ** | **ጣ**  |  **ጤ**   |  **ጥ**  |  **ጦ**  |
-|  xe  |  xu  |  xi  |  xa  |  xie   |  x  |  xo  |
-|  **ቸ**  | **ቹ**  |  **ቺ**  |  **ቻ**  |  **ቼ**   |  **ች**  |  **ቾ**  |
-|  che  |  chu  |  chi  |  cha  |  chie   |  ch  |  cho  |
-|  **ጨ**  |  **ጩ** |  **ጪ**  |  **ጫ**  |  **ጬ**   | **ጭ** |  **ጮ**  |
-|  ce  |  cu  |  ci  |  ca  |  cie   |  c  |  co  |
-|  **ጰ**  |  **ጱ**  |  **ጲ**  |  **ጳ**  |  **ጴ**   |  **ጵ**  |  **ጶ**  |
-|  phe  |  phu  |  phi  |  pha  |  phie   |  ph  |  pho  |
-|  **ፐ**  |  **ፑ**  |  **ፒ**  |  **ፓ**  |  **ፔ**   |  **ፕ**  |  **ፖ**  |
-|  pe  |  pu |  pi  |  pa  |  pie   |  p  |  po  |
-
-**Addition** <br>
-|Alphabets |ሸ| ኘ| ዥ| ጸ| 
-|-----|-----|-----|-----|------|
-|Prefix |sh |gn |zh| ts|
-#
-
-## **Donate and feedback** 
-
-contact me : [![image](https://img.icons8.com/color/20/null/telegram-app--v1.png)](https://t.me/ny_off_tm) [Telegram](https://t.me/ny_off_tm) <br>
-        [![image](https://img.icons8.com/fluency/20/000000/instagram-new.png)](https://www.instagram.com/ny.off.ig/) [Instagram](https://www.instagram.com/ny.off.ig/) 
-
+Metadata-Version: 2.1
+Name: fidel
+Version: 0.0.8
+Summary: Python package that can change Amharic language that written in English alphabet to Amharic alphabet character.
+Author: Niftalem Yeneneh
+Author-email: ny.dev0.em@gmail.com
+Keywords: python,amharic,english to amharic,ethiopia,translate,fidel
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# **Fidel / ፊደል**
+## What is **Fidel / ፊደል** ?
+**Fidel** is a python package that can change Amharic language that written in English alphabet to Amharic alphabet character. <br>
+**| For example: abebe beso bela -> አበበ በሶ በላ**
+#
+
+## **Dependencies**
+* [Symspellpy](https://github.com/mammothb/symspellpy)
+#
+
+## **Installation** 
+```
+pip install fidel
+```
+## **Upgrade**
+```
+pip install --upgrade fidel
+```
+#
+
+
+## **Usage**
+
+### **Basic Usage**
+``` python
+from fidel import Translate
+text = "bexam xru sew new"
+translated = Translate(text).translate()
+print(translated)
+```
+output
+```
+በጣም ጥሩ ሰው ነው
+```
+
+### **Autocorrect**
+``` python
+from fidel import Translate
+text = "betam tiru sew nw"
+translated = Translate(text=text,autoCorrect=False).translate() # The default is False
+corrected = Translate(text=text,autoCorrect=True).translate()
+print(f"Translated : {translated}")
+print(f"Corrected: {corrected}")
+
+```
+output
+```
+Translated : በታም ቲሩ ሰው ንው
+Corrected: በጣም ጥሩ ሰው ነው
+```
+### **Amharic Symbol**
+``` python 
+from fidel import Translate
+text = "abebe, kebede ena ayele bexam xru sew nachew."
+symbol_true = Translate(text=text,symbol=True).translate() # The default is True
+symbol_false = Translate(text=text,symbol=False).translate()
+print(f"True symbol: {symbol_true}")
+print(f"False symbol: {symbol_false}")
+```
+output
+```
+True symbol:  አበበ፣ ከበደ እና አየለ በጣም ጥሩ ሰው ናቸው።
+False symbol: አበበ, ከበደ እና አየለ በጣም ጥሩ ሰው ናቸው.
+```
+### **Exclude words** and **split words**
+**Exclude words** from being translated.
+- To prevent words from being translate, put the words inside "``" 
+``` python
+from fidel import Translate
+text = "`Alex` xru sew new"
+translated = Translate(text).translate()
+print(translated)
+
+```
+output
+```
+Alex ጥሩ ሰው ነው
+```
+**Split words**
+- To prevent words from being ዲቃላ (The eigth letters) we should put "|" between consonants.
+``` python
+from fidel import Translate
+text = "ljtua t|sewer" # Without "|" the output is "ልጅቷ ጸወር"
+translated = Translate(text).translate()
+print(translated)
+```
+output
+```
+ልጅቷ ትሰወር
+```
+
+### **Reverse Translate**
+``` python
+from fidel import Reverse
+text = "በጣም ጥሩ ሰው ነው።"
+reversed = Reverse(text, symbol=True) # The default symbol value is True 
+print(reversed)
+```
+output
+```
+betam xru sew nw.
+```
+#
+
+## **Rules** 
+There are some **rules** that should be apply when writing the text.
+ 1. For **1st alphabets (ለግዕዝ)** use "e" example: "le" - ለ
+ 2. For **2nd alphabets (ለካእብ)** use "u" example: "lu" - ሉ
+ 3. For **3rd alphabets (ለሳልስ)** use "i" example: "li" - ሊ
+ 4. For **4rh alphabets (ለራዕብ)** use "a" example: "la" - ላ
+ 5. For **5th alphabets (ለሀምስ)** use "ie" example: "lie" - ሌ
+ 6. For **6th alphabets (ለሳድስ)** use only vowel example: "l" - ል
+ 7. For **7th alphabets (ለሳብዕ)** use "o" example: "lo" - ሎ
+ 8. For **8th alphabets(ለዲቃላ ቃላት)** use "ua" example: "ua" -  ሏ 
+
+**Note** The above rules may violate for some alphabets family check out ambiguous alphabets.
+## **Ambiguous alphabets**
+
+| ግዕዝ | ካእብ | ሳልስ | ራዕብ | ሀምስ | ሳድስ | ሳብዕ |
+|-----|-----|-----|-----|------|-----|-----|
+|  **ሀ**  |  **ሁ**  |  **ሂ**  |  **ሀ**  |  **ሄ**   |  **ህ**  |  **ሆ**  |
+| ha  | hu  | hi  | ha  | hie  |  h  |  ho |
+|  **አ**  |  **ኡ**  |  **ኢ**  |  **ኣ**  |  **ኤ**   |  **እ**  |  **ኦ**  |
+|  a  |  u  |  i  |  a   |  ie  |  e  |  o  |
+|  **ተ**  |  **ቱ**  |  **ቲ**  |  **ታ**  |  **ቴ**   |  **ት**  |  **ቶ**  |
+|  te |  tu  |  ti  |  ta  |  tie   |  t  |  to  |
+|  **ጠ**  |  **ጡ**  |  **ጢ** | **ጣ**  |  **ጤ**   |  **ጥ**  |  **ጦ**  |
+|  xe  |  xu  |  xi  |  xa  |  xie   |  x  |  xo  |
+|  **ቸ**  | **ቹ**  |  **ቺ**  |  **ቻ**  |  **ቼ**   |  **ች**  |  **ቾ**  |
+|  che  |  chu  |  chi  |  cha  |  chie   |  ch  |  cho  |
+|  **ጨ**  |  **ጩ** |  **ጪ**  |  **ጫ**  |  **ጬ**   | **ጭ** |  **ጮ**  |
+|  ce  |  cu  |  ci  |  ca  |  cie   |  c  |  co  |
+|  **ጰ**  |  **ጱ**  |  **ጲ**  |  **ጳ**  |  **ጴ**   |  **ጵ**  |  **ጶ**  |
+|  phe  |  phu  |  phi  |  pha  |  phie   |  ph  |  pho  |
+|  **ፐ**  |  **ፑ**  |  **ፒ**  |  **ፓ**  |  **ፔ**   |  **ፕ**  |  **ፖ**  |
+|  pe  |  pu |  pi  |  pa  |  pie   |  p  |  po  |
+
+**Addition** <br>
+|Alphabets |ሸ| ኘ| ዥ| ጸ| 
+|-----|-----|-----|-----|------|
+|Prefix |sh |gn |zh| ts|
```

### Comparing `fidel-0.0.7/README.md` & `fidel-0.0.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,48 +8,106 @@
 * [Symspellpy](https://github.com/mammothb/symspellpy)
 #
 
 ## **Installation** 
 ```
 pip install fidel
 ```
+## **Upgrade**
+```
+pip install --upgrade fidel
+```
 #
 
+
 ## **Usage**
 
-### **Without Autocorrect**
+### **Basic Usage**
 ``` python
 from fidel import Translate
 text = "bexam xru sew new"
-trans_word = Translate(text=text,AutoCorrect=False).translate()
-print(trans_word)
+translated = Translate(text).translate()
+print(translated)
 ```
 output
 ```
 በጣም ጥሩ ሰው ነው
 ```
 
-### **Autocorrect Mode**
+### **Autocorrect**
 ``` python
 from fidel import Translate
 text = "betam tiru sew nw"
-trans_word = Translate(text=text,AutoCorrect=False).translate()
-corrected_word = Translate(text=text,AutoCorrect=True).translate()
-print(f"translated : {trans_word}")
-print(f"corrected_word : {corrected_word}")
+translated = Translate(text=text,autoCorrect=False).translate() # The default is False
+corrected = Translate(text=text,autoCorrect=True).translate()
+print(f"Translated : {translated}")
+print(f"Corrected: {corrected}")
+
+```
+output
+```
+Translated : በታም ቲሩ ሰው ንው
+Corrected: በጣም ጥሩ ሰው ነው
+```
+### **Amharic Symbol**
+``` python 
+from fidel import Translate
+text = "abebe, kebede ena ayele bexam xru sew nachew."
+symbol_true = Translate(text=text,symbol=True).translate() # The default is True
+symbol_false = Translate(text=text,symbol=False).translate()
+print(f"True symbol: {symbol_true}")
+print(f"False symbol: {symbol_false}")
+```
+output
+```
+True symbol:  አበበ፣ ከበደ እና አየለ በጣም ጥሩ ሰው ናቸው።
+False symbol: አበበ, ከበደ እና አየለ በጣም ጥሩ ሰው ናቸው.
+```
+### **Exclude words** and **split words**
+**Exclude words** from being translated.
+- To prevent words from being translate, put the words inside "``" 
+``` python
+from fidel import Translate
+text = "`Alex` xru sew new"
+translated = Translate(text).translate()
+print(translated)
+
 ```
 output
 ```
-translated : በታም ቲሩ ሰው ንው
-corrected_word : በጣም ጥሩ ሰው ነው
+Alex ጥሩ ሰው ነው
+```
+**Split words**
+- To prevent words from being ዲቃላ (The eigth letters) we should put "|" between consonants.
+``` python
+from fidel import Translate
+text = "ljtua t|sewer" # Without "|" the output is "ልጅቷ ጸወር"
+translated = Translate(text).translate()
+print(translated)
+```
+output
+```
+ልጅቷ ትሰወር
+```
+
+### **Reverse Translate**
+``` python
+from fidel import Reverse
+text = "በጣም ጥሩ ሰው ነው።"
+reversed = Reverse(text, symbol=True) # The default symbol value is True 
+print(reversed)
+```
+output
+```
+betam xru sew nw.
 ```
 #
 
 ## **Rules** 
-There are some **rules** that should be apply when writing the text
+There are some **rules** that should be apply when writing the text.
  1. For **1st alphabets (ለግዕዝ)** use "e" example: "le" - ለ
  2. For **2nd alphabets (ለካእብ)** use "u" example: "lu" - ሉ
  3. For **3rd alphabets (ለሳልስ)** use "i" example: "li" - ሊ
  4. For **4rh alphabets (ለራዕብ)** use "a" example: "la" - ላ
  5. For **5th alphabets (ለሀምስ)** use "ie" example: "lie" - ሌ
  6. For **6th alphabets (ለሳድስ)** use only vowel example: "l" - ል
  7. For **7th alphabets (ለሳብዕ)** use "o" example: "lo" - ሎ
@@ -77,14 +135,7 @@
 |  **ፐ**  |  **ፑ**  |  **ፒ**  |  **ፓ**  |  **ፔ**   |  **ፕ**  |  **ፖ**  |
 |  pe  |  pu |  pi  |  pa  |  pie   |  p  |  po  |
 
 **Addition** <br>
 |Alphabets |ሸ| ኘ| ዥ| ጸ| 
 |-----|-----|-----|-----|------|
 |Prefix |sh |gn |zh| ts|
-#
-
-## **Donate and feedback** 
-
-contact me : [![image](https://img.icons8.com/color/20/null/telegram-app--v1.png)](https://t.me/ny_off_tm) [Telegram](https://t.me/ny_off_tm) <br>
-        [![image](https://img.icons8.com/fluency/20/000000/instagram-new.png)](https://www.instagram.com/ny.off.ig/) [Instagram](https://www.instagram.com/ny.off.ig/) 
-
```

### Comparing `fidel-0.0.7/setup.py` & `fidel-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Python package that can change Amharic language that written in English alphabet to Amharic alphabet character.'
 
 setup(
     name="fidel",
     version=VERSION,
     author="Niftalem Yeneneh",
-    author_email="n.y.official.em@gmail.com",
+    author_email="ny.dev0.em@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=['fidel'],
     package_dir={'': 'src'},
     package_data={'': ['data/*.txt']},
     install_requires=["symspellpy == 6.7.1" ],
```

### Comparing `fidel-0.0.7/src/fidel/data/word_list.txt` & `fidel-0.0.8/src/fidel/data/word_list.txt`

 * *Files identical despite different names*

### Comparing `fidel-0.0.7/src/fidel/translate.py` & `fidel-0.0.8/src/fidel/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,71 @@
-from fidel.word import sep_words
+from fidel.utilities.word import sep_words
 from symspellpy import SymSpell, Verbosity
-from fidel.dictionary import dict 
+from fidel.utilities.dictionary import dict
+from fidel.helpers.filter import filter_symbol
 import os
 
 PROJECT_DIR = os.path.dirname(__file__)
 
-class Translate():
+class Translate:
 	'''
 	Args:
-		text: The string being translated.
-		AutoCorrect: boolean to turn on and off auto correct default.
+		text: The text to be translated.
+		autocorrect: Boolean to enable and disable auto correct default.
+		symbol: Boolean to enable and disable symbol changing.
+	''' 
+	def __init__(self, text:str, autoCorrect:bool=False, symbol=True):
+		self.text = text
+		self.autocorrect = autoCorrect
+		self.symbol = symbol  
+
+	def translate(self) -> str:
+		result = func(func(self.text).translate(self.symbol)).auto_correct() if self.autocorrect == True else func(self.text).translate(self.symbol)
+		
+		return result
+
+def Reverse(text:str, symbol:True) -> str:
 	'''
-	def __init__(self,text:str,AutoCorrect:True) -> str:
+	Reverse translate.
+	Args:
+		text: The text to be translated.
+		symbol: Boolean to enable and disable symbol changing.
+	'''
+	main_dic = dict(symbol)
+	reversed_dic = {key:value for value,key in main_dic.items()} # Swap key and value and form new dictionary
+	translated_ver = ""
+
+	for letters in text:
+		translated_ver += reversed_dic.get(letters, letters)
+
+	return translated_ver.replace("h⨳"," ")
+
+class func:
+	def __init__(self, text:str):
 		self.text = text
-		self.autocorrect = False
-		self.autocorrect = AutoCorrect
-	def translate(self):
-		'''
-		Args:
-			``None``
-		return:
-			string that (translated) or (translated + autocorrect) deepend on AutoCorrect Value.
-		'''
-		if self.autocorrect == True:
-			result = func.auto_correct(func.translate(self.text))
-			return result
-		else:
-			result = func.translate(self.text)
-			return result
-
-
-class func():
-	def translate(text:str) -> str:
-		'''
-		Args:
-			text: The string being translated.
-		'''
-		list_inp = sep_words(text) # Separating words
-		added_word = "" 
-		main_dic = dict() # Prepare dictionary
-		for words in list_inp:
-			added_word += main_dic.get(words,words) # Add every changed characters
-		main_word = added_word.strip(" ") # Remove unneccesary spaces
-		return main_word
-	def auto_correct(text:str) -> str:
-		'''
-		Args:
-			text: The string being corrected.
-		'''
+
+	def translate(self,symbol: bool) -> str:
+
+		list_inp = sep_words(self.text) # Separating words
+		translated_ver = ""
+		main_dic = dict(symbol) # Prepare dictionary
+		for letters in list_inp:
+			translated_ver += main_dic.get(letters, letters.replace("`","")) # Add every changed characters
+		translated_ver = translated_ver.strip(" ") # Remove unneccesary spaces
+		
+		return translated_ver
+
+	def auto_correct(self) -> str:
 		result = "" # Corrected words added to this string
 		sym_spell = SymSpell(max_dictionary_edit_distance=2, prefix_length=7)
-		dictionary_path = os.path.join(PROJECT_DIR,"data/word_list.txt")
-		a = sym_spell.load_dictionary(dictionary_path ,term_index=0, count_index=1,encoding="UTF-8") # Preparing word list dictionary
-		trans_word = text.split(" ") # Translate and split by spaces
+		dictionary_path = os.path.join(PROJECT_DIR, "data/word_list.txt")
+		a = sym_spell.load_dictionary(dictionary_path, term_index=0, count_index=1, encoding="UTF-8") # Preparing word list dictionary
+		trans_word = self.text.split(" ") # Translate and split by spaces
 		for word in range(len(trans_word)):
-			suggestions = sym_spell.lookup(trans_word[word],verbosity=Verbosity.CLOSEST,max_edit_distance=2,ignore_token=r"\w+\d",include_unknown=True) # Get closest words
+			pure_text = filter_symbol(trans_word[word])
+			suggestions = sym_spell.lookup(pure_text.encode(),verbosity=Verbosity.CLOSEST, max_edit_distance=2, ignore_token=r"\w+\d", include_unknown=True) # Get closest words
 			for suggestion in range(len(suggestions)): # For each closest word
-				if len(str(suggestions[suggestion].term)) == len(trans_word[word]): # If the closest word have equal length as input word 
-					result += suggestions[suggestion].term + " " # Add the the closest word to result string
+				if len(str(suggestions[suggestion].term)) == len(trans_word[word]): # If the closest word have equal length as input word ?
+					result += pure_text.decode(suggestions[suggestion].term + " ") # Add the the closest word to result string
 					break
-		return result
+
+		return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fidel-0.0.7/src/fidel.egg-info/PKG-INFO` & `fidel-0.0.8/src/fidel.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,152 @@
-Metadata-Version: 2.1
-Name: fidel
-Version: 0.0.7
-Summary: Python package that can change Amharic language that written in English alphabet to Amharic alphabet character.
-Author: Niftalem Yeneneh
-Author-email: n.y.official.em@gmail.com
-Keywords: python,amharic,english to amharic,ethiopia,translate,fidel
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# **Fidel / ፊደል**
-## What is **Fidel / ፊደል** ?
-**Fidel** is a python package that can change Amharic language that written in English alphabet to Amharic alphabet character. <br>
-**| For example: abebe beso bela -> አበበ በሶ በላ**
-#
-
-## **Dependencies**
-* [Symspellpy](https://github.com/mammothb/symspellpy)
-#
-
-## **Installation** 
-```
-pip install fidel
-```
-#
-
-## **Usage**
-
-### **Without Autocorrect**
-``` python
-from fidel import Translate
-text = "bexam xru sew new"
-trans_word = Translate(text=text,AutoCorrect=False).translate()
-print(trans_word)
-```
-output
-```
-በጣም ጥሩ ሰው ነው
-```
-
-### **Autocorrect Mode**
-``` python
-from fidel import Translate
-text = "betam tiru sew nw"
-trans_word = Translate(text=text,AutoCorrect=False).translate()
-corrected_word = Translate(text=text,AutoCorrect=True).translate()
-print(f"translated : {trans_word}")
-print(f"corrected_word : {corrected_word}")
-```
-output
-```
-translated : በታም ቲሩ ሰው ንው
-corrected_word : በጣም ጥሩ ሰው ነው
-```
-#
-
-## **Rules** 
-There are some **rules** that should be apply when writing the text
- 1. For **1st alphabets (ለግዕዝ)** use "e" example: "le" - ለ
- 2. For **2nd alphabets (ለካእብ)** use "u" example: "lu" - ሉ
- 3. For **3rd alphabets (ለሳልስ)** use "i" example: "li" - ሊ
- 4. For **4rh alphabets (ለራዕብ)** use "a" example: "la" - ላ
- 5. For **5th alphabets (ለሀምስ)** use "ie" example: "lie" - ሌ
- 6. For **6th alphabets (ለሳድስ)** use only vowel example: "l" - ል
- 7. For **7th alphabets (ለሳብዕ)** use "o" example: "lo" - ሎ
- 8. For **8th alphabets(ለዲቃላ ቃላት)** use "ua" example: "ua" -  ሏ 
-
-**Note** The above rules may violate for some alphabets family check out ambiguous alphabets.
-## **Ambiguous alphabets**
-
-| ግዕዝ | ካእብ | ሳልስ | ራዕብ | ሀምስ | ሳድስ | ሳብዕ |
-|-----|-----|-----|-----|------|-----|-----|
-|  **ሀ**  |  **ሁ**  |  **ሂ**  |  **ሀ**  |  **ሄ**   |  **ህ**  |  **ሆ**  |
-| ha  | hu  | hi  | ha  | hie  |  h  |  ho |
-|  **አ**  |  **ኡ**  |  **ኢ**  |  **ኣ**  |  **ኤ**   |  **እ**  |  **ኦ**  |
-|  a  |  u  |  i  |  a   |  ie  |  e  |  o  |
-|  **ተ**  |  **ቱ**  |  **ቲ**  |  **ታ**  |  **ቴ**   |  **ት**  |  **ቶ**  |
-|  te |  tu  |  ti  |  ta  |  tie   |  t  |  to  |
-|  **ጠ**  |  **ጡ**  |  **ጢ** | **ጣ**  |  **ጤ**   |  **ጥ**  |  **ጦ**  |
-|  xe  |  xu  |  xi  |  xa  |  xie   |  x  |  xo  |
-|  **ቸ**  | **ቹ**  |  **ቺ**  |  **ቻ**  |  **ቼ**   |  **ች**  |  **ቾ**  |
-|  che  |  chu  |  chi  |  cha  |  chie   |  ch  |  cho  |
-|  **ጨ**  |  **ጩ** |  **ጪ**  |  **ጫ**  |  **ጬ**   | **ጭ** |  **ጮ**  |
-|  ce  |  cu  |  ci  |  ca  |  cie   |  c  |  co  |
-|  **ጰ**  |  **ጱ**  |  **ጲ**  |  **ጳ**  |  **ጴ**   |  **ጵ**  |  **ጶ**  |
-|  phe  |  phu  |  phi  |  pha  |  phie   |  ph  |  pho  |
-|  **ፐ**  |  **ፑ**  |  **ፒ**  |  **ፓ**  |  **ፔ**   |  **ፕ**  |  **ፖ**  |
-|  pe  |  pu |  pi  |  pa  |  pie   |  p  |  po  |
-
-**Addition** <br>
-|Alphabets |ሸ| ኘ| ዥ| ጸ| 
-|-----|-----|-----|-----|------|
-|Prefix |sh |gn |zh| ts|
-#
-
-## **Donate and feedback** 
-
-contact me : [![image](https://img.icons8.com/color/20/null/telegram-app--v1.png)](https://t.me/ny_off_tm) [Telegram](https://t.me/ny_off_tm) <br>
-        [![image](https://img.icons8.com/fluency/20/000000/instagram-new.png)](https://www.instagram.com/ny.off.ig/) [Instagram](https://www.instagram.com/ny.off.ig/) 
-
+Metadata-Version: 2.1
+Name: fidel
+Version: 0.0.8
+Summary: Python package that can change Amharic language that written in English alphabet to Amharic alphabet character.
+Author: Niftalem Yeneneh
+Author-email: ny.dev0.em@gmail.com
+Keywords: python,amharic,english to amharic,ethiopia,translate,fidel
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# **Fidel / ፊደል**
+## What is **Fidel / ፊደል** ?
+**Fidel** is a python package that can change Amharic language that written in English alphabet to Amharic alphabet character. <br>
+**| For example: abebe beso bela -> አበበ በሶ በላ**
+#
+
+## **Dependencies**
+* [Symspellpy](https://github.com/mammothb/symspellpy)
+#
+
+## **Installation** 
+```
+pip install fidel
+```
+## **Upgrade**
+```
+pip install --upgrade fidel
+```
+#
+
+
+## **Usage**
+
+### **Basic Usage**
+``` python
+from fidel import Translate
+text = "bexam xru sew new"
+translated = Translate(text).translate()
+print(translated)
+```
+output
+```
+በጣም ጥሩ ሰው ነው
+```
+
+### **Autocorrect**
+``` python
+from fidel import Translate
+text = "betam tiru sew nw"
+translated = Translate(text=text,autoCorrect=False).translate() # The default is False
+corrected = Translate(text=text,autoCorrect=True).translate()
+print(f"Translated : {translated}")
+print(f"Corrected: {corrected}")
+
+```
+output
+```
+Translated : በታም ቲሩ ሰው ንው
+Corrected: በጣም ጥሩ ሰው ነው
+```
+### **Amharic Symbol**
+``` python 
+from fidel import Translate
+text = "abebe, kebede ena ayele bexam xru sew nachew."
+symbol_true = Translate(text=text,symbol=True).translate() # The default is True
+symbol_false = Translate(text=text,symbol=False).translate()
+print(f"True symbol: {symbol_true}")
+print(f"False symbol: {symbol_false}")
+```
+output
+```
+True symbol:  አበበ፣ ከበደ እና አየለ በጣም ጥሩ ሰው ናቸው።
+False symbol: አበበ, ከበደ እና አየለ በጣም ጥሩ ሰው ናቸው.
+```
+### **Exclude words** and **split words**
+**Exclude words** from being translated.
+- To prevent words from being translate, put the words inside "``" 
+``` python
+from fidel import Translate
+text = "`Alex` xru sew new"
+translated = Translate(text).translate()
+print(translated)
+
+```
+output
+```
+Alex ጥሩ ሰው ነው
+```
+**Split words**
+- To prevent words from being ዲቃላ (The eigth letters) we should put "|" between consonants.
+``` python
+from fidel import Translate
+text = "ljtua t|sewer" # Without "|" the output is "ልጅቷ ጸወር"
+translated = Translate(text).translate()
+print(translated)
+```
+output
+```
+ልጅቷ ትሰወር
+```
+
+### **Reverse Translate**
+``` python
+from fidel import Reverse
+text = "በጣም ጥሩ ሰው ነው።"
+reversed = Reverse(text, symbol=True) # The default symbol value is True 
+print(reversed)
+```
+output
+```
+betam xru sew nw.
+```
+#
+
+## **Rules** 
+There are some **rules** that should be apply when writing the text.
+ 1. For **1st alphabets (ለግዕዝ)** use "e" example: "le" - ለ
+ 2. For **2nd alphabets (ለካእብ)** use "u" example: "lu" - ሉ
+ 3. For **3rd alphabets (ለሳልስ)** use "i" example: "li" - ሊ
+ 4. For **4rh alphabets (ለራዕብ)** use "a" example: "la" - ላ
+ 5. For **5th alphabets (ለሀምስ)** use "ie" example: "lie" - ሌ
+ 6. For **6th alphabets (ለሳድስ)** use only vowel example: "l" - ል
+ 7. For **7th alphabets (ለሳብዕ)** use "o" example: "lo" - ሎ
+ 8. For **8th alphabets(ለዲቃላ ቃላት)** use "ua" example: "ua" -  ሏ 
+
+**Note** The above rules may violate for some alphabets family check out ambiguous alphabets.
+## **Ambiguous alphabets**
+
+| ግዕዝ | ካእብ | ሳልስ | ራዕብ | ሀምስ | ሳድስ | ሳብዕ |
+|-----|-----|-----|-----|------|-----|-----|
+|  **ሀ**  |  **ሁ**  |  **ሂ**  |  **ሀ**  |  **ሄ**   |  **ህ**  |  **ሆ**  |
+| ha  | hu  | hi  | ha  | hie  |  h  |  ho |
+|  **አ**  |  **ኡ**  |  **ኢ**  |  **ኣ**  |  **ኤ**   |  **እ**  |  **ኦ**  |
+|  a  |  u  |  i  |  a   |  ie  |  e  |  o  |
+|  **ተ**  |  **ቱ**  |  **ቲ**  |  **ታ**  |  **ቴ**   |  **ት**  |  **ቶ**  |
+|  te |  tu  |  ti  |  ta  |  tie   |  t  |  to  |
+|  **ጠ**  |  **ጡ**  |  **ጢ** | **ጣ**  |  **ጤ**   |  **ጥ**  |  **ጦ**  |
+|  xe  |  xu  |  xi  |  xa  |  xie   |  x  |  xo  |
+|  **ቸ**  | **ቹ**  |  **ቺ**  |  **ቻ**  |  **ቼ**   |  **ች**  |  **ቾ**  |
+|  che  |  chu  |  chi  |  cha  |  chie   |  ch  |  cho  |
+|  **ጨ**  |  **ጩ** |  **ጪ**  |  **ጫ**  |  **ጬ**   | **ጭ** |  **ጮ**  |
+|  ce  |  cu  |  ci  |  ca  |  cie   |  c  |  co  |
+|  **ጰ**  |  **ጱ**  |  **ጲ**  |  **ጳ**  |  **ጴ**   |  **ጵ**  |  **ጶ**  |
+|  phe  |  phu  |  phi  |  pha  |  phie   |  ph  |  pho  |
+|  **ፐ**  |  **ፑ**  |  **ፒ**  |  **ፓ**  |  **ፔ**   |  **ፕ**  |  **ፖ**  |
+|  pe  |  pu |  pi  |  pa  |  pie   |  p  |  po  |
+
+**Addition** <br>
+|Alphabets |ሸ| ኘ| ዥ| ጸ| 
+|-----|-----|-----|-----|------|
+|Prefix |sh |gn |zh| ts|
```

