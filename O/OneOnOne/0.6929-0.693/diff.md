# Comparing `tmp/OneOnOne-0.6929.tar.gz` & `tmp/OneOnOne-0.693.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6929.tar", last modified: Sat Jul 22 14:20:59 2023, max compression
+gzip compressed data, was "OneOnOne-0.693.tar", last modified: Sat Jul 22 17:17:45 2023, max compression
```

## Comparing `OneOnOne-0.6929.tar` & `OneOnOne-0.693.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 14:20:59.960933 OneOnOne-0.6929/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6929/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 14:20:59.956785 OneOnOne-0.6929/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    51728 2023-07-22 14:20:51.000000 OneOnOne-0.6929/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6929/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6929/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6929/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6929/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6929/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6929/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 14:20:59.960075 OneOnOne-0.6929/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 14:20:59.000000 OneOnOne-0.6929/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 14:20:59.960508 OneOnOne-0.6929/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3359 2023-07-22 14:03:15.000000 OneOnOne-0.6929/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 14:20:59.961085 OneOnOne-0.6929/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 14:19:56.000000 OneOnOne-0.6929/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:17:45.728390 OneOnOne-0.693/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.693/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:17:45.724656 OneOnOne-0.693/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    51744 2023-07-22 17:17:21.000000 OneOnOne-0.693/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.693/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.693/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.693/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.693/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.693/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.693/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:17:45.727594 OneOnOne-0.693/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 17:17:45.000000 OneOnOne-0.693/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-22 17:17:45.728005 OneOnOne-0.693/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3366 2023-07-22 16:02:47.000000 OneOnOne-0.693/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 17:17:45.728501 OneOnOne-0.693/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1942 2023-07-22 17:17:39.000000 OneOnOne-0.693/setup.py
```

### Comparing `OneOnOne-0.6929/LICENSE` & `OneOnOne-0.693/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6929/OneOnOne/__init__.py` & `OneOnOne-0.693/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1022,15 +1022,16 @@
             path=input("Please enter image path in the current directory (str):    ")
             img = Image.open(os.getcwd()+f"{path}")
             img.show()
             img = iio.imread(os.getcwd()+f"{path}")
             processed_image = preprocess_image_input(img)
             self.pred = self.contextmodel.model.predict(processed_image)
         else:
-            self.pred = self.contextmodel.model.predict_generator(self.val_it, random.randint(1, 3000))
+            # random.randint(1, 3000)
+            self.pred = self.contextmodel.model.predict_generator(self.val_it, 1)
 
     def preprocess_image_input(self,input_images):
         if self.model_type=="efficientnetb6":
             input_images = input_images.astype('float32')
             output_ims = tf.keras.applications.efficientnet.preprocess_input(input_images)
 
         return output_ims
```

### Comparing `OneOnOne-0.6929/OneOnOne/classes.py` & `OneOnOne-0.693/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6929/OneOnOne/classification.py` & `OneOnOne-0.693/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6929/OneOnOne/contextdecider.py` & `OneOnOne-0.693/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6929/OneOnOne/htmlparser.py` & `OneOnOne-0.693/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6929/OneOnOne/questionanswer.py` & `OneOnOne-0.693/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6929/OneOnOne/sampling.py` & `OneOnOne-0.693/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6929/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.693/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6929
+Version: 0.693
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6929/PKG-INFO` & `OneOnOne-0.693/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6929
+Version: 0.693
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6929/README.md` & `OneOnOne-0.693/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <a href="https://pypi.org/project/OneOnOne/0.6896/" target="_blank">
   </a>
 </p>
 
 <h3 align="center"><span style="color:#FFC0CB">Your one-stop destination to utilize image-classification models with just one line of code.</span></h3>
 
 <h4 align="center">
-A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc.
+A python library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc.
 You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, don't worry! This library has got you covered. Along with that for simple-bridging of NLP with Image Classification and utilization of basic use-cases of NLP frameworks, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about, and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset.
 </h4>
 
 <h4 align="center">____________________________________________________________________________</h4>
 
 <dl>
   <dt><span style="color:#FFC0CB">How to import the library?</span></dt>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                           ****** OneOnOne ð ******
 **** Your one-stop destination to utilize image-classification models with just
                             one line of code. ****
-  *** A library meant to simplify your life by providing you with pre-trained
-   models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for
-  training your own models from scratch by just tweaking a few values. If you
+  *** A python library meant to simplify your life by providing you with pre-
+ trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt
+for training your own models from scratch by just tweaking a few values. If you
  want to try popular active-learning sampling methods on image classification,
   don't worry! This library has got you covered. Along with that for simple-
 bridging of NLP with Image Classification and utilization of basic use-cases of
    NLP frameworks, we have context-deciders, HTML parsers and simple chatbot
   object classes, to create an interface similar to Google Lens. You input an
 image or item that you are curious about, and you can ask one-on-one questions
 from the chatbot. This is made possible by using the tiny imagenet dataset. ***
```

### Comparing `OneOnOne-0.6929/setup.py` & `OneOnOne-0.693/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6929
+VERSION=0.6930
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

