# Comparing `tmp/hurdat2parser-2.2.3.tar.gz` & `tmp/hurdat2parser-2.2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hurdat2parser-2.2.3.tar", last modified: Mon May 15 15:05:53 2023, max compression
+gzip compressed data, was "hurdat2parser-2.2.3.1.tar", last modified: Sat Jul 22 15:11:01 2023, max compression
```

## Comparing `hurdat2parser-2.2.3.tar` & `hurdat2parser-2.2.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 15:05:53.112444 hurdat2parser-2.2.3/
--rw-rw-rw-   0        0        0     1117 2023-05-15 14:55:10.000000 hurdat2parser-2.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0    28153 2023-05-15 15:05:53.111444 hurdat2parser-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    27558 2023-05-15 15:05:01.000000 hurdat2parser-2.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 15:05:53.030365 hurdat2parser-2.2.3/hurdat2parser/
--rw-rw-rw-   0        0        0    58032 2023-04-29 06:29:45.000000 hurdat2parser-2.2.3/hurdat2parser/__init__.py
--rw-rw-rw-   0        0        0     7088 2023-02-28 07:16:47.000000 hurdat2parser-2.2.3/hurdat2parser/_aliases.py
--rw-rw-rw-   0        0        0    79991 2023-05-15 14:53:04.000000 hurdat2parser-2.2.3/hurdat2parser/_calculations.py
--rw-rw-rw-   0        0        0    14830 2023-02-24 08:17:51.000000 hurdat2parser-2.2.3/hurdat2parser/_future.py
--rw-rw-rw-   0        0        0   163453 2022-07-18 22:48:06.000000 hurdat2parser-2.2.3/hurdat2parser/_maps.py
--rw-rw-rw-   0        0        0    37461 2023-04-29 07:03:19.000000 hurdat2parser-2.2.3/hurdat2parser/_reports.py
-drwxrwxrwx   0        0        0        0 2023-05-15 15:05:53.107032 hurdat2parser-2.2.3/hurdat2parser.egg-info/
--rw-rw-rw-   0        0        0    28153 2023-05-15 15:05:52.000000 hurdat2parser-2.2.3/hurdat2parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-05-15 15:05:52.000000 hurdat2parser-2.2.3/hurdat2parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 15:05:52.000000 hurdat2parser-2.2.3/hurdat2parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 15:05:52.000000 hurdat2parser-2.2.3/hurdat2parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-05-15 15:05:52.000000 hurdat2parser-2.2.3/hurdat2parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 15:05:52.000000 hurdat2parser-2.2.3/hurdat2parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-22 04:30:18.000000 hurdat2parser-2.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 15:05:53.113446 hurdat2parser-2.2.3/setup.cfg
--rw-rw-rw-   0        0        0      900 2023-05-15 14:55:34.000000 hurdat2parser-2.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 15:11:01.675263 hurdat2parser-2.2.3.1/
+-rw-rw-rw-   0        0        0     1114 2023-07-22 14:22:25.000000 hurdat2parser-2.2.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    27783 2023-07-22 15:11:01.675263 hurdat2parser-2.2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    27186 2023-07-22 14:17:17.000000 hurdat2parser-2.2.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 15:11:01.555232 hurdat2parser-2.2.3.1/hurdat2parser/
+-rw-rw-rw-   0        0        0    59152 2023-07-22 14:37:30.000000 hurdat2parser-2.2.3.1/hurdat2parser/__init__.py
+-rw-rw-rw-   0        0        0     8214 2023-07-22 14:39:42.000000 hurdat2parser-2.2.3.1/hurdat2parser/_aliases.py
+-rw-rw-rw-   0        0        0    81119 2023-07-22 14:39:23.000000 hurdat2parser-2.2.3.1/hurdat2parser/_calculations.py
+-rw-rw-rw-   0        0        0    15958 2023-07-22 14:40:03.000000 hurdat2parser-2.2.3.1/hurdat2parser/_future.py
+-rw-rw-rw-   0        0        0   164580 2023-07-22 14:40:39.000000 hurdat2parser-2.2.3.1/hurdat2parser/_maps.py
+-rw-rw-rw-   0        0        0    38762 2023-07-22 14:42:43.000000 hurdat2parser-2.2.3.1/hurdat2parser/_reports.py
+drwxrwxrwx   0        0        0        0 2023-07-22 15:11:01.667262 hurdat2parser-2.2.3.1/hurdat2parser.egg-info/
+-rw-rw-rw-   0        0        0    27783 2023-07-22 15:11:01.000000 hurdat2parser-2.2.3.1/hurdat2parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-07-22 15:11:01.000000 hurdat2parser-2.2.3.1/hurdat2parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 15:11:01.000000 hurdat2parser-2.2.3.1/hurdat2parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-22 15:11:00.000000 hurdat2parser-2.2.3.1/hurdat2parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-07-22 15:11:01.000000 hurdat2parser-2.2.3.1/hurdat2parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-22 15:11:01.000000 hurdat2parser-2.2.3.1/hurdat2parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-22 04:30:18.000000 hurdat2parser-2.2.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 15:11:01.675263 hurdat2parser-2.2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-07-22 14:24:50.000000 hurdat2parser-2.2.3.1/setup.py
```

### Comparing `hurdat2parser-2.2.3/LICENSE.txt` & `hurdat2parser-2.2.3.1/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-hurdat2parser 2.2.3, Copyright (c) 2019-2023, Kyle S. Gentry
+hurdat2parser 2.2.3.1, Copyright (c) 2023, Kyle S. Gentry
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hurdat2parser-2.2.3/PKG-INFO` & `hurdat2parser-2.2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 Metadata-Version: 2.1
 Name: hurdat2parser
-Version: 2.2.3
+Version: 2.2.3.1
 Summary: Interpret Hurricane Data contained in HURDAT2
 Home-page: http://github.com/ksgwxfan/hurdat2parser
 Author: Kyle S. Gentry
 Author-email: KyleSGentry@outlook.com
 License: MIT
 Keywords: hurricane hurdat2 meteorology weather
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# hurdat2parser -- v2.2.3
+# hurdat2parser -- v2.2.3.1
 ---
 ### *Interpreting the Hurdat2 Tropical Cyclone Dataset using Python*
 
 Hurdat2 ([https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat)) is a collection of records from individual Tropical Cyclones. The two primary Hurdat2 records are for the Atlantic (since 1850) and East/Central-Pacific Oceans (since 1949).
 
 The purpose of this module is to provide a quick way to analyze the Hurdat2 datasets. It includes methods for retrieving, inspecting, ranking, or even exporting data for seasons, individual storms, or climatological eras.
 
 PyPI Link: [https://pypi.org/project/hurdat2parser/](https://pypi.org/project/hurdat2parser/)
 
 ## Contents
-* [Changes/Fixes in this Version (2.2.3)](#changes-in-this-version-223)
+* [Changes/Fixes in this Version (2.2.3.1)](#changes-in-this-version-2231)
 * [Requirements, Installation, and getting the data](#installation)
 * [Importing the module](#importing-the-module)
 * [Example Calls](#example-calls)
 * [Hurdat2 Object Structure](#hurdat2-object-structure)
 * [Methods &amp; Attributes](#methods-and-attributes)
 * [Note on Landfall Data](#landfall-data)
 * [Future/Under-Development/Unreleased Methods](#access-to-future-methods)
 * [Roadmap](#roadmap)
 * [Credits](#credits)
 * [Copyright/License](#copyright)
 
-## Changes in this Version (2.2.3)
-- Accounts for the possibility of typos/errors in the acutal database.
-  - Notifies the user if a storm has already been ingested, but does overwrite the previous `TropicalCyclone` entry.
-  - Will skip a `TCRecordEntry` and notify the user if an error occurs whilst trying to generate it.
-- fix for `track_map()` to work for cyclones prior to 1900. There was an issue with the label formatting I was using.
-- fix for rankings for empty partial seasons in `rank_seasons_thru` where quantity of ranks were being returned as one too many.
+## Changes in this Version (2.2.3.1)
+- Hotfix for `<TropicalCyclone>.track_map()` that simply skips over `tkinter`-dependent lines upon error (will occur if user does not have `tkinter` installed).
 
 [&#8679; back to Contents](#contents)
 
 ## Installation
 
 - At the command prompt, run `pip install hurdat2parser`
   - When installing, packages `pyshp`, `geojson`, and `matplotlib` will be downloaded as dependencies (if necessary). From scratch, it's around 30MB total of dependency downloads.
```

### Comparing `hurdat2parser-2.2.3/README.md` & `hurdat2parser-2.2.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-# hurdat2parser -- v2.2.3
+# hurdat2parser -- v2.2.3.1
 ---
 ### *Interpreting the Hurdat2 Tropical Cyclone Dataset using Python*
 
 Hurdat2 ([https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat)) is a collection of records from individual Tropical Cyclones. The two primary Hurdat2 records are for the Atlantic (since 1850) and East/Central-Pacific Oceans (since 1949).
 
 The purpose of this module is to provide a quick way to analyze the Hurdat2 datasets. It includes methods for retrieving, inspecting, ranking, or even exporting data for seasons, individual storms, or climatological eras.
 
 PyPI Link: [https://pypi.org/project/hurdat2parser/](https://pypi.org/project/hurdat2parser/)
 
 ## Contents
-* [Changes/Fixes in this Version (2.2.3)](#changes-in-this-version-223)
+* [Changes/Fixes in this Version (2.2.3.1)](#changes-in-this-version-2231)
 * [Requirements, Installation, and getting the data](#installation)
 * [Importing the module](#importing-the-module)
 * [Example Calls](#example-calls)
 * [Hurdat2 Object Structure](#hurdat2-object-structure)
 * [Methods &amp; Attributes](#methods-and-attributes)
 * [Note on Landfall Data](#landfall-data)
 * [Future/Under-Development/Unreleased Methods](#access-to-future-methods)
 * [Roadmap](#roadmap)
 * [Credits](#credits)
 * [Copyright/License](#copyright)
 
-## Changes in this Version (2.2.3)
-- Accounts for the possibility of typos/errors in the acutal database.
-  - Notifies the user if a storm has already been ingested, but does overwrite the previous `TropicalCyclone` entry.
-  - Will skip a `TCRecordEntry` and notify the user if an error occurs whilst trying to generate it.
-- fix for `track_map()` to work for cyclones prior to 1900. There was an issue with the label formatting I was using.
-- fix for rankings for empty partial seasons in `rank_seasons_thru` where quantity of ranks were being returned as one too many.
+## Changes in this Version (2.2.3.1)
+- Hotfix for `<TropicalCyclone>.track_map()` that simply skips over `tkinter`-dependent lines upon error (will occur if user does not have `tkinter` installed).
 
 [&#8679; back to Contents](#contents)
 
 ## Installation
 
 - At the command prompt, run `pip install hurdat2parser`
   - When installing, packages `pyshp`, `geojson`, and `matplotlib` will be downloaded as dependencies (if necessary). From scratch, it's around 30MB total of dependency downloads.
```

### Comparing `hurdat2parser-2.2.3/hurdat2parser/__init__.py` & `hurdat2parser-2.2.3.1/hurdat2parser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""hurdat2parser v2.2.3
+"""hurdat2parser v2.2.3.1
 
 https://github.com/ksgwxfan/hurdat2parser
 
 hurdat2parser v2.x is provides a convenient access to interpret and work with
 tropical cyclone data that is contained in a widely-used and updated dataset,
 HURDAT2 (https://www.nhc.noaa.gov/data/#hurdat). The purpose of this module is to
 provide a quick way to investigate HURDAT2 data. It includes methods for
@@ -19,14 +19,36 @@
     >>> import hurdat2parser
     >>> atl = hurdat2parser.Hurdat2("path_to_hurdat2.txt")
 
     OR ATTEMPT TO RETRIEVE FROM ONLINE
     >>> atl = hurdat2parser.Hurdat2(basin="atl")
     # Use "pac" to get the NE/CEN Pacific version
 
+MIT License
+
+hurdat2parser 2.2.3.1, Copyright (c) 2023, Kyle S. Gentry
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
 hurdat2parser, Copyright (c) 2019-2023, Kyle Gentry (KyleSGentry@outlook.com)
 License: MIT
 ksgwxfan.github.io
 echotops.blogspot.com
 """
 
 # in _calculations: added bounding_box and latitude/longitude bounds properties
```

### Comparing `hurdat2parser-2.2.3/hurdat2parser/_aliases.py` & `hurdat2parser-2.2.3.1/hurdat2parser/_aliases.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+"""
+hurdat2parser 2.2.3.1, Copyright (c) 2023, Kyle S. Gentry
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
 
 class Hurdat2Aliases:
 
     @property
     def tc(self):
         return self._tc
```

### Comparing `hurdat2parser-2.2.3/hurdat2parser/_calculations.py` & `hurdat2parser-2.2.3.1/hurdat2parser/_calculations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+"""
+hurdat2parser 2.2.3.1, Copyright (c) 2023, Kyle S. Gentry
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
 import statistics
 import math
 import textwrap
 import datetime
 import calendar
 import collections
```

### Comparing `hurdat2parser-2.2.3/hurdat2parser/_future.py` & `hurdat2parser-2.2.3.1/hurdat2parser/_future.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+"""
+hurdat2parser 2.2.3.1, Copyright (c) 2023, Kyle S. Gentry
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
 import statistics
 import math
 import operator
 
 from . import _maps
 from . import _calculations
```

### Comparing `hurdat2parser-2.2.3/hurdat2parser/_maps.py` & `hurdat2parser-2.2.3.1/hurdat2parser/_maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,33 @@
-"""All coordinates herein were retrieved from naturalearthdata.com."""
+"""
+hurdat2parser 2.2.3.1, Copyright (c) 2023, Kyle S. Gentry
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+---
+
+All coordinates herein were retrieved from naturalearthdata.com."""
 
 # Natural Earth 110m (ne_110m_admin_0_countries_lakes)
 all_land = [
   [
     "Afghanistan,Angola,Albania,United Arab Emirates,Argentina,Armenia,Antarctica,Fr. S. Antarctic Lands,Australia,Austria,Azerbaijan,Burundi,Belgium,Benin,Burkina Faso,Bangladesh,Bulgaria,Bahamas,Bosnia and Herz.,Belarus,Bolivia,Brazil,Brunei,Bhutan,Botswana,Central African Rep.,Canada,Switzerland,Chile,China,C\u00f4te d'Ivoire,Cameroon,Dem. Rep. Congo,Congo,Cuba,N. Cyprus,Cyprus,Czech Rep.,Germany,Djibouti,Denmark,Dominican Rep.,Algeria,Ecuador,Egypt,Eritrea,Spain,Estonia,Ethiopia,Finland,Fiji,Falkland Is.,Gabon,United Kingdom,Georgia,Ghana,Guinea,Gambia,Guinea-Bissau,Eq. Guinea,Greece,Greenland,Croatia,Haiti,Hungary,Indonesia,India,Ireland,Iran,Iraq,Iceland,Israel,Italy,Jamaica,Jordan,Japan,Kazakhstan,Kenya,Kyrgyzstan,Cambodia,Korea,Kosovo,Kuwait,Lao PDR,Lebanon,Liberia,Libya,Sri Lanka,Lesotho,Lithuania,Luxembourg,Latvia,Morocco,Moldova,Madagascar,Macedonia,Mali,Myanmar,Montenegro,Mongolia,Mozambique,Mauritania,Malawi,Malaysia,Namibia,New Caledonia,Niger,Nigeria,Netherlands,Norway,Nepal,New Zealand,Oman,Pakistan,Peru,Philippines,Papua New Guinea,Poland,Puerto Rico,Dem. Rep. Korea,Portugal,Paraguay,Palestine,Qatar,Romania,Russia,Rwanda,W. Sahara,Saudi Arabia,Sudan,S. Sudan,Senegal,Solomon Is.,Sierra Leone,Somaliland,Somalia,Serbia,Slovakia,Slovenia,Sweden,Swaziland,Syria,Chad,Togo,Thailand,Tajikistan,Turkmenistan,Timor-Leste,Tunisia,Turkey,Taiwan,Tanzania,Uganda,Ukraine,Uruguay,Uzbekistan,Vietnam,Vanuatu,Yemen,South Africa,Zambia,Zimbabwe",
     [[-159.20, -79.49], [-161.12, -79.63], [-162.43, -79.28], [-163.02, -78.92], [-163.06, -78.86], [-163.71, -78.59], [-163.71, -78.59], [-163.10, -78.22], [-161.24, -78.38], [-160.24, -78.69], [-159.48, -79.04], [-159.20, -79.49]],
     [[-59.57, -80.04], [-59.86, -80.54], [-60.15, -81.00], [-62.25, -80.86], [-64.48, -80.92], [-65.74, -80.58], [-65.74, -80.54], [-66.29, -80.25], [-64.03, -80.29], [-61.88, -80.39], [-61.13, -79.98], [-60.61, -79.62], [-59.57, -80.04]],
```

### Comparing `hurdat2parser-2.2.3/hurdat2parser/_reports.py` & `hurdat2parser-2.2.3.1/hurdat2parser/_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+"""
+hurdat2parser 2.2.3.1, Copyright (c) 2023, Kyle S. Gentry
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
 import operator
 import json
 import statistics
 import math
 import os
 import re
 import csv
@@ -656,33 +680,38 @@
         figman = plt.get_current_fig_manager()
         figman.set_window_title(
             "{} - {} Tracks".format(
                 self.atcfid,
                 self.name
             )
         )
-        MIN_SCREEN_DIM = "height" \
-            if figman.window.winfo_screenheight() < figman.window.winfo_screenwidth() \
-            else "width"
-
-        # set figure dimensions with a 4:3 aspect ratio
-        if MIN_SCREEN_DIM == "height":
-            fig.set_figheight(
-                figman.window.winfo_screenmmheight() / 25.4 - 2
-            )
-            fig.set_figwidth(
-                fig.get_figheight() * 1 / kw.get("aspect_ratio", 3/4)
-            )
-        else:
-            fig.set_figwidth(
-                figman.window.winfo_screenmmwidth() / 25.4 - 2
-            )
-            fig.set_figheight(
-                fig.get_figwidth() * kw.get("aspect_ratio", 3/4)
-            )
+
+        # This blocks out tkinter-specific code 
+        try:
+            MIN_SCREEN_DIM = "height" \
+                if figman.window.winfo_screenheight() < figman.window.winfo_screenwidth() \
+                else "width"
+
+            # set figure dimensions with a 4:3 aspect ratio
+            if MIN_SCREEN_DIM == "height":
+                fig.set_figheight(
+                    figman.window.winfo_screenmmheight() / 25.4 - 2
+                )
+                fig.set_figwidth(
+                    fig.get_figheight() * 1 / kw.get("aspect_ratio", 3/4)
+                )
+            else:
+                fig.set_figwidth(
+                    figman.window.winfo_screenmmwidth() / 25.4 - 2
+                )
+                fig.set_figheight(
+                    fig.get_figwidth() * kw.get("aspect_ratio", 3/4)
+                )
+        except:
+            pass
 
         fig.suptitle("Tracks for {} - {}".format(
             "{} {} ({})".format(
                 self.status_highest,
                 self.name.title(),
                 self.atcfid
             ) if self.name != "UNNAMED" else \
```

### Comparing `hurdat2parser-2.2.3/hurdat2parser.egg-info/PKG-INFO` & `hurdat2parser-2.2.3.1/hurdat2parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 Metadata-Version: 2.1
 Name: hurdat2parser
-Version: 2.2.3
+Version: 2.2.3.1
 Summary: Interpret Hurricane Data contained in HURDAT2
 Home-page: http://github.com/ksgwxfan/hurdat2parser
 Author: Kyle S. Gentry
 Author-email: KyleSGentry@outlook.com
 License: MIT
 Keywords: hurricane hurdat2 meteorology weather
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# hurdat2parser -- v2.2.3
+# hurdat2parser -- v2.2.3.1
 ---
 ### *Interpreting the Hurdat2 Tropical Cyclone Dataset using Python*
 
 Hurdat2 ([https://www.nhc.noaa.gov/data/#hurdat](https://www.nhc.noaa.gov/data/#hurdat)) is a collection of records from individual Tropical Cyclones. The two primary Hurdat2 records are for the Atlantic (since 1850) and East/Central-Pacific Oceans (since 1949).
 
 The purpose of this module is to provide a quick way to analyze the Hurdat2 datasets. It includes methods for retrieving, inspecting, ranking, or even exporting data for seasons, individual storms, or climatological eras.
 
 PyPI Link: [https://pypi.org/project/hurdat2parser/](https://pypi.org/project/hurdat2parser/)
 
 ## Contents
-* [Changes/Fixes in this Version (2.2.3)](#changes-in-this-version-223)
+* [Changes/Fixes in this Version (2.2.3.1)](#changes-in-this-version-2231)
 * [Requirements, Installation, and getting the data](#installation)
 * [Importing the module](#importing-the-module)
 * [Example Calls](#example-calls)
 * [Hurdat2 Object Structure](#hurdat2-object-structure)
 * [Methods &amp; Attributes](#methods-and-attributes)
 * [Note on Landfall Data](#landfall-data)
 * [Future/Under-Development/Unreleased Methods](#access-to-future-methods)
 * [Roadmap](#roadmap)
 * [Credits](#credits)
 * [Copyright/License](#copyright)
 
-## Changes in this Version (2.2.3)
-- Accounts for the possibility of typos/errors in the acutal database.
-  - Notifies the user if a storm has already been ingested, but does overwrite the previous `TropicalCyclone` entry.
-  - Will skip a `TCRecordEntry` and notify the user if an error occurs whilst trying to generate it.
-- fix for `track_map()` to work for cyclones prior to 1900. There was an issue with the label formatting I was using.
-- fix for rankings for empty partial seasons in `rank_seasons_thru` where quantity of ranks were being returned as one too many.
+## Changes in this Version (2.2.3.1)
+- Hotfix for `<TropicalCyclone>.track_map()` that simply skips over `tkinter`-dependent lines upon error (will occur if user does not have `tkinter` installed).
 
 [&#8679; back to Contents](#contents)
 
 ## Installation
 
 - At the command prompt, run `pip install hurdat2parser`
   - When installing, packages `pyshp`, `geojson`, and `matplotlib` will be downloaded as dependencies (if necessary). From scratch, it's around 30MB total of dependency downloads.
```

### Comparing `hurdat2parser-2.2.3/setup.py` & `hurdat2parser-2.2.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
  
 with open("README.md", "r") as fh: 
     readme = fh.read() 
 
 setup(
     name = 'hurdat2parser',
-    version = '2.2.3',
+    version = '2.2.3.1',
     author = 'Kyle S. Gentry',
     author_email = 'KyleSGentry@outlook.com',
     url = 'http://github.com/ksgwxfan/hurdat2parser',
     description = 'Interpret Hurricane Data contained in HURDAT2',
     long_description = readme,
     long_description_content_type = "text/markdown",
     license = 'MIT',
```

