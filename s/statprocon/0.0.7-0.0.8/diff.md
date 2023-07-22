# Comparing `tmp/statprocon-0.0.7.tar.gz` & `tmp/statprocon-0.0.8.tar.gz`

## Comparing `statprocon-0.0.7.tar` & `statprocon-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 statprocon-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 statprocon-0.0.7/CODEOWNERS
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.7/requirements-dev.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/workspace.xml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/xmr.iml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.7/statprocon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.7/statprocon/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.7/statprocon/charts/__init__.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 statprocon-0.0.7/statprocon/charts/xmr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 statprocon-0.0.7/tests/test_xmr.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.7/LICENSE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 statprocon-0.0.7/README.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 statprocon-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 statprocon-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 statprocon-0.0.8/CODEOWNERS
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.8/requirements-dev.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/workspace.xml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/xmr.iml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.8/statprocon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.8/statprocon/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.8/statprocon/charts/__init__.py
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 statprocon-0.0.8/statprocon/charts/xmr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     9111 2020-02-02 00:00:00.000000 statprocon-0.0.8/tests/test_xmr.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 statprocon-0.0.8/README.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 statprocon-0.0.8/PKG-INFO
```

### Comparing `statprocon-0.0.7/requirements-dev.txt` & `statprocon-0.0.8/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.7/.idea/workspace.xml` & `statprocon-0.0.8/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `statprocon-0.0.7/.idea/workspace.xml` & `statprocon-0.0.8/.idea/workspace.xml`

```diff
@@ -1,15 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment="">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/CHANGELOG.md" beforeDir="false" afterPath="$PROJECT_DIR$/CHANGELOG.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/statprocon/charts/xmr.py" beforeDir="false" afterPath="$PROJECT_DIR$/statprocon/charts/xmr.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -85,15 +86,16 @@
       <changelist id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment=""/>
       <created>1688827023388</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1688827023388</updated>
       <workItem from="1688827024910" duration="1917000"/>
       <workItem from="1688848868641" duration="17704000"/>
-      <workItem from="1688944372544" duration="17043000"/>
+      <workItem from="1688944372544" duration="17391000"/>
+      <workItem from="1690054614395" duration="3077000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `statprocon-0.0.7/.idea/xmr.iml` & `statprocon-0.0.8/.idea/xmr.iml`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.7/statprocon/charts/xmr.py` & `statprocon-0.0.8/statprocon/charts/xmr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import csv
 import io
 
 from decimal import Decimal
-from typing import cast, Union, Optional
+from typing import cast, Union, Optional, Sequence
 
-TYPE_COUNTS = list[Decimal | int | float]
-TYPE_MOVING_RANGES = list[Decimal | int | None]
+TYPE_COUNT_VALUE = Decimal | int
+TYPE_MOVING_RANGE_VALUE = Decimal | int | None
+
+TYPE_COUNTS = Sequence[TYPE_COUNT_VALUE | float]
+TYPE_MOVING_RANGES = Sequence[TYPE_MOVING_RANGE_VALUE]
 
 
 class XmR:
     ROUNDING = 3
 
     def __init__(
             self,
@@ -31,94 +34,117 @@
             self.j = min(self.j, subset_end_index)
 
         assert self.i <= self.j
 
     def __repr__(self) -> str:
         result = ''
         for k, v in self.to_dict().items():
-            k_format = '{0: <6}'.format(k)
-            values = ''
+            k_format = '{0: <9}'.format(k)
             if isinstance(v, list):
                 values = '[' + ', '.join(map(str, v)) + ']'
             else:
                 values = v
             result += f'{k_format}: {values}\n'
         return result
 
-    def to_dict(self) -> dict:
+    def x_to_dict(self) -> dict:
+        """
+        Return the values needed for the X chart as a dictionary
+        """
+        n = len(self.counts)
         return {
-            'Counts': self.counts,
-            'UNPL': self.upper_natural_process_limit(),
-            'X bar': self.x_average(),
-            'LNPL': self.lower_natural_process_limit(),
-            'MR': self.moving_ranges(),
-            'URL': self.upper_range_limit(),
-            'MR bar': self.mr_average(),
+            'values': self.counts,
+            'unpl': [self.upper_natural_process_limit()] * n,
+            'cl': [self.x_central_line()] * n,
+            'lnpl': [self.lower_natural_process_limit()] * n,
         }
 
+    def mr_to_dict(self) -> dict:
+        """
+        Return the values needed for the MR chart as a dictionary
+        """
+        mr = self.moving_ranges()
+        n = len(mr)
+        return {
+            'values': mr,
+            'url': [self.upper_range_limit()] * n,
+            'cl': [self.mr_central_line()] * n,
+        }
+
+    def to_dict(self) -> dict:
+        # Naming comes from pg. 163
+        #   So Which Way Should You Compute Limits? from Making Sense of Data
+        result = {}
+        for k, v in self.x_to_dict().items():
+            result[f'x_{k}'] = v
+        for k, v in self.mr_to_dict().items():
+            result[f'mr_{k}'] = v
+
+        return result
+
     def to_csv(self) -> str:
         output = io.StringIO()
         writer = csv.writer(output)
 
         unpl = self.upper_natural_process_limit()
-        x_bar = self.x_average()
+        x_bar = self.x_central_line()
         lnpl = self.lower_natural_process_limit()
         moving_ranges = self.moving_ranges()
         url = self.upper_range_limit()
-        mr_bar = self.mr_average()
+        mr_bar = self.mr_central_line()
 
-        writer.writerow(['Counts', 'UNPL', 'X Avg', 'LNPL', 'MR', 'URL', 'MR Avg'])
+        writer.writerow(['x_values', 'x_unpl', 'x_cl', 'x_lnpl', 'mr_values', 'mr_url', 'mr_cl'])
         for i, x in enumerate(self.counts):
             row = [x, unpl, x_bar, lnpl, moving_ranges[i], url, mr_bar]
             writer.writerow(row)
 
         return output.getvalue()
 
     def moving_ranges(self) -> TYPE_MOVING_RANGES:
         """
         Moving ranges are the absolute differences between successive count values.
         The first element will always be None
         """
         if self._mr:
             return self._mr
 
-        result: TYPE_MOVING_RANGES = []
+        result: list[TYPE_MOVING_RANGE_VALUE] = []
         for i, c in enumerate(self.counts):
             if i == 0:
                 result.append(None)
             else:
                 value = cast(Union[Decimal | int], abs(c - self.counts[i - 1]))
                 result.append(value)
         self._mr = result
         return self._mr
 
-    def x_average(self) -> Decimal:
+    def x_central_line(self) -> Decimal:
         avg = self.mean(self.counts[self.i:self.j])
         return self.round(avg)
 
-    def mr_average(self) -> Decimal:
+    def mr_central_line(self) -> Decimal:
         assert self.moving_ranges()[0] is None
         valid_values = cast(TYPE_COUNTS, self.moving_ranges()[self.i+1:self.j])
         avg = self.mean(valid_values)
         return self.round(avg)
 
     def upper_range_limit(self) -> Decimal:
-        limit = Decimal('3.268') * self.mr_average()
+        limit = Decimal('3.268') * self.mr_central_line()
         return self.round(limit)
 
     def upper_natural_process_limit(self) -> Decimal:
-        limit = self.x_average() + (Decimal('2.660') * self.mr_average())
+        limit = self.x_central_line() + (Decimal('2.660') * self.mr_central_line())
         return self.round(limit)
 
     def lower_natural_process_limit(self) -> Decimal:
         """
         LNPL can be negative.
         It's the caller's responsibility to take max(LNPL, 0) if a negative LNPL does not make sense
         """
-        limit = self.x_average() - (Decimal('2.660') * self.mr_average())
+        limit = self.x_central_line() - (Decimal('2.660') * self.mr_central_line())
         return self.round(limit)
 
     def rule_1_x_indices_beyond_limits(
             self,
             upper_limit: Optional[Decimal] = None,
             lower_limit: Optional[Decimal] = None
     ) -> list[bool]:
```

### Comparing `statprocon-0.0.7/tests/test_xmr.py` & `statprocon-0.0.8/tests/test_xmr.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,39 +12,39 @@
         mr = xmr.moving_ranges()
         self.assertEqual(mr, [])
 
     def test_repr(self):
         counts = [3, 4, 5]
         xmr = XmR(counts)
 
-        expected = """Counts: [3, 4, 5]
-UNPL  : 6.660
-X bar : 4.000
-LNPL  : 1.340
-MR    : [None, 1, 1]
-URL   : 3.268
-MR bar: 1.000
+        expected = """x_values : [3, 4, 5]
+x_unpl   : [6.660, 6.660, 6.660]
+x_cl     : [4.000, 4.000, 4.000]
+x_lnpl   : [1.340, 1.340, 1.340]
+mr_values: [None, 1, 1]
+mr_url   : [3.268, 3.268, 3.268]
+mr_cl    : [1.000, 1.000, 1.000]
 """
         self.assertEqual(xmr.__repr__(), expected)
 
     def test_to_csv(self):
         counts = [3, 4, 5]
         xmr = XmR(counts)
 
-        expected = """Counts,UNPL,X Avg,LNPL,MR,URL,MR Avg\r
+        expected = """x_values,x_unpl,x_cl,x_lnpl,mr_values,mr_url,mr_cl\r
 3,6.660,4.000,1.340,,3.268,1.000\r
 4,6.660,4.000,1.340,1,3.268,1.000\r
 5,6.660,4.000,1.340,1,3.268,1.000\r
 """
         self.assertEqual(xmr.to_csv(), expected)
 
     def test_average_contains_one_more_exponent_as_input(self):
         counts = [3, 3, 4]
         xmr = XmR(counts)
-        self.assertEqual(xmr.x_average(), Decimal('3.333'))
+        self.assertEqual(xmr.x_central_line(), Decimal('3.333'))
 
     def test_moving_range_ints(self):
         counts = [1, 10, 100, 50]
         xmr = XmR(counts)
         mr = xmr.moving_ranges()
         self.assertEqual(mr, [None, 9, 90, 50])
 
@@ -87,15 +87,15 @@
 
         xmr = XmR(counts, subset_end_index=24)
         self.assertEqual(xmr.upper_natural_process_limit(), Decimal('30.442'))
         self.assertEqual(xmr.upper_range_limit(), Decimal('28.134'))
 
         # Adjust manually so that all subset values should be 1
         xmr.i = 4
-        self.assertEqual(xmr.x_average(), 1)
+        self.assertEqual(xmr.x_central_line(), 1)
         self.assertEqual(xmr.lower_natural_process_limit(), xmr.upper_natural_process_limit())
 
     def test_rule_1_points_beyond_upper_limits(self):
         """
         This test dataset comes from Table 9.1: Accident Rates in Making Sense of Data
         """
 
@@ -207,15 +207,15 @@
         unpl = Decimal('5082.28')
         url = Decimal('1163.19')
 
         xmr = XmR(counts)
 
         self.assertListEqual(xmr.moving_ranges(), moving_ranges)
         self.assertEqual(x_avg, xmr.mean(counts))
-        self.assertEqual(mr_avg, round(xmr.mr_average(), 2))
+        self.assertEqual(mr_avg, round(xmr.mr_central_line(), 2))
         self.assertEqual(lnpl, round(xmr.lower_natural_process_limit(), 2))
         self.assertEqual(unpl, round(xmr.upper_natural_process_limit(), 2))
         self.assertEqual(url, round(xmr.upper_range_limit(), 2))
 
     def test_peak_flow_rates(self):
         """
         Data comes from pg 130 of "Making Sense of Data"
@@ -232,11 +232,11 @@
         lnpl = Decimal('43.8')  # 43.7 in book
         url = Decimal('171.1')  # 171.3 in book
 
         xmr = XmR(x_values)
 
         self.assertListEqual(xmr.moving_ranges(), mr_values)
         self.assertEqual(x_avg, round(xmr.mean(x_values), 1))
-        self.assertEqual(mr_avg, round(xmr.mr_average(), 1))
+        self.assertEqual(mr_avg, round(xmr.mr_central_line(), 1))
         self.assertEqual(lnpl, round(xmr.lower_natural_process_limit(), 1))
         self.assertEqual(unpl, round(xmr.upper_natural_process_limit(), 1))
         self.assertEqual(url, round(xmr.upper_range_limit(), 1))
```

### Comparing `statprocon-0.0.7/LICENSE` & `statprocon-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.7/README.md` & `statprocon-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 counts = [10, 50, 40, 30]
 
 xmr = XmR(counts)
 moving_ranges = xmr.moving_ranges()
 unpl = xmr.upper_natural_process_limit()
 lnpl = xmr.lower_natural_process_limit()
-x_bar = xmr.x_average()
+x_bar = xmr.x_central_line()
 
 url = xmr.upper_range_limit()
-mr_bar = xmr.mr_average()
+mr_bar = xmr.mr_central_line()
 
 ```
 
 Currently, this library only supports the data for generating an XmR chart.
 An XmR chart is the simplest type of process behaviour chart.
 XmR is short for individual values (X) and a moving range (mR).
 More chart data options can be added via pull requests.
@@ -42,14 +42,16 @@
 print(xmr.to_csv())
 ```
 
 ### Google Sheets Charts
 
 Quickly generate XmR Charts in Google Sheets
 
+https://github.com/mattmccormick/statprocon/assets/436801/0de1a9f3-a8ad-4047-8c9d-0f890e0bf453
+
 1. Make a copy of the [statprocon XmR Template sheet](https://docs.google.com/spreadsheets/d/1IdCBpE8FK4qP8B7qHQeXX6amLZ8oyhc8OjlBlGHmWTg/edit?usp=sharing)
 1. Paste the CSV output from above into cell A1
 1. Click `Data -> Split Text to Columns`
 
 The X and MR charts will appear on the right.
 
 Note that the Lower Natural Process Limit may not make sense if your count data could not possibly go negative.
```

### Comparing `statprocon-0.0.7/pyproject.toml` & `statprocon-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statprocon"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Matt McCormick", email="mattmccor@gmail.com" },
 ]
 description = "A Python helper library for generating Process Behaviour Charts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `statprocon-0.0.7/PKG-INFO` & `statprocon-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statprocon
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python helper library for generating Process Behaviour Charts
 Project-URL: Homepage, https://github.com/mattmccormick/statprocon
 Project-URL: Bug Tracker, https://github.com/mattmccormick/statprocon/issues
 Project-URL: Changelog, https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md
 Author-email: Matt McCormick <mattmccor@gmail.com>
 License-File: LICENSE
 Keywords: Process Behavior Chart,Process Behaviour Chart,QCC,Quality Control Chart,SPC,Shewhart,Statistical Process Control,Wheeler,XmR
@@ -32,18 +32,18 @@
 
 counts = [10, 50, 40, 30]
 
 xmr = XmR(counts)
 moving_ranges = xmr.moving_ranges()
 unpl = xmr.upper_natural_process_limit()
 lnpl = xmr.lower_natural_process_limit()
-x_bar = xmr.x_average()
+x_bar = xmr.x_central_line()
 
 url = xmr.upper_range_limit()
-mr_bar = xmr.mr_average()
+mr_bar = xmr.mr_central_line()
 
 ```
 
 Currently, this library only supports the data for generating an XmR chart.
 An XmR chart is the simplest type of process behaviour chart.
 XmR is short for individual values (X) and a moving range (mR).
 More chart data options can be added via pull requests.
@@ -58,14 +58,16 @@
 print(xmr.to_csv())
 ```
 
 ### Google Sheets Charts
 
 Quickly generate XmR Charts in Google Sheets
 
+https://github.com/mattmccormick/statprocon/assets/436801/0de1a9f3-a8ad-4047-8c9d-0f890e0bf453
+
 1. Make a copy of the [statprocon XmR Template sheet](https://docs.google.com/spreadsheets/d/1IdCBpE8FK4qP8B7qHQeXX6amLZ8oyhc8OjlBlGHmWTg/edit?usp=sharing)
 1. Paste the CSV output from above into cell A1
 1. Click `Data -> Split Text to Columns`
 
 The X and MR charts will appear on the right.
 
 Note that the Lower Natural Process Limit may not make sense if your count data could not possibly go negative.
```

