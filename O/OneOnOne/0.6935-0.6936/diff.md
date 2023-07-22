# Comparing `tmp/OneOnOne-0.6935.tar.gz` & `tmp/OneOnOne-0.6936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6935.tar", last modified: Sat Jul 22 18:09:39 2023, max compression
+gzip compressed data, was "OneOnOne-0.6936.tar", last modified: Sat Jul 22 18:19:34 2023, max compression
```

## Comparing `OneOnOne-0.6935.tar` & `OneOnOne-0.6936.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 18:09:39.348059 OneOnOne-0.6935/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6935/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 18:09:39.341598 OneOnOne-0.6935/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    52518 2023-07-22 18:09:34.000000 OneOnOne-0.6935/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6935/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6935/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6935/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6935/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6935/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6935/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 18:09:39.346548 OneOnOne-0.6935/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 18:09:39.347300 OneOnOne-0.6935/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3366 2023-07-22 16:02:47.000000 OneOnOne-0.6935/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 18:09:39.348303 OneOnOne-0.6935/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1941 2023-07-22 18:09:34.000000 OneOnOne-0.6935/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 18:19:34.206036 OneOnOne-0.6936/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6936/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 18:19:34.200038 OneOnOne-0.6936/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    52559 2023-07-22 18:19:28.000000 OneOnOne-0.6936/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6936/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6936/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6936/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6936/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6936/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6936/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 18:19:34.205198 OneOnOne-0.6936/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 18:19:34.000000 OneOnOne-0.6936/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 18:19:34.000000 OneOnOne-0.6936/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 18:19:34.000000 OneOnOne-0.6936/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 18:19:34.000000 OneOnOne-0.6936/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 18:19:34.000000 OneOnOne-0.6936/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 18:19:34.205657 OneOnOne-0.6936/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3366 2023-07-22 16:02:47.000000 OneOnOne-0.6936/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 18:19:34.206147 OneOnOne-0.6936/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1941 2023-07-22 18:19:28.000000 OneOnOne-0.6936/setup.py
```

### Comparing `OneOnOne-0.6935/LICENSE` & `OneOnOne-0.6936/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6935/OneOnOne/__init__.py` & `OneOnOne-0.6936/OneOnOne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,21 @@
 
 
         for file in os.listdir(os.getcwd()):
             if file.endswith(f"{self.model_name}.zip"):
                 zip_file = ZipFile(file)
                 zip_file.extractall(os.getcwd() + f'/models_to_load/')
 
+    def get_model(self):
+
         self.model=load_model(self.path)
         self.model.summary()
 
+        return self.model
+
 
 class Classification:
     def __init__(self, model_type="resnet50", batch_size=16, epochs=250, dataset="cifar10", validation_split=0.3, shuffle_bool=True, early_stopping_patience=10, lr_reducer_patience=10):
         warnings.filterwarnings("ignore")
 
         self.model_type = model_type.lower()
         self.date=datetime.datetime.now()
@@ -1033,18 +1037,18 @@
         # self.pretrained.model
         if self.user_input:
             path=input("Please enter image path in the current directory (str):    ")
             img = Image.open(os.getcwd()+f"{path}")
             img.show()
             img = iio.imread(os.getcwd()+f"{path}")
             processed_image = self.preprocess_image_input(img)
-            self.pred = self.contextmodel.model.predict(processed_image)
+            self.pred = self.contextmodel.predict(processed_image)
         else:
             # random.randint(1, 3000)
-            self.pred = self.contextmodel.model.predict_generator(self.val_it, random.randint(1, 16))
+            self.pred = self.contextmodel.predict_generator(self.val_it, random.randint(1, 16))
 
     def preprocess_image_input(self,input_images):
         if self.model_type=="efficientnetb6":
             input_images = input_images.astype('float32')
             output_ims = tf.keras.applications.efficientnet.preprocess_input(input_images)
 
         return output_ims
```

### Comparing `OneOnOne-0.6935/OneOnOne/classes.py` & `OneOnOne-0.6936/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6935/OneOnOne/classification.py` & `OneOnOne-0.6936/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6935/OneOnOne/contextdecider.py` & `OneOnOne-0.6936/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6935/OneOnOne/htmlparser.py` & `OneOnOne-0.6936/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6935/OneOnOne/questionanswer.py` & `OneOnOne-0.6936/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6935/OneOnOne/sampling.py` & `OneOnOne-0.6936/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6935/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6936/OneOnOne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6935
+Version: 0.6936
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6935/PKG-INFO` & `OneOnOne-0.6936/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6935
+Version: 0.6936
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6935/README.md` & `OneOnOne-0.6936/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6935/setup.py` & `OneOnOne-0.6936/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6935
+VERSION=0.6936
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

