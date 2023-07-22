# Comparing `tmp/OneOnOne-0.6912.tar.gz` & `tmp/OneOnOne-0.6913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6912.tar", last modified: Sat Jul 22 03:05:18 2023, max compression
+gzip compressed data, was "OneOnOne-0.6913.tar", last modified: Sat Jul 22 03:07:55 2023, max compression
```

## Comparing `OneOnOne-0.6912.tar` & `OneOnOne-0.6913.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:05:18.352123 OneOnOne-0.6912/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6912/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:05:18.347244 OneOnOne-0.6912/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    47957 2023-07-22 03:04:29.000000 OneOnOne-0.6912/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6912/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6912/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6912/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6912/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6912/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6912/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:05:18.351243 OneOnOne-0.6912/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:05:18.000000 OneOnOne-0.6912/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 03:05:18.000000 OneOnOne-0.6912/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 03:05:18.000000 OneOnOne-0.6912/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 03:05:18.000000 OneOnOne-0.6912/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 03:05:18.000000 OneOnOne-0.6912/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:05:18.351729 OneOnOne-0.6912/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6912/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 03:05:18.352239 OneOnOne-0.6912/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 03:04:35.000000 OneOnOne-0.6912/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:07:55.014702 OneOnOne-0.6913/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6913/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:07:55.010696 OneOnOne-0.6913/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    47957 2023-07-22 03:07:46.000000 OneOnOne-0.6913/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6913/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6913/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6913/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6913/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6913/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6913/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:07:55.013771 OneOnOne-0.6913/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:07:54.000000 OneOnOne-0.6913/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 03:07:54.000000 OneOnOne-0.6913/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 03:07:54.000000 OneOnOne-0.6913/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 03:07:54.000000 OneOnOne-0.6913/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 03:07:54.000000 OneOnOne-0.6913/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:07:55.014319 OneOnOne-0.6913/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6913/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 03:07:55.014841 OneOnOne-0.6913/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 03:07:51.000000 OneOnOne-0.6913/setup.py
```

### Comparing `OneOnOne-0.6912/LICENSE` & `OneOnOne-0.6913/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6912/OneOnOne/__init__.py` & `OneOnOne-0.6913/OneOnOne/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,16 @@
         elif self.dataset == "cifar100":
             self.output_layer_classes = 100
             self.input_shape = (224, 224, 3)
 
         elif self.dataset=="tinyimagenet":
             self.output_layer_classes = 200
             self.input_shape = (32, 32, 3)
-            from classes import i2d
             self.download_dataset()
+            from classes import i2d
 
         else:
             print("Invalid Input!")
 
         self.token=input("Train/Load?  :   ")
         self.train_it, self.val_it = self.get_dataset()
 
@@ -432,16 +432,16 @@
         self.datagen = self.get_datagen()
         if self.dataset == "cifar10" or self.dataset == "mnist":
             self.output_layer_classes = 10
             self.input_shape = (224, 224, 3)
         elif self.dataset == "tinyimagenet":
             self.output_layer_classes = 200
             self.input_shape = (32, 32, 3)
-            from classes import i2d
             self.download_dataset()
+            from classes import i2d
         else:
             print("Invalid Input!")
 
         self.train_it, self.val_it = self.get_dataset()
 
         if samplingtype== "random":
           random_num = np.random.randint(self.first_data_samples,self.X_train.shape[0],size=self.X_train.shape[0]-self.first_data_samples)
@@ -981,16 +981,16 @@
         elif self.dataset == "cifar100":
             self.output_layer_classes = 100
             self.input_shape = (224, 224, 3)
 
         elif self.dataset == "tinyimagenet":
             self.output_layer_classes = 200
             self.input_shape = (32, 32, 3)
-            from classes import i2d
             self.download_dataset()
+            from classes import i2d
 
         else:
             print("Invalid Input!")
 
         self.train_it, self.val_it = self.get_dataset()
 
         self.pretrained = PretrainedModel(model_type=self.model_type, dataset=self.dataset,
```

### Comparing `OneOnOne-0.6912/OneOnOne/classes.py` & `OneOnOne-0.6913/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6912/OneOnOne/classification.py` & `OneOnOne-0.6913/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6912/OneOnOne/contextdecider.py` & `OneOnOne-0.6913/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6912/OneOnOne/htmlparser.py` & `OneOnOne-0.6913/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6912/OneOnOne/questionanswer.py` & `OneOnOne-0.6913/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6912/OneOnOne/sampling.py` & `OneOnOne-0.6913/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6912/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6913/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6912
+Version: 0.6913
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6912/PKG-INFO` & `OneOnOne-0.6913/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6912
+Version: 0.6913
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6912/README.md` & `OneOnOne-0.6913/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6912/setup.py` & `OneOnOne-0.6913/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6912
+VERSION=0.6913
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

