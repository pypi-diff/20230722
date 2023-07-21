# Comparing `tmp/gdxpds-1.3.0.tar.gz` & `tmp/gdxpds-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdxpds-1.3.0.tar", last modified: Tue May  9 16:49:26 2023, max compression
+gzip compressed data, was "gdxpds-1.4.0.tar", last modified: Fri Jul 21 22:53:03 2023, max compression
```

## Comparing `gdxpds-1.3.0.tar` & `gdxpds-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.437545 gdxpds-1.3.0/
--rw-rw-rw-   0        0        0     3065 2023-05-09 16:32:48.000000 gdxpds-1.3.0/CHANGES.txt
--rw-rw-rw-   0        0        0     1558 2023-05-09 16:32:48.000000 gdxpds-1.3.0/LICENSE
--rw-rw-rw-   0        0        0       27 2023-05-09 16:32:48.000000 gdxpds-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2214 2023-05-09 16:49:26.436565 gdxpds-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2499 2023-05-09 16:32:48.000000 gdxpds-1.3.0/README.md
--rw-rw-rw-   0        0        0     1854 2023-05-09 16:43:36.000000 gdxpds-1.3.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.370910 gdxpds-1.3.0/bin/
--rw-rw-rw-   0        0        0     2412 2023-05-09 16:32:48.000000 gdxpds-1.3.0/bin/csv_to_gdx.py
--rw-rw-rw-   0        0        0     1631 2023-05-09 16:32:48.000000 gdxpds-1.3.0/bin/gdx_to_csv.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.388131 gdxpds-1.3.0/gdxpds/
--rw-rw-rw-   0        0        0     1598 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/__init__.py
--rw-rw-rw-   0        0        0      426 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/_version.py
--rw-rw-rw-   0        0        0    43114 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/gdx.py
--rw-rw-rw-   0        0        0     4172 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/read_gdx.py
--rw-rw-rw-   0        0        0     6697 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/special.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.433545 gdxpds-1.3.0/gdxpds/test/
--rw-rw-rw-   0        0        0   102107 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/CONVqn.gdx
--rw-rw-rw-   0        0        0   306969 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/OptimalCSPConfig_In.gdx
--rw-rw-rw-   0        0        0  1994352 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/OptimalCSPConfig_Out.gdx
--rw-rw-rw-   0        0        0     1114 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/__init__.py
--rw-rw-rw-   0        0        0     2851 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/all_generator_properties_input.gdx
--rw-rw-rw-   0        0        0      507 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/annual_generation.csv
--rw-rw-rw-   0        0        0      342 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/conftest.py
--rw-rw-rw-   0        0        0      507 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/installed_capacity.csv
--rw-rw-rw-   0        0        0     4671 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_conversions.py
--rw-rw-rw-   0        0        0     1559 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_read.py
--rw-rw-rw-   0        0        0      806 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_session.py
--rw-rw-rw-   0        0        0     5999 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_specials.py
--rw-rw-rw-   0        0        0    17494 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_write.py
--rw-rw-rw-   0        0        0     5589 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/tools.py
--rw-rw-rw-   0        0        0     4702 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/write_gdx.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.398573 gdxpds-1.3.0/gdxpds.egg-info/
--rw-rw-rw-   0        0        0     2214 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      771 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 16:49:26.437545 gdxpds-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-05-09 16:40:27.000000 gdxpds-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 22:53:03.967294 gdxpds-1.4.0/
+-rw-rw-rw-   0        0        0     3258 2023-07-21 22:52:18.000000 gdxpds-1.4.0/CHANGES.txt
+-rw-rw-rw-   0        0        0     1558 2023-07-21 22:52:18.000000 gdxpds-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-07-21 22:52:18.000000 gdxpds-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2214 2023-07-21 22:53:03.964676 gdxpds-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2499 2023-07-21 22:52:18.000000 gdxpds-1.4.0/README.md
+-rw-rw-rw-   0        0        0     1854 2023-07-21 22:52:18.000000 gdxpds-1.4.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 22:53:03.834916 gdxpds-1.4.0/bin/
+-rw-rw-rw-   0        0        0     2412 2023-07-21 22:52:18.000000 gdxpds-1.4.0/bin/csv_to_gdx.py
+-rw-rw-rw-   0        0        0     1631 2023-07-21 22:52:18.000000 gdxpds-1.4.0/bin/gdx_to_csv.py
+drwxrwxrwx   0        0        0        0 2023-07-21 22:53:03.869053 gdxpds-1.4.0/gdxpds/
+-rw-rw-rw-   0        0        0     1614 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/__init__.py
+-rw-rw-rw-   0        0        0      426 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/_version.py
+-rw-rw-rw-   0        0        0    43930 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/gdx.py
+-rw-rw-rw-   0        0        0     5848 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/read_gdx.py
+-rw-rw-rw-   0        0        0     6697 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/special.py
+drwxrwxrwx   0        0        0        0 2023-07-21 22:53:03.959676 gdxpds-1.4.0/gdxpds/test/
+-rw-rw-rw-   0        0        0   102107 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/CONVqn.gdx
+-rw-rw-rw-   0        0        0   306969 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/OptimalCSPConfig_In.gdx
+-rw-rw-rw-   0        0        0  1994352 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/OptimalCSPConfig_Out.gdx
+-rw-rw-rw-   0        0        0     1114 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/__init__.py
+-rw-rw-rw-   0        0        0     2851 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/all_generator_properties_input.gdx
+-rw-rw-rw-   0        0        0      507 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/annual_generation.csv
+-rw-rw-rw-   0        0        0      342 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/conftest.py
+-rw-rw-rw-   0        0        0      507 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/installed_capacity.csv
+-rw-rw-rw-   0        0        0     4671 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/test_conversions.py
+-rw-rw-rw-   0        0        0     2058 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/test_read.py
+-rw-rw-rw-   0        0        0      806 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/test_session.py
+-rw-rw-rw-   0        0        0     5999 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/test_specials.py
+-rw-rw-rw-   0        0        0    17494 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/test/test_write.py
+-rw-rw-rw-   0        0        0     5589 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/tools.py
+-rw-rw-rw-   0        0        0     4702 2023-07-21 22:52:18.000000 gdxpds-1.4.0/gdxpds/write_gdx.py
+drwxrwxrwx   0        0        0        0 2023-07-21 22:53:03.892265 gdxpds-1.4.0/gdxpds.egg-info/
+-rw-rw-rw-   0        0        0     2214 2023-07-21 22:53:03.000000 gdxpds-1.4.0/gdxpds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      771 2023-07-21 22:53:03.000000 gdxpds-1.4.0/gdxpds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 22:53:03.000000 gdxpds-1.4.0/gdxpds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-07-21 22:53:03.000000 gdxpds-1.4.0/gdxpds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 22:53:03.000000 gdxpds-1.4.0/gdxpds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 22:53:03.968259 gdxpds-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-07-21 22:52:18.000000 gdxpds-1.4.0/setup.py
```

### Comparing `gdxpds-1.3.0/CHANGES.txt` & `gdxpds-1.4.0/CHANGES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+v1.4.0, 07/21/23 -- add get_data_types function that maps symbol name to gdx.GamsDataType; 
+                    add load_set_text kwarg to gdx.GdxSymbol.load, to_dataframe, and to_dataframes
 v1.3.0, 05/09/23 -- performance improvements (faster read and write)
                     GAMS directory finder improvements
                     documentation improvements
                     skip over individual GdxSymbols that fail to load
                     drop support for Python versions < 3.7
                     various minor improvements and bug fixes                                        
 v1.2.0, 09/18/20 -- search for GAMS in more places, especially on Windows
```

### Comparing `gdxpds-1.3.0/LICENSE` & `gdxpds-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/PKG-INFO` & `gdxpds-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdxpds
-Version: 1.3.0
+Version: 1.4.0
 Summary: gdx-pandas is a python package to translate between gdx (GAMS data) and pandas
 Home-page: https://github.com/NREL/gdx-pandas
 Author: Elaine T. Hale
 Author-email: elaine.hale@nrel.gov
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: admin
```

### Comparing `gdxpds-1.3.0/README.md` & `gdxpds-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/README.txt` & `gdxpds-1.4.0/README.txt`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/bin/csv_to_gdx.py` & `gdxpds-1.4.0/bin/csv_to_gdx.py`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/bin/gdx_to_csv.py` & `gdxpds-1.4.0/bin/gdx_to_csv.py`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/__init__.py` & `gdxpds-1.4.0/gdxpds/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,9 +43,9 @@
         gams_dir = GamsDirFinder().gams_dir
     except: pass
     logger.warning(f"Unable to load gdxcc with default GAMS directory '{gams_dir}'. "
                    "You may need to explicitly call gdxpds.load_gdxcc(gams_dir) "
                    "before importing pandas to avoid a library conflict.")
 
 
-from gdxpds.read_gdx import to_dataframes, list_symbols, to_dataframe
+from gdxpds.read_gdx import to_dataframes, list_symbols, to_dataframe, get_data_types
 from gdxpds.write_gdx import to_gdx
```

### Comparing `gdxpds-1.3.0/gdxpds/gdx.py` & `gdxpds-1.4.0/gdxpds/gdx.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,15 @@
             ret, name, dims, data_type = gdxcc.gdxSymbolInfo(self.H,index)
             if ret != 1:
                 raise GdxError(self.H,f"Could not get symbol info for symbol {index}")
             try:
                 sym = GdxSymbol(name,data_type,dims=dims,file=self,index=index)
                 self.append(sym)
             except Exception as e:
-                logger.error(f"Unable to initialize GdxSymbol {name!r}, because {e}. SKIPPING.")
+                logger.error(f"Unable to initialize GdxSymbol {name!r}, because {e}. SKIPPING.")            
 
         # read all symbols if not lazy_load
         if not self.lazy_load:
             for symbol in self:
                 symbol.load()
         return
 
@@ -552,15 +552,18 @@
         self._data_type = GamsDataType(data_type)
         self._variable_type = None; self.variable_type = variable_type
         self._equation_type = None; self.equation_type = equation_type
         self._dataframe = None; self._dims = None
         self.dims = dims       
         assert self._dataframe is not None
         self._file = file
-        self._index = index        
+        self._index = index       
+
+        # adding this flag to implement ability to load set text instead of boolean values
+        self._fixup_set_vals = True
 
         if self.file is not None:
             # reading from file
             # get additional meta-data
             ret, records, userinfo, description = gdxcc.gdxSymbolInfoX(self.file.H,self.index)
             if ret != 1:
                 raise GdxError(self.file.H,"Unable to get extended symbol information for {}".format(self.name))
@@ -946,15 +949,17 @@
 
         colname = self._dataframe.columns[-1]
         assert colname == self.value_col_names[0], f"Unexpected final column {colname!r} in Set dataframe"
         if self._dataframe[colname].isnull().values.any():
             logger.warning(f"Filling null values in {self} with True. To be "
                 "filled:\n{self._dataframe[self._dataframe[colname].isnull()]}")
             replace_df_column(self._dataframe, colname, self._dataframe[colname].fillna(value=True))
-        replace_df_column(self._dataframe,colname,self._dataframe[colname].apply(lambda x: c_bool(x)))
+        if self._fixup_set_vals:
+            replace_df_column(self._dataframe,colname,self._dataframe[colname].apply(lambda x: c_bool(x)))
+        self._fixup_set_vals = True
         return
 
     @property
     def num_records(self):
         """
         Number of rows in the data table, per the DataFrame if :py:attr:`loaded`, or per GAMS.
 
@@ -982,17 +987,24 @@
         s += ", " + self.description    
         s += ", " + self.full_typename    
         s += ", {} records".format(self.num_records)
         s += ", {} dims {}".format(self.num_dims, self.dims)
         s += ", loaded" if self.loaded else ", not loaded"
         return s
 
-    def load(self):
+    def load(self, load_set_text=False):
         """
-        Loads this :py:class:`GdxSymbol` from its :py:attr:`file`
+        Loads this :py:class:`GdxSymbol` from its :py:attr:`file`, thereby popluating
+        :py:attr:`dataframe`.
+
+        Parameters
+        ----------
+        load_set_text : bool
+            If True (default is False) and this symbol is a :class:`GamsDataType.Set <GamsDataType>`,
+            loads the GDX Text field into the :py:attr:`dataframe` rather than a `c_bool`.
         """
         if self.loaded:
             logger.info("Nothing to do. Symbol already loaded.")
             return
         if not self.file:
             raise Error("Cannot load {} because there is no file pointer".format(repr(self)))
         if not self.index:
@@ -1007,16 +1019,21 @@
 
         def reader():
             handle = self.file.H
             for i in range(records):
                 yield gdxcc.gdxDataReadStr(handle)
 
         vc = self.value_cols  # do this for speed in the next line
-        data = [elements + [values[col_ind] for col_name, col_ind in vc] for ret, elements, values, afdim in reader()]
-        # gdxdict called gdxGetElemText here, but I do not currently see value in doing that
+        if load_set_text and (self.data_type == GamsDataType.Set):
+            data = [elements + [gdxcc.gdxGetElemText(self.file.H,int(values[col_ind]))[1] 
+                                for _col_name, col_ind in vc] 
+                    for _ret, elements, values, _afdim in reader()]
+            self._fixup_set_vals = False
+        else:
+            data = [elements + [values[col_ind] for col_name, col_ind in vc] for ret, elements, values, afdim in reader()]
         self.dataframe = data
         if not self.data_type in (GamsDataType.Set, GamsDataType.Alias):
             self.dataframe = special.convert_gdx_to_np_svs(self.dataframe, self.num_dims)
         self._loaded = True
         return
 
     def unload(self):
```

### Comparing `gdxpds-1.3.0/gdxpds/read_gdx.py` & `gdxpds-1.4.0/gdxpds/write_gdx.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,132 +1,129 @@
-from collections import OrderedDict
 import logging
+from numbers import Number
 
 # gdxpds needs to be imported before pandas to try to avoid library conflict on 
 # Linux that causes a segmentation fault.
 from gdxpds.tools import Error
-from gdxpds.gdx import GdxFile
+from gdxpds.gdx import GdxFile, GdxSymbol, GAMS_VALUE_COLS_MAP, GamsDataType
+
+import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 class Translator(object):
-    def __init__(self,gdx_file,gams_dir=None,lazy_load=False):
-        self.__gdx = GdxFile(gams_dir=gams_dir,lazy_load=lazy_load)
-        self.__gdx.read(gdx_file)
-        self.__dataframes = None
+    def __init__(self,dataframes,gams_dir=None):
+        self.dataframes = dataframes
+        self.__gams_dir=None
 
     def __exit__(self, *args):
-        self.__gdx.__exit__(self, *args)
+        if self.__gdx is not None:
+            self.__gdx.__exit__(self, *args)
 
     def __del__(self):
-        self.__gdx.__del__()
+        if self.__gdx is not None:
+            self.__gdx.__del__()
 
     @property
-    def gams_dir(self):
-        return self.gdx.gams_dir
+    def dataframes(self):
+        return self.__dataframes
 
-    @gams_dir.setter
-    def gams_dir(self, value):
-        self.gdx.gams_dir = value
+    @dataframes.setter
+    def dataframes(self,value):
+        err_msg = "Expecting map of name, pandas.DataFrame pairs."
+        try:
+            for symbol_name, df in value.items():
+                if not isinstance(symbol_name, str): raise Error(err_msg)
+                if not isinstance(df, pd.DataFrame): raise Error(err_msg)
+        except AttributeError: raise Error(err_msg)
+        self.__dataframes = value
+        self.__gdx = None
 
     @property
-    def gdx_file(self):
-        return self.gdx.filename
+    def gams_dir(self):
+        return self.__gams_dir
 
-    @gdx_file.setter
-    def gdx_file(self,value):
-        self.__gdx.__del__()
-        self.__gdx = GdxFile(gams_dir=self.gdx.gams_dir,lazy_load=self.gdx.lazy_load)
-        self.__gdx.read(value)
-        self.__dataframes = None
+    @gams_dir.setter
+    def gams_dir(self, value):
+        self.__gams_dir = value
 
     @property
     def gdx(self):
+        if self.__gdx is None:
+            self.__gdx = GdxFile(gams_dir=self.__gams_dir)
+            for symbol_name, df in self.dataframes.items():
+                self.__add_symbol_to_gdx(symbol_name, df)
         return self.__gdx
 
-    @property
-    def dataframes(self):
-        if self.__dataframes is None:
-            self.__dataframes = OrderedDict()
-            for symbol in self.__gdx:
-                if not symbol.loaded:
-                    symbol.load()
-                self.__dataframes[symbol.name] = symbol.dataframe.copy()
-        return self.__dataframes
-
-    @property
-    def symbols(self):
-        return [symbol_name for symbol_name in self.gdx]
-
-    def dataframe(self, symbol_name):
-        if not symbol_name in self.gdx:
-            raise Error("No symbol named '{}' in '{}'.".format(symbol_name, self.gdx_file))
-        if not self.gdx[symbol_name].loaded:
-            self.gdx[symbol_name].load()
-        # This was returning { symbol_name: dataframe }, which seems intuitively off.
-        return self.gdx[symbol_name].dataframe.copy()
-
-def to_dataframes(gdx_file,gams_dir=None):
-    """
-    Primary interface for converting a GAMS GDX file to pandas DataFrames.
-
-    Parameters
-    ----------
-    gdx_file : pathlib.Path or str
-        Path to the GDX file to read
-    gams_dir : None or pathlib.Path or str
-        optional path to GAMS directory
+    def save_gdx(self,path,gams_dir=None):
+        if gams_dir is not None:
+            self.__gams_dir=gams_dir
+        self.gdx.write(path)
+
+    def __add_symbol_to_gdx(self, symbol_name, df):
+        data_type, num_dims = self.__infer_data_type(symbol_name,df)
+        logger.info("Inferred data type of {} to be {}.".format(symbol_name,data_type.name))
+
+        self.__gdx.append(GdxSymbol(symbol_name,data_type,dims=num_dims))
+        self.__gdx[symbol_name].dataframe = df
+        return
+
+    def __infer_data_type(self,symbol_name,df):
+        """
+        Returns
+        -------
+        (gdxpds.GamsDataType, int)
+            symbol type and number of dimensions implied by df
+        """
+        # See if structure implies that symbol_name may be a Variable or an Equation
+        # If so, break tie based on naming convention--Variables start with upper case, 
+        # equations start with lower case
+        var_or_eqn = False        
+        df_col_names = df.columns
+        var_eqn_col_names = [col_name for col_name, col_ind in GAMS_VALUE_COLS_MAP[GamsDataType.Variable]]
+        if len(df_col_names) >= len(var_eqn_col_names):
+            # might be variable or equation
+            var_or_eqn = True
+            trunc_df_col_names = df_col_names[len(df_col_names) - len(var_eqn_col_names):]
+            for i, df_col in enumerate(trunc_df_col_names):
+                if df_col and (df_col.lower() != var_eqn_col_names[i].lower()):
+                    var_or_eqn = False
+                    break
+            if var_or_eqn:
+                num_dims = len(df_col_names) - len(var_eqn_col_names)
+                if symbol_name[0].upper() == symbol_name[0]:
+                    return GamsDataType.Variable, num_dims
+                else:
+                    return GamsDataType.Equation, num_dims
+
+        # Parameter or set
+        num_dims = len(df_col_names) - 1
+        if len(df.index) > 0:
+            if isinstance(df.iloc[0,-1],Number):
+                return GamsDataType.Parameter, num_dims
+        return GamsDataType.Set, num_dims
 
-    Returns
-    -------
-    dict of str to pd.DataFrame
-        Returns a dict of Pandas DataFrames, one item for each symbol in the GDX
-        file, keyed with the symbol name.
-    """
-    dfs = Translator(gdx_file,gams_dir=gams_dir).dataframes
-    return dfs
 
-def list_symbols(gdx_file,gams_dir=None):
+def to_gdx(dataframes,path=None,gams_dir=None):
     """
-    Returns the list of symbols available in gdx_file.
+    Creates a :py:class:`gdxpds.gdx.GdxFile` from dataframes and optionally writes it to path
 
     Parameters
     ----------
-    gdx_file : pathlib.Path or str
-        Path to the GDX file to read
+    dataframes : dict of str to pd.DataFrame
+        symbol name to pd.DataFrame dict to be compiled into a single gdx file. Each DataFrame 
+        is assumed to represent a single set or parameter. The last column must be the parameter's
+        value, or the set's listing of True/False, and must be labeled as (case insensitive) 
+        'value'.
+    path : None or pathlib.Path or str
+        If provided, the gdx file will be written to this path
     gams_dir : None or pathlib.Path or str
-        optional path to GAMS directory
 
     Returns
     -------
-    list of str
-        List of symbol names
+    :py:class:`gdxpds.gdx.GdxFile`
     """
-    symbols = Translator(gdx_file,gams_dir=gams_dir,lazy_load=True).symbols
-    return symbols
+    translator = Translator(dataframes,gams_dir=gams_dir)
+    if path is not None:
+        translator.save_gdx(path)
+    return translator.gdx
 
-def to_dataframe(gdx_file,symbol_name,gams_dir=None,old_interface=True):
-    """
-    Interface for getting the data for a single symbol
-
-    Parameters
-    ----------
-    gdx_file : pathlib.Path or str
-        Path to the GDX file to read
-    symbol_name : str
-        Name of the symbol whose data are to be read
-    gams_dir : None or pathlib.Path or str
-        optional path to GAMS directory
-    old_interface : bool
-        Whether to use the old interface and return a dict, or the new interface, 
-        and simply return a pd.DataFrame
-    
-    Returns
-    -------
-    dict of str to pd.DataFrame OR pd.DataFrame
-        If old_interface (the default), returns a dict with a single entry, 
-        where the key is symbol_name and the value is the corresponding 
-        pd.DataFrame. Otherwise (if not old_interface), returns just the 
-        pd.DataFrame.
-    """
-    df = Translator(gdx_file,gams_dir=gams_dir,lazy_load=True).dataframe(symbol_name)
-    return {symbol_name: df} if old_interface else df
```

### Comparing `gdxpds-1.3.0/gdxpds/special.py` & `gdxpds-1.4.0/gdxpds/special.py`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/test/CONVqn.gdx` & `gdxpds-1.4.0/gdxpds/test/CONVqn.gdx`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/test/OptimalCSPConfig_In.gdx` & `gdxpds-1.4.0/gdxpds/test/OptimalCSPConfig_In.gdx`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/test/OptimalCSPConfig_Out.gdx` & `gdxpds-1.4.0/gdxpds/test/OptimalCSPConfig_Out.gdx`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/test/__init__.py` & `gdxpds-1.4.0/gdxpds/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/test/all_generator_properties_input.gdx` & `gdxpds-1.4.0/gdxpds/test/all_generator_properties_input.gdx`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/test/test_conversions.py` & `gdxpds-1.4.0/gdxpds/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/test/test_read.py` & `gdxpds-1.4.0/gdxpds/test/test_read.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 
 import pytest
 
 import gdxpds.gdx
-from gdxpds import to_dataframes
+from gdxpds import to_dataframes, list_symbols, get_data_types
 from gdxpds.test import base_dir
 
 logger = logging.getLogger(__name__)
 
 def test_read():
     filename = 'all_generator_properties_input.gdx'
     gdx_file = os.path.join(base_dir,filename)
@@ -22,15 +22,31 @@
         to_dataframes(None)
     assert "Could not open None" in str(excinfo.value)
 
 def test_read_path():
     filename = 'all_generator_properties_input.gdx'
     from pathlib import Path
     gdx_file = Path(base_dir) / filename
-    to_dataframes(gdx_file)
+    
+    symbol_names = list_symbols(gdx_file)
+    n = len(symbol_names) 
+    assert isinstance(symbol_names[0], str)
+    assert n == 7
+    
+    dfs = to_dataframes(gdx_file)
+    assert len(dfs) == n
+
+    # data frames are loaded in order
+    for i, symbol_name in enumerate(dfs):
+        assert symbol_names[i] == symbol_name
+
+    dtypes = get_data_types(gdx_file)
+    # this file is all parameters
+    for val in dtypes.values():
+        val == gdxpds.gdx.GamsDataType.Parameter
 
 def test_unload():
     filename = 'all_generator_properties_input.gdx'
     gdx_file = os.path.join(base_dir,filename)
     with gdxpds.gdx.GdxFile() as f:
         f.read(gdx_file)
         assert not f['startupfuel'].loaded
```

### Comparing `gdxpds-1.3.0/gdxpds/test/test_session.py` & `gdxpds-1.4.0/gdxpds/test/test_session.py`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/test/test_specials.py` & `gdxpds-1.4.0/gdxpds/test/test_specials.py`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/test/test_write.py` & `gdxpds-1.4.0/gdxpds/test/test_write.py`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds/tools.py` & `gdxpds-1.4.0/gdxpds/tools.py`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/gdxpds.egg-info/PKG-INFO` & `gdxpds-1.4.0/gdxpds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdxpds
-Version: 1.3.0
+Version: 1.4.0
 Summary: gdx-pandas is a python package to translate between gdx (GAMS data) and pandas
 Home-page: https://github.com/NREL/gdx-pandas
 Author: Elaine T. Hale
 Author-email: elaine.hale@nrel.gov
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: admin
```

### Comparing `gdxpds-1.3.0/gdxpds.egg-info/SOURCES.txt` & `gdxpds-1.4.0/gdxpds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdxpds-1.3.0/setup.py` & `gdxpds-1.4.0/setup.py`

 * *Files identical despite different names*

