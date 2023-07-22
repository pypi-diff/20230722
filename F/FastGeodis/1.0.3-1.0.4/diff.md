# Comparing `tmp/FastGeodis-1.0.3.tar.gz` & `tmp/FastGeodis-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastGeodis-1.0.3.tar", last modified: Sun Apr 23 20:06:37 2023, max compression
+gzip compressed data, was "FastGeodis-1.0.4.tar", last modified: Sat Jul 22 18:28:58 2023, max compression
```

## Comparing `FastGeodis-1.0.3.tar` & `FastGeodis-1.0.4.tar`

### file list

```diff
@@ -1,65 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.701039 FastGeodis-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.681038 FastGeodis-1.0.3/FastGeodis/
--rw-r--r--   0 runner    (1001) docker     (122)    28532 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/common.h
--rwxr-xr-x   0 runner    (1001) docker     (122)    20550 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/fastgeodis.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8500 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/fastgeodis.h
--rw-r--r--   0 runner    (1001) docker     (122)    13677 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/fastgeodis_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    22686 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/fastgeodis_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (122)    13293 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/geodis_fastmarch.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    16506 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/geodis_pixelqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11364 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/FastGeodis/geodis_toivanen.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.681038 FastGeodis-1.0.3/FastGeodis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21675 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-23 20:06:37.000000 FastGeodis-1.0.3/FastGeodis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21675 2023-04-23 20:06:37.701039 FastGeodis-1.0.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (122)    19445 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.681038 FastGeodis-1.0.3/dependency/fmm/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.685038 FastGeodis-1.0.3/dependency/fmm/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/.github/workflows/cmake.yml
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/.github/workflows/cpplint.yml
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    21350 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.685038 FastGeodis-1.0.3/dependency/fmm/bindings/python/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/bindings/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5796 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/bindings/python/py-fast-marching-method.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/examples/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.685038 FastGeodis-1.0.3/dependency/fmm/examples/cpp/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/examples/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4797 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/examples/cpp/minimal_example.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.685038 FastGeodis-1.0.3/dependency/fmm/examples/python/
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/examples/python/py-fast-marching-minimal-example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.697039 FastGeodis-1.0.3/dependency/fmm/img/
--rw-r--r--   0 runner    (1001) docker     (122)  1901907 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    23780 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_concept.png
--rw-r--r--   0 runner    (1001) docker     (122)    51743 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_dilation_bands.png
--rw-r--r--   0 runner    (1001) docker     (122)    25143 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_eikonal_solvers.png
--rw-r--r--   0 runner    (1001) docker     (122)    24417 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_input_values.png
--rw-r--r--   0 runner    (1001) docker     (122)    35239 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_inside_outside.png
--rw-r--r--   0 runner    (1001) docker     (122)    56744 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/img/fmm_readme_point_source_error.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.673038 FastGeodis-1.0.3/dependency/fmm/include/thinks/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.697039 FastGeodis-1.0.3/dependency/fmm/include/thinks/fast_marching_method/
--rw-r--r--   0 runner    (1001) docker     (122)    81519 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/include/thinks/fast_marching_method/fast_marching_method.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 20:06:37.701039 FastGeodis-1.0.3/dependency/fmm/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    22357 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/eikonal_solvers_test.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/main.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2729 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/py-bindings-test.py
--rw-r--r--   0 runner    (1001) docker     (122)    33623 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/signed_arrival_time_test.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    18622 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/dependency/fmm/tests/util.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-23 20:06:37.701039 FastGeodis-1.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     4666 2023-04-23 20:04:21.000000 FastGeodis-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 18:28:58.765886 FastGeodis-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 18:28:58.761886 FastGeodis-1.0.4/FastGeodis/
+-rw-r--r--   0 runner    (1001) docker     (122)    28532 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/FastGeodis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/FastGeodis/common.h
+-rwxr-xr-x   0 runner    (1001) docker     (122)    20550 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/FastGeodis/fastgeodis.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8500 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/FastGeodis/fastgeodis.h
+-rw-r--r--   0 runner    (1001) docker     (122)    13677 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/FastGeodis/fastgeodis_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    22686 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/FastGeodis/fastgeodis_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    13829 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/FastGeodis/geodis_fastmarch.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16506 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/FastGeodis/geodis_pixelqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11364 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/FastGeodis/geodis_toivanen.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 18:28:58.765886 FastGeodis-1.0.4/FastGeodis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21675 2023-07-22 18:28:58.000000 FastGeodis-1.0.4/FastGeodis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-07-22 18:28:58.000000 FastGeodis-1.0.4/FastGeodis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 18:28:58.000000 FastGeodis-1.0.4/FastGeodis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 18:28:58.000000 FastGeodis-1.0.4/FastGeodis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-22 18:28:58.000000 FastGeodis-1.0.4/FastGeodis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-22 18:28:58.000000 FastGeodis-1.0.4/FastGeodis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21675 2023-07-22 18:28:58.765886 FastGeodis-1.0.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (122)    19445 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 18:28:58.753886 FastGeodis-1.0.4/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 18:28:58.753886 FastGeodis-1.0.4/dependency/fmm/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 18:28:58.753886 FastGeodis-1.0.4/dependency/fmm/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 18:28:58.753886 FastGeodis-1.0.4/dependency/fmm/include/thinks/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 18:28:58.765886 FastGeodis-1.0.4/dependency/fmm/include/thinks/fast_marching_method/
+-rw-r--r--   0 runner    (1001) docker     (122)    81519 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/dependency/fmm/include/thinks/fast_marching_method/fast_marching_method.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-22 18:28:58.765886 FastGeodis-1.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4666 2023-07-22 18:26:33.000000 FastGeodis-1.0.4/setup.py
```

### Comparing `FastGeodis-1.0.3/FastGeodis/__init__.py` & `FastGeodis-1.0.4/FastGeodis/__init__.py`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/FastGeodis/common.h` & `FastGeodis-1.0.4/FastGeodis/common.h`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/FastGeodis/fastgeodis.cpp` & `FastGeodis-1.0.4/FastGeodis/fastgeodis.cpp`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/FastGeodis/fastgeodis.h` & `FastGeodis-1.0.4/FastGeodis/fastgeodis.h`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/FastGeodis/fastgeodis_cpu.cpp` & `FastGeodis-1.0.4/FastGeodis/fastgeodis_cpu.cpp`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/FastGeodis/fastgeodis_cuda.cu` & `FastGeodis-1.0.4/FastGeodis/fastgeodis_cuda.cu`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/FastGeodis/geodis_fastmarch.cpp` & `FastGeodis-1.0.4/FastGeodis/geodis_fastmarch.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -76,30 +76,34 @@
     gy_ptr[0][0][0][0] = -1.0;
     gy_ptr[0][0][1][0] = 1.0;
 
     // tile if channel>1 to have num_filters==channel
     gx = torch::tile(gx, {channel, 1, 1, 1});
     gy = torch::tile(gy, {channel, 1, 1, 1});
 
-    auto imagegx = F::conv2d(image, 
+    // padding to enable 'same' padding for even kernel size
+    // help from: https://github.com/masadcv/PyTorchSamePaddingExplainer
+    auto imagepadx = torch::constant_pad_nd(image, {0, 1, 0, 0}, 0);
+    auto imagepady = torch::constant_pad_nd(image, {0, 0, 0, 1}, 0);
+
+    // dx and dy gradients
+    auto imagegx = F::conv2d(imagepadx, 
                              gx, 
                              F::Conv2dFuncOptions()
                              .stride(1)
-                             .padding(torch::kSame)
                              .groups(channel)
                             );
-
-    auto imagegy = F::conv2d(image, 
+    auto imagegy = F::conv2d(imagepady, 
                              gy, 
                              F::Conv2dFuncOptions()
                              .stride(1)
-                             .padding(torch::kSame)
                              .groups(channel)
                             );
     
+    // combine dx and dy to get gradient
     auto imagegrad = 0.5 * (
         torch::abs(imagegx) + 
         torch::abs(imagegy)
         );
     
     // reduce sum over channel if multiple channels gradient 
     auto imagegradret = torch::sum(imagegrad, 1);
@@ -270,38 +274,43 @@
     gz_ptr[0][0][1][0][0] = 1.0;
 
     // tile if channel>1 to have num_filters==channel
     gx = torch::tile(gx, {channel, 1, 1, 1, 1});
     gy = torch::tile(gy, {channel, 1, 1, 1, 1});
     gz = torch::tile(gz, {channel, 1, 1, 1, 1});
 
-    auto imagegx = F::conv3d(image, 
+    // padding to enable 'same' padding for even kernel size
+    // help from: https://github.com/masadcv/PyTorchSamePaddingExplainer
+    auto imagepadx = torch::constant_pad_nd(image, {0, 1, 0, 0, 0, 0}, 0);
+    auto imagepady = torch::constant_pad_nd(image, {0, 0, 0, 1, 0, 0}, 0);
+    auto imagepadz = torch::constant_pad_nd(image, {0, 0, 0, 0, 0, 1}, 0);
+
+    // dx, dy and dz gradients
+    auto imagegx = F::conv3d(imagepadx, 
                              gx, 
                              F::Conv3dFuncOptions()
                              .stride(1)
-                             .padding(torch::kSame)
                              .groups(channel)
                             );
 
-    auto imagegy = F::conv3d(image, 
+    auto imagegy = F::conv3d(imagepady, 
                              gy, 
                              F::Conv3dFuncOptions()
                              .stride(1)
-                             .padding(torch::kSame)
                              .groups(channel)
                             );
 
-    auto imagegz = F::conv3d(image, 
+    auto imagegz = F::conv3d(imagepadz, 
                              gz, 
                              F::Conv3dFuncOptions()
                              .stride(1)
-                             .padding(torch::kSame)
                              .groups(channel)
                             );
     
+    // combine dx, dy and dz to get gradient
     auto imagegrad = (1.0/3.0) * (
         torch::abs(imagegx) + 
         torch::abs(imagegy) + 
         torch::abs(imagegz)
         );
 
     // reduce sum over channel if multiple channels gradient
```

### Comparing `FastGeodis-1.0.3/FastGeodis/geodis_pixelqueue.cpp` & `FastGeodis-1.0.4/FastGeodis/geodis_pixelqueue.cpp`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/FastGeodis/geodis_toivanen.cpp` & `FastGeodis-1.0.4/FastGeodis/geodis_toivanen.cpp`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/FastGeodis.egg-info/PKG-INFO` & `FastGeodis-1.0.4/FastGeodis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastGeodis
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fast Implementation of Generalised Geodesic Distance Transform for CPU (OpenMP) and GPU (CUDA)
 Home-page: https://github.com/masadcv/FastGeodis
 Author: Muhammad Asad
 Author-email: masadcv@gmail.com
 License: BSD-3-Clause License
 Description: # FastGeodis: Fast Generalised Geodesic Distance Transform
         [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
```

### Comparing `FastGeodis-1.0.3/LICENSE` & `FastGeodis-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/PKG-INFO` & `FastGeodis-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastGeodis
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fast Implementation of Generalised Geodesic Distance Transform for CPU (OpenMP) and GPU (CUDA)
 Home-page: https://github.com/masadcv/FastGeodis
 Author: Muhammad Asad
 Author-email: masadcv@gmail.com
 License: BSD-3-Clause License
 Description: # FastGeodis: Fast Generalised Geodesic Distance Transform
         [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
```

### Comparing `FastGeodis-1.0.3/README.md` & `FastGeodis-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/dependency/fmm/include/thinks/fast_marching_method/fast_marching_method.hpp` & `FastGeodis-1.0.4/dependency/fmm/include/thinks/fast_marching_method/fast_marching_method.hpp`

 * *Files identical despite different names*

### Comparing `FastGeodis-1.0.3/setup.py` & `FastGeodis-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     install_requires = fp.read().splitlines()
 
 # add dependencies folder in include path
 dep_dir = os.path.join(".", "dependency")
 
 setup(
     name="FastGeodis",
-    version="1.0.3",
+    version="1.0.4",
     description="Fast Implementation of Generalised Geodesic Distance Transform for CPU (OpenMP) and GPU (CUDA)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/masadcv/FastGeodis",
     author="Muhammad Asad",
     author_email="masadcv@gmail.com",
     license="BSD-3-Clause License",
```

