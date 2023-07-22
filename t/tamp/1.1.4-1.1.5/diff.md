# Comparing `tmp/tamp-1.1.4.tar.gz` & `tmp/tamp-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamp-1.1.4.tar", max compression
+gzip compressed data, was "tamp-1.1.5.tar", max compression
```

## Comparing `tamp-1.1.4.tar` & `tamp-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-06-29 05:21:12.923381 tamp-1.1.4/LICENSE
--rw-r--r--   0        0        0    17337 2023-06-29 05:21:12.923381 tamp-1.1.4/README.rst
--rw-r--r--   0        0        0     2851 2023-06-29 05:21:12.923381 tamp-1.1.4/build.py
--rw-r--r--   0        0        0     5577 2023-06-29 05:21:36.279327 tamp-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     2806 2023-06-29 05:21:36.283326 tamp-1.1.4/tamp/__init__.py
--rw-r--r--   0        0        0     1619 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/__init__.pyi
--rw-r--r--   0        0        0       57 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/__main__.py
--rw-r--r--   0        0        0       65 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_common.pxd
--rw-r--r--   0        0        0      343 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_common.pyx
--rw-r--r--   0        0        0     4498 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_compressor.pyx
--rw-r--r--   0        0        0     4168 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_decompressor.pyx
--rw-r--r--   0        0        0      850 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_src/tamp/common.c
--rw-r--r--   0        0        0     1791 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_src/tamp/common.h
--rw-r--r--   0        0        0    12165 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_src/tamp/compressor.c
--rw-r--r--   0        0        0     5805 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_src/tamp/compressor.h
--rw-r--r--   0        0        0     9579 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_src/tamp/decompressor.c
--rw-r--r--   0        0        0     2787 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/_c_src/tamp/decompressor.h
--rw-r--r--   0        0        0        0 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/cli/__init__.py
--rw-r--r--   0        0        0     2715 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/cli/main.py
--rw-r--r--   0        0        0     8656 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/compressor.py
--rw-r--r--   0        0        0     7257 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/compressor_viper.py
--rw-r--r--   0        0        0     2802 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/ctamp.pxd
--rw-r--r--   0        0        0     7882 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/decompressor.py
--rw-r--r--   0        0        0     9681 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/decompressor_viper.py
--rw-r--r--   0        0        0        0 2023-06-29 05:21:12.927381 tamp-1.1.4/tamp/py.typed
--rw-r--r--   0        0        0    17949 1970-01-01 00:00:00.000000 tamp-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-22 20:54:52.919725 tamp-1.1.5/LICENSE
+-rw-r--r--   0        0        0    17788 2023-07-22 20:54:52.919725 tamp-1.1.5/README.rst
+-rw-r--r--   0        0        0     2892 2023-07-22 20:54:52.923725 tamp-1.1.5/build.py
+-rw-r--r--   0        0        0     5603 2023-07-22 20:55:20.956011 tamp-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2788 2023-07-22 20:55:20.960011 tamp-1.1.5/tamp/__init__.py
+-rw-r--r--   0        0        0     1619 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/__init__.pyi
+-rw-r--r--   0        0        0       57 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/__main__.py
+-rw-r--r--   0        0        0       65 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_common.pxd
+-rw-r--r--   0        0        0      343 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_common.pyx
+-rw-r--r--   0        0        0     4498 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_compressor.pyx
+-rw-r--r--   0        0        0     4168 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_decompressor.pyx
+-rw-r--r--   0        0        0      829 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_src/tamp/common.c
+-rw-r--r--   0        0        0     1791 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_src/tamp/common.h
+-rw-r--r--   0        0        0    12165 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_src/tamp/compressor.c
+-rw-r--r--   0        0        0     5805 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_src/tamp/compressor.h
+-rw-r--r--   0        0        0     9378 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_src/tamp/decompressor.c
+-rw-r--r--   0        0        0     2787 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/_c_src/tamp/decompressor.h
+-rw-r--r--   0        0        0        0 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/cli/__init__.py
+-rw-r--r--   0        0        0     2715 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/cli/main.py
+-rw-r--r--   0        0        0     8656 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/compressor.py
+-rw-r--r--   0        0        0     6871 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/compressor_viper.py
+-rw-r--r--   0        0        0     2802 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/ctamp.pxd
+-rw-r--r--   0        0        0     7882 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/decompressor.py
+-rw-r--r--   0        0        0     7409 2023-07-22 20:54:52.923725 tamp-1.1.5/tamp/decompressor_viper.py
+-rw-r--r--   0        0        0        0 2023-07-22 20:54:52.927725 tamp-1.1.5/tamp/py.typed
+-rw-r--r--   0        0        0    18400 1970-01-01 00:00:00.000000 tamp-1.1.5/PKG-INFO
```

### Comparing `tamp-1.1.4/LICENSE` & `tamp-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/README.rst` & `tamp-1.1.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -292,38 +292,46 @@
 | Decompression | 54.0               | 0.70  | 0.98 | 0.82         | 0.82            |
 +---------------+--------------------+-------+------+--------------+-----------------+
 
 Heatshrink v0.4.1 was used in these benchmarks.
 When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, tripling the memory requirement.
 Tamp could use a similar indexing to increase compression speed, but has chosen not to to focus on the primary goal of a low-memory compressor.
 
+To give an idea of Tamp's speed on an embedded device, the following table shows compression/decompression in **bytes/second of the first 100KB of enwik8 on a pi pico (rp2040)** at the default 125MHz clock rate.
+This isn't exactly an apples-to-apples comparison because the C benchmark does not use a filesystem (and thusly, reduced overhead) nor dynamic memory allocation, but is good enough to get the idea across.
+
++---------------+---------------------+------------+
+| Action        | tamp                | tamp       |
+|               | (Micropython Viper) | (C)        |
++===============+=====================+============+
+| Compression   | ~4,300              | ~28,500    |
++---------------+---------------------+------------+
+| Decompression | ~42,000             | ~1,042,524 |
++---------------+---------------------+------------+
+
 Binary Size
 ^^^^^^^^^^^
-To give an idea on the resulting binary sizes, Tamp and other libraries were compiled for the Pi Pico.
+To give an idea on the resulting binary sizes, Tamp and other libraries were compiled for the Pi Pico (``armv6m``).
 All libraries were compiled with ``-O3``.
 Numbers reported in bytes.
 
 +--------------------+------------+--------------+---------------------------+
 | Library            | Compressor | Decompressor | Compressor + Decompressor |
 +====================+============+==============+===========================+
-| Tamp (micropython) | 4779       | 4717         | 8262                      |
+| Tamp (micropython) | 4429       | 4205         | 7554                      |
 +--------------------+------------+--------------+---------------------------+
-| Tamp (C)           | 2008       | 1976         | 3848                      |
+| Tamp (C)           | 2008       | 1972         | 3864                      |
 +--------------------+------------+--------------+---------------------------+
 | Heatshrink         | 2956       | 3876         | 6832                      |
 +--------------------+------------+--------------+---------------------------+
 | uzlib              | 2355       | 3963         | 6318                      |
 +--------------------+------------+--------------+---------------------------+
 
 Heatshrink doesn't include a high level API; in an apples-to-apples comparison the Tamp library would be even smaller.
 
-When to use Tamp
-================
-On a Pi Pico (rp2040), the viper implementation of Tamp can compress data at around 4,300 bytes/s when using a 10-bit window. The data can then be decompressed at around 44,100 bytes/s.
-Tamp is good for compressing data on-device. If purely decompressing data on-device, it will nearly always be better to use the micropython-builtin ``zlib.decompress``, when available.
 
 .. |GHA tests| image:: https://github.com/BrianPugh/tamp/workflows/tests/badge.svg
    :target: https://github.com/BrianPugh/tamp/actions?query=workflow%3Atests
    :alt: GHA Status
 .. |Codecov report| image:: https://codecov.io/github/BrianPugh/tamp/coverage.svg?branch=main
    :target: https://codecov.io/github/BrianPugh/tamp?branch=main
    :alt: Coverage
```

### Comparing `tamp-1.1.4/build.py` & `tamp-1.1.5/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         ]
     else:  # UNIX-based systems
         extra_compile_args = [
             "-O3",
             "-Werror",
             "-Wno-unreachable-code-fallthrough",
             "-Wno-deprecated-declarations",
+            "-Wno-parentheses-equality",
         ]
     include_dirs = ["tamp/_c_src/", "tamp/"]
 
     extensions = [
         Extension(
             "tamp._c_compressor",
             [
```

### Comparing `tamp-1.1.4/pyproject.toml` & `tamp-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "tamp"
-version = "1.1.4"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "1.1.5"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/tamp"
 repository = "https://github.com/BrianPugh/tamp"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.rst"
 packages = [{include = "tamp"}]
@@ -63,14 +63,16 @@
 name = "tamp"
 ignore = [
     "__pycache__",
     "*.pyi",
     "*.pyx",
     "*.pxd",
     "*.pyc",
+    "*.so",
+    "*.html",
     "_c_src/",
     "cli/",
     "*.c",
     "*.h",
 ]
 
 [tool.belay.group.dev]
```

### Comparing `tamp-1.1.4/tamp/__init__.py` & `tamp-1.1.5/tamp/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning-plugin handle it.
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 
 
 class ExcessBitsError(Exception):
     """Provided data has more bits than expected ``literal`` bits."""
 
 
 def bit_size(value):
@@ -29,40 +29,42 @@
         return bytearray(size)
 
     chars = b" \x000ei>to<ans\nr/."  # 16 most common chars in dataset
 
     def _gen_stream(xorshift32):
         for _ in range(size >> 3):
             value = next(xorshift32)
-            yield chars[value & 0x0F]
-            yield chars[value >> 4 & 0x0F]
-            yield chars[value >> 8 & 0x0F]
-            yield chars[value >> 12 & 0x0F]
-            yield chars[value >> 16 & 0x0F]
-            yield chars[value >> 20 & 0x0F]
-            yield chars[value >> 24 & 0x0F]
-            yield chars[value >> 28 & 0x0F]
+            for _ in range(8):
+                yield chars[value & 0x0F]
+                value >>= 4
 
     return bytearray(_gen_stream(_xorshift32(seed)))
 
 
 def compute_min_pattern_size(window, literal):
     """Compute whether the minimum pattern length should be 2 or 3."""
+    """
+    # Easy to understand version; commented out for smaller optimized version;
     if window > 15 or window < 8:
         raise ValueError
     if literal == 5:
         return 2 + (window > 10)
     elif literal == 6:
         return 2 + (window > 12)
     elif literal == 7:
         return 2 + (window > 14)
     elif literal == 8:
         return 2
     else:
         raise ValueError
+    """
+    if not (7 < window < 16 and 4 < literal < 9):
+        raise ValueError
+
+    return 2 + (window > (10 + ((literal - 5) << 1)))
 
 
 try:
     from .compressor_viper import Compressor, TextCompressor, compress
 except ImportError:
     try:
         from ._c_compressor import Compressor, TextCompressor, compress
```

### Comparing `tamp-1.1.4/tamp/__init__.pyi` & `tamp-1.1.5/tamp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/_c_compressor.pyx` & `tamp-1.1.5/tamp/_c_compressor.pyx`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/_c_decompressor.pyx` & `tamp-1.1.5/tamp/_c_decompressor.pyx`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/_c_src/tamp/common.c` & `tamp-1.1.5/tamp/_c_src/tamp/common.c`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #include <stdlib.h>
-#include <string.h>
-
 #include "common.h"
 
 static const unsigned char common_characters[] = {
     0x20, 0x00, 0x30, 0x65, 0x69, 0x3e, 0x74, 0x6f,
     0x3c, 0x61, 0x6e, 0x73, 0xa, 0x72, 0x2f, 0x2e
 };
```

### Comparing `tamp-1.1.4/tamp/_c_src/tamp/common.h` & `tamp-1.1.5/tamp/_c_src/tamp/common.h`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/_c_src/tamp/compressor.c` & `tamp-1.1.5/tamp/_c_src/tamp/compressor.c`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/_c_src/tamp/compressor.h` & `tamp-1.1.5/tamp/_c_src/tamp/compressor.h`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/_c_src/tamp/decompressor.c` & `tamp-1.1.5/tamp/_c_src/tamp/decompressor.c`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 
 
 /**
  * @brief Decode a huffman match-size symbol from the decompressor's bit_buffer.
  *
  * Internally updates bit_buffer and bit_buffer_pos.
  *
- * bit_buffer is GUARANTEED to have enough bits to decode something.
+ * bit_buffer MUST have at least 8 bits prior to calling.
  *
- * @return Tamp Status Code.
- *     TAMP_INVALID_SYMBOL if no valid symbol decoded. Buffer is NOT restored.
+ * @returns Decoded match_size
  */
-static int8_t huffman_decode(uint32_t *bit_buffer, uint8_t *bit_buffer_pos){
+static inline int8_t huffman_decode(uint32_t *bit_buffer, uint8_t *bit_buffer_pos){
     uint8_t code;
     uint8_t bit_len;
 
     (*bit_buffer_pos)--;
     code = *bit_buffer >> 31;
     *bit_buffer <<= 1;
     if(TAMP_LIKELY(code == 0))
@@ -178,18 +177,15 @@
             bit_buffer <<= 1;
             bit_buffer_pos--;
 
             // There must be at least 8 bits, otherwise no possible decoding.
             if(TAMP_UNLIKELY(bit_buffer_pos < 8))
                 return TAMP_INPUT_EXHAUSTED;
 
-            if(TAMP_UNLIKELY(match_size = huffman_decode(&bit_buffer, &bit_buffer_pos)) < 0){
-                // Insufficient input
-                return TAMP_INPUT_EXHAUSTED;
-            }
+            match_size = huffman_decode(&bit_buffer, &bit_buffer_pos);
             if(TAMP_UNLIKELY(match_size == FLUSH)){
                 // flush bit_buffer to the nearest byte and skip the remainder of decoding
                 decompressor->bit_buffer = bit_buffer << (bit_buffer_pos & 7);
                 decompressor->bit_buffer_pos = bit_buffer_pos & ~7;  // Round bit_buffer_pos down to nearest multiple of 8.
                 continue;
             }
             if(TAMP_UNLIKELY(bit_buffer_pos < decompressor->conf_window)){
```

### Comparing `tamp-1.1.4/tamp/_c_src/tamp/decompressor.h` & `tamp-1.1.5/tamp/_c_src/tamp/decompressor.h`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/cli/main.py` & `tamp-1.1.5/tamp/cli/main.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/compressor.py` & `tamp-1.1.5/tamp/compressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/compressor_viper.py` & `tamp-1.1.5/tamp/compressor_viper.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 import micropython
 from micropython import const
 
 from . import ExcessBitsError, bit_size, compute_min_pattern_size, initialize_dictionary
 
 # encodes [2, 15] pattern lengths
-huffman_codes = b"\x00\x03\x08\x0b\x14$&+KT\x94\x95\xaa'"
+_HUFFMAN_CODES = b"\x00\x03\x08\x0b\x14$&+KT\x94\x95\xaa'"
 # These bit lengths pre-add the 1 bit for the 0-value is_literal flag.
-huffman_bits = b"\x02\x03\x05\x05\x06\x07\x07\x07\x08\x08\x09\x09\x09\x07"
-FLUSH_CODE = const(0xAB)  # 8 bits
+_HUFFMAN_BITS = b"\x02\x03\x05\x05\x06\x07\x07\x07\x08\x08\x09\x09\x09\x07"
+_FLUSH_CODE = const(0xAB)  # 8 bits
 
 
 def _f_write(f, number, size):
     f.write(number.to_bytes(size, "big"))
 
 
 class Compressor:
@@ -23,46 +23,40 @@
         self,
         f,
         *,
         window=10,
         literal=8,
         dictionary=None,
     ):
+        self._close_f_on_close = False
         if not hasattr(f, "write"):  # It's probably a path-like object.
             f = open(str(f), "wb")
             self._close_f_on_close = True
-        else:
-            self._close_f_on_close = False
 
         self.window_bits = window
         self.literal_bits = literal
 
         self.min_pattern_size = compute_min_pattern_size(window, literal)
-        self.max_pattern_size = self.min_pattern_size + 13
-        self.max_pattern_bytes_exclusive = self.max_pattern_size + 1
-
-        self.f = f
-        self.f_buf = 0
-        self.f_pos = 0
 
         # Window Buffer
         if dictionary:
             if bit_size(len(dictionary) - 1) != window:
                 raise ValueError
             self.window_buf = dictionary
         else:
             self.window_buf = initialize_dictionary(1 << window)
         self.window_pos = 0
 
         # Input Buffer
-        self.input_buf = bytearray(self.max_pattern_size)
+        self.input_buf = bytearray(16)
         self.input_size = 0
         self.input_pos = 0
 
         # Write header
+        self.f = f
         self.f_buf = ((window - 8) << 5 | (literal - 5) << 3 | int(bool(dictionary)) << 2) << (22)
         self.f_pos = 8
 
     @micropython.viper
     def _compress_input_buffer_single(self) -> int:
         bytes_written = 0
         # Viper-ize everything
@@ -71,46 +65,43 @@
         input_pos = int(self.input_pos)
 
         literal_bits = int(self.literal_bits)
         literal_flag = 1 << literal_bits
 
         f_buf = int(self.f_buf)
         f_pos = int(self.f_pos)
-        huffman_bits_ptr8 = ptr8(huffman_bits)
-        huffman_codes_ptr8 = ptr8(huffman_codes)
+        huffman_bits_ptr8 = ptr8(_HUFFMAN_BITS)
+        huffman_codes_ptr8 = ptr8(_HUFFMAN_CODES)
 
         window_bits = int(self.window_bits)
         window_buf = ptr8(self.window_buf)
         window_size = 1 << int(window_bits)
         window_pos = int(self.window_pos)
 
         min_pattern_size = int(self.min_pattern_size)
-        max_pattern_size = int(self.max_pattern_size)
 
         f = self.f
 
         # Find largest match
         search_i = int(0)
         match_size = int(0)
 
         if input_size >= min_pattern_size:
             for window_index in range(window_size - min_pattern_size + 1):
                 if input_buf[input_pos] != window_buf[window_index]:
                     continue  # Significant speed short-cut
 
-                input_index = (input_pos + 1) % max_pattern_size
+                input_index = (input_pos + 1) & 0xF
                 if input_buf[input_index] != window_buf[window_index + 1]:
                     continue  # Small Speed short-cut
 
                 current_match_size = int(2)
                 for k in range(current_match_size, input_size):
-                    input_index = (input_pos + k) % max_pattern_size
-                    if input_buf[input_index] != window_buf[window_index + k]:
-                        break
-                    if window_index + k >= window_size:
+                    input_index = (input_pos + k) & 0xF
+                    if input_buf[input_index] != window_buf[window_index + k] or window_index + k >= window_size:
                         break
                     current_match_size = k + 1
                 if current_match_size > match_size:
                     match_size = current_match_size
                     search_i = window_index
 
                     if match_size == input_size:
@@ -145,15 +136,15 @@
             _f_write(f, f_buf >> 14, 2)
             f_buf = (f_buf & 0x3FFF) << 16
             f_pos -= 16
             bytes_written += 2
 
         for _ in range(match_size):  # Copy pattern into buffer
             window_buf[window_pos] = input_buf[input_pos]
-            input_pos = (input_pos + 1) % max_pattern_size
+            input_pos = (input_pos + 1) & 0xF
             window_pos = (window_pos + 1) % window_size
 
         input_size -= match_size
 
         self.input_size = input_size
         self.input_pos = input_pos
         self.window_pos = window_pos
@@ -168,21 +159,21 @@
         bytes_written = 0
 
         data_l = int(len(data))
         data_p = ptr8(data)
 
         input_buf = ptr8(self.input_buf)
 
-        max_pattern_size = int(self.max_pattern_size)
+        max_pattern_size = int(self.min_pattern_size) + 13
 
         for i in range(data_l):
             input_size = int(self.input_size)
             input_pos = int(self.input_pos)
 
-            pos = (input_pos + input_size) % max_pattern_size
+            pos = (input_pos + input_size) & 0xF
             input_buf[pos] = data_p[i]
             input_size += 1
             self.input_size = input_size
 
             if input_size == max_pattern_size:
                 bytes_written += int(self._compress_input_buffer_single())
         return bytes_written
@@ -190,29 +181,28 @@
     def flush(self, write_token=True):
         bytes_written = 0
         while self.input_size:
             bytes_written += self._compress_input_buffer_single()
 
         if self.f_pos > 0 and write_token:
             self.f_pos += 9
-            self.f_buf |= FLUSH_CODE << (30 - self.f_pos)
+            self.f_buf |= _FLUSH_CODE << (30 - self.f_pos)
 
         while self.f_pos > 0:
             _f_write(self.f, self.f_buf >> 22, 1)
-            self.f_buf = (self.f_buf & 0x03FFFFF) << 8
+            self.f_buf = (self.f_buf & 0x3FFFFF) << 8
             self.f_pos -= 8
             bytes_written += 1
 
         self.f_pos = 0
 
         return bytes_written
 
     def close(self):
-        bytes_written = 0
-        bytes_written += self.flush(write_token=False)
+        bytes_written = self.flush(write_token=False)
         if self._close_f_on_close:
             self.f.close()
         return bytes_written
 
     def __enter__(self):
         return self
```

### Comparing `tamp-1.1.4/tamp/ctamp.pxd` & `tamp-1.1.5/tamp/ctamp.pxd`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/decompressor.py` & `tamp-1.1.5/tamp/decompressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.4/tamp/decompressor_viper.py` & `tamp-1.1.5/tamp/decompressor_viper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 from io import BytesIO
 
 import micropython
+from micropython import const
 
 from . import compute_min_pattern_size, initialize_dictionary
 
+_HUFFMAN_TABLE = b"BBBBBBBBBBBBBBBBeeee\x8a\x8bxxffffmmmmTTTTTTTTyy\x8c\x8fggggCCCCCCCCCCCCCCCC"
+
+_FLUSH = const(15)
+
 
 class Decompressor:
     def __init__(self, f, *, dictionary=None):
+        self._close_f_on_close = False
         if not hasattr(f, "read"):  # It's probably a path-like object.
             f = open(str(f), "rb")
             self._close_f_on_close = True
-        else:
-            self._close_f_on_close = False
 
         self.f = f
         self.f_buf = 0
         self.f_pos = 0
 
         # Read Header
         header = self.f.read(1)[0]
         self.w_bits = (header >> 5) + 8
         self.literal_bits = ((header >> 3) & 0b11) + 5
         uses_custom_dictionary = header & 0b100
         reserved = header & 0b10
         more_header_bytes = header & 0b1
 
-        if reserved:
-            raise NotImplementedError
-
-        if more_header_bytes:
+        if reserved or more_header_bytes:
             raise NotImplementedError
 
         if uses_custom_dictionary:
             if not dictionary:
                 raise ValueError
             self.w_buf = dictionary
         else:
             self.w_buf = initialize_dictionary(1 << self.w_bits)
         self.w_pos = 0
 
         self.min_pattern_size = compute_min_pattern_size(self.w_bits, self.literal_bits)
-        self.max_pattern_size = self.min_pattern_size + 13
 
         self.overflow_buf = bytearray(self.min_pattern_size + 13)
         self.overflow_pos = 0
         self.overflow_size = 0
 
     def readinto(self, buf):
         raise NotImplementedError
 
     @micropython.viper
     def _decompress_into(self, out) -> int:
         """Attempt to fill out, will place into overflow."""
         out_capacity = int(len(out))  # const
         out_buf = ptr8(out)
 
+        huffman_table = ptr8(_HUFFMAN_TABLE)
+
         literal_bits = int(self.literal_bits)
 
         overflow_buf = self.overflow_buf
         overflow_buf_ptr = ptr8(overflow_buf)
         overflow_pos = int(self.overflow_pos)
         overflow_size = int(self.overflow_size)
 
@@ -101,81 +103,42 @@
                 if match_size:
                     if f_pos < (literal_bits + 1):
                         f_buf |= int(f.read(1)[0]) << (22 - f_pos)
                         f_pos += 8
 
                     # Now update buffers from is_literal
                     f_buf = (f_buf << 1) & full_mask
-                    f_pos -= 1
 
                     c = f_buf >> (30 - literal_bits)
                     f_buf = (f_buf << literal_bits) & full_mask
-                    f_pos -= literal_bits
+                    f_pos -= literal_bits + 1
 
                     out_buf[out_pos] = c
                     w_buf_ptr[w_pos] = c
                     out_pos += 1
                 else:
-                    # Read and decode Huffman
-                    # always read; we'll need the bits regardless
-                    f_buf |= int(f.read(1)[0]) << (22 - f_pos)
-                    f_pos += 8
+                    # Read and decode Huffman; we'll need the bits regardless
+                    if f_pos < 9:
+                        f_buf |= int(f.read(1)[0]) << (22 - f_pos)
+                        f_pos += 8
 
                     if f_buf >> 28:
-                        if (f_buf >> 27) == 0b11:
-                            match_size = 1
-                            delta = 2
-                        else:
-                            proposed_code = f_buf >> 25
-                            delta = 4
-                            if proposed_code == 0b1000:
-                                match_size = 2
-                            elif proposed_code == 0b1011:
-                                match_size = 3
-                            else:
-                                if (f_buf >> 24) == 0b10100:
-                                    match_size = 4
-                                    delta = 5
-                                else:
-                                    proposed_code = f_buf >> 23
-                                    delta = 6
-                                    if proposed_code == 0b100100:
-                                        match_size = 5
-                                    elif proposed_code == 0b100110:
-                                        match_size = 6
-                                    elif proposed_code == 0b101011:
-                                        match_size = 7
-                                    elif proposed_code == 0b100111:
-                                        match_size = 13
-                                    else:
-                                        proposed_code = f_buf >> 22
-                                        delta = 7
-                                        if proposed_code == 0b1001011:
-                                            match_size = 8
-                                        elif proposed_code == 0b1010100:
-                                            match_size = 9
-                                        else:
-                                            proposed_code = f_buf >> 21
-                                            delta = 8
-                                            if proposed_code == 0b10010100:
-                                                match_size = 10
-                                            elif proposed_code == 0b10010101:
-                                                match_size = 11
-                                            elif proposed_code == 0b10101010:
-                                                match_size = 12
-                                            elif proposed_code == 0b10101011:
-                                                f_pos = f_buf = 0  # FLUSH
-                                                continue
-                                            else:
-                                                raise RuntimeError("Invalid Huffman code")
-                    else:  # 0b0
+                        code = (f_buf >> 21) & 0x7F
+                        code = 33 if code >= 64 else huffman_table[code]
+                        match_size = code & 0xF
+                        if match_size == _FLUSH:
+                            f_buf = f_pos = 0
+                            continue
+                        delta = code >> 4
+                    else:
                         match_size = 0
                         delta = 1
 
                     token_bits = 1 + delta + w_bits
+
                     while f_pos < token_bits:
                         f_buf |= int(f.read(1)[0]) << (22 - f_pos)
                         f_pos += 8
 
                     # We now absolutely have enough data to decode token.
 
                     match_size += min_pattern_size
```

### Comparing `tamp-1.1.4/PKG-INFO` & `tamp-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tamp
-Version: 1.1.4
+Version: 1.1.5
 Summary: 
 Home-page: https://github.com/BrianPugh/tamp
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -310,38 +310,46 @@
 | Decompression | 54.0               | 0.70  | 0.98 | 0.82         | 0.82            |
 +---------------+--------------------+-------+------+--------------+-----------------+
 
 Heatshrink v0.4.1 was used in these benchmarks.
 When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, tripling the memory requirement.
 Tamp could use a similar indexing to increase compression speed, but has chosen not to to focus on the primary goal of a low-memory compressor.
 
+To give an idea of Tamp's speed on an embedded device, the following table shows compression/decompression in **bytes/second of the first 100KB of enwik8 on a pi pico (rp2040)** at the default 125MHz clock rate.
+This isn't exactly an apples-to-apples comparison because the C benchmark does not use a filesystem (and thusly, reduced overhead) nor dynamic memory allocation, but is good enough to get the idea across.
+
++---------------+---------------------+------------+
+| Action        | tamp                | tamp       |
+|               | (Micropython Viper) | (C)        |
++===============+=====================+============+
+| Compression   | ~4,300              | ~28,500    |
++---------------+---------------------+------------+
+| Decompression | ~42,000             | ~1,042,524 |
++---------------+---------------------+------------+
+
 Binary Size
 ^^^^^^^^^^^
-To give an idea on the resulting binary sizes, Tamp and other libraries were compiled for the Pi Pico.
+To give an idea on the resulting binary sizes, Tamp and other libraries were compiled for the Pi Pico (``armv6m``).
 All libraries were compiled with ``-O3``.
 Numbers reported in bytes.
 
 +--------------------+------------+--------------+---------------------------+
 | Library            | Compressor | Decompressor | Compressor + Decompressor |
 +====================+============+==============+===========================+
-| Tamp (micropython) | 4779       | 4717         | 8262                      |
+| Tamp (micropython) | 4429       | 4205         | 7554                      |
 +--------------------+------------+--------------+---------------------------+
-| Tamp (C)           | 2008       | 1976         | 3848                      |
+| Tamp (C)           | 2008       | 1972         | 3864                      |
 +--------------------+------------+--------------+---------------------------+
 | Heatshrink         | 2956       | 3876         | 6832                      |
 +--------------------+------------+--------------+---------------------------+
 | uzlib              | 2355       | 3963         | 6318                      |
 +--------------------+------------+--------------+---------------------------+
 
 Heatshrink doesn't include a high level API; in an apples-to-apples comparison the Tamp library would be even smaller.
 
-When to use Tamp
-================
-On a Pi Pico (rp2040), the viper implementation of Tamp can compress data at around 4,300 bytes/s when using a 10-bit window. The data can then be decompressed at around 44,100 bytes/s.
-Tamp is good for compressing data on-device. If purely decompressing data on-device, it will nearly always be better to use the micropython-builtin ``zlib.decompress``, when available.
 
 .. |GHA tests| image:: https://github.com/BrianPugh/tamp/workflows/tests/badge.svg
    :target: https://github.com/BrianPugh/tamp/actions?query=workflow%3Atests
    :alt: GHA Status
 .. |Codecov report| image:: https://codecov.io/github/BrianPugh/tamp/coverage.svg?branch=main
    :target: https://codecov.io/github/BrianPugh/tamp?branch=main
    :alt: Coverage
```

