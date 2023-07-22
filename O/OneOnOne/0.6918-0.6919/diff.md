# Comparing `tmp/OneOnOne-0.6918.tar.gz` & `tmp/OneOnOne-0.6919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6918.tar", last modified: Sat Jul 22 03:57:17 2023, max compression
+gzip compressed data, was "OneOnOne-0.6919.tar", last modified: Sat Jul 22 04:04:31 2023, max compression
```

## Comparing `OneOnOne-0.6918.tar` & `OneOnOne-0.6919.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:57:17.569314 OneOnOne-0.6918/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6918/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:57:17.564906 OneOnOne-0.6918/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    49668 2023-07-22 03:55:39.000000 OneOnOne-0.6918/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6918/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6918/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6918/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6918/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6918/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6918/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:57:17.568462 OneOnOne-0.6918/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:57:17.000000 OneOnOne-0.6918/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 03:57:17.000000 OneOnOne-0.6918/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 03:57:17.000000 OneOnOne-0.6918/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 03:57:17.000000 OneOnOne-0.6918/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 03:57:17.000000 OneOnOne-0.6918/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:57:17.568926 OneOnOne-0.6918/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6918/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 03:57:17.569426 OneOnOne-0.6918/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 03:57:11.000000 OneOnOne-0.6918/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 04:04:31.881960 OneOnOne-0.6919/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6919/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 04:04:31.877540 OneOnOne-0.6919/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    49685 2023-07-22 04:04:17.000000 OneOnOne-0.6919/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6919/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6919/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6919/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6919/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6919/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6919/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 04:04:31.881120 OneOnOne-0.6919/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 04:04:31.000000 OneOnOne-0.6919/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 04:04:31.000000 OneOnOne-0.6919/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 04:04:31.000000 OneOnOne-0.6919/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 04:04:31.000000 OneOnOne-0.6919/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 04:04:31.000000 OneOnOne-0.6919/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 04:04:31.881565 OneOnOne-0.6919/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6919/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 04:04:31.882073 OneOnOne-0.6919/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 04:04:27.000000 OneOnOne-0.6919/setup.py
```

### Comparing `OneOnOne-0.6918/LICENSE` & `OneOnOne-0.6919/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6918/OneOnOne/__init__.py` & `OneOnOne-0.6919/OneOnOne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,16 +638,16 @@
                                                       batch_size=self.batch_size,
                                                       subset="validation", shuffle=self.shuffle_bool)
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
-            print(number_of_train_samples)
-            print(number_of_val_samples)
+            # print(number_of_train_samples)
+            # print(number_of_val_samples)
 
         else:
 
             shuffle_random_token = input("Do you want to shuffle the training data? (yes/no):  ")
 
             if shuffle_random_token.lower() == "yes":
                 seed_token = input("Enter random seed (int):  ")
@@ -1115,16 +1115,16 @@
                                                       batch_size=self.batch_size,
                                                       subset="validation", shuffle=self.shuffle_bool)
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
-            print(number_of_train_samples)
-            print(number_of_val_samples)
+            # print(number_of_train_samples)
+            # print(number_of_val_samples)
         else:
             if self.dataset == "cifar10":
                 classes = ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']
                 num_classes = len(classes)
                 (training_images, training_labels), (
                     validation_images, validation_labels) = tf.keras.datasets.cifar10.load_data()
 
@@ -1197,15 +1197,15 @@
 
     def question_answer(self, question):
 
         # input_ids = self.tokenizer.encode(question, self.context)
 
         # tokens = self.tokenizer.convert_ids_to_tokens(input_ids)
 
-        tokens = token.tokenize(text, max_length=MAX_TOKENS, truncation=True)
+        tokens = self.tokenizer.tokenize(text, max_length=MAX_TOKENS, truncation=True)
 
         sep_idx = input_ids.index(self.tokenizer.sep_token_id)
 
         num_seg_a = sep_idx + 1
 
         num_seg_b = len(input_ids) - num_seg_a
```

### Comparing `OneOnOne-0.6918/OneOnOne/classes.py` & `OneOnOne-0.6919/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6918/OneOnOne/classification.py` & `OneOnOne-0.6919/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6918/OneOnOne/contextdecider.py` & `OneOnOne-0.6919/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6918/OneOnOne/htmlparser.py` & `OneOnOne-0.6919/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6918/OneOnOne/questionanswer.py` & `OneOnOne-0.6919/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6918/OneOnOne/sampling.py` & `OneOnOne-0.6919/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6918/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6919/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6918
+Version: 0.6919
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6918/PKG-INFO` & `OneOnOne-0.6919/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6918
+Version: 0.6919
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6918/README.md` & `OneOnOne-0.6919/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6918/setup.py` & `OneOnOne-0.6919/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6918
+VERSION=0.6919
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

