# Comparing `tmp/OneOnOne-0.6914.tar.gz` & `tmp/OneOnOne-0.6915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6914.tar", last modified: Sat Jul 22 03:17:25 2023, max compression
+gzip compressed data, was "OneOnOne-0.6915.tar", last modified: Sat Jul 22 03:26:27 2023, max compression
```

## Comparing `OneOnOne-0.6914.tar` & `OneOnOne-0.6915.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:17:25.583808 OneOnOne-0.6914/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6914/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:17:25.573972 OneOnOne-0.6914/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    48498 2023-07-22 03:17:08.000000 OneOnOne-0.6914/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6914/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6914/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6914/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6914/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6914/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6914/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:17:25.583000 OneOnOne-0.6914/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:17:25.000000 OneOnOne-0.6914/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 03:17:25.000000 OneOnOne-0.6914/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 03:17:25.000000 OneOnOne-0.6914/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 03:17:25.000000 OneOnOne-0.6914/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 03:17:25.000000 OneOnOne-0.6914/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:17:25.583435 OneOnOne-0.6914/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6914/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 03:17:25.583935 OneOnOne-0.6914/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 03:17:14.000000 OneOnOne-0.6914/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:26:27.946700 OneOnOne-0.6915/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6915/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:26:27.942234 OneOnOne-0.6915/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    49276 2023-07-22 03:26:23.000000 OneOnOne-0.6915/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6915/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6915/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6915/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6915/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6915/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6915/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 03:26:27.945858 OneOnOne-0.6915/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:26:27.000000 OneOnOne-0.6915/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 03:26:27.000000 OneOnOne-0.6915/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 03:26:27.000000 OneOnOne-0.6915/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 03:26:27.000000 OneOnOne-0.6915/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 03:26:27.000000 OneOnOne-0.6915/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 03:26:27.946300 OneOnOne-0.6915/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3356 2023-07-19 17:38:43.000000 OneOnOne-0.6915/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 03:26:27.946817 OneOnOne-0.6915/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 03:26:23.000000 OneOnOne-0.6915/setup.py
```

### Comparing `OneOnOne-0.6914/LICENSE` & `OneOnOne-0.6915/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6914/OneOnOne/__init__.py` & `OneOnOne-0.6915/OneOnOne/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,14 +288,15 @@
                                        min_lr=0.5e-6)
 
         callbacks = [checkpoint, lr_reducer, lr_scheduler, early_stopping]
 
         return callbacks
 
     def get_datagen(self):
+
         datagen = ImageDataGenerator(
             featurewise_center=False,
             samplewise_center=False,
             featurewise_std_normalization=False,
             samplewise_std_normalization=False,
             zca_whitening=False,
             zca_epsilon=1e-06,
@@ -412,17 +413,17 @@
         return keys, total_list_parameter_history
 
     def evaluate(self):
         loss, accuracy = self.model.evaluate(self.val_it, batch_size=self.batch_size, verbose=1)
 
 
 class Sampling:
-    def __init__(self, samplingtype, dataset="cifar10", model_type = "resnet50", goal=99, jump=5000, first_data_samples=10000, batch_size = 16, epochs = 250, shuffle_bool = True, early_stopping_patience = 10, lr_reducer_patience = 10):
+    def __init__(self, samplingtype, dataset="cifar10", model_type = "resnet50", goal=99, jump=5000, validation_split=0.3, first_data_samples=10000, batch_size = 16, epochs = 250, shuffle_bool = True, early_stopping_patience = 10, lr_reducer_patience = 10):
 
-        self.validation_split=0
+        self.validation_split=validation_split
         self.model_type = model_type.lower()
         self.epochs=epochs
         self.jump = jump
         self.samplingtype = samplingtype.lower()
         self.goal = goal
         self.shuffle_bool = shuffle
         self.batch_size = batch_size
@@ -578,19 +579,14 @@
                                        min_lr=0.5e-6)
 
         callbacks = [checkpoint, lr_reducer, lr_scheduler, early_stopping]
 
         return callbacks
 
     def get_datagen(self):
-        
-        if self.dataset=="tinyimagenet":
-            self.validation_split=input("Validation split (example - 0.3):   ")
-        else:
-            pass
             
         datagen = ImageDataGenerator(
             featurewise_center=False,
             samplewise_center=False,
             featurewise_std_normalization=False,
             samplewise_std_normalization=False,
             zca_whitening=False,
@@ -844,15 +840,14 @@
                 pickle.dump(history.history, file_pi)
             print("saved.")
 
 
 
     def get_iterations(self):
 
-
         eval_metrics=[0,0]
 
         num=0
         batch_size_data = [0]
         acuracy_data = [0]
         epoch_data = []
         history_data = []
@@ -975,19 +970,22 @@
             text_for_one_word = self.produce_text(word)
             full_context = full_context + text_for_one_word[3:-1]
 
         return full_context
 
 
 class ContextDecider:
-    def __init__(self, dataset="tinyimagenet", model_type="efficientnetb6", samplingtype="none", threshold=0.2):
+    def __init__(self, dataset="tinyimagenet", model_type="efficientnetb6", samplingtype="none", validation_split=0.3, threshold=0.2):
+
         self.dataset = dataset.lower()
         self.model_type = model_type.lower()
+        self.validation_split=validation_split
         self.threshold = threshold
         self.samplingtype = samplingtype
+        self.datagen = self.get_datagen()
 
         if self.dataset == "cifar10" or self.dataset == "mnist":
             self.output_layer_classes = 10
             self.input_shape = (224, 224, 3)
 
         elif self.dataset == "cifar100":
             self.output_layer_classes = 100
@@ -1005,14 +1003,40 @@
         self.train_it, self.val_it = self.get_dataset()
 
         self.pretrained = PretrainedModel(model_type=self.model_type, dataset=self.dataset,
                                           samplingtype=self.samplingtype)
         # self.pretrained.model
         self.pred = self.pretrained.model.predict_generator(self.val_it, 1)
 
+    def get_datagen(self):
+
+        datagen = ImageDataGenerator(
+            featurewise_center=False,
+            samplewise_center=False,
+            featurewise_std_normalization=False,
+            samplewise_std_normalization=False,
+            zca_whitening=False,
+            zca_epsilon=1e-06,
+            rotation_range=30,
+            width_shift_range=0.1,
+            height_shift_range=0.1,
+            shear_range=0.,
+            zoom_range=0.,
+            channel_shift_range=0.,
+            fill_mode='nearest',
+            cval=0.,
+            horizontal_flip=True,
+            vertical_flip=False,
+            rescale=None,
+            preprocessing_function=None,
+            data_format=None,
+            validation_split=self.validation_split)
+
+        return datagen
+
     def decide_context(self):
 
         predicted_list = []
         classes_prob_list = []
         prediction_index = []
         final_classes = []
```

### Comparing `OneOnOne-0.6914/OneOnOne/classes.py` & `OneOnOne-0.6915/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6914/OneOnOne/classification.py` & `OneOnOne-0.6915/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6914/OneOnOne/contextdecider.py` & `OneOnOne-0.6915/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6914/OneOnOne/htmlparser.py` & `OneOnOne-0.6915/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6914/OneOnOne/questionanswer.py` & `OneOnOne-0.6915/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6914/OneOnOne/sampling.py` & `OneOnOne-0.6915/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6914/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6915/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6914
+Version: 0.6915
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6914/PKG-INFO` & `OneOnOne-0.6915/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6914
+Version: 0.6915
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6914/README.md` & `OneOnOne-0.6915/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6914/setup.py` & `OneOnOne-0.6915/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6914
+VERSION=0.6915
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

