# Comparing `tmp/iso3166-updates-1.4.1.tar.gz` & `tmp/iso3166-updates-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-updates-1.4.1.tar", last modified: Fri Jul 21 15:13:27 2023, max compression
+gzip compressed data, was "iso3166-updates-1.4.2.tar", last modified: Sat Jul 22 20:59:19 2023, max compression
```

## Comparing `iso3166-updates-1.4.1.tar` & `iso3166-updates-1.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:13:27.693669 iso3166-updates-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-21 15:13:27.693669 iso3166-updates-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:13:27.689669 iso3166-updates-1.4.1/iso3166_updates/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/iso3166_updates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/iso3166_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   318079 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/iso3166_updates/iso3166-updates.json
--rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/iso3166_updates/iso3166_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:13:27.693669 iso3166-updates-1.4.1/iso3166_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:13:26.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-21 15:13:27.693669 iso3166-updates-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:59:19.011927 iso3166-updates-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-22 20:58:51.000000 iso3166-updates-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-22 20:58:51.000000 iso3166-updates-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23103 2023-07-22 20:59:19.011927 iso3166-updates-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-07-22 20:58:51.000000 iso3166-updates-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:59:19.007927 iso3166-updates-1.4.2/iso3166_updates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-22 20:58:51.000000 iso3166-updates-1.4.2/iso3166_updates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-22 20:58:51.000000 iso3166-updates-1.4.2/iso3166_updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   318079 2023-07-22 20:58:51.000000 iso3166-updates-1.4.2/iso3166_updates/iso3166-updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-07-22 20:58:51.000000 iso3166-updates-1.4.2/iso3166_updates/iso3166_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:59:19.011927 iso3166-updates-1.4.2/iso3166_updates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23103 2023-07-22 20:59:18.000000 iso3166-updates-1.4.2/iso3166_updates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-22 20:59:18.000000 iso3166-updates-1.4.2/iso3166_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:59:18.000000 iso3166-updates-1.4.2/iso3166_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:59:18.000000 iso3166-updates-1.4.2/iso3166_updates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-22 20:59:18.000000 iso3166-updates-1.4.2/iso3166_updates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-22 20:59:18.000000 iso3166-updates-1.4.2/iso3166_updates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-22 20:59:19.011927 iso3166-updates-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-22 20:58:51.000000 iso3166-updates-1.4.2/setup.py
```

### Comparing `iso3166-updates-1.4.1/LICENSE` & `iso3166-updates-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-updates-1.4.1/PKG-INFO` & `iso3166-updates-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
@@ -90,17 +90,18 @@
 
 > https://www.iso3166-updates.com/api
 
 The other endpoints available in the API are:
 
 * https://iso3166-updates.com/api/alpha2/<input_alpha2>
 * https://iso3166-updates.com/api/name/<input_name>
-* https://iso3166-updates.com/api/year/<year>
+* https://iso3166-updates.com/api/year/<input_year>
 * https://iso3166-updates.com/api/alpha2/<input_alpha2>/year/<input_year>
-* https://iso3166-updates.com/api/month/<month>
+* https://iso3166-updates.com/api/name/<input_name>/year/<input_year>
+* https://iso3166-updates.com/api/month/<input_month>
 
 Four query string parameters/paths are available in the API - `alpha2`, `name`, `year` and `months`. 
 
 * The 2 letter `alpha2` country code can be appended to the url as a query string parameter or as its own path (e.g ?alpha2=JP or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g ?alpha2=FR, DE, HU, ID, MA or /alpha2/FR,DE,HU,ID,MA). For redudancy, the 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g ?alpha2=FRA, DEU, HUN, IDN, MAR or /alpha2/FRA,DEU,HUN,IDN,MAR). 
 
 * The `name` parameter takes in a country's name as it is commonly known in English (e.g France, Moldova, Benin). A closeness function is used to get the most approximate available country from the one the user input. If one is not found then an error is raised.
 
@@ -160,30 +161,35 @@
 **Get all listed changes/updates for all countries and years:**
 ```python
 iso.updates.all
 ```
 
 **Get all listed ISO 3166-2 changes/updates for Andorra (AD):**
 ```python
-iso.updates.AD
+iso.updates["AD"]
 ```
 
 **Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY:**
 ```python
 iso.updates["BA","DE","FR","HU","PY"]
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
 ```python
-iso.updates.year("2012-2021")["IE"]
+iso.updates.year("2012-2021").IE
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015:**
 ```python
-iso.updates.year(">2015")["TA"]
+iso.updates.year(">2015").TA
+```
+
+**Get any listed ISO 3166-2 changes/updates for Romania, with updates with year < 2007:**
+```python
+iso.updates.year("<2007").RO
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
 ```python
 iso.updates.year("<2010")["YE"]
 ```
 Usage (get_all_iso3166_updates.py script)
```

### Comparing `iso3166-updates-1.4.1/README.md` & `iso3166-updates-1.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,18 @@
 
 > https://www.iso3166-updates.com/api
 
 The other endpoints available in the API are:
 
 * https://iso3166-updates.com/api/alpha2/<input_alpha2>
 * https://iso3166-updates.com/api/name/<input_name>
-* https://iso3166-updates.com/api/year/<year>
+* https://iso3166-updates.com/api/year/<input_year>
 * https://iso3166-updates.com/api/alpha2/<input_alpha2>/year/<input_year>
-* https://iso3166-updates.com/api/month/<month>
+* https://iso3166-updates.com/api/name/<input_name>/year/<input_year>
+* https://iso3166-updates.com/api/month/<input_month>
 
 Four query string parameters/paths are available in the API - `alpha2`, `name`, `year` and `months`. 
 
 * The 2 letter `alpha2` country code can be appended to the url as a query string parameter or as its own path (e.g ?alpha2=JP or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g ?alpha2=FR, DE, HU, ID, MA or /alpha2/FR,DE,HU,ID,MA). For redudancy, the 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g ?alpha2=FRA, DEU, HUN, IDN, MAR or /alpha2/FRA,DEU,HUN,IDN,MAR). 
 
 * The `name` parameter takes in a country's name as it is commonly known in English (e.g France, Moldova, Benin). A closeness function is used to get the most approximate available country from the one the user input. If one is not found then an error is raised.
 
@@ -125,30 +126,35 @@
 **Get all listed changes/updates for all countries and years:**
 ```python
 iso.updates.all
 ```
 
 **Get all listed ISO 3166-2 changes/updates for Andorra (AD):**
 ```python
-iso.updates.AD
+iso.updates["AD"]
 ```
 
 **Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY:**
 ```python
 iso.updates["BA","DE","FR","HU","PY"]
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
 ```python
-iso.updates.year("2012-2021")["IE"]
+iso.updates.year("2012-2021").IE
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015:**
 ```python
-iso.updates.year(">2015")["TA"]
+iso.updates.year(">2015").TA
+```
+
+**Get any listed ISO 3166-2 changes/updates for Romania, with updates with year < 2007:**
+```python
+iso.updates.year("<2007").RO
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
 ```python
 iso.updates.year("<2010")["YE"]
 ```
 Usage (get_all_iso3166_updates.py script)
```

### Comparing `iso3166-updates-1.4.1/iso3166_updates/README.md` & `iso3166-updates-1.4.2/iso3166_updates/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,35 @@
 **Get all listed changes/updates for all countries and years:**
 ```python
 iso.updates.all
 ```
 
 **Get all listed ISO 3166-2 changes/updates for Andorra (AD):**
 ```python
-iso.updates.AD
+iso.updates["AD"]
 ```
 
 **Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY:**
 ```python
 iso.updates["BA","DE","FR","HU","PY"]
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
 ```python
-iso.updates.year("2012-2021")["IE"]
+iso.updates.year("2012-2021").IE
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015:**
 ```python
-iso.updates.year(">2015")["TA"]
+iso.updates.year(">2015").TA
+```
+
+**Get any listed ISO 3166-2 changes/updates for Romania, with updates with year < 2007:**
+```python
+iso.updates.year("<2007").RO
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
 ```python
 iso.updates.year("<2010")["YE"]
 ```
```

### Comparing `iso3166-updates-1.4.1/iso3166_updates/__init__.py` & `iso3166-updates-1.4.2/iso3166_updates/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .iso3166_updates import *
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.4.0"
+__version__ = "1.4.2"
 __description__ = "A Python package that pulls the latest updates & changes to all ISO3166 listed countries."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Development'
```

### Comparing `iso3166-updates-1.4.1/iso3166_updates/iso3166-updates.json` & `iso3166-updates-1.4.2/iso3166_updates/iso3166-updates.json`

 * *Files identical despite different names*

### Comparing `iso3166-updates-1.4.1/iso3166_updates/iso3166_updates.py` & `iso3166-updates-1.4.2/iso3166_updates/iso3166_updates.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     ----------
     None
 
     Usage
     -----
     import iso3166_updates as iso
 
+    #get ALL listed changes/updates for ALL countries 
+    iso.updates.all
+
     #get ALL listed country updates/changes data for Ireland, Colombia, Denmark and Finland
     iso.updates['IE']
     iso.updates['CO']
     iso.updates['DK']
     iso.updates['FI']
 
     #get ALL listed country updates/changes data for France and Germany
@@ -58,14 +61,17 @@
             raise OSError("Issue finding iso3166-updates.json in dir: {}".format(
                 os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename)))
 
         #open iso3166-updates json file and load it into class variable
         with open(os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename)) as iso3166_updates_json:
             self.all = json.load(iso3166_updates_json)
 
+        #make all updates object subscriptable using Map class
+        self.all = Map(self.all)
+
         #get list of all countries by 2 letter alpha3 code
         self.alpha2 = sorted(list(iso3166.countries_by_alpha2.keys()))
         
         #get list of all countries by 3 letter alpha3 code
         self.alpha3 = sorted(list(iso3166.countries_by_alpha3.keys()))
     
     def year(self, input_year):
@@ -81,28 +87,22 @@
             greater than or less than. 
 
         Returns
         -------
         :country_output_dict : dict
             output dictionary of sought ISO 3166 updates for input year/years.
         """
-        #convert year str to array
-        if not (isinstance(input_year, list)):
-            input_year = [input_year]
-
-        country_output_dict = {}
-
-        #raise error if invalid data types input for year parameter
-        for year_ in input_year:
-            if not isinstance(year_, str):
-                raise TypeError("Invalid data type for year parameter, expected str, got {}.".format(type(year_)))
-
         #if single str of 1 or more years input then convert to array, remove whitespace, seperate using comma
         if (isinstance(input_year, str)):
             input_year = input_year.replace(' ', '').split(',')
+        else:
+            #raise error if invalid data type for year parameter
+            raise TypeError("Invalid data type for year parameter, expected str, got {}.".format(type(input_year)))
+        
+        country_output_dict = {}
 
         year_range = False
         greater_than = False
         less_than = False
         
         #a '-' seperating 2 years implies a year range of sought country updates, validate format of years in range
         #a ',' seperating 2 year implies a list of years
@@ -176,27 +176,30 @@
                         for year_ in input_year:
                             if (current_updates_year == str(year_)):
                                 country_output_dict[code].append(self.all[code][update])
 
             #remove any empty objects from dict 
             country_output_dict = {i:j for i,j in country_output_dict.items() if j != []}
 
+        #make updates object subscritable using Map class
+        country_output_dict = Map(country_output_dict)
+
         return country_output_dict
 
     def __getitem__(self, alpha2_code):
         """
         Get all listed updates/changes in the updates json object for an input country/countries,
         using the 2 letter ISO 3166-1 code. This function uses the Map class to make the clas
         subscriptable. It can accept 1 or more 2 letter alpha-2 codes for countries. Also the
         3 letter alpha-3 code for a country can be input which will be converted into its alpha-2 
         counterpart.
         
         Parameters
         ----------
-        : alpha2_code : str
+        :alpha2_code : str
             one or more 2 letter alpha-2 code for sought country/territory e.g (AD, EG, DE). Can 
             also accept 3 letter alpha-3 code e.g (AND, EGT, DEU), this will be converted into 
             its alpha-2 counterpart.
 
         Returns
         -------
         :country_updates_dict: dict
@@ -286,15 +289,15 @@
 class Map(dict):
     """
     Class that accepts a dict and allows you to use dot notation to access
     members of the dictionary. 
 
     Parameters
     ----------
-    : dict
+    :dict
         input dictionary to convert into instance of map class so the keys/vals
         can be accessed via dot notation.
 
     Usage
     -----
     # create instance of map class
     m = Map({'first_name': 'Eduardo'}, last_name='Pool', age=24, sports=['Soccer'])
```

### Comparing `iso3166-updates-1.4.1/iso3166_updates.egg-info/PKG-INFO` & `iso3166-updates-1.4.2/iso3166_updates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
@@ -90,17 +90,18 @@
 
 > https://www.iso3166-updates.com/api
 
 The other endpoints available in the API are:
 
 * https://iso3166-updates.com/api/alpha2/<input_alpha2>
 * https://iso3166-updates.com/api/name/<input_name>
-* https://iso3166-updates.com/api/year/<year>
+* https://iso3166-updates.com/api/year/<input_year>
 * https://iso3166-updates.com/api/alpha2/<input_alpha2>/year/<input_year>
-* https://iso3166-updates.com/api/month/<month>
+* https://iso3166-updates.com/api/name/<input_name>/year/<input_year>
+* https://iso3166-updates.com/api/month/<input_month>
 
 Four query string parameters/paths are available in the API - `alpha2`, `name`, `year` and `months`. 
 
 * The 2 letter `alpha2` country code can be appended to the url as a query string parameter or as its own path (e.g ?alpha2=JP or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g ?alpha2=FR, DE, HU, ID, MA or /alpha2/FR,DE,HU,ID,MA). For redudancy, the 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g ?alpha2=FRA, DEU, HUN, IDN, MAR or /alpha2/FRA,DEU,HUN,IDN,MAR). 
 
 * The `name` parameter takes in a country's name as it is commonly known in English (e.g France, Moldova, Benin). A closeness function is used to get the most approximate available country from the one the user input. If one is not found then an error is raised.
 
@@ -160,30 +161,35 @@
 **Get all listed changes/updates for all countries and years:**
 ```python
 iso.updates.all
 ```
 
 **Get all listed ISO 3166-2 changes/updates for Andorra (AD):**
 ```python
-iso.updates.AD
+iso.updates["AD"]
 ```
 
 **Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY:**
 ```python
 iso.updates["BA","DE","FR","HU","PY"]
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
 ```python
-iso.updates.year("2012-2021")["IE"]
+iso.updates.year("2012-2021").IE
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015:**
 ```python
-iso.updates.year(">2015")["TA"]
+iso.updates.year(">2015").TA
+```
+
+**Get any listed ISO 3166-2 changes/updates for Romania, with updates with year < 2007:**
+```python
+iso.updates.year("<2007").RO
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
 ```python
 iso.updates.year("<2010")["YE"]
 ```
 Usage (get_all_iso3166_updates.py script)
```

### Comparing `iso3166-updates-1.4.1/setup.cfg` & `iso3166-updates-1.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-updates
-version = 1.4.1
+version = 1.4.2
 description = A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 url = https://github.com/amckenna41/iso3166-updates
 download_url = https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
```

### Comparing `iso3166-updates-1.4.1/setup.py` & `iso3166-updates-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pathlib
 from setuptools import setup, find_packages
 import sys
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 __description__ = "A Python package that pulls the latest updates & changes to all ISO3166 listed countries."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Development'
```

