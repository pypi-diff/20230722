# Comparing `tmp/OneOnOne-0.693.tar.gz` & `tmp/OneOnOne-0.6931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.693.tar", last modified: Sat Jul 22 17:17:45 2023, max compression
+gzip compressed data, was "OneOnOne-0.6931.tar", last modified: Sat Jul 22 17:28:35 2023, max compression
```

## Comparing `OneOnOne-0.693.tar` & `OneOnOne-0.6931.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:17:45.728390 OneOnOne-0.693/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.693/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:17:45.724656 OneOnOne-0.693/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    51744 2023-07-22 17:17:21.000000 OneOnOne-0.693/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.693/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.693/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.693/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.693/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.693/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.693/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:17:45.727594 OneOnOne-0.693/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-22 17:17:45.728005 OneOnOne-0.693/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3366 2023-07-22 16:02:47.000000 OneOnOne-0.693/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 17:17:45.728501 OneOnOne-0.693/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 17:17:39.000000 OneOnOne-0.693/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:28:35.263556 OneOnOne-0.6931/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6931/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:28:35.258289 OneOnOne-0.6931/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    51818 2023-07-22 17:28:25.000000 OneOnOne-0.6931/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6931/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6931/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6931/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6931/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6931/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6931/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:28:35.262459 OneOnOne-0.6931/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 17:28:35.000000 OneOnOne-0.6931/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 17:28:35.263104 OneOnOne-0.6931/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3366 2023-07-22 16:02:47.000000 OneOnOne-0.6931/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 17:28:35.263674 OneOnOne-0.6931/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 17:21:32.000000 OneOnOne-0.6931/setup.py
```

### Comparing `OneOnOne-0.693/LICENSE` & `OneOnOne-0.6931/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.693/OneOnOne/__init__.py` & `OneOnOne-0.6931/OneOnOne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1023,15 +1023,15 @@
             img = Image.open(os.getcwd()+f"{path}")
             img.show()
             img = iio.imread(os.getcwd()+f"{path}")
             processed_image = preprocess_image_input(img)
             self.pred = self.contextmodel.model.predict(processed_image)
         else:
             # random.randint(1, 3000)
-            self.pred = self.contextmodel.model.predict_generator(self.val_it, 1)
+            self.pred = self.contextmodel.model.predict_generator(self.val_it, random.randint(1, 16))
 
     def preprocess_image_input(self,input_images):
         if self.model_type=="efficientnetb6":
             input_images = input_images.astype('float32')
             output_ims = tf.keras.applications.efficientnet.preprocess_input(input_images)
 
         return output_ims
@@ -1128,18 +1128,18 @@
         print("Done.")
 
     def get_dataset(self):
 
         if self.dataset == "tinyimagenet":
             train_it = self.datagen.flow_from_directory(os.getcwd() + '/tiny-imagenet-200/train',
                                                         batch_size=self.batch_size, subset="training",
-                                                        shuffle=self.shuffle_bool)
+                                                        shuffle=self.shuffle_bool,seed=random.randint(1,100))
             val_it = self.datagen.flow_from_directory(os.getcwd() + '/tiny-imagenet-200/train',
                                                       batch_size=self.batch_size,
-                                                      subset="validation", shuffle=self.shuffle_bool)
+                                                      subset="validation", shuffle=self.shuffle_bool,seed=random.randint(1,100))
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
             # print(number_of_train_samples)
             # print(number_of_val_samples)
```

### Comparing `OneOnOne-0.693/OneOnOne/classes.py` & `OneOnOne-0.6931/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.693/OneOnOne/classification.py` & `OneOnOne-0.6931/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.693/OneOnOne/contextdecider.py` & `OneOnOne-0.6931/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.693/OneOnOne/htmlparser.py` & `OneOnOne-0.6931/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.693/OneOnOne/questionanswer.py` & `OneOnOne-0.6931/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.693/OneOnOne/sampling.py` & `OneOnOne-0.6931/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.693/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6931/OneOnOne.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.693
+Version: 0.6931
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.693/PKG-INFO` & `OneOnOne-0.6931/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.693
+Version: 0.6931
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.693/README.md` & `OneOnOne-0.6931/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.693/setup.py` & `OneOnOne-0.6931/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6930
+VERSION=0.6931
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

