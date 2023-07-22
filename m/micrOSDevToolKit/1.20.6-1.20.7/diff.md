# Comparing `tmp/micrOSDevToolKit-1.20.6.tar.gz` & `tmp/micrOSDevToolKit-1.20.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.20.6.tar", last modified: Thu Jul 20 10:01:14 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.20.7.tar", last modified: Sat Jul 22 08:34:21 2023, max compression
```

## Comparing `micrOSDevToolKit-1.20.6.tar` & `micrOSDevToolKit-1.20.7.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:14.053271 micrOSDevToolKit-1.20.6/
--rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.20.6/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-20 10:01:14.052746 micrOSDevToolKit-1.20.6/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.20.6/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.20.6/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.615476 micrOSDevToolKit-1.20.6/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.6/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.640193 micrOSDevToolKit-1.20.6/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.6/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.6/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.643851 micrOSDevToolKit-1.20.6/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.20.6/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.6/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.717173 micrOSDevToolKit-1.20.6/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.6/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.20.6/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.20.6/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.6/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.785141 micrOSDevToolKit-1.20.6/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.20.6/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.20.6/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.20.6/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.20.6/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.20.6/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6889 2023-07-17 15:14:53.000000 micrOSDevToolKit-1.20.6/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-20 09:51:34.000000 micrOSDevToolKit-1.20.6/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.20.6/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_lmpacman.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.20.6/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.20.6/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.6/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.6/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.20.6/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.20.6/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.20.6/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.20.6/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.20.6/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19574 2023-07-17 15:01:38.000000 micrOSDevToolKit-1.20.6/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.20.6/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.6/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.6/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.20.6/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.20.6/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.20.6/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.20.6/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.789556 micrOSDevToolKit-1.20.6/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-20 10:01:13.000000 micrOSDevToolKit-1.20.6/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     8866 2023-07-20 10:01:13.000000 micrOSDevToolKit-1.20.6/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-20 10:01:13.000000 micrOSDevToolKit-1.20.6/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-20 10:01:13.000000 micrOSDevToolKit-1.20.6/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-20 10:01:13.000000 micrOSDevToolKit-1.20.6/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-20 10:01:14.053502 micrOSDevToolKit-1.20.6/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-20 10:00:32.000000 micrOSDevToolKit-1.20.6/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.799676 micrOSDevToolKit-1.20.6/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.20.6/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.20.6/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.20.6/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.20.6/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.818776 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.824047 micrOSDevToolKit-1.20.6/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.20.6/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.20.6/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.20.6/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.20.6/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.838952 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.892380 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.20.6/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.894584 micrOSDevToolKit-1.20.6/toolkit/user_data/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.20.6/toolkit/user_data/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.894967 micrOSDevToolKit-1.20.6/toolkit/user_data/node_config_archive/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/user_data/node_config_archive/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:13.932940 micrOSDevToolKit-1.20.6/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-20 10:01:14.050715 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2111 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_lmpacman.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5760 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-20 09:55:04.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-20 09:55:05.000000 micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.939029 micrOSDevToolKit-1.20.7/
+-rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.20.7/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-22 08:34:21.938478 micrOSDevToolKit-1.20.7/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.20.7/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.20.7/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.603584 micrOSDevToolKit-1.20.7/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.607276 micrOSDevToolKit-1.20.7/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.7/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.7/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.609053 micrOSDevToolKit-1.20.7/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.20.7/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.647185 micrOSDevToolKit-1.20.7/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.700945 micrOSDevToolKit-1.20.7/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.20.7/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.20.7/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.20.7/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.20.7/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.20.7/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.20.7/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-22 08:22:13.000000 micrOSDevToolKit-1.20.7/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.20.7/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.20.7/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.20.7/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.20.7/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.20.7/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.20.7/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19574 2023-07-17 15:01:38.000000 micrOSDevToolKit-1.20.7/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.20.7/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.20.7/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.20.7/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.20.7/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.20.7/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.703552 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     8866 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-22 08:34:21.939251 micrOSDevToolKit-1.20.7/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-22 08:33:36.000000 micrOSDevToolKit-1.20.7/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.711568 micrOSDevToolKit-1.20.7/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.20.7/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.20.7/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.20.7/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.20.7/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.726819 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.732144 micrOSDevToolKit-1.20.7/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.20.7/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.20.7/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.20.7/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.20.7/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.749579 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.779128 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.20.7/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.780040 micrOSDevToolKit-1.20.7/toolkit/user_data/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.20.7/toolkit/user_data/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.780453 micrOSDevToolKit-1.20.7/toolkit/user_data/node_config_archive/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/user_data/node_config_archive/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.780890 micrOSDevToolKit-1.20.7/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.934938 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5760 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.20.6/PKG-INFO` & `micrOSDevToolKit-1.20.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.20.6
+Version: 1.20.7
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.20.6/README.md` & `micrOSDevToolKit-1.20.7/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/devToolKit.py` & `micrOSDevToolKit-1.20.7/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/media/dnd.png` & `micrOSDevToolKit-1.20.7/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/media/logo.png` & `micrOSDevToolKit-1.20.7/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/media/logo_mini.png` & `micrOSDevToolKit-1.20.7/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.20.7/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.7/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.7/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.20.7/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.20.7/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.7/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.20.7/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/Common.py` & `micrOSDevToolKit-1.20.7/micrOS/source/Common.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.20.7/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/Debug.py` & `micrOSDevToolKit-1.20.7/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.20.7/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.20.7/micrOS/source/InterConnect.py`

 * *Files 10% similar despite different names*

```diff
@@ -126,21 +126,19 @@
     Async send command wrapper for further async task integration and sync send_cmd usage (main)
     :param host: hostname / IP address
     :param cmd: command string to server socket shell
     :param com_obj: InterCon object to utilize send_cmd method and task status updates
     """
     # Send command
     with com_obj.task:
-        out = await com_obj.send_cmd(host, cmd)          # Send CMD
-        if out is None:
-            await asyncio.sleep_ms(150)
-            out = await com_obj.send_cmd(host, cmd)      # Send CMD (retry)
-            if out is None:
-                await asyncio.sleep_ms(150)
-                out = await com_obj.send_cmd(host, cmd)  # Send CMD (retry)
+        for _ in range(0, 4):                           # Retry mechanism
+            out = await com_obj.send_cmd(host, cmd)     # Send CMD
+            if out is not None:                         # Retry mechanism
+                break
+            await asyncio.sleep_ms(100)                 # Retry mechanism
         com_obj.task.out = '' if out is None else out
     return com_obj.task.out
 
 
 def send_cmd(host, cmd):
     """
     Sync wrapper of async _send_cmd (InterCon.send_cmd consumer with retry)
```

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.20.7/micrOS/source/InterpreterShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.20.3-0'
+    MICROS_VERSION = '1.20.4-0'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply('msg')
         """
         self.msg_obj = msg_obj
```

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.20.7/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_lmpacman.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_lmpacman.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.20.7/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/Network.py` & `micrOSDevToolKit-1.20.7/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/Notify.py` & `micrOSDevToolKit-1.20.7/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.20.7/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.20.7/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.20.7/micrOS/source/TaskManager.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/Time.py` & `micrOSDevToolKit-1.20.7/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.20.7/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.20.7/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.20.7/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOS/source/urequests.py` & `micrOSDevToolKit-1.20.7/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.20.6
+Version: 1.20.7
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.20.6/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/setup.py` & `micrOSDevToolKit-1.20.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.20.6',
+    version='1.20.7',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.20.6/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.20.7/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.20.7/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.20.7/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/Gateway.py` & `micrOSDevToolKit-1.20.7/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.20.7/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.20.7/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.20.7/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.20.7/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.20.7/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.20.7/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.20.7/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/socketClient.py` & `micrOSDevToolKit-1.20.7/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Debug.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 00000340: 7d00 0518 436f 6e6e 6563 7469 6f6e 2069  }...Connection i
 00000350: 7320 6275 7379 2e20 4279 6521 0005 345b  s busy. Bye!..4[
 00000360: 696e 7465 7263 6f6e 5d20 7072 6f6d 7074  intercon] prompt
 00000370: 206d 6973 6d61 7463 682c 2068 6f73 746e   mismatch, hostn
 00000380: 616d 653a 207b 7d20 7072 6f6d 7074 3a20  ame: {} prompt: 
 00000390: 7b7d 2000 050b 5b63 6f6e 6669 6775 7265  {} ...[configure
 000003a0: 5d00 875c 101c 0126 322c 2c2c 2c6c 8972  ]..\...&2,,,,l.r
-000003b0: 8414 8417 8051 1b02 1640 8010 0310 042a  .....Q...@.....*
+000003b0: 8412 8417 8051 1b02 1640 8010 0310 042a  .....Q...@.....*
 000003c0: 021b 051c 0316 031c 0416 0459 8010 062a  ...........Y...*
 000003d0: 011b 071c 0616 0659 8010 082a 011b 091c  .......Y...*....
 000003e0: 0816 0859 8010 0a2a 011b 0b1c 0a16 0a59  ...Y...*.......Y
 000003f0: 8010 0c2a 011b 0c1c 0c16 0c59 8010 0d2a  ...*.......Y...*
 00000400: 011b 0e1c 0d16 0d59 5432 0010 0f34 0216  .......YT2...4..
 00000410: 0f32 0116 1132 0216 1332 0316 1d51 6304  .2...2...2...Qc.
 00000420: 840c 081a 0f88 0a24 4864 4068 4084 3284  .......$Hd@h@.2.
@@ -106,27 +106,26 @@
 00000690: 1436 2281 0036 015e 5168 c3b3 4344 40c9  .6"..6.^Qh..CD@.
 000006a0: 8001 b314 3710 3836 0114 2f36 00c3 b151  ....7.86../6...Q
 000006b0: de44 47b3 142f 3600 4241 b1c1 b2b3 e5c2  .DG../6.BA......
 000006c0: b1b2 142f 3600 dd43 4c23 08b2 dd43 4610  .../6..CL#...CF.
 000006d0: 39b3 dd44 4340 5301 4a0d 5712 4bdf 4446  9..DC@S.J.W.K.DF
 000006e0: 5940 4701 4a01 5d42 a17f b214 2db1 1015  Y@G.J.]B....-...
 000006f0: 3602 142d 103a 103b 3602 c2b2 b12a 0263  6..-.:.;6....*.c
-00000700: 8738 cf40 2211 4546 4780 7c80 0726 2b25  .8.@".EFG.|..&+%
-00000710: 2d2b 252d 2b32 b213 1247 5659 b214 13b0  -+%-+2...GVY....
-00000720: b136 025e 5168 c3b3 51de 4475 1240 1414  .6.^Qh..Q.Du.@..
-00000730: 2281 1636 015e 5168 59b2 1413 b0b1 3602  "..6.^QhY.....6.
-00000740: 5e51 68c3 b351 de44 5812 4014 1422 8116  ^Qh..Q.DX.@.."..
-00000750: 3601 5e51 6859 b214 13b0 b136 025e 5168  6.^QhY.....6.^Qh
-00000760: c3b3 51de 4444 1015 4241 b3b2 1312 1816  ..Q.DD..BA......
-00000770: 515c 5db2 1312 1316 6386 246a 9e01 1345  Q\].....c.$j...E
-00000780: 4680 9060 4086 0725 2a37 2353 2c00 01b0  F..`@..%*7#S,...
-00000790: b120 0002 c212 0f34 00c3 1017 1418 b234  . .....4.......4
-000007a0: 0036 01c4 b313 1214 1910 1a12 1125 0025  .6...........%.%
-000007b0: 01b3 3403 101b b436 8400 c5b5 4453 2c02  ..4....6....DS,.
-000007c0: 2300 1418 b436 0110 1c62 b410 1b62 c642  #....6...b...b.B
-000007d0: 4c2c 0223 0110 1c62 b410 1b62 c6b6 6301  L,.#...b...b..c.
-000007e0: 8508 4a12 3c4e 4e80 9620 2f2a 3b25 0114  ..J.<NN.. /*;%..
-000007f0: 3010 3b36 0180 5514 2f36 00c2 120f 1422  0.;6..U./6....."
-00000800: 2500 3601 445b 103d 1418 1031 143e 2500  %.6.D[.=...1.>%.
-00000810: 1430 1031 3601 7e51 2e02 5536 01b2 3602  .0.16.~Q..U6..6.
-00000820: 6310 3d14 1825 0014 2d10 3f10 1536 02b2  c.=..%..-.?..6..
-00000830: 3602 6358 0008 1d80 a760 120f 131e 63    6.cX.....`....c
+00000700: 8568 df40 1e11 4546 4780 7c80 0726 252b  .h.@..EFG.|..&%+
+00000710: 2622 3532 b213 1247 3e59 8042 6457 c3b2  &"52...G>Y.BdW..
+00000720: 1413 b0b1 3602 5e51 68c4 b451 ded3 4442  ....6.^Qh..Q..DB
+00000730: 4254 1240 1414 2280 6436 015e 5168 5981  BT.@..".d6.^QhY.
+00000740: e557 84d7 4317 59b4 51de 4444 1015 4241  .W..C.Y.Q.DD..BA
+00000750: b4b2 1312 1816 515c 5db2 1312 1316 6386  ......Q\].....c.
+00000760: 246a 9e01 1345 4680 8e60 4086 0725 2a37  $j...EF..`@..%*7
+00000770: 2353 2c00 01b0 b120 0002 c212 0f34 00c3  #S,.... .....4..
+00000780: 1017 1418 b234 0036 01c4 b313 1214 1910  .....4.6........
+00000790: 1a12 1125 0025 01b3 3403 101b b436 8400  ...%.%..4....6..
+000007a0: c5b5 4453 2c02 2300 1418 b436 0110 1c62  ..DS,.#....6...b
+000007b0: b410 1b62 c642 4c2c 0223 0110 1c62 b410  ...b.BL,.#...b..
+000007c0: 1b62 c6b6 6301 8508 4a12 3c4e 4e80 9420  .b..c...J.<NN.. 
+000007d0: 2f2a 3b25 0114 3010 3b36 0180 5514 2f36  /*;%..0.;6..U./6
+000007e0: 00c2 120f 1422 2500 3601 445b 103d 1418  ....."%.6.D[.=..
+000007f0: 1031 143e 2500 1430 1031 3601 7e51 2e02  .1.>%..0.16.~Q..
+00000800: 5536 01b2 3602 6310 3d14 1825 0014 2d10  U6..6.c.=..%..-.
+00000810: 3f10 1536 02b2 3602 6358 0008 1d80 a560  ?..6..6.cX.....`
+00000820: 120f 131e 63                             ....c
```

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 1473 6f66 745f  ug..reset..soft_
 000000a0: 7265 7365 7400 0e6d 6163 6869 6e65 000a  reset..machine..
-000000b0: 5368 656c 6c00 1031 2e32 302e 332d 3000  Shell..1.20.3-0.
+000000b0: 5368 656c 6c00 1031 2e32 302e 342d 3000  Shell..1.20.4-0.
 000000c0: 230e 6d73 675f 6f62 6a00 0c64 6576 6669  #.msg_obj..devfi
 000000d0: 6400 105f 5f64 6576 6669 6400 0861 7574  d..__devfid..aut
 000000e0: 6800 165f 5f61 7574 685f 6d6f 6465 000a  h..__auth_mode..
 000000f0: 6877 7569 6400 0e5f 5f68 7775 6964 0012  hwuid..__hwuid..
 00000100: 5f5f 6175 7468 5f6f 6b00 165f 5f63 6f6e  __auth_ok..__con
 00000110: 665f 6d6f 6465 000e 7665 7273 696f 6e00  f_mode..version.
 00000120: 1c4d 4943 524f 535f 5645 5253 494f 4e00  .MICROS_VERSION.
```

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_lmpacman.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_lmpacman.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.6/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*

