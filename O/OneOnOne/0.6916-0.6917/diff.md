# Comparing `tmp/OneOnOne-0.6916.tar.gz` & `tmp/OneOnOne-0.6917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6916.tar", last modified: Sat Jul 22 03:35:44 2023, max compression
+gzip compressed data, was "OneOnOne-0.6917.tar", last modified: Sat Jul 22 03:39:20 2023, max compression
```

## Comparing `OneOnOne-0.6916.tar` & `OneOnOne-0.6917.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:35:44.574562 OneOnOne-0.6916/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6916/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:35:44.570558 OneOnOne-0.6916/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    49625 2023-07-22 03:35:34.000000 OneOnOne-0.6916/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6916/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6916/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6916/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6916/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6916/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6916/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:35:44.573715 OneOnOne-0.6916/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:35:44.000000 OneOnOne-0.6916/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 03:35:44.000000 OneOnOne-0.6916/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 03:35:44.000000 OneOnOne-0.6916/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 03:35:44.000000 OneOnOne-0.6916/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 03:35:44.000000 OneOnOne-0.6916/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:35:44.574170 OneOnOne-0.6916/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6916/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 03:35:44.574703 OneOnOne-0.6916/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 03:35:40.000000 OneOnOne-0.6916/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:39:20.955252 OneOnOne-0.6917/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6917/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:39:20.950358 OneOnOne-0.6917/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    49631 2023-07-22 03:39:16.000000 OneOnOne-0.6917/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6917/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6917/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6917/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6917/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6917/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6917/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:39:20.953910 OneOnOne-0.6917/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:39:20.000000 OneOnOne-0.6917/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 03:39:20.000000 OneOnOne-0.6917/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 03:39:20.000000 OneOnOne-0.6917/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 03:39:20.000000 OneOnOne-0.6917/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 03:39:20.000000 OneOnOne-0.6917/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:39:20.954570 OneOnOne-0.6917/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6917/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 03:39:20.955400 OneOnOne-0.6917/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 03:39:16.000000 OneOnOne-0.6917/setup.py
```

### Comparing `OneOnOne-0.6916/LICENSE` & `OneOnOne-0.6917/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6916/OneOnOne/__init__.py` & `OneOnOne-0.6917/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,17 +335,17 @@
             os.system("!gdown --id 1JgRlpet7-P-x7Exweb8HC-zUcYsF5fGN")
 
         print("Done.")
 
     def get_dataset(self):
 
         if self.dataset=="tinyimagenet":
-            train_it = self.datagen.flow_from_directory(os.getcwd()+'tiny-imagenet-200/train',
+            train_it = self.datagen.flow_from_directory(os.getcwd()+'/tiny-imagenet-200/train',
                                                         batch_size=self.batch_size, subset="training", shuffle=self.shuffle_bool)
-            val_it = self.datagen.flow_from_directory(os.getcwd()+'tiny-imagenet-200/train', batch_size=self.batch_size,
+            val_it = self.datagen.flow_from_directory(os.getcwd()+'/tiny-imagenet-200/train', batch_size=self.batch_size,
                                                       subset="validation", shuffle=self.shuffle_bool)
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
             print(number_of_train_samples)
@@ -627,18 +627,18 @@
 
 
         print("Done.")
 
     def get_dataset(self):
 
         if self.dataset == "tinyimagenet":
-            train_it = self.datagen.flow_from_directory(os.getcwd()+'tiny-imagenet-200/train',
+            train_it = self.datagen.flow_from_directory(os.getcwd()+'/tiny-imagenet-200/train',
                                                         batch_size=self.batch_size, subset="training",
                                                         shuffle=self.shuffle_bool)
-            val_it = self.datagen.flow_from_directory(os.getcwd()+'tiny-imagenet-200/train',
+            val_it = self.datagen.flow_from_directory(os.getcwd()+'/tiny-imagenet-200/train',
                                                       batch_size=self.batch_size,
                                                       subset="validation", shuffle=self.shuffle_bool)
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
@@ -1102,18 +1102,18 @@
             os.system("!gdown --id 1JgRlpet7-P-x7Exweb8HC-zUcYsF5fGN")
 
         print("Done.")
 
     def get_dataset(self):
 
         if self.dataset == "tinyimagenet":
-            train_it = self.datagen.flow_from_directory(os.getcwd() + 'tiny-imagenet-200/train',
+            train_it = self.datagen.flow_from_directory(os.getcwd() + '/tiny-imagenet-200/train',
                                                         batch_size=self.batch_size, subset="training",
                                                         shuffle=self.shuffle_bool)
-            val_it = self.datagen.flow_from_directory(os.getcwd() + 'tiny-imagenet-200/train',
+            val_it = self.datagen.flow_from_directory(os.getcwd() + '/tiny-imagenet-200/train',
                                                       batch_size=self.batch_size,
                                                       subset="validation", shuffle=self.shuffle_bool)
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
```

### Comparing `OneOnOne-0.6916/OneOnOne/classes.py` & `OneOnOne-0.6917/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6916/OneOnOne/classification.py` & `OneOnOne-0.6917/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6916/OneOnOne/contextdecider.py` & `OneOnOne-0.6917/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6916/OneOnOne/htmlparser.py` & `OneOnOne-0.6917/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6916/OneOnOne/questionanswer.py` & `OneOnOne-0.6917/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6916/OneOnOne/sampling.py` & `OneOnOne-0.6917/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6916/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6917/OneOnOne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6916
+Version: 0.6917
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6916/PKG-INFO` & `OneOnOne-0.6917/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6916
+Version: 0.6917
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6916/README.md` & `OneOnOne-0.6917/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6916/setup.py` & `OneOnOne-0.6917/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6916
+VERSION=0.6917
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

