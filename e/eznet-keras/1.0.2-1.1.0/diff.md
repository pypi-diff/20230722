# Comparing `tmp/eznet_keras-1.0.2.tar.gz` & `tmp/eznet_keras-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eznet_keras-1.0.2.tar", last modified: Sun Jul 16 12:29:35 2023, max compression
+gzip compressed data, was "eznet_keras-1.1.0.tar", last modified: Sat Jul 22 18:25:15 2023, max compression
```

## Comparing `eznet_keras-1.0.2.tar` & `eznet_keras-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.441559 eznet_keras-1.0.2/
--rw-rw-rw-   0        0        0     1189 2023-01-20 13:30:59.000000 eznet_keras-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0    14243 2023-07-16 12:29:35.442556 eznet_keras-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13171 2023-07-16 12:07:46.000000 eznet_keras-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.421105 eznet_keras-1.0.2/eznet_keras/
--rw-rw-rw-   0        0        0       40 2023-02-06 16:31:38.000000 eznet_keras-1.0.2/eznet_keras/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.437572 eznet_keras-1.0.2/eznet_keras/keras2cpp/
--rw-rw-rw-   0        0        0       24 2023-01-18 12:07:49.000000 eznet_keras-1.0.2/eznet_keras/keras2cpp/__init__.py
--rw-rw-rw-   0        0        0     9834 2022-07-10 10:31:49.000000 eznet_keras-1.0.2/eznet_keras/keras2cpp/create_unit_tests.py
--rw-rw-rw-   0        0        0     5519 2022-07-10 10:31:49.000000 eznet_keras-1.0.2/eznet_keras/keras2cpp/keras2cpp.py
--rw-rw-rw-   0        0        0      576 2022-07-10 10:31:49.000000 eznet_keras-1.0.2/eznet_keras/keras2cpp/python_model.py
-drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.441559 eznet_keras-1.0.2/eznet_keras/models/
--rw-rw-rw-   0        0        0      425 2023-01-19 20:08:07.000000 eznet_keras-1.0.2/eznet_keras/models/__init__.py
--rw-rw-rw-   0        0        0    17915 2023-07-15 17:25:36.000000 eznet_keras-1.0.2/eznet_keras/models/ann.py
--rw-rw-rw-   0        0        0    26308 2023-07-14 09:38:07.000000 eznet_keras-1.0.2/eznet_keras/models/conv_block.py
--rw-rw-rw-   0        0        0    31709 2023-07-16 12:07:25.000000 eznet_keras-1.0.2/eznet_keras/models/conv_network.py
--rw-rw-rw-   0        0        0    11975 2023-07-14 12:26:34.000000 eznet_keras-1.0.2/eznet_keras/models/dense_block.py
--rw-rw-rw-   0        0        0    11960 2023-07-15 17:49:42.000000 eznet_keras-1.0.2/eznet_keras/models/keras_smart_module.py
--rw-rw-rw-   0        0        0    25219 2023-07-15 17:23:22.000000 eznet_keras-1.0.2/eznet_keras/models/recurrent_network.py
--rw-rw-rw-   0        0        0     5319 2023-01-19 20:20:51.000000 eznet_keras-1.0.2/eznet_keras/models/var_ae.py
--rw-rw-rw-   0        0        0     2442 2023-01-19 20:22:43.000000 eznet_keras-1.0.2/eznet_keras/test.py
--rw-rw-rw-   0        0        0    13856 2023-07-15 13:47:05.000000 eznet_keras-1.0.2/eznet_keras/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 12:29:35.435578 eznet_keras-1.0.2/eznet_keras.egg-info/
--rw-rw-rw-   0        0        0    14243 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      698 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 12:29:35.000000 eznet_keras-1.0.2/eznet_keras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-16 12:29:35.443552 eznet_keras-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1823 2023-07-16 12:07:54.000000 eznet_keras-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:25:15.290820 eznet_keras-1.1.0/
+-rw-rw-rw-   0        0        0     1189 2023-01-20 13:30:59.000000 eznet_keras-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    14243 2023-07-22 18:25:15.290820 eznet_keras-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13171 2023-07-22 18:21:31.000000 eznet_keras-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 18:25:15.268892 eznet_keras-1.1.0/eznet_keras/
+-rw-rw-rw-   0        0        0       40 2023-02-06 16:31:38.000000 eznet_keras-1.1.0/eznet_keras/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:25:15.284839 eznet_keras-1.1.0/eznet_keras/keras2cpp/
+-rw-rw-rw-   0        0        0       24 2023-01-18 12:07:49.000000 eznet_keras-1.1.0/eznet_keras/keras2cpp/__init__.py
+-rw-rw-rw-   0        0        0     9834 2022-07-10 10:31:49.000000 eznet_keras-1.1.0/eznet_keras/keras2cpp/create_unit_tests.py
+-rw-rw-rw-   0        0        0     5519 2022-07-10 10:31:49.000000 eznet_keras-1.1.0/eznet_keras/keras2cpp/keras2cpp.py
+-rw-rw-rw-   0        0        0      576 2022-07-10 10:31:49.000000 eznet_keras-1.1.0/eznet_keras/keras2cpp/python_model.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:25:15.289822 eznet_keras-1.1.0/eznet_keras/models/
+-rw-rw-rw-   0        0        0      425 2023-01-19 20:08:07.000000 eznet_keras-1.1.0/eznet_keras/models/__init__.py
+-rw-rw-rw-   0        0        0    20207 2023-07-22 18:17:31.000000 eznet_keras-1.1.0/eznet_keras/models/ann.py
+-rw-rw-rw-   0        0        0    26308 2023-07-14 09:38:07.000000 eznet_keras-1.1.0/eznet_keras/models/conv_block.py
+-rw-rw-rw-   0        0        0    33696 2023-07-22 18:07:38.000000 eznet_keras-1.1.0/eznet_keras/models/conv_network.py
+-rw-rw-rw-   0        0        0    12738 2023-07-22 15:35:30.000000 eznet_keras-1.1.0/eznet_keras/models/dense_block.py
+-rw-rw-rw-   0        0        0    14906 2023-07-22 18:14:35.000000 eznet_keras-1.1.0/eznet_keras/models/keras_smart_module.py
+-rw-rw-rw-   0        0        0    27119 2023-07-22 18:19:14.000000 eznet_keras-1.1.0/eznet_keras/models/recurrent_network.py
+-rw-rw-rw-   0        0        0     5319 2023-01-19 20:20:51.000000 eznet_keras-1.1.0/eznet_keras/models/var_ae.py
+-rw-rw-rw-   0        0        0     2442 2023-01-19 20:22:43.000000 eznet_keras-1.1.0/eznet_keras/test.py
+-rw-rw-rw-   0        0        0    15984 2023-07-22 17:29:48.000000 eznet_keras-1.1.0/eznet_keras/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:25:15.282850 eznet_keras-1.1.0/eznet_keras.egg-info/
+-rw-rw-rw-   0        0        0    14243 2023-07-22 18:25:15.000000 eznet_keras-1.1.0/eznet_keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2023-07-22 18:25:15.000000 eznet_keras-1.1.0/eznet_keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 18:25:15.000000 eznet_keras-1.1.0/eznet_keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-22 18:25:15.000000 eznet_keras-1.1.0/eznet_keras.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-22 18:25:15.000000 eznet_keras-1.1.0/eznet_keras.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-22 18:25:15.294806 eznet_keras-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1823 2023-07-22 18:21:18.000000 eznet_keras-1.1.0/setup.py
```

### Comparing `eznet_keras-1.0.2/LICENSE.txt` & `eznet_keras-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.2/PKG-INFO` & `eznet_keras-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eznet_keras
-Version: 1.0.2
+Version: 1.1.0
 Summary: Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc.
 Home-page: https://github.com/pniaz20/eznet_keras
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: tensorflow,keras,deep learning,neural network,keras2cpp
 Classifier: Development Status :: 3 - Alpha
@@ -25,16 +25,16 @@
 
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 1.0.2  
-Last Update: July 15, 2023
+Version: 1.1.0  
+Last Update: July 22, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
```

### Comparing `eznet_keras-1.0.2/README.md` & `eznet_keras-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 1.0.2  
-Last Update: July 15, 2023
+Version: 1.1.0  
+Last Update: July 22, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
```

### Comparing `eznet_keras-1.0.2/eznet_keras/keras2cpp/create_unit_tests.py` & `eznet_keras-1.1.0/eznet_keras/keras2cpp/create_unit_tests.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.2/eznet_keras/keras2cpp/keras2cpp.py` & `eznet_keras-1.1.0/eznet_keras/keras2cpp/keras2cpp.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.2/eznet_keras/keras2cpp/python_model.py` & `eznet_keras-1.1.0/eznet_keras/keras2cpp/python_model.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.2/eznet_keras/models/ann.py` & `eznet_keras-1.1.0/eznet_keras/models/ann.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,39 +15,46 @@
         # General and I/O parameters
         "model_name": "ANN",
         "input_shape": [10],
         "output_size": 3,
         # Architecture parameters
         "width": 32,
         "depth": 2,
+        "hidden_params": None,
         "hidden_activation": "LeakyReLU",
         "hidden_activation_params": {'alpha': 0.1},
         "norm_layer_type":"BatchNormalization",
         "norm_layer_position": "before",
         "norm_layer_params": None,
         "dropout": 0.2,
         "include_output_layer": True,
+        "output_dense_params": None,
         "output_activation": "Softmax",
         "output_activation_params": None,
         # Training procedure parameters
         "learning_rate": 0.001,
         "exponential_decay_rate": 0.9,
         "batch_size": 32,
         "epochs": 2,
         "early_stopping_patience_epochs": 2,
         "validation_data": [0.05,'trainset'],
         "l2_reg": 0.0001,
+        "l1_reg": None,
         "loss_function": "categorical_crossentropy",
+        "loss_function_params": None,
         'optimizer': 'Adam',
         'optimizer_params': None,
         'metrics': ['accuracy'],
+        "metrics_params": None,
         'checkpoint_path': None,
         'early_stopping_monitor': 'loss',
         'early_stopping_mode': 'min',
-        'early_stopping_value': 1.0e-6
+        'early_stopping_value': 1.0e-6,
+        'other_callbacks': None,
+        'custom_schedule': None
     }
     
     
     def __init__(self, hparams:dict=None):
         """Typical Artificial Neural Network class, also known as multilayer perceptron. This class will create a fully connected feedforward artificial neural network.
         It can be used for classification, regression, etc. It basically encompasses enough options to build all kinds of serial ANNs with any number of 
         inputs, outputs, layers with custom or arbitrary width or depth, etc. Supports multiple activation functions for hidden layers and the output layer. The netwrok consists
@@ -80,45 +87,57 @@
                 all feature maps, such that only the last dimension will change. An input of `[batch, dim1, dim2, in_dim]` will come out as `[batch, dim1, dim2, layer_size]`
                 from a dense block.
             - `output_size` (int): number of outputs to predict, i.e. size of the output layer, if there is going to be an output layer.
             - `width` (int|list): (list of) hidden layer widths. 
                 a number sets them all the same, and a list/array sets each hidden layer according to the list.
             - `depth` (int): Specifies the depth of the network (number of hidden layers).
                 It must be specified unless `width` is provided as a list. Then the depth will be inferred form it.
+            - `hidden_params` (dict): (list of) kwargs parameters for the hidden layer constructor, if any. Defaults to None. Will overwrite everything else if specified.
             - `hidden_activation` (str): (list of) Activations. It can be an activation function name ("relu","sigmoid","tanh", etc.), an activation layer name ("ReLU", 
                 "LeakyReLU", "Softmax", etc.), or a custom Keras Layer class (not instance). Defaults to None.
             - `hidden_activation_params` (dict): (list of) kwargs parameters for the hidden layer activation constructor, if any. Ignored for any dense block if the activation is
                 provided as a lower-case function name. By the way, the slope of the negative section in `LeakyReLU` is `alpha`. Defaults to None.
             - `norm_layer_type` (str): (list of) Types of normalization layers to use for each hidden layer. Options are "BatchNormalization", "LayerNormalization", etc.
                 This can also be a Keras Layer class (not instance) rather than a string. Defaults to None.
             - `norm_layer_position` (str): (list of) where the normalization layer should be included relative to the activation function (if any), 'before' or 'after'.
             - `norm_layer_params` (dict): (list of) Dictionaries of kwargs parameters for the normalization layers' constructors. Defaults to None.
             - `dropout` (float): (list of) the dropout rates after every hidden layer. It should be a probability value between 0 and 1, or None by default.
             - `include_output_layer` (bool): Whether to include an output layer at the end of the network. Defaults to True.
+            - `output_dense_params` (dict): Parameters for the output dense layer, if any. Defaults to None. Will overwrite everything else if specified.
             - `output_activation` (str): Activation of the output layer, if any. Defaults to None.
                 For classification problems, you may want to choose "sigmoid" or "softmax".
                 That being said, you usually don't need to specify an activation for the output layer at all, if e.g. 'from_logits' is used.
                 For regression problems, no activation is needed. It is by default linear, unless you want to manually specify an activation.
             - `output_activation_params` (dict): Parameters for the output activation function, if any. Ignored if lower-case function name is provided for activation.
                 Defaults to None.
             - `learning_rate` (float): Initial learning rate of training.
             - `exponential_decay_rate` (float): Exponential decay rate for learning rate, if any. Defaults to None.
             - `optimizer` (str): Optimizer. Examples: "Adam", "SGD" ,"RMSProp", etc. The name of any optimizer class in `tf.keras.optimizers` can be used, or a custom class.
+            This can also be a custom optimizer class (not instance), in which case `optimizer_params` can be specified for its constructor kwargs.
             - `optimizer_params` (dict): Additional parameters of the optimizer, if any. Defaults to None.
             - `batch_size` (int): Minibatch size for training.
             - `epochs` (int): Maximum number of epochs for training.
             - `early_stopping_patience_epochs` (int): Epochs to tolerate unimproved (val) loss, before early stopping.
             - `validation_data` (list): List of [validation_split, 'trainset'|'testset']. Defaults to None.
             - `l2_reg` (float): L2 regularization parameter. Defaults to None.
-            - `loss_function` (str): Loss function. Examples: "mse","binary_crossentropy", "categorical_crossentropy", etc. It can also be a loss function instance.
-            - `metrics` (list): list of metrics for Keras compilation, e.g. ['accuracy'].
+            - `l1_reg` (float): L1 regularization parameter. Defaults to None.
+            - `loss_function` (str): Loss function. It can be a lower-case name such as "mse", "binary_crossentropy", "categorical_crossentropy", etc.,
+                the name of a `tf.keras.losses` class such as `BinaryCrossentropy`, `CategoricalCrossentropy`, `MeanSquaredError', etc., or a valid loss class (not instance).
+            - `loss_function_params` (dict): Additional kwargs parameters of the loss function constructor, if any. Ignored if the loss function is a lower-case name string.
+            - `metrics` (list): list of metrics for Keras compilation. Each member of the list can be a lower-case metric name such as "mse" or "accuracy", the name of a 
+                `tf.keras.metrics` class such as `Accuracy`, `MeanSquaredError`, etc., or a valid metric class (not instance).
+            - `metrics_params` (list): (list of) additional kwargs parameters of the metrics constructors, if any. Ignored for every metric that is a lower-case name string.
+                If this entry is a single dicitonary rather than a list, it will be broadcast to all metrics in the metrics list.
             - `checkpoint_path` (str): Path to the directory where checkpoints will be saved at every epoch.
             - `early_stopping_monitor` (str): Monitor whose critical value will cause early stopping. Default is 'loss', but 'val_loss' is typically used.
             - `early_stopping_mode` (str): Mode of the parameter whose critical value will be used for early stopping. Deafults to 'min' for any error. 'max' is for accuracy, etc.
             - `early_stopping_value` (float): Value of the monitor at which point training will stop becasue the critical value has been reached.
+            - `other_callbacks` (list): List of other callbacks to be used in training, if any. Defaults to None.
+            - `custom_schedule` (schedule): Custom learning rate schedule inheriting from `tf.keras.optimizers.schedules.LearningRateSchedule`. Defaults to None.
+            
         
         Note that for all such hyperparameters that have a (list of) at the beginning, the entry can be a single item repeated for all hidden layers, or it can be a list of items
         for all hidden layers. If a list is provided, it must have the same length as the depth of the network. 
         
         Also note that depth does not include the input and output layers.
         This gives you the ability to specify different width, dropout rate, normalization layer and its parameters, and so forth.
 
@@ -135,28 +154,30 @@
         self._input_shape = hparams.get("input_shape")
         if self._input_shape is not None:
             assert isinstance(self._input_shape, (list,tuple)), "input_shape must be a list or tuple."
         self._output_size = hparams.get("output_size")
         self._dropout = hparams.get("dropout")
         self._width = hparams.get("width")
         self._depth = hparams.get("depth")
+        self._hidden_params = hparams.get("hidden_params")
         if self._depth is None:
             assert isinstance(self._width, (list,tuple)), "If depth is not provided, width must be a list or tuple."
             self._depth = len(self._width)
         elif self._width is None:
             assert isinstance(self._depth, int), "If width is not provided, depth must be an integer."
             warnings.warn("Width is not provided. It will be set to the same value as the final dimension of the input shape.", UserWarning)
             self._width = self._input_shape[-1]
         elif isinstance(self._width, (list,tuple)):
             assert len(self._width) == self._depth, "If width is a list or tuple, it must have length equal to the depth."
             
             
         self._hidden_activation = hparams.get("hidden_activation")
         self._hidden_activation_params = hparams.get("hidden_activation_params")
         self._include_output_layer = hparams.get("include_output_layer")
+        self._output_dense_params = hparams.get("output_dense_params")
         self._output_activation = hparams.get("output_activation")
         self._output_activation_params = hparams.get("output_activation_params")
         self._norm_layer_type = hparams.get("norm_layer_type")
         self._norm_layer_position = hparams.get("norm_layer_position")
         self._norm_layer_params = hparams.get("norm_layer_params")
         self.batch_input_shape = (self._batch_size,) + tuple(self._input_shape)
         self.batch_output_shape = (self._batch_size,) + tuple(self._input_shape[:-1]) + (self._output_size,)
@@ -169,14 +190,15 @@
             else:
                 self._output_activation_module = self._output_activation
         else:
             self._output_activation_module = None
         
         # Generate arrays containing parameters of each Dense Block (Every block contains a linear, normalization, activation, and dropout layer).
         self._dense_width_vec = self._gen_hparam_vec_for_dense(self._width, 'width')
+        self._dense_params_vec = self._gen_hparam_vec_for_dense(self._hidden_params, 'hidden_params')
         self._dense_activation_vec = self._gen_hparam_vec_for_dense(self._hidden_activation, 'hidden_activation')
         self._dense_activation_params_vec = self._gen_hparam_vec_for_dense(self._hidden_activation_params, 'hidden_activation_params')
         self._dense_norm_layer_type_vec = self._gen_hparam_vec_for_dense(self._norm_layer_type, 'norm_layer_type')
         self._dense_norm_layer_params_vec = self._gen_hparam_vec_for_dense(self._norm_layer_params, 'norm_layer_params')
         self._dense_norm_layer_position_vec = self._gen_hparam_vec_for_dense(self._norm_layer_position, 'norm_layer_position')
         self._dense_dropout_vec = self._gen_hparam_vec_for_dense(self._dropout, 'dropout')
         
@@ -192,24 +214,28 @@
                 'output_size':self._dense_width_vec[i],
                 'activation':self._dense_activation_vec[i],
                 'activation_params':self._dense_activation_params_vec[i],
                 'norm_layer_type':self._dense_norm_layer_type_vec[i],
                 'norm_layer_position':self._dense_norm_layer_position_vec[i],
                 'norm_layer_params':self._dense_norm_layer_params_vec[i],
                 'dropout':self._dense_dropout_vec[i],
-                'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None)
+                'kernel_regularizer':self.make_regularizer(),
+                'dense_params':self._dense_params_vec[i],
             }
             if i==0 and self._input_shape is not None:
                 _kwargs.update({'input_shape':self._input_shape})
             add_dense_block(**_kwargs)
             # in_size = out_size
         
         # Output layer
         if self._include_output_layer:
-            self.net.add(tf.keras.layers.Dense(self._output_size, kernel_regularizer=(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None)))
+            _kwargs = {'units':self._output_size, 'kernel_regularizer':self.make_regularizer()}
+            if self._output_dense_params:
+                _kwargs.update(self._output_dense_params)
+            self.net.add(tf.keras.layers.Dense(**_kwargs))
             if self._output_activation:
                 if isinstance(self._output_activation, str):
                     if self._output_activation.lower() == self._output_activation:
                         self.net.add(tf.keras.layers.Activation(self._output_activation))
                     elif self._output_activation_params:
                         self.net.add(getattr(tf.keras.layers, self._output_activation)(**self._output_activation_params))
                     else:
@@ -229,15 +255,15 @@
 
 
 
 if __name__ == '__main__':
     
     hparams = {
         # General and I/O parameters
-        "model_name": "My Model",
+        "model_name": "My_Model",
         "input_shape": [28, 28, 3], #[10],
         "output_size": 24,
         # Architecture parameters
         "width": 32,
         "depth": 3,
         "hidden_activation": "LeakyReLU",
         "hidden_activation_params": {'alpha':0.1},
```

### Comparing `eznet_keras-1.0.2/eznet_keras/models/conv_block.py` & `eznet_keras-1.1.0/eznet_keras/models/conv_block.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.2/eznet_keras/models/conv_network.py` & `eznet_keras-1.1.0/eznet_keras/models/conv_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,39 +39,46 @@
         "pool_params": None,
         "min_image_size": 4,
         "flatten_after_conv": True,
         # Fully connected blocks
         "include_dense_layers": True,
         "dense_width": "auto",
         "dense_depth": 2,
+        "dense_params": None,
         "dense_activation": "relu",
         "dense_activation_params": None,
         "dense_norm_layer_type": "BatchNormalization",
         "dense_norm_layer_position": "before",
         "dense_norm_layer_params": None,
         "dense_dropout": 0.1,
         "include_output_layer": True,
+        "output_dense_params": None,
         "output_activation": "softmax",
         "output_activation_params": None,
         # Training procedure
         "l2_reg": 0.0001,
+        "l1_reg": None,
         "batch_size": 32,
         "epochs": 2,
         "validation_data": [0.05,'testset'],
         "early_stopping_patience_epochs": 5,
         "learning_rate": 0.01,
         "exponential_decay_rate": 0.9,
         "loss_function": "categorical_crossentropy",
+        "loss_function_params": None,
         "optimizer": "Adam",
         "optimizer_params": None,
         'metrics':['accuracy'],
+        'metrics_params':None,
         'checkpoint_path':None,
         'early_stopping_monitor':'loss',
         'early_stopping_mode':'min',
-        'early_stopping_value':1.0e-6
+        'early_stopping_value':1.0e-6,
+        'other_callbacks': None,
+        'custom_schedule': None,
     }
     
     
     def __init__(self, hparams:dict=None):
         """Standard Convolutional Neural Network, containing convolutional blocks followed by fully-connected blocks. It supports 1D, 2D, and 3D convolutions, and can be used for 
         image classification, timeseries classification, video classification, and so forth. The module can easily be trained and evaluated using its own methods,
         because it inherits from `KerasSmartModel`. The architecture consists of conv blocks followed by dense blocks. Each conv block is assumed to contain a convolution layer, 
@@ -151,52 +158,63 @@
             negates any reason for flattening. Defaults to None.
             
         #### Dense blocks
         
         - `dense_width` ("auto"|int|list): Width of the hidden layers of the Dense network. "auto", a number (for all of them) or a list holding width of each hidden layer.
             If "auto", it will start with the output size of the Flatten() layer, halving at every Dense block.
         - `dense_depth` (int): Depth (number of hidden layers) of the Dense network. `0` will mean no hidden layers, meaning Flatten will be directly followed by the output layer.
+        - `dense_params` (dict): (list of) kwargs dict to pass to the dense layer constructor in each block. Defaults to None.
         - `dense_activation` (str|list): (list of) activation function for hidden layers of the Dense network. These can be activation functions ("relu", "sigmoid", "tanh", etc.),
             activation layers ("ReLU", "LeakyReLU", "Softmax", etc.), or custom Layer classes (not instances). Defaults to None, in which case no activation function will be used.
         - `dense_activation_params` (dict|list): (list of) dicts for the dense activation functions' constructors. Ignored if lower-case activation functions are provided.
             By the way, the slope of the negative section in `LeakyReLU` is `alpha`.
         - `dense_norm_layer_type` (str|list): (list of) types of normalization layers to use in the dense blocks. Examples: 'BatchNormalization', 'LayerNormalization', etc.
             Defaults to None, in which case no normalization layer will be used. Instead of strings, custom Keras Layer classes (not instances) can also be provided.
         - `dense_norm_layer_position` ("before"|"after"|list): (list of) positions of the normalization layers in the dense blocks relative to the activation functions. 
             Defaults to "before". If it is a list, it should be a list of strings of the same length as `dense_depth`.
         - `dense_norm_layer_params` (dict|list): (list of) kwargs dict for the dense normalization layers' constructors.
         - `dense_dropout` (float|list): (list of) Dropout rates (if any) for the hidden layers of the Dense network.
         - `include_output_layer` (bool): Whether to include an output layer. Defaults to True.
+        - `output_dense_params` (dict): kwargs dict for the output layer's Dense constructor. Defaults to None.
         - `output_activation` (str): Activation (with the same format as dense activation) for the output layer, if any.
             **NOTE** Depending on the loss function, you may not need an activation function.
             For classification problems, you may want to choose "sigmoid" or "softmax".
             That being said, you usually don't need to specify an activation for the output layer at all, if e.g. 'from_logits' is used.
             For regression problems, no activation is needed. It is by default linear, unless you want to manually specify an activation.
         - `output_activation_params` (dict): Dictionary of parameters for the output activation function's constructor. Ignored if a lower-case function name is provided.
         
         #### Training procedure
         
         - `batch_size` (int): Minibatch size, the expected input size of the network.
         - `learning_rate` (float): Initial learning rate of training.
         - `exponential_decay_rate` (float): Exponential decay rate gamma for learning rate, if any.
-        - `optimizer` (str): Optimizer. Examples: 'Adam', 'SGD', 'RMSprop', etc. It can be the name of any Keras optimizer.
+        - `optimizer` (str): Optimizer. Examples: 'Adam', 'SGD', 'RMSprop', etc. It can be the name of any Keras optimizer class.
+            This can also be a custom optimizer class (not instance), in which case `optimizer_params` can be specified for its constructor kwargs.
         - `optimizer_params` (dict): Additional parameters of the optimizer constructor, if any.
         - `epochs` (int): Maximum number of epochs for training.
         - `early_stopping_patience_epochs` (int): Epochs to tolerate unimproved (val) loss, before early stopping.
         - `l2_reg` (float): L2 regularization parameter.
-        - `loss_function` (str): Loss function. Examples: 'mse','categorical_crossentropy', etc. A Keras loss function instance can also be provided rather than a string.
+        - `l1_reg` (float): L1 regularization parameter.
+        - `loss_function` (str): Loss function. It can be a lower-case name such as "mse", "binary_crossentropy", "categorical_crossentropy", etc.,
+            the name of a `tf.keras.losses` class such as `BinaryCrossentropy`, `CategoricalCrossentropy`, `MeanSquaredError', etc., or a valid loss class (not instance).
+        - `loss_function_params` (dict): Additional kwargs parameters of the loss function constructor, if any. Ignored if the loss function is a lower-case name string.
+        - `metrics` (list): list of metrics for Keras compilation. Each member of the list can be a lower-case metric name such as "mse" or "accuracy", the name of a 
+            `tf.keras.metrics` class such as `Accuracy`, `MeanSquaredError`, etc., or a valid metric class (not instance).
+        - `metrics_params` (list): (list of) additional kwargs parameters of the metrics constructors, if any. Ignored for every metric that is a lower-case name string.
+            If this entry is a single dicitonary rather than a list, it will be broadcast to all metrics in the metrics list.
         - `validation_data` (tuple): Validation data, if any. It should be a tuple of `(portion, from_dataset)`. For instance, `[0.05, 'testset']` means 5% of the testset will be 
             used for validation. The second element of the tuple can only be `'trainset'` and `'testset'`. The first element must be a float between 0 and 1. 
             If the second element is not specified, testset will be used by default.
-        - `metrics` (list): list of metrics for Keras compilation, e.g. ['accuracy']. This will be passed directly to Keras compile function, so it can be a list of class instances
-            or a list of strings.
         - `checkpoint_path` (str): Path to the directory where checkpoints will be saved at every epoch.
         - `early_stopping_monitor` (str): Monitor whose critical value will cause early stopping. Default is 'loss', but 'val_loss' is typically used.
         - `early_stopping_mode` (str): Mode of the parameter whose critical value will be used for early stopping. Deafults to 'min' for any error. 'max' is for accuracy, etc.
         - `early_stopping_value` (float): Value of the monitor at which point training will stop because the critical value has been reached.
+        - `other_callbacks` (list): List of other callbacks to be used during training, if any. Defaults to None.
+        - `custom_schedule` (schedule): Custom learning rate schedule inheriting from `tf.keras.optimizers.schedules.LearningRateSchedule`. Defaults to None.
+        
         
         ### Returns
         
         - Returns a `tf.keras.models.Model` object that can be trained and used accordingly.
         - Run `net.summary()` afterwards to see what you have inside the network.
         - A `KerasSmartModel` object is returned. This module has its own functions for training, evaluation, etc.
         """
@@ -288,15 +306,15 @@
                 'pool_kernel_size':self._pool_kernel_size_vec[i], 
                 'pool_padding':self._pool_padding_vec[i], 
                 'pool_stride':self._pool_stride_vec[i], 
                 'pool_params':self._pool_params_vec[i], 
                 'dropout':self._conv_dropout_vec[i],
                 'spatial_dropout':self._conv_spatial_dropout_vec[i], 
                 'min_image_dim':self._min_image_size,
-                'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg>0 else None)
+                'kernel_regularizer':self.make_regularizer()
             }
             if i==0:
                 _kwargs.update({'input_shape':self._input_shape})
             d = add_conv_block(**_kwargs)
             self.net = d['model']
             output_image = d['output_image']
             self.size_list.append(output_image+[out_channels])
@@ -319,24 +337,26 @@
         self.size_list.append([self._dense_input_size])
         
         # Construct dense layers
         if self._include_dense_layers:
             
             # Dense layers hyperparameters
             self._dense_width = hparams.get("dense_width")
+            self._dense_params = hparams.get("dense_params")
             self._dense_activation = hparams.get("dense_activation")
             self._dense_activation_params = hparams.get("dense_activation_params")
             self._dense_norm_layer_type = hparams.get("dense_norm_layer_type")
             self._dense_norm_layer_params = hparams.get("dense_norm_layer_params")
             self._dense_norm_layer_position = hparams.get("dense_norm_layer_position")
             self._dense_dropout = hparams.get("dense_dropout")
             
             # Generate lists of hyperparameters for the dense layers
             self._dense_width_vec = self._gen_hparam_vec_for_dense(self._dense_width, 'dense_width',
                 check_auto=True, init_for_auto=self._dense_input_size, powers_of_two_if_auto=True, direction_if_auto="down")
+            self._dense_params_vec = self._gen_hparam_vec_for_dense(self._dense_params, 'dense_params')
             self._dense_activation_vec = self._gen_hparam_vec_for_dense(self._dense_activation, 'dense_activation')
             self._dense_activation_params_vec = self._gen_hparam_vec_for_dense(self._dense_activation_params, 'dense_activation_params')
             self._dense_norm_layer_type_vec = self._gen_hparam_vec_for_dense(self._dense_norm_layer_type, 'dense_norm_layer_type')
             self._dense_norm_layer_params_vec = self._gen_hparam_vec_for_dense(self._dense_norm_layer_params, 'dense_norm_layer_params')
             self._dense_norm_layer_position_vec = self._gen_hparam_vec_for_dense(self._dense_norm_layer_position, 'dense_norm_layer_position')
             self._dense_dropout_vec = self._gen_hparam_vec_for_dense(self._dense_dropout, 'dense_dropout')
             
@@ -350,28 +370,33 @@
                         'output_size':self._dense_width_vec[i],
                         'activation':self._dense_activation_vec[i],
                         'activation_params':self._dense_activation_params_vec[i],
                         'norm_layer_type':self._dense_norm_layer_type_vec[i],
                         'norm_layer_position':self._dense_norm_layer_position_vec[i],
                         'norm_layer_params':self._dense_norm_layer_params_vec[i],
                         'dropout': self._dense_dropout_vec[i],
-                        'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg>0 else None)
+                        'kernel_regularizer':self.make_regularizer(),
+                        'dense_params':self._dense_params_vec[i]
                     }
                     add_dense_block(**_kwargs)
                     # in_size = out_size
                     self.size_list.append([out_size])
         
         # Construct output layer
         if self._include_output_layer:
             # Output hyperparameters
+            self._output_dense_params = hparams.get("output_dense_params")
             self._output_activation = hparams.get("output_activation")
             self._output_activation_params = hparams.get("output_activation_params")
         
             # Output layer
-            self.net.add(tf.keras.layers.Dense(self._output_shape[-1], kernel_regularizer=(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg>0 else None)))
+            _kwargs = {'units':self._output_shape[-1], 'kernel_regularizer':self.make_regularizer()}
+            if self._output_dense_params:
+                _kwargs.update(self._output_dense_params)
+            self.net.add(tf.keras.layers.Dense(**_kwargs))
             if self._output_activation:
                 if isinstance(self._output_activation, str):
                     if self._output_activation.lower() == self._output_activation:
                         self.net.add(tf.keras.layers.Activation(self._output_activation))
                     elif self._output_activation_params:
                         self.net.add(getattr(tf.keras.layers, self._output_activation)(**self._output_activation_params))
                     else:
```

### Comparing `eznet_keras-1.0.2/eznet_keras/models/dense_block.py` & `eznet_keras-1.1.0/eznet_keras/models/dense_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,27 @@
     import os, sys
     parent_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
     sys.path.append(parent_dir)
     from utils import *
 
 
 class Dense_Block(tf.keras.layers.Layer):
-    def __init__(self, input_shape:list=None, output_size:int=None, activation:str=None, activation_params:dict=None, norm_layer_type:str=None, norm_layer_position:str='before', 
+    def __init__(self, input_shape:list=None, output_size:int=None, activation:str=None, activation_params:dict=None, dense_params:dict=None, norm_layer_type:str=None, norm_layer_position:str='before', 
                  norm_layer_params:dict=None, dropout:float=None, kernel_regularizer:tf.keras.regularizers.Regularizer=None):
         """Dense (fully connected) block containing one linear layer, followed optionally by a normalization layer, an activation function and a Dropout layer.
 
         ### Args:
+
             - `input_shape` (list|tuple): Shape of the input without the batch size.
             - `output_size` (int, optional): Number of output features. Defaults to None, in which case it will be input_size.
             - `activation` (str, optional): Activation. It can be an activation function name ("relu","sigmoid","tanh", etc.), an activation layer name ("ReLU", "LeakyReLU",
                 "Softmax", etc.), or a custom Keras Layer class (not instance). Defaults to None.
             - `activation_params` (dict, optional): kwargs to pass to the activation function constructor. Defaults to None. Ignored if `activation` is a lower-case function name.
                 By the way, the slope of the negative section in `LeakyReLU` is `alpha`.
+            - `dense_params` (dict, optional): kwargs to pass to the dense layer constructor. Defaults to None. This will overwrite any other parameters such as regularizers, etc.
             - `norm_layer_type` (str, optional): Type of normalization layer. Defaults to None. Examples: 'BatchNormalization', 'LayerNormalization', etc.
                 It can also be a Keras Layer class (not instance).
             - `norm_layer_position` (str, optional): Position of norm layer relative to activation. Defaults to 'before'. Alternative is 'after'.
             - `norm_layer_params` (dict, optional): kwargs to pass to the norm layer constructor. Defaults to None.
             - `dropout` (float, optional): Dropout rate at the end. Defaults to None. Must be a float between 0 and 1.
             - `kernel_regularizer` (regularizer, optinal): Regularizer instance to be used for the kernel weights in the layers.
         
@@ -49,14 +51,15 @@
         self._input_shape = input_shape
         self._output_size = output_size
         self._activation = activation
         self._activation_params = activation_params
         self._norm_layer_type = norm_layer_type
         self._norm_layer_position = norm_layer_position
         self._norm_layer_params = norm_layer_params
+        self._dense_params = dense_params
         self._dropout = dropout
         if activation is not None:
             if isinstance(activation, str):
                 if activation.lower()==activation:
                     self._activation_module = getattr(tf.keras.activations, activation)
                 else:
                     self._activation_module = getattr(tf.keras.layers, activation)
@@ -70,18 +73,24 @@
             else:
                 self._norm_layer_module = norm_layer_type
         else:
             self._norm_layer_module = None
         self._dropout_module = tf.keras.layers.Dropout if dropout else None
         self._kernel_regularizer = kernel_regularizer
         self.net = tf.keras.models.Sequential()
+        _kwargs = {
+            'units': output_size
+        }
         if input_shape:
-            self.net.add(tf.keras.layers.Dense(output_size, input_shape=input_shape, kernel_regularizer=kernel_regularizer))
-        else:
-            self.net.add(tf.keras.layers.Dense(output_size, kernel_regularizer=kernel_regularizer))
+            _kwargs.update({'input_shape':input_shape})
+        if kernel_regularizer is not None:
+            _kwargs.update({'kernel_regularizer':kernel_regularizer})
+        if dense_params is not None:
+            _kwargs.update(dense_params)
+        self.net.add(tf.keras.layers.Dense(**_kwargs))
         if norm_layer_type and norm_layer_position=='before': 
             if norm_layer_params: self.net.add(self._norm_layer_module(**norm_layer_params))
             else: self.net.add(self._norm_layer_module())
         if activation:
             if isinstance(activation, str) and activation.lower()==activation: 
                 self.net.add(tf.keras.layers.Activation(self._activation_module))
             else:
@@ -102,42 +111,44 @@
             'output_size':self._output_size,
             'activation':self._activation,
             'activation_params':self._activation_params,
             'norm_layer_type':self._norm_layer_type,
             'norm_layer_position':self._norm_layer_position,
             'norm_layer_params':self._norm_layer_params,
             'dropout':self._dropout,
-            'kernel_regularizer':self._kernel_regularizer
+            'kernel_regularizer':self._kernel_regularizer,
+            'dense_params':self._dense_params
         }
         config['hparams'] = hparams
         return config
     
     @classmethod
     def from_config(cls, config):
         return cls(**config['hparams'])
     
     def summary(self):
         return self.net.summary()
         
 
 
 
-def add_dense_block(model:tf.keras.models.Sequential, output_size:int, input_shape:list=None, activation:str=None, activation_params:dict=None, 
+def add_dense_block(model:tf.keras.models.Sequential, output_size:int, input_shape:list=None, activation:str=None, activation_params:dict=None, dense_params:dict=None,
                     norm_layer_type:str=None, norm_layer_position:str='before', norm_layer_params:dict=None, dropout:float=None, 
                     kernel_regularizer:tf.keras.regularizers.Regularizer=None):
     """Add a Dense (fully connected) block containing one linear layer, followed optionally by a normalization layer, an activation function and a Dropout layer, 
     to a `tf.keras.models.Sequential` instance.
 
         ### Args:
             - `input_shape` (list|tuple, optional): Shape of the input disregarding the batch size.
             - `output_size` (int, optional): Number of output features. Defaults to None, in which case it will be input_size.
             - `activation` (str, optional): Activation. It can be an activation function name ("relu","sigmoid","tanh", etc.), an activation layer name ("ReLU", "LeakyReLU",
                 "Softmax", etc.), or a custom Keras Layer class (not instance). Defaults to None.
             - `activation_params` (dict, optional): kwargs to pass to the activation function constructor. Defaults to None. Ignored if `activation` is a lower-case function name.
                 By the way, the slope of the negative section in `LeakyReLU` is `alpha`.
+            - `dense_params` (dict, optional): kwargs to pass to the dense layer constructor. Defaults to None. This will overwrite any other parameters such as regularizers, etc.
             - `norm_layer_type` (str, optional): Type of normalization layer. Defaults to None. Examples: 'BatchNormalization', 'LayerNormalization', etc.
                 It can also be a Keras Layer class (not instance).
             - `norm_layer_position` (str, optional): Position of norm layer relative to activation. Defaults to 'before'. Alternative is 'after'.
             - `norm_layer_params` (dict, optional): kwargs to pass to the norm layer constructor. Defaults to None.
             - `dropout` (float, optional): Dropout rate at the end. Defaults to None. Must be a float between 0 and 1.
             - `kernel_regularizer` (regularizer, optinal): Regularizer to be used for the kernel weights in the layers.
             
@@ -162,18 +173,25 @@
         if isinstance(norm_layer_type, str):
             _norm_layer_module = getattr(tf.keras.layers, norm_layer_type)
         else:
             _norm_layer_module = norm_layer_type
     else:
         _norm_layer_module = None
     
-    if input_shape:
-        model.add(tf.keras.layers.Dense(output_size, input_shape=input_shape, kernel_regularizer=kernel_regularizer))
-    else:
-        model.add(tf.keras.layers.Dense(output_size, kernel_regularizer=kernel_regularizer))
+    
+    _kwargs = {
+        'units': output_size
+    }
+    if input_shape is not None:
+        _kwargs.update({'input_shape':input_shape})
+    if kernel_regularizer is not None:
+        _kwargs.update({'kernel_regularizer':kernel_regularizer})
+    if dense_params is not None:
+        _kwargs.update(dense_params)
+    model.add(tf.keras.layers.Dense(**_kwargs))
         
     if norm_layer_type and norm_layer_position=='before': 
         if norm_layer_params: model.add(_norm_layer_module(**norm_layer_params))
         else: model.add(_norm_layer_module())
         
     if activation: 
         if isinstance(activation, str) and activation.lower()==activation:
```

### Comparing `eznet_keras-1.0.2/eznet_keras/models/keras_smart_module.py` & `eznet_keras-1.1.0/eznet_keras/models/keras_smart_module.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,29 +8,33 @@
     from utils import *
 
 class KerasSmartModel(tf.keras.models.Model):
     
     sample_hparams = {
         'model_name': 'KerasSmartModel',
         'l2_reg': 0.0001,
+        'l1_reg': None,
         'batch_size': 16,
         'epochs': 2,
         'validation_data': 0.1,
         'early_stopping_patience_epochs': 10,
         'learning_rate': 0.0001,
         'exponential_decay_rate': 0.99,
         'loss_function': 'categorical_crossentropy',
         'loss_function_params': None,
         'metrics':['accuracy'],
+        'metrics_params': None,
         'optimizer': 'Adam',
         'optimizer_params': None,
         'checkpoint_path':None,
         'early_stopping_monitor':'loss',
         'early_stopping_mode':'min',
-        'early_stopping_value':1.0e-6
+        'early_stopping_value':1.0e-6,
+        'other_callbacks': None,
+        'custom_schedule': None
     }
     
     def __init__(self, hparams:dict=None):
         """
         Base class for smart, trainable pytorch modules. All hyperparameters are contained within the `hparams`
         dictionary. Some training-related hyperparameters are common across almost all kinds of PyTorch modules,
         which can be overloaded by the child class. The module includes functions for training, evaluation, and
@@ -40,24 +44,33 @@
 
         `net = KerasSmartModel(hparams)` where `hparams` is dictionary of hyperparameters containing the following:
             - `model_name` (str): Name of the model.
             - `batch_size` (int): Minibatch size, the expected input size of the network.
             - `learning_rate` (float): Initial learning rate of training.
             - `exponential_decay_rate` (float): Exponential decay rate for learning rate, if any.
             - `optimizer` (str): Optimizer. Examples are "Adam", "SGD", "RMSprop", "Adagrad", etc. The name of any Keras optimizer can be used.
+                This can also be a custom optimizer class (not instance), in which case `optimizer_params` can be specified for its constructor kwargs.
             - `optimizer_params` (dict): Additional parameters of the optimizer constructor, if any.
             - `epochs` (int): Maximum number of epochs for training.
             - `early_stopping_patience_epochs` (int): Epochs to tolerate unimproved (val) loss, before early stopping (i.e., patience).
-            - `l2_reg` (float): L2 regularization parameter.
-            - `loss_function` (str): Loss function. Examples: "mse", "binary_crossentropy", "categorical_crossentropy", etc. It can also be a Keras loss function instance.
-            - `metrics` (list): list of metrics for Keras compilation. Examples: ['mse'], ['accuracy'], etc. It can also be a Keras metric instance.
+            - `l2_reg` (float): L2 regularization parameter. Defaults to None.
+            - `l1_reg` (float): L1 regularization parameter. Defaults to None.
+            - `loss_function` (str): Loss function. It can be a lower-case name such as "mse", "binary_crossentropy", "categorical_crossentropy", etc.,
+                the name of a `tf.keras.losses` class such as `BinaryCrossentropy`, `CategoricalCrossentropy`, `MeanSquaredError', etc., or a valid loss class (not instance).
+            - `loss_function_params` (dict): Additional kwargs parameters of the loss function constructor, if any. Ignored if the loss function is a lower-case name string.
+            - `metrics` (list): list of metrics for Keras compilation. Each member of the list can be a lower-case metric name such as "mse" or "accuracy", the name of a 
+                `tf.keras.metrics` class such as `Accuracy`, `MeanSquaredError`, etc., or a valid metric class (not instance).
+            - `metrics_params` (list): (list of) additional kwargs parameters of the metrics constructors, if any. Ignored for every metric that is a lower-case name string.
+                If this entry is a single dicitonary rather than a list, it will be broadcast to all metrics in the metrics list.
             - `checkpoint_path` (str): Path to the directory where checkpoints will be saved at every epoch.
             - `early_stopping_monitor` (str): Monitor whose critical value will cause early stopping. Default is 'loss', but 'val_loss' is typically used.
             - `early_stopping_mode` (str): Mode of the parameter whose critical value will be used for early stopping. Deafults to 'min' for any error. 'max' is for accuracy, etc.
             - `early_stopping_value` (float): Value of the monitor at which point training will stop becasue the critical value has been reached.
+            - `other_callbacks` (list): List of other callbacks to be used during training. Defaults to None.
+            - `custom_schedule` (schedule): Custom learning rate schedule inheriting from `tf.keras.optimizers.schedules.LearningRateSchedule`. Defaults to None.
 
         ### Returns
 
         Returns a `tf.keras.models.Model` object that can be trained and used accordingly.
         Run `net.summary()` afterwards to see what you have inside the network.
         
         ### Notes:
@@ -74,48 +87,58 @@
           method.
         """
         super(KerasSmartModel, self).__init__()
         if not hparams: hparams = self.sample_hparams
         self.hparams = hparams
         self._batch_size = int(hparams["batch_size"]) if hparams.get("batch_size") else 32
         self._loss_function = hparams.get("loss_function")
-        # self._loss_function_params = hparams.get("loss_function_params")
-        self._metrics_list = hparams.get("metrics")
+        self._loss_function_params = hparams.get("loss_function_params")
+        self._metrics = hparams.get("metrics")
+        self._metrics_params = hparams.get("metrics_params")
         self._optimizer = hparams.get("optimizer")
         self._optimizer_params = hparams.get("optimizer_params")
         self._early_stopping_patience_epochs = hparams.get("early_stopping_patience_epochs")
         self._learning_rate = hparams.get("learning_rate")
         self._exponential_decay_rate = hparams.get("exponential_decay_rate")
         self._validation_data = hparams.get("validation_data")
         self._epochs = hparams.get("epochs")
-        self._l2_reg = hparams.get("l2_reg") if hparams.get("l2_reg") else 0.0
+        self._l2_reg = hparams.get("l2_reg") if hparams.get("l2_reg") else None
+        self._l1_reg = hparams.get("l1_reg") if hparams.get("l1_reg") else None
         self.history = None
         self.batch_input_shape = (self._batch_size, 1)
         self.batch_output_shape = (self._batch_size, 1)
         self._callbacks = [GarbageCollectionCallback()]
-        self._es = tf.keras.callbacks.EarlyStopping(monitor='val_loss' if 'validation_data' in hparams else 'loss', 
+        self._es = tf.keras.callbacks.EarlyStopping(monitor='val_loss' if hparams.get('validation_data') is not None else 'loss', 
                                                     mode="min", patience=self._early_stopping_patience_epochs) if self._early_stopping_patience_epochs else None
         if self._es:
             self._callbacks.append(self._es)
         self._chkpt = hparams.get("checkpoint_path")
         if self._chkpt:
-            self._chk = tf.keras.callbacks.ModelCheckpoint(self._chkpt, monitor=('val_loss' if 'validation_data' in hparams else 'loss'), 
+            self._chk = tf.keras.callbacks.ModelCheckpoint(self._chkpt, monitor=('val_loss' if hparams.get('validation_data') is not None else 'loss'), 
                                                            verbose=0, save_best_only=True, mode='min')
         else:
             self._chk = None
         if self._chk:
             self._callbacks.append(self._chk)
         self.early_stopping_monitor = hparams.get("early_stopping_monitor")
         self.early_stopping_mode = hparams.get("early_stopping_mode")
         self.early_stopping_value = hparams.get("early_stopping_value")
         if self.early_stopping_monitor:
             self._es_crit = EarlyStopAtCriteria(monitor=self.early_stopping_monitor, mode=self.early_stopping_mode, value=self.early_stopping_value)
             self._callbacks.append(self._es_crit)
         else:
             self._es_crit = None
+        self._other_callbacks = hparams.get("other_callbacks")
+        if self._other_callbacks is not None:
+            assert isinstance(self._other_callbacks, list), "other_callbacks must be a list of callbacks"
+            self._callbacks.extend(self._other_callbacks)
+        self._custom_schedule = hparams.get("custom_schedule")
+        
+    
+        # Construct an empty Sequential model
         self.net = tf.keras.models.Sequential()
     
     
     def call(self, x, *args, **kwargs):
         return self.net(x, *args, **kwargs)
     
     # def build(self):
@@ -135,16 +158,18 @@
     
     def compile_model(self, num_samples=None):
         """Compiles Keras Smart Model based on its constructor hyperparameters
 
         Args:
             num_samples (int, optional): Number of samples. Defaults to None.
         """
-        compile_keras_model(self.net, self._batch_size, self._learning_rate, self._optimizer, self._loss_function, 
-                              self._metrics_list, self._optimizer_params, self._exponential_decay_rate, num_samples)
+        compile_keras_model(self.net, _batchsize=self._batch_size, _learnrate=self._learning_rate, _optimizer=self._optimizer, 
+                            _loss=self._loss_function, _metrics=self._metrics, _optimizer_params=self._optimizer_params,
+                            _loss_params=self._loss_function_params, _metrics_params=self._metrics_params, 
+                            _exponential_decay_rate=self._exponential_decay_rate, num_samples=num_samples, custom_schedule=self._custom_schedule)
             
     def fit_model(self, x_train, y_train, x_val=None, y_val=None, verbose:int=1, **kwargs):
         """Fit (train) the Keras Smart Model to training data.
 
         Args:
             x_train (array): Training inputs
             y_train (array): Training target outputs
@@ -198,23 +223,33 @@
             - `metrics` (list, optional): Metrics list. Defaults to ['loss']. It can also be ['loss','val_loss'] if validation data was provided, or ['accuracy','val_accuracy'].
             - `fig_title` (str, optional): Title of the figure. Defaults to 'model loss'.
             - `saveto` (str, optional): Path to where to save the figure. Defaults to None. Path does not need to exist.
             - `close_after_finish` (bool, optional): Clsoe the figure after saving it with `plt.close()`. Defaults to True. Only applicable if `saveto` is provided.
         """
         plot_keras_model_history(self.history.history, metrics, fig_title, saveto, close_after_finish)
         
-    # def evaluate(self, *args, **kwargs):
-    #     """Evaluate model performance on test data.
+    def evaluate(self, *args, **kwargs):
+        """Evaluate model performance on test data.
+
+        Returns:
+            The same thing that Keras evaluate returns.
+        """
+        return self.net.evaluate(*args, **kwargs)
+    
+    def predict(self, *args, **kwargs):
+        """Predict the outputs given inputs
 
-    #     Returns:
-    #         The same thing that Keras evaluate returns.
-    #     """
-    #     return self.net.evaluate(*args, **kwargs)
-    
-    # def predict(self, *args, **kwargs):
-    #     """Predict the outputs given inputs
-
-    #     Returns:
-    #         Teh same thing that Keras predict returns.
-    #     """
-    #     return self.net.predict(*args, **kwargs)
+        Returns:
+            Teh same thing that Keras predict returns.
+        """
+        return self.net.predict(*args, **kwargs)
+    
+    def make_regularizer(self):
+        if self._l1_reg is not None and self._L1_reg > 0 and (self._l2_reg is None or self._l2_reg == 0): # Only do L1 regularization
+            return tf.keras.regularizers.L1(self._l1_reg)
+        elif self._l2_reg is not None and self._l2_reg > 0 and (self._l1_reg is None or self._l1_reg == 0): # Only do L2 regularization
+            return tf.keras.regularizers.L2(self._l2_reg)
+        elif self._l1_reg is not None and self._l1_reg > 0 and self._l2_reg is not None and self._l2_reg > 0: # Do both L1 and L2 regularization
+            return tf.keras.regularizers.L1L2(self._l1_reg, self._l2_reg)
+        else:
+            return None
```

### Comparing `eznet_keras-1.0.2/eznet_keras/models/recurrent_network.py` & `eznet_keras-1.1.0/eznet_keras/models/recurrent_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,40 +34,47 @@
         'rnn_recurrent_dropout': None,
         'rnn_layer_dropout': 0.1,
         'rnn_params': None,
         # Dense layer parameters
         'include_dense_layers': True,
         'dense_width': 30,
         'dense_depth': 2,
+        'dense_params': None,
         'dense_dropout': 0.2,
         'dense_activation': 'relu',
         'dense_activation_params': None,
         'norm_layer_type': 'BatchNormalization',
         'norm_layer_params': None,
         'norm_layer_position': 'before',
         # Output layer parameters
         'include_output_layer': True,
+        'output_dense_params': None,
         'output_activation': "softmax",
         'output_activation_params': None,
         # Training procedure parameters
         'l2_reg': 0.0001,
+        'l1_reg': None,
         'batch_size': 16,
         'epochs': 2,
         'validation_data': [0.05,'testset'],
         'early_stopping_patience_epochs': 10,
         'learning_rate': 0.001,
         'exponential_decay_rate': 0.95,
         'loss_function': 'categorical_crossentropy',
+        'loss_function_params': None,
         'metrics':['accuracy'],
+        'metrics_params': None,
         'optimizer': 'Adam',
         'optimizer_params': None,
         'checkpoint_path':None,
         'early_stopping_monitor':'loss',
         'early_stopping_mode':'min',
-        'early_stopping_value':1.0e-6
+        'early_stopping_value':1.0e-6,
+        'other_callbacks': None,
+        'custom_schedule': None
     }
     
     def __init__(self, hparams:dict=None):
         """Sequence to Dense network with RNN for time-series classification, regression, and forecasting, as well as NLP applications.
         This network uses any RNN layers as encoders to extract information from input sequences, and (optionally) fully-connected 
         multilayer perceptrons (Dense) to decode the sequence into an output, which can be class probabilitites 
         (timeseries classification), a continuous number (regression), or an unfolded sequence (forecasting) of a 
@@ -125,14 +132,15 @@
             
             
         #### Dense network architecture hyperparameters
         
             - `include_dense_layers` (bool): Whether to include a Dense network after the RNN layers. Default is True.
             - `dense_width` (int|list): (list of) Widths of the Dense network. It can be a number (for all) or a list holding width of each hidden layer.
             - `dense_depth` (int): Depth (number of hidden layers) of the Dense network, not including the output layer.
+            - `dense_params` (dict): (list of) dictionaries of kwargs for the Dense layers' constructors. Default is None.
             - `dense_activation` (str|list): (list of) Activation functions for hidden layers of the Dense network.
                 It can be activation function ("relu", "sigmoid", "softmax", etc.), activation layer ("ReLU", "LeakyReLU", "Softmax", etc.), or a custom Keras layer class 
                 (not instance)
             - `dense_activation_params` (dict|list): (list of) Dictionaries of parameters for the activation function constructors of the Dense network.
                 Ignored if the activation function is a lower-case function name. By the way, for `LeakyReLU`, the left-hand slope is specified by the `alpha` key.
             - `norm_layer_type` (str|list): (list of) Types of normalization layers to use in the dense section, if any. 
                 Options are "BatchNormalization", "LayerNormalization", etc. It can be a layer name or a Keras Layer class (not instance).
@@ -140,38 +148,47 @@
             - `norm_layer_position` (str|list): (list of) Whether the normalization layer should come 'before' or 'after' the activation of each hidden layer in the dense network.
             - `dense_dropout` (float|list): (list of) Dropout rates (if any) for the hidden layers of the Dense network.
 
         #### Output layer hyperparameters
         
             - `include_output_layer` (bool): Whether to include an output layer, regardless of whether there was a Dense network. Default is True.
                 The output layer is a dense layer followed optionally by an activation.
+            - `output_dense_params` (dict): Dictionary of kwargs for the output layer's Dense constructor, if any. Defaults to None.
             - `output_activation` (str): Activation function for the output layer of the Dense network, if any.
                 Like the `dense_activation` key, it can be activation function name, layer name, or a custom Keras Layer class (not instance).
                 **NOTE** If the `loss_function` is `sparse_categorical_crossentropy`, then no output activation is erquired.
                 However, if it is `categorical_crossentropy` (a.k.a. negative log-likelihood), then you must specify an output activation as in "softmax".
             - `output_activation_params` (dict): Dictionary of parameters for the activation function constructor of the output layer.
             
         #### Training procedure hyperparameters
         
             - `batch_size` (int): Minibatch size, the expected input size of the network. Defaults to 32.
             - `learning_rate` (float): Initial learning rate of training. Defaults to 0.001. Will be given directly to the optimization function.
             - `exponential_decay_rate` (float): Exponential decay rate for learning rate, if any.
-            - `optimizer` (str): Optimizer. Examples: 'Adam', 'SGD', 'RMSProp', etc. It can be the name of a Keras optimizer or custom optimizer class. Will be given directly
-                to the `compile` function. If it is custom, it should be a class, not an instance. Constructor kwargs should be given via the next key.
+            - `optimizer` (str): Optimizer. Examples: 'Adam', 'SGD', 'RMSProp', etc. It can be the name of any Keras optimizer class.
+                This can also be a custom optimizer class (not instance), in which case `optimizer_params` can be specified for its constructor kwargs.
             - `optimizer_params` (dict): Additional parameters of the optimizer constructor, if any. Defaults to None.
             - `epochs` (int): Maximum number of epochs for training. Defaults to 2.
             - `early_stopping_patience_epochs` (int): Epochs to tolerate unimproved (val) loss, before early stopping. Defaults to None.
             - `validation_data` (list): Portion of validation data. Should be a tuple like [validation split, dataset as in 'trainset' or 'testset']. Defaults to None.
             - `l2_reg` (float): L2 regularization parameter. Defaults to None.
-            - `loss_function` (str): Loss function. Examples: 'binary_crossentropy', 'categorical_crossentropy', 'mse', etc. Will be given directly to the `compile` function.
-            - `metrics` (list): list of metrics for Keras compilation, such as ['accuracy']. Will be given directly to the `compile` function.
+            - `l1_reg` (float): L1 regularization parameter. Defaults to None.
+            - `loss_function` (str): Loss function. It can be a lower-case name such as "mse", "binary_crossentropy", "categorical_crossentropy", etc.,
+                the name of a `tf.keras.losses` class such as `BinaryCrossentropy`, `CategoricalCrossentropy`, `MeanSquaredError', etc., or a valid loss class (not instance).
+            - `loss_function_params` (dict): Additional kwargs parameters of the loss function constructor, if any. Ignored if the loss function is a lower-case name string.
+            - `metrics` (list): list of metrics for Keras compilation. Each member of the list can be a lower-case metric name such as "mse" or "accuracy", the name of a 
+                `tf.keras.metrics` class such as `Accuracy`, `MeanSquaredError`, etc., or a valid metric class (not instance).
+            - `metrics_params` (list): (list of) additional kwargs parameters of the metrics constructors, if any. Ignored for every metric that is a lower-case name string.
+                If this entry is a single dicitonary rather than a list, it will be broadcast to all metrics in the metrics list.
             - `checkpoint_path` (str): Path to the directory where checkpoints will be saved at every epoch. The path does not need to exist beforehand.
             - `early_stopping_monitor` (str): Monitor whose critical value will cause early stopping. Default is 'loss', but 'val_loss' is typically used.
             - `early_stopping_mode` (str): Mode of the parameter whose critical value will be used for early stopping. Deafults to 'min' for any error. 'max' is for accuracy, etc.
             - `early_stopping_value` (float): Value of the monitor at which point training will stop becasue the critical value has been reached.
+            - `other_callbacks` (list): List of other callbacks to be used during training. Defaults to None.
+            - `custom_schedule` (schedule): Custom learning rate schedule inheriting from `tf.keras.optimizers.schedules.LearningRateSchedule`. Defaults to None.
 
         ### Returns
         
         Returns a `tf.keras.models.Model` object that can be trained and used accordingly.
         Run `net.summary()` afterwards to see what you have inside the network.
         The returned model is an instance of `KerasSmartModel`, which has built-in functions for training, evaluation, etc.
         """
@@ -204,25 +221,27 @@
         self._rnn_layer_dropout = hparams.get("rnn_layer_dropout")        
             
         # Read Dense hyperparameters
         self._include_dense_layers = hparams.get("include_dense_layers") if "include_dense_layers" in hparams else \
             (hparams.get('dense_depth') is not None and hparams.get('dense_depth') > 0)
         self._dense_width = hparams["dense_width"]
         self._dense_depth = hparams["dense_depth"] if hparams.get("dense_depth") else 0
+        self._dense_params = hparams.get("dense_params")
         self._dense_activation = hparams.get("dense_activation")
         self._dense_activation_params = hparams.get("dense_activation_params")
         self._norm_layer_type = hparams.get("norm_layer_type")
         self._norm_layer_params = hparams.get("norm_layer_params")
         self._norm_layer_position = hparams.get("norm_layer_position")
         self._dense_dropout = hparams.get("dense_dropout")
         
         # Read Output hyperparameters
         self._include_output_layer = hparams.get("include_output_layer") if "include_output_layer" in hparams else True
         if not self._include_output_layer:
             assert self._out_features is None, "If `include_output_layer` is False, then `out_features` must be None. Check your hyperparameters."
+        self._output_dense_params = hparams.get("output_dense_params")
         self._output_activation = hparams.get("output_activation")
         self._output_activation_params = hparams.get("output_activation_params")
         
         # Calculate shape-related variables
         self._N = int(self._batch_size)
         self._D = int(2 if self._bidirectional else 1)
         self._H_in = int(self._in_features)
@@ -261,15 +280,15 @@
         # Construct RNN layers
         for i in range(self._rnn_depth):
             _kwargs = {
                 'units': self._H_cell_vec[i],
                 'dropout': self._rnn_input_dropout_vec[i] if self._rnn_input_dropout_vec[i] is not None else 0.0,
                 'recurrent_dropout': self._rnn_recurrent_dropout_vec[i] if self._rnn_recurrent_dropout_vec[i] is not None else 0.0,
                 'return_sequences':(True if self._rnn_depth > 1 else self._final_rnn_return_sequences), 
-                'kernel_regularizer':(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None)
+                'kernel_regularizer':self.make_regularizer()
             }
             if self._rnn_params is not None: 
                 _kwargs.update(self._rnn_params)
             if i != self._rnn_depth-1:
                 _kwargs.update({'return_sequences':True})
             else:
                 _kwargs.update({'return_sequences':self._final_rnn_return_sequences})
@@ -283,34 +302,38 @@
             self.net.add(tf.keras.layers.Flatten())
         
         # Construct Dense Network
         if self._include_dense_layers and self._dense_depth > 0:
                 
             # Generate arrays containing parameters of each Dense Block (Every block contains a linear, normalization, activation, and dropout layer).
             self._dense_width_vec = self._gen_hparam_vec_for_dense(self._dense_width, 'dense_width')
+            self._dense_params_vec = self._gen_hparam_vec_for_dense(self._dense_params, 'dense_params')
             self._dense_activation_vec = self._gen_hparam_vec_for_dense(self._dense_activation, 'dense_activation')
             self._dense_activation_params_vec = self._gen_hparam_vec_for_dense(self._dense_activation_params, 'dense_activation_params')
             self._dense_norm_layer_type_vec = self._gen_hparam_vec_for_dense(self._norm_layer_type, 'norm_layer_type')
             self._dense_norm_layer_params_vec = self._gen_hparam_vec_for_dense(self._norm_layer_params, 'norm_layer_params')
             self._dense_norm_layer_position_vec = self._gen_hparam_vec_for_dense(self._norm_layer_position, 'norm_layer_position')
             self._dense_dropout_vec = self._gen_hparam_vec_for_dense(self._dense_dropout, 'dense_dropout')
             
             # Construct the dense layers
             # in_size = self._dense_input_size
             for i in range(self._dense_depth):
                 out_size = self._dense_width_vec[i]
                 add_dense_block(self.net, output_size=out_size, input_shape=None, activation=self._dense_activation_vec[i], activation_params=self._dense_activation_params_vec[i], 
                         norm_layer_type=self._dense_norm_layer_type_vec[i], norm_layer_position=self._dense_norm_layer_position_vec[i], 
                         norm_layer_params=self._dense_norm_layer_params_vec[i], dropout=self._dense_dropout_vec[i], 
-                        kernel_regularizer=(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None))
+                        kernel_regularizer=self.make_regularizer(), dense_params=self._dense_params_vec[i])
                 # in_size = out_size
         
         # Output layer
         if self._include_output_layer:
-            self.net.add(tf.keras.layers.Dense(self._output_width, kernel_regularizer=(tf.keras.regularizers.L2(self._l2_reg) if self._l2_reg else None)))
+            _kwargs = {'units':self._output_width, 'kernel_regularizer':self.make_regularizer()}
+            if self._output_dense_params is not None:
+                _kwargs.update(self._output_dense_params)
+            self.net.add(tf.keras.layers.Dense(**_kwargs))
             if self._output_activation:
                 if isinstance(self._output_activation, str):
                     if self._output_activation.lower() == self._output_activation:
                         self.net.add(tf.keras.layers.Activation(self._output_activation))
                     elif self._output_activation_params:
                         self.net.add(getattr(tf.keras.layers, self._output_activation)(**self._output_activation_params))
                     else:
```

### Comparing `eznet_keras-1.0.2/eznet_keras/models/var_ae.py` & `eznet_keras-1.1.0/eznet_keras/models/var_ae.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.2/eznet_keras/test.py` & `eznet_keras-1.1.0/eznet_keras/test.py`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.2/eznet_keras/utils.py` & `eznet_keras-1.1.0/eznet_keras/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -62,32 +62,86 @@
     plt.legend(loc='upper right')
     if saveto:
         plt.savefig(make_path(saveto), dpi=600)
         if close_after_finish:
             plt.close()
         
 
+
+
 def compile_keras_model(model, _batchsize:int, _learnrate:float, _optimizer:str, _loss:str, _metrics:list, 
-                          _optimizerparams:dict=None, _learnrate_decay_gamma:float=None, num_samples:int=None):
-    if _learnrate_decay_gamma:
+                          _optimizer_params:dict=None, _loss_params:dict=None, _metrics_params:list=None, _exponential_decay_rate:float=None, num_samples:int=None, custom_schedule=None):
+    if custom_schedule:
+        lr = custom_schedule
+    elif _exponential_decay_rate:
         itersPerEpoch = (num_samples//_batchsize) if num_samples else 1
         sch = tf.keras.optimizers.schedules.ExponentialDecay(initial_learning_rate=_learnrate, 
-        decay_steps=itersPerEpoch, decay_rate=_learnrate_decay_gamma)
+        decay_steps=itersPerEpoch, decay_rate=_exponential_decay_rate)
         lr = sch
     else:
         lr = _learnrate
-    if _optimizerparams:
-        optparam = _optimizerparams
+    
+    _opt_module = getattr(tf.keras.optimizers, _optimizer) if isinstance(_optimizer, str) else _optimizer
+    
+    if _optimizer_params:
+        optparam = _optimizer_params
         # opt = optdict_keras[_optimizer](learning_rate=lr, **optparam)
-        opt = getattr(tf.keras.optimizers, _optimizer)(learning_rate=lr, **optparam)
+        opt = _opt_module(learning_rate=lr, **optparam)
     else:
         # opt = optdict_keras[_optimizer](learning_rate=lr)
-        opt = getattr(tf.keras.optimizers, _optimizer)(learning_rate=lr)
-    model.compile(optimizer=opt, loss=_loss, metrics=_metrics)
+        opt = _opt_module(learning_rate=lr)
+    
+    if isinstance(_loss, str):
+        if _loss.lower()==_loss: # Put it as is
+            _lossfunc = _loss
+        else: # It is the name of a Keras losses class
+            _loss_module = getattr(tf.keras.losses, _loss)
+            if _loss_params:
+                _lossfunc = _loss_module(**_loss_params)
+            else:
+                _lossfunc = _loss_module()
+    else: # It is a custom loss function class
+        if _loss_params:
+            _lossfunc = _loss(**_loss_params)
+        else:
+            _lossfunc = _loss()
+        
     
+    assert isinstance(_metrics, list), "Metrics must be a list of strings or a list of metrics"
+    if _metrics_params and isinstance(_metrics_params, dict):
+        _metrics_params = [_metrics_params]
+    if _metrics_params:
+        assert len(_metrics_params)==1 or len(_metrics_params)==len(_metrics), \
+            "If metrics_params is specified, it must be a list of length 1 or the same length as metrics."
+    if _metrics_params:
+        _metrics_params_vec = _metrics_params if len(_metrics_params)==len(_metrics) else [_metrics_params[0]]*len(_metrics)
+            
+    _metrics_list = []
+    for i,metric in enumerate(_metrics):
+        if isinstance(metric, str):
+            if metric.lower()==metric: # Put it as is
+                metr = metric
+            else: # It is the name of a Keras metrics class
+                _metr_module = getattr(tf.keras.metrics, metric)
+                if _metrics_params_vec[i] is not None:
+                    metr = _metr_module(**_metrics_params_vec[i])
+                else:
+                    metr = _metr_module()
+        else: # It is a custom metric class
+            if _metrics_params_vec[i] is not None:
+                metr = metric(**_metrics_params_vec[i])
+            else:
+                metr = metric()
+        _metrics_list.append(metr)
+    
+    
+    model.compile(optimizer=opt, loss=_lossfunc, metrics=_metrics_list)
+    
+
+
 
 def fit_keras_model(model, x_train, y_train, x_val=None, y_val=None, 
     _batchsize:int=None, _epochs:int=1, _callbacks:list=None, verbose:int=1, **kwargs):
     while True:
         try:
             history = model.fit(x_train, y_train, batch_size=_batchsize, epochs=_epochs, 
                 validation_data=((x_val, y_val) if x_val is not None and y_val is not None else None), verbose=verbose,
```

### Comparing `eznet_keras-1.0.2/eznet_keras.egg-info/PKG-INFO` & `eznet_keras-1.1.0/eznet_keras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eznet-keras
-Version: 1.0.2
+Version: 1.1.0
 Summary: Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc.
 Home-page: https://github.com/pniaz20/eznet_keras
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: tensorflow,keras,deep learning,neural network,keras2cpp
 Classifier: Development Status :: 3 - Alpha
@@ -25,16 +25,16 @@
 
 # ezNet-Keras
 
 Keras (TensorFlow) implementation of **ezNet** ("easy net"), a package containing "easy" implementation of a collection of basic and widely-used deep learning models.  
 This implementation is for Keras (Tensorflow). See [Here](https://github.com/pniaz20/eznet_torch) for an identical PyTorch implementation.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 1.0.2  
-Last Update: July 15, 2023
+Version: 1.1.0  
+Last Update: July 22, 2023
 
 Install with:
 
 ```bash
 pip install eznet-keras
 ```
```

### Comparing `eznet_keras-1.0.2/eznet_keras.egg-info/SOURCES.txt` & `eznet_keras-1.1.0/eznet_keras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eznet_keras-1.0.2/setup.py` & `eznet_keras-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = '1.0.2' 
+VERSION = '1.1.0' 
 DESCRIPTION = "Easily build Keras models: utils for training/testing, built-in ANN, CNN, RNN models, modular Dense and Convolutional blocks, etc."
 
 # Setting up
 setup(
         # the name must match the folder name
         name="eznet_keras", 
         version=VERSION,
```

