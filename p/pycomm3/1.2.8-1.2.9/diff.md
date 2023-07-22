# Comparing `tmp/pycomm3-1.2.8.tar.gz` & `tmp/pycomm3-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycomm3-1.2.8.tar", last modified: Fri Jul  1 14:31:47 2022, max compression
+gzip compressed data, was "pycomm3-1.2.9.tar", last modified: Wed Aug 17 13:44:44 2022, max compression
```

## Comparing `pycomm3-1.2.8.tar` & `pycomm3-1.2.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-07-01 14:31:47.353793 pycomm3-1.2.8/
--rw-rw-rw-   0        0        0     1138 2021-12-01 00:27:13.000000 pycomm3-1.2.8/LICENSE
--rw-rw-rw-   0        0        0       37 2021-12-01 00:27:13.000000 pycomm3-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0    13941 2022-07-01 14:31:47.352795 pycomm3-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    12807 2021-12-01 00:27:13.000000 pycomm3-1.2.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-07-01 14:31:47.215140 pycomm3-1.2.8/pycomm3/
--rw-rw-rw-   0        0        0     1498 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-07-01 14:31:04.000000 pycomm3-1.2.8/pycomm3/_version.py
-drwxrwxrwx   0        0        0        0 2022-07-01 14:31:47.300256 pycomm3-1.2.8/pycomm3/cip/
--rw-rw-rw-   0        0        0     1351 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/cip/__init__.py
--rw-rw-rw-   0        0        0    31314 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/cip/data_types.py
--rw-rw-rw-   0        0        0     6340 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/cip/object_library.py
--rw-rw-rw-   0        0        0     3519 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/cip/pccc.py
--rw-rw-rw-   0        0        0     3710 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/cip/services.py
--rw-rw-rw-   0        0        0    51219 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/cip/status_info.py
--rw-rw-rw-   0        0        0    24151 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/cip_driver.py
--rw-rw-rw-   0        0        0     2521 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/const.py
--rw-rw-rw-   0        0        0     7652 2021-12-07 20:36:14.000000 pycomm3-1.2.8/pycomm3/custom_types.py
--rw-rw-rw-   0        0        0     1945 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/exceptions.py
--rw-rw-rw-   0        0        0     3126 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/logger.py
--rw-rw-rw-   0        0        0    62237 2022-07-01 14:28:59.000000 pycomm3-1.2.8/pycomm3/logix_driver.py
--rw-rw-rw-   0        0        0     4069 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/map.py
-drwxrwxrwx   0        0        0        0 2022-07-01 14:31:47.350786 pycomm3-1.2.8/pycomm3/packets/
--rw-rw-rw-   0        0        0     2285 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/packets/__init__.py
--rw-rw-rw-   0        0        0     6540 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/packets/base.py
--rw-rw-rw-   0        0        0     5600 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/packets/cip.py
--rw-rw-rw-   0        0        0     9054 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/packets/ethernetip.py
--rw-rw-rw-   0        0        0    15736 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/packets/logix.py
--rw-rw-rw-   0        0        0     7581 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/packets/util.py
--rw-rw-rw-   0        0        0        0 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/py.typed
--rw-rw-rw-   0        0        0    26742 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/slc_driver.py
--rw-rw-rw-   0        0        0     2861 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/socket_.py
--rw-rw-rw-   0        0        0     2100 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/tag.py
--rw-rw-rw-   0        0        0     1987 2021-12-01 00:27:13.000000 pycomm3-1.2.8/pycomm3/util.py
-drwxrwxrwx   0        0        0        0 2022-07-01 14:31:47.242191 pycomm3-1.2.8/pycomm3.egg-info/
--rw-rw-rw-   0        0        0    13941 2022-07-01 14:31:46.000000 pycomm3-1.2.8/pycomm3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      769 2022-07-01 14:31:47.000000 pycomm3-1.2.8/pycomm3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-01 14:31:46.000000 pycomm3-1.2.8/pycomm3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-07-01 14:31:46.000000 pycomm3-1.2.8/pycomm3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-07-01 14:31:46.000000 pycomm3-1.2.8/pycomm3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-01 14:31:47.353793 pycomm3-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1701 2021-12-01 00:27:13.000000 pycomm3-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-17 13:44:44.214863 pycomm3-1.2.9/
+-rw-rw-rw-   0        0        0     1138 2021-12-01 00:27:13.000000 pycomm3-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0       37 2021-12-01 00:27:13.000000 pycomm3-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    13941 2022-08-17 13:44:44.213851 pycomm3-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12807 2021-12-01 00:27:13.000000 pycomm3-1.2.9/README.rst
+drwxrwxrwx   0        0        0        0 2022-08-17 13:44:44.153412 pycomm3-1.2.9/pycomm3/
+-rw-rw-rw-   0        0        0     1498 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-08-17 13:44:15.000000 pycomm3-1.2.9/pycomm3/_version.py
+drwxrwxrwx   0        0        0        0 2022-08-17 13:44:44.200839 pycomm3-1.2.9/pycomm3/cip/
+-rw-rw-rw-   0        0        0     1351 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/cip/__init__.py
+-rw-rw-rw-   0        0        0    31314 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/cip/data_types.py
+-rw-rw-rw-   0        0        0     6340 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/cip/object_library.py
+-rw-rw-rw-   0        0        0     3519 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/cip/pccc.py
+-rw-rw-rw-   0        0        0     3710 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/cip/services.py
+-rw-rw-rw-   0        0        0    51219 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/cip/status_info.py
+-rw-rw-rw-   0        0        0    24151 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/cip_driver.py
+-rw-rw-rw-   0        0        0     2521 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/const.py
+-rw-rw-rw-   0        0        0     7652 2021-12-07 20:36:14.000000 pycomm3-1.2.9/pycomm3/custom_types.py
+-rw-rw-rw-   0        0        0     1945 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/exceptions.py
+-rw-rw-rw-   0        0        0     3126 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/logger.py
+-rw-rw-rw-   0        0        0    62237 2022-08-17 13:40:24.000000 pycomm3-1.2.9/pycomm3/logix_driver.py
+-rw-rw-rw-   0        0        0     4069 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/map.py
+drwxrwxrwx   0        0        0        0 2022-08-17 13:44:44.211842 pycomm3-1.2.9/pycomm3/packets/
+-rw-rw-rw-   0        0        0     2285 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/packets/__init__.py
+-rw-rw-rw-   0        0        0     6540 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/packets/base.py
+-rw-rw-rw-   0        0        0     5600 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/packets/cip.py
+-rw-rw-rw-   0        0        0     9054 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/packets/ethernetip.py
+-rw-rw-rw-   0        0        0    15736 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/packets/logix.py
+-rw-rw-rw-   0        0        0     7581 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/packets/util.py
+-rw-rw-rw-   0        0        0        0 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/py.typed
+-rw-rw-rw-   0        0        0    29519 2022-08-17 13:40:48.000000 pycomm3-1.2.9/pycomm3/slc_driver.py
+-rw-rw-rw-   0        0        0     2861 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/socket_.py
+-rw-rw-rw-   0        0        0     2100 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/tag.py
+-rw-rw-rw-   0        0        0     1987 2021-12-01 00:27:13.000000 pycomm3-1.2.9/pycomm3/util.py
+drwxrwxrwx   0        0        0        0 2022-08-17 13:44:44.185943 pycomm3-1.2.9/pycomm3.egg-info/
+-rw-rw-rw-   0        0        0    13941 2022-08-17 13:44:44.000000 pycomm3-1.2.9/pycomm3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2022-08-17 13:44:44.000000 pycomm3-1.2.9/pycomm3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-17 13:44:44.000000 pycomm3-1.2.9/pycomm3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2022-08-17 13:44:44.000000 pycomm3-1.2.9/pycomm3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-08-17 13:44:44.000000 pycomm3-1.2.9/pycomm3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-08-17 13:44:44.215848 pycomm3-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1701 2021-12-01 00:27:13.000000 pycomm3-1.2.9/setup.py
```

### Comparing `pycomm3-1.2.8/LICENSE` & `pycomm3-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/PKG-INFO` & `pycomm3-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycomm3
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python Ethernet/IP library for communicating with Allen-Bradley PLCs.
 Home-page: https://github.com/ottowayi/pycomm3
 Author: Ian Ottoway
 Author-email: ian@ottoway.dev
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pycomm3-1.2.8/README.rst` & `pycomm3-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/__init__.py` & `pycomm3-1.2.9/pycomm3/__init__.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/_version.py` & `pycomm3-1.2.9/pycomm3/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-__version_info__ = (1, 2, 8)
+__version_info__ = (1, 2, 9)
 __version__ = ".".join(f"{x}" for x in __version_info__)
```

### Comparing `pycomm3-1.2.8/pycomm3/cip/__init__.py` & `pycomm3-1.2.9/pycomm3/cip/__init__.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/cip/data_types.py` & `pycomm3-1.2.9/pycomm3/cip/data_types.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/cip/object_library.py` & `pycomm3-1.2.9/pycomm3/cip/object_library.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/cip/pccc.py` & `pycomm3-1.2.9/pycomm3/cip/pccc.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/cip/services.py` & `pycomm3-1.2.9/pycomm3/cip/services.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/cip/status_info.py` & `pycomm3-1.2.9/pycomm3/cip/status_info.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/cip_driver.py` & `pycomm3-1.2.9/pycomm3/cip_driver.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/const.py` & `pycomm3-1.2.9/pycomm3/const.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/custom_types.py` & `pycomm3-1.2.9/pycomm3/custom_types.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/exceptions.py` & `pycomm3-1.2.9/pycomm3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/logger.py` & `pycomm3-1.2.9/pycomm3/logger.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/logix_driver.py` & `pycomm3-1.2.9/pycomm3/logix_driver.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/map.py` & `pycomm3-1.2.9/pycomm3/map.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/packets/__init__.py` & `pycomm3-1.2.9/pycomm3/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/packets/base.py` & `pycomm3-1.2.9/pycomm3/packets/base.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/packets/cip.py` & `pycomm3-1.2.9/pycomm3/packets/cip.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/packets/ethernetip.py` & `pycomm3-1.2.9/pycomm3/packets/ethernetip.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/packets/logix.py` & `pycomm3-1.2.9/pycomm3/packets/logix.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/packets/util.py` & `pycomm3-1.2.9/pycomm3/packets/util.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/slc_driver.py` & `pycomm3-1.2.9/pycomm3/slc_driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -126,21 +126,22 @@
         No idea what this part is, but it starts all messages
         """
         return b"".join(
             (
                 b"\x4b",
                 b"\x02",
                 b"\x20",  # 8-bit class
-                PCCC_PATH,
+                PCCC_PATH,  # b"\x67\x24\x01"
                 b"\x07",
-                self._cfg["vid"],
-                self._cfg["vsn"],
+                self._cfg["vid"], #"vid": b"\x09\x10",
+                self._cfg["vsn"], #"vsn": b"\x09\x10\x19\x71",
             )
         )
 
+
     @with_forward_open
     def read(self, *addresses: str) -> ReadWriteReturnType:
         """
         Reads data file addresses. To read multiple words add the word count to the address using curly braces,
         e.g. ``N120:10{10}``.
 
         Does not track request/response size like the CLXDriver.
@@ -174,16 +175,18 @@
             USINT.encode(int(_tag.get("pos_number", 0))),  # sub-element number
         ]
 
         request = SendUnitDataRequestPacket(self._sequence)
         request.add(b"".join(message_request))
         response = self.send(request)
         self.__log.debug(f"SLC read_tag({tag})")
+        
 
         status = request_status(response.raw)
+
         if status is not None:
             return Tag(_tag["tag"], None, _tag["file_type"], status)
 
         try:
             return _parse_read_reply(_tag, response.raw[SLC_REPLY_START:])
         except ResponseError as err:
             self.__log.exception(f'Failed to parse read reply for {_tag["tag"]}')
@@ -270,24 +273,84 @@
             finally:
                 return typ
         else:
             self.__log.error(
                 f"failed to get processor type: {request_status(response.raw)}",
             )
             return None
+        
+    @with_forward_open
+    def get_datalog_queue(self, num_data_logs, queue_num):
+        data = []
+        
+        for i in range(num_data_logs):        
+            data.append(self._get_datalog(queue_num))
+        
+        #extra read to clear the queue
+        #will thow error in _get_datalog due to Status == None
+        trash = self._get_datalog(queue_num)
+        
+        if data is not None:
+            return data
+        else:
+            raise ResponseError("No Data in Queue")
+        raise ResponseError("Failed to read processor type")
+        
+    def _get_datalog(self, queue_num):
+        msg_request = [
+            b"\x4b",            # Ethernet/IP Service Code
+            b"\x02",            # Request Path Size, 2 words
+            b"\x20",            # Request Path, Path Segment (8-bit Class)
+            b"\x67",            # Request Path, Path Segment, Class (PCCC Class)
+            b"\x24",            # Request Path, Path Segment (8 Bit Instance)
+            b"\x01",            # Request Path, Path Segment, Instance 
+            b"\x07",            # Requestor ID, Length
+            b"\x4d\x00",        # Requestor ID, CIP Vendor ID
+            b"\xa1\x4e\xc3\x30",# Requestor ID, CIP Serial Number
+            b"\x0f",            # PCCC Command Data, CMD code
+            b"\x00",            # PCCC Command Data, Status Code
+            b"\x30\x00",         # PCCC Command Data, Transaction Code
+            b"\xa2",            # PCCC Command Data, Function Code
+            b"\x6d",            # Function Specific Data, Byte Size
+            b"\x00",            # Function Specific Data, File Number
+            b"\xa5",            # Function Specific Data, File Type
+            USINT.encode(queue_num), # Function Specific Data, Element Number (queue to be read)
+            b"\x00",            # Function Specific Data, Sub-Element Number
+        ]
+        
+        request = SendUnitDataRequestPacket(self._sequence)
+        request.add(b"".join(msg_request))
+        response = self.send(request)
 
+        status = request_status(response.raw)
+        
+        if status is None:
+            try:
+                datalog_entry = response.raw[SLC_REPLY_START:]
+                datalog_entry = datalog_entry.decode("UTF-8")
+            except Exception as err:
+                self.__log.exception("Failed to retreive data log")
+            finally:
+                return datalog_entry
+        else:
+            self.__log.error(
+                f"Failed to retreive data log",
+            )
+            return None
+        
+    
     @with_forward_open
     def get_file_directory(self):
         plc_type = self.get_processor_type()
 
         if plc_type is not None:
             sys0_info = _get_sys0_info(plc_type)
             # file_type, element = _get_file_and_element_for_plc_type(plc_type)
             sys0_info["size"] = self._get_file_directory_size(sys0_info)
-
+            
             if sys0_info["size"] is not None:
                 data = self._read_whole_file_directory(sys0_info)
                 return _parse_file0(sys0_info, data)
             else:
                 raise ResponseError("Failed to read file directory size")
         else:
             raise ResponseError("Failed to read processor type")
@@ -429,14 +492,15 @@
         return {
             "file_position": 233,
             "row_size": 10,
             "file_type": b"\x03",
             "size_element": b"\x2b",
             "size_len": b"\x08",
             "size_const": 19968,  # no idea why, but this seems like a const added to the size? wtf?
+            "file_type_queue": b"\xA5",
         }
     else:  # SLC 5/05
         return {
             "file_position": 79,
             "row_size": 10,
             "file_type": b"\x01",
             "size_element": b"\x23",
```

### Comparing `pycomm3-1.2.8/pycomm3/socket_.py` & `pycomm3-1.2.9/pycomm3/socket_.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/tag.py` & `pycomm3-1.2.9/pycomm3/tag.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3/util.py` & `pycomm3-1.2.9/pycomm3/util.py`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/pycomm3.egg-info/PKG-INFO` & `pycomm3-1.2.9/pycomm3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycomm3
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python Ethernet/IP library for communicating with Allen-Bradley PLCs.
 Home-page: https://github.com/ottowayi/pycomm3
 Author: Ian Ottoway
 Author-email: ian@ottoway.dev
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pycomm3-1.2.8/pycomm3.egg-info/SOURCES.txt` & `pycomm3-1.2.9/pycomm3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycomm3-1.2.8/setup.py` & `pycomm3-1.2.9/setup.py`

 * *Files identical despite different names*

