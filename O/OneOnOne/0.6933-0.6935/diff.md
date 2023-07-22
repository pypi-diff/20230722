# Comparing `tmp/OneOnOne-0.6933.tar.gz` & `tmp/OneOnOne-0.6935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6933.tar", last modified: Sat Jul 22 17:57:55 2023, max compression
+gzip compressed data, was "OneOnOne-0.6935.tar", last modified: Sat Jul 22 18:09:39 2023, max compression
```

## Comparing `OneOnOne-0.6933.tar` & `OneOnOne-0.6935.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:57:55.036790 OneOnOne-0.6933/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6933/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:57:55.032858 OneOnOne-0.6933/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    52489 2023-07-22 17:57:50.000000 OneOnOne-0.6933/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6933/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6933/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6933/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6933/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6933/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6933/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 17:57:55.035899 OneOnOne-0.6933/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 17:57:54.000000 OneOnOne-0.6933/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 17:57:54.000000 OneOnOne-0.6933/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 17:57:54.000000 OneOnOne-0.6933/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 17:57:54.000000 OneOnOne-0.6933/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 17:57:54.000000 OneOnOne-0.6933/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 17:57:55.036309 OneOnOne-0.6933/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3366 2023-07-22 16:02:47.000000 OneOnOne-0.6933/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 17:57:55.036957 OneOnOne-0.6933/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1941 2023-07-22 17:57:50.000000 OneOnOne-0.6933/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 18:09:39.348059 OneOnOne-0.6935/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6935/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 18:09:39.341598 OneOnOne-0.6935/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    52518 2023-07-22 18:09:34.000000 OneOnOne-0.6935/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6935/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6935/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6935/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6935/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6935/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6935/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-22 18:09:39.346548 OneOnOne-0.6935/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      139 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-22 18:09:39.000000 OneOnOne-0.6935/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-22 18:09:39.347300 OneOnOne-0.6935/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3366 2023-07-22 16:02:47.000000 OneOnOne-0.6935/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-22 18:09:39.348303 OneOnOne-0.6935/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1941 2023-07-22 18:09:34.000000 OneOnOne-0.6935/setup.py
```

### Comparing `OneOnOne-0.6933/LICENSE` & `OneOnOne-0.6935/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6933/OneOnOne/__init__.py` & `OneOnOne-0.6935/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1016,31 +1016,31 @@
 
         self.train_it, self.val_it = self.get_dataset()
 
         if self.load:
             path=input("Please input the model's path/name in the current directory (str):     ")
             self.contextmodel=load_model(os.getcwd()+path)
         else:
-            check=False
-            for file in os.listdir(os.getcwd()):
-                if file.endswith(f'{self.model_type}_{self.dataset}_{self.samplingtype}.zip'):
-                    zip_file = ZipFile(file)
-                    zip_file.extractall(os.getcwd() + f'/models_to_load/')
-                    self.contextmodel = load_model(os.getcwd() + f'/models_to_load/'+f'{self.model_type}_{self.dataset}_{self.samplingtype}')
-                    check=True
-            if not check:
-                self.contextmodel = PretrainedModel(model_type=self.model_type, dataset=self.dataset,
+            # check=False
+            # for file in os.listdir(os.getcwd()):
+            #     if file.endswith(f'{self.model_type}_{self.dataset}_{self.samplingtype}.zip'):
+            #         zip_file = ZipFile(file)
+            #         zip_file.extractall(os.getcwd() + f'/models_to_load/')
+            #         self.contextmodel = load_model(os.getcwd() + f'/models_to_load/'+f'{self.model_type}_{self.dataset}_{self.samplingtype}')
+            #         check=True
+            # if not check:
+            self.contextmodel = PretrainedModel(model_type=self.model_type, dataset=self.dataset,
                                           samplingtype=self.samplingtype)
         # self.pretrained.model
         if self.user_input:
             path=input("Please enter image path in the current directory (str):    ")
             img = Image.open(os.getcwd()+f"{path}")
             img.show()
             img = iio.imread(os.getcwd()+f"{path}")
-            processed_image = preprocess_image_input(img)
+            processed_image = self.preprocess_image_input(img)
             self.pred = self.contextmodel.model.predict(processed_image)
         else:
             # random.randint(1, 3000)
             self.pred = self.contextmodel.model.predict_generator(self.val_it, random.randint(1, 16))
 
     def preprocess_image_input(self,input_images):
         if self.model_type=="efficientnetb6":
@@ -1119,22 +1119,22 @@
             output = output + b
 
         return output
 
     def download_dataset(self):
 
         print("Extracting...")
-        if not 'tiny-imagenet-200.zip' in os.listdir(os.getcwd()):
+        if not 'tiny-imagenet-200' in os.listdir(os.getcwd()):
             url = 'http://cs231n.stanford.edu/tiny-imagenet-200.zip'
             tiny_imgdataset = wget.download(url, out=os.getcwd())
 
-        for file in os.listdir(os.getcwd()):
-            if file.endswith("tiny-imagenet-200.zip"):
-                zip_file = ZipFile(file)
-                zip_file.extractall()
+            for file in os.listdir(os.getcwd()):
+                if file.endswith("tiny-imagenet-200.zip"):
+                    zip_file = ZipFile(file)
+                    zip_file.extractall()
 
         try:
             os.system("gdown --id 1JgRlpet7-P-x7Exweb8HC-zUcYsF5fGN")
         except:
             os.system("!gdown --id 1JgRlpet7-P-x7Exweb8HC-zUcYsF5fGN")
 
         print("Done.")
```

### Comparing `OneOnOne-0.6933/OneOnOne/classes.py` & `OneOnOne-0.6935/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6933/OneOnOne/classification.py` & `OneOnOne-0.6935/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6933/OneOnOne/contextdecider.py` & `OneOnOne-0.6935/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6933/OneOnOne/htmlparser.py` & `OneOnOne-0.6935/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6933/OneOnOne/questionanswer.py` & `OneOnOne-0.6935/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6933/OneOnOne/sampling.py` & `OneOnOne-0.6935/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6933/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6935/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6933
+Version: 0.6935
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6933/PKG-INFO` & `OneOnOne-0.6935/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6933
+Version: 0.6935
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6933/README.md` & `OneOnOne-0.6935/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6933/setup.py` & `OneOnOne-0.6935/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6933
+VERSION=0.6935
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

