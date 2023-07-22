# Comparing `tmp/pwforecast-1.1.4.tar.gz` & `tmp/pwforecast-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwforecast-1.1.4.tar", last modified: Thu Jul 20 08:14:06 2023, max compression
+gzip compressed data, was "pwforecast-1.2.0.tar", last modified: Sat Jul 22 08:00:44 2023, max compression
```

## Comparing `pwforecast-1.1.4.tar` & `pwforecast-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:14:06.626301 pwforecast-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 08:13:51.000000 pwforecast-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-20 08:14:06.626301 pwforecast-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-20 08:13:51.000000 pwforecast-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:14:06.626301 pwforecast-1.1.4/pwforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-07-20 08:13:51.000000 pwforecast-1.1.4/pwforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:14:06.626301 pwforecast-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-20 08:13:51.000000 pwforecast-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:00:44.071480 pwforecast-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-22 08:00:34.000000 pwforecast-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-22 08:00:44.071480 pwforecast-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-22 08:00:34.000000 pwforecast-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:00:44.071480 pwforecast-1.2.0/pwforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-22 08:00:44.000000 pwforecast-1.2.0/pwforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-22 08:00:44.000000 pwforecast-1.2.0/pwforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 08:00:44.000000 pwforecast-1.2.0/pwforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-22 08:00:44.000000 pwforecast-1.2.0/pwforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 08:00:44.000000 pwforecast-1.2.0/pwforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-07-22 08:00:34.000000 pwforecast-1.2.0/pwforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 08:00:44.071480 pwforecast-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-22 08:00:34.000000 pwforecast-1.2.0/setup.py
```

### Comparing `pwforecast-1.1.4/LICENSE` & `pwforecast-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwforecast-1.1.4/PKG-INFO` & `pwforecast-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.1.4
+Version: 1.2.0
 Summary: A Python module to charge/discharge Tesla Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pwforecast-1.1.4/README.md` & `pwforecast-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pwforecast-1.1.4/pwforecast.egg-info/PKG-INFO` & `pwforecast-1.2.0/pwforecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.1.4
+Version: 1.2.0
 Summary: A Python module to charge/discharge Tesla Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pwforecast-1.1.4/pwforecast.py` & `pwforecast-1.2.0/pwforecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,26 @@
             to the Powerwall specs, it has an overall charge/discharge
             efficiency of 90%. We therefore assume a discharge efficiency of
             95%. Default 0.95.
 
     """
     def __init__(self, teslapy_session, solcast_api_key, solcast_site_ids):
 
+        # get the battery, which is a class representing the site.
+        battery_list = teslapy_session.battery_list()
+        assert len(battery_list) == 1, 'More than one battery list returned!'
+        battery = battery_list[0]
+
+        # fetch battery data to populate the battery dictionary
+        battery.get_battery_data()
+        assert battery['battery_count'] > 0, 'No batteries detected!'
+
         # internal vars
         self._teslapy_session = teslapy_session
+        self._battery = battery
         self._solcast_api_key = solcast_api_key
         self._solcast_site_ids = solcast_site_ids
 
         # basic configuration
         self.min_reserve_peak_rate = 20
         self.min_reserve_off_peak_rate = 30
         self.max_reserve = 100
@@ -181,21 +191,15 @@
         provided forecast production.
 
         Returns:
             int: The charge percentage the Powerwall should be
             charged/discharged to based on.
 
         """
-        # get the battery, which is a class representing the site.
-        battery_list = self._teslapy_session.battery_list()
-        assert len(battery_list) == 1, 'More than one battery list returned!'
-        battery = battery_list[0]
-
-        battery_data = battery.get_battery_data()
-        total_pack_energy = battery_data['total_pack_energy']
+        total_pack_energy = self._battery['total_pack_energy']
 
         # calculate available energy.
         factors = [self.visible_pack_energy, self.discharge_efficiency]
         availability_factor = sum(factors) - (len(factors) - 1)
         available_pack_energy = total_pack_energy * availability_factor
 
         # fill the Powerwall until required energy is satisfied.
@@ -230,46 +234,39 @@
             Exception: If an invalid charge state is detected and the retry
                 limit has been reached.
 
         """
         # cast to int in case a float is provided
         percent_target = int(percent_target)
 
-        # get the battery, which is a class representing the site
-        battery_list = self._teslapy_session.battery_list()
-        assert len(battery_list) == 1, 'More than one battery list returned!'
-        battery = battery_list[0]
-        battery_data = {}
+        # calculate pack state of health for summary report
+        total_pack_energy = self._battery['total_pack_energy']
+        battery_count = self._battery['battery_count']
+        pack_soh = ((100 / (self.full_pack_energy * battery_count))
+                    * total_pack_energy)
 
         # loop to allow reserve retries
+        battery_data = {}
         for index in range(1, self.set_backup_reserve_retry_limit+1):
 
             # set the battery reserve
             print('Setting backup reserve to {}%, attempt {} of {}'.format(
                 percent_target, index, self.set_backup_reserve_retry_limit))
-            battery.set_backup_reserve_percent(percent_target)
+            self._battery.set_backup_reserve_percent(percent_target)
 
             # sleep to let the devices update and api sync
             time.sleep(self.set_backup_reserve_response_sleep)
 
-            # check to see if the battery charge/discharge state has correctly
-            # changed
-            battery_data = battery.get_battery_data()
-            msg = 'More than one power reading returned!'
-            assert len(battery_data['power_reading']) == 1, msg
-            total_pack_energy = battery_data['total_pack_energy']
-            battery_count = battery_data['battery_count']
-            assert battery_count > 0, 'No batteries detected!'
-            pack_soh = ((100
-                         / (self.full_pack_energy * battery_count))
-                        * total_pack_energy)
-            percent_charged = battery_data['percentage_charged']
-            power_reading = battery_data['power_reading'][0]
-            battery_power = power_reading['battery_power']
-            solar_power = power_reading['solar_power']
+            # get live site data to monitor power flow. site data contains
+            # all that we need with a smaller payload than get_battery_data(),
+            # so let's be kind to tesla servers.
+            live_site_data = self._battery.api('SITE_DATA')['response']
+            percent_charged = live_site_data['percentage_charged']
+            battery_power = live_site_data['battery_power']
+            solar_power = live_site_data['solar_power']
 
             # battery within charge margin, set reserve percent and don't check
             # power flow as it can lead to false positives.
             if (percent_target-self.charge_margin
                     <= percent_charged
                     <= percent_target+self.charge_margin):
                 print('Battery charge within target reserve margin')
@@ -306,16 +303,16 @@
                     msg = ('Reapplying setting to try and ensure Powerwall '
                            'willstop discharging at set reserve.')
                     print(msg)
                 else:
                     break
 
             else:
-                print('Incorrect charge/discharge state')
-                pprint.pprint(power_reading)
+                print('Incorrect charge/discharge state. Site data:')
+                pprint.pprint(live_site_data)
 
         # no break
         else:
             pprint.pprint(battery_data)
             raise Exception('Unable to switch battery mode correctly!')
 
         return {'soc': percent_charged,
```

### Comparing `pwforecast-1.1.4/setup.py` & `pwforecast-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # read the contents of README file
 this_directory = Path(__file__).parent
 readme = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pwforecast',
-    version='1.1.4',
+    version='1.2.0',
     author='Tim Hawker',
     license='MIT',
     url='https://github.com/timhawker/pwforecast',
     description=('A Python module to charge/discharge Tesla Powerwall based '
                  'on solar forecast and peak/off peak tariffs.'),
     long_description_content_type='text/markdown',
     long_description=readme,
```

