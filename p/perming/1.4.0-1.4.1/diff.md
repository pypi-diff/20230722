# Comparing `tmp/perming-1.4.0-py3-none-any.whl.zip` & `tmp/perming-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13772 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-21 13:32 perming/__init__.py
+Zip file size: 13796 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-21 15:46 perming/__init__.py
 -rw-rw-rw-  2.0 fat      176 b- defN 23-May-29 15:03 perming/_typing.py
--rw-rw-rw-  2.0 fat    22794 b- defN 23-Jul-21 15:04 perming/_utils.py
+-rw-rw-rw-  2.0 fat    22968 b- defN 23-Jul-21 16:03 perming/_utils.py
 -rw-rw-rw-  2.0 fat      568 b- defN 23-May-29 16:53 perming/_version.py
 -rw-rw-rw-  2.0 fat    13988 b- defN 23-Jul-13 04:45 perming/common.py
 -rw-rw-rw-  2.0 fat     5605 b- defN 23-Jul-13 07:33 perming/general.py
--rw-rw-rw-  2.0 fat    10926 b- defN 23-Jul-21 15:09 perming-1.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 15:09 perming-1.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-21 15:09 perming-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      747 b- defN 23-Jul-21 15:09 perming-1.4.0.dist-info/RECORD
-10 files, 55791 bytes uncompressed, 12518 bytes compressed:  77.6%
+-rw-rw-rw-  2.0 fat    10823 b- defN 23-Jul-21 16:38 perming-1.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 16:38 perming-1.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-21 16:38 perming-1.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      747 b- defN 23-Jul-21 16:38 perming-1.4.1.dist-info/RECORD
+10 files, 55862 bytes uncompressed, 12542 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: perming/common.py
 Comment: 
 
 Filename: perming/general.py
 Comment: 
 
-Filename: perming-1.4.0.dist-info/METADATA
+Filename: perming-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: perming-1.4.0.dist-info/WHEEL
+Filename: perming-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: perming-1.4.0.dist-info/top_level.txt
+Filename: perming-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: perming-1.4.0.dist-info/RECORD
+Filename: perming-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perming/__init__.py

```diff
@@ -23,8 +23,8 @@
 COMMON_MODELS = {
     'Regression': Regressier,
     'Binary-classification': Binarier,
     'Multi-classification': Mutipler,
     'Multi-outputs': Ranker
 }
 
-__version__ = '1.4.0'
+__version__ = '1.4.1'
```

## perming/_utils.py

```diff
@@ -234,26 +234,28 @@
                         outputs_val = self.model(val_set[0].to(self.device)) # return value from cuda
                         self.val_loss += self.criterion(outputs_val, val_set[1].to(self.device))
                 self.val_loss /= val_length
                 val_counts = i + 1 + total_step * epoch
 
                 # early stop
                 if early_stop:
-                    bool_val_first: bool = i == 0 and epoch == 0
-                    if bool_val_first: # record first time of val_loss
+                    if val_counts == 1: # record first time of val_loss
                         val_loss_pre = self.val_loss
+                        val_pos_ini = 1
                     else:
                         if val_loss_pre < self.val_loss:
                             val_loss_pre = self.val_loss
+                            val_pos_ini = val_counts # renew val_pos_ini to record the postion of previous lowest loss
                         else:
-                            if val_counts % patience == 0:
+                            if (val_counts - val_pos_ini + 1) == patience:
                                 if val_loss_pre - self.val_loss < tolerance:
                                     self.stop_iter: bool = True
                                 else:
                                     val_loss_pre = self.val_loss
+                                    val_pos_ini = val_counts
                 # console print
                 if (i + 1) % interval == 0:
                     print('Epoch [{}/{}], Step [{}/{}], Training Loss: {:.4f}, Validation Loss: {:.4f}'.format(epoch+1, num_epochs, i+1, total_step, self.train_loss.item(), self.val_loss.item()))
 
             if self.stop_iter:
                 print('Process stop at epoch [{}/{}] with patience {} within tolerance {}'.format(epoch+1, num_epochs, patience, tolerance))
                 break
```

## Comparing `perming-1.4.0.dist-info/METADATA` & `perming-1.4.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,122 +1,124 @@
-Metadata-Version: 2.1
-Name: perming
-Version: 1.4.0
-Summary: The supervised learning framework based on perceptron for tabular data.
-Home-page: https://github.com/linjing-lab/easy-pytorch/tree/main/released_box
-Download-URL: https://github.com/linjing-lab/easy-pytorch/tags
-Author: 林景
-Author-email: linjing010729@163.com
-License: MPL 2.0
-Project-URL: Source, https://github.com/linjing-lab/easy-pytorch/tree/main/released_box/perming
-Project-URL: Tracker, https://github.com/linjing-lab/easy-pytorch/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-Requires-Dist: numpy (>=1.21.0)
-Requires-Dist: joblib (>=1.1.0)
-
-# perming
-
-perming: Perceptron Models Are Training on Windows Platform with Default GPU Acceleration.
-
-- p: use polars or pandas to read dataset.
-- per: perceptron algorithm used as based model.
-- m: models concluding regressier and classifier (binary & multiple).
-- ing: training on windows platform with strong gpu acceleration.
-
-## init backend
- 
-refer to https://pytorch.org/get-started/locally/ and choose the PyTorch that support `cuda` compatible with your Windows. The current software version only supports Windows system.
-
-test with: PyTorch 1.7.1+cu101
-
-## general model
-
-|GENERAL_BOX(Box)|Parameters|Meaning|
-|--|--|--|
-|`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)<br />device: str="cuda"<br />*<br />activation: str="relu"<br />inplace_on: bool=True<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier or Regressier Based on Basic Information of the Dataset Obtained through Data Preprocessing and Feature Engineering.|
-|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
-|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Numpy Dataset into `torch.utils.data.DataLoader`.|
-|train_val|num_epochs: int=2<br />tolerance: float=1e-3<br />patience: int=10<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
-|test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
-|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
-|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
-
-## common models (cuda first)
-
-- Regression
-
-|Regressier|Parameters|Meaning|
-|--|--|--|
-|`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="MSELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Regressier Based on Basic Information of the Regression Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=1`.|
-|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
-|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
-|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
-|test|/|Test Module Only Show with Loss at 3 Stages: Train, Test, Val|
-|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
-|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
-
-- Binary-classification
-
-|Binarier|Parameters|Meaning|
-|--|--|--|
-|`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="BCELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=2`.|
-|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
-|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Binary-classification Dataset with Numpy format into `torch.utils.data.DataLoader`.|
-|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
-|test|sort_by: str="accuracy"<br />sort_state: bool=True|Test Module Show with Correct Class and Loss at 3 Stages: Train, Test, Val|
-|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
-|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
-
-- Multi-classification
-
-|Multipler|Parameters|Meaning|
-|--|--|--|
-|`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes>2`.|
-|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
-|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Multi-classification Dataset with Numpy format into `torch.utils.data.DataLoader`.|
-|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
-|test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
-|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
-|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
-
-- Multi-outputs
-
-|Ranker|Parameters|Meaning|
-|--|--|--|
-|`__init__`|input_: int<br />num_outputs: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="MultiLabelSoftMarginLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Ranker Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with (n_samples, n_outputs).|
-|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
-|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Multi-outputs Dataset with Numpy format into `torch.utils.data.DataLoader`.|
-|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
-|test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
-|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
-|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
-
-> prefer replace shape *(n,1)* with shape *(n,)* using `numpy.squeeze(input_matrix)`
-
-## pip install
-
-download latest version:
-```text
-git clone https://github.com/linjing-lab/easy-pytorch.git
-cd easy-pytorch/released_box
-pip install -e . --verbose
-```
-download stable version:
-```text
-pip install perming --upgrade
-```
+Metadata-Version: 2.1
+Name: perming
+Version: 1.4.1
+Summary: The supervised learning framework based on perceptron for tabular data.
+Home-page: https://github.com/linjing-lab/easy-pytorch/tree/main/released_box
+Download-URL: https://github.com/linjing-lab/easy-pytorch/tags
+Author: 林景
+Author-email: linjing010729@163.com
+License: MPL 2.0
+Project-URL: Source, https://github.com/linjing-lab/easy-pytorch/tree/main/released_box/perming
+Project-URL: Tracker, https://github.com/linjing-lab/easy-pytorch/issues
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+Requires-Dist: numpy (>=1.21.0)
+Requires-Dist: joblib (>=1.1.0)
+
+# perming
+
+perming: Perceptron Models Are Training on Windows Platform with Default GPU Acceleration.
+
+- p: use polars or pandas to read dataset.
+- per: perceptron algorithm used as based model.
+- m: models concluding regressier and classifier (binary & multiple).
+- ing: training on windows platform with strong gpu acceleration.
+
+## init backend
+ 
+refer to https://pytorch.org/get-started/locally/ and choose the PyTorch that support `cuda` compatible with your Windows. The current software version only supports Windows system.
+
+test with: PyTorch 1.7.1+cu101
+
+## general model
+
+|GENERAL_BOX(Box)|Parameters|Meaning|
+|--|--|--|
+|`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)<br />device: str="cuda"<br />*<br />activation: str="relu"<br />inplace_on: bool=True<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier or Regressier Based on Basic Information of the Dataset Obtained through Data Preprocessing and Feature Engineering.|
+|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
+|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Numpy Dataset into `torch.utils.data.DataLoader`.|
+|train_val|num_epochs: int=2<br />tolerance: float=1e-3<br />patience: int=10<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
+|test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
+|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
+|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
+
+## common models (cuda first)
+
+- Regression
+
+|Regressier|Parameters|Meaning|
+|--|--|--|
+|`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="MSELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Regressier Based on Basic Information of the Regression Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=1`.|
+|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
+|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
+|test|/|Test Module Only Show with Loss at 3 Stages: Train, Test, Val|
+|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
+|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
+
+- Binary-classification
+
+|Binarier|Parameters|Meaning|
+|--|--|--|
+|`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="BCELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=2`.|
+|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
+|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Binary-classification Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
+|test|sort_by: str="accuracy"<br />sort_state: bool=True|Test Module Show with Correct Class and Loss at 3 Stages: Train, Test, Val|
+|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
+|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
+
+- Multi-classification
+
+|Multipler|Parameters|Meaning|
+|--|--|--|
+|`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes>2`.|
+|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
+|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Multi-classification Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
+|test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
+|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
+|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
+
+- Multi-outputs
+
+|Ranker|Parameters|Meaning|
+|--|--|--|
+|`__init__`|input_: int<br />num_outputs: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="MultiLabelSoftMarginLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Ranker Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with (n_samples, n_outputs).|
+|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
+|data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Multi-outputs Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|train_val|num_epochs: int=2<br />interval: int=100<br />tolerance: float=1e-3<br />patience: int=10<br />backend: str="threading"<br />n_jobs: int=-1<br />early_stop: bool=False|Using `num_epochs`, `tolerance`, `patience` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
+|test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
+|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
+|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
+
+> prefer replace shape *(n,1)* with shape *(n,)* using `numpy.squeeze(input_matrix)`
+
+## pip install
+
+download latest version:
+```text
+git clone https://github.com/linjing-lab/easy-pytorch.git
+cd easy-pytorch/released_box
+pip install -e . --verbose
+```
+download stable version:
+```text
+pip install perming --upgrade
+```
+
```

