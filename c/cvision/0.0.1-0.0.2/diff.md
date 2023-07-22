# Comparing `tmp/cvision-0.0.1.tar.gz` & `tmp/cvision-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvision-0.0.1.tar", last modified: Sat Jul 22 11:21:29 2023, max compression
+gzip compressed data, was "cvision-0.0.2.tar", last modified: Sat Jul 22 16:47:16 2023, max compression
```

## Comparing `cvision-0.0.1.tar` & `cvision-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 11:21:29.910356 cvision-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 cvision-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      648 2023-07-22 11:21:29.910356 cvision-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 cvision-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 11:21:29.886984 cvision-0.0.1/cvision/
--rw-rw-rw-   0        0        0       36 2023-07-22 11:17:24.000000 cvision-0.0.1/cvision/__init__.py
--rw-rw-rw-   0        0        0     2186 2023-07-22 11:16:12.000000 cvision-0.0.1/cvision/cvision.py
-drwxrwxrwx   0        0        0        0 2023-07-22 11:21:29.910356 cvision-0.0.1/cvision.egg-info/
--rw-rw-rw-   0        0        0      648 2023-07-22 11:21:29.000000 cvision-0.0.1/cvision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-07-22 11:21:29.000000 cvision-0.0.1/cvision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 11:21:29.000000 cvision-0.0.1/cvision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-22 11:21:29.000000 cvision-0.0.1/cvision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 11:21:29.910356 cvision-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-07-22 11:19:24.000000 cvision-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 16:47:16.434217 cvision-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-20 20:17:27.000000 cvision-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      648 2023-07-22 16:47:16.434217 cvision-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-20 20:16:36.000000 cvision-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 16:47:16.402974 cvision-0.0.2/cvision/
+-rw-rw-rw-   0        0        0       31 2023-07-22 16:44:59.000000 cvision-0.0.2/cvision/__init__.py
+-rw-rw-rw-   0        0        0     2331 2023-07-22 16:44:33.000000 cvision-0.0.2/cvision/cvision.py
+drwxrwxrwx   0        0        0        0 2023-07-22 16:47:16.434217 cvision-0.0.2/cvision.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-07-22 16:47:16.000000 cvision-0.0.2/cvision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-07-22 16:47:16.000000 cvision-0.0.2/cvision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 16:47:16.000000 cvision-0.0.2/cvision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 16:47:16.000000 cvision-0.0.2/cvision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 16:47:16.434217 cvision-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-07-22 16:45:25.000000 cvision-0.0.2/setup.py
```

### Comparing `cvision-0.0.1/LICENSE.txt` & `cvision-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvision-0.0.1/PKG-INFO` & `cvision-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvision
-Version: 0.0.1
+Version: 0.0.2
 Summary: Computer vision package
 Home-page: UNKNOWN
 Author: Dr Anna Sung and Prof Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `cvision-0.0.1/cvision/cvision.py` & `cvision-0.0.2/cvision/cvision.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,63 @@
-from PIL import Image
-import requests
-from io import BytesIO
-import pandas as pd
-from transformers import CLIPProcessor, CLIPModel
-from google.colab import files
+def imageexp():
+  from PIL import Image
+  import requests
+  from io import BytesIO
+  import pandas as pd
+  from transformers import CLIPProcessor, CLIPModel
+  from google.colab import files
+
+
+  V01 = "Very Expensive"
+  V02 = "Expensive"
+  V03 = "Average"
+  V04 = "Inexpensive"
+  V05 = "Very inexpensive"
 
 # Load CLIP model and processor (for expensive level rating)
-model = CLIPModel.from_pretrained("openai/clip-vit-large-patch14")
-processor = CLIPProcessor.from_pretrained("openai/clip-vit-large-patch14")
+  model = CLIPModel.from_pretrained("openai/clip-vit-large-patch14")
+  processor = CLIPProcessor.from_pretrained("openai/clip-vit-large-patch14")
 
-# Helper function to process each image and get the total_index and comment
-def process_image(image_path):
-   image = Image.open(image_path)
+# Helper function to process each image and get the total_index_colour and comment_colour
+  def process_image_val(image_path):
+     image = Image.open(image_path)
 
    # Process image and text
-   inputs = processor(text=["very expensive", "expensive", "average", "inexpensive", "very inexpensive"], images=image, return_tensors="pt", padding=True)
-   outputs = model(**inputs)
-   logits_per_image = outputs.logits_per_image
-   probs = logits_per_image.softmax(dim=1)
-   labels = ["very expensive", "expensive", "average", "inexpensive", "very inexpensive"]
-   label_probs = [(label, prob.item()) for label, prob in zip(labels, probs[0])]
-   label_probs_sorted = sorted(label_probs, key=lambda x: x[1], reverse=True)
+     inputs = processor(text=[V01, V02, V03, V04, V05], images=image, return_tensors="pt", padding=True)
+     outputs = model(**inputs)
+     logits_per_image = outputs.logits_per_image
+     probs = logits_per_image.softmax(dim=1)
+     labels = [V01, V02, V03, V04, V05]
+     label_probs = [(label, prob.item()) for label, prob in zip(labels, probs[0])]
+     label_probs_sorted = sorted(label_probs, key=lambda x: x[1], reverse=True)
 
    # Calculate total_index
-   label_values = [5, 4, 3, 2, 1]
-   total_index = sum(label_values[labels.index(label)] * confidence for label, confidence in label_probs_sorted)
+     label_values = [5, 4, 3, 2, 1]
+     total_index_val = sum(label_values[labels.index(label)] * confidence for label, confidence in label_probs_sorted)
 
    # Determine comment based on total_index
-   comment = ""
-   if total_index >= 4:
-       comment = "Very expensive"
-   elif total_index >= 3:
-       comment = "Expensive"
-   elif total_index >= 2:
-       comment = "Average"
-   elif total_index >= 1:
-       comment = "Inexpensive"
-   else:
-       comment = "Very inexpensive"
+     comment_val = ""
+     if total_index_val >= 4:
+        comment_val = V01
+     elif total_index_val >= 3:
+        comment_val = V02
+     elif total_index_val >= 2:
+        comment_val = V03
+     elif total_index_val >= 1:
+        comment_val = V04
+     else:
+        comment_val = V05
 
-   return total_index, comment
+     return total_index_val, comment_val
 
 # Upload the batch of photos and process them one by one
-uploaded_files = files.upload()
-output_data = []
-for image_path in uploaded_files.keys():
-   total_index, comment = process_image(BytesIO(uploaded_files[image_path]))
-   output_data.append({"Image_Path": image_path, "Total_Index": total_index, "Comment": comment})
+  uploaded_files = files.upload()
+  output_data = []
+  for image_path in uploaded_files.keys():
+    total_index_val, comment_val = process_image_val(BytesIO(uploaded_files[image_path]))
+    output_data.append({"Image_Path": image_path, "Total_Index": total_index_val, "Comment": comment_val})
 
 # Save the output data to a CSV file
-output_df = pd.DataFrame(output_data)
-output_csv_path = "output_results.csv"
-output_df.to_csv(output_csv_path, index=False)
-print(f"Output data saved to {output_csv_path}.")
+  output_df = pd.DataFrame(output_data)
+  output_csv_path = "output_results.csv"
+  output_df.to_csv(output_csv_path, index=False)
+  print(f"Output data saved to {output_csv_path}.")
```

### Comparing `cvision-0.0.1/cvision.egg-info/PKG-INFO` & `cvision-0.0.2/cvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvision
-Version: 0.0.1
+Version: 0.0.2
 Summary: Computer vision package
 Home-page: UNKNOWN
 Author: Dr Anna Sung and Prof Kelvin Leong
 Author-email: <k.leong@chester.ac.uk>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `cvision-0.0.1/setup.py` & `cvision-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.01' 
+VERSION = '0.0.02' 
 DESCRIPTION = 'Computer vision package'
 LONG_DESCRIPTION = 'This Python package aims to evaluate image with computer vision.'
 
 
 setup(
         name="cvision", 
         version=VERSION,
```

