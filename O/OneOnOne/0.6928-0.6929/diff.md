# Comparing `tmp/OneOnOne-0.6928.tar.gz` & `tmp/OneOnOne-0.6929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6928.tar", last modified: Sat Jul 22 13:58:42 2023, max compression
+gzip compressed data, was "OneOnOne-0.6929.tar", last modified: Sat Jul 22 14:20:59 2023, max compression
```

## Comparing `OneOnOne-0.6928.tar` & `OneOnOne-0.6929.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 13:58:42.508551 OneOnOne-0.6928/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6928/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 13:58:42.499082 OneOnOne-0.6928/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    51035 2023-07-22 13:58:31.000000 OneOnOne-0.6928/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6928/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6928/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6928/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6928/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6928/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6928/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 13:58:42.506208 OneOnOne-0.6928/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 13:58:42.000000 OneOnOne-0.6928/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 13:58:42.000000 OneOnOne-0.6928/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 13:58:42.000000 OneOnOne-0.6928/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 13:58:42.000000 OneOnOne-0.6928/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 13:58:42.000000 OneOnOne-0.6928/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 13:58:42.507268 OneOnOne-0.6928/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6928/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 13:58:42.508846 OneOnOne-0.6928/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 13:56:55.000000 OneOnOne-0.6928/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 14:20:59.960933 OneOnOne-0.6929/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6929/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 14:20:59.956785 OneOnOne-0.6929/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    51728 2023-07-22 14:20:51.000000 OneOnOne-0.6929/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6929/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6929/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6929/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6929/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6929/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6929/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 14:20:59.960075 OneOnOne-0.6929/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 14:20:59.960508 OneOnOne-0.6929/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3359 2023-07-22 14:03:15.000000 OneOnOne-0.6929/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 14:20:59.961085 OneOnOne-0.6929/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 14:19:56.000000 OneOnOne-0.6929/setup.py
```

### Comparing `OneOnOne-0.6928/LICENSE` & `OneOnOne-0.6929/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6928/OneOnOne/__init__.py` & `OneOnOne-0.6929/OneOnOne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,19 @@
 from bs4 import BeautifulSoup
 import re
 from tqdm import keras
 import pkgutil
 import requests, zipfile
 from io import BytesIO
 import gdown
+import imageio as iio
+from PIL import Image
+
+import warnings
+warnings.filterwarnings("ignore")
 
 class PretrainedModel:
     def __init__(self, model_type="resnet50", dataset="cifar10", samplingtype="none"):
 
         self.model_type=model_type.lower()
         self.dataset=dataset.lower()
         self.samplingtype=samplingtype.lower()
@@ -970,17 +975,18 @@
             text_for_one_word = self.produce_text(word)
             full_context = full_context + text_for_one_word[3:-1]
 
         return full_context
 
 
 class ContextDecider:
-    def __init__(self, load=False, dataset="tinyimagenet", model_type="efficientnetb6", samplingtype="none", threshold=0.2, validation_split=0.3, batch_size=70000, shuffle_bool=True):
+    def __init__(self, load=False, user_input=False, dataset="tinyimagenet", model_type="efficientnetb6", samplingtype="none", threshold=0.2, validation_split=0.3, batch_size=16, shuffle_bool=True):
 
         self.load=load
+        self.user_input=user_input
         self.dataset = dataset.lower()
         self.model_type = model_type.lower()
         self.samplingtype = samplingtype
         self.threshold = threshold
         self.validation_split=validation_split
         self.batch_size = batch_size
         self.shuffle_bool = shuffle_bool
@@ -1008,15 +1014,30 @@
         if self.load:
             path=input("Please input the model's path/name in the current directory (str):     ")
             self.contextmodel=load_model(os.getcwd()+path)
         else:
             self.contextmodel = PretrainedModel(model_type=self.model_type, dataset=self.dataset,
                                           samplingtype=self.samplingtype)
         # self.pretrained.model
-        self.pred = self.contextmodel.model.predict_generator(self.val_it, random.randint(1, self.batch_size))
+        if self.user_input:
+            path=input("Please enter image path in the current directory (str):    ")
+            img = Image.open(os.getcwd()+f"{path}")
+            img.show()
+            img = iio.imread(os.getcwd()+f"{path}")
+            processed_image = preprocess_image_input(img)
+            self.pred = self.contextmodel.model.predict(processed_image)
+        else:
+            self.pred = self.contextmodel.model.predict_generator(self.val_it, random.randint(1, 3000))
+
+    def preprocess_image_input(self,input_images):
+        if self.model_type=="efficientnetb6":
+            input_images = input_images.astype('float32')
+            output_ims = tf.keras.applications.efficientnet.preprocess_input(input_images)
+
+        return output_ims
 
     def get_datagen(self):
 
         datagen = ImageDataGenerator(
             featurewise_center=False,
             samplewise_center=False,
             featurewise_std_normalization=False,
@@ -1169,23 +1190,23 @@
         self.positive_commands = ("y", "yes", "yeah", "sure", "yup", "ya", "probably", "maybe")
         self.context = context
         self.max_length = len(self.context)
         self.chatbot = chatbot.lower()
 
         if self.chatbot == "bert":
             self.model = BertForQuestionAnswering.from_pretrained('bert-large-uncased-whole-word-masking-finetuned-squad')
-            self.tokenizer = BertTokenizer.from_pretrained('bert-large-uncased-whole-word-masking-finetuned-squad',model_max_length=len(self.context))
+            self.tokenizer = BertTokenizer.from_pretrained('bert-large-uncased-whole-word-masking-finetuned-squad')
 
         elif self.chatbot == "gpt2":
             self.model = GPT2ForQuestionAnswering.from_pretrained("gpt2")
-            self.tokenizer = GPT2Tokenizer.from_pretrained("gpt2",model_max_length=len(self.context))
+            self.tokenizer = GPT2Tokenizer.from_pretrained("gpt2")
 
         elif self.chatbot == "roberta":
             self.model = RobertaForQuestionAnswering.from_pretrained("deepset/roberta-base-squad2")
-            self.tokenizer = AutoTokenizer.from_pretrained("deepset/roberta-base-squad2",model_max_length=len(self.context))
+            self.tokenizer = AutoTokenizer.from_pretrained("deepset/roberta-base-squad2")
 
         # elif self.chatbot == "ernie":
         #     self.model = ErnieModel.from_pretrained("nghuyong/ernie-1.0-base-zh")
         #     self.tokenizer = AutoTokenizer.from_pretrained("nghuyong/ernie-1.0-base-zh")
 
         # elif self.chatbot == "vqa":
         #     self.model = BlipForQuestionAnswering.from_pretrained("Salesforce/blip-vqa-base").to("cuda")
```

### Comparing `OneOnOne-0.6928/OneOnOne/classes.py` & `OneOnOne-0.6929/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6928/OneOnOne/classification.py` & `OneOnOne-0.6929/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6928/OneOnOne/contextdecider.py` & `OneOnOne-0.6929/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6928/OneOnOne/htmlparser.py` & `OneOnOne-0.6929/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6928/OneOnOne/questionanswer.py` & `OneOnOne-0.6929/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6928/OneOnOne/sampling.py` & `OneOnOne-0.6929/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6928/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6929/OneOnOne.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6928
+Version: 0.6929
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6928/PKG-INFO` & `OneOnOne-0.6929/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6928
+Version: 0.6929
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6928/README.md` & `OneOnOne-0.6929/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 ```python
 from OneOnOne import HTMLparser
 from OneOnOne import QuestionAnswer
 
 parser=HTMLparser(list_of_context_words)
 text=parser.get_context_text()
 
-qa=QuestionAnswer(text,"bert")
+qa=QuestionAnswer(text,"roberta")
 qa.ask()
 ```
 
 
 <h4 align="center">____________________________________________________________________________</h4>
```

#### html2text {}

```diff
@@ -38,15 +38,15 @@
 ```python from OneOnOne import ContextDecider decider=ContextDecider
 (dataset="tinyimagenet", model_type="efficientnetb6", samplingtype="none",
 threshold=0.4) list_of_context_words=decider.decide_context() ```
   If you want your predicted class(es) of the input image to be used as the
   context for your chatbot, simply run,
 ```python from OneOnOne import HTMLparser from OneOnOne import QuestionAnswer
 parser=HTMLparser(list_of_context_words) text=parser.get_context_text()
-qa=QuestionAnswer(text,"bert") qa.ask() ```
+qa=QuestionAnswer(text,"roberta") qa.ask() ```
                                       ***
  ____________________________________________________________________________
                                       ***
 This library is being actively updated and new features are being added
 frequently. New datasets and pre-trained models will be updated soon. Any bugs
 detected will be fixed asap. Feel free to share your feedback! I would really
 appreciate it! â¤ï¸ï¸
```

### Comparing `OneOnOne-0.6928/setup.py` & `OneOnOne-0.6929/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6928
+VERSION=0.6929
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

