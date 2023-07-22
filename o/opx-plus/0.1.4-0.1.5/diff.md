# Comparing `tmp/opx_plus-0.1.4.tar.gz` & `tmp/opx_plus-0.1.5.tar.gz`

## Comparing `opx_plus-0.1.4.tar` & `opx_plus-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 opx_plus-0.1.4/.DS_Store
--rw-r--r--   0        0        0    10750 2020-02-02 00:00:00.000000 opx_plus-0.1.4/opx_plus.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 opx_plus-0.1.4/requirements.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 opx_plus-0.1.4/top_level.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opx_plus-0.1.4/.idea/.gitignore
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 opx_plus-0.1.4/.idea/OPX_Plus.iml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 opx_plus-0.1.4/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 opx_plus-0.1.4/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opx_plus-0.1.4/.idea/vcs.xml
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 opx_plus-0.1.4/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opx_plus-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opx_plus-0.1.4/src/__init__.py
--rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.4/src/opx_plus.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 opx_plus-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 opx_plus-0.1.4/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 opx_plus-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 opx_plus-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 opx_plus-0.1.5/.DS_Store
+-rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 opx_plus-0.1.5/opx_plus.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 opx_plus-0.1.5/requirements.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 opx_plus-0.1.5/top_level.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opx_plus-0.1.5/.idea/.gitignore
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 opx_plus-0.1.5/.idea/OPX_Plus.iml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 opx_plus-0.1.5/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 opx_plus-0.1.5/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opx_plus-0.1.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 opx_plus-0.1.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opx_plus-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opx_plus-0.1.5/src/__init__.py
+-rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.5/src/opx_plus.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 opx_plus-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 opx_plus-0.1.5/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 opx_plus-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 opx_plus-0.1.5/PKG-INFO
```

### Comparing `opx_plus-0.1.4/.DS_Store` & `opx_plus-0.1.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.4/opx_plus.py` & `opx_plus-0.1.5/opx_plus.py`

 * *Files 6% similar despite different names*

```diff
@@ -169,34 +169,29 @@
                 to_sheet[f'{column_letter}{row_index + row_incrementer}'].value = s
     if include_header:
         print(f'C&Ped VALUE & HEADERs from {csv_path.split("/")[-1]} to "{to_sheet.title}"')
     else:
         print(f'C&Ped VALUEs from {csv_path.split("/")[-1]} to "{to_sheet.title}"')
 
 
-def paste_df_to_sheet(df, to_sheet, include_header=False):
+def paste_df_to_sheet(df, to_sheet):
     data = df.values.tolist()
-    if include_header:
-        data = [df.columns.tolist()] + data
-
     row_incrementer = 0
-    if not include_header:
-        data = data[1:]
-        row_incrementer += 1
+    data = [df.columns.tolist()] + data
 
     for row_index, row in enumerate(data):
         for column_index, cell in enumerate(row):
             column_letter = openpyxl.utils.get_column_letter(column_index + 1)
             s = cell
             if s is not None:
                 try:
                     s = float(s)
                 except ValueError:
                     pass
-            to_sheet[f'{column_letter}{row_index + row_incrementer}'].value = s
+            to_sheet[f'{column_letter}{row_index + row_incrementer+1}'].value = s
 
 
 def copy_over_and_down_formulas(from_ws, to_ws, formula_cells):
     for row in openpyxl.utils.rows_from_range(formula_cells):
         c_list = []
         for cell in row:
             c_list.append(cell.rstrip('1234567890'))
```

### Comparing `opx_plus-0.1.4/.idea/workspace.xml` & `opx_plus-0.1.5/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.4/src/opx_plus.py` & `opx_plus-0.1.5/src/opx_plus.py`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.4/LICENSE.txt` & `opx_plus-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.4/README.md` & `opx_plus-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.4/pyproject.toml` & `opx_plus-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "opx_plus"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Steven Wilson", github="https://github.com/StevenWilson9" },
 ]
 description = "Adds additional functionality on top of OpenPyXL"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `opx_plus-0.1.4/PKG-INFO` & `opx_plus-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opx_plus
-Version: 0.1.4
+Version: 0.1.5
 Summary: Adds additional functionality on top of OpenPyXL
 Project-URL: Homepage, https://github.com/StevenWilson9/OPX_Plus
 Project-URL: Bug Tracker, https://github.com/StevenWilson9/OPX_Plus/issues
 Author: Steven Wilson
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

