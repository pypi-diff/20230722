# Comparing `tmp/coptpy_stubs-1.1.3-py3-none-any.whl.zip` & `tmp/coptpy_stubs-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12367 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       23 b- defN 23-Jul-03 09:28 coptpy-stubs/__init__.pyi
--rw-rw-r--  2.0 unx   106284 b- defN 23-Jul-03 09:28 coptpy-stubs/coptpy.pyi
--rw-rw-r--  2.0 unx      361 b- defN 23-Jul-03 09:28 coptpy_stubs-1.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-03 09:28 coptpy_stubs-1.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 23-Jul-03 09:28 coptpy_stubs-1.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      479 b- defN 23-Jul-03 09:28 coptpy_stubs-1.1.3.dist-info/RECORD
-6 files, 107252 bytes uncompressed, 11497 bytes compressed:  89.3%
+Zip file size: 12400 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx       23 b- defN 23-Jul-21 15:18 coptpy-stubs/__init__.pyi
+-rw-rw-r--  2.0 unx   107023 b- defN 23-Jul-21 15:18 coptpy-stubs/coptpy.pyi
+-rw-rw-r--  2.0 unx      361 b- defN 23-Jul-21 15:18 coptpy_stubs-1.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-21 15:18 coptpy_stubs-1.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jul-21 15:18 coptpy_stubs-1.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      479 b- defN 23-Jul-21 15:18 coptpy_stubs-1.1.4.dist-info/RECORD
+6 files, 107991 bytes uncompressed, 11530 bytes compressed:  89.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: coptpy-stubs/__init__.pyi
 Comment: 
 
 Filename: coptpy-stubs/coptpy.pyi
 Comment: 
 
-Filename: coptpy_stubs-1.1.3.dist-info/METADATA
+Filename: coptpy_stubs-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: coptpy_stubs-1.1.3.dist-info/WHEEL
+Filename: coptpy_stubs-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: coptpy_stubs-1.1.3.dist-info/top_level.txt
+Filename: coptpy_stubs-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: coptpy_stubs-1.1.3.dist-info/RECORD
+Filename: coptpy_stubs-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## coptpy-stubs/coptpy.pyi

```diff
@@ -3108,14 +3108,23 @@
     def setAttr(
         self,
         attrname: str,
         newvalue: Union[float, Iterable[float],
                         Iterable[Iterable[float]], np.ndarray]
     ) -> None: ...
 
+    def getInfo(self, infoname: str) -> np.ndarray: ...
+
+    def setInfo(
+        self,
+        infoname: str,
+        newval: Union[float, Iterable[float],
+                    Iterable[Iterable[float]], np.ndarray]
+    ) -> None: ...
+    
     # base methods
     def diagonal(
         self,
         offset: int = 0,
         axis1: int = 0,
         axis2: int = 1
     ) -> MConstr: ...
@@ -3175,14 +3184,23 @@
     def setAttr(
         self,
         attrname: str,
         newvalue: Union[float, Iterable[float],
                         Iterable[Iterable[float]], np.ndarray]
     ) -> None: ...
 
+    def getInfo(self, infoname: str) -> np.ndarray: ...
+
+    def setInfo(
+        self,
+        infoname: str,
+        newval: Union[float, Iterable[float],
+                    Iterable[Iterable[float]], np.ndarray]
+    ) -> None: ...
+
     # base methods
     def diagonal(
         self,
         offset: int = 0,
         axis1: int = 0,
         axis2: int = 1
     ) -> MQConstr: ...
@@ -3485,14 +3503,23 @@
     def setAttr(
         self,
         attrname: str,
         newvalue: Union[float, Iterable[float],
                         Iterable[Iterable[float]], np.ndarray]
     ) -> None: ...
 
+    def getInfo(self, infoname: str) -> np.ndarray: ...
+
+    def setInfo(
+        self,
+        infoname: str,
+        newval: Union[float, Iterable[float],
+                    Iterable[Iterable[float]], np.ndarray]
+    ) -> None: ...
+
     def sum(self, axis: int = None) -> MLinExpr: ...
 
     # base methods
     def diagonal(
         self,
         offset: int = 0,
         axis1: int = 0,
```

