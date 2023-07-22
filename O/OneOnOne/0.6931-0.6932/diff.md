# Comparing `tmp/OneOnOne-0.6931.tar.gz` & `tmp/OneOnOne-0.6932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6931.tar", last modified: Sat Jul 22 17:28:35 2023, max compression
+gzip compressed data, was "OneOnOne-0.6932.tar", last modified: Sat Jul 22 17:39:10 2023, max compression
```

## Comparing `OneOnOne-0.6931.tar` & `OneOnOne-0.6932.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:28:35.263556 OneOnOne-0.6931/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6931/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:28:35.258289 OneOnOne-0.6931/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    51818 2023-07-22 17:28:25.000000 OneOnOne-0.6931/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6931/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6931/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6931/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6931/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6931/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6931/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:28:35.262459 OneOnOne-0.6931/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 17:28:35.263104 OneOnOne-0.6931/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3366 2023-07-22 16:02:47.000000 OneOnOne-0.6931/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 17:28:35.263674 OneOnOne-0.6931/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 17:21:32.000000 OneOnOne-0.6931/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:39:10.651967 OneOnOne-0.6932/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6932/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:39:10.647125 OneOnOne-0.6932/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    52037 2023-07-22 17:32:50.000000 OneOnOne-0.6932/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6932/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6932/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6932/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6932/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6932/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6932/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:39:10.650695 OneOnOne-0.6932/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 17:39:10.000000 OneOnOne-0.6932/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 17:39:10.000000 OneOnOne-0.6932/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 17:39:10.000000 OneOnOne-0.6932/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 17:39:10.000000 OneOnOne-0.6932/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 17:39:10.000000 OneOnOne-0.6932/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 17:39:10.651358 OneOnOne-0.6932/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3366 2023-07-22 16:02:47.000000 OneOnOne-0.6932/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 17:39:10.652188 OneOnOne-0.6932/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1941 2023-07-22 17:39:06.000000 OneOnOne-0.6932/setup.py
```

### Comparing `OneOnOne-0.6931/LICENSE` & `OneOnOne-0.6932/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6931/OneOnOne/__init__.py` & `OneOnOne-0.6932/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 import requests, zipfile
 from io import BytesIO
 import gdown
 import imageio as iio
 from PIL import Image
 
 import warnings
-warnings.filterwarnings("ignore")
 
 class PretrainedModel:
     def __init__(self, model_type="resnet50", dataset="cifar10", samplingtype="none"):
+        warnings.filterwarnings("ignore")
 
         self.model_type=model_type.lower()
         self.dataset=dataset.lower()
         self.samplingtype=samplingtype.lower()
 
         self.map={"resnet50_cifar10_none":"1YVG0lAnpBfM_MB7ctV1vHcslb6O-3Vbm","resnet50_cifar10_leastconfidence":"1fSJYo5VOppTkgWb-Fu2Sf_JL4s9JUmoK","resnet50_cifar10_mixed":"","resnet50_cifar10_margin":"","efficientnetb6_cifar10_none":"16Wqfx7mcEhssZksF1yUAUEG6mkhMSeme","efficientnetb6_tinyimagenet_none":"1pGX8zB99ugqcvPohxykPC1JLM0Ld0L-D"}
 
@@ -93,14 +93,15 @@
 
         self.model=load_model(self.path)
         self.model.summary()
 
 
 class Classification:
     def __init__(self, model_type="resnet50", batch_size=16, epochs=250, dataset="cifar10", validation_split=0.3, shuffle_bool=True, early_stopping_patience=10, lr_reducer_patience=10):
+        warnings.filterwarnings("ignore")
 
         self.model_type = model_type.lower()
         self.date=datetime.datetime.now()
         self.dataset=dataset.lower()
         self.shuffle_bool = shuffle
         self.batch_size = batch_size
         self.epochs = epochs
@@ -419,14 +420,15 @@
 
     def evaluate(self):
         loss, accuracy = self.model.evaluate(self.val_it, batch_size=self.batch_size, verbose=1)
 
 
 class Sampling:
     def __init__(self, samplingtype, dataset="cifar10", model_type = "resnet50", goal=99, jump=5000, validation_split=0.3, first_data_samples=10000, batch_size = 16, epochs = 250, shuffle_bool = True, early_stopping_patience = 10, lr_reducer_patience = 10):
+        warnings.filterwarnings("ignore")
 
         self.validation_split=validation_split
         self.model_type = model_type.lower()
         self.epochs=epochs
         self.jump = jump
         self.samplingtype = samplingtype.lower()
         self.goal = goal
@@ -937,14 +939,16 @@
 
         self.model.save(os.getcwd() + f"/trained_models/{self.model_type}_{self.dataset}_{self.samplingtype}_{self.date}_completed")
 
         return history_data,epoch_data,batch_size_data,acuracy_data
 
 class HTMLparser:
     def __init__(self, words):
+        warnings.filterwarnings("ignore")
+
         self.words = words
     def clean_html(self,raw_html):
         clean_brackets = re.compile('<.*?>')
         cleantext = re.sub(clean_brackets, '', raw_html)
         cleantext = re.sub(' ,', '', cleantext)
         cleantext = re.sub('\n', '', cleantext)
         cleantext = cleantext.replace('\\', '')
@@ -976,14 +980,15 @@
             full_context = full_context + text_for_one_word[3:-1]
 
         return full_context
 
 
 class ContextDecider:
     def __init__(self, load=False, user_input=False, dataset="tinyimagenet", model_type="efficientnetb6", samplingtype="none", threshold=0.2, validation_split=0.3, batch_size=16, shuffle_bool=True):
+        warnings.filterwarnings("ignore")
 
         self.load=load
         self.user_input=user_input
         self.dataset = dataset.lower()
         self.model_type = model_type.lower()
         self.samplingtype = samplingtype
         self.threshold = threshold
@@ -1182,14 +1187,15 @@
             self.y_test = validation_labels
 
         return train_it, val_it
 
 
 class QuestionAnswer:
     def __init__(self, context, chatbot="bert"):
+        warnings.filterwarnings("ignore")
 
         self.exit_commands = ("no", "n", "quit", "pause", "exit", "goodbye", "bye", "later", "stop")
         self.positive_commands = ("y", "yes", "yeah", "sure", "yup", "ya", "probably", "maybe")
         self.context = context
         self.max_length = len(self.context)
         self.chatbot = chatbot.lower()
```

### Comparing `OneOnOne-0.6931/OneOnOne/classes.py` & `OneOnOne-0.6932/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6931/OneOnOne/classification.py` & `OneOnOne-0.6932/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6931/OneOnOne/contextdecider.py` & `OneOnOne-0.6932/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6931/OneOnOne/htmlparser.py` & `OneOnOne-0.6932/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6931/OneOnOne/questionanswer.py` & `OneOnOne-0.6932/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6931/OneOnOne/sampling.py` & `OneOnOne-0.6932/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6931/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6932/OneOnOne.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6931
+Version: 0.6932
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6931/PKG-INFO` & `OneOnOne-0.6932/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6931
+Version: 0.6932
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6931/README.md` & `OneOnOne-0.6932/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6931/setup.py` & `OneOnOne-0.6932/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6931
-
+VERSION=0.6932
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

