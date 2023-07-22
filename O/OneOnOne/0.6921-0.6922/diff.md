# Comparing `tmp/OneOnOne-0.6921.tar.gz` & `tmp/OneOnOne-0.6922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6921.tar", last modified: Sat Jul 22 04:26:51 2023, max compression
+gzip compressed data, was "OneOnOne-0.6922.tar", last modified: Sat Jul 22 05:49:17 2023, max compression
```

## Comparing `OneOnOne-0.6921.tar` & `OneOnOne-0.6922.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 04:26:51.563810 OneOnOne-0.6921/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6921/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 04:26:51.558330 OneOnOne-0.6921/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    49698 2023-07-22 04:26:43.000000 OneOnOne-0.6921/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6921/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6921/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6921/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6921/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6921/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6921/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 04:26:51.563006 OneOnOne-0.6921/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 04:26:51.000000 OneOnOne-0.6921/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 04:26:51.000000 OneOnOne-0.6921/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 04:26:51.000000 OneOnOne-0.6921/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 04:26:51.000000 OneOnOne-0.6921/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 04:26:51.000000 OneOnOne-0.6921/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 04:26:51.563442 OneOnOne-0.6921/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6921/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 04:26:51.563923 OneOnOne-0.6921/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 04:26:47.000000 OneOnOne-0.6921/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 05:49:17.362765 OneOnOne-0.6922/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6922/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 05:49:17.357570 OneOnOne-0.6922/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    49696 2023-07-22 04:30:39.000000 OneOnOne-0.6922/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6922/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6922/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6922/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6922/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6922/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6922/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 05:49:17.361360 OneOnOne-0.6922/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 05:49:17.000000 OneOnOne-0.6922/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 05:49:17.000000 OneOnOne-0.6922/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 05:49:17.000000 OneOnOne-0.6922/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 05:49:17.000000 OneOnOne-0.6922/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 05:49:17.000000 OneOnOne-0.6922/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 05:49:17.362048 OneOnOne-0.6922/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6922/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 05:49:17.362943 OneOnOne-0.6922/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 05:49:12.000000 OneOnOne-0.6922/setup.py
```

### Comparing `OneOnOne-0.6921/LICENSE` & `OneOnOne-0.6922/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6921/OneOnOne/__init__.py` & `OneOnOne-0.6922/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1193,15 +1193,15 @@
             self.model = BlipForQuestionAnswering.from_pretrained("Salesforce/blip-vqa-base").to("cuda")
 
         else:
             print("invalid input")
 
     def question_answer(self, question):
 
-        # input_ids = self.tokenizer.encode(question, self.context)
+        input_ids = self.tokenizer.encode(question, self.context)
 
         # tokens = self.tokenizer.convert_ids_to_tokens(input_ids)
 
         tokens = self.tokenizer.tokenize(self.context, max_length=self.max_length, truncation=True)
 
         sep_idx = input_ids.index(self.tokenizer.sep_token_id)
```

### Comparing `OneOnOne-0.6921/OneOnOne/classes.py` & `OneOnOne-0.6922/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6921/OneOnOne/classification.py` & `OneOnOne-0.6922/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6921/OneOnOne/contextdecider.py` & `OneOnOne-0.6922/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6921/OneOnOne/htmlparser.py` & `OneOnOne-0.6922/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6921/OneOnOne/questionanswer.py` & `OneOnOne-0.6922/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6921/OneOnOne/sampling.py` & `OneOnOne-0.6922/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6921/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6922/OneOnOne.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6921
+Version: 0.6922
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6921/PKG-INFO` & `OneOnOne-0.6922/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6921
+Version: 0.6922
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6921/README.md` & `OneOnOne-0.6922/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6921/setup.py` & `OneOnOne-0.6922/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6921
+VERSION=0.6922
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

