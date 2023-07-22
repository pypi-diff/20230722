# Comparing `tmp/platypush-0.9.5.tar.gz` & `tmp/platypush-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/platypush-0.9.5.tar", last modified: Sun Jan 13 19:42:18 2019, max compression
+gzip compressed data, was "dist/platypush-0.9.6.tar", last modified: Sun Feb 24 18:06:50 2019, max compression
```

## Comparing `platypush-0.9.5.tar` & `platypush-0.9.6.tar`

### file list

```diff
@@ -1,1581 +1,2168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/
--rw-r--r--   0 root         (0) root         (0)      103 2018-01-29 15:10:34.000000 platypush-0.9.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6600 2019-01-13 19:42:18.000000 platypush-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4260 2018-12-05 20:19:33.000000 platypush-0.9.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/bin/
--rwxr-xr-x   0 root         (0) root         (0)     6436 2018-12-19 23:11:36.000000 platypush-0.9.5/bin/platyvenv
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/
--rw-r--r--   0 root         (0) root         (0)     5849 2019-01-13 19:11:28.000000 platypush-0.9.5/platypush/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2018-07-04 11:25:50.000000 platypush-0.9.5/platypush/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/
--rw-r--r--   0 root         (0) root         (0)     9267 2019-01-13 19:37:16.000000 platypush-0.9.5/platypush/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/adafruit/
--rw-r--r--   0 root         (0) root         (0)        0 2019-01-11 23:18:57.000000 platypush-0.9.5/platypush/backend/adafruit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2628 2019-01-12 00:56:45.000000 platypush-0.9.5/platypush/backend/adafruit/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/assistant/
--rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/assistant/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/assistant/google/
--rw-r--r--   0 root         (0) root         (0)     4529 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/assistant/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15640 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/assistant/google/pushtotalk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/assistant/snowboy/
--rw-r--r--   0 root         (0) root         (0)     2373 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/assistant/snowboy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/button/
--rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/button/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/button/flic/
--rw-r--r--   0 root         (0) root         (0)     4048 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/button/flic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/button/flic/fliclib/
--rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/button/flic/fliclib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24818 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/button/flic/fliclib/aioflic.py
--rw-r--r--   0 root         (0) root         (0)    23805 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/button/flic/fliclib/fliclib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/camera/
--rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/camera/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6740 2019-01-10 21:53:15.000000 platypush-0.9.5/platypush/backend/camera/pi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/
--rw-r--r--   0 root         (0) root         (0)    20954 2019-01-13 19:37:50.000000 platypush-0.9.5/platypush/backend/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/poll/
--rw-r--r--   0 root         (0) root         (0)     3481 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/http/poll/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/request/
--rw-r--r--   0 root         (0) root         (0)     3993 2019-01-13 19:38:16.000000 platypush-0.9.5/platypush/backend/http/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/request/ota/
--rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/http/request/ota/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/request/ota/booking/
--rw-r--r--   0 root         (0) root         (0)     1613 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/http/request/ota/booking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/request/rss/
--rw-r--r--   0 root         (0) root         (0)     9324 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/http/request/rss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/css/
--rw-r--r--   0 root         (0) root         (0)     4327 2018-05-04 11:12:39.000000 platypush-0.9.5/platypush/backend/http/static/css/application.css
--rw-r--r--   0 root         (0) root         (0)        0 2018-04-17 21:10:49.000000 platypush-0.9.5/platypush/backend/http/static/css/assistant.google.css
--rw-r--r--   0 root         (0) root         (0)      367 2018-05-05 21:56:36.000000 platypush-0.9.5/platypush/backend/http/static/css/dashboard.css
--rw-r--r--   0 root         (0) root         (0)      573 2018-08-22 18:33:17.000000 platypush-0.9.5/platypush/backend/http/static/css/gpio.css
--rw-r--r--   0 root         (0) root         (0)      486 2018-05-01 08:13:41.000000 platypush-0.9.5/platypush/backend/http/static/css/gpio.sensor.mcp3008.css
--rw-r--r--   0 root         (0) root         (0)      341 2018-04-13 23:00:00.000000 platypush-0.9.5/platypush/backend/http/static/css/gpio.zeroborg.css
--rw-r--r--   0 root         (0) root         (0)     2274 2018-06-18 22:37:33.000000 platypush-0.9.5/platypush/backend/http/static/css/light.hue.css
--rw-r--r--   0 root         (0) root         (0)      119 2018-06-12 18:30:23.000000 platypush-0.9.5/platypush/backend/http/static/css/map.css
--rw-r--r--   0 root         (0) root         (0)     3470 2018-04-12 10:38:19.000000 platypush-0.9.5/platypush/backend/http/static/css/music.mpd.css
--rw-r--r--   0 root         (0) root         (0)     3693 2019-01-08 17:23:09.000000 platypush-0.9.5/platypush/backend/http/static/css/music.snapcast.css
--rw-r--r--   0 root         (0) root         (0)     7797 2014-12-29 18:30:41.000000 platypush-0.9.5/platypush/backend/http/static/css/normalize.css
--rw-r--r--   0 root         (0) root         (0)      454 2018-01-28 19:40:20.000000 platypush-0.9.5/platypush/backend/http/static/css/skeleton-tabs.css
--rw-r--r--   0 root         (0) root         (0)    11452 2014-12-29 18:30:41.000000 platypush-0.9.5/platypush/backend/http/static/css/skeleton.css
--rw-r--r--   0 root         (0) root         (0)      612 2018-05-11 18:40:45.000000 platypush-0.9.5/platypush/backend/http/static/css/switch.switchbot.css
--rw-r--r--   0 root         (0) root         (0)      600 2018-06-26 19:51:16.000000 platypush-0.9.5/platypush/backend/http/static/css/switch.tplink.css
--rw-r--r--   0 root         (0) root         (0)      592 2018-05-08 07:54:04.000000 platypush-0.9.5/platypush/backend/http/static/css/switch.wemo.css
--rw-r--r--   0 root         (0) root         (0)     5637 2018-03-27 21:13:47.000000 platypush-0.9.5/platypush/backend/http/static/css/toggles.css
--rw-r--r--   0 root         (0) root         (0)      124 2018-04-17 07:27:41.000000 platypush-0.9.5/platypush/backend/http/static/css/tts.css
--rw-r--r--   0 root         (0) root         (0)     1773 2018-04-26 13:27:44.000000 platypush-0.9.5/platypush/backend/http/static/css/video.omxplayer.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/css/widgets/
--rw-r--r--   0 root         (0) root         (0)      536 2018-06-10 15:19:50.000000 platypush-0.9.5/platypush/backend/http/static/css/widgets/calendar.css
--rw-r--r--   0 root         (0) root         (0)      962 2018-06-23 11:26:20.000000 platypush-0.9.5/platypush/backend/http/static/css/widgets/date-time-weather.css
--rw-r--r--   0 root         (0) root         (0)      566 2018-05-07 15:17:15.000000 platypush-0.9.5/platypush/backend/http/static/css/widgets/image-carousel.css
--rw-r--r--   0 root         (0) root         (0)     1101 2018-08-17 23:08:57.000000 platypush-0.9.5/platypush/backend/http/static/css/widgets/music.css
--rw-r--r--   0 root         (0) root         (0)      589 2018-05-05 21:41:52.000000 platypush-0.9.5/platypush/backend/http/static/css/widgets/rss-news.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/
--rw-r--r--   0 root         (0) root         (0)       79 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/.git
--rw-r--r--   0 root         (0) root         (0)      301 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/.gitignore
--rw-r--r--   0 root         (0) root         (0)      427 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/.npmignore
--rw-r--r--   0 root         (0) root         (0)     5271 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)      173 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/Gemfile
--rw-r--r--   0 root         (0) root         (0)     1383 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/Gemfile.lock
--rw-r--r--   0 root         (0) root         (0)      323 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/HELP-US-OUT.txt
--rw-r--r--   0 root         (0) root         (0)     5345 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/README.md
--rw-r--r--   0 root         (0) root         (0)     1643 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/_config.yml
--rw-r--r--   0 root         (0) root         (0)      403 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/bower.json
--rw-r--r--   0 root         (0) root         (0)      499 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/component.json
--rw-r--r--   0 root         (0) root         (0)      610 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/composer.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/css/
--rw-r--r--   0 root         (0) root         (0)    37414 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/css/font-awesome.css
--rw-r--r--   0 root         (0) root         (0)    21778 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/css/font-awesome.css.map
--rw-r--r--   0 root         (0) root         (0)    31000 2018-01-28 22:51:53.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/
--rw-r--r--   0 root         (0) root         (0)   134808 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)   165742 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/
--rw-r--r--   0 root         (0) root         (0)      713 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/animated.less
--rw-r--r--   0 root         (0) root         (0)      585 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/bordered-pulled.less
--rw-r--r--   0 root         (0) root         (0)      452 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/core.less
--rw-r--r--   0 root         (0) root         (0)      119 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/fixed-width.less
--rw-r--r--   0 root         (0) root         (0)      495 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/font-awesome.less
--rw-r--r--   0 root         (0) root         (0)    49712 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/icons.less
--rw-r--r--   0 root         (0) root         (0)      370 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/larger.less
--rw-r--r--   0 root         (0) root         (0)      377 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/list.less
--rw-r--r--   0 root         (0) root         (0)     1603 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/mixins.less
--rw-r--r--   0 root         (0) root         (0)      771 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/path.less
--rw-r--r--   0 root         (0) root         (0)      622 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/rotated-flipped.less
--rw-r--r--   0 root         (0) root         (0)      118 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/screen-reader.less
--rw-r--r--   0 root         (0) root         (0)      476 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/stacked.less
--rw-r--r--   0 root         (0) root         (0)    22563 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/less/variables.less
--rw-r--r--   0 root         (0) root         (0)     1040 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/
--rw-r--r--   0 root         (0) root         (0)      715 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_animated.scss
--rw-r--r--   0 root         (0) root         (0)      592 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_bordered-pulled.scss
--rw-r--r--   0 root         (0) root         (0)      459 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_core.scss
--rw-r--r--   0 root         (0) root         (0)      120 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_fixed-width.scss
--rw-r--r--   0 root         (0) root         (0)    50498 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_icons.scss
--rw-r--r--   0 root         (0) root         (0)      375 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_larger.scss
--rw-r--r--   0 root         (0) root         (0)      378 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_list.scss
--rw-r--r--   0 root         (0) root         (0)     1637 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_mixins.scss
--rw-r--r--   0 root         (0) root         (0)      783 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_path.scss
--rw-r--r--   0 root         (0) root         (0)      672 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_rotated-flipped.scss
--rw-r--r--   0 root         (0) root         (0)      134 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_screen-reader.scss
--rw-r--r--   0 root         (0) root         (0)      482 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_stacked.scss
--rw-r--r--   0 root         (0) root         (0)    22644 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_variables.scss
--rw-r--r--   0 root         (0) root         (0)      430 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/font-awesome.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/
--rw-r--r--   0 root         (0) root         (0)       14 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/CNAME
--rw-r--r--   0 root         (0) root         (0)     1101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/
--rw-r--r--   0 root         (0) root         (0)      815 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/prettify.css
--rw-r--r--   0 root         (0) root         (0)     3063 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/pygments.css
--rw-r--r--   0 root         (0) root         (0)   165597 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/site.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/
--rw-r--r--   0 root         (0) root         (0)    41311 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome-ie7.css
--rw-r--r--   0 root         (0) root         (0)    37782 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome-ie7.min.css
--rw-r--r--   0 root         (0) root         (0)    27232 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome.css
--rw-r--r--   0 root         (0) root         (0)    22084 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/
--rw-r--r--   0 root         (0) root         (0)    61896 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)    37405 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   197829 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)    79076 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    43572 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/
--rw-r--r--   0 root         (0) root         (0)     2084 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/bootstrap.less
--rw-r--r--   0 root         (0) root         (0)     2101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/core.less
--rw-r--r--   0 root         (0) root         (0)     2398 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/extras.less
--rw-r--r--   0 root         (0) root         (0)    19299 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/font-awesome-ie7.less
--rw-r--r--   0 root         (0) root         (0)     1319 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/font-awesome.less
--rw-r--r--   0 root         (0) root         (0)    17555 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/icons.less
--rw-r--r--   0 root         (0) root         (0)     1041 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/mixins.less
--rw-r--r--   0 root         (0) root         (0)      742 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/path.less
--rw-r--r--   0 root         (0) root         (0)     8888 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/variables.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/
--rw-r--r--   0 root         (0) root         (0)     2088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_bootstrap.scss
--rw-r--r--   0 root         (0) root         (0)     2157 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_core.scss
--rw-r--r--   0 root         (0) root         (0)     2406 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_extras.scss
--rw-r--r--   0 root         (0) root         (0)    17555 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_icons.scss
--rw-r--r--   0 root         (0) root         (0)     1078 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_mixins.scss
--rw-r--r--   0 root         (0) root         (0)      753 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_path.scss
--rw-r--r--   0 root         (0) root         (0)     8061 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_variables.scss
--rw-r--r--   0 root         (0) root         (0)    22328 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/font-awesome-ie7.scss
--rw-r--r--   0 root         (0) root         (0)     1284 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/font-awesome.scss
--rw-r--r--   0 root         (0) root         (0)   276410 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome.zip
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/ico/
--rw-r--r--   0 root         (0) root         (0)     1150 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/ico/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/
--rw-r--r--   0 root         (0) root         (0)     2290 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/contribution-sample.png
--rw-r--r--   0 root         (0) root         (0)   114822 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/fort_awesome.jpg
--rw-r--r--   0 root         (0) root         (0)     8777 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/glyphicons-halflings-white.png
--rw-r--r--   0 root         (0) root         (0)    12764 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/glyphicons-halflings.png
--rw-r--r--   0 root         (0) root         (0)   184736 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/icon-flag.pdf
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/
--rw-r--r--   0 root         (0) root         (0)     8400 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/ZeroClipboard-1.1.7.min.js
--rw-r--r--   0 root         (0) root         (0)     1635 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/ZeroClipboard-1.1.7.swf
--rw-r--r--   0 root         (0) root         (0)    15922 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/backbone.min.js
--rw-r--r--   0 root         (0) root         (0)    28538 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/bootstrap-2.3.1.min.js
--rw-r--r--   0 root         (0) root         (0)    31596 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/bootstrap-222.min.js
--rw-r--r--   0 root         (0) root         (0)    93868 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/jquery-1.7.1.min.js
--rw-r--r--   0 root         (0) root         (0)    13632 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/prettify.min.js
--rw-r--r--   0 root         (0) root         (0)     1000 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/site.js
--rw-r--r--   0 root         (0) root         (0)    12140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/underscore.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/
--rw-r--r--   0 root         (0) root         (0)      636 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/accordion.less
--rw-r--r--   0 root         (0) root         (0)     1369 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/alerts.less
--rw-r--r--   0 root         (0) root         (0)     1489 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/bootstrap.less
--rw-r--r--   0 root         (0) root         (0)      431 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/breadcrumbs.less
--rw-r--r--   0 root         (0) root         (0)     5709 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/button-groups.less
--rw-r--r--   0 root         (0) root         (0)     4766 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/buttons.less
--rw-r--r--   0 root         (0) root         (0)     2482 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/carousel.less
--rw-r--r--   0 root         (0) root         (0)      644 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/close.less
--rw-r--r--   0 root         (0) root         (0)     1282 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/code.less
--rw-r--r--   0 root         (0) root         (0)      306 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/component-animations.less
--rw-r--r--   0 root         (0) root         (0)     5695 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/dropdowns.less
--rw-r--r--   0 root         (0) root         (0)    15866 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/forms.less
--rw-r--r--   0 root         (0) root         (0)      429 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/grid.less
--rw-r--r--   0 root         (0) root         (0)      521 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/hero-unit.less
--rw-r--r--   0 root         (0) root         (0)     1884 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/labels-badges.less
--rw-r--r--   0 root         (0) root         (0)      329 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/layouts.less
--rw-r--r--   0 root         (0) root         (0)      860 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/media.less
--rw-r--r--   0 root         (0) root         (0)    23042 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/mixins.less
--rw-r--r--   0 root         (0) root         (0)     1978 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/modals.less
--rw-r--r--   0 root         (0) root         (0)    12002 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/navbar.less
--rw-r--r--   0 root         (0) root         (0)     8163 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/navs.less
--rw-r--r--   0 root         (0) root         (0)      760 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/pager.less
--rw-r--r--   0 root         (0) root         (0)     2678 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/pagination.less
--rw-r--r--   0 root         (0) root         (0)     3077 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/popovers.less
--rw-r--r--   0 root         (0) root         (0)     2858 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/progress-bars.less
--rw-r--r--   0 root         (0) root         (0)     4201 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/reset.less
--rw-r--r--   0 root         (0) root         (0)      565 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-1200px-min.less
--rw-r--r--   0 root         (0) root         (0)     3920 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-767px-max.less
--rw-r--r--   0 root         (0) root         (0)      463 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-768px-979px.less
--rw-r--r--   0 root         (0) root         (0)     4328 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-navbar.less
--rw-r--r--   0 root         (0) root         (0)     1602 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-utilities.less
--rw-r--r--   0 root         (0) root         (0)     1069 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive.less
--rw-r--r--   0 root         (0) root         (0)      885 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/scaffolding.less
--rw-r--r--   0 root         (0) root         (0)    10841 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/sprites.less
--rw-r--r--   0 root         (0) root         (0)     6255 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/tables.less
--rw-r--r--   0 root         (0) root         (0)     1192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/thumbnails.less
--rw-r--r--   0 root         (0) root         (0)     1684 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/tooltip.less
--rw-r--r--   0 root         (0) root         (0)     4857 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/type.less
--rw-r--r--   0 root         (0) root         (0)      335 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/utilities.less
--rw-r--r--   0 root         (0) root         (0)     9142 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/variables.less
--rw-r--r--   0 root         (0) root         (0)      552 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/wells.less
--rw-r--r--   0 root         (0) root         (0)     3382 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/lazy.less
--rw-r--r--   0 root         (0) root         (0)     2374 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/mixins.less
--rw-r--r--   0 root         (0) root         (0)      921 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-1200px-min.less
--rw-r--r--   0 root         (0) root         (0)     1595 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-767px-max.less
--rw-r--r--   0 root         (0) root         (0)     1230 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-768px-979px.less
--rw-r--r--   0 root         (0) root         (0)      170 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-navbar.less
--rw-r--r--   0 root         (0) root         (0)     1405 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive.less
--rw-r--r--   0 root         (0) root         (0)     7153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/site.less
--rw-r--r--   0 root         (0) root         (0)      378 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/sticky-footer.less
--rw-r--r--   0 root         (0) root         (0)    10482 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/variables.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/cheatsheet/
--rw-r--r--   0 root         (0) root         (0)    61253 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/cheatsheet/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/community/
--rw-r--r--   0 root         (0) root         (0)    16656 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/community/index.html
--rw-r--r--   0 root         (0) root         (0)       55 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/design.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/examples/
--rw-r--r--   0 root         (0) root         (0)    42204 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/examples/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/get-started/
--rw-r--r--   0 root         (0) root         (0)    16041 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/get-started/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adjust/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adjust/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adn/
--rw-r--r--   0 root         (0) root         (0)    10039 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adn/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-center/
--rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-center/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-justify/
--rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-justify/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-left/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-right/
--rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ambulance/
--rw-r--r--   0 root         (0) root         (0)    10119 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ambulance/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/anchor/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/anchor/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/android/
--rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/android/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-down/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-left/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-right/
--rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-up/
--rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/apple/
--rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/apple/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/archive/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/archive/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-down/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-left/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-right/
--rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-up/
--rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/asterisk/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/asterisk/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/backward/
--rw-r--r--   0 root         (0) root         (0)    10111 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/backward/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ban-circle/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ban-circle/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bar-chart/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bar-chart/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/barcode/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/barcode/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beaker/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beaker/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beer/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beer/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell-alt/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket/
--rw-r--r--   0 root         (0) root         (0)    10117 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket-sign/
--rw-r--r--   0 root         (0) root         (0)    10182 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bold/
--rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bold/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bolt/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bolt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/book/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/book/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark-empty/
--rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark-empty/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/briefcase/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/briefcase/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/btc/
--rw-r--r--   0 root         (0) root         (0)    10158 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/btc/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bug/
--rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bug/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/building/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/building/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullhorn/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullhorn/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullseye/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullseye/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar-empty/
--rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar-empty/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera-retro/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera-retro/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-down/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-left/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-right/
--rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-up/
--rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/certificate/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/certificate/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-empty/
--rw-r--r--   0 root         (0) root         (0)    10239 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-empty/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-minus/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-minus/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-sign/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-down/
--rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-left/
--rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-right/
--rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-down/
--rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-left/
--rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-right/
--rw-r--r--   0 root         (0) root         (0)    10240 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-up/
--rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-up/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-down/
--rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-left/
--rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-right/
--rw-r--r--   0 root         (0) root         (0)    10240 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-up/
--rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-blank/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-blank/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-download/
--rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-download/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-upload/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-upload/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cny/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cny/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code-fork/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code-fork/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/coffee/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/coffee/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cog/
--rw-r--r--   0 root         (0) root         (0)    10130 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cog/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cogs/
--rw-r--r--   0 root         (0) root         (0)    10144 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cogs/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-alt/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-top/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-top/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/columns/
--rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/columns/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment-alt/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments-alt/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/compass/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/compass/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/copy/
--rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/copy/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/credit-card/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/credit-card/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/crop/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/crop/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/css3/
--rw-r--r--   0 root         (0) root         (0)    10052 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/css3/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cut/
--rw-r--r--   0 root         (0) root         (0)    10045 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cut/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dashboard/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dashboard/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/desktop/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/desktop/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-down/
--rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-left/
--rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-right/
--rw-r--r--   0 root         (0) root         (0)    10240 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-up/
--rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download-alt/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dribbble/
--rw-r--r--   0 root         (0) root         (0)    10104 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dribbble/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dropbox/
--rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dropbox/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit-sign/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eject/
--rw-r--r--   0 root         (0) root         (0)    10072 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eject/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-horizontal/
--rw-r--r--   0 root         (0) root         (0)    10257 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-horizontal/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-vertical/
--rw-r--r--   0 root         (0) root         (0)    10231 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-vertical/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope-alt/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eraser/
--rw-r--r--   0 root         (0) root         (0)    10126 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eraser/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eur/
--rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eur/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exchange/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exchange/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation-sign/
--rw-r--r--   0 root         (0) root         (0)    10218 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand-alt/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link/
--rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link-sign/
--rw-r--r--   0 root         (0) root         (0)    10244 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-close/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-close/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-open/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-open/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook/
--rw-r--r--   0 root         (0) root         (0)    10104 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook-sign/
--rw-r--r--   0 root         (0) root         (0)    10169 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facetime-video/
--rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facetime-video/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-backward/
--rw-r--r--   0 root         (0) root         (0)    10176 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-backward/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-forward/
--rw-r--r--   0 root         (0) root         (0)    10163 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-forward/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/female/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/female/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fighter-jet/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fighter-jet/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file/
--rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-alt/
--rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text/
--rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text-alt/
--rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/film/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/film/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/filter/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/filter/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire-extinguisher/
--rw-r--r--   0 root         (0) root         (0)    10231 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire-extinguisher/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-alt/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-checkered/
--rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-checkered/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flickr/
--rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flickr/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close-alt/
--rw-r--r--   0 root         (0) root         (0)    10218 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open-alt/
--rw-r--r--   0 root         (0) root         (0)    10205 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/font/
--rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/font/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/food/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/food/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/forward/
--rw-r--r--   0 root         (0) root         (0)    10098 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/forward/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/foursquare/
--rw-r--r--   0 root         (0) root         (0)    10130 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/foursquare/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/frown/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/frown/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fullscreen/
--rw-r--r--   0 root         (0) root         (0)    10137 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fullscreen/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gamepad/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gamepad/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gbp/
--rw-r--r--   0 root         (0) root         (0)    10042 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gbp/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gift/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gift/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github/
--rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-alt/
--rw-r--r--   0 root         (0) root         (0)    10130 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-sign/
--rw-r--r--   0 root         (0) root         (0)    10143 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gittip/
--rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gittip/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/glass/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/glass/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/globe/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/globe/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus/
--rw-r--r--   0 root         (0) root         (0)    10143 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus-sign/
--rw-r--r--   0 root         (0) root         (0)    10208 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/group/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/group/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/h-sign/
--rw-r--r--   0 root         (0) root         (0)    10080 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/h-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-down/
--rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-left/
--rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-right/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-up/
--rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hdd/
--rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hdd/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/headphones/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/headphones/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart-empty/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart-empty/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/home/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/home/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hospital/
--rw-r--r--   0 root         (0) root         (0)    10106 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hospital/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/html5/
--rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/html5/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inbox/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inbox/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-left/
--rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-right/
--rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info-sign/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inr/
--rw-r--r--   0 root         (0) root         (0)    10124 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inr/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/instagram/
--rw-r--r--   0 root         (0) root         (0)    10117 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/instagram/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/italic/
--rw-r--r--   0 root         (0) root         (0)    10084 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/italic/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/jpy/
--rw-r--r--   0 root         (0) root         (0)    10122 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/jpy/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/key/
--rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/key/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/keyboard/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/keyboard/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/krw/
--rw-r--r--   0 root         (0) root         (0)    10122 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/krw/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/laptop/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/laptop/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/leaf/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/leaf/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/legal/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/legal/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lemon/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lemon/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-down/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-up/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lightbulb/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lightbulb/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/link/
--rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/link/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin/
--rw-r--r--   0 root         (0) root         (0)    10104 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin-sign/
--rw-r--r--   0 root         (0) root         (0)    10169 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linux/
--rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linux/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list/
--rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-alt/
--rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ol/
--rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ol/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ul/
--rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ul/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/location-arrow/
--rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/location-arrow/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lock/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lock/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-down/
--rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-left/
--rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-right/
--rw-r--r--   0 root         (0) root         (0)    10214 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-up/
--rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magic/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magic/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magnet/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magnet/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mail-reply-all/
--rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mail-reply-all/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/male/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/male/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/map-marker/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/map-marker/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/maxcdn/
--rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/maxcdn/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/medkit/
--rw-r--r--   0 root         (0) root         (0)    10080 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/medkit/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/meh/
--rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/meh/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone-off/
--rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone-off/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign-alt/
--rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mobile-phone/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mobile-phone/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/money/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/money/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/moon/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/moon/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/move/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/move/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/music/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/music/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/off/
--rw-r--r--   0 root         (0) root         (0)    10135 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/off/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok/
--rw-r--r--   0 root         (0) root         (0)    10036 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-circle/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-circle/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-sign/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paper-clip/
--rw-r--r--   0 root         (0) root         (0)    10222 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paper-clip/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paste/
--rw-r--r--   0 root         (0) root         (0)    10071 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paste/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pause/
--rw-r--r--   0 root         (0) root         (0)    10072 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pause/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pencil/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pencil/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone-sign/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/picture/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/picture/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest/
--rw-r--r--   0 root         (0) root         (0)    10117 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest-sign/
--rw-r--r--   0 root         (0) root         (0)    10182 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plane/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plane/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play/
--rw-r--r--   0 root         (0) root         (0)    10059 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-circle/
--rw-r--r--   0 root         (0) root         (0)    10150 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-circle/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-sign/
--rw-r--r--   0 root         (0) root         (0)    10124 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign-alt/
--rw-r--r--   0 root         (0) root         (0)    10213 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/print/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/print/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pushpin/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pushpin/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/puzzle-piece/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/puzzle-piece/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/qrcode/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/qrcode/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question-sign/
--rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-left/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-left/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-right/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-right/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/random/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/random/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/refresh/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/refresh/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-circle/
--rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-circle/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-sign/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/renren/
--rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/renren/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reorder/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reorder/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/repeat/
--rw-r--r--   0 root         (0) root         (0)    10173 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/repeat/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply/
--rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply-all/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply-all/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-full/
--rw-r--r--   0 root         (0) root         (0)    10150 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-full/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-horizontal/
--rw-r--r--   0 root         (0) root         (0)    10231 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-horizontal/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-small/
--rw-r--r--   0 root         (0) root         (0)    10163 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-small/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-vertical/
--rw-r--r--   0 root         (0) root         (0)    10205 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-vertical/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/retweet/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/retweet/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/road/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/road/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rocket/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rocket/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss/
--rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss-sign/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/save/
--rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/save/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/screenshot/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/screenshot/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/search/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/search/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-alt/
--rw-r--r--   0 root         (0) root         (0)    10216 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-sign/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shield/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shield/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shopping-cart/
--rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shopping-cart/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sign-blank/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sign-blank/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signal/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signal/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signin/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signin/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signout/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signout/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sitemap/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sitemap/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/skype/
--rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/skype/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/smile/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/smile/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet/
--rw-r--r--   0 root         (0) root         (0)    10218 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet-alt/
--rw-r--r--   0 root         (0) root         (0)    10270 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes/
--rw-r--r--   0 root         (0) root         (0)    10244 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes-alt/
--rw-r--r--   0 root         (0) root         (0)    10296 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order/
--rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order-alt/
--rw-r--r--   0 root         (0) root         (0)    10231 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-down/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-up/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/spinner/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/spinner/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stackexchange/
--rw-r--r--   0 root         (0) root         (0)    10169 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stackexchange/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-empty/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-empty/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half-empty/
--rw-r--r--   0 root         (0) root         (0)    10296 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half-empty/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-backward/
--rw-r--r--   0 root         (0) root         (0)    10176 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-backward/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-forward/
--rw-r--r--   0 root         (0) root         (0)    10163 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-forward/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stethoscope/
--rw-r--r--   0 root         (0) root         (0)    10145 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stethoscope/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stop/
--rw-r--r--   0 root         (0) root         (0)    10059 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stop/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/strikethrough/
--rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/strikethrough/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/subscript/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/subscript/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/suitcase/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/suitcase/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sun/
--rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sun/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/superscript/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/superscript/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/table/
--rw-r--r--   0 root         (0) root         (0)    10071 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/table/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tablet/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tablet/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tag/
--rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tag/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tags/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tags/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tasks/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tasks/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/terminal/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/terminal/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-height/
--rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-height/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-width/
--rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-width/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th/
--rw-r--r--   0 root         (0) root         (0)    10032 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-large/
--rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-large/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-list/
--rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-list/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down-alt/
--rw-r--r--   0 root         (0) root         (0)    10205 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up-alt/
--rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ticket/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ticket/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/time/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/time/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tint/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tint/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trash/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trash/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trello/
--rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trello/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trophy/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trophy/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/truck/
--rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/truck/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr/
--rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr-sign/
--rw-r--r--   0 root         (0) root         (0)    10143 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter/
--rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter-sign/
--rw-r--r--   0 root         (0) root         (0)    10156 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/umbrella/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/umbrella/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/underline/
--rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/underline/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/undo/
--rw-r--r--   0 root         (0) root         (0)    10146 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/undo/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlink/
--rw-r--r--   0 root         (0) root         (0)    10084 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlink/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock-alt/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload-alt/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload-alt/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/usd/
--rw-r--r--   0 root         (0) root         (0)    10125 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/usd/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user/
--rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user-md/
--rw-r--r--   0 root         (0) root         (0)    10093 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user-md/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/vk/
--rw-r--r--   0 root         (0) root         (0)    10026 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/vk/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-down/
--rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-down/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-off/
--rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-off/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-up/
--rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-up/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/warning-sign/
--rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/warning-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/weibo/
--rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/weibo/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/windows/
--rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/windows/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/wrench/
--rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/wrench/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing/
--rw-r--r--   0 root         (0) root         (0)    10052 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing-sign/
--rw-r--r--   0 root         (0) root         (0)    10117 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube/
--rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-play/
--rw-r--r--   0 root         (0) root         (0)    10195 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-play/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-sign/
--rw-r--r--   0 root         (0) root         (0)    10156 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-sign/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-in/
--rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-in/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-out/
--rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-out/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icons/
--rw-r--r--   0 root         (0) root         (0)    63049 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icons/index.html
--rw-r--r--   0 root         (0) root         (0)    50111 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icons.yml
--rw-r--r--   0 root         (0) root         (0)    15711 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/license/
--rw-r--r--   0 root         (0) root         (0)    12107 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/license/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/test/
--rw-r--r--   0 root         (0) root         (0)    44340 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/test/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/whats-new/
--rw-r--r--   0 root         (0) root         (0)    21505 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/whats-new/index.html
--rw-r--r--   0 root         (0) root         (0)       14 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/CNAME
--rw-r--r--   0 root         (0) root         (0)     1292 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/Makefile
--rw-r--r--   0 root         (0) root         (0)     5564 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/README.md-nobuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/
--rw-r--r--   0 root         (0) root         (0)     1136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/accessibility-facdn.html
--rw-r--r--   0 root         (0) root         (0)     6020 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/accessibility-manual.html
--rw-r--r--   0 root         (0) root         (0)      703 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/background.html
--rw-r--r--   0 root         (0) root         (0)      848 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/cta-cdn-ally.html
--rw-r--r--   0 root         (0) root         (0)     1285 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/other.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/ads/
--rw-r--r--   0 root         (0) root         (0)      150 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/ads/carbon.html
--rw-r--r--   0 root         (0) root         (0)      439 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/brand-adblock-warning.html
--rw-r--r--   0 root         (0) root         (0)      476 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/brand-license.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/code/
--rw-r--r--   0 root         (0) root         (0)      374 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/code/core.less
--rw-r--r--   0 root         (0) root         (0)      380 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/code/core.scss
--rw-r--r--   0 root         (0) root         (0)      311 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/code/license.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/
--rw-r--r--   0 root         (0) root         (0)     1093 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/getting-support.html
--rw-r--r--   0 root         (0) root         (0)      277 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/project-milestones.html
--rw-r--r--   0 root         (0) root         (0)      811 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/reporting-bugs.html
--rw-r--r--   0 root         (0) root         (0)     1473 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/requesting-new-icons.html
--rw-r--r--   0 root         (0) root         (0)      614 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/submitting-pull-requests.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/
--rw-r--r--   0 root         (0) root         (0)     3814 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/accessible.html
--rw-r--r--   0 root         (0) root         (0)     2778 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/animated.html
--rw-r--r--   0 root         (0) root         (0)     1628 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/basic.html
--rw-r--r--   0 root         (0) root         (0)     4388 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/bootstrap.html
--rw-r--r--   0 root         (0) root         (0)     1422 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/bordered-pulled.html
--rw-r--r--   0 root         (0) root         (0)      625 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/custom.html
--rw-r--r--   0 root         (0) root         (0)     1852 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/fixed-width.html
--rw-r--r--   0 root         (0) root         (0)     1815 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/larger.html
--rw-r--r--   0 root         (0) root         (0)     1325 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/list.html
--rw-r--r--   0 root         (0) root         (0)     1772 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/rotated-flipped.html
--rw-r--r--   0 root         (0) root         (0)     2614 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/stacked.html
--rw-r--r--   0 root         (0) root         (0)     2311 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/footer.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/
--rw-r--r--   0 root         (0) root         (0)      604 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/accessibility.html
--rw-r--r--   0 root         (0) root         (0)      764 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/brand.html
--rw-r--r--   0 root         (0) root         (0)      574 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/chart.html
--rw-r--r--   0 root         (0) root         (0)      589 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/currency.html
--rw-r--r--   0 root         (0) root         (0)      604 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/directional.html
--rw-r--r--   0 root         (0) root         (0)      594 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/file-type.html
--rw-r--r--   0 root         (0) root         (0)      608 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/form-control.html
--rw-r--r--   0 root         (0) root         (0)      579 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/gender.html
--rw-r--r--   0 root         (0) root         (0)      569 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/hand.html
--rw-r--r--   0 root         (0) root         (0)      584 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/medical.html
--rw-r--r--   0 root         (0) root         (0)     1069 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/new.html
--rw-r--r--   0 root         (0) root         (0)      584 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/payment.html
--rw-r--r--   0 root         (0) root         (0)      995 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/spinner.html
--rw-r--r--   0 root         (0) root         (0)      604 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/text-editor.html
--rw-r--r--   0 root         (0) root         (0)      619 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/transportation.html
--rw-r--r--   0 root         (0) root         (0)      609 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/video-player.html
--rw-r--r--   0 root         (0) root         (0)      624 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/web-application.html
--rw-r--r--   0 root         (0) root         (0)     4083 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/jumbotron-carousel.html
--rw-r--r--   0 root         (0) root         (0)      382 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/jumbotron.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/modals/
--rw-r--r--   0 root         (0) root         (0)     3557 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/modals/download.html
--rw-r--r--   0 root         (0) root         (0)     2929 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/modals/fa5.html
--rw-r--r--   0 root         (0) root         (0)     8209 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/navbar.html
--rw-r--r--   0 root         (0) root         (0)     1505 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/new-features.html
--rw-r--r--   0 root         (0) root         (0)     5308 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/new-naming.html
--rw-r--r--   0 root         (0) root         (0)      519 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/new-upgrading.html
--rw-r--r--   0 root         (0) root         (0)      889 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/newsletter-subscribe.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/
--rw-r--r--   0 root         (0) root         (0)     1442 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/camera-retro-tee.html
--rw-r--r--   0 root         (0) root         (0)     1429 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/classics-tee.html
--rw-r--r--   0 root         (0) root         (0)      755 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/cta-suggestions.html
--rw-r--r--   0 root         (0) root         (0)     1328 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/fa-ther-tee.html
--rw-r--r--   0 root         (0) root         (0)     1440 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/green-logo-tee.html
--rw-r--r--   0 root         (0) root         (0)     1431 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/old-skool-tee.html
--rw-r--r--   0 root         (0) root         (0)     1134 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/rock-paper-scissors-lizard-spock-tee.html
--rw-r--r--   0 root         (0) root         (0)     1403 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/space-shuttle-tee.html
--rw-r--r--   0 root         (0) root         (0)     1735 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/white-logo-tee.html
--rw-r--r--   0 root         (0) root         (0)      139 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/stripe-ad.html
--rw-r--r--   0 root         (0) root         (0)     1330 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/stripe-social.html
--rw-r--r--   0 root         (0) root         (0)      978 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tell-me-thanks.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/
--rw-r--r--   0 root         (0) root         (0)      589 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped-inside-anchor.html
--rw-r--r--   0 root         (0) root         (0)      733 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped-inside-btn.html
--rw-r--r--   0 root         (0) root         (0)      493 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped.html
--rw-r--r--   0 root         (0) root         (0)     1842 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked-inside-anchor.html
--rw-r--r--   0 root         (0) root         (0)      151 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked-with-text.html
--rw-r--r--   0 root         (0) root         (0)     1818 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked.html
--rw-r--r--   0 root         (0) root         (0)     1174 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/thanks-to.html
--rw-r--r--   0 root         (0) root         (0)     2321 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/why.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_layouts/
--rw-r--r--   0 root         (0) root         (0)     4320 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_layouts/base.html
--rw-r--r--   0 root         (0) root         (0)     3502 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_layouts/icon.html
--rw-r--r--   0 root         (0) root         (0)     1174 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_layouts/survey.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_plugins/
--rw-r--r--   0 root         (0) root         (0)      998 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_plugins/flatten_icon_filters.rb
--rw-r--r--   0 root         (0) root         (0)      885 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_plugins/icon_page_generator.rb
--rw-r--r--   0 root         (0) root         (0)     2973 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_plugins/site.rb
--rw-r--r--   0 root         (0) root         (0)     1265 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/accessibility.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/css/
--rw-r--r--   0 root         (0) root         (0)      815 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/css/prettify.css
--rw-r--r--   0 root         (0) root         (0)     3063 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/css/pygments.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/
--rw-r--r--   0 root         (0) root         (0)      323 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/HELP-US-OUT.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/
--rw-r--r--   0 root         (0) root         (0)   134808 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)   165742 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/
--rw-r--r--   0 root         (0) root         (0)      722 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/animated.less
--rw-r--r--   0 root         (0) root         (0)      594 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/bordered-pulled.less
--rw-r--r--   0 root         (0) root         (0)      115 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/core.less
--rw-r--r--   0 root         (0) root         (0)      128 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/fixed-width.less
--rw-r--r--   0 root         (0) root         (0)      368 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/font-awesome.less
--rw-r--r--   0 root         (0) root         (0)      342 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/icons.less
--rw-r--r--   0 root         (0) root         (0)      379 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/larger.less
--rw-r--r--   0 root         (0) root         (0)      386 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/list.less
--rw-r--r--   0 root         (0) root         (0)     1265 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/mixins.less
--rw-r--r--   0 root         (0) root         (0)      771 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/path.less
--rw-r--r--   0 root         (0) root         (0)      631 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/rotated-flipped.less
--rw-r--r--   0 root         (0) root         (0)      118 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/screen-reader.less
--rw-r--r--   0 root         (0) root         (0)      485 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/stacked.less
--rw-r--r--   0 root         (0) root         (0)      658 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/variables.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/
--rw-r--r--   0 root         (0) root         (0)      724 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_animated.scss
--rw-r--r--   0 root         (0) root         (0)      601 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_bordered-pulled.scss
--rw-r--r--   0 root         (0) root         (0)      116 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_core.scss
--rw-r--r--   0 root         (0) root         (0)      129 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_fixed-width.scss
--rw-r--r--   0 root         (0) root         (0)      344 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_icons.scss
--rw-r--r--   0 root         (0) root         (0)      384 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_larger.scss
--rw-r--r--   0 root         (0) root         (0)      387 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_list.scss
--rw-r--r--   0 root         (0) root         (0)     1293 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_mixins.scss
--rw-r--r--   0 root         (0) root         (0)      783 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_path.scss
--rw-r--r--   0 root         (0) root         (0)      681 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_rotated-flipped.scss
--rw-r--r--   0 root         (0) root         (0)      134 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_screen-reader.scss
--rw-r--r--   0 root         (0) root         (0)      491 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_stacked.scss
--rw-r--r--   0 root         (0) root         (0)      739 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_variables.scss
--rw-r--r--   0 root         (0) root         (0)      303 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/font-awesome.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/ico/
--rw-r--r--   0 root         (0) root         (0)    52047 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/ico/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/img/
--rw-r--r--   0 root         (0) root         (0)    72993 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/img/algolia.png
--rw-r--r--   0 root         (0) root         (0)    14209 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/img/logo-themeisle.png
--rw-r--r--   0 root         (0) root         (0)     8268 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/img/logo-wpbeginner.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/
--rw-r--r--   0 root         (0) root         (0)     8400 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/ZeroClipboard-1.1.7.min.js
--rw-r--r--   0 root         (0) root         (0)     1635 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/ZeroClipboard-1.1.7.swf
--rw-r--r--   0 root         (0) root         (0)     2376 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/html5shiv.js
--rw-r--r--   0 root         (0) root         (0)    20740 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/monetization.js
--rw-r--r--   0 root         (0) root         (0)    13632 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/prettify.min.js
--rw-r--r--   0 root         (0) root         (0)     4035 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/respond.min.js
--rw-r--r--   0 root         (0) root         (0)     3080 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/search.js
--rw-r--r--   0 root         (0) root         (0)     1562 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/site.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/
--rw-r--r--   0 root         (0) root         (0)     8099 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/.csscomb.json
--rw-r--r--   0 root         (0) root         (0)      456 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/.csslintrc
--rw-r--r--   0 root         (0) root         (0)     1518 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/alerts.less
--rw-r--r--   0 root         (0) root         (0)     1199 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/badges.less
--rw-r--r--   0 root         (0) root         (0)     1291 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/bootstrap.less
--rw-r--r--   0 root         (0) root         (0)      594 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/breadcrumbs.less
--rw-r--r--   0 root         (0) root         (0)     5675 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/button-groups.less
--rw-r--r--   0 root         (0) root         (0)     3662 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/buttons.less
--rw-r--r--   0 root         (0) root         (0)     5407 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/carousel.less
--rw-r--r--   0 root         (0) root         (0)      764 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/close.less
--rw-r--r--   0 root         (0) root         (0)     1401 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/code.less
--rw-r--r--   0 root         (0) root         (0)      666 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/component-animations.less
--rw-r--r--   0 root         (0) root         (0)     4876 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/dropdowns.less
--rw-r--r--   0 root         (0) root         (0)    15859 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/forms.less
--rw-r--r--   0 root         (0) root         (0)    19803 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/glyphicons.less
--rw-r--r--   0 root         (0) root         (0)     1387 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/grid.less
--rw-r--r--   0 root         (0) root         (0)     4246 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/input-groups.less
--rw-r--r--   0 root         (0) root         (0)     1062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/jumbotron.less
--rw-r--r--   0 root         (0) root         (0)     1079 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/labels.less
--rw-r--r--   0 root         (0) root         (0)     3124 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/list-group.less
--rw-r--r--   0 root         (0) root         (0)      900 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/media.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/
--rw-r--r--   0 root         (0) root         (0)      257 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/alerts.less
--rw-r--r--   0 root         (0) root         (0)      151 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/background-variant.less
--rw-r--r--   0 root         (0) root         (0)      468 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/border-radius.less
--rw-r--r--   0 root         (0) root         (0)     1476 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/buttons.less
--rw-r--r--   0 root         (0) root         (0)      120 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/center-block.less
--rw-r--r--   0 root         (0) root         (0)      605 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/clearfix.less
--rw-r--r--   0 root         (0) root         (0)     2641 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/forms.less
--rw-r--r--   0 root         (0) root         (0)     4388 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/gradients.less
--rw-r--r--   0 root         (0) root         (0)     2797 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/grid-framework.less
--rw-r--r--   0 root         (0) root         (0)     3107 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/grid.less
--rw-r--r--   0 root         (0) root         (0)      574 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/hide-text.less
--rw-r--r--   0 root         (0) root         (0)     1062 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/image.less
--rw-r--r--   0 root         (0) root         (0)      161 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/labels.less
--rw-r--r--   0 root         (0) root         (0)      546 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/list-group.less
--rw-r--r--   0 root         (0) root         (0)      232 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/nav-divider.less
--rw-r--r--   0 root         (0) root         (0)      364 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/nav-vertical-align.less
--rw-r--r--   0 root         (0) root         (0)      148 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/opacity.less
--rw-r--r--   0 root         (0) root         (0)      485 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/pagination.less
--rw-r--r--   0 root         (0) root         (0)      537 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/panels.less
--rw-r--r--   0 root         (0) root         (0)      191 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/progress-bar.less
--rw-r--r--   0 root         (0) root         (0)      248 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/reset-filter.less
--rw-r--r--   0 root         (0) root         (0)      470 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/reset-text.less
--rw-r--r--   0 root         (0) root         (0)      196 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/resize.less
--rw-r--r--   0 root         (0) root         (0)      354 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/responsive-visibility.less
--rw-r--r--   0 root         (0) root         (0)      127 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/size.less
--rw-r--r--   0 root         (0) root         (0)      159 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/tab-focus.less
--rw-r--r--   0 root         (0) root         (0)      700 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/table-row.less
--rw-r--r--   0 root         (0) root         (0)      128 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/text-emphasis.less
--rw-r--r--   0 root         (0) root         (0)      162 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/text-overflow.less
--rw-r--r--   0 root         (0) root         (0)     6650 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/vendor-prefixes.less
--rw-r--r--   0 root         (0) root         (0)     1136 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins.less
--rw-r--r--   0 root         (0) root         (0)     3565 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/modals.less
--rw-r--r--   0 root         (0) root         (0)    14628 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/navbar.less
--rw-r--r--   0 root         (0) root         (0)     4930 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/navs.less
--rw-r--r--   0 root         (0) root         (0)     7559 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/normalize.less
--rw-r--r--   0 root         (0) root         (0)      861 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/pager.less
--rw-r--r--   0 root         (0) root         (0)     2059 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/pagination.less
--rw-r--r--   0 root         (0) root         (0)     6279 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/panels.less
--rw-r--r--   0 root         (0) root         (0)     3488 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/popovers.less
--rw-r--r--   0 root         (0) root         (0)     1939 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/print.less
--rw-r--r--   0 root         (0) root         (0)     1925 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/progress-bars.less
--rw-r--r--   0 root         (0) root         (0)      546 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/responsive-embed.less
--rw-r--r--   0 root         (0) root         (0)     4262 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/responsive-utilities.less
--rw-r--r--   0 root         (0) root         (0)     2988 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/scaffolding.less
--rw-r--r--   0 root         (0) root         (0)     4612 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/tables.less
--rw-r--r--   0 root         (0) root         (0)     8197 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/theme.less
--rw-r--r--   0 root         (0) root         (0)      753 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/thumbnails.less
--rw-r--r--   0 root         (0) root         (0)     2985 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/tooltip.less
--rw-r--r--   0 root         (0) root         (0)     5954 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/type.less
--rw-r--r--   0 root         (0) root         (0)      747 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/utilities.less
--rw-r--r--   0 root         (0) root         (0)    27473 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/variables.less
--rw-r--r--   0 root         (0) root         (0)      527 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/wells.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/gandy-grid/
--rw-r--r--   0 root         (0) root         (0)      920 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/gandy-grid/grid.less
--rw-r--r--   0 root         (0) root         (0)      287 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/gandy-grid/mixins.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/
--rw-r--r--   0 root         (0) root         (0)      151 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/algolia.less
--rw-r--r--   0 root         (0) root         (0)     6483 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/banner-ad.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/
--rw-r--r--   0 root         (0) root         (0)      335 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/alerts.less
--rw-r--r--   0 root         (0) root         (0)      208 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/buttons.less
--rw-r--r--   0 root         (0) root         (0)     1972 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/jumbotron.less
--rw-r--r--   0 root         (0) root         (0)      284 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/labels.less
--rw-r--r--   0 root         (0) root         (0)      133 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/modals.less
--rw-r--r--   0 root         (0) root         (0)     4172 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/navbar.less
--rw-r--r--   0 root         (0) root         (0)      213 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/panels.less
--rw-r--r--   0 root         (0) root         (0)      119 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/tooltip.less
--rw-r--r--   0 root         (0) root         (0)      414 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/type.less
--rw-r--r--   0 root         (0) root         (0)     4873 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/variables.less
--rw-r--r--   0 root         (0) root         (0)      232 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/wells.less
--rw-r--r--   0 root         (0) root         (0)      328 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bsap-ad.less
--rw-r--r--   0 root         (0) root         (0)      425 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/carbon-ad.less
--rw-r--r--   0 root         (0) root         (0)      481 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/example-rating.less
--rw-r--r--   0 root         (0) root         (0)      320 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/fa5.less
--rw-r--r--   0 root         (0) root         (0)      544 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/feature-list.less
--rw-r--r--   0 root         (0) root         (0)      695 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/fontawesome-icon-list.less
--rw-r--r--   0 root         (0) root         (0)     1180 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/footer.less
--rw-r--r--   0 root         (0) root         (0)     1746 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/jumbotron-carousel.less
--rw-r--r--   0 root         (0) root         (0)       30 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/layout.less
--rw-r--r--   0 root         (0) root         (0)     4864 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/lazy.less
--rw-r--r--   0 root         (0) root         (0)      435 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/newsletter.less
--rw-r--r--   0 root         (0) root         (0)       62 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/print.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/
--rw-r--r--   0 root         (0) root         (0)      918 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-lg.less
--rw-r--r--   0 root         (0) root         (0)       97 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-md.less
--rw-r--r--   0 root         (0) root         (0)      327 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-sm-up.less
--rw-r--r--   0 root         (0) root         (0)      874 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-sm.less
--rw-r--r--   0 root         (0) root         (0)     1764 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-xs.less
--rw-r--r--   0 root         (0) root         (0)      586 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/search.less
--rw-r--r--   0 root         (0) root         (0)      325 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/social-buttons.less
--rw-r--r--   0 root         (0) root         (0)     2145 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/store.less
--rw-r--r--   0 root         (0) root         (0)       68 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/stripe-ad.less
--rw-r--r--   0 root         (0) root         (0)      148 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/sumome.less
--rw-r--r--   0 root         (0) root         (0)    12164 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/textured-bg.less
--rw-r--r--   0 root         (0) root         (0)      896 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/views.less
--rw-r--r--   0 root         (0) root         (0)     1229 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/cdn/
--rw-r--r--   0 root         (0) root         (0)     1858 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/cdn/error.html
--rw-r--r--   0 root         (0) root         (0)     2396 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/cdn/success.html
--rw-r--r--   0 root         (0) root         (0)     1493 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/cheatsheet.html
--rw-r--r--   0 root         (0) root         (0)     1194 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/community.html
--rw-r--r--   0 root         (0) root         (0)       55 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/design.html
--rw-r--r--   0 root         (0) root         (0)     1913 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/examples.html
--rw-r--r--   0 root         (0) root         (0)    12155 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/get-started.html
--rw-r--r--   0 root         (0) root         (0)     4356 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/icons.html
--rw-r--r--   0 root         (0) root         (0)   121432 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/icons.yml
--rw-r--r--   0 root         (0) root         (0)      592 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/index.html
--rw-r--r--   0 root         (0) root         (0)     2465 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/license.html
--rw-r--r--   0 root         (0) root         (0)     2517 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/store.html
--rw-r--r--   0 root         (0) root         (0)      289 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/survey.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/
--rw-r--r--   0 root         (0) root         (0)    34746 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/2.3.2.html
--rw-r--r--   0 root         (0) root         (0)     1214 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/all.html
--rw-r--r--   0 root         (0) root         (0)    36075 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/glyphicons.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/height/
--rw-r--r--   0 root         (0) root         (0)     2288 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/height/4.4.0.html
--rw-r--r--   0 root         (0) root         (0)     2288 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/height/4.5.0.html
--rw-r--r--   0 root         (0) root         (0)     2281 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/height/current.html
--rw-r--r--   0 root         (0) root         (0)    36410 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/index.html
--rw-r--r--   0 root         (0) root         (0)     1065 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/thanks.html
--rw-r--r--   0 root         (0) root         (0)     1928 2018-01-28 22:51:54.000000 platypush-0.9.5/platypush/backend/http/static/font-awesome/src/whats-new.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/js/
--rw-r--r--   0 root         (0) root         (0)     9305 2019-01-08 18:21:23.000000 platypush-0.9.5/platypush/backend/http/static/js/application.js
--rw-r--r--   0 root         (0) root         (0)     1256 2018-06-20 22:21:49.000000 platypush-0.9.5/platypush/backend/http/static/js/assistant.google.js
--rw-r--r--   0 root         (0) root         (0)     1473 2018-06-13 18:44:07.000000 platypush-0.9.5/platypush/backend/http/static/js/dashboard.js
--rw-r--r--   0 root         (0) root         (0)     1668 2018-08-22 18:21:52.000000 platypush-0.9.5/platypush/backend/http/static/js/gpio.js
--rw-r--r--   0 root         (0) root         (0)     1484 2018-06-11 22:33:06.000000 platypush-0.9.5/platypush/backend/http/static/js/gpio.sensor.mcp3008.js
--rw-r--r--   0 root         (0) root         (0)     3746 2018-04-17 21:10:49.000000 platypush-0.9.5/platypush/backend/http/static/js/gpio.zeroborg.js
--rw-r--r--   0 root         (0) root         (0)    86927 2018-01-28 17:47:10.000000 platypush-0.9.5/platypush/backend/http/static/js/jquery-3.3.1.min.js
--rw-r--r--   0 root         (0) root         (0)   253668 2018-06-18 22:37:33.000000 platypush-0.9.5/platypush/backend/http/static/js/jquery-ui-1.12.1.min.js
--rw-r--r--   0 root         (0) root         (0)    27459 2019-01-09 14:04:43.000000 platypush-0.9.5/platypush/backend/http/static/js/light.hue.js
--rw-r--r--   0 root         (0) root         (0)     6938 2018-06-13 18:40:49.000000 platypush-0.9.5/platypush/backend/http/static/js/map.js
--rw-r--r--   0 root         (0) root         (0)    28775 2019-01-10 21:27:10.000000 platypush-0.9.5/platypush/backend/http/static/js/music.mpd.js
--rw-r--r--   0 root         (0) root         (0)    20211 2019-01-10 15:50:01.000000 platypush-0.9.5/platypush/backend/http/static/js/music.snapcast.js
--rw-r--r--   0 root         (0) root         (0)      697 2018-05-04 11:06:18.000000 platypush-0.9.5/platypush/backend/http/static/js/pushbullet.js
--rw-r--r--   0 root         (0) root         (0)      370 2018-01-28 19:40:20.000000 platypush-0.9.5/platypush/backend/http/static/js/skeleton-tabs.js
--rw-r--r--   0 root         (0) root         (0)      837 2018-05-11 18:40:45.000000 platypush-0.9.5/platypush/backend/http/static/js/switch.switchbot.js
--rw-r--r--   0 root         (0) root         (0)     2455 2018-06-26 20:58:28.000000 platypush-0.9.5/platypush/backend/http/static/js/switch.tplink.js
--rw-r--r--   0 root         (0) root         (0)     2365 2018-06-26 20:01:59.000000 platypush-0.9.5/platypush/backend/http/static/js/switch.wemo.js
--rw-r--r--   0 root         (0) root         (0)      793 2018-10-14 15:16:40.000000 platypush-0.9.5/platypush/backend/http/static/js/tts.google.js
--rw-r--r--   0 root         (0) root         (0)      786 2018-04-17 21:10:49.000000 platypush-0.9.5/platypush/backend/http/static/js/tts.js
--rw-r--r--   0 root         (0) root         (0)     4757 2018-04-29 14:14:46.000000 platypush-0.9.5/platypush/backend/http/static/js/video.omxplayer.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/js/widgets/
--rw-r--r--   0 root         (0) root         (0)     2854 2018-06-06 00:26:28.000000 platypush-0.9.5/platypush/backend/http/static/js/widgets/calendar.js
--rw-r--r--   0 root         (0) root         (0)     3328 2018-06-25 18:25:10.000000 platypush-0.9.5/platypush/backend/http/static/js/widgets/date-time-weather.js
--rw-r--r--   0 root         (0) root         (0)     1680 2018-09-15 16:25:17.000000 platypush-0.9.5/platypush/backend/http/static/js/widgets/image-carousel.js
--rw-r--r--   0 root         (0) root         (0)     5844 2018-08-17 22:35:57.000000 platypush-0.9.5/platypush/backend/http/static/js/widgets/music.js
--rw-r--r--   0 root         (0) root         (0)     2440 2018-09-15 16:25:27.000000 platypush-0.9.5/platypush/backend/http/static/js/widgets/rss-news.js
--rw-r--r--   0 root         (0) root         (0)    18950 2018-06-23 11:26:20.000000 platypush-0.9.5/platypush/backend/http/static/js/widgets/skycons.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/static/resources/
--rw-r--r--   0 root         (0) root         (0)       91 2018-05-05 00:31:10.000000 platypush-0.9.5/platypush/backend/http/static/resources/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/templates/
--rw-r--r--   0 root         (0) root         (0)     3323 2018-11-01 23:07:20.000000 platypush-0.9.5/platypush/backend/http/templates/dashboard.html
--rw-r--r--   0 root         (0) root         (0)     3182 2019-01-07 18:02:03.000000 platypush-0.9.5/platypush/backend/http/templates/index.html
--rw-r--r--   0 root         (0) root         (0)     1926 2018-11-01 23:07:39.000000 platypush-0.9.5/platypush/backend/http/templates/map.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      208 2018-04-17 21:10:49.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/assistant.google.html
--rw-r--r--   0 root         (0) root         (0)      229 2018-08-22 17:15:15.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/gpio.html
--rw-r--r--   0 root         (0) root         (0)      262 2018-04-30 07:39:49.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/gpio.sensor.mcp3008.html
--rw-r--r--   0 root         (0) root         (0)     1692 2018-04-12 18:07:28.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/gpio.zeroborg.html
--rw-r--r--   0 root         (0) root         (0)     1093 2019-01-02 20:06:58.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/light.hue.html
--rw-r--r--   0 root         (0) root         (0)     6563 2018-05-03 00:17:03.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/music.mpd.html
--rw-r--r--   0 root         (0) root         (0)     7059 2019-01-10 15:50:01.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/music.snapcast.html
--rw-r--r--   0 root         (0) root         (0)      262 2018-04-30 07:39:49.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/serial.html
--rw-r--r--   0 root         (0) root         (0)      818 2018-05-11 18:40:45.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/switch.switchbot.html
--rw-r--r--   0 root         (0) root         (0)      249 2018-06-26 19:50:39.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/switch.tplink.html
--rw-r--r--   0 root         (0) root         (0)      243 2018-05-08 07:16:12.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/switch.wemo.html
--rw-r--r--   0 root         (0) root         (0)      681 2018-10-14 15:23:35.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/tts.google.html
--rw-r--r--   0 root         (0) root         (0)      668 2018-04-17 21:10:49.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/tts.html
--rw-r--r--   0 root         (0) root         (0)     2930 2018-04-24 12:41:20.000000 platypush-0.9.5/platypush/backend/http/templates/plugins/video.omxplayer.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/http/templates/widgets/
--rw-r--r--   0 root         (0) root         (0)      466 2018-05-04 17:44:41.000000 platypush-0.9.5/platypush/backend/http/templates/widgets/calendar.html
--rw-r--r--   0 root         (0) root         (0)     1094 2018-06-23 11:26:20.000000 platypush-0.9.5/platypush/backend/http/templates/widgets/date-time-weather.html
--rw-r--r--   0 root         (0) root         (0)      548 2018-05-07 14:53:51.000000 platypush-0.9.5/platypush/backend/http/templates/widgets/image-carousel.html
--rw-r--r--   0 root         (0) root         (0)     2032 2018-08-17 23:01:51.000000 platypush-0.9.5/platypush/backend/http/templates/widgets/music.html
--rw-r--r--   0 root         (0) root         (0)      244 2018-05-05 12:53:08.000000 platypush-0.9.5/platypush/backend/http/templates/widgets/rss-news.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/inotify/
--rw-r--r--   0 root         (0) root         (0)     2834 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/inotify/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1302 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/joystick.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/kafka/
--rw-r--r--   0 root         (0) root         (0)     3187 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/kafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/light/
--rw-r--r--   0 root         (0) root         (0)        0 2019-01-09 14:13:02.000000 platypush-0.9.5/platypush/backend/light/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3243 2019-01-10 22:38:31.000000 platypush-0.9.5/platypush/backend/light/hue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/local/
--rw-r--r--   0 root         (0) root         (0)     2487 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/local/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4383 2018-12-26 22:40:45.000000 platypush-0.9.5/platypush/backend/midi.py
--rw-r--r--   0 root         (0) root         (0)     5575 2019-01-13 19:38:43.000000 platypush-0.9.5/platypush/backend/mqtt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/music/
--rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/music/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/music/mpd/
--rw-r--r--   0 root         (0) root         (0)     5000 2019-01-12 01:15:05.000000 platypush-0.9.5/platypush/backend/music/mpd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8041 2019-01-13 19:39:23.000000 platypush-0.9.5/platypush/backend/music/snapcast.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/pushbullet/
--rw-r--r--   0 root         (0) root         (0)     4822 2018-12-27 21:44:03.000000 platypush-0.9.5/platypush/backend/pushbullet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2610 2018-12-26 14:24:49.000000 platypush-0.9.5/platypush/backend/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/scard/
--rw-r--r--   0 root         (0) root         (0)     2996 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/scard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/sensor/
--rw-r--r--   0 root         (0) root         (0)     3740 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/sensor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      602 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/sensor/accelerometer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/sensor/distance/
--rw-r--r--   0 root         (0) root         (0)      547 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/sensor/distance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/sensor/ir/
--rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/sensor/ir/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/sensor/ir/zeroborg/
--rw-r--r--   0 root         (0) root         (0)     2162 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/sensor/ir/zeroborg/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/sensor/ir/zeroborg/scan.py
--rw-r--r--   0 root         (0) root         (0)     9316 2018-12-27 18:57:06.000000 platypush-0.9.5/platypush/backend/sensor/leap.py
--rw-r--r--   0 root         (0) root         (0)      653 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/sensor/mcp3008.py
--rw-r--r--   0 root         (0) root         (0)      575 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/sensor/serial.py
--rw-r--r--   0 root         (0) root         (0)     3272 2019-01-13 19:39:51.000000 platypush-0.9.5/platypush/backend/tcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/backend/weather/
--rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.5/platypush/backend/weather/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1335 2018-10-25 18:46:34.000000 platypush-0.9.5/platypush/backend/weather/forecast.py
--rw-r--r--   0 root         (0) root         (0)     5852 2018-11-02 16:48:45.000000 platypush-0.9.5/platypush/backend/websocket.py
--rw-r--r--   0 root         (0) root         (0)     4971 2018-12-02 22:47:41.000000 platypush-0.9.5/platypush/backend/wiimote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/bus/
--rw-r--r--   0 root         (0) root         (0)     2035 2018-10-23 20:48:24.000000 platypush-0.9.5/platypush/bus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1193 2018-11-27 23:31:22.000000 platypush-0.9.5/platypush/bus/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/config/
--rw-r--r--   0 root         (0) root         (0)     8982 2018-12-30 19:11:30.000000 platypush-0.9.5/platypush/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/context/
--rw-r--r--   0 root         (0) root         (0)     3497 2019-01-08 17:23:09.000000 platypush-0.9.5/platypush/context/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/cron/
--rw-r--r--   0 root         (0) root         (0)        0 2018-01-15 21:37:01.000000 platypush-0.9.5/platypush/cron/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2500 2018-09-26 23:51:10.000000 platypush-0.9.5/platypush/cron/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/event/
--rw-r--r--   0 root         (0) root         (0)        0 2017-12-24 00:15:01.000000 platypush-0.9.5/platypush/event/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5418 2019-01-13 19:40:13.000000 platypush-0.9.5/platypush/event/hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/event/processor/
--rw-r--r--   0 root         (0) root         (0)     1987 2018-11-02 16:48:45.000000 platypush-0.9.5/platypush/event/processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      348 2019-01-02 19:48:19.000000 platypush-0.9.5/platypush/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/
--rw-r--r--   0 root         (0) root         (0)     2101 2018-10-26 09:06:55.000000 platypush-0.9.5/platypush/message/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/
--rw-r--r--   0 root         (0) root         (0)     8544 2018-10-09 23:00:30.000000 platypush-0.9.5/platypush/message/event/__init__.py
--rw-r--r--   0 root         (0) root         (0)      745 2019-01-11 23:31:00.000000 platypush-0.9.5/platypush/message/event/adafruit.py
--rw-r--r--   0 root         (0) root         (0)      487 2018-09-24 20:07:13.000000 platypush-0.9.5/platypush/message/event/application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/assistant/
--rw-r--r--   0 root         (0) root         (0)     3276 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/assistant/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/button/
--rw-r--r--   0 root         (0) root         (0)        0 2017-12-24 12:21:59.000000 platypush-0.9.5/platypush/message/event/button/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/button/flic/
--rw-r--r--   0 root         (0) root         (0)     1586 2018-07-25 00:14:43.000000 platypush-0.9.5/platypush/message/event/button/flic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      471 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/geo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/http/
--rw-r--r--   0 root         (0) root         (0)      500 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/http/ota/
--rw-r--r--   0 root         (0) root         (0)        0 2018-01-11 17:40:02.000000 platypush-0.9.5/platypush/message/event/http/ota/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/http/ota/booking/
--rw-r--r--   0 root         (0) root         (0)      251 2018-01-16 18:56:14.000000 platypush-0.9.5/platypush/message/event/http/ota/booking/__init__.py
--rw-r--r--   0 root         (0) root         (0)      951 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/http/rss.py
--rw-r--r--   0 root         (0) root         (0)      566 2018-09-18 16:58:23.000000 platypush-0.9.5/platypush/message/event/joystick.py
--rw-r--r--   0 root         (0) root         (0)      414 2018-07-27 23:55:19.000000 platypush-0.9.5/platypush/message/event/kafka.py
--rw-r--r--   0 root         (0) root         (0)     1490 2019-01-09 08:10:33.000000 platypush-0.9.5/platypush/message/event/light.py
--rw-r--r--   0 root         (0) root         (0)      513 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/midi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/music/
--rw-r--r--   0 root         (0) root         (0)     3224 2019-01-10 00:25:07.000000 platypush-0.9.5/platypush/message/event/music/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2654 2019-01-06 17:47:47.000000 platypush-0.9.5/platypush/message/event/music/snapcast.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/path/
--rw-r--r--   0 root         (0) root         (0)     1862 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/path/__init__.py
--rw-r--r--   0 root         (0) root         (0)      366 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/ping.py
--rw-r--r--   0 root         (0) root         (0)     1118 2018-01-06 23:39:45.000000 platypush-0.9.5/platypush/message/event/pushbullet.py
--rw-r--r--   0 root         (0) root         (0)      934 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/scard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/sensor/
--rw-r--r--   0 root         (0) root         (0)     1073 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/sensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/sensor/ir/
--rw-r--r--   0 root         (0) root         (0)      862 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/sensor/ir/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1261 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/sensor/leap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/sensor/light/
--rw-r--r--   0 root         (0) root         (0)      433 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/sensor/light/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/serial/
--rw-r--r--   0 root         (0) root         (0)      495 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/serial/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1611 2018-10-22 17:06:40.000000 platypush-0.9.5/platypush/message/event/torrent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/video/
--rw-r--r--   0 root         (0) root         (0)     1238 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/video/__init__.py
--rw-r--r--   0 root         (0) root         (0)      259 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/weather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/event/web/
--rw-r--r--   0 root         (0) root         (0)      875 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)      391 2018-07-09 20:38:08.000000 platypush-0.9.5/platypush/message/event/web/widget.py
--rw-r--r--   0 root         (0) root         (0)      619 2018-12-01 17:46:32.000000 platypush-0.9.5/platypush/message/event/wiimote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/request/
--rw-r--r--   0 root         (0) root         (0)     9658 2019-01-13 19:07:31.000000 platypush-0.9.5/platypush/message/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/message/response/
--rw-r--r--   0 root         (0) root         (0)     2254 2018-10-09 23:00:30.000000 platypush-0.9.5/platypush/message/response/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/platydock/
--rwxr-xr-x   0 root         (0) root         (0)     9922 2018-12-19 23:39:16.000000 platypush-0.9.5/platypush/platydock/__init__.py
--rw-r--r--   0 root         (0) root         (0)       67 2018-12-19 01:19:59.000000 platypush-0.9.5/platypush/platydock/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/
--rw-r--r--   0 root         (0) root         (0)     1673 2019-01-13 19:07:02.000000 platypush-0.9.5/platypush/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/adafruit/
--rw-r--r--   0 root         (0) root         (0)        0 2018-07-24 07:16:52.000000 platypush-0.9.5/platypush/plugins/adafruit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7999 2019-01-12 21:42:14.000000 platypush-0.9.5/platypush/plugins/adafruit/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/assistant/
--rw-r--r--   0 root         (0) root         (0)        0 2017-12-28 08:59:41.000000 platypush-0.9.5/platypush/plugins/assistant/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/assistant/google/
--rw-r--r--   0 root         (0) root         (0)      951 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/assistant/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)      982 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/assistant/google/pushtotalk.py
--rw-r--r--   0 root         (0) root         (0)     8214 2018-12-28 08:37:16.000000 platypush-0.9.5/platypush/plugins/autoremote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/calendar/
--rw-r--r--   0 root         (0) root         (0)     3779 2018-12-20 15:39:13.000000 platypush-0.9.5/platypush/plugins/calendar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3791 2018-12-21 17:37:37.000000 platypush-0.9.5/platypush/plugins/calendar/ical.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/camera/
--rw-r--r--   0 root         (0) root         (0)        0 2018-06-13 21:37:41.000000 platypush-0.9.5/platypush/plugins/camera/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1255 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/camera/pi.py
--rw-r--r--   0 root         (0) root         (0)      648 2018-07-23 22:33:17.000000 platypush-0.9.5/platypush/plugins/clipboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/db/
--rw-r--r--   0 root         (0) root         (0)    11944 2018-07-15 21:39:10.000000 platypush-0.9.5/platypush/plugins/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1273 2018-11-02 16:48:45.000000 platypush-0.9.5/platypush/plugins/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/google/
--rw-r--r--   0 root         (0) root         (0)     1570 2018-06-25 22:36:19.000000 platypush-0.9.5/platypush/plugins/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1486 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/google/calendar.py
--rw-r--r--   0 root         (0) root         (0)     2661 2018-05-04 17:13:44.000000 platypush-0.9.5/platypush/plugins/google/credentials.py
--rw-r--r--   0 root         (0) root         (0)     3570 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/google/mail.py
--rw-r--r--   0 root         (0) root         (0)     3138 2018-07-27 23:55:18.000000 platypush-0.9.5/platypush/plugins/google/maps.py
--rw-r--r--   0 root         (0) root         (0)     2770 2018-12-15 00:18:48.000000 platypush-0.9.5/platypush/plugins/google/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/gpio/
--rw-r--r--   0 root         (0) root         (0)     3222 2018-08-22 17:20:10.000000 platypush-0.9.5/platypush/plugins/gpio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/
--rw-r--r--   0 root         (0) root         (0)      998 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/accelerometer/
--rw-r--r--   0 root         (0) root         (0)     2039 2018-09-06 00:46:30.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/accelerometer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/accelerometer/lib/
--rw-r--r--   0 root         (0) root         (0)    11346 2018-09-06 00:11:41.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/accelerometer/lib/LIS3DH.py
--rw-r--r--   0 root         (0) root         (0)        0 2018-09-06 00:23:41.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/accelerometer/lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/distance/
--rw-r--r--   0 root         (0) root         (0)     2758 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/distance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/mcp3008/
--rw-r--r--   0 root         (0) root         (0)     6074 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/gpio/sensor/mcp3008/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/gpio/zeroborg/
--rw-r--r--   0 root         (0) root         (0)     8024 2018-08-22 00:03:30.000000 platypush-0.9.5/platypush/plugins/gpio/zeroborg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/gpio/zeroborg/lib/
--rw-r--r--   0 root         (0) root         (0)    29838 2018-03-27 21:13:47.000000 platypush-0.9.5/platypush/plugins/gpio/zeroborg/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2741 2018-12-28 08:54:12.000000 platypush-0.9.5/platypush/plugins/homeseer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/http/
--rw-r--r--   0 root         (0) root         (0)        0 2018-01-06 10:36:30.000000 platypush-0.9.5/platypush/plugins/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/http/request/
--rw-r--r--   0 root         (0) root         (0)     4800 2018-07-19 18:05:08.000000 platypush-0.9.5/platypush/plugins/http/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/http/request/ota/
--rw-r--r--   0 root         (0) root         (0)        0 2018-01-12 14:19:31.000000 platypush-0.9.5/platypush/plugins/http/request/ota/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/http/request/ota/booking/
--rw-r--r--   0 root         (0) root         (0)     1178 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/http/request/ota/booking/__init__.py
--rw-r--r--   0 root         (0) root         (0)      506 2019-01-09 17:21:13.000000 platypush-0.9.5/platypush/plugins/http/request/rss.py
--rw-r--r--   0 root         (0) root         (0)     2150 2018-07-25 00:14:43.000000 platypush-0.9.5/platypush/plugins/ifttt.py
--rw-r--r--   0 root         (0) root         (0)     2076 2018-07-27 23:55:19.000000 platypush-0.9.5/platypush/plugins/kafka.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/lastfm/
--rw-r--r--   0 root         (0) root         (0)     2089 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/lastfm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/light/
--rw-r--r--   0 root         (0) root         (0)      607 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/light/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/light/hue/
--rw-r--r--   0 root         (0) root         (0)    24191 2019-01-13 19:40:34.000000 platypush-0.9.5/platypush/plugins/light/hue/__init__.py
--rw-r--r--   0 root         (0) root         (0)      960 2018-07-18 22:02:30.000000 platypush-0.9.5/platypush/plugins/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/media/
--rw-r--r--   0 root         (0) root         (0)      103 2018-04-20 14:29:56.000000 platypush-0.9.5/platypush/plugins/media/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11723 2018-11-13 22:22:53.000000 platypush-0.9.5/platypush/plugins/media/chromecast.py
--rw-r--r--   0 root         (0) root         (0)     4457 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/media/ctrl.py
--rw-r--r--   0 root         (0) root         (0)    12622 2018-11-11 17:52:29.000000 platypush-0.9.5/platypush/plugins/media/kodi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/media/lib/
--rw-r--r--   0 root         (0) root         (0)        0 2018-11-12 23:52:50.000000 platypush-0.9.5/platypush/plugins/media/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3392 2018-11-13 00:23:26.000000 platypush-0.9.5/platypush/plugins/media/lib/plexcast.py
--rw-r--r--   0 root         (0) root         (0)    12232 2018-11-13 00:28:24.000000 platypush-0.9.5/platypush/plugins/media/plex.py
--rw-r--r--   0 root         (0) root         (0)     4258 2018-12-26 22:39:47.000000 platypush-0.9.5/platypush/plugins/midi.py
--rw-r--r--   0 root         (0) root         (0)     6343 2018-11-02 16:48:45.000000 platypush-0.9.5/platypush/plugins/mqtt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/music/
--rw-r--r--   0 root         (0) root         (0)      910 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/music/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/music/mpd/
--rw-r--r--   0 root         (0) root         (0)    15292 2019-01-10 17:02:57.000000 platypush-0.9.5/platypush/plugins/music/mpd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19268 2019-01-11 18:58:43.000000 platypush-0.9.5/platypush/plugins/music/snapcast.py
--rw-r--r--   0 root         (0) root         (0)     3307 2018-12-27 00:54:31.000000 platypush-0.9.5/platypush/plugins/pushbullet.py
--rw-r--r--   0 root         (0) root         (0)     2958 2019-01-06 21:56:45.000000 platypush-0.9.5/platypush/plugins/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/serial/
--rw-r--r--   0 root         (0) root         (0)     8264 2018-12-16 22:12:07.000000 platypush-0.9.5/platypush/plugins/serial/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/shell/
--rw-r--r--   0 root         (0) root         (0)     1105 2019-01-13 18:03:29.000000 platypush-0.9.5/platypush/plugins/shell/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/sound/
--rw-r--r--   0 root         (0) root         (0)    31836 2018-12-27 23:06:23.000000 platypush-0.9.5/platypush/plugins/sound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11998 2018-12-27 23:24:14.000000 platypush-0.9.5/platypush/plugins/sound/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/switch/
--rw-r--r--   0 root         (0) root         (0)      705 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/switch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/switch/switchbot/
--rw-r--r--   0 root         (0) root         (0)     6350 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/switch/switchbot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2606 2018-05-08 13:48:22.000000 platypush-0.9.5/platypush/plugins/switch/switchbot/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2668 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/switch/tplink.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/switch/wemo/
--rw-r--r--   0 root         (0) root         (0)     3342 2019-01-11 18:58:43.000000 platypush-0.9.5/platypush/plugins/switch/wemo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9139 2018-12-19 23:55:30.000000 platypush-0.9.5/platypush/plugins/torrent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/tts/
--rw-r--r--   0 root         (0) root         (0)     1307 2018-07-15 15:28:17.000000 platypush-0.9.5/platypush/plugins/tts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3313 2018-10-14 08:45:01.000000 platypush-0.9.5/platypush/plugins/tts/google.py
--rw-r--r--   0 root         (0) root         (0)     4580 2019-01-13 18:28:02.000000 platypush-0.9.5/platypush/plugins/utils.py
--rw-r--r--   0 root         (0) root         (0)     4810 2018-10-06 21:29:41.000000 platypush-0.9.5/platypush/plugins/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/video/
--rw-r--r--   0 root         (0) root         (0)        0 2017-12-28 08:59:41.000000 platypush-0.9.5/platypush/plugins/video/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15483 2018-12-15 00:18:48.000000 platypush-0.9.5/platypush/plugins/video/omxplayer.py
--rw-r--r--   0 root         (0) root         (0)     2611 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/video/torrentcast.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/plugins/weather/
--rw-r--r--   0 root         (0) root         (0)        0 2018-05-05 22:42:46.000000 platypush-0.9.5/platypush/plugins/weather/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9721 2018-07-06 01:46:22.000000 platypush-0.9.5/platypush/plugins/weather/forecast.py
--rw-r--r--   0 root         (0) root         (0)     2531 2018-11-01 22:32:03.000000 platypush-0.9.5/platypush/plugins/websocket.py
--rw-r--r--   0 root         (0) root         (0)     1614 2018-12-01 17:35:56.000000 platypush-0.9.5/platypush/plugins/wiimote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/procedure/
--rw-r--r--   0 root         (0) root         (0)     9628 2019-01-12 17:27:51.000000 platypush-0.9.5/platypush/procedure/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/pusher/
--rw-r--r--   0 root         (0) root         (0)     7645 2018-05-30 13:59:10.000000 platypush-0.9.5/platypush/pusher/__init__.py
--rw-r--r--   0 root         (0) root         (0)       64 2018-01-04 15:09:40.000000 platypush-0.9.5/platypush/pusher/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush/utils/
--rw-r--r--   0 root         (0) root         (0)     5274 2019-01-10 22:15:35.000000 platypush-0.9.5/platypush/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6600 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    74188 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1450 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2019-01-13 19:42:18.000000 platypush-0.9.5/platypush.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2019-01-13 19:42:18.000000 platypush-0.9.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     3874 2019-01-13 19:11:23.000000 platypush-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-13 19:42:18.000000 platypush-0.9.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2018-01-04 09:37:29.000000 platypush-0.9.5/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      380 2018-01-02 18:37:08.000000 platypush-0.9.5/tests/context.py
--rw-r--r--   0 root         (0) root         (0)     1001 2018-09-26 23:44:15.000000 platypush-0.9.5/tests/test_event_parse.py
--rw-r--r--   0 root         (0) root         (0)     1906 2018-09-24 21:13:04.000000 platypush-0.9.5/tests/test_http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/
+-rw-r--r--   0 root         (0) root         (0)      103 2018-01-29 15:10:34.000000 platypush-0.9.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6845 2019-02-24 18:06:50.000000 platypush-0.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4260 2018-12-05 20:19:33.000000 platypush-0.9.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     6436 2018-12-19 23:11:36.000000 platypush-0.9.6/bin/platyvenv
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/
+-rw-r--r--   0 root         (0) root         (0)     7224 2019-02-24 18:03:49.000000 platypush-0.9.6/platypush/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2018-07-04 11:25:50.000000 platypush-0.9.6/platypush/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/
+-rw-r--r--   0 root         (0) root         (0)     9273 2019-02-22 17:24:05.000000 platypush-0.9.6/platypush/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/adafruit/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-01-11 23:18:57.000000 platypush-0.9.6/platypush/backend/adafruit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2628 2019-01-12 00:56:45.000000 platypush-0.9.6/platypush/backend/adafruit/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/assistant/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/assistant/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/assistant/google/
+-rw-r--r--   0 root         (0) root         (0)     6701 2019-02-05 10:58:51.000000 platypush-0.9.6/platypush/backend/assistant/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15640 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/assistant/google/pushtotalk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/assistant/snowboy/
+-rw-r--r--   0 root         (0) root         (0)     2373 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/assistant/snowboy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/button/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/button/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/button/flic/
+-rw-r--r--   0 root         (0) root         (0)     4048 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/button/flic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/button/flic/fliclib/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/button/flic/fliclib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24818 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/button/flic/fliclib/aioflic.py
+-rw-r--r--   0 root         (0) root         (0)    23805 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/button/flic/fliclib/fliclib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/camera/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/camera/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6740 2019-01-10 21:53:15.000000 platypush-0.9.6/platypush/backend/camera/pi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/
+-rw-r--r--   0 root         (0) root         (0)    10391 2019-02-24 14:52:47.000000 platypush-0.9.6/platypush/backend/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/app/
+-rw-r--r--   0 root         (0) root         (0)      588 2019-02-23 23:17:03.000000 platypush-0.9.6/platypush/backend/http/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/app/routes/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-02-23 17:13:44.000000 platypush-0.9.6/platypush/backend/http/app/routes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      931 2019-02-23 17:18:56.000000 platypush-0.9.6/platypush/backend/http/app/routes/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2019-02-23 17:19:05.000000 platypush-0.9.6/platypush/backend/http/app/routes/execute.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2019-02-23 17:19:13.000000 platypush-0.9.6/platypush/backend/http/app/routes/index.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2019-02-23 18:23:10.000000 platypush-0.9.6/platypush/backend/http/app/routes/map.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2019-02-23 17:18:36.000000 platypush-0.9.6/platypush/backend/http/app/routes/resources.py
+-rw-r--r--   0 root         (0) root         (0)     4389 2019-02-23 19:56:14.000000 platypush-0.9.6/platypush/backend/http/app/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/media/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-02-07 13:27:14.000000 platypush-0.9.6/platypush/backend/http/media/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/media/handlers/
+-rw-r--r--   0 root         (0) root         (0)     2221 2019-02-11 22:34:35.000000 platypush-0.9.6/platypush/backend/http/media/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2019-02-07 13:27:14.000000 platypush-0.9.6/platypush/backend/http/media/handlers/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/poll/
+-rw-r--r--   0 root         (0) root         (0)     3481 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/http/poll/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/request/
+-rw-r--r--   0 root         (0) root         (0)     3993 2019-01-13 19:38:16.000000 platypush-0.9.6/platypush/backend/http/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/request/ota/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/http/request/ota/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/request/ota/booking/
+-rw-r--r--   0 root         (0) root         (0)     1613 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/http/request/ota/booking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/request/rss/
+-rw-r--r--   0 root         (0) root         (0)     9324 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/http/request/rss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/css/
+-rw-r--r--   0 root         (0) root         (0)     4676 2019-02-10 10:08:32.000000 platypush-0.9.6/platypush/backend/http/static/css/application.css
+-rw-r--r--   0 root         (0) root         (0)        0 2018-04-17 21:10:49.000000 platypush-0.9.6/platypush/backend/http/static/css/assistant.google.css
+-rw-r--r--   0 root         (0) root         (0)      367 2018-05-05 21:56:36.000000 platypush-0.9.6/platypush/backend/http/static/css/dashboard.css
+-rw-r--r--   0 root         (0) root         (0)      573 2018-08-22 18:33:17.000000 platypush-0.9.6/platypush/backend/http/static/css/gpio.css
+-rw-r--r--   0 root         (0) root         (0)      486 2018-05-01 08:13:41.000000 platypush-0.9.6/platypush/backend/http/static/css/gpio.sensor.mcp3008.css
+-rw-r--r--   0 root         (0) root         (0)      341 2018-04-13 23:00:00.000000 platypush-0.9.6/platypush/backend/http/static/css/gpio.zeroborg.css
+-rw-r--r--   0 root         (0) root         (0)     2274 2018-06-18 22:37:33.000000 platypush-0.9.6/platypush/backend/http/static/css/light.hue.css
+-rw-r--r--   0 root         (0) root         (0)      119 2018-06-12 18:30:23.000000 platypush-0.9.6/platypush/backend/http/static/css/map.css
+-rw-r--r--   0 root         (0) root         (0)     4444 2019-02-10 23:37:06.000000 platypush-0.9.6/platypush/backend/http/static/css/media.css
+-rw-r--r--   0 root         (0) root         (0)     3470 2018-04-12 10:38:19.000000 platypush-0.9.6/platypush/backend/http/static/css/music.mpd.css
+-rw-r--r--   0 root         (0) root         (0)     3693 2019-01-08 17:23:09.000000 platypush-0.9.6/platypush/backend/http/static/css/music.snapcast.css
+-rw-r--r--   0 root         (0) root         (0)     7797 2014-12-29 18:30:41.000000 platypush-0.9.6/platypush/backend/http/static/css/normalize.css
+-rw-r--r--   0 root         (0) root         (0)      454 2018-01-28 19:40:20.000000 platypush-0.9.6/platypush/backend/http/static/css/skeleton-tabs.css
+-rw-r--r--   0 root         (0) root         (0)    11452 2014-12-29 18:30:41.000000 platypush-0.9.6/platypush/backend/http/static/css/skeleton.css
+-rw-r--r--   0 root         (0) root         (0)      612 2018-05-11 18:40:45.000000 platypush-0.9.6/platypush/backend/http/static/css/switch.switchbot.css
+-rw-r--r--   0 root         (0) root         (0)      600 2018-06-26 19:51:16.000000 platypush-0.9.6/platypush/backend/http/static/css/switch.tplink.css
+-rw-r--r--   0 root         (0) root         (0)      592 2018-05-08 07:54:04.000000 platypush-0.9.6/platypush/backend/http/static/css/switch.wemo.css
+-rw-r--r--   0 root         (0) root         (0)     5637 2018-03-27 21:13:47.000000 platypush-0.9.6/platypush/backend/http/static/css/toggles.css
+-rw-r--r--   0 root         (0) root         (0)      124 2018-04-17 07:27:41.000000 platypush-0.9.6/platypush/backend/http/static/css/tts.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/css/widgets/
+-rw-r--r--   0 root         (0) root         (0)      536 2018-06-10 15:19:50.000000 platypush-0.9.6/platypush/backend/http/static/css/widgets/calendar.css
+-rw-r--r--   0 root         (0) root         (0)      962 2018-06-23 11:26:20.000000 platypush-0.9.6/platypush/backend/http/static/css/widgets/date-time-weather.css
+-rw-r--r--   0 root         (0) root         (0)      566 2018-05-07 15:17:15.000000 platypush-0.9.6/platypush/backend/http/static/css/widgets/image-carousel.css
+-rw-r--r--   0 root         (0) root         (0)     1101 2018-08-17 23:08:57.000000 platypush-0.9.6/platypush/backend/http/static/css/widgets/music.css
+-rw-r--r--   0 root         (0) root         (0)      589 2018-05-05 21:41:52.000000 platypush-0.9.6/platypush/backend/http/static/css/widgets/rss-news.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/
+-rw-r--r--   0 root         (0) root         (0)      167 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)       77 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/.git
+-rw-r--r--   0 root         (0) root         (0)       57 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/.gitignore
+-rw-r--r--   0 root         (0) root         (0)       48 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/.prettierignore
+-rw-r--r--   0 root         (0) root         (0)      374 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/.prettierrc.json
+-rw-r--r--   0 root         (0) root         (0)       81 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)      950 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/Gruntfile.coffee
+-rw-r--r--   0 root         (0) root         (0)     1087 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2097 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/assets/
+-rw-r--r--   0 root         (0) root         (0)     2573 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/assets/docs.css
+-rw-r--r--   0 root         (0) root         (0)      430 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/assets/docs.js
+-rw-r--r--   0 root         (0) root         (0)     2616 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/assets/docs.less
+-rw-r--r--   0 root         (0) root         (0)      208 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/bower.json
+-rw-r--r--   0 root         (0) root         (0)      409 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/composer.json
+-rw-r--r--   0 root         (0) root         (0)     1002 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/convertSvgToAssetCatalog.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/css/
+-rw-r--r--   0 root         (0) root         (0)    37994 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/css/flag-icon.css
+-rw-r--r--   0 root         (0) root         (0)    33818 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/css/flag-icon.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/
+-rw-r--r--   0 root         (0) root         (0)    32679 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ad.svg
+-rw-r--r--   0 root         (0) root         (0)      262 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ae.svg
+-rw-r--r--   0 root         (0) root         (0)    21123 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/af.svg
+-rw-r--r--   0 root         (0) root         (0)      761 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ag.svg
+-rw-r--r--   0 root         (0) root         (0)    47971 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ai.svg
+-rw-r--r--   0 root         (0) root         (0)     3220 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/al.svg
+-rw-r--r--   0 root         (0) root         (0)      231 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/am.svg
+-rw-r--r--   0 root         (0) root         (0)     1601 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ao.svg
+-rw-r--r--   0 root         (0) root         (0)     3180 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/aq.svg
+-rw-r--r--   0 root         (0) root         (0)     3500 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ar.svg
+-rw-r--r--   0 root         (0) root         (0)     7838 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/as.svg
+-rw-r--r--   0 root         (0) root         (0)      242 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/at.svg
+-rw-r--r--   0 root         (0) root         (0)     1317 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/au.svg
+-rw-r--r--   0 root         (0) root         (0)    12084 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/aw.svg
+-rw-r--r--   0 root         (0) root         (0)      541 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ax.svg
+-rw-r--r--   0 root         (0) root         (0)      498 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/az.svg
+-rw-r--r--   0 root         (0) root         (0)     1242 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ba.svg
+-rw-r--r--   0 root         (0) root         (0)      613 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bb.svg
+-rw-r--r--   0 root         (0) root         (0)      192 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bd.svg
+-rw-r--r--   0 root         (0) root         (0)      290 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/be.svg
+-rw-r--r--   0 root         (0) root         (0)      383 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bf.svg
+-rw-r--r--   0 root         (0) root         (0)      294 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bg.svg
+-rw-r--r--   0 root         (0) root         (0)      569 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bh.svg
+-rw-r--r--   0 root         (0) root         (0)     1045 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bi.svg
+-rw-r--r--   0 root         (0) root         (0)      499 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bj.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bl.svg
+-rw-r--r--   0 root         (0) root         (0)    22304 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bm.svg
+-rw-r--r--   0 root         (0) root         (0)    14506 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bn.svg
+-rw-r--r--   0 root         (0) root         (0)   119582 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bo.svg
+-rw-r--r--   0 root         (0) root         (0)      228 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bq.svg
+-rw-r--r--   0 root         (0) root         (0)     7816 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/br.svg
+-rw-r--r--   0 root         (0) root         (0)      568 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bs.svg
+-rw-r--r--   0 root         (0) root         (0)    25138 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bt.svg
+-rw-r--r--   0 root         (0) root         (0)      582 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bv.svg
+-rw-r--r--   0 root         (0) root         (0)      254 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bw.svg
+-rw-r--r--   0 root         (0) root         (0)     6086 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/by.svg
+-rw-r--r--   0 root         (0) root         (0)    47095 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/bz.svg
+-rw-r--r--   0 root         (0) root         (0)      705 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ca.svg
+-rw-r--r--   0 root         (0) root         (0)     3089 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cc.svg
+-rw-r--r--   0 root         (0) root         (0)      507 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cd.svg
+-rw-r--r--   0 root         (0) root         (0)      632 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cf.svg
+-rw-r--r--   0 root         (0) root         (0)      469 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cg.svg
+-rw-r--r--   0 root         (0) root         (0)      295 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ch.svg
+-rw-r--r--   0 root         (0) root         (0)      283 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ci.svg
+-rw-r--r--   0 root         (0) root         (0)     1843 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ck.svg
+-rw-r--r--   0 root         (0) root         (0)      574 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cl.svg
+-rw-r--r--   0 root         (0) root         (0)      824 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cm.svg
+-rw-r--r--   0 root         (0) root         (0)      743 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cn.svg
+-rw-r--r--   0 root         (0) root         (0)      289 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/co.svg
+-rw-r--r--   0 root         (0) root         (0)      293 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cr.svg
+-rw-r--r--   0 root         (0) root         (0)      573 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cu.svg
+-rw-r--r--   0 root         (0) root         (0)     1357 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cv.svg
+-rw-r--r--   0 root         (0) root         (0)      682 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cw.svg
+-rw-r--r--   0 root         (0) root         (0)     2505 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cx.svg
+-rw-r--r--   0 root         (0) root         (0)     6024 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cy.svg
+-rw-r--r--   0 root         (0) root         (0)      480 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/cz.svg
+-rw-r--r--   0 root         (0) root         (0)      221 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/de.svg
+-rw-r--r--   0 root         (0) root         (0)      585 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/dj.svg
+-rw-r--r--   0 root         (0) root         (0)      235 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/dk.svg
+-rw-r--r--   0 root         (0) root         (0)    16480 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/dm.svg
+-rw-r--r--   0 root         (0) root         (0)   391693 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/do.svg
+-rw-r--r--   0 root         (0) root         (0)      309 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/dz.svg
+-rw-r--r--   0 root         (0) root         (0)    29916 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ec.svg
+-rw-r--r--   0 root         (0) root         (0)      352 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ee.svg
+-rw-r--r--   0 root         (0) root         (0)     9978 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/eg.svg
+-rw-r--r--   0 root         (0) root         (0)      823 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/eh.svg
+-rw-r--r--   0 root         (0) root         (0)     3388 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/er.svg
+-rw-r--r--   0 root         (0) root         (0)      257 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/es-ct.svg
+-rw-r--r--   0 root         (0) root         (0)    93922 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/es.svg
+-rw-r--r--   0 root         (0) root         (0)     1239 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/et.svg
+-rw-r--r--   0 root         (0) root         (0)     1250 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/eu.svg
+-rw-r--r--   0 root         (0) root         (0)      240 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/fi.svg
+-rw-r--r--   0 root         (0) root         (0)    27355 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/fj.svg
+-rw-r--r--   0 root         (0) root         (0)    30626 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/fk.svg
+-rw-r--r--   0 root         (0) root         (0)      759 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/fm.svg
+-rw-r--r--   0 root         (0) root         (0)      534 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/fo.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/fr.svg
+-rw-r--r--   0 root         (0) root         (0)      278 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ga.svg
+-rw-r--r--   0 root         (0) root         (0)      232 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gb-eng.svg
+-rw-r--r--   0 root         (0) root         (0)    25211 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gb-nir.svg
+-rw-r--r--   0 root         (0) root         (0)      239 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gb-sct.svg
+-rw-r--r--   0 root         (0) root         (0)     9076 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gb-wls.svg
+-rw-r--r--   0 root         (0) root         (0)      795 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gb.svg
+-rw-r--r--   0 root         (0) root         (0)     1831 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gd.svg
+-rw-r--r--   0 root         (0) root         (0)     1541 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ge.svg
+-rw-r--r--   0 root         (0) root         (0)      261 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gf.svg
+-rw-r--r--   0 root         (0) root         (0)      625 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gg.svg
+-rw-r--r--   0 root         (0) root         (0)      296 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gh.svg
+-rw-r--r--   0 root         (0) root         (0)     2949 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gi.svg
+-rw-r--r--   0 root         (0) root         (0)      240 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gl.svg
+-rw-r--r--   0 root         (0) root         (0)      382 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gm.svg
+-rw-r--r--   0 root         (0) root         (0)      295 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gn.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gp.svg
+-rw-r--r--   0 root         (0) root         (0)     5277 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gq.svg
+-rw-r--r--   0 root         (0) root         (0)      872 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gr.svg
+-rw-r--r--   0 root         (0) root         (0)    35105 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gs.svg
+-rw-r--r--   0 root         (0) root         (0)    37811 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gt.svg
+-rw-r--r--   0 root         (0) root         (0)     4630 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gu.svg
+-rw-r--r--   0 root         (0) root         (0)      889 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gw.svg
+-rw-r--r--   0 root         (0) root         (0)      481 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/gy.svg
+-rw-r--r--   0 root         (0) root         (0)     3554 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/hk.svg
+-rw-r--r--   0 root         (0) root         (0)     1308 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/hm.svg
+-rw-r--r--   0 root         (0) root         (0)     1116 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/hn.svg
+-rw-r--r--   0 root         (0) root         (0)    41785 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/hr.svg
+-rw-r--r--   0 root         (0) root         (0)    15301 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ht.svg
+-rw-r--r--   0 root         (0) root         (0)      276 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/hu.svg
+-rw-r--r--   0 root         (0) root         (0)      239 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/id.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ie.svg
+-rw-r--r--   0 root         (0) root         (0)      848 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/il.svg
+-rw-r--r--   0 root         (0) root         (0)    10253 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/im.svg
+-rw-r--r--   0 root         (0) root         (0)     1088 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/in.svg
+-rw-r--r--   0 root         (0) root         (0)    27465 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/io.svg
+-rw-r--r--   0 root         (0) root         (0)     1481 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/iq.svg
+-rw-r--r--   0 root         (0) root         (0)    15360 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ir.svg
+-rw-r--r--   0 root         (0) root         (0)      526 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/is.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/it.svg
+-rw-r--r--   0 root         (0) root         (0)     4699 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/je.svg
+-rw-r--r--   0 root         (0) root         (0)      389 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/jm.svg
+-rw-r--r--   0 root         (0) root         (0)      691 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/jo.svg
+-rw-r--r--   0 root         (0) root         (0)      497 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/jp.svg
+-rw-r--r--   0 root         (0) root         (0)     1492 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ke.svg
+-rw-r--r--   0 root         (0) root         (0)     3334 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/kg.svg
+-rw-r--r--   0 root         (0) root         (0)     7283 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/kh.svg
+-rw-r--r--   0 root         (0) root         (0)     5950 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ki.svg
+-rw-r--r--   0 root         (0) root         (0)     1041 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/km.svg
+-rw-r--r--   0 root         (0) root         (0)      817 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/kn.svg
+-rw-r--r--   0 root         (0) root         (0)      852 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/kp.svg
+-rw-r--r--   0 root         (0) root         (0)     1725 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/kr.svg
+-rw-r--r--   0 root         (0) root         (0)      507 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/kw.svg
+-rw-r--r--   0 root         (0) root         (0)    22455 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ky.svg
+-rw-r--r--   0 root         (0) root         (0)    11422 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/kz.svg
+-rw-r--r--   0 root         (0) root         (0)      504 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/la.svg
+-rw-r--r--   0 root         (0) root         (0)     2750 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/lb.svg
+-rw-r--r--   0 root         (0) root         (0)      370 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/lc.svg
+-rw-r--r--   0 root         (0) root         (0)     8341 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/li.svg
+-rw-r--r--   0 root         (0) root         (0)    11338 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/lk.svg
+-rw-r--r--   0 root         (0) root         (0)      694 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/lr.svg
+-rw-r--r--   0 root         (0) root         (0)     1242 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ls.svg
+-rw-r--r--   0 root         (0) root         (0)      442 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/lt.svg
+-rw-r--r--   0 root         (0) root         (0)      232 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/lu.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/lv.svg
+-rw-r--r--   0 root         (0) root         (0)      530 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ly.svg
+-rw-r--r--   0 root         (0) root         (0)      250 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ma.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mc.svg
+-rw-r--r--   0 root         (0) root         (0)    11368 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/md.svg
+-rw-r--r--   0 root         (0) root         (0)    63990 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/me.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mf.svg
+-rw-r--r--   0 root         (0) root         (0)      302 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mg.svg
+-rw-r--r--   0 root         (0) root         (0)      763 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mh.svg
+-rw-r--r--   0 root         (0) root         (0)      410 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mk.svg
+-rw-r--r--   0 root         (0) root         (0)      279 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ml.svg
+-rw-r--r--   0 root         (0) root         (0)      865 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mm.svg
+-rw-r--r--   0 root         (0) root         (0)     1259 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mn.svg
+-rw-r--r--   0 root         (0) root         (0)     1547 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mo.svg
+-rw-r--r--   0 root         (0) root         (0)    23656 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mp.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mq.svg
+-rw-r--r--   0 root         (0) root         (0)      435 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mr.svg
+-rw-r--r--   0 root         (0) root         (0)     6693 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ms.svg
+-rw-r--r--   0 root         (0) root         (0)    10513 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mt.svg
+-rw-r--r--   0 root         (0) root         (0)      319 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mu.svg
+-rw-r--r--   0 root         (0) root         (0)      307 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mv.svg
+-rw-r--r--   0 root         (0) root         (0)     3891 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mw.svg
+-rw-r--r--   0 root         (0) root         (0)    91037 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mx.svg
+-rw-r--r--   0 root         (0) root         (0)     1271 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/my.svg
+-rw-r--r--   0 root         (0) root         (0)     2601 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/mz.svg
+-rw-r--r--   0 root         (0) root         (0)      980 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/na.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/nc.svg
+-rw-r--r--   0 root         (0) root         (0)      282 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ne.svg
+-rw-r--r--   0 root         (0) root         (0)     5595 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/nf.svg
+-rw-r--r--   0 root         (0) root         (0)      260 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ng.svg
+-rw-r--r--   0 root         (0) root         (0)    18632 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ni.svg
+-rw-r--r--   0 root         (0) root         (0)      372 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/nl.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/no.svg
+-rw-r--r--   0 root         (0) root         (0)     1196 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/np.svg
+-rw-r--r--   0 root         (0) root         (0)      668 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/nr.svg
+-rw-r--r--   0 root         (0) root         (0)     1730 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/nu.svg
+-rw-r--r--   0 root         (0) root         (0)     2999 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/nz.svg
+-rw-r--r--   0 root         (0) root         (0)    22825 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/om.svg
+-rw-r--r--   0 root         (0) root         (0)      659 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pa.svg
+-rw-r--r--   0 root         (0) root         (0)    73524 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pe.svg
+-rw-r--r--   0 root         (0) root         (0)     4230 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pf.svg
+-rw-r--r--   0 root         (0) root         (0)     2099 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pg.svg
+-rw-r--r--   0 root         (0) root         (0)     1522 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ph.svg
+-rw-r--r--   0 root         (0) root         (0)      691 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pk.svg
+-rw-r--r--   0 root         (0) root         (0)      222 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pl.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pm.svg
+-rw-r--r--   0 root         (0) root         (0)     8592 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pn.svg
+-rw-r--r--   0 root         (0) root         (0)      619 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pr.svg
+-rw-r--r--   0 root         (0) root         (0)      541 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ps.svg
+-rw-r--r--   0 root         (0) root         (0)     8748 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pt.svg
+-rw-r--r--   0 root         (0) root         (0)      509 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/pw.svg
+-rw-r--r--   0 root         (0) root         (0)    17460 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/py.svg
+-rw-r--r--   0 root         (0) root         (0)      356 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/qa.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/re.svg
+-rw-r--r--   0 root         (0) root         (0)      305 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ro.svg
+-rw-r--r--   0 root         (0) root         (0)   187500 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/rs.svg
+-rw-r--r--   0 root         (0) root         (0)      290 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ru.svg
+-rw-r--r--   0 root         (0) root         (0)      748 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/rw.svg
+-rw-r--r--   0 root         (0) root         (0)    10225 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sa.svg
+-rw-r--r--   0 root         (0) root         (0)      952 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sb.svg
+-rw-r--r--   0 root         (0) root         (0)      570 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sc.svg
+-rw-r--r--   0 root         (0) root         (0)      493 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sd.svg
+-rw-r--r--   0 root         (0) root         (0)      698 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/se.svg
+-rw-r--r--   0 root         (0) root         (0)      951 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sg.svg
+-rw-r--r--   0 root         (0) root         (0)    30261 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sh.svg
+-rw-r--r--   0 root         (0) root         (0)     2065 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/si.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sj.svg
+-rw-r--r--   0 root         (0) root         (0)     1178 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sk.svg
+-rw-r--r--   0 root         (0) root         (0)      438 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sl.svg
+-rw-r--r--   0 root         (0) root         (0)    15876 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sm.svg
+-rw-r--r--   0 root         (0) root         (0)      414 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sn.svg
+-rw-r--r--   0 root         (0) root         (0)      498 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/so.svg
+-rw-r--r--   0 root         (0) root         (0)      320 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sr.svg
+-rw-r--r--   0 root         (0) root         (0)      397 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ss.svg
+-rw-r--r--   0 root         (0) root         (0)      920 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/st.svg
+-rw-r--r--   0 root         (0) root         (0)    84167 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sv.svg
+-rw-r--r--   0 root         (0) root         (0)    13097 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sx.svg
+-rw-r--r--   0 root         (0) root         (0)      579 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sy.svg
+-rw-r--r--   0 root         (0) root         (0)     6700 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/sz.svg
+-rw-r--r--   0 root         (0) root         (0)    14766 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tc.svg
+-rw-r--r--   0 root         (0) root         (0)      279 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/td.svg
+-rw-r--r--   0 root         (0) root         (0)     1196 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tf.svg
+-rw-r--r--   0 root         (0) root         (0)      733 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tg.svg
+-rw-r--r--   0 root         (0) root         (0)      288 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/th.svg
+-rw-r--r--   0 root         (0) root         (0)     1785 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tj.svg
+-rw-r--r--   0 root         (0) root         (0)      778 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tk.svg
+-rw-r--r--   0 root         (0) root         (0)      577 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tl.svg
+-rw-r--r--   0 root         (0) root         (0)    31846 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tm.svg
+-rw-r--r--   0 root         (0) root         (0)      740 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tn.svg
+-rw-r--r--   0 root         (0) root         (0)      361 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/to.svg
+-rw-r--r--   0 root         (0) root         (0)      575 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tr.svg
+-rw-r--r--   0 root         (0) root         (0)      320 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tt.svg
+-rw-r--r--   0 root         (0) root         (0)     2163 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tv.svg
+-rw-r--r--   0 root         (0) root         (0)      957 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tw.svg
+-rw-r--r--   0 root         (0) root         (0)      602 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/tz.svg
+-rw-r--r--   0 root         (0) root         (0)      238 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ua.svg
+-rw-r--r--   0 root         (0) root         (0)     4034 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ug.svg
+-rw-r--r--   0 root         (0) root         (0)     3972 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/um.svg
+-rw-r--r--   0 root         (0) root         (0)    20456 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/un.svg
+-rw-r--r--   0 root         (0) root         (0)     3921 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/us.svg
+-rw-r--r--   0 root         (0) root         (0)     1715 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/uy.svg
+-rw-r--r--   0 root         (0) root         (0)     1454 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/uz.svg
+-rw-r--r--   0 root         (0) root         (0)    90846 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/va.svg
+-rw-r--r--   0 root         (0) root         (0)      498 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/vc.svg
+-rw-r--r--   0 root         (0) root         (0)     1188 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ve.svg
+-rw-r--r--   0 root         (0) root         (0)    24993 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/vg.svg
+-rw-r--r--   0 root         (0) root         (0)     8711 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/vi.svg
+-rw-r--r--   0 root         (0) root         (0)      498 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/vn.svg
+-rw-r--r--   0 root         (0) root         (0)     3735 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/vu.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/wf.svg
+-rw-r--r--   0 root         (0) root         (0)      706 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ws.svg
+-rw-r--r--   0 root         (0) root         (0)     9003 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/xk.svg
+-rw-r--r--   0 root         (0) root         (0)      275 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/ye.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/yt.svg
+-rw-r--r--   0 root         (0) root         (0)      872 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/za.svg
+-rw-r--r--   0 root         (0) root         (0)     5419 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/zm.svg
+-rw-r--r--   0 root         (0) root         (0)     6759 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/1x1/zw.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/
+-rw-r--r--   0 root         (0) root         (0)    33893 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ad.svg
+-rw-r--r--   0 root         (0) root         (0)      254 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ae.svg
+-rw-r--r--   0 root         (0) root         (0)    21257 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/af.svg
+-rw-r--r--   0 root         (0) root         (0)      743 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ag.svg
+-rw-r--r--   0 root         (0) root         (0)    42204 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ai.svg
+-rw-r--r--   0 root         (0) root         (0)     3218 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/al.svg
+-rw-r--r--   0 root         (0) root         (0)      223 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/am.svg
+-rw-r--r--   0 root         (0) root         (0)     1601 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ao.svg
+-rw-r--r--   0 root         (0) root         (0)     2969 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/aq.svg
+-rw-r--r--   0 root         (0) root         (0)     3427 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ar.svg
+-rw-r--r--   0 root         (0) root         (0)     8082 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/as.svg
+-rw-r--r--   0 root         (0) root         (0)      240 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/at.svg
+-rw-r--r--   0 root         (0) root         (0)     1330 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/au.svg
+-rw-r--r--   0 root         (0) root         (0)     9945 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/aw.svg
+-rw-r--r--   0 root         (0) root         (0)      553 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ax.svg
+-rw-r--r--   0 root         (0) root         (0)      512 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/az.svg
+-rw-r--r--   0 root         (0) root         (0)     1304 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ba.svg
+-rw-r--r--   0 root         (0) root         (0)      610 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bb.svg
+-rw-r--r--   0 root         (0) root         (0)      190 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bd.svg
+-rw-r--r--   0 root         (0) root         (0)      290 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/be.svg
+-rw-r--r--   0 root         (0) root         (0)      357 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bf.svg
+-rw-r--r--   0 root         (0) root         (0)      286 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bg.svg
+-rw-r--r--   0 root         (0) root         (0)      543 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bh.svg
+-rw-r--r--   0 root         (0) root         (0)     1071 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bi.svg
+-rw-r--r--   0 root         (0) root         (0)      496 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bj.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bl.svg
+-rw-r--r--   0 root         (0) root         (0)    22617 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bm.svg
+-rw-r--r--   0 root         (0) root         (0)    14367 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bn.svg
+-rw-r--r--   0 root         (0) root         (0)   117922 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bo.svg
+-rw-r--r--   0 root         (0) root         (0)      224 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bq.svg
+-rw-r--r--   0 root         (0) root         (0)     8231 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/br.svg
+-rw-r--r--   0 root         (0) root         (0)      546 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bs.svg
+-rw-r--r--   0 root         (0) root         (0)    25318 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bt.svg
+-rw-r--r--   0 root         (0) root         (0)      579 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bv.svg
+-rw-r--r--   0 root         (0) root         (0)      252 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bw.svg
+-rw-r--r--   0 root         (0) root         (0)     5956 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/by.svg
+-rw-r--r--   0 root         (0) root         (0)    46832 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/bz.svg
+-rw-r--r--   0 root         (0) root         (0)      725 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ca.svg
+-rw-r--r--   0 root         (0) root         (0)     3135 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cc.svg
+-rw-r--r--   0 root         (0) root         (0)      349 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cd.svg
+-rw-r--r--   0 root         (0) root         (0)      685 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cf.svg
+-rw-r--r--   0 root         (0) root         (0)      481 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cg.svg
+-rw-r--r--   0 root         (0) root         (0)      297 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ch.svg
+-rw-r--r--   0 root         (0) root         (0)      280 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ci.svg
+-rw-r--r--   0 root         (0) root         (0)     1884 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ck.svg
+-rw-r--r--   0 root         (0) root         (0)      557 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cl.svg
+-rw-r--r--   0 root         (0) root         (0)      824 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cm.svg
+-rw-r--r--   0 root         (0) root         (0)      801 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cn.svg
+-rw-r--r--   0 root         (0) root         (0)      289 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/co.svg
+-rw-r--r--   0 root         (0) root         (0)      293 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cr.svg
+-rw-r--r--   0 root         (0) root         (0)      616 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cu.svg
+-rw-r--r--   0 root         (0) root         (0)     1409 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cv.svg
+-rw-r--r--   0 root         (0) root         (0)      675 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cw.svg
+-rw-r--r--   0 root         (0) root         (0)     2466 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cx.svg
+-rw-r--r--   0 root         (0) root         (0)     5930 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cy.svg
+-rw-r--r--   0 root         (0) root         (0)      478 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/cz.svg
+-rw-r--r--   0 root         (0) root         (0)      213 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/de.svg
+-rw-r--r--   0 root         (0) root         (0)      585 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/dj.svg
+-rw-r--r--   0 root         (0) root         (0)      239 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/dk.svg
+-rw-r--r--   0 root         (0) root         (0)    15992 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/dm.svg
+-rw-r--r--   0 root         (0) root         (0)   394127 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/do.svg
+-rw-r--r--   0 root         (0) root         (0)      298 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/dz.svg
+-rw-r--r--   0 root         (0) root         (0)    29359 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ec.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ee.svg
+-rw-r--r--   0 root         (0) root         (0)     9964 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/eg.svg
+-rw-r--r--   0 root         (0) root         (0)      873 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/eh.svg
+-rw-r--r--   0 root         (0) root         (0)     3202 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/er.svg
+-rw-r--r--   0 root         (0) root         (0)      258 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/es-ct.svg
+-rw-r--r--   0 root         (0) root         (0)    92061 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/es.svg
+-rw-r--r--   0 root         (0) root         (0)     1240 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/et.svg
+-rw-r--r--   0 root         (0) root         (0)     1249 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/eu.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/fi.svg
+-rw-r--r--   0 root         (0) root         (0)    27208 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/fj.svg
+-rw-r--r--   0 root         (0) root         (0)    30431 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/fk.svg
+-rw-r--r--   0 root         (0) root         (0)      770 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/fm.svg
+-rw-r--r--   0 root         (0) root         (0)      564 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/fo.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/fr.svg
+-rw-r--r--   0 root         (0) root         (0)      274 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ga.svg
+-rw-r--r--   0 root         (0) root         (0)      242 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gb-eng.svg
+-rw-r--r--   0 root         (0) root         (0)    23686 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gb-nir.svg
+-rw-r--r--   0 root         (0) root         (0)      231 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gb-sct.svg
+-rw-r--r--   0 root         (0) root         (0)     9183 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gb-wls.svg
+-rw-r--r--   0 root         (0) root         (0)      837 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gb.svg
+-rw-r--r--   0 root         (0) root         (0)     1687 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gd.svg
+-rw-r--r--   0 root         (0) root         (0)     1397 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ge.svg
+-rw-r--r--   0 root         (0) root         (0)      258 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gf.svg
+-rw-r--r--   0 root         (0) root         (0)      595 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gg.svg
+-rw-r--r--   0 root         (0) root         (0)      281 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gh.svg
+-rw-r--r--   0 root         (0) root         (0)     2957 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gi.svg
+-rw-r--r--   0 root         (0) root         (0)      226 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gl.svg
+-rw-r--r--   0 root         (0) root         (0)      540 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gm.svg
+-rw-r--r--   0 root         (0) root         (0)      295 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gn.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gp.svg
+-rw-r--r--   0 root         (0) root         (0)     5185 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gq.svg
+-rw-r--r--   0 root         (0) root         (0)      815 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gr.svg
+-rw-r--r--   0 root         (0) root         (0)    34612 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gs.svg
+-rw-r--r--   0 root         (0) root         (0)    37811 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gt.svg
+-rw-r--r--   0 root         (0) root         (0)     4854 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gu.svg
+-rw-r--r--   0 root         (0) root         (0)      813 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gw.svg
+-rw-r--r--   0 root         (0) root         (0)      488 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/gy.svg
+-rw-r--r--   0 root         (0) root         (0)     3503 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/hk.svg
+-rw-r--r--   0 root         (0) root         (0)     1324 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/hm.svg
+-rw-r--r--   0 root         (0) root         (0)     1112 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/hn.svg
+-rw-r--r--   0 root         (0) root         (0)    41588 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/hr.svg
+-rw-r--r--   0 root         (0) root         (0)    15215 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ht.svg
+-rw-r--r--   0 root         (0) root         (0)      274 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/hu.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/id.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ie.svg
+-rw-r--r--   0 root         (0) root         (0)      895 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/il.svg
+-rw-r--r--   0 root         (0) root         (0)     9925 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/im.svg
+-rw-r--r--   0 root         (0) root         (0)     1074 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/in.svg
+-rw-r--r--   0 root         (0) root         (0)    27443 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/io.svg
+-rw-r--r--   0 root         (0) root         (0)     1476 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/iq.svg
+-rw-r--r--   0 root         (0) root         (0)    15448 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ir.svg
+-rw-r--r--   0 root         (0) root         (0)      518 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/is.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/it.svg
+-rw-r--r--   0 root         (0) root         (0)     4718 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/je.svg
+-rw-r--r--   0 root         (0) root         (0)      389 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/jm.svg
+-rw-r--r--   0 root         (0) root         (0)      714 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/jo.svg
+-rw-r--r--   0 root         (0) root         (0)      481 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/jp.svg
+-rw-r--r--   0 root         (0) root         (0)     1380 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ke.svg
+-rw-r--r--   0 root         (0) root         (0)     3383 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/kg.svg
+-rw-r--r--   0 root         (0) root         (0)     7282 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/kh.svg
+-rw-r--r--   0 root         (0) root         (0)     5815 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ki.svg
+-rw-r--r--   0 root         (0) root         (0)     1058 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/km.svg
+-rw-r--r--   0 root         (0) root         (0)      813 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/kn.svg
+-rw-r--r--   0 root         (0) root         (0)      789 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/kp.svg
+-rw-r--r--   0 root         (0) root         (0)     1819 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/kr.svg
+-rw-r--r--   0 root         (0) root         (0)      503 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/kw.svg
+-rw-r--r--   0 root         (0) root         (0)    21834 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ky.svg
+-rw-r--r--   0 root         (0) root         (0)    11334 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/kz.svg
+-rw-r--r--   0 root         (0) root         (0)      454 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/la.svg
+-rw-r--r--   0 root         (0) root         (0)     2811 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/lb.svg
+-rw-r--r--   0 root         (0) root         (0)      370 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/lc.svg
+-rw-r--r--   0 root         (0) root         (0)     8318 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/li.svg
+-rw-r--r--   0 root         (0) root         (0)    11326 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/lk.svg
+-rw-r--r--   0 root         (0) root         (0)      721 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/lr.svg
+-rw-r--r--   0 root         (0) root         (0)     1219 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ls.svg
+-rw-r--r--   0 root         (0) root         (0)      442 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/lt.svg
+-rw-r--r--   0 root         (0) root         (0)      228 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/lu.svg
+-rw-r--r--   0 root         (0) root         (0)      233 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/lv.svg
+-rw-r--r--   0 root         (0) root         (0)      531 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ly.svg
+-rw-r--r--   0 root         (0) root         (0)      250 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ma.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mc.svg
+-rw-r--r--   0 root         (0) root         (0)    11264 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/md.svg
+-rw-r--r--   0 root         (0) root         (0)    62977 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/me.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mf.svg
+-rw-r--r--   0 root         (0) root         (0)      302 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mg.svg
+-rw-r--r--   0 root         (0) root         (0)      741 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mh.svg
+-rw-r--r--   0 root         (0) root         (0)      382 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mk.svg
+-rw-r--r--   0 root         (0) root         (0)      276 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ml.svg
+-rw-r--r--   0 root         (0) root         (0)      848 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mm.svg
+-rw-r--r--   0 root         (0) root         (0)     1253 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mn.svg
+-rw-r--r--   0 root         (0) root         (0)     1511 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mo.svg
+-rw-r--r--   0 root         (0) root         (0)    23415 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mp.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mq.svg
+-rw-r--r--   0 root         (0) root         (0)      447 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mr.svg
+-rw-r--r--   0 root         (0) root         (0)     6785 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ms.svg
+-rw-r--r--   0 root         (0) root         (0)     8803 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mt.svg
+-rw-r--r--   0 root         (0) root         (0)      319 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mu.svg
+-rw-r--r--   0 root         (0) root         (0)      289 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mv.svg
+-rw-r--r--   0 root         (0) root         (0)     3708 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mw.svg
+-rw-r--r--   0 root         (0) root         (0)    95527 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mx.svg
+-rw-r--r--   0 root         (0) root         (0)     1279 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/my.svg
+-rw-r--r--   0 root         (0) root         (0)     2618 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/mz.svg
+-rw-r--r--   0 root         (0) root         (0)     1002 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/na.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/nc.svg
+-rw-r--r--   0 root         (0) root         (0)      276 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ne.svg
+-rw-r--r--   0 root         (0) root         (0)     5842 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/nf.svg
+-rw-r--r--   0 root         (0) root         (0)      260 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ng.svg
+-rw-r--r--   0 root         (0) root         (0)    18572 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ni.svg
+-rw-r--r--   0 root         (0) root         (0)      364 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/nl.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/no.svg
+-rw-r--r--   0 root         (0) root         (0)     1058 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/np.svg
+-rw-r--r--   0 root         (0) root         (0)      645 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/nr.svg
+-rw-r--r--   0 root         (0) root         (0)     1742 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/nu.svg
+-rw-r--r--   0 root         (0) root         (0)     2974 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/nz.svg
+-rw-r--r--   0 root         (0) root         (0)    22841 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/om.svg
+-rw-r--r--   0 root         (0) root         (0)      743 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pa.svg
+-rw-r--r--   0 root         (0) root         (0)    74209 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pe.svg
+-rw-r--r--   0 root         (0) root         (0)     4288 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pf.svg
+-rw-r--r--   0 root         (0) root         (0)     1667 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pg.svg
+-rw-r--r--   0 root         (0) root         (0)     1578 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ph.svg
+-rw-r--r--   0 root         (0) root         (0)      740 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pk.svg
+-rw-r--r--   0 root         (0) root         (0)      222 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pl.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pm.svg
+-rw-r--r--   0 root         (0) root         (0)    10939 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pn.svg
+-rw-r--r--   0 root         (0) root         (0)      631 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pr.svg
+-rw-r--r--   0 root         (0) root         (0)      555 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ps.svg
+-rw-r--r--   0 root         (0) root         (0)     8369 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pt.svg
+-rw-r--r--   0 root         (0) root         (0)      464 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/pw.svg
+-rw-r--r--   0 root         (0) root         (0)    17301 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/py.svg
+-rw-r--r--   0 root         (0) root         (0)      359 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/qa.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/re.svg
+-rw-r--r--   0 root         (0) root         (0)      305 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ro.svg
+-rw-r--r--   0 root         (0) root         (0)   187637 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/rs.svg
+-rw-r--r--   0 root         (0) root         (0)      286 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ru.svg
+-rw-r--r--   0 root         (0) root         (0)      747 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/rw.svg
+-rw-r--r--   0 root         (0) root         (0)    10290 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sa.svg
+-rw-r--r--   0 root         (0) root         (0)      947 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sb.svg
+-rw-r--r--   0 root         (0) root         (0)      565 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sc.svg
+-rw-r--r--   0 root         (0) root         (0)      491 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sd.svg
+-rw-r--r--   0 root         (0) root         (0)      685 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/se.svg
+-rw-r--r--   0 root         (0) root         (0)      886 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sg.svg
+-rw-r--r--   0 root         (0) root         (0)    29664 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sh.svg
+-rw-r--r--   0 root         (0) root         (0)     2049 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/si.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sj.svg
+-rw-r--r--   0 root         (0) root         (0)     1203 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sk.svg
+-rw-r--r--   0 root         (0) root         (0)      275 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sl.svg
+-rw-r--r--   0 root         (0) root         (0)    15947 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sm.svg
+-rw-r--r--   0 root         (0) root         (0)      424 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sn.svg
+-rw-r--r--   0 root         (0) root         (0)      491 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/so.svg
+-rw-r--r--   0 root         (0) root         (0)      315 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sr.svg
+-rw-r--r--   0 root         (0) root         (0)      386 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ss.svg
+-rw-r--r--   0 root         (0) root         (0)      916 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/st.svg
+-rw-r--r--   0 root         (0) root         (0)    83639 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sv.svg
+-rw-r--r--   0 root         (0) root         (0)    13294 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sx.svg
+-rw-r--r--   0 root         (0) root         (0)      565 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sy.svg
+-rw-r--r--   0 root         (0) root         (0)     6747 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/sz.svg
+-rw-r--r--   0 root         (0) root         (0)    14507 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tc.svg
+-rw-r--r--   0 root         (0) root         (0)      267 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/td.svg
+-rw-r--r--   0 root         (0) root         (0)     1088 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tf.svg
+-rw-r--r--   0 root         (0) root         (0)      722 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tg.svg
+-rw-r--r--   0 root         (0) root         (0)      287 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/th.svg
+-rw-r--r--   0 root         (0) root         (0)     1828 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tj.svg
+-rw-r--r--   0 root         (0) root         (0)      788 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tk.svg
+-rw-r--r--   0 root         (0) root         (0)      597 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tl.svg
+-rw-r--r--   0 root         (0) root         (0)    32561 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tm.svg
+-rw-r--r--   0 root         (0) root         (0)      750 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tn.svg
+-rw-r--r--   0 root         (0) root         (0)      355 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/to.svg
+-rw-r--r--   0 root         (0) root         (0)      554 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tr.svg
+-rw-r--r--   0 root         (0) root         (0)      315 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tt.svg
+-rw-r--r--   0 root         (0) root         (0)     2296 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tv.svg
+-rw-r--r--   0 root         (0) root         (0)      942 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tw.svg
+-rw-r--r--   0 root         (0) root         (0)      543 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/tz.svg
+-rw-r--r--   0 root         (0) root         (0)      238 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ua.svg
+-rw-r--r--   0 root         (0) root         (0)     3953 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ug.svg
+-rw-r--r--   0 root         (0) root         (0)     4517 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/um.svg
+-rw-r--r--   0 root         (0) root         (0)    20221 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/un.svg
+-rw-r--r--   0 root         (0) root         (0)     4461 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/us.svg
+-rw-r--r--   0 root         (0) root         (0)     1718 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/uy.svg
+-rw-r--r--   0 root         (0) root         (0)     1454 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/uz.svg
+-rw-r--r--   0 root         (0) root         (0)    91211 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/va.svg
+-rw-r--r--   0 root         (0) root         (0)      451 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/vc.svg
+-rw-r--r--   0 root         (0) root         (0)     1168 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ve.svg
+-rw-r--r--   0 root         (0) root         (0)    24793 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/vg.svg
+-rw-r--r--   0 root         (0) root         (0)     8757 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/vi.svg
+-rw-r--r--   0 root         (0) root         (0)      488 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/vn.svg
+-rw-r--r--   0 root         (0) root         (0)     3768 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/vu.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/wf.svg
+-rw-r--r--   0 root         (0) root         (0)      693 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ws.svg
+-rw-r--r--   0 root         (0) root         (0)     9679 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/xk.svg
+-rw-r--r--   0 root         (0) root         (0)      275 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/ye.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/yt.svg
+-rw-r--r--   0 root         (0) root         (0)      853 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/za.svg
+-rw-r--r--   0 root         (0) root         (0)     5503 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/zm.svg
+-rw-r--r--   0 root         (0) root         (0)     6780 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/flags/4x3/zw.svg
+-rw-r--r--   0 root         (0) root         (0)    59551 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/less/
+-rw-r--r--   0 root         (0) root         (0)      605 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/less/flag-icon-base.less
+-rw-r--r--   0 root         (0) root         (0)     3984 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/less/flag-icon-list.less
+-rw-r--r--   0 root         (0) root         (0)      147 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/less/flag-icon-more.less
+-rw-r--r--   0 root         (0) root         (0)       99 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/less/flag-icon.less
+-rw-r--r--   0 root         (0) root         (0)       95 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/less/variables.less
+-rw-r--r--   0 root         (0) root         (0)     1218 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/sass/
+-rw-r--r--   0 root         (0) root         (0)      616 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/sass/_flag-icon-base.scss
+-rw-r--r--   0 root         (0) root         (0)     6831 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/sass/_flag-icon-list.scss
+-rw-r--r--   0 root         (0) root         (0)      122 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/sass/_variables.scss
+-rw-r--r--   0 root         (0) root         (0)       73 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/sass/flag-icon.scss
+-rw-r--r--   0 root         (0) root         (0)      328 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/svgo.yaml
+-rw-r--r--   0 root         (0) root         (0)   131390 2019-02-10 01:19:44.000000 platypush-0.9.6/platypush/backend/http/static/flag-icons/yarn.lock
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/
+-rw-r--r--   0 root         (0) root         (0)       79 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/.git
+-rw-r--r--   0 root         (0) root         (0)      301 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      427 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/.npmignore
+-rw-r--r--   0 root         (0) root         (0)     5271 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)      173 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/Gemfile
+-rw-r--r--   0 root         (0) root         (0)     1383 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/Gemfile.lock
+-rw-r--r--   0 root         (0) root         (0)      323 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/HELP-US-OUT.txt
+-rw-r--r--   0 root         (0) root         (0)     5345 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/README.md
+-rw-r--r--   0 root         (0) root         (0)     1643 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/_config.yml
+-rw-r--r--   0 root         (0) root         (0)      403 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/bower.json
+-rw-r--r--   0 root         (0) root         (0)      499 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/component.json
+-rw-r--r--   0 root         (0) root         (0)      610 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/composer.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/css/
+-rw-r--r--   0 root         (0) root         (0)    37414 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/css/font-awesome.css
+-rw-r--r--   0 root         (0) root         (0)    21778 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/css/font-awesome.css.map
+-rw-r--r--   0 root         (0) root         (0)    31000 2018-01-28 22:51:53.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/
+-rw-r--r--   0 root         (0) root         (0)   134808 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 root         (0) root         (0)   165742 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/
+-rw-r--r--   0 root         (0) root         (0)      713 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/animated.less
+-rw-r--r--   0 root         (0) root         (0)      585 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/bordered-pulled.less
+-rw-r--r--   0 root         (0) root         (0)      452 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/core.less
+-rw-r--r--   0 root         (0) root         (0)      119 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/fixed-width.less
+-rw-r--r--   0 root         (0) root         (0)      495 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/font-awesome.less
+-rw-r--r--   0 root         (0) root         (0)    49712 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/icons.less
+-rw-r--r--   0 root         (0) root         (0)      370 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/larger.less
+-rw-r--r--   0 root         (0) root         (0)      377 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/list.less
+-rw-r--r--   0 root         (0) root         (0)     1603 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/mixins.less
+-rw-r--r--   0 root         (0) root         (0)      771 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/path.less
+-rw-r--r--   0 root         (0) root         (0)      622 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/rotated-flipped.less
+-rw-r--r--   0 root         (0) root         (0)      118 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/screen-reader.less
+-rw-r--r--   0 root         (0) root         (0)      476 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/stacked.less
+-rw-r--r--   0 root         (0) root         (0)    22563 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/less/variables.less
+-rw-r--r--   0 root         (0) root         (0)     1040 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/
+-rw-r--r--   0 root         (0) root         (0)      715 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_animated.scss
+-rw-r--r--   0 root         (0) root         (0)      592 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_bordered-pulled.scss
+-rw-r--r--   0 root         (0) root         (0)      459 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_core.scss
+-rw-r--r--   0 root         (0) root         (0)      120 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_fixed-width.scss
+-rw-r--r--   0 root         (0) root         (0)    50498 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_icons.scss
+-rw-r--r--   0 root         (0) root         (0)      375 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_larger.scss
+-rw-r--r--   0 root         (0) root         (0)      378 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_list.scss
+-rw-r--r--   0 root         (0) root         (0)     1637 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_mixins.scss
+-rw-r--r--   0 root         (0) root         (0)      783 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_path.scss
+-rw-r--r--   0 root         (0) root         (0)      672 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_rotated-flipped.scss
+-rw-r--r--   0 root         (0) root         (0)      134 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_screen-reader.scss
+-rw-r--r--   0 root         (0) root         (0)      482 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_stacked.scss
+-rw-r--r--   0 root         (0) root         (0)    22644 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_variables.scss
+-rw-r--r--   0 root         (0) root         (0)      430 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/font-awesome.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/
+-rw-r--r--   0 root         (0) root         (0)       14 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/CNAME
+-rw-r--r--   0 root         (0) root         (0)     1101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/
+-rw-r--r--   0 root         (0) root         (0)      815 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/prettify.css
+-rw-r--r--   0 root         (0) root         (0)     3063 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/pygments.css
+-rw-r--r--   0 root         (0) root         (0)   165597 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/site.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/
+-rw-r--r--   0 root         (0) root         (0)    41311 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome-ie7.css
+-rw-r--r--   0 root         (0) root         (0)    37782 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome-ie7.min.css
+-rw-r--r--   0 root         (0) root         (0)    27232 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome.css
+-rw-r--r--   0 root         (0) root         (0)    22084 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/
+-rw-r--r--   0 root         (0) root         (0)    61896 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/FontAwesome.otf
+-rw-r--r--   0 root         (0) root         (0)    37405 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   197829 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)    79076 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    43572 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/
+-rw-r--r--   0 root         (0) root         (0)     2084 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/bootstrap.less
+-rw-r--r--   0 root         (0) root         (0)     2101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/core.less
+-rw-r--r--   0 root         (0) root         (0)     2398 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/extras.less
+-rw-r--r--   0 root         (0) root         (0)    19299 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/font-awesome-ie7.less
+-rw-r--r--   0 root         (0) root         (0)     1319 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/font-awesome.less
+-rw-r--r--   0 root         (0) root         (0)    17555 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/icons.less
+-rw-r--r--   0 root         (0) root         (0)     1041 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/mixins.less
+-rw-r--r--   0 root         (0) root         (0)      742 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/path.less
+-rw-r--r--   0 root         (0) root         (0)     8888 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/variables.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/
+-rw-r--r--   0 root         (0) root         (0)     2088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_bootstrap.scss
+-rw-r--r--   0 root         (0) root         (0)     2157 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_core.scss
+-rw-r--r--   0 root         (0) root         (0)     2406 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_extras.scss
+-rw-r--r--   0 root         (0) root         (0)    17555 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_icons.scss
+-rw-r--r--   0 root         (0) root         (0)     1078 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_mixins.scss
+-rw-r--r--   0 root         (0) root         (0)      753 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_path.scss
+-rw-r--r--   0 root         (0) root         (0)     8061 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_variables.scss
+-rw-r--r--   0 root         (0) root         (0)    22328 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/font-awesome-ie7.scss
+-rw-r--r--   0 root         (0) root         (0)     1284 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/font-awesome.scss
+-rw-r--r--   0 root         (0) root         (0)   276410 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome.zip
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/ico/
+-rw-r--r--   0 root         (0) root         (0)     1150 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/ico/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/
+-rw-r--r--   0 root         (0) root         (0)     2290 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/contribution-sample.png
+-rw-r--r--   0 root         (0) root         (0)   114822 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/fort_awesome.jpg
+-rw-r--r--   0 root         (0) root         (0)     8777 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/glyphicons-halflings-white.png
+-rw-r--r--   0 root         (0) root         (0)    12764 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/glyphicons-halflings.png
+-rw-r--r--   0 root         (0) root         (0)   184736 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/icon-flag.pdf
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/
+-rw-r--r--   0 root         (0) root         (0)     8400 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/ZeroClipboard-1.1.7.min.js
+-rw-r--r--   0 root         (0) root         (0)     1635 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/ZeroClipboard-1.1.7.swf
+-rw-r--r--   0 root         (0) root         (0)    15922 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/backbone.min.js
+-rw-r--r--   0 root         (0) root         (0)    28538 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/bootstrap-2.3.1.min.js
+-rw-r--r--   0 root         (0) root         (0)    31596 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/bootstrap-222.min.js
+-rw-r--r--   0 root         (0) root         (0)    93868 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/jquery-1.7.1.min.js
+-rw-r--r--   0 root         (0) root         (0)    13632 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/prettify.min.js
+-rw-r--r--   0 root         (0) root         (0)     1000 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/site.js
+-rw-r--r--   0 root         (0) root         (0)    12140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/underscore.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/
+-rw-r--r--   0 root         (0) root         (0)      636 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/accordion.less
+-rw-r--r--   0 root         (0) root         (0)     1369 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/alerts.less
+-rw-r--r--   0 root         (0) root         (0)     1489 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/bootstrap.less
+-rw-r--r--   0 root         (0) root         (0)      431 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/breadcrumbs.less
+-rw-r--r--   0 root         (0) root         (0)     5709 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/button-groups.less
+-rw-r--r--   0 root         (0) root         (0)     4766 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/buttons.less
+-rw-r--r--   0 root         (0) root         (0)     2482 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/carousel.less
+-rw-r--r--   0 root         (0) root         (0)      644 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/close.less
+-rw-r--r--   0 root         (0) root         (0)     1282 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/code.less
+-rw-r--r--   0 root         (0) root         (0)      306 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/component-animations.less
+-rw-r--r--   0 root         (0) root         (0)     5695 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/dropdowns.less
+-rw-r--r--   0 root         (0) root         (0)    15866 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/forms.less
+-rw-r--r--   0 root         (0) root         (0)      429 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/grid.less
+-rw-r--r--   0 root         (0) root         (0)      521 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/hero-unit.less
+-rw-r--r--   0 root         (0) root         (0)     1884 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/labels-badges.less
+-rw-r--r--   0 root         (0) root         (0)      329 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/layouts.less
+-rw-r--r--   0 root         (0) root         (0)      860 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/media.less
+-rw-r--r--   0 root         (0) root         (0)    23042 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/mixins.less
+-rw-r--r--   0 root         (0) root         (0)     1978 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/modals.less
+-rw-r--r--   0 root         (0) root         (0)    12002 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/navbar.less
+-rw-r--r--   0 root         (0) root         (0)     8163 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/navs.less
+-rw-r--r--   0 root         (0) root         (0)      760 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/pager.less
+-rw-r--r--   0 root         (0) root         (0)     2678 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/pagination.less
+-rw-r--r--   0 root         (0) root         (0)     3077 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/popovers.less
+-rw-r--r--   0 root         (0) root         (0)     2858 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/progress-bars.less
+-rw-r--r--   0 root         (0) root         (0)     4201 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/reset.less
+-rw-r--r--   0 root         (0) root         (0)      565 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-1200px-min.less
+-rw-r--r--   0 root         (0) root         (0)     3920 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-767px-max.less
+-rw-r--r--   0 root         (0) root         (0)      463 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-768px-979px.less
+-rw-r--r--   0 root         (0) root         (0)     4328 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-navbar.less
+-rw-r--r--   0 root         (0) root         (0)     1602 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-utilities.less
+-rw-r--r--   0 root         (0) root         (0)     1069 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive.less
+-rw-r--r--   0 root         (0) root         (0)      885 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/scaffolding.less
+-rw-r--r--   0 root         (0) root         (0)    10841 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/sprites.less
+-rw-r--r--   0 root         (0) root         (0)     6255 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/tables.less
+-rw-r--r--   0 root         (0) root         (0)     1192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/thumbnails.less
+-rw-r--r--   0 root         (0) root         (0)     1684 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/tooltip.less
+-rw-r--r--   0 root         (0) root         (0)     4857 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/type.less
+-rw-r--r--   0 root         (0) root         (0)      335 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/utilities.less
+-rw-r--r--   0 root         (0) root         (0)     9142 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/variables.less
+-rw-r--r--   0 root         (0) root         (0)      552 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/wells.less
+-rw-r--r--   0 root         (0) root         (0)     3382 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/lazy.less
+-rw-r--r--   0 root         (0) root         (0)     2374 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/mixins.less
+-rw-r--r--   0 root         (0) root         (0)      921 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-1200px-min.less
+-rw-r--r--   0 root         (0) root         (0)     1595 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-767px-max.less
+-rw-r--r--   0 root         (0) root         (0)     1230 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-768px-979px.less
+-rw-r--r--   0 root         (0) root         (0)      170 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-navbar.less
+-rw-r--r--   0 root         (0) root         (0)     1405 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive.less
+-rw-r--r--   0 root         (0) root         (0)     7153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/site.less
+-rw-r--r--   0 root         (0) root         (0)      378 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/sticky-footer.less
+-rw-r--r--   0 root         (0) root         (0)    10482 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/variables.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/cheatsheet/
+-rw-r--r--   0 root         (0) root         (0)    61253 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/cheatsheet/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/community/
+-rw-r--r--   0 root         (0) root         (0)    16656 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/community/index.html
+-rw-r--r--   0 root         (0) root         (0)       55 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/design.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/examples/
+-rw-r--r--   0 root         (0) root         (0)    42204 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/examples/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/get-started/
+-rw-r--r--   0 root         (0) root         (0)    16041 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/get-started/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adjust/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adjust/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adn/
+-rw-r--r--   0 root         (0) root         (0)    10039 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adn/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-center/
+-rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-center/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-justify/
+-rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-justify/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-left/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-right/
+-rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ambulance/
+-rw-r--r--   0 root         (0) root         (0)    10119 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ambulance/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/anchor/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/anchor/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/android/
+-rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/android/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-down/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-left/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-right/
+-rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-up/
+-rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/apple/
+-rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/apple/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/archive/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/archive/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-down/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-left/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-right/
+-rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-up/
+-rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/asterisk/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/asterisk/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/backward/
+-rw-r--r--   0 root         (0) root         (0)    10111 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/backward/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ban-circle/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ban-circle/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bar-chart/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bar-chart/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/barcode/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/barcode/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beaker/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beaker/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beer/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beer/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell-alt/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket/
+-rw-r--r--   0 root         (0) root         (0)    10117 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket-sign/
+-rw-r--r--   0 root         (0) root         (0)    10182 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bold/
+-rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bold/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bolt/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bolt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/book/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/book/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark-empty/
+-rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark-empty/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/briefcase/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/briefcase/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/btc/
+-rw-r--r--   0 root         (0) root         (0)    10158 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/btc/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bug/
+-rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bug/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/building/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/building/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullhorn/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullhorn/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullseye/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullseye/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar-empty/
+-rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar-empty/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera-retro/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera-retro/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-down/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-left/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-right/
+-rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-up/
+-rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/certificate/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/certificate/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-empty/
+-rw-r--r--   0 root         (0) root         (0)    10239 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-empty/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-minus/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-minus/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-sign/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-down/
+-rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-left/
+-rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-right/
+-rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-down/
+-rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-left/
+-rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-right/
+-rw-r--r--   0 root         (0) root         (0)    10240 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-up/
+-rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-up/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-down/
+-rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-left/
+-rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-right/
+-rw-r--r--   0 root         (0) root         (0)    10240 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-up/
+-rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-blank/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-blank/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-download/
+-rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-download/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-upload/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-upload/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cny/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cny/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code-fork/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code-fork/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/coffee/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/coffee/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cog/
+-rw-r--r--   0 root         (0) root         (0)    10130 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cog/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cogs/
+-rw-r--r--   0 root         (0) root         (0)    10144 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cogs/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-alt/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-top/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-top/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/columns/
+-rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/columns/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment-alt/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments-alt/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/compass/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/compass/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/copy/
+-rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/copy/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/credit-card/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/credit-card/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/crop/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/crop/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/css3/
+-rw-r--r--   0 root         (0) root         (0)    10052 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/css3/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cut/
+-rw-r--r--   0 root         (0) root         (0)    10045 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cut/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dashboard/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dashboard/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/desktop/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/desktop/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-down/
+-rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-left/
+-rw-r--r--   0 root         (0) root         (0)    10227 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-right/
+-rw-r--r--   0 root         (0) root         (0)    10240 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-up/
+-rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download-alt/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dribbble/
+-rw-r--r--   0 root         (0) root         (0)    10104 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dribbble/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dropbox/
+-rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dropbox/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit-sign/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eject/
+-rw-r--r--   0 root         (0) root         (0)    10072 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eject/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-horizontal/
+-rw-r--r--   0 root         (0) root         (0)    10257 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-horizontal/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-vertical/
+-rw-r--r--   0 root         (0) root         (0)    10231 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-vertical/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope-alt/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eraser/
+-rw-r--r--   0 root         (0) root         (0)    10126 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eraser/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eur/
+-rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eur/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exchange/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exchange/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation-sign/
+-rw-r--r--   0 root         (0) root         (0)    10218 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand-alt/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link/
+-rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link-sign/
+-rw-r--r--   0 root         (0) root         (0)    10244 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-close/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-close/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-open/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-open/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook/
+-rw-r--r--   0 root         (0) root         (0)    10104 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook-sign/
+-rw-r--r--   0 root         (0) root         (0)    10169 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facetime-video/
+-rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facetime-video/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-backward/
+-rw-r--r--   0 root         (0) root         (0)    10176 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-backward/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-forward/
+-rw-r--r--   0 root         (0) root         (0)    10163 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-forward/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/female/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/female/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fighter-jet/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fighter-jet/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file/
+-rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-alt/
+-rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text/
+-rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text-alt/
+-rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/film/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/film/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/filter/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/filter/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire-extinguisher/
+-rw-r--r--   0 root         (0) root         (0)    10231 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire-extinguisher/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-alt/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-checkered/
+-rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-checkered/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flickr/
+-rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flickr/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close-alt/
+-rw-r--r--   0 root         (0) root         (0)    10218 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open-alt/
+-rw-r--r--   0 root         (0) root         (0)    10205 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/font/
+-rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/font/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/food/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/food/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/forward/
+-rw-r--r--   0 root         (0) root         (0)    10098 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/forward/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/foursquare/
+-rw-r--r--   0 root         (0) root         (0)    10130 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/foursquare/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/frown/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/frown/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fullscreen/
+-rw-r--r--   0 root         (0) root         (0)    10137 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fullscreen/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gamepad/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gamepad/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gbp/
+-rw-r--r--   0 root         (0) root         (0)    10042 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gbp/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gift/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gift/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github/
+-rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-alt/
+-rw-r--r--   0 root         (0) root         (0)    10130 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-sign/
+-rw-r--r--   0 root         (0) root         (0)    10143 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gittip/
+-rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gittip/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/glass/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/glass/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/globe/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/globe/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus/
+-rw-r--r--   0 root         (0) root         (0)    10143 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus-sign/
+-rw-r--r--   0 root         (0) root         (0)    10208 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/group/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/group/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/h-sign/
+-rw-r--r--   0 root         (0) root         (0)    10080 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/h-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-down/
+-rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-left/
+-rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-right/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-up/
+-rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hdd/
+-rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hdd/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/headphones/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/headphones/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart-empty/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart-empty/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/home/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/home/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hospital/
+-rw-r--r--   0 root         (0) root         (0)    10106 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hospital/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/html5/
+-rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/html5/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inbox/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inbox/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-left/
+-rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-right/
+-rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info-sign/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inr/
+-rw-r--r--   0 root         (0) root         (0)    10124 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inr/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/instagram/
+-rw-r--r--   0 root         (0) root         (0)    10117 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/instagram/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/italic/
+-rw-r--r--   0 root         (0) root         (0)    10084 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/italic/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/jpy/
+-rw-r--r--   0 root         (0) root         (0)    10122 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/jpy/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/key/
+-rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/key/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/keyboard/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/keyboard/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/krw/
+-rw-r--r--   0 root         (0) root         (0)    10122 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/krw/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/laptop/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/laptop/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/leaf/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/leaf/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/legal/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/legal/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lemon/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lemon/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-down/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-up/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lightbulb/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lightbulb/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/link/
+-rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/link/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin/
+-rw-r--r--   0 root         (0) root         (0)    10104 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin-sign/
+-rw-r--r--   0 root         (0) root         (0)    10169 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linux/
+-rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linux/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list/
+-rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-alt/
+-rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ol/
+-rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ol/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ul/
+-rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ul/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/location-arrow/
+-rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/location-arrow/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lock/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lock/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-down/
+-rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-left/
+-rw-r--r--   0 root         (0) root         (0)    10201 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-right/
+-rw-r--r--   0 root         (0) root         (0)    10214 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-up/
+-rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magic/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magic/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magnet/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magnet/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mail-reply-all/
+-rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mail-reply-all/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/male/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/male/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/map-marker/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/map-marker/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/maxcdn/
+-rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/maxcdn/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/medkit/
+-rw-r--r--   0 root         (0) root         (0)    10080 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/medkit/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/meh/
+-rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/meh/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone-off/
+-rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone-off/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign-alt/
+-rw-r--r--   0 root         (0) root         (0)    10192 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mobile-phone/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mobile-phone/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/money/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/money/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/moon/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/moon/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/move/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/move/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/music/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/music/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/off/
+-rw-r--r--   0 root         (0) root         (0)    10135 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/off/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok/
+-rw-r--r--   0 root         (0) root         (0)    10036 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-circle/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-circle/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-sign/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paper-clip/
+-rw-r--r--   0 root         (0) root         (0)    10222 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paper-clip/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paste/
+-rw-r--r--   0 root         (0) root         (0)    10071 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paste/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pause/
+-rw-r--r--   0 root         (0) root         (0)    10072 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pause/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pencil/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pencil/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone-sign/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/picture/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/picture/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest/
+-rw-r--r--   0 root         (0) root         (0)    10117 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest-sign/
+-rw-r--r--   0 root         (0) root         (0)    10182 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plane/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plane/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play/
+-rw-r--r--   0 root         (0) root         (0)    10059 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-circle/
+-rw-r--r--   0 root         (0) root         (0)    10150 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-circle/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-sign/
+-rw-r--r--   0 root         (0) root         (0)    10124 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign-alt/
+-rw-r--r--   0 root         (0) root         (0)    10213 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/print/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/print/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pushpin/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pushpin/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/puzzle-piece/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/puzzle-piece/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/qrcode/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/qrcode/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question-sign/
+-rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-left/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-left/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-right/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-right/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/random/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/random/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/refresh/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/refresh/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-circle/
+-rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-circle/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-sign/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/renren/
+-rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/renren/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reorder/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reorder/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/repeat/
+-rw-r--r--   0 root         (0) root         (0)    10173 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/repeat/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply/
+-rw-r--r--   0 root         (0) root         (0)    10162 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply-all/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply-all/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-full/
+-rw-r--r--   0 root         (0) root         (0)    10150 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-full/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-horizontal/
+-rw-r--r--   0 root         (0) root         (0)    10231 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-horizontal/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-small/
+-rw-r--r--   0 root         (0) root         (0)    10163 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-small/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-vertical/
+-rw-r--r--   0 root         (0) root         (0)    10205 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-vertical/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/retweet/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/retweet/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/road/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/road/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rocket/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rocket/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss/
+-rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss-sign/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/save/
+-rw-r--r--   0 root         (0) root         (0)    10058 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/save/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/screenshot/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/screenshot/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/search/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/search/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-alt/
+-rw-r--r--   0 root         (0) root         (0)    10216 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-sign/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shield/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shield/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shopping-cart/
+-rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shopping-cart/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sign-blank/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sign-blank/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signal/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signal/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signin/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signin/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signout/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signout/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sitemap/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sitemap/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/skype/
+-rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/skype/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/smile/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/smile/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet/
+-rw-r--r--   0 root         (0) root         (0)    10218 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet-alt/
+-rw-r--r--   0 root         (0) root         (0)    10270 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes/
+-rw-r--r--   0 root         (0) root         (0)    10244 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes-alt/
+-rw-r--r--   0 root         (0) root         (0)    10296 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order/
+-rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order-alt/
+-rw-r--r--   0 root         (0) root         (0)    10231 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-down/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-up/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/spinner/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/spinner/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stackexchange/
+-rw-r--r--   0 root         (0) root         (0)    10169 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stackexchange/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-empty/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-empty/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half-empty/
+-rw-r--r--   0 root         (0) root         (0)    10296 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half-empty/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-backward/
+-rw-r--r--   0 root         (0) root         (0)    10176 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-backward/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-forward/
+-rw-r--r--   0 root         (0) root         (0)    10163 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-forward/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stethoscope/
+-rw-r--r--   0 root         (0) root         (0)    10145 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stethoscope/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stop/
+-rw-r--r--   0 root         (0) root         (0)    10059 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stop/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/strikethrough/
+-rw-r--r--   0 root         (0) root         (0)    10175 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/strikethrough/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/subscript/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/subscript/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/suitcase/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/suitcase/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sun/
+-rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sun/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/superscript/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/superscript/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/table/
+-rw-r--r--   0 root         (0) root         (0)    10071 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/table/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tablet/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tablet/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tag/
+-rw-r--r--   0 root         (0) root         (0)    10049 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tag/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tags/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tags/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tasks/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tasks/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/terminal/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/terminal/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-height/
+-rw-r--r--   0 root         (0) root         (0)    10149 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-height/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-width/
+-rw-r--r--   0 root         (0) root         (0)    10136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-width/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th/
+-rw-r--r--   0 root         (0) root         (0)    10032 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-large/
+-rw-r--r--   0 root         (0) root         (0)    10110 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-large/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-list/
+-rw-r--r--   0 root         (0) root         (0)    10097 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-list/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down-alt/
+-rw-r--r--   0 root         (0) root         (0)    10205 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up-alt/
+-rw-r--r--   0 root         (0) root         (0)    10179 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ticket/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ticket/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/time/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/time/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tint/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tint/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trash/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trash/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trello/
+-rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trello/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trophy/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trophy/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/truck/
+-rw-r--r--   0 root         (0) root         (0)    10075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/truck/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr/
+-rw-r--r--   0 root         (0) root         (0)    10078 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr-sign/
+-rw-r--r--   0 root         (0) root         (0)    10143 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter/
+-rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter-sign/
+-rw-r--r--   0 root         (0) root         (0)    10156 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/umbrella/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/umbrella/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/underline/
+-rw-r--r--   0 root         (0) root         (0)    10123 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/underline/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/undo/
+-rw-r--r--   0 root         (0) root         (0)    10146 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/undo/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlink/
+-rw-r--r--   0 root         (0) root         (0)    10084 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlink/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock-alt/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload-alt/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload-alt/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/usd/
+-rw-r--r--   0 root         (0) root         (0)    10125 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/usd/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user/
+-rw-r--r--   0 root         (0) root         (0)    10062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user-md/
+-rw-r--r--   0 root         (0) root         (0)    10093 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user-md/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/vk/
+-rw-r--r--   0 root         (0) root         (0)    10026 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/vk/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-down/
+-rw-r--r--   0 root         (0) root         (0)    10153 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-down/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-off/
+-rw-r--r--   0 root         (0) root         (0)    10140 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-off/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-up/
+-rw-r--r--   0 root         (0) root         (0)    10127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-up/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/warning-sign/
+-rw-r--r--   0 root         (0) root         (0)    10166 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/warning-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/weibo/
+-rw-r--r--   0 root         (0) root         (0)    10065 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/weibo/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/windows/
+-rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/windows/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/wrench/
+-rw-r--r--   0 root         (0) root         (0)    10088 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/wrench/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing/
+-rw-r--r--   0 root         (0) root         (0)    10052 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing-sign/
+-rw-r--r--   0 root         (0) root         (0)    10117 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube/
+-rw-r--r--   0 root         (0) root         (0)    10091 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-play/
+-rw-r--r--   0 root         (0) root         (0)    10195 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-play/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-sign/
+-rw-r--r--   0 root         (0) root         (0)    10156 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-sign/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-in/
+-rw-r--r--   0 root         (0) root         (0)    10101 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-in/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-out/
+-rw-r--r--   0 root         (0) root         (0)    10114 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-out/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icons/
+-rw-r--r--   0 root         (0) root         (0)    63049 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icons/index.html
+-rw-r--r--   0 root         (0) root         (0)    50111 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icons.yml
+-rw-r--r--   0 root         (0) root         (0)    15711 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/license/
+-rw-r--r--   0 root         (0) root         (0)    12107 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/license/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/test/
+-rw-r--r--   0 root         (0) root         (0)    44340 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/test/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/whats-new/
+-rw-r--r--   0 root         (0) root         (0)    21505 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/whats-new/index.html
+-rw-r--r--   0 root         (0) root         (0)       14 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/CNAME
+-rw-r--r--   0 root         (0) root         (0)     1292 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/Makefile
+-rw-r--r--   0 root         (0) root         (0)     5564 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/README.md-nobuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/
+-rw-r--r--   0 root         (0) root         (0)     1136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/accessibility-facdn.html
+-rw-r--r--   0 root         (0) root         (0)     6020 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/accessibility-manual.html
+-rw-r--r--   0 root         (0) root         (0)      703 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/background.html
+-rw-r--r--   0 root         (0) root         (0)      848 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/cta-cdn-ally.html
+-rw-r--r--   0 root         (0) root         (0)     1285 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/other.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/ads/
+-rw-r--r--   0 root         (0) root         (0)      150 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/ads/carbon.html
+-rw-r--r--   0 root         (0) root         (0)      439 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/brand-adblock-warning.html
+-rw-r--r--   0 root         (0) root         (0)      476 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/brand-license.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/code/
+-rw-r--r--   0 root         (0) root         (0)      374 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/code/core.less
+-rw-r--r--   0 root         (0) root         (0)      380 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/code/core.scss
+-rw-r--r--   0 root         (0) root         (0)      311 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/code/license.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/
+-rw-r--r--   0 root         (0) root         (0)     1093 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/getting-support.html
+-rw-r--r--   0 root         (0) root         (0)      277 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/project-milestones.html
+-rw-r--r--   0 root         (0) root         (0)      811 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/reporting-bugs.html
+-rw-r--r--   0 root         (0) root         (0)     1473 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/requesting-new-icons.html
+-rw-r--r--   0 root         (0) root         (0)      614 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/submitting-pull-requests.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/
+-rw-r--r--   0 root         (0) root         (0)     3814 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/accessible.html
+-rw-r--r--   0 root         (0) root         (0)     2778 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/animated.html
+-rw-r--r--   0 root         (0) root         (0)     1628 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/basic.html
+-rw-r--r--   0 root         (0) root         (0)     4388 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/bootstrap.html
+-rw-r--r--   0 root         (0) root         (0)     1422 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/bordered-pulled.html
+-rw-r--r--   0 root         (0) root         (0)      625 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/custom.html
+-rw-r--r--   0 root         (0) root         (0)     1852 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/fixed-width.html
+-rw-r--r--   0 root         (0) root         (0)     1815 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/larger.html
+-rw-r--r--   0 root         (0) root         (0)     1325 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/list.html
+-rw-r--r--   0 root         (0) root         (0)     1772 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/rotated-flipped.html
+-rw-r--r--   0 root         (0) root         (0)     2614 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/stacked.html
+-rw-r--r--   0 root         (0) root         (0)     2311 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/footer.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/
+-rw-r--r--   0 root         (0) root         (0)      604 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/accessibility.html
+-rw-r--r--   0 root         (0) root         (0)      764 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/brand.html
+-rw-r--r--   0 root         (0) root         (0)      574 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/chart.html
+-rw-r--r--   0 root         (0) root         (0)      589 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/currency.html
+-rw-r--r--   0 root         (0) root         (0)      604 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/directional.html
+-rw-r--r--   0 root         (0) root         (0)      594 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/file-type.html
+-rw-r--r--   0 root         (0) root         (0)      608 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/form-control.html
+-rw-r--r--   0 root         (0) root         (0)      579 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/gender.html
+-rw-r--r--   0 root         (0) root         (0)      569 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/hand.html
+-rw-r--r--   0 root         (0) root         (0)      584 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/medical.html
+-rw-r--r--   0 root         (0) root         (0)     1069 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/new.html
+-rw-r--r--   0 root         (0) root         (0)      584 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/payment.html
+-rw-r--r--   0 root         (0) root         (0)      995 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/spinner.html
+-rw-r--r--   0 root         (0) root         (0)      604 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/text-editor.html
+-rw-r--r--   0 root         (0) root         (0)      619 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/transportation.html
+-rw-r--r--   0 root         (0) root         (0)      609 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/video-player.html
+-rw-r--r--   0 root         (0) root         (0)      624 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/web-application.html
+-rw-r--r--   0 root         (0) root         (0)     4083 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/jumbotron-carousel.html
+-rw-r--r--   0 root         (0) root         (0)      382 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/jumbotron.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/modals/
+-rw-r--r--   0 root         (0) root         (0)     3557 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/modals/download.html
+-rw-r--r--   0 root         (0) root         (0)     2929 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/modals/fa5.html
+-rw-r--r--   0 root         (0) root         (0)     8209 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/navbar.html
+-rw-r--r--   0 root         (0) root         (0)     1505 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/new-features.html
+-rw-r--r--   0 root         (0) root         (0)     5308 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/new-naming.html
+-rw-r--r--   0 root         (0) root         (0)      519 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/new-upgrading.html
+-rw-r--r--   0 root         (0) root         (0)      889 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/newsletter-subscribe.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/
+-rw-r--r--   0 root         (0) root         (0)     1442 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/camera-retro-tee.html
+-rw-r--r--   0 root         (0) root         (0)     1429 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/classics-tee.html
+-rw-r--r--   0 root         (0) root         (0)      755 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/cta-suggestions.html
+-rw-r--r--   0 root         (0) root         (0)     1328 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/fa-ther-tee.html
+-rw-r--r--   0 root         (0) root         (0)     1440 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/green-logo-tee.html
+-rw-r--r--   0 root         (0) root         (0)     1431 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/old-skool-tee.html
+-rw-r--r--   0 root         (0) root         (0)     1134 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/rock-paper-scissors-lizard-spock-tee.html
+-rw-r--r--   0 root         (0) root         (0)     1403 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/space-shuttle-tee.html
+-rw-r--r--   0 root         (0) root         (0)     1735 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/white-logo-tee.html
+-rw-r--r--   0 root         (0) root         (0)      139 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/stripe-ad.html
+-rw-r--r--   0 root         (0) root         (0)     1330 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/stripe-social.html
+-rw-r--r--   0 root         (0) root         (0)      978 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tell-me-thanks.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/
+-rw-r--r--   0 root         (0) root         (0)      589 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped-inside-anchor.html
+-rw-r--r--   0 root         (0) root         (0)      733 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped-inside-btn.html
+-rw-r--r--   0 root         (0) root         (0)      493 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped.html
+-rw-r--r--   0 root         (0) root         (0)     1842 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked-inside-anchor.html
+-rw-r--r--   0 root         (0) root         (0)      151 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked-with-text.html
+-rw-r--r--   0 root         (0) root         (0)     1818 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked.html
+-rw-r--r--   0 root         (0) root         (0)     1174 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/thanks-to.html
+-rw-r--r--   0 root         (0) root         (0)     2321 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/why.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_layouts/
+-rw-r--r--   0 root         (0) root         (0)     4320 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_layouts/base.html
+-rw-r--r--   0 root         (0) root         (0)     3502 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_layouts/icon.html
+-rw-r--r--   0 root         (0) root         (0)     1174 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_layouts/survey.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_plugins/
+-rw-r--r--   0 root         (0) root         (0)      998 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_plugins/flatten_icon_filters.rb
+-rw-r--r--   0 root         (0) root         (0)      885 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_plugins/icon_page_generator.rb
+-rw-r--r--   0 root         (0) root         (0)     2973 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_plugins/site.rb
+-rw-r--r--   0 root         (0) root         (0)     1265 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/accessibility.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/css/
+-rw-r--r--   0 root         (0) root         (0)      815 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/css/prettify.css
+-rw-r--r--   0 root         (0) root         (0)     3063 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/css/pygments.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/
+-rw-r--r--   0 root         (0) root         (0)      323 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/HELP-US-OUT.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/
+-rw-r--r--   0 root         (0) root         (0)   134808 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 root         (0) root         (0)   165742 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/
+-rw-r--r--   0 root         (0) root         (0)      722 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/animated.less
+-rw-r--r--   0 root         (0) root         (0)      594 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/bordered-pulled.less
+-rw-r--r--   0 root         (0) root         (0)      115 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/core.less
+-rw-r--r--   0 root         (0) root         (0)      128 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/fixed-width.less
+-rw-r--r--   0 root         (0) root         (0)      368 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/font-awesome.less
+-rw-r--r--   0 root         (0) root         (0)      342 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/icons.less
+-rw-r--r--   0 root         (0) root         (0)      379 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/larger.less
+-rw-r--r--   0 root         (0) root         (0)      386 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/list.less
+-rw-r--r--   0 root         (0) root         (0)     1265 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/mixins.less
+-rw-r--r--   0 root         (0) root         (0)      771 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/path.less
+-rw-r--r--   0 root         (0) root         (0)      631 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/rotated-flipped.less
+-rw-r--r--   0 root         (0) root         (0)      118 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/screen-reader.less
+-rw-r--r--   0 root         (0) root         (0)      485 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/stacked.less
+-rw-r--r--   0 root         (0) root         (0)      658 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/variables.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/
+-rw-r--r--   0 root         (0) root         (0)      724 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_animated.scss
+-rw-r--r--   0 root         (0) root         (0)      601 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_bordered-pulled.scss
+-rw-r--r--   0 root         (0) root         (0)      116 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_core.scss
+-rw-r--r--   0 root         (0) root         (0)      129 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_fixed-width.scss
+-rw-r--r--   0 root         (0) root         (0)      344 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_icons.scss
+-rw-r--r--   0 root         (0) root         (0)      384 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_larger.scss
+-rw-r--r--   0 root         (0) root         (0)      387 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_list.scss
+-rw-r--r--   0 root         (0) root         (0)     1293 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_mixins.scss
+-rw-r--r--   0 root         (0) root         (0)      783 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_path.scss
+-rw-r--r--   0 root         (0) root         (0)      681 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_rotated-flipped.scss
+-rw-r--r--   0 root         (0) root         (0)      134 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_screen-reader.scss
+-rw-r--r--   0 root         (0) root         (0)      491 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_stacked.scss
+-rw-r--r--   0 root         (0) root         (0)      739 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_variables.scss
+-rw-r--r--   0 root         (0) root         (0)      303 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/font-awesome.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/ico/
+-rw-r--r--   0 root         (0) root         (0)    52047 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/ico/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/img/
+-rw-r--r--   0 root         (0) root         (0)    72993 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/img/algolia.png
+-rw-r--r--   0 root         (0) root         (0)    14209 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/img/logo-themeisle.png
+-rw-r--r--   0 root         (0) root         (0)     8268 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/img/logo-wpbeginner.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/
+-rw-r--r--   0 root         (0) root         (0)     8400 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/ZeroClipboard-1.1.7.min.js
+-rw-r--r--   0 root         (0) root         (0)     1635 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/ZeroClipboard-1.1.7.swf
+-rw-r--r--   0 root         (0) root         (0)     2376 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/html5shiv.js
+-rw-r--r--   0 root         (0) root         (0)    20740 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/monetization.js
+-rw-r--r--   0 root         (0) root         (0)    13632 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/prettify.min.js
+-rw-r--r--   0 root         (0) root         (0)     4035 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/respond.min.js
+-rw-r--r--   0 root         (0) root         (0)     3080 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/search.js
+-rw-r--r--   0 root         (0) root         (0)     1562 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/site.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/
+-rw-r--r--   0 root         (0) root         (0)     8099 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/.csscomb.json
+-rw-r--r--   0 root         (0) root         (0)      456 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/.csslintrc
+-rw-r--r--   0 root         (0) root         (0)     1518 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/alerts.less
+-rw-r--r--   0 root         (0) root         (0)     1199 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/badges.less
+-rw-r--r--   0 root         (0) root         (0)     1291 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/bootstrap.less
+-rw-r--r--   0 root         (0) root         (0)      594 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/breadcrumbs.less
+-rw-r--r--   0 root         (0) root         (0)     5675 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/button-groups.less
+-rw-r--r--   0 root         (0) root         (0)     3662 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/buttons.less
+-rw-r--r--   0 root         (0) root         (0)     5407 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/carousel.less
+-rw-r--r--   0 root         (0) root         (0)      764 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/close.less
+-rw-r--r--   0 root         (0) root         (0)     1401 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/code.less
+-rw-r--r--   0 root         (0) root         (0)      666 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/component-animations.less
+-rw-r--r--   0 root         (0) root         (0)     4876 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/dropdowns.less
+-rw-r--r--   0 root         (0) root         (0)    15859 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/forms.less
+-rw-r--r--   0 root         (0) root         (0)    19803 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/glyphicons.less
+-rw-r--r--   0 root         (0) root         (0)     1387 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/grid.less
+-rw-r--r--   0 root         (0) root         (0)     4246 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/input-groups.less
+-rw-r--r--   0 root         (0) root         (0)     1062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/jumbotron.less
+-rw-r--r--   0 root         (0) root         (0)     1079 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/labels.less
+-rw-r--r--   0 root         (0) root         (0)     3124 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/list-group.less
+-rw-r--r--   0 root         (0) root         (0)      900 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/media.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/
+-rw-r--r--   0 root         (0) root         (0)      257 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/alerts.less
+-rw-r--r--   0 root         (0) root         (0)      151 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/background-variant.less
+-rw-r--r--   0 root         (0) root         (0)      468 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/border-radius.less
+-rw-r--r--   0 root         (0) root         (0)     1476 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/buttons.less
+-rw-r--r--   0 root         (0) root         (0)      120 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/center-block.less
+-rw-r--r--   0 root         (0) root         (0)      605 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/clearfix.less
+-rw-r--r--   0 root         (0) root         (0)     2641 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/forms.less
+-rw-r--r--   0 root         (0) root         (0)     4388 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/gradients.less
+-rw-r--r--   0 root         (0) root         (0)     2797 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/grid-framework.less
+-rw-r--r--   0 root         (0) root         (0)     3107 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/grid.less
+-rw-r--r--   0 root         (0) root         (0)      574 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/hide-text.less
+-rw-r--r--   0 root         (0) root         (0)     1062 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/image.less
+-rw-r--r--   0 root         (0) root         (0)      161 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/labels.less
+-rw-r--r--   0 root         (0) root         (0)      546 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/list-group.less
+-rw-r--r--   0 root         (0) root         (0)      232 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/nav-divider.less
+-rw-r--r--   0 root         (0) root         (0)      364 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/nav-vertical-align.less
+-rw-r--r--   0 root         (0) root         (0)      148 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/opacity.less
+-rw-r--r--   0 root         (0) root         (0)      485 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/pagination.less
+-rw-r--r--   0 root         (0) root         (0)      537 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/panels.less
+-rw-r--r--   0 root         (0) root         (0)      191 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/progress-bar.less
+-rw-r--r--   0 root         (0) root         (0)      248 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/reset-filter.less
+-rw-r--r--   0 root         (0) root         (0)      470 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/reset-text.less
+-rw-r--r--   0 root         (0) root         (0)      196 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/resize.less
+-rw-r--r--   0 root         (0) root         (0)      354 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/responsive-visibility.less
+-rw-r--r--   0 root         (0) root         (0)      127 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/size.less
+-rw-r--r--   0 root         (0) root         (0)      159 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/tab-focus.less
+-rw-r--r--   0 root         (0) root         (0)      700 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/table-row.less
+-rw-r--r--   0 root         (0) root         (0)      128 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/text-emphasis.less
+-rw-r--r--   0 root         (0) root         (0)      162 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/text-overflow.less
+-rw-r--r--   0 root         (0) root         (0)     6650 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/vendor-prefixes.less
+-rw-r--r--   0 root         (0) root         (0)     1136 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins.less
+-rw-r--r--   0 root         (0) root         (0)     3565 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/modals.less
+-rw-r--r--   0 root         (0) root         (0)    14628 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/navbar.less
+-rw-r--r--   0 root         (0) root         (0)     4930 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/navs.less
+-rw-r--r--   0 root         (0) root         (0)     7559 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/normalize.less
+-rw-r--r--   0 root         (0) root         (0)      861 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/pager.less
+-rw-r--r--   0 root         (0) root         (0)     2059 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/pagination.less
+-rw-r--r--   0 root         (0) root         (0)     6279 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/panels.less
+-rw-r--r--   0 root         (0) root         (0)     3488 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/popovers.less
+-rw-r--r--   0 root         (0) root         (0)     1939 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/print.less
+-rw-r--r--   0 root         (0) root         (0)     1925 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/progress-bars.less
+-rw-r--r--   0 root         (0) root         (0)      546 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/responsive-embed.less
+-rw-r--r--   0 root         (0) root         (0)     4262 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/responsive-utilities.less
+-rw-r--r--   0 root         (0) root         (0)     2988 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/scaffolding.less
+-rw-r--r--   0 root         (0) root         (0)     4612 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/tables.less
+-rw-r--r--   0 root         (0) root         (0)     8197 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/theme.less
+-rw-r--r--   0 root         (0) root         (0)      753 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/thumbnails.less
+-rw-r--r--   0 root         (0) root         (0)     2985 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/tooltip.less
+-rw-r--r--   0 root         (0) root         (0)     5954 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/type.less
+-rw-r--r--   0 root         (0) root         (0)      747 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/utilities.less
+-rw-r--r--   0 root         (0) root         (0)    27473 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/variables.less
+-rw-r--r--   0 root         (0) root         (0)      527 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/wells.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/gandy-grid/
+-rw-r--r--   0 root         (0) root         (0)      920 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/gandy-grid/grid.less
+-rw-r--r--   0 root         (0) root         (0)      287 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/gandy-grid/mixins.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/
+-rw-r--r--   0 root         (0) root         (0)      151 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/algolia.less
+-rw-r--r--   0 root         (0) root         (0)     6483 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/banner-ad.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/
+-rw-r--r--   0 root         (0) root         (0)      335 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/alerts.less
+-rw-r--r--   0 root         (0) root         (0)      208 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/buttons.less
+-rw-r--r--   0 root         (0) root         (0)     1972 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/jumbotron.less
+-rw-r--r--   0 root         (0) root         (0)      284 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/labels.less
+-rw-r--r--   0 root         (0) root         (0)      133 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/modals.less
+-rw-r--r--   0 root         (0) root         (0)     4172 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/navbar.less
+-rw-r--r--   0 root         (0) root         (0)      213 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/panels.less
+-rw-r--r--   0 root         (0) root         (0)      119 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/tooltip.less
+-rw-r--r--   0 root         (0) root         (0)      414 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/type.less
+-rw-r--r--   0 root         (0) root         (0)     4873 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/variables.less
+-rw-r--r--   0 root         (0) root         (0)      232 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/wells.less
+-rw-r--r--   0 root         (0) root         (0)      328 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bsap-ad.less
+-rw-r--r--   0 root         (0) root         (0)      425 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/carbon-ad.less
+-rw-r--r--   0 root         (0) root         (0)      481 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/example-rating.less
+-rw-r--r--   0 root         (0) root         (0)      320 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/fa5.less
+-rw-r--r--   0 root         (0) root         (0)      544 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/feature-list.less
+-rw-r--r--   0 root         (0) root         (0)      695 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/fontawesome-icon-list.less
+-rw-r--r--   0 root         (0) root         (0)     1180 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/footer.less
+-rw-r--r--   0 root         (0) root         (0)     1746 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/jumbotron-carousel.less
+-rw-r--r--   0 root         (0) root         (0)       30 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/layout.less
+-rw-r--r--   0 root         (0) root         (0)     4864 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/lazy.less
+-rw-r--r--   0 root         (0) root         (0)      435 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/newsletter.less
+-rw-r--r--   0 root         (0) root         (0)       62 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/print.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/
+-rw-r--r--   0 root         (0) root         (0)      918 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-lg.less
+-rw-r--r--   0 root         (0) root         (0)       97 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-md.less
+-rw-r--r--   0 root         (0) root         (0)      327 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-sm-up.less
+-rw-r--r--   0 root         (0) root         (0)      874 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-sm.less
+-rw-r--r--   0 root         (0) root         (0)     1764 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-xs.less
+-rw-r--r--   0 root         (0) root         (0)      586 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/search.less
+-rw-r--r--   0 root         (0) root         (0)      325 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/social-buttons.less
+-rw-r--r--   0 root         (0) root         (0)     2145 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/store.less
+-rw-r--r--   0 root         (0) root         (0)       68 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/stripe-ad.less
+-rw-r--r--   0 root         (0) root         (0)      148 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/sumome.less
+-rw-r--r--   0 root         (0) root         (0)    12164 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/textured-bg.less
+-rw-r--r--   0 root         (0) root         (0)      896 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/views.less
+-rw-r--r--   0 root         (0) root         (0)     1229 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/cdn/
+-rw-r--r--   0 root         (0) root         (0)     1858 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/cdn/error.html
+-rw-r--r--   0 root         (0) root         (0)     2396 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/cdn/success.html
+-rw-r--r--   0 root         (0) root         (0)     1493 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/cheatsheet.html
+-rw-r--r--   0 root         (0) root         (0)     1194 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/community.html
+-rw-r--r--   0 root         (0) root         (0)       55 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/design.html
+-rw-r--r--   0 root         (0) root         (0)     1913 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/examples.html
+-rw-r--r--   0 root         (0) root         (0)    12155 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/get-started.html
+-rw-r--r--   0 root         (0) root         (0)     4356 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/icons.html
+-rw-r--r--   0 root         (0) root         (0)   121432 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/icons.yml
+-rw-r--r--   0 root         (0) root         (0)      592 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/index.html
+-rw-r--r--   0 root         (0) root         (0)     2465 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/license.html
+-rw-r--r--   0 root         (0) root         (0)     2517 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/store.html
+-rw-r--r--   0 root         (0) root         (0)      289 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/survey.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/
+-rw-r--r--   0 root         (0) root         (0)    34746 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/2.3.2.html
+-rw-r--r--   0 root         (0) root         (0)     1214 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/all.html
+-rw-r--r--   0 root         (0) root         (0)    36075 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/glyphicons.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/height/
+-rw-r--r--   0 root         (0) root         (0)     2288 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/height/4.4.0.html
+-rw-r--r--   0 root         (0) root         (0)     2288 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/height/4.5.0.html
+-rw-r--r--   0 root         (0) root         (0)     2281 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/height/current.html
+-rw-r--r--   0 root         (0) root         (0)    36410 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/index.html
+-rw-r--r--   0 root         (0) root         (0)     1065 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/thanks.html
+-rw-r--r--   0 root         (0) root         (0)     1928 2018-01-28 22:51:54.000000 platypush-0.9.6/platypush/backend/http/static/font-awesome/src/whats-new.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/js/
+-rw-r--r--   0 root         (0) root         (0)    11307 2019-02-21 19:12:43.000000 platypush-0.9.6/platypush/backend/http/static/js/application.js
+-rw-r--r--   0 root         (0) root         (0)     1227 2019-02-06 08:47:00.000000 platypush-0.9.6/platypush/backend/http/static/js/assistant.google.js
+-rw-r--r--   0 root         (0) root         (0)     1473 2018-06-13 18:44:07.000000 platypush-0.9.6/platypush/backend/http/static/js/dashboard.js
+-rw-r--r--   0 root         (0) root         (0)     1668 2018-08-22 18:21:52.000000 platypush-0.9.6/platypush/backend/http/static/js/gpio.js
+-rw-r--r--   0 root         (0) root         (0)     1484 2018-06-11 22:33:06.000000 platypush-0.9.6/platypush/backend/http/static/js/gpio.sensor.mcp3008.js
+-rw-r--r--   0 root         (0) root         (0)     3746 2018-04-17 21:10:49.000000 platypush-0.9.6/platypush/backend/http/static/js/gpio.zeroborg.js
+-rw-r--r--   0 root         (0) root         (0)    86927 2018-01-28 17:47:10.000000 platypush-0.9.6/platypush/backend/http/static/js/jquery-3.3.1.min.js
+-rw-r--r--   0 root         (0) root         (0)   253668 2018-06-18 22:37:33.000000 platypush-0.9.6/platypush/backend/http/static/js/jquery-ui-1.12.1.min.js
+-rw-r--r--   0 root         (0) root         (0)    27459 2019-01-09 14:04:43.000000 platypush-0.9.6/platypush/backend/http/static/js/light.hue.js
+-rw-r--r--   0 root         (0) root         (0)     6938 2018-06-13 18:40:49.000000 platypush-0.9.6/platypush/backend/http/static/js/map.js
+-rw-r--r--   0 root         (0) root         (0)    27078 2019-02-19 22:14:11.000000 platypush-0.9.6/platypush/backend/http/static/js/media.js
+-rw-r--r--   0 root         (0) root         (0)    30314 2019-02-13 17:01:39.000000 platypush-0.9.6/platypush/backend/http/static/js/music.mpd.js
+-rw-r--r--   0 root         (0) root         (0)    20238 2019-01-13 22:42:05.000000 platypush-0.9.6/platypush/backend/http/static/js/music.snapcast.js
+-rw-r--r--   0 root         (0) root         (0)      697 2018-05-04 11:06:18.000000 platypush-0.9.6/platypush/backend/http/static/js/pushbullet.js
+-rw-r--r--   0 root         (0) root         (0)      370 2018-01-28 19:40:20.000000 platypush-0.9.6/platypush/backend/http/static/js/skeleton-tabs.js
+-rw-r--r--   0 root         (0) root         (0)      837 2018-05-11 18:40:45.000000 platypush-0.9.6/platypush/backend/http/static/js/switch.switchbot.js
+-rw-r--r--   0 root         (0) root         (0)     2455 2018-06-26 20:58:28.000000 platypush-0.9.6/platypush/backend/http/static/js/switch.tplink.js
+-rw-r--r--   0 root         (0) root         (0)     2365 2018-06-26 20:01:59.000000 platypush-0.9.6/platypush/backend/http/static/js/switch.wemo.js
+-rw-r--r--   0 root         (0) root         (0)      793 2018-10-14 15:16:40.000000 platypush-0.9.6/platypush/backend/http/static/js/tts.google.js
+-rw-r--r--   0 root         (0) root         (0)      786 2018-04-17 21:10:49.000000 platypush-0.9.6/platypush/backend/http/static/js/tts.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/js/widgets/
+-rw-r--r--   0 root         (0) root         (0)     2854 2018-06-06 00:26:28.000000 platypush-0.9.6/platypush/backend/http/static/js/widgets/calendar.js
+-rw-r--r--   0 root         (0) root         (0)     3328 2018-06-25 18:25:10.000000 platypush-0.9.6/platypush/backend/http/static/js/widgets/date-time-weather.js
+-rw-r--r--   0 root         (0) root         (0)     1680 2018-09-15 16:25:17.000000 platypush-0.9.6/platypush/backend/http/static/js/widgets/image-carousel.js
+-rw-r--r--   0 root         (0) root         (0)     6337 2019-02-13 16:46:56.000000 platypush-0.9.6/platypush/backend/http/static/js/widgets/music.js
+-rw-r--r--   0 root         (0) root         (0)     2440 2018-09-15 16:25:27.000000 platypush-0.9.6/platypush/backend/http/static/js/widgets/rss-news.js
+-rw-r--r--   0 root         (0) root         (0)    18950 2018-06-23 11:26:20.000000 platypush-0.9.6/platypush/backend/http/static/js/widgets/skycons.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/static/resources/
+-rw-r--r--   0 root         (0) root         (0)       91 2018-05-05 00:31:10.000000 platypush-0.9.6/platypush/backend/http/static/resources/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/templates/
+-rw-r--r--   0 root         (0) root         (0)     3379 2019-01-30 08:04:18.000000 platypush-0.9.6/platypush/backend/http/templates/dashboard.html
+-rw-r--r--   0 root         (0) root         (0)     3182 2019-01-07 18:02:03.000000 platypush-0.9.6/platypush/backend/http/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)     1926 2018-11-01 23:07:39.000000 platypush-0.9.6/platypush/backend/http/templates/map.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      208 2018-04-17 21:10:49.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/assistant.google.html
+-rw-r--r--   0 root         (0) root         (0)      229 2018-08-22 17:15:15.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/gpio.html
+-rw-r--r--   0 root         (0) root         (0)      262 2018-04-30 07:39:49.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/gpio.sensor.mcp3008.html
+-rw-r--r--   0 root         (0) root         (0)     1692 2018-04-12 18:07:28.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/gpio.zeroborg.html
+-rw-r--r--   0 root         (0) root         (0)     1093 2019-01-02 20:06:58.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/light.hue.html
+-rw-r--r--   0 root         (0) root         (0)     6099 2019-02-19 22:14:11.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/media.html
+-rw-r--r--   0 root         (0) root         (0)     6099 2019-02-19 22:14:11.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/media.mplayer.html
+-rw-r--r--   0 root         (0) root         (0)     6099 2019-02-19 22:14:11.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/media.mpv.html
+-rw-r--r--   0 root         (0) root         (0)     6099 2019-02-19 22:14:11.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/media.omxplayer.html
+-rw-r--r--   0 root         (0) root         (0)     6099 2019-02-19 22:14:11.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/media.vlc.html
+-rw-r--r--   0 root         (0) root         (0)     6563 2018-05-03 00:17:03.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/music.mpd.html
+-rw-r--r--   0 root         (0) root         (0)     7059 2019-01-10 15:50:01.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/music.snapcast.html
+-rw-r--r--   0 root         (0) root         (0)      262 2018-04-30 07:39:49.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/serial.html
+-rw-r--r--   0 root         (0) root         (0)      818 2018-05-11 18:40:45.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/switch.switchbot.html
+-rw-r--r--   0 root         (0) root         (0)      249 2018-06-26 19:50:39.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/switch.tplink.html
+-rw-r--r--   0 root         (0) root         (0)      243 2018-05-08 07:16:12.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/switch.wemo.html
+-rw-r--r--   0 root         (0) root         (0)      681 2018-10-14 15:23:35.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/tts.google.html
+-rw-r--r--   0 root         (0) root         (0)      668 2018-04-17 21:10:49.000000 platypush-0.9.6/platypush/backend/http/templates/plugins/tts.html
+-rw-r--r--   0 root         (0) root         (0)      637 2019-02-12 00:26:03.000000 platypush-0.9.6/platypush/backend/http/templates/webplayer.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/http/templates/widgets/
+-rw-r--r--   0 root         (0) root         (0)      466 2018-05-04 17:44:41.000000 platypush-0.9.6/platypush/backend/http/templates/widgets/calendar.html
+-rw-r--r--   0 root         (0) root         (0)     1094 2018-06-23 11:26:20.000000 platypush-0.9.6/platypush/backend/http/templates/widgets/date-time-weather.html
+-rw-r--r--   0 root         (0) root         (0)      548 2018-05-07 14:53:51.000000 platypush-0.9.6/platypush/backend/http/templates/widgets/image-carousel.html
+-rw-r--r--   0 root         (0) root         (0)     2032 2018-08-17 23:01:51.000000 platypush-0.9.6/platypush/backend/http/templates/widgets/music.html
+-rw-r--r--   0 root         (0) root         (0)      244 2018-05-05 12:53:08.000000 platypush-0.9.6/platypush/backend/http/templates/widgets/rss-news.html
+-rw-r--r--   0 root         (0) root         (0)     3126 2019-02-22 22:35:18.000000 platypush-0.9.6/platypush/backend/http/utils.py
+-rw-r--r--   0 root         (0) root         (0)      157 2019-02-24 11:03:46.000000 platypush-0.9.6/platypush/backend/http/uwsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/inotify/
+-rw-r--r--   0 root         (0) root         (0)     2834 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/inotify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/joystick.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/kafka/
+-rw-r--r--   0 root         (0) root         (0)     3187 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/kafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/light/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-01-09 14:13:02.000000 platypush-0.9.6/platypush/backend/light/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3349 2019-01-19 22:20:06.000000 platypush-0.9.6/platypush/backend/light/hue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/local/
+-rw-r--r--   0 root         (0) root         (0)     2487 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/local/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4383 2018-12-26 22:40:45.000000 platypush-0.9.6/platypush/backend/midi.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2019-01-27 00:22:12.000000 platypush-0.9.6/platypush/backend/mqtt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/music/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/music/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9008 2019-02-13 16:38:27.000000 platypush-0.9.6/platypush/backend/music/mopidy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/music/mpd/
+-rw-r--r--   0 root         (0) root         (0)     5091 2019-01-14 19:23:16.000000 platypush-0.9.6/platypush/backend/music/mpd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8605 2019-02-16 19:21:01.000000 platypush-0.9.6/platypush/backend/music/snapcast.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/pushbullet/
+-rw-r--r--   0 root         (0) root         (0)     4822 2018-12-27 21:44:03.000000 platypush-0.9.6/platypush/backend/pushbullet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2018-12-26 14:24:49.000000 platypush-0.9.6/platypush/backend/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/scard/
+-rw-r--r--   0 root         (0) root         (0)     2996 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/scard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/sensor/
+-rw-r--r--   0 root         (0) root         (0)     3740 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/sensor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      602 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/sensor/accelerometer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/sensor/distance/
+-rw-r--r--   0 root         (0) root         (0)      547 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/sensor/distance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/sensor/ir/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/sensor/ir/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/sensor/ir/zeroborg/
+-rw-r--r--   0 root         (0) root         (0)     2162 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/sensor/ir/zeroborg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/sensor/ir/zeroborg/scan.py
+-rw-r--r--   0 root         (0) root         (0)     9316 2018-12-27 18:57:06.000000 platypush-0.9.6/platypush/backend/sensor/leap.py
+-rw-r--r--   0 root         (0) root         (0)      653 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/sensor/mcp3008.py
+-rw-r--r--   0 root         (0) root         (0)      575 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/sensor/serial.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2019-01-13 19:39:51.000000 platypush-0.9.6/platypush/backend/tcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/backend/weather/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-10-25 17:40:10.000000 platypush-0.9.6/platypush/backend/weather/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2018-10-25 18:46:34.000000 platypush-0.9.6/platypush/backend/weather/forecast.py
+-rw-r--r--   0 root         (0) root         (0)     5858 2019-02-22 18:14:46.000000 platypush-0.9.6/platypush/backend/websocket.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2018-12-02 22:47:41.000000 platypush-0.9.6/platypush/backend/wiimote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/bus/
+-rw-r--r--   0 root         (0) root         (0)     2187 2019-02-23 22:57:15.000000 platypush-0.9.6/platypush/bus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1379 2019-02-22 17:24:05.000000 platypush-0.9.6/platypush/bus/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/config/
+-rw-r--r--   0 root         (0) root         (0)     8982 2018-12-30 19:11:30.000000 platypush-0.9.6/platypush/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/context/
+-rw-r--r--   0 root         (0) root         (0)     3773 2019-02-13 16:25:56.000000 platypush-0.9.6/platypush/context/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/cron/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-01-15 21:37:01.000000 platypush-0.9.6/platypush/cron/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2018-09-26 23:51:10.000000 platypush-0.9.6/platypush/cron/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/event/
+-rw-r--r--   0 root         (0) root         (0)        0 2017-12-24 00:15:01.000000 platypush-0.9.6/platypush/event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5418 2019-01-13 19:40:13.000000 platypush-0.9.6/platypush/event/hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/event/processor/
+-rw-r--r--   0 root         (0) root         (0)     1987 2018-11-02 16:48:45.000000 platypush-0.9.6/platypush/event/processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      407 2019-01-26 23:54:07.000000 platypush-0.9.6/platypush/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/
+-rw-r--r--   0 root         (0) root         (0)     2101 2018-10-26 09:06:55.000000 platypush-0.9.6/platypush/message/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/
+-rw-r--r--   0 root         (0) root         (0)     8544 2018-10-09 23:00:30.000000 platypush-0.9.6/platypush/message/event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      745 2019-01-11 23:31:00.000000 platypush-0.9.6/platypush/message/event/adafruit.py
+-rw-r--r--   0 root         (0) root         (0)      487 2018-09-24 20:07:13.000000 platypush-0.9.6/platypush/message/event/application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/assistant/
+-rw-r--r--   0 root         (0) root         (0)     4466 2019-01-19 00:47:05.000000 platypush-0.9.6/platypush/message/event/assistant/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/button/
+-rw-r--r--   0 root         (0) root         (0)        0 2017-12-24 12:21:59.000000 platypush-0.9.6/platypush/message/event/button/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/button/flic/
+-rw-r--r--   0 root         (0) root         (0)     1586 2018-07-25 00:14:43.000000 platypush-0.9.6/platypush/message/event/button/flic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      471 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/geo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/http/
+-rw-r--r--   0 root         (0) root         (0)      500 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/http/ota/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-01-11 17:40:02.000000 platypush-0.9.6/platypush/message/event/http/ota/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/http/ota/booking/
+-rw-r--r--   0 root         (0) root         (0)      251 2018-01-16 18:56:14.000000 platypush-0.9.6/platypush/message/event/http/ota/booking/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      951 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/http/rss.py
+-rw-r--r--   0 root         (0) root         (0)      566 2018-09-18 16:58:23.000000 platypush-0.9.6/platypush/message/event/joystick.py
+-rw-r--r--   0 root         (0) root         (0)      414 2018-07-27 23:55:19.000000 platypush-0.9.6/platypush/message/event/kafka.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2019-01-09 08:10:33.000000 platypush-0.9.6/platypush/message/event/light.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2019-02-20 22:39:23.000000 platypush-0.9.6/platypush/message/event/media.py
+-rw-r--r--   0 root         (0) root         (0)      513 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/midi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/music/
+-rw-r--r--   0 root         (0) root         (0)     3716 2019-02-12 18:17:07.000000 platypush-0.9.6/platypush/message/event/music/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2019-01-06 17:47:47.000000 platypush-0.9.6/platypush/message/event/music/snapcast.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/path/
+-rw-r--r--   0 root         (0) root         (0)     1862 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/path/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      366 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/ping.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2018-01-06 23:39:45.000000 platypush-0.9.6/platypush/message/event/pushbullet.py
+-rw-r--r--   0 root         (0) root         (0)      934 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/scard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/sensor/
+-rw-r--r--   0 root         (0) root         (0)     1073 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/sensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/sensor/ir/
+-rw-r--r--   0 root         (0) root         (0)      862 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/sensor/ir/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/sensor/leap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/sensor/light/
+-rw-r--r--   0 root         (0) root         (0)      433 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/sensor/light/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/serial/
+-rw-r--r--   0 root         (0) root         (0)      495 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/serial/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2019-02-15 18:06:05.000000 platypush-0.9.6/platypush/message/event/sound.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2019-02-04 20:08:26.000000 platypush-0.9.6/platypush/message/event/torrent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/video/
+-rw-r--r--   0 root         (0) root         (0)     1295 2019-02-01 08:34:50.000000 platypush-0.9.6/platypush/message/event/video/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      259 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/weather.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/event/web/
+-rw-r--r--   0 root         (0) root         (0)      875 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      391 2018-07-09 20:38:08.000000 platypush-0.9.6/platypush/message/event/web/widget.py
+-rw-r--r--   0 root         (0) root         (0)      619 2018-12-01 17:46:32.000000 platypush-0.9.6/platypush/message/event/wiimote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/request/
+-rw-r--r--   0 root         (0) root         (0)     9590 2019-02-23 20:07:05.000000 platypush-0.9.6/platypush/message/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/message/response/
+-rw-r--r--   0 root         (0) root         (0)     2254 2018-10-09 23:00:30.000000 platypush-0.9.6/platypush/message/response/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/platydock/
+-rwxr-xr-x   0 root         (0) root         (0)     9922 2018-12-19 23:39:16.000000 platypush-0.9.6/platypush/platydock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       67 2018-12-19 01:19:59.000000 platypush-0.9.6/platypush/platydock/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/
+-rw-r--r--   0 root         (0) root         (0)     1673 2019-01-13 19:07:02.000000 platypush-0.9.6/platypush/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/adafruit/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-07-24 07:16:52.000000 platypush-0.9.6/platypush/plugins/adafruit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7999 2019-01-12 21:42:14.000000 platypush-0.9.6/platypush/plugins/adafruit/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/assistant/
+-rw-r--r--   0 root         (0) root         (0)        0 2017-12-28 08:59:41.000000 platypush-0.9.6/platypush/plugins/assistant/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/assistant/google/
+-rw-r--r--   0 root         (0) root         (0)      951 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/assistant/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      982 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/assistant/google/pushtotalk.py
+-rw-r--r--   0 root         (0) root         (0)     8214 2018-12-28 08:37:16.000000 platypush-0.9.6/platypush/plugins/autoremote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/calendar/
+-rw-r--r--   0 root         (0) root         (0)     3779 2018-12-20 15:39:13.000000 platypush-0.9.6/platypush/plugins/calendar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3791 2018-12-21 17:37:37.000000 platypush-0.9.6/platypush/plugins/calendar/ical.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/camera/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-06-13 21:37:41.000000 platypush-0.9.6/platypush/plugins/camera/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/camera/pi.py
+-rw-r--r--   0 root         (0) root         (0)      648 2018-07-23 22:33:17.000000 platypush-0.9.6/platypush/plugins/clipboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/db/
+-rw-r--r--   0 root         (0) root         (0)    11944 2018-07-15 21:39:10.000000 platypush-0.9.6/platypush/plugins/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2018-11-02 16:48:45.000000 platypush-0.9.6/platypush/plugins/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/google/
+-rw-r--r--   0 root         (0) root         (0)     1570 2018-06-25 22:36:19.000000 platypush-0.9.6/platypush/plugins/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/google/calendar.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2018-05-04 17:13:44.000000 platypush-0.9.6/platypush/plugins/google/credentials.py
+-rw-r--r--   0 root         (0) root         (0)     3570 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/google/mail.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2018-07-27 23:55:18.000000 platypush-0.9.6/platypush/plugins/google/maps.py
+-rw-r--r--   0 root         (0) root         (0)     2770 2018-12-15 00:18:48.000000 platypush-0.9.6/platypush/plugins/google/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/gpio/
+-rw-r--r--   0 root         (0) root         (0)     3222 2018-08-22 17:20:10.000000 platypush-0.9.6/platypush/plugins/gpio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/
+-rw-r--r--   0 root         (0) root         (0)      998 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/accelerometer/
+-rw-r--r--   0 root         (0) root         (0)     2039 2018-09-06 00:46:30.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/accelerometer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/accelerometer/lib/
+-rw-r--r--   0 root         (0) root         (0)    11346 2018-09-06 00:11:41.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/accelerometer/lib/LIS3DH.py
+-rw-r--r--   0 root         (0) root         (0)        0 2018-09-06 00:23:41.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/accelerometer/lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/distance/
+-rw-r--r--   0 root         (0) root         (0)     2758 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/distance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/mcp3008/
+-rw-r--r--   0 root         (0) root         (0)     6074 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/gpio/sensor/mcp3008/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/gpio/zeroborg/
+-rw-r--r--   0 root         (0) root         (0)     8024 2018-08-22 00:03:30.000000 platypush-0.9.6/platypush/plugins/gpio/zeroborg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/gpio/zeroborg/lib/
+-rw-r--r--   0 root         (0) root         (0)    29838 2018-03-27 21:13:47.000000 platypush-0.9.6/platypush/plugins/gpio/zeroborg/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2018-12-28 08:54:12.000000 platypush-0.9.6/platypush/plugins/homeseer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/http/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-01-06 10:36:30.000000 platypush-0.9.6/platypush/plugins/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/http/request/
+-rw-r--r--   0 root         (0) root         (0)     4800 2018-07-19 18:05:08.000000 platypush-0.9.6/platypush/plugins/http/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/http/request/ota/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-01-12 14:19:31.000000 platypush-0.9.6/platypush/plugins/http/request/ota/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/http/request/ota/booking/
+-rw-r--r--   0 root         (0) root         (0)     1178 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/http/request/ota/booking/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      506 2019-01-09 17:21:13.000000 platypush-0.9.6/platypush/plugins/http/request/rss.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2018-07-25 00:14:43.000000 platypush-0.9.6/platypush/plugins/ifttt.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2018-07-27 23:55:19.000000 platypush-0.9.6/platypush/plugins/kafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/lastfm/
+-rw-r--r--   0 root         (0) root         (0)     2089 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/lastfm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/light/
+-rw-r--r--   0 root         (0) root         (0)      607 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/light/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/light/hue/
+-rw-r--r--   0 root         (0) root         (0)    25205 2019-02-09 00:53:17.000000 platypush-0.9.6/platypush/plugins/light/hue/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      960 2018-07-18 22:02:30.000000 platypush-0.9.6/platypush/plugins/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/media/
+-rw-r--r--   0 root         (0) root         (0)    16335 2019-02-20 22:39:23.000000 platypush-0.9.6/platypush/plugins/media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15801 2019-02-12 10:12:58.000000 platypush-0.9.6/platypush/plugins/media/chromecast.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2019-02-21 00:49:37.000000 platypush-0.9.6/platypush/plugins/media/ctrl.py
+-rw-r--r--   0 root         (0) root         (0)    12594 2019-02-05 09:31:17.000000 platypush-0.9.6/platypush/plugins/media/kodi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/media/lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-11-12 23:52:50.000000 platypush-0.9.6/platypush/plugins/media/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2018-11-13 00:23:26.000000 platypush-0.9.6/platypush/plugins/media/lib/plexcast.py
+-rw-r--r--   0 root         (0) root         (0)    15919 2019-02-20 22:39:23.000000 platypush-0.9.6/platypush/plugins/media/mplayer.py
+-rw-r--r--   0 root         (0) root         (0)    12471 2019-02-20 22:39:23.000000 platypush-0.9.6/platypush/plugins/media/mpv.py
+-rw-r--r--   0 root         (0) root         (0)     9500 2019-02-10 20:09:44.000000 platypush-0.9.6/platypush/plugins/media/omxplayer.py
+-rw-r--r--   0 root         (0) root         (0)    12232 2018-11-13 00:28:24.000000 platypush-0.9.6/platypush/plugins/media/plex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/media/search/
+-rw-r--r--   0 root         (0) root         (0)      606 2019-02-17 17:58:24.000000 platypush-0.9.6/platypush/plugins/media/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10500 2019-02-18 23:31:28.000000 platypush-0.9.6/platypush/plugins/media/search/local.py
+-rw-r--r--   0 root         (0) root         (0)      450 2019-02-17 18:00:01.000000 platypush-0.9.6/platypush/plugins/media/search/torrent.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2019-02-17 23:25:26.000000 platypush-0.9.6/platypush/plugins/media/search/youtube.py
+-rw-r--r--   0 root         (0) root         (0)     6791 2019-02-11 21:16:02.000000 platypush-0.9.6/platypush/plugins/media/subtitles.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2019-02-21 18:24:47.000000 platypush-0.9.6/platypush/plugins/media/vlc.py
+-rw-r--r--   0 root         (0) root         (0)    15164 2019-02-20 22:39:23.000000 platypush-0.9.6/platypush/plugins/media/webtorrent.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2018-12-26 22:39:47.000000 platypush-0.9.6/platypush/plugins/midi.py
+-rw-r--r--   0 root         (0) root         (0)     6343 2018-11-02 16:48:45.000000 platypush-0.9.6/platypush/plugins/mqtt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/music/
+-rw-r--r--   0 root         (0) root         (0)      910 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/music/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/music/mpd/
+-rw-r--r--   0 root         (0) root         (0)    15903 2019-02-13 22:49:54.000000 platypush-0.9.6/platypush/plugins/music/mpd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19276 2019-02-07 13:27:14.000000 platypush-0.9.6/platypush/plugins/music/snapcast.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2018-12-27 00:54:31.000000 platypush-0.9.6/platypush/plugins/pushbullet.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2019-01-06 21:56:45.000000 platypush-0.9.6/platypush/plugins/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/serial/
+-rw-r--r--   0 root         (0) root         (0)     8264 2018-12-16 22:12:07.000000 platypush-0.9.6/platypush/plugins/serial/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/shell/
+-rw-r--r--   0 root         (0) root         (0)     1105 2019-01-13 18:03:29.000000 platypush-0.9.6/platypush/plugins/shell/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/sound/
+-rw-r--r--   0 root         (0) root         (0)    33431 2019-02-15 18:06:48.000000 platypush-0.9.6/platypush/plugins/sound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11998 2018-12-27 23:24:14.000000 platypush-0.9.6/platypush/plugins/sound/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/switch/
+-rw-r--r--   0 root         (0) root         (0)      705 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/switch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/switch/switchbot/
+-rw-r--r--   0 root         (0) root         (0)     6350 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/switch/switchbot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2018-05-08 13:48:22.000000 platypush-0.9.6/platypush/plugins/switch/switchbot/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/switch/tplink.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/switch/wemo/
+-rw-r--r--   0 root         (0) root         (0)     3342 2019-01-11 18:58:43.000000 platypush-0.9.6/platypush/plugins/switch/wemo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9139 2019-02-04 17:30:03.000000 platypush-0.9.6/platypush/plugins/torrent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/tts/
+-rw-r--r--   0 root         (0) root         (0)     1307 2018-07-15 15:28:17.000000 platypush-0.9.6/platypush/plugins/tts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2018-10-14 08:45:01.000000 platypush-0.9.6/platypush/plugins/tts/google.py
+-rw-r--r--   0 root         (0) root         (0)     9263 2019-01-14 21:06:56.000000 platypush-0.9.6/platypush/plugins/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2018-10-06 21:29:41.000000 platypush-0.9.6/platypush/plugins/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/video/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-02-01 08:33:56.000000 platypush-0.9.6/platypush/plugins/video/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/video/torrentcast.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/plugins/weather/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-05-05 22:42:46.000000 platypush-0.9.6/platypush/plugins/weather/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9721 2018-07-06 01:46:22.000000 platypush-0.9.6/platypush/plugins/weather/forecast.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2018-11-01 22:32:03.000000 platypush-0.9.6/platypush/plugins/websocket.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2018-12-01 17:35:56.000000 platypush-0.9.6/platypush/plugins/wiimote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/procedure/
+-rw-r--r--   0 root         (0) root         (0)     9649 2019-02-15 17:38:03.000000 platypush-0.9.6/platypush/procedure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/pusher/
+-rw-r--r--   0 root         (0) root         (0)     7645 2019-01-27 00:22:12.000000 platypush-0.9.6/platypush/pusher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       64 2018-01-04 15:09:40.000000 platypush-0.9.6/platypush/pusher/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush/utils/
+-rw-r--r--   0 root         (0) root         (0)     6859 2019-02-06 17:58:54.000000 platypush-0.9.6/platypush/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6845 2019-02-24 18:06:49.000000 platypush-0.9.6/platypush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)   107007 2019-02-24 18:06:50.000000 platypush-0.9.6/platypush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-02-24 18:06:49.000000 platypush-0.9.6/platypush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2019-02-24 18:06:49.000000 platypush-0.9.6/platypush.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2019-02-24 18:06:49.000000 platypush-0.9.6/platypush.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2019-02-24 18:06:49.000000 platypush-0.9.6/platypush.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2019-02-24 18:06:50.000000 platypush-0.9.6/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     4278 2019-02-24 18:03:51.000000 platypush-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-02-24 18:06:50.000000 platypush-0.9.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-01-04 09:37:29.000000 platypush-0.9.6/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      380 2018-01-02 18:37:08.000000 platypush-0.9.6/tests/context.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2018-09-26 23:44:15.000000 platypush-0.9.6/tests/test_event_parse.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2018-09-24 21:13:04.000000 platypush-0.9.6/tests/test_http.py
```

### Comparing `platypush-0.9.5/PKG-INFO` & `platypush-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platypush
-Version: 0.9.5
+Version: 0.9.6
 Summary: Platypush service
 Home-page: https://github.com/BlackLight/platypush
 Author: Fabio Manganiello
 Author-email: info@fabiomanganiello.com
 License: MIT
 Description: Platypush
         =========
@@ -73,36 +73,41 @@
         
 Keywords: pushbullet notifications automation
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >= 3
-Provides-Extra: Support for sound devices
-Provides-Extra: Support for Kodi plugin
-Provides-Extra: Support for MPD/Mopidy music server plugin
-Provides-Extra: Support for torrents download
-Provides-Extra: Support for PDF generation
-Provides-Extra: Support for Pushbullet backend
-Provides-Extra: Support for Apache Kafka backend
-Provides-Extra: Support for Plex plugin
-Provides-Extra: Support for OMXPlayer plugin
-Provides-Extra: Support for smart cards detection
-Provides-Extra: Support for YouTube in the OMXPlayer plugin
+Provides-Extra: Support for RSS feeds
 Provides-Extra: Support for database plugin
-Provides-Extra: Support for Google Assistant
+Provides-Extra: Support for custom hotword detection
+Provides-Extra: Support for torrents download
+Provides-Extra: Support for custom thread and process names
+Provides-Extra: Support for web media subtitles
+Provides-Extra: Support for text2speech plugin
 Provides-Extra: Support for MCP3008 analog-to-digital converter plugin
+Provides-Extra: Support for mopidy backend
+Provides-Extra: Support for Plex plugin
+Provides-Extra: Support for sound devices
 Provides-Extra: Support for GPIO pins access
-Provides-Extra: Support for RSS feeds
-Provides-Extra: Support for Belkin WeMo Switch plugin
-Provides-Extra: Support for Philips Hue plugin
 Provides-Extra: Support for joystick backend
-Provides-Extra: Support for Last.FM scrobbler plugin
-Provides-Extra: Support for custom hotword detection
+Provides-Extra: Support for Philips Hue plugin
+Provides-Extra: Support for external web server
+Provides-Extra: Support for Kodi plugin
 Provides-Extra: Support for HTTP backend
-Provides-Extra: Support for real-time MIDI events
+Provides-Extra: Support for OMXPlayer plugin
+Provides-Extra: Support for PDF generation
+Provides-Extra: Support for MPD/Mopidy music server plugin
+Provides-Extra: Support for most of the HTTP poll backends
+Provides-Extra: Support for mpv player plugin
 Provides-Extra: Support for the Google APIs
+Provides-Extra: Support for Apache Kafka backend
+Provides-Extra: Support for Google Assistant
 Provides-Extra: Support for ICal calendars
-Provides-Extra: Support for HTTP poll backend
+Provides-Extra: Support for smart cards detection
+Provides-Extra: Support for Last.FM scrobbler plugin
+Provides-Extra: Support for Belkin WeMo Switch plugin
+Provides-Extra: Support for Pushbullet backend
 Provides-Extra: Support for Chromecast plugin
-Provides-Extra: Support for most of the HTTP poll backends
-Provides-Extra: Support for text2speech plugin
+Provides-Extra: Support for YouTube in the OMXPlayer plugin
+Provides-Extra: Support for real-time MIDI events
+Provides-Extra: Support for HTTP poll backend
```

### Comparing `platypush-0.9.5/README.md` & `platypush-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/bin/platyvenv` & `platypush-0.9.6/bin/platyvenv`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/__init__.py` & `platypush-0.9.6/platypush/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .message.event.application import ApplicationStartedEvent, ApplicationStoppedEvent
 from .message.request import Request
 from .message.response import Response
 from .utils import set_thread_name
 
 
 __author__ = 'Fabio Manganiello <blacklight86@gmail.com>'
-__version__ = '0.9.5'
+__version__ = '0.9.6'
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 
 class Daemon:
     """ Main class for the Platypush daemon """
 
@@ -49,35 +49,42 @@
 
     # backend_name => backend_obj map
     backends = None
 
     # number of executions retries before a request fails
     n_tries = 2
 
-    def __init__(self, config_file=None, pidfile=None, requests_to_process=None):
+    def __init__(self, config_file=None, pidfile=None, requests_to_process=None,
+                 no_capture_stdout=False, no_capture_stderr=False):
         """
         Constructor
         Params:
             config_file -- Configuration file override (default: None)
             pidfile -- File where platypush will store its PID upon launch,
                        useful if you're planning to integrate the application
                        within a service or a launcher script (default: None)
             requests_to_process -- Exit after processing the specified number
                                    of requests (default: None, loop forever)
+            no_capture_stdout -- Set to true if you want to disable the stdout
+                                 capture by the logging system
+            no_capture_stderr -- Set to true if you want to disable the stderr
+                                 capture by the logging system
         """
 
         if pidfile:
             self.pidfile = pidfile
             with open(self.pidfile, 'w') as f:
                 f.write(str(os.getpid()))
 
         self.config_file = config_file
         Config.init(self.config_file)
         logging.basicConfig(**Config.get('logging'))
 
+        self.no_capture_stdout = no_capture_stdout
+        self.no_capture_stderr = no_capture_stderr
         self.event_processor = EventProcessor()
         self.requests_to_process = requests_to_process
         self.processed_requests = 0
 
     @classmethod
     def build_from_cmdline(cls, args):
         """
@@ -88,17 +95,29 @@
         parser = argparse.ArgumentParser()
         parser.add_argument('--config', '-c', dest='config', required=False,
                             default=None, help=cls.config_file.__doc__)
         parser.add_argument('--pidfile', '-P', dest='pidfile', required=False,
                             default=None, help="File where platypush will " +
                             "store its PID, useful if you're planning to " +
                             "integrate it in a service")
+        parser.add_argument('--no-capture-stdout', dest='no_capture_stdout',
+                            required=False, action='store_true',
+                            help="Set this flag if you have max stack depth " +
+                            "exceeded errors so stdout won't be captured by " +
+                            "the logging system")
+        parser.add_argument('--no-capture-stderr', dest='no_capture_stderr',
+                            required=False, action='store_true',
+                            help="Set this flag if you have max stack depth " +
+                            "exceeded errors so stderr won't be captured by " +
+                            "the logging system")
 
         opts, args = parser.parse_known_args(args)
-        return cls(config_file=opts.config, pidfile=opts.pidfile)
+        return cls(config_file=opts.config, pidfile=opts.pidfile,
+                   no_capture_stdout=opts.no_capture_stdout,
+                   no_capture_stderr=opts.no_capture_stderr)
 
     def on_message(self):
         """
         Default message handler
         """
 
         def _f(msg):
@@ -135,15 +154,21 @@
         for backend in self.backends.values():
             backend.stop()
         self.bus.stop()
 
 
     def start(self):
         """ Start the daemon """
+        if not self.no_capture_stdout:
+            sys.stdout = Logger(LOGGER.info)
+        if not self.no_capture_stderr:
+            sys.stderr = Logger(LOGGER.warning)
+
         set_thread_name('platypush')
+
         print('---- Starting platypush v.{}'.format(__version__))
 
         redis_conf = Config.get('backend.redis')
         if redis_conf:
             self.bus = RedisBus(on_message=self.on_message(),
                                 **redis_conf.get('redis_args', {}))
         else:
@@ -173,14 +198,12 @@
 
 
 def main():
     """
     Platypush daemon main
     """
 
-    sys.stdout = Logger(LOGGER.info)
-    sys.stderr = Logger(LOGGER.warning)
     app = Daemon.build_from_cmdline(sys.argv[1:])
     app.start()
 
 
 # vim:sw=4:ts=4:et:
```

### Comparing `platypush-0.9.5/platypush/backend/__init__.py` & `platypush-0.9.6/platypush/backend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         redis = redis.Redis(**redis_args)
         return redis
 
     def get_message_response(self, msg):
         try:
             redis = self._get_redis()
             response = redis.blpop(get_redis_queue_name_by_message(msg), timeout=60)
-            if response and response[1]:
+            if response and len(response) > 1:
                 response = Message.build(response[1])
             else:
                 response = None
 
             return response
         except Exception as e:
             self.logger.error('Error while processing response to {}: {}'.format(msg, str(e)))
```

### Comparing `platypush-0.9.5/platypush/backend/adafruit/io.py` & `platypush-0.9.6/platypush/backend/adafruit/io.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/assistant/google/__init__.py` & `platypush-0.9.6/platypush/backend/assistant/google/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 import os
 import subprocess
 import time
 
 import google.oauth2.credentials
 
 from google.assistant.library import Assistant
-from google.assistant.library.event import EventType
+from google.assistant.library.event import EventType, AlertType
 from google.assistant.library.file_helpers import existing_file
 
 from platypush.backend import Backend
 from platypush.message.event.assistant import \
     ConversationStartEvent, ConversationEndEvent, ConversationTimeoutEvent, \
-    ResponseEvent, NoResponseEvent, SpeechRecognizedEvent
+    ResponseEvent, NoResponseEvent, SpeechRecognizedEvent, AlarmStartedEvent, \
+    AlarmEndEvent, TimerStartedEvent, TimerEndEvent, AlertStartedEvent, \
+    AlertEndEvent
 
 
 class AssistantGoogleBackend(Backend):
     """
     Google Assistant backend.
 
     It listens for voice commands and post conversation events on the bus.
@@ -36,14 +38,22 @@
             when a conversation returned no response
         * :class:`platypush.message.event.assistant.ResponseEvent` \
             when the assistant is speaking a response
         * :class:`platypush.message.event.assistant.ConversationTimeoutEvent` \
             when a conversation times out
         * :class:`platypush.message.event.assistant.ConversationEndEvent` \
             when a new conversation ends
+        * :class:`platypush.message.event.assistant.AlarmStartedEvent` \
+            when an alarm starts
+        * :class:`platypush.message.event.assistant.AlarmEndEvent` \
+            when an alarm ends
+        * :class:`platypush.message.event.assistant.TimerStartedEvent` \
+            when a timer starts
+        * :class:`platypush.message.event.assistant.TimerEndEvent` \
+            when a timer ends
 
     Requires:
 
         * **google-assistant-library** (``pip install google-assistant-library``)
         * **google-assistant-sdk[samples]** (``pip install google-assistant-sdk[samples]``)
     """
 
@@ -65,41 +75,67 @@
         :type device_model_id: str
         """
 
         super().__init__(**kwargs)
         self.credentials_file = credentials_file
         self.device_model_id = device_model_id
         self.assistant = None
+        self._has_error = False
 
         with open(self.credentials_file, 'r') as f:
             self.credentials = google.oauth2.credentials.Credentials(
                 token=None,
                 **json.load(f))
 
         self.logger.info('Initialized Google Assistant backend')
 
     def _process_event(self, event):
         self.logger.info('Received assistant event: {}'.format(event))
+        self._has_error = False
 
         if event.type == EventType.ON_CONVERSATION_TURN_STARTED:
             self.bus.post(ConversationStartEvent())
         elif event.type == EventType.ON_CONVERSATION_TURN_FINISHED:
             if not event.args.get('with_follow_on_turn'):
                 self.bus.post(ConversationEndEvent())
         elif event.type == EventType.ON_CONVERSATION_TURN_TIMEOUT:
             self.bus.post(ConversationTimeoutEvent())
         elif event.type == EventType.ON_NO_RESPONSE:
             self.bus.post(NoResponseEvent())
         elif hasattr(EventType, 'ON_RENDER_RESPONSE') and \
             event.type == EventType.ON_RENDER_RESPONSE:
             self.bus.post(ResponseEvent(response_text=event.args.get('text')))
+        elif hasattr(EventType, 'ON_RESPONDING_STARTED') and \
+                event.type == EventType.ON_RESPONDING_STARTED and \
+                event.args.get('is_error_response', False) is True:
+            self.logger.warning('Assistant response error')
         elif event.type == EventType.ON_RECOGNIZING_SPEECH_FINISHED:
             phrase = event.args['text'].lower().strip()
             self.logger.info('Speech recognized: {}'.format(phrase))
             self.bus.post(SpeechRecognizedEvent(phrase=phrase))
+        elif event.type == EventType.ON_ALERT_STARTED:
+            if event.args.get('alert_type') == AlertType.ALARM:
+                self.bus.post(AlarmStartedEvent())
+            elif event.args.get('alert_type') == AlertType.TIMER:
+                self.bus.post(TimerStartedEvent())
+            else:
+                self.bus.post(AlertStartedEvent())
+        elif event.type == EventType.ON_ALERT_FINISHED:
+            if event.args.get('alert_type') == AlertType.ALARM:
+                self.bus.post(AlarmEndEvent())
+            elif event.args.get('alert_type') == AlertType.TIMER:
+                self.bus.post(TimerEndEvent())
+            else:
+                self.bus.post(AlertEndEvent())
+        elif event.type == EventType.ON_ASSISTANT_ERROR:
+            self._has_error = True
+            if event.args.get('is_fatal'):
+                self.logger.error('Fatal assistant error')
+            else:
+                self.logger.warning('Assistant error')
 
 
     def start_conversation(self):
         """ Starts an assistant conversation """
         if self.assistant:
             self.assistant.start_conversation()
 
@@ -109,14 +145,22 @@
         if self.assistant:
             self.assistant.stop_conversation()
 
 
     def run(self):
         super().run()
 
-        with Assistant(self.credentials, self.device_model_id) as assistant:
-            self.assistant = assistant
-            for event in assistant.start():
-                self._process_event(event)
+        while not self.should_stop():
+            self._has_error = False
+
+            with Assistant(self.credentials, self.device_model_id) as assistant:
+                self.assistant = assistant
+                for event in assistant.start():
+                    self._process_event(event)
+                    if self._has_error:
+                        self.logger.info('Restarting the assistant after ' +
+                                         'an unrecoverable error')
+                        time.sleep(5)
+                        continue
 
 
 # vim:sw=4:ts=4:et:
```

### Comparing `platypush-0.9.5/platypush/backend/assistant/google/pushtotalk.py` & `platypush-0.9.6/platypush/backend/assistant/google/pushtotalk.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/assistant/snowboy/__init__.py` & `platypush-0.9.6/platypush/backend/assistant/snowboy/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/button/flic/__init__.py` & `platypush-0.9.6/platypush/backend/button/flic/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/button/flic/fliclib/aioflic.py` & `platypush-0.9.6/platypush/backend/button/flic/fliclib/aioflic.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/button/flic/fliclib/fliclib.py` & `platypush-0.9.6/platypush/backend/button/flic/fliclib/fliclib.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/camera/pi.py` & `platypush-0.9.6/platypush/backend/camera/pi.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/poll/__init__.py` & `platypush-0.9.6/platypush/backend/http/poll/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/request/__init__.py` & `platypush-0.9.6/platypush/backend/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/request/ota/booking/__init__.py` & `platypush-0.9.6/platypush/backend/http/request/ota/booking/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/request/rss/__init__.py` & `platypush-0.9.6/platypush/backend/http/request/rss/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/application.css` & `platypush-0.9.6/platypush/backend/http/static/css/application.css`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,27 @@
             line-height: 38px;
         }
 
         .modal-body {
             padding: 2.5rem 2rem 1.5rem 2rem;
         }
 
+        .form-footer {
+            text-align: right;
+            margin-top: 2rem;
+            border-top: 1px solid #ddd;
+        }
+
+            .form-footer * > input[type=button],
+            .form-footer * > button {
+                margin-top: 2rem;
+                text-transform: uppercase;
+                font-size: 1.3rem;
+            }
+
 #date-time {
     text-align: right;
     padding-right: 30px;
 }
 
     #date-time > .date {
         color: #666;
```

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/gpio.css` & `platypush-0.9.6/platypush/backend/http/static/css/gpio.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/light.hue.css` & `platypush-0.9.6/platypush/backend/http/static/css/light.hue.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/music.mpd.css` & `platypush-0.9.6/platypush/backend/http/static/css/music.mpd.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/music.snapcast.css` & `platypush-0.9.6/platypush/backend/http/static/css/music.snapcast.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/normalize.css` & `platypush-0.9.6/platypush/backend/http/static/css/normalize.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/skeleton.css` & `platypush-0.9.6/platypush/backend/http/static/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/switch.switchbot.css` & `platypush-0.9.6/platypush/backend/http/static/css/switch.switchbot.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/switch.tplink.css` & `platypush-0.9.6/platypush/backend/http/static/css/switch.tplink.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/switch.wemo.css` & `platypush-0.9.6/platypush/backend/http/static/css/switch.wemo.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/toggles.css` & `platypush-0.9.6/platypush/backend/http/static/css/toggles.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/widgets/calendar.css` & `platypush-0.9.6/platypush/backend/http/static/css/widgets/calendar.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/widgets/date-time-weather.css` & `platypush-0.9.6/platypush/backend/http/static/css/widgets/date-time-weather.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/widgets/image-carousel.css` & `platypush-0.9.6/platypush/backend/http/static/css/widgets/image-carousel.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/widgets/music.css` & `platypush-0.9.6/platypush/backend/http/static/css/widgets/music.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/css/widgets/rss-news.css` & `platypush-0.9.6/platypush/backend/http/static/css/widgets/rss-news.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/CONTRIBUTING.md` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/Gemfile.lock` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/README.md` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/README.md`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/_config.yml` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/_config.yml`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/composer.json` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/composer.json`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/css/font-awesome.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/css/font-awesome.css.map` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/css/font-awesome.min.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/FontAwesome.otf` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.eot` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.svg` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.ttf` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.woff` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.woff2` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/less/animated.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/less/animated.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/less/bordered-pulled.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/less/bordered-pulled.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/less/icons.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/less/icons.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/less/mixins.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/less/mixins.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/less/path.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/less/path.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/less/rotated-flipped.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/less/rotated-flipped.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/less/variables.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/less/variables.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/package.json` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/package.json`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_animated.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_animated.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_bordered-pulled.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_bordered-pulled.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_icons.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_icons.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_mixins.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_path.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_path.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_rotated-flipped.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_rotated-flipped.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/scss/_variables.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/Makefile` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/prettify.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/prettify.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/pygments.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/pygments.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/site.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/css/site.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome-ie7.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome-ie7.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome-ie7.min.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome-ie7.min.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome.min.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/FontAwesome.otf` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.eot` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.svg` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.ttf` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.woff` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/font/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/bootstrap.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/bootstrap.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/core.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/core.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/extras.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/extras.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/font-awesome-ie7.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/font-awesome-ie7.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/font-awesome.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/font-awesome.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/icons.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/icons.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/mixins.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/mixins.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/path.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/path.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/variables.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/less/variables.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_bootstrap.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_bootstrap.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_core.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_core.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_extras.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_extras.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_icons.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_icons.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_mixins.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_path.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_path.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_variables.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/font-awesome-ie7.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/font-awesome-ie7.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/font-awesome.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome/scss/font-awesome.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome.zip` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/font-awesome.zip`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/ico/favicon.ico` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/contribution-sample.png` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/contribution-sample.png`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/fort_awesome.jpg` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/fort_awesome.jpg`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/glyphicons-halflings-white.png` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/glyphicons-halflings.png` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/icon-flag.pdf` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/img/icon-flag.pdf`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/ZeroClipboard-1.1.7.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/ZeroClipboard-1.1.7.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/ZeroClipboard-1.1.7.swf` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/ZeroClipboard-1.1.7.swf`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/backbone.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/backbone.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/bootstrap-2.3.1.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/bootstrap-2.3.1.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/bootstrap-222.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/bootstrap-222.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/jquery-1.7.1.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/jquery-1.7.1.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/prettify.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/prettify.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/site.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/site.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/underscore.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/js/underscore.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/accordion.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/accordion.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/alerts.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/alerts.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/bootstrap.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/bootstrap.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/button-groups.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/button-groups.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/buttons.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/buttons.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/carousel.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/carousel.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/close.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/close.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/code.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/code.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/dropdowns.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/dropdowns.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/forms.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/forms.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/hero-unit.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/hero-unit.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/labels-badges.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/labels-badges.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/media.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/media.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/mixins.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/mixins.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/modals.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/modals.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/navbar.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/navbar.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/navs.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/navs.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/pager.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/pager.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/pagination.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/pagination.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/popovers.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/popovers.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/progress-bars.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/progress-bars.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/reset.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/reset.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-1200px-min.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-1200px-min.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-767px-max.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-767px-max.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-navbar.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-navbar.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-utilities.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive-utilities.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/responsive.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/scaffolding.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/scaffolding.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/sprites.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/sprites.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/tables.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/tables.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/thumbnails.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/thumbnails.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/tooltip.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/tooltip.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/type.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/type.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/variables.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/variables.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/wells.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/bootstrap-2.3.2/wells.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/lazy.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/lazy.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/mixins.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/mixins.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-1200px-min.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-1200px-min.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-767px-max.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-767px-max.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-768px-979px.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive-768px-979px.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/responsive.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/site.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/site.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/variables.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/assets/less/variables.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/cheatsheet/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/cheatsheet/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/community/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/community/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/examples/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/examples/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/get-started/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/get-started/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adjust/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adjust/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adn/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/adn/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-center/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-center/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-justify/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-justify/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/align-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ambulance/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ambulance/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/anchor/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/anchor/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/android/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/android/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/angle-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/apple/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/apple/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/archive/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/archive/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/arrow-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/asterisk/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/asterisk/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/backward/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/backward/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ban-circle/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ban-circle/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bar-chart/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bar-chart/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/barcode/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/barcode/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beaker/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beaker/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beer/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/beer/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bell-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bitbucket-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bold/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bold/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bolt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bolt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/book/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/book/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark-empty/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bookmark-empty/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/briefcase/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/briefcase/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/btc/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/btc/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bug/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bug/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/building/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/building/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullhorn/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullhorn/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullseye/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/bullseye/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar-empty/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/calendar-empty/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera-retro/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/camera-retro/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/caret-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/certificate/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/certificate/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-empty/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-empty/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-minus/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-minus/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/check-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-sign-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/chevron-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-arrow-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-blank/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/circle-blank/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-download/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-download/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-upload/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cloud-upload/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cny/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cny/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code-fork/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/code-fork/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/coffee/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/coffee/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cog/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cog/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cogs/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cogs/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-top/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/collapse-top/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/columns/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/columns/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comment-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/comments-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/compass/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/compass/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/copy/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/copy/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/credit-card/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/credit-card/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/crop/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/crop/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/css3/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/css3/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cut/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/cut/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dashboard/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/desktop/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/desktop/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/double-angle-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/download-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dribbble/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dribbble/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dropbox/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/dropbox/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/edit-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eject/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eject/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-horizontal/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-horizontal/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-vertical/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ellipsis-vertical/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/envelope-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eraser/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eraser/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eur/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eur/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exchange/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exchange/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/exclamation-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/expand-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/external-link-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-close/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-close/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-open/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/eye-open/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facebook-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facetime-video/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/facetime-video/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-backward/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-backward/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-forward/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fast-forward/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/female/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/female/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fighter-jet/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fighter-jet/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/file-text-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/film/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/film/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/filter/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/filter/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire-extinguisher/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fire-extinguisher/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-checkered/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flag-checkered/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flickr/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/flickr/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-close-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/folder-open-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/font/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/font/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/food/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/food/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/forward/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/forward/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/foursquare/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/foursquare/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/frown/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/frown/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fullscreen/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/fullscreen/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gamepad/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gamepad/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gbp/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gbp/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gift/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gift/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/github-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gittip/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/gittip/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/glass/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/glass/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/globe/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/globe/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/google-plus-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/group/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/group/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/h-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/h-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hand-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hdd/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hdd/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/headphones/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/headphones/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart-empty/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/heart-empty/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/home/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/home/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hospital/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/hospital/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/html5/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/html5/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inbox/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inbox/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/indent-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/info-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inr/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/inr/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/instagram/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/instagram/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/italic/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/italic/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/jpy/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/jpy/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/key/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/key/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/keyboard/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/keyboard/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/krw/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/krw/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/laptop/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/laptop/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/leaf/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/leaf/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/legal/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/legal/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lemon/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lemon/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/level-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lightbulb/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lightbulb/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/link/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/link/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linkedin-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linux/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/linux/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ol/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ol/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ul/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/list-ul/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/location-arrow/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/location-arrow/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lock/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/lock/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/long-arrow-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magic/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magic/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magnet/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/magnet/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mail-reply-all/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mail-reply-all/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/male/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/male/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/map-marker/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/map-marker/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/maxcdn/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/maxcdn/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/medkit/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/medkit/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/meh/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/meh/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone-off/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/microphone-off/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/minus-sign-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mobile-phone/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/mobile-phone/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/money/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/money/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/moon/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/moon/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/move/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/move/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/music/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/music/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/off/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/off/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-circle/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-circle/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ok-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paper-clip/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paper-clip/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paste/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/paste/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pause/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pause/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pencil/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pencil/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/phone-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/picture/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/picture/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pinterest-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plane/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plane/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-circle/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-circle/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/play-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/plus-sign-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/print/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/print/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pushpin/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/pushpin/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/puzzle-piece/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/puzzle-piece/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/qrcode/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/qrcode/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/question-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-left/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-left/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-right/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/quote-right/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/random/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/random/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/refresh/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/refresh/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-circle/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-circle/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/remove-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/renren/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/renren/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reorder/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reorder/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/repeat/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/repeat/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply-all/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/reply-all/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-full/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-full/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-horizontal/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-horizontal/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-small/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-small/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-vertical/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/resize-vertical/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/retweet/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/retweet/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/road/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/road/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rocket/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rocket/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/rss-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/save/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/save/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/screenshot/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/screenshot/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/search/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/search/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/share-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shield/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shield/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shopping-cart/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/shopping-cart/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sign-blank/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sign-blank/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signal/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signal/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signin/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signin/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signout/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/signout/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sitemap/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sitemap/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/skype/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/skype/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/smile/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/smile/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-alphabet-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-attributes-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-by-order-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sort-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/spinner/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/spinner/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stackexchange/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stackexchange/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-empty/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-empty/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half-empty/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/star-half-empty/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-backward/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-backward/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-forward/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/step-forward/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stethoscope/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stethoscope/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stop/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/stop/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/strikethrough/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/strikethrough/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/subscript/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/subscript/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/suitcase/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/suitcase/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sun/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/sun/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/superscript/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/superscript/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/table/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/table/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tablet/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tablet/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tag/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tag/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tags/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tags/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tasks/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tasks/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/terminal/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/terminal/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-height/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-height/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-width/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/text-width/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-large/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-large/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-list/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/th-list/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-down-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/thumbs-up-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ticket/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/ticket/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/time/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/time/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tint/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tint/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trash/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trash/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trello/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trello/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trophy/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/trophy/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/truck/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/truck/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/tumblr-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/twitter-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/umbrella/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/umbrella/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/underline/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/underline/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/undo/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/undo/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlink/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlink/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/unlock-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload-alt/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/upload-alt/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/usd/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/usd/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user-md/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/user-md/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/vk/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/vk/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-down/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-down/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-off/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-off/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-up/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/volume-up/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/warning-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/warning-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/weibo/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/weibo/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/windows/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/windows/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/wrench/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/wrench/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/xing-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-play/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-play/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-sign/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/youtube-sign/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-in/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-in/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-out/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icon/zoom-out/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icons/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icons/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/icons.yml` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/icons.yml`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/license/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/license/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/test/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/test/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/3.2.1/whats-new/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/3.2.1/whats-new/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/Makefile` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/Makefile`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/README.md-nobuild` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/README.md-nobuild`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/accessibility-facdn.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/accessibility-facdn.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/accessibility-manual.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/accessibility-manual.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/background.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/background.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/cta-cdn-ally.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/cta-cdn-ally.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/accessibility/other.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/accessibility/other.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/getting-support.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/getting-support.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/reporting-bugs.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/reporting-bugs.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/requesting-new-icons.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/requesting-new-icons.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/community/submitting-pull-requests.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/community/submitting-pull-requests.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/accessible.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/accessible.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/animated.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/animated.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/basic.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/basic.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/bootstrap.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/bootstrap.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/bordered-pulled.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/bordered-pulled.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/custom.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/custom.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/fixed-width.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/fixed-width.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/larger.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/larger.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/list.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/list.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/rotated-flipped.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/rotated-flipped.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/examples/stacked.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/examples/stacked.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/footer.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/footer.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/accessibility.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/accessibility.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/brand.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/brand.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/chart.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/chart.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/currency.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/currency.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/directional.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/directional.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/file-type.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/file-type.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/form-control.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/form-control.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/gender.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/gender.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/hand.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/hand.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/medical.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/medical.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/new.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/new.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/payment.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/payment.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/spinner.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/spinner.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/text-editor.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/text-editor.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/transportation.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/transportation.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/video-player.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/video-player.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/icons/web-application.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/icons/web-application.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/jumbotron-carousel.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/jumbotron-carousel.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/modals/download.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/modals/download.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/modals/fa5.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/modals/fa5.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/navbar.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/navbar.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/new-features.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/new-features.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/new-naming.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/new-naming.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/new-upgrading.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/new-upgrading.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/newsletter-subscribe.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/newsletter-subscribe.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/camera-retro-tee.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/camera-retro-tee.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/classics-tee.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/classics-tee.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/cta-suggestions.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/cta-suggestions.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/fa-ther-tee.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/fa-ther-tee.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/green-logo-tee.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/green-logo-tee.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/old-skool-tee.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/old-skool-tee.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/rock-paper-scissors-lizard-spock-tee.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/rock-paper-scissors-lizard-spock-tee.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/space-shuttle-tee.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/space-shuttle-tee.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/products/white-logo-tee.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/products/white-logo-tee.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/stripe-social.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/stripe-social.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tell-me-thanks.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tell-me-thanks.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped-inside-anchor.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped-inside-anchor.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped-inside-btn.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/rotated-flipped-inside-btn.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked-inside-anchor.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked-inside-anchor.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/tests/stacked.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/thanks-to.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/thanks-to.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_includes/why.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_includes/why.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_layouts/base.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_layouts/base.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_layouts/icon.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_layouts/icon.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_layouts/survey.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_layouts/survey.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_plugins/flatten_icon_filters.rb` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_plugins/flatten_icon_filters.rb`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_plugins/icon_page_generator.rb` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_plugins/icon_page_generator.rb`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/_plugins/site.rb` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/_plugins/site.rb`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/accessibility.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/accessibility.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/css/prettify.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/css/prettify.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/css/pygments.css` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/css/pygments.css`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/FontAwesome.otf` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.eot` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.svg` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.ttf` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.woff` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.woff2` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/animated.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/animated.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/bordered-pulled.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/bordered-pulled.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/mixins.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/mixins.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/path.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/path.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/rotated-flipped.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/rotated-flipped.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/variables.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/less/variables.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_animated.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_animated.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_bordered-pulled.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_bordered-pulled.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_mixins.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_path.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_path.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_rotated-flipped.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_rotated-flipped.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_variables.scss` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/font-awesome/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/ico/favicon.ico` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/img/algolia.png` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/img/algolia.png`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/img/logo-themeisle.png` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/img/logo-themeisle.png`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/img/logo-wpbeginner.png` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/img/logo-wpbeginner.png`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/ZeroClipboard-1.1.7.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/ZeroClipboard-1.1.7.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/ZeroClipboard-1.1.7.swf` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/ZeroClipboard-1.1.7.swf`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/html5shiv.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/html5shiv.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/monetization.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/monetization.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/prettify.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/prettify.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/respond.min.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/search.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/search.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/js/site.js` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/js/site.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/.csscomb.json` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/.csscomb.json`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/alerts.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/alerts.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/badges.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/badges.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/bootstrap.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/bootstrap.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/breadcrumbs.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/breadcrumbs.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/button-groups.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/button-groups.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/buttons.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/buttons.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/carousel.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/carousel.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/close.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/close.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/code.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/code.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/component-animations.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/component-animations.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/dropdowns.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/dropdowns.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/forms.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/forms.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/glyphicons.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/glyphicons.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/grid.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/grid.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/input-groups.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/input-groups.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/jumbotron.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/jumbotron.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/labels.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/labels.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/list-group.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/list-group.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/media.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/media.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/buttons.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/buttons.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/clearfix.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/clearfix.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/forms.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/forms.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/gradients.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/gradients.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/grid-framework.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/grid-framework.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/grid.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/grid.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/hide-text.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/hide-text.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/image.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/image.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/list-group.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/list-group.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/panels.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/panels.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/table-row.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/table-row.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/vendor-prefixes.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins/vendor-prefixes.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/mixins.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/modals.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/modals.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/navbar.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/navbar.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/navs.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/navs.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/normalize.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/normalize.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/pager.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/pager.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/pagination.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/pagination.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/panels.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/panels.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/popovers.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/popovers.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/print.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/print.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/progress-bars.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/progress-bars.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/responsive-embed.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/responsive-embed.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/responsive-utilities.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/responsive-utilities.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/scaffolding.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/scaffolding.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/tables.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/tables.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/theme.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/theme.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/thumbnails.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/thumbnails.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/tooltip.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/tooltip.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/type.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/type.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/utilities.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/utilities.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/variables.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/variables.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/wells.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/bootstrap-3.3.5/wells.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/gandy-grid/grid.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/gandy-grid/grid.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/banner-ad.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/banner-ad.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/jumbotron.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/jumbotron.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/navbar.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/navbar.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/variables.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/bootstrap/variables.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/feature-list.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/feature-list.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/fontawesome-icon-list.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/fontawesome-icon-list.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/footer.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/footer.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/jumbotron-carousel.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/jumbotron-carousel.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/lazy.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/lazy.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-lg.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-lg.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-sm.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-sm.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-xs.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/responsive/screen-xs.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/search.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/search.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/store.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/store.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/textured-bg.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/textured-bg.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site/views.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site/views.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/assets/less/site.less` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/assets/less/site.less`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/cdn/error.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/cdn/error.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/cdn/success.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/cdn/success.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/cheatsheet.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/cheatsheet.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/community.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/community.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/examples.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/examples.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/get-started.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/get-started.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/icons.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/icons.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/icons.yml` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/icons.yml`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/license.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/license.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/store.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/store.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/2.3.2.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/2.3.2.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/all.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/all.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/glyphicons.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/glyphicons.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/height/4.4.0.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/height/4.4.0.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/height/4.5.0.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/height/4.5.0.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/height/current.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/height/current.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/test/index.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/test/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/thanks.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/thanks.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/font-awesome/src/whats-new.html` & `platypush-0.9.6/platypush/backend/http/static/font-awesome/src/whats-new.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/application.js` & `platypush-0.9.6/platypush/backend/http/static/js/application.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,14 @@
 $(document).ready(function() {
     var websocket,
         pendingConnection = false,
         openedWebsocket,
         dateTimeInterval,
         websocketTimeoutId,
+        modalFadingInTimeoutId,
         websocketReconnectMsecs = 30000,
         eventListeners = [];
 
     var initWebsocket = function() {
         try {
             url_prefix = window.has_ssl ? 'wss://' : 'ws://';
             websocket = new WebSocket(url_prefix + window.location.hostname + ':' + window.websocket_port);
@@ -27,14 +28,15 @@
             };
         };
 
         websocketTimeoutId = setTimeout(
             onWebsocketTimeout(websocket), websocketReconnectMsecs);
 
         websocket.onmessage = function(event) {
+            console.debug(event);
             for (var listener of eventListeners) {
                 data = event.data;
                 if (typeof event.data === 'string') {
                     data = JSON.parse(data);
                 }
 
                 listener(data);
@@ -193,53 +195,92 @@
             }).addClass('active');
 
         });
     };
 
     var initModalOpenBindings = function() {
         $('body').on('mouseup touchend', '[data-modal]', function(event) {
-            var $source = $(event.target);
+            var $source = $(this);
             var $modal = $($source.data('modal'));
             $modal.height($(document).height() + 2);
 
             var $container = $modal.find('.modal-container');
             var top = 40 + $(window).scrollTop();
             $container.css('margin-top', top + 'px');
 
+            modalFadingInTimeoutId = setTimeout(function() {
+                modalFadingInTimeoutId = undefined;
+            }, 100);
+
             $modal.fadeIn();
         });
     };
 
     var initModalCloseBindings = function() {
         $('body').on('mouseup touchend', '[data-dismiss-modal]', function(event) {
-            var $source = $(event.target);
+            var $source = $(this);
             var $modal = $($source.data('dismiss-modal'));
             $modal.fadeOut();
         });
 
         $('body').on('mouseup touchend', function(event) {
             var $source = $(event.target);
             if (!$source.parents('.modal').length &&
                 !$source.data('modal') &&
                 !$source.data('dismiss-modal')) {
-                $('.modal').filter(':visible').fadeOut();
+                if (!modalFadingInTimeoutId) {
+                    $('.modal').filter(':visible').fadeOut();
+                }
+            }
+        });
+    };
+
+    var initPanelOpenBindings = function() {
+        $('body').on('mouseup touchend', '[data-panel]', function(event) {
+            var $source = $(this);
+            var $panel = $($source.data('panel'));
+            setTimeout(() => {
+                $panel.show();
+            }, 200);
+        });
+    };
+
+    var initPanelCloseBindings = function() {
+        $('body').on('mouseup touchend', function(event) {
+            var $source = $(event.target);
+            if ($source.data('panel') || $source.parents('[data-panel]').length) {
+                var $panel = $source.data('panel') ? $($source.data('panel')) :
+                    $($source.parents('[data-panel]').data('panel'));
+                $panel.toggle();
+                return;
+            }
+
+            if (!$source.parents('.panel').length &&
+                !$source.data('panel')) {
+                $('.panel').filter(':visible').hide();
             }
         });
     };
 
     var initModals = function() {
         initModalOpenBindings();
         initModalCloseBindings();
     };
 
+    var initPanels = function() {
+        initPanelOpenBindings();
+        initPanelCloseBindings();
+    };
+
     var init = function() {
         initWebsocket();
         initElements();
         initDateTime();
         initModals();
+        initPanels();
     };
 
     window.registerEventListener = registerEventListener;
     init();
 });
 
 function execute(request, onSuccess, onError, onComplete) {
@@ -257,26 +298,47 @@
         },
         error: function(xhr, status, error) {
             if (onError) {
                 onError(xhr, status, error);
             }
         },
         success: function(response, status, xhr) {
+            if ('errors' in response && response.errors.length) {
+                if (onError) {
+                    onError(xhr, '500', response.errors);
+                }
+            }
+
             if (onSuccess) {
                 onSuccess(response, status, xhr);
             }
         },
         beforeSend: function(xhr) {
             if (window.token) {
                 xhr.setRequestHeader('X-Token', window.token);
             }
         },
     });
 }
 
+function run(request) {
+    request['type'] = 'request';
+    return new Promise((resolve, reject) => {
+        execute(request,
+            onSuccess = (response) => {
+                resolve(response);
+            },
+
+            onError = (xhr, status, error) => {
+                reject(xhr, status, error);
+            }
+        );
+    });
+}
+
 function createNotification(options) {
     var $notificationContainer = $('#notification-container');
     var $notification = $('<div></div>').addClass('notification');
     var $title = $('<div></div>').addClass('notification-title');
     var timeout = 'timeout' in options ? options.timeout : 10000;
 
     if ('title' in options) {
@@ -345,8 +407,15 @@
         }
     );
 
     $title.appendTo($notification);
     $body.appendTo($notification);
     $notification.prependTo($notificationContainer);
     $notification.fadeIn();
+}
+
+function showError(errorMessage) {
+    createNotification({
+        'icon': 'exclamation',
+        'text': errorMessage,
+    });
 }
```

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/assistant.google.js` & `platypush-0.9.6/platypush/backend/http/static/js/assistant.google.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,9 @@
 $(document).ready(function() {
     var onEvent = function(event) {
-        console.log(event);
-
         switch (event.args.type) {
             case 'platypush.message.event.assistant.ConversationStartEvent':
                 createNotification({
                     'text': 'Assistant listening',
                     'icon': 'microphone',
                 });
```

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/dashboard.js` & `platypush-0.9.6/platypush/backend/http/static/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/gpio.js` & `platypush-0.9.6/platypush/backend/http/static/js/gpio.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/gpio.sensor.mcp3008.js` & `platypush-0.9.6/platypush/backend/http/static/js/gpio.sensor.mcp3008.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/gpio.zeroborg.js` & `platypush-0.9.6/platypush/backend/http/static/js/gpio.zeroborg.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/jquery-3.3.1.min.js` & `platypush-0.9.6/platypush/backend/http/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/jquery-ui-1.12.1.min.js` & `platypush-0.9.6/platypush/backend/http/static/js/jquery-ui-1.12.1.min.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/light.hue.js` & `platypush-0.9.6/platypush/backend/http/static/js/light.hue.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/map.js` & `platypush-0.9.6/platypush/backend/http/static/js/map.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/music.mpd.js` & `platypush-0.9.6/platypush/backend/http/static/js/music.mpd.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,15 @@
 $(document).ready(function() {
     var seekInterval,
+        longPressTimeout,
         curPath = [],
         curTrackUpdateHandler,
         curTrackElapsed = {
-            timestamp: null,
-            elapsed: null,
+            timestamp: undefined,
+            elapsed: undefined,
         },
 
         $musicSearchForm = $('#music-search-form'),
         $musicSearchResults = $('#music-search-results'),
         $musicSearchResultsContainer = $('#music-search-results-container'),
         $musicSearchResultsForm = $('#music-search-results-form'),
         $musicResultsAddBtn = $('#music-results-add'),
@@ -41,112 +42,150 @@
         var $volumeCtrl = $('#volume-ctrl');
         var $trackSeeker = $('#track-seeker');
         var $randomBtn = $playbackControls.find('[data-action=random]');
         var $repeatBtn = $playbackControls.find('[data-action=repeat]');
         var elapsed;
         var length;
 
+        var timeToStr = (time) => {
+            if (typeof time === 'string') {
+                return time;
+            }
+
+            return parseInt(parseInt(time) / 60) + ':' +
+                (parseInt(time) % 60 < 10 ? '0' : '') + (parseInt(time) % 60);
+        };
+
         if (status) {
-            if (seekInterval) {
-                clearInterval(seekInterval);
+            if ('position' in status) {
+                elapsed = parseInt(status.position);
+                $trackSeeker.val(elapsed);
             }
 
             if ('time' in status) {
-                var time = status.time.split(':');
-                elapsed = parseInt(parseInt(time[0]) / 60) + ':' +
-                    (parseInt(time[0]) % 60 < 10 ? '0' : '') + (parseInt(time[0]) % 60);
+                if (seekInterval) {
+                    clearInterval(seekInterval);
+                    seekInterval = undefined;
+                }
 
-                if (time.length > 1) {
-                    length = parseInt(parseInt(time[1]) / 60) + ':' +
-                        (parseInt(time[1]) % 60 < 10 ? '0' : '') + (parseInt(time[1]) % 60);
+                if (typeof status.time === 'string' && status.time.indexOf(':') > -1) {
+                    // backend.music.mpd time format: "elapsed:total"
+                    [elapsed, length] = status.time.split(':');
+                    elapsed = parseInt(elapsed);
+                    length = parseInt(length);
+                } else {
+                    // backend.music.mopidy time format: integer with elapsed seconds
+                    length = parseInt(status.time);
                 }
+            }
 
-                $trackSeeker.val(parseInt(time[0]));
-                $trackSeeker.attr('max', parseInt(time[1]));
+            if (elapsed !== undefined) {
+                $trackSeeker.val(elapsed);
                 curTrackElapsed = {
-                    timestamp: new Date().getTime(),
-                    elapsed: parseInt(time[0]),
+                    'timestamp': new Date().getTime(),
+                    'elapsed': elapsed,
                 };
             }
 
-            switch (status.state.toLowerCase()) {
-                case 'stop':
-                    $playbackControls.find('button[data-action=pause]').hide();
-                    $playbackControls.find('button[data-action=play]').show();
-                    $curTrack.find('.artist').hide();
-                    $curTrack.find('.track').hide();
-                    $curTrack.find('.no-track').show();
-
-                    $trackSeeker.prop('disabled', true);
-                    $('.seek-time').text('-:--');
-                    break;
-
-                case 'pause':
-                    $playbackControls.find('button[data-action=pause]').hide();
-                    $playbackControls.find('button[data-action=play]').show();
-                    $curTrack.find('.artist').show();
-                    $curTrack.find('.track').show();
-                    $curTrack.find('.no-track').hide();
-
-                    $trackSeeker.prop('disabled', false);
-                    $('#seek-time-elapsed').text(elapsed ? elapsed : '-:--');
-                    $('#seek-time-length').text(length ? length : '-:--');
-                    break;
-
-                case 'play':
-                    $playbackControls.find('button[data-action=pause]').show();
-                    $playbackControls.find('button[data-action=play]').hide();
-                    $curTrack.find('.artist').show();
-                    $curTrack.find('.track').show();
-                    $curTrack.find('.no-track').hide();
-
-                    $trackSeeker.prop('disabled', false);
-                    $('#seek-time-elapsed').text(elapsed ? elapsed : '-:--');
-                    $('#seek-time-length').text(length ? length : '-:--');
-
-                    seekInterval = setInterval(function() {
-                        var length = parseInt($trackSeeker.attr('max'));
-                        var value = parseInt((new Date().getTime() - curTrackElapsed.timestamp) / 1000) +
-                            curTrackElapsed.elapsed;
-
-                        if (value < length) {
-                            $trackSeeker.val(value);
-                            elapsed = parseInt(value / 60) + ':' + (value % 60 < 10 ? '0' : '') + (value % 60);
-                            $('#seek-time-elapsed').text(elapsed);
+            if (length !== undefined) {
+                $trackSeeker.attr('max', length);
+            }
+
+            if ('state' in status) {
+                switch (status.state.toLowerCase()) {
+                    case 'stop':
+                        $playbackControls.find('button[data-action=pause]').hide();
+                        $playbackControls.find('button[data-action=play]').show();
+                        $curTrack.find('.artist').hide();
+                        $curTrack.find('.track').hide();
+                        $curTrack.find('.no-track').show();
+
+                        $trackSeeker.prop('disabled', true);
+                        if (seekInterval) {
+                            clearInterval(seekInterval);
+                            seekInterval = undefined;
                         }
-                    }, 1000);
-                    break;
+
+                        $('.seek-time').text('-:--');
+                        break;
+
+                    case 'pause':
+                        $playbackControls.find('button[data-action=pause]').hide();
+                        $playbackControls.find('button[data-action=play]').show();
+                        $curTrack.find('.artist').show();
+                        $curTrack.find('.track').show();
+                        $curTrack.find('.no-track').hide();
+
+                        $trackSeeker.prop('disabled', false);
+                        $('#seek-time-elapsed').text(elapsed ? timeToStr(elapsed) : '-:--');
+                        $('#seek-time-length').text(length ? timeToStr(length) : '-:--');
+                        break;
+
+                    case 'play':
+                        $playbackControls.find('button[data-action=pause]').show();
+                        $playbackControls.find('button[data-action=play]').hide();
+                        $curTrack.find('.artist').show();
+                        $curTrack.find('.track').show();
+                        $curTrack.find('.no-track').hide();
+
+                        $trackSeeker.prop('disabled', false);
+                        $('#seek-time-elapsed').text(elapsed ? timeToStr(elapsed) : '-:--');
+                        $('#seek-time-length').text(length ? timeToStr(length) : '-:--');
+
+                        seekInterval = setInterval(function() {
+                            if (curTrackElapsed.elapsed === undefined) {
+                                return;
+                            }
+
+                            var length = parseInt($trackSeeker.attr('max'));
+                            var value = parseInt((new Date().getTime() - curTrackElapsed.timestamp) / 1000) +
+                                curTrackElapsed.elapsed;
+
+                            if (value < length) {
+                                $trackSeeker.val(value);
+                                elapsed = value;
+                                $('#seek-time-elapsed').text(timeToStr(elapsed));
+                            }
+                        }, 1000);
+                        break;
+                }
             }
 
-            $volumeCtrl.val(parseInt(status.volume));
+            if ('volume' in status) {
+                $volumeCtrl.val(parseInt(status.volume));
+            }
 
-            var repeat = parseInt(status.repeat);
-            if (repeat) {
-                $repeatBtn.addClass('enabled');
-            } else {
-                $repeatBtn.removeClass('enabled');
+            if ('repeat' in status) {
+                var repeat = parseInt(status.repeat);
+                if (repeat) {
+                    $repeatBtn.addClass('enabled');
+                } else {
+                    $repeatBtn.removeClass('enabled');
+                }
             }
 
-            var random = parseInt(status.random);
-            if (random) {
-                $randomBtn.addClass('enabled');
-            } else {
-                $randomBtn.removeClass('enabled');
+            if ('random' in status) {
+                var random = parseInt(status.random);
+                if (random) {
+                    $randomBtn.addClass('enabled');
+                } else {
+                    $randomBtn.removeClass('enabled');
+                }
             }
         }
 
         if (track) {
             $curTrack.find('.artist').text(track.artist);
             $curTrack.find('.track').text(track.title);
 
             var updatePlayingTrack = function(track) {
                 return function() {
                     var $curTrack = $playlistContent.find('.playlist-track').filter(
                         function() {
-                            return $(this).data('pos') == track.pos
+                            return $(this).data('file') === track.file
                         });
 
                     if ($curTrack.length === 0) {
                         return;
                     }
 
                     var offset = $curTrack.offset().top -
@@ -179,14 +218,15 @@
                         '</b><br/>' +
                         ('title' in event.args.track ? event.args.track.title : '[No name]'),
                 });
 
             case 'platypush.message.event.music.MusicStopEvent':
             case 'platypush.message.event.music.MusicPlayEvent':
             case 'platypush.message.event.music.MusicPauseEvent':
+            case 'platypush.message.event.music.SeekChangeEvent':
                 updateControls(status = event.args.status, track = event.args.track);
                 break;
 
             case 'platypush.message.event.music.PlaylistChangeEvent':
                 updatePlaylist(tracks = event.args.changes);
                 break;
         }
@@ -226,16 +266,18 @@
                 action: 'music.mpd.playid',
                 args: {
                     track_id: $track.data('track-id')
                 }
             });
         }
 
-        clearTimeout(longPressTimeout);
-        longPressTimeout = undefined;
+        if (longPressTimeout) {
+            clearTimeout(longPressTimeout);
+            longPressTimeout = undefined;
+        }
     };
 
     var updatePlaylist = function(tracks) {
         if (tracks == null) {
             initPlaylist();
             return;
         }
```

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/music.snapcast.js` & `platypush-0.9.6/platypush/backend/http/static/js/music.snapcast.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -303,15 +303,15 @@
             execute({
                 type: 'request',
                 action: 'music.snapcast.volume',
                 args: args,
             });
         });
 
-        $container.on('click touch', '.snapcast-host-settings', function(evt) {
+        $container.on('mousedown touchstart', '.snapcast-host-settings', function(evt) {
             var host = $(this).parents('.snapcast-host-container').data('host');
             var hostName = $(this).parents('.snapcast-host-container').data('name');
             var $modal = $($(this).data('modal'));
 
             $modal.find('.modal-header').text(hostName);
 
             var info = serverInfo[host];
@@ -319,15 +319,15 @@
             var $info = $form.find('.snapcast-host-info');
 
             for (var attr in info) {
                 $info.find('[data-bind=' + attr + ']').text(info[attr]);
             }
         });
 
-        $container.on('click touch', '.snapcast-group-settings', function(evt) {
+        $container.on('mousedown touchstart', '.snapcast-group-settings', function(evt) {
             var host = $(this).parents('.snapcast-host-container').data('host');
             var groupId = $(this).parents('.snapcast-group-container').data('id');
             var groupName = $(this).parents('.snapcast-group-container').data('name');
             var $modal = $($(this).data('modal'));
             var $form = $modal.find('#snapcast-group-form');
             var $clients = $(this).parents('.snapcast-host-container')
                 .find('.snapcast-client-container');
@@ -370,15 +370,15 @@
                 $option.appendTo($streams);
             }
 
             $form.find('.snapcast-group-stream')
                 .find('select[name=stream]').html($streams.html());
         });
 
-        $container.on('click touch', '.snapcast-client-settings', function(evt) {
+        $container.on('mousedown touchstart', '.snapcast-client-settings', function(evt) {
             var host = $(this).parents('.snapcast-host-container').data('host');
             var clientId = $(this).parents('.snapcast-client-container').data('id');
             var clientName = $(this).parents('.snapcast-client-container').data('name');
             var info = clientInfo[clientId];
             var $modal = $($(this).data('modal'));
             var $form = $modal.find('#snapcast-client-form');
             var $info = $form.find('.snapcast-client-info');
```

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/pushbullet.js` & `platypush-0.9.6/platypush/backend/http/static/js/pushbullet.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/switch.switchbot.js` & `platypush-0.9.6/platypush/backend/http/static/js/switch.switchbot.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/switch.tplink.js` & `platypush-0.9.6/platypush/backend/http/static/js/switch.tplink.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/switch.wemo.js` & `platypush-0.9.6/platypush/backend/http/static/js/switch.wemo.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/tts.google.js` & `platypush-0.9.6/platypush/backend/http/static/js/tts.google.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/tts.js` & `platypush-0.9.6/platypush/backend/http/static/js/tts.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/widgets/calendar.js` & `platypush-0.9.6/platypush/backend/http/static/js/widgets/calendar.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/widgets/date-time-weather.js` & `platypush-0.9.6/platypush/backend/http/static/js/widgets/date-time-weather.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/widgets/image-carousel.js` & `platypush-0.9.6/platypush/backend/http/static/js/widgets/image-carousel.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/widgets/music.js` & `platypush-0.9.6/platypush/backend/http/static/js/widgets/music.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -86,14 +86,19 @@
 
     var setTrackElapsed = function(time) {
         if (refreshElapsedInterval) {
             clearInterval(refreshElapsedInterval);
             refreshElapsedInterval = undefined;
         }
 
+        if (time === undefined) {
+            $timeElapsedElement.text('-:--');
+            return;
+        }
+
         timeElapsed = parseInt(time);
         $timeElapsedElement.text(secondsToTimeString(timeElapsed));
 
         var ratio = 100 * Math.min(timeElapsed / timeTotal, 1);
         $elapsedTimeBar.css('width', ratio + '%');
 
         refreshElapsedInterval = setInterval(function() {
@@ -101,22 +106,41 @@
             ratio = 100 * Math.min(timeElapsed / timeTotal, 1);
             $elapsedTimeBar.css('width', ratio + '%');
             $timeElapsedElement.text(secondsToTimeString(timeElapsed));
         }, 1000);
     };
 
     var refreshStatus = function(status) {
-        setState(state = status.state);
+        if (!status) {
+            return;
+        }
+
+        if ('state' in status) {
+            setState(state = status.state);
+            if (status.state === 'stop') {
+                setTrackElapsed();
+            }
+        }
+
         if ('elapsed' in status) {
             setTrackElapsed(status.elapsed);
+        } else if ('position' in status) {
+            setTrackElapsed(status.position);
         }
     };
 
     var refreshTrack = function(track) {
-        setTrackTime(track.time);
+        if (!track) {
+            return;
+        }
+
+        if ('time' in track) {
+            setTrackTime(track.time);
+        }
+
         $artistElement.text(track.artist);
         $titleElement.text(track.title);
     };
 
     var refreshPlaybackStatus = function(status) {
         if ('volume' in status) {
             $volumeElement.text(status.volume + '%');
```

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/widgets/rss-news.js` & `platypush-0.9.6/platypush/backend/http/static/js/widgets/rss-news.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/static/js/widgets/skycons.js` & `platypush-0.9.6/platypush/backend/http/static/js/widgets/skycons.js`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/dashboard.html` & `platypush-0.9.6/platypush/backend/http/templates/dashboard.html`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         {% if token %}
             window.token = '{% print(token) %}';
         {% else %}
             window.token = undefined;
         {% endif %}
 
         window.config = {{ config | safe }};
-        window.widgets = {{ config['widgets'] | safe }};
+        window.widgets = {{ config['widgets'] | safe }}.reduce(function(map, w) { map[w.widget] = w; return map }, {})
     </script>
 </head>
 
 <body>
     <main>
         <!-- You can send events of type platypush.message.event.web.DashboardIframeUpdateEvent
              to control what is shown in the optional iframe modal -->
@@ -40,24 +40,24 @@
             <div class="modal-container">
                 <iframe></iframe>
             </div>
         </div>
 
         <div id="widgets-container">
             {% set used_columns = [0] %}
-            {% for widget_name, widget in config['widgets'].items() %}
+            {% for widget in config['widgets'] %}
                 {% if used_columns[0] % 12 == 0 %}
                 <div class="row">
                 {% endif %}
 
                 <div class="widget {% print(utils.widget_columns_to_html_class(widget['columns'])) %}
-                        {% print(widget_name) %}"
-                        id="{% print(widget['id'] if 'id' in widget else widget_name) %}">
+                        {% print(widget['widget']) %}"
+                        id="{% print(widget['id'] if 'id' in widget else widget['widget']) %}">
                     {% with properties=widget %}
-                        {% include 'widgets/' + widget_name + '.html' %}
+                        {% include 'widgets/' + widget['widget'] + '.html' %}
                     {% endwith %}
                 </div>
 
                 {# increment counter #}
                 {% if used_columns.append(used_columns.pop() + widget['columns']) %}{% endif %}
 
                 {% if used_columns[0] % 12 == 0 %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 
 
-{% set used_columns = [0] %} {% for widget_name, widget in config
-['widgets'].items() %} {% if used_columns[0] % 12 == 0 %}
+{% set used_columns = [0] %} {% for widget in config['widgets'] %} {% if
+used_columns[0] % 12 == 0 %}
 {% endif %}
-{% with properties=widget %} {% include 'widgets/' + widget_name + '.html' %}
-{% endwith %}
+{% with properties=widget %} {% include 'widgets/' + widget['widget'] + '.html'
+%} {% endwith %}
 {# increment counter #} {% if used_columns.append(used_columns.pop() + widget
 ['columns']) %}{% endif %} {% if used_columns[0] % 12 == 0 %}
 {% endif %} {% endfor %}
```

### Comparing `platypush-0.9.5/platypush/backend/http/templates/index.html` & `platypush-0.9.6/platypush/backend/http/templates/index.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/map.html` & `platypush-0.9.6/platypush/backend/http/templates/map.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/plugins/gpio.zeroborg.html` & `platypush-0.9.6/platypush/backend/http/templates/plugins/gpio.zeroborg.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/plugins/light.hue.html` & `platypush-0.9.6/platypush/backend/http/templates/plugins/light.hue.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/plugins/music.mpd.html` & `platypush-0.9.6/platypush/backend/http/templates/plugins/music.mpd.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/plugins/music.snapcast.html` & `platypush-0.9.6/platypush/backend/http/templates/plugins/music.snapcast.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/plugins/switch.switchbot.html` & `platypush-0.9.6/platypush/backend/http/templates/plugins/switch.switchbot.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/plugins/tts.google.html` & `platypush-0.9.6/platypush/backend/http/templates/plugins/tts.google.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/plugins/tts.html` & `platypush-0.9.6/platypush/backend/http/templates/plugins/tts.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/widgets/date-time-weather.html` & `platypush-0.9.6/platypush/backend/http/templates/widgets/date-time-weather.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/widgets/image-carousel.html` & `platypush-0.9.6/platypush/backend/http/templates/widgets/image-carousel.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/http/templates/widgets/music.html` & `platypush-0.9.6/platypush/backend/http/templates/widgets/music.html`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/inotify/__init__.py` & `platypush-0.9.6/platypush/backend/inotify/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/joystick.py` & `platypush-0.9.6/platypush/backend/joystick.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/kafka/__init__.py` & `platypush-0.9.6/platypush/backend/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/light/hue.py` & `platypush-0.9.6/platypush/backend/light/hue.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,19 @@
         """
 
         super().__init__(*args, **kwargs)
         self.poll_seconds = poll_seconds
 
 
     def _get_lights(self):
-        return get_plugin('light.hue').get_lights().output
+        plugin = get_plugin('light.hue')
+        if not plugin:
+            plugin = get_plugin('light.hue', reload=True)
+
+        return plugin.get_lights().output
 
     def _listener(self):
         def _thread():
             lights = self._get_lights()
 
             while not self.should_stop():
                 try:
```

### Comparing `platypush-0.9.5/platypush/backend/local/__init__.py` & `platypush-0.9.6/platypush/backend/local/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/midi.py` & `platypush-0.9.6/platypush/backend/midi.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/mqtt.py` & `platypush-0.9.6/platypush/backend/mqtt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import json
 import os
 import threading
 
-import paho.mqtt.client as mqtt
-import paho.mqtt.publish as publisher
-
 from platypush.backend import Backend
 from platypush.context import get_plugin
 from platypush.message import Message
 from platypush.message.request import Request
 from platypush.utils import set_thread_name
 
 
@@ -61,14 +58,15 @@
         super().__init__(*args, **kwargs)
 
         self.host = host
         self.port = port
         self.topic = '{}/{}'.format(topic, self.device_id)
         self.username = username
         self.password = password
+        self._client = None
 
         self.tls_cafile = os.path.abspath(os.path.expanduser(tls_cafile)) \
             if tls_cafile else None
 
         self.tls_certfile = os.path.abspath(os.path.expanduser(tls_certfile)) \
             if tls_certfile else None
 
@@ -123,29 +121,36 @@
                 return
 
             if isinstance(msg, Request):
                 threading.Thread(target=response_thread,
                                  name='MQTTProcessor',
                                  args=(msg,)).start()
 
+        import paho.mqtt.client as mqtt
+
         super().run()
-        client = mqtt.Client()
-        client.on_connect = on_connect
-        client.on_message = on_message
+        self._client = mqtt.Client()
+        self._client.on_connect = on_connect
+        self._client.on_message = on_message
 
         if self.username and self.password:
-            client.username_pw_set(self.username, self.password)
+            self._client.username_pw_set(self.username, self.password)
 
         if self.tls_cafile:
-            client.tls_set(ca_certs=self.tls_cafile, certfile=self.tls_certfile,
+            self._client.tls_set(ca_certs=self.tls_cafile, certfile=self.tls_certfile,
                            keyfile=self.tls_keyfile, tls_version=self.tls_version,
                            ciphers=self.tls_ciphers)
 
-        client.connect(self.host, self.port, 60)
+        self._client.connect(self.host, self.port, 60)
         self.logger.info('Initialized MQTT backend on host {}:{}, topic {}'.
                      format(self.host, self.port, self.topic))
 
-        client.loop_forever()
+        self._client.loop_forever()
 
+    def stop(self):
+        self.logger.info('Received STOP event on MqttBackend')
+        if self._client:
+            self._client.disconnect()
+            self._client.loop_stop()
+            self._client = None
 
 # vim:sw=4:ts=4:et:
-
```

### Comparing `platypush-0.9.5/platypush/backend/music/mpd/__init__.py` & `platypush-0.9.6/platypush/backend/music/mpd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,18 @@
         last_playlist = None
         plugin = None
 
         while not self.should_stop():
             success = False
 
             while not success:
+                state = None
+                playlist = None
+                track = None
+
                 try:
                     plugin = get_plugin('music.mpd')
                     if not plugin:
                         raise StopIteration
 
                     status = plugin.status().output
                     if not status or status.get('state') is None:
```

### Comparing `platypush-0.9.5/platypush/backend/music/snapcast.py` & `platypush-0.9.6/platypush/backend/music/snapcast.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,43 +27,49 @@
         * :class:`platypush.message.event.music.snapcast.GroupMuteChangeEvent`
         * :class:`platypush.message.event.music.snapcast.GroupStreamChangeEvent`
         * :class:`platypush.message.event.music.snapcast.StreamUpdateEvent`
         * :class:`platypush.message.event.music.snapcast.ServerUpdateEvent`
     """
 
     _DEFAULT_SNAPCAST_PORT = 1705
+    _DEFAULT_POLL_SECONDS = 10   # Poll servers each 10 seconds
     _SOCKET_EOL = '\r\n'.encode()
 
     def __init__(self, hosts=['localhost'], ports=[_DEFAULT_SNAPCAST_PORT],
-                 *args, **kwargs):
+                 poll_seconds=_DEFAULT_POLL_SECONDS, *args, **kwargs):
         """
         :param hosts: List of Snapcast server names or IPs to monitor (default:
             `['localhost']`
         :type hosts: list[str]
 
         :param ports: List of control ports for the configured Snapcast servers
             (default: `[1705]`)
         :type ports: list[int]
+
+        :param poll_seconds: How often the backend will poll remote servers for
+            status updated (default: 10 seconds)
+        :type poll_seconds: float
         """
 
         super().__init__(*args, **kwargs)
 
         self.hosts = hosts[:]
         self.ports = ports[:]
+        self.poll_seconds = poll_seconds
         self._socks = {}
         self._threads = {}
         self._statuses = {}
 
         if len(hosts) > len(ports):
             for _ in range(len(ports), len(hosts)):
                 self.ports.append(self._DEFAULT_SNAPCAST_PORT)
 
 
     def _connect(self, host, port):
-        if host in self._socks:
+        if self._socks.get(host):
             return self._socks[host]
 
         self.logger.debug('Connecting to {}:{}'.format(host, port))
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.connect((host, port))
         self._socks[host] = sock
         self.logger.info('Connected to {}:{}'.format(host, port))
@@ -138,15 +144,15 @@
             except Exception as e:
                 self.logger.warning(('Exception while getting the status ' +
                                      'of the Snapcast server {}:{}: {}').
                                     format(host, port, str(e)))
 
                 try:
                     self._disconnect(host, port)
-                    time.sleep(5)
+                    time.sleep(self.poll_seconds)
                 except:
                     pass
 
             while not self.should_stop():
                 try:
                     sock = self._connect(host, port)
                     msgs = self._recv(sock)
@@ -164,17 +170,18 @@
                 except Exception as e:
                     self.logger.warning(('Exception while getting the status ' +
                                          'of the Snapcast server {}:{}: {}').
                                         format(host, port, str(e)))
 
                     try:
                         self._disconnect(host, port)
-                        time.sleep(5)
                     except:
                         pass
+                    finally:
+                        time.sleep(self.poll_seconds)
 
         return _thread
 
     @classmethod
     def _get_req_id(cls):
         return get_plugin('music.snapcast')._get_req_id()
 
@@ -184,15 +191,20 @@
         request = {
             'id': self._get_req_id(),
             'jsonrpc':'2.0',
             'method':'Server.GetStatus'
         }
 
         get_plugin('music.snapcast')._send(sock, request)
-        return self._recv(sock).get('result', {}).get('server', {})
+        try:
+            return self._recv(sock).get('result', {}).get('server', {})
+        except Exception as e:
+            self.logger.warning('Unable to connect to {}:{}: {}'.format(
+                host, port, str(e)))
+            self._socks[hosts] = None
 
     def run(self):
         super().run()
 
         self.logger.info('Initialized Snapcast backend - hosts: {} ports: {}'.
                          format(self.hosts, self.ports))
```

### Comparing `platypush-0.9.5/platypush/backend/pushbullet/__init__.py` & `platypush-0.9.6/platypush/backend/pushbullet/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/redis.py` & `platypush-0.9.6/platypush/backend/redis.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/scard/__init__.py` & `platypush-0.9.6/platypush/backend/scard/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/sensor/__init__.py` & `platypush-0.9.6/platypush/backend/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/sensor/accelerometer.py` & `platypush-0.9.6/platypush/backend/sensor/accelerometer.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/sensor/distance/__init__.py` & `platypush-0.9.6/platypush/backend/sensor/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/sensor/ir/zeroborg/__init__.py` & `platypush-0.9.6/platypush/backend/sensor/ir/zeroborg/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/sensor/leap.py` & `platypush-0.9.6/platypush/backend/sensor/leap.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/sensor/mcp3008.py` & `platypush-0.9.6/platypush/backend/sensor/mcp3008.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/sensor/serial.py` & `platypush-0.9.6/platypush/backend/sensor/serial.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/tcp.py` & `platypush-0.9.6/platypush/backend/tcp.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/weather/forecast.py` & `platypush-0.9.6/platypush/backend/weather/forecast.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/backend/websocket.py` & `platypush-0.9.6/platypush/backend/websocket.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import threading
 import websockets
 
 from platypush.backend import Backend
 from platypush.context import get_plugin, get_or_create_event_loop
 from platypush.message import Message
 from platypush.message.request import Request
+from platypush.message.response import Response
 from platypush.utils import get_ssl_server_context
 
 
 class WebsocketBackend(Backend):
     """
     Backend to communicate messages over a websocket medium.
 
@@ -19,16 +20,19 @@
 
         * **websockets** (``pip install websockets``)
     """
 
     # Websocket client message recv timeout in seconds
     _websocket_client_timeout = 0
 
-    def __init__(self, port=8765, bind_address='0.0.0.0', ssl_cafile=None,
-                 ssl_capath=None, ssl_cert=None, ssl_key=None,
+    # Default websocket service port
+    _default_websocket_port = 8765
+
+    def __init__(self, port=_default_websocket_port, bind_address='0.0.0.0',
+                 ssl_cafile=None, ssl_capath=None, ssl_cert=None, ssl_key=None,
                  client_timeout=_websocket_client_timeout, **kwargs):
         """
         :param port: Listen port for the websocket server (default: 8765)
         :type port: int
 
         :param bind_address: Bind address for the websocket server (default: 0.0.0.0, listen for any IP connection)
         :type websocket_port: str
@@ -112,34 +116,30 @@
                     msg = Message.build(msg)
                     self.logger.info('Received message from {}: {}'.
                                     format(websocket.remote_address[0], msg))
 
                     self.on_message(msg)
 
                     if isinstance(msg, Request):
-                        response = self.get_message_response(msg)
-                        if not response:
-                            return
-
+                        response = self.get_message_response(msg) or Response()
                         self.logger.info('Processing response on the websocket backend: {}'.
-                                            format(response))
+                                         format(response))
 
                         await websocket.send(str(response))
 
+            except websockets.exceptions.ConnectionClosed as e:
+                self.active_websockets.remove(websocket)
+                self.logger.debug('Websocket client {} closed connection'.
+                                  format(websocket.remote_address[0]))
+            except asyncio.TimeoutError as e:
+                self.active_websockets.remove(websocket)
+                self.logger.debug('Websocket connection to {} timed out'.
+                                  format(websocket.remote_address[0]))
             except Exception as e:
-                if isinstance(e, websockets.exceptions.ConnectionClosed):
-                    self.active_websockets.remove(websocket)
-                    self.logger.debug('Websocket client {} closed connection'.
-                                    format(websocket.remote_address[0]))
-                elif isinstance(e, asyncio.TimeoutError):
-                    self.active_websockets.remove(websocket)
-                    self.logger.debug('Websocket connection to {} timed out'.
-                                    format(websocket.remote_address[0]))
-                else:
-                    self.logger.exception(e)
+                self.logger.exception(e)
 
         self.logger.info('Initialized websocket backend on port {}, bind address: {}'.
                          format(self.port, self.bind_address))
 
         websocket_args = {}
         if self.ssl_context:
             websocket_args['ssl'] = self.ssl_context
```

### Comparing `platypush-0.9.5/platypush/backend/wiimote.py` & `platypush-0.9.6/platypush/backend/wiimote.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/bus/__init__.py` & `platypush-0.9.6/platypush/bus/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,24 @@
         """ Stops the bus by sending a STOP event """
         evt = StopEvent(target=Config.get('device_id'),
                         origin=Config.get('device_id'),
                         thread_id=self.thread_id)
 
         self.post(evt)
 
+    def _msg_executor(self, msg):
+        def executor():
+            try:
+                self.on_message(msg)
+            except Exception as e:
+                logger.error('Error on processing message {}'.format(msg))
+                logger.exception(e)
+
+        return executor
+
     def poll(self):
         """
         Reads messages from the bus until either stop event message or KeyboardInterrupt
         """
 
         if not self.on_message:
             logger.warning('No message handlers installed, cannot poll')
@@ -50,20 +60,15 @@
         while not stop:
             msg = self.get()
             if msg.timestamp and time.time() - msg.timestamp > self._MSG_EXPIRY_TIMEOUT:
                 logger.debug('{} seconds old message on the bus expired, ignoring it: {}'
                             .format(int(time.time()-msg.timestamp), msg))
                 continue
 
-            try:
-                self.on_message(msg)
-            except Exception as e:
-                logger.error('Error on processing message {}'.format(msg))
-                logger.exception(e)
+            threading.Thread(target=self._msg_executor(msg)).start()
 
             if isinstance(msg, StopEvent) and msg.targets_me():
                 logger.info('Received STOP event on the bus')
                 stop=True
 
 
 # vim:sw=4:ts=4:et:
-
```

### Comparing `platypush-0.9.5/platypush/bus/redis.py` & `platypush-0.9.6/platypush/bus/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import json
 import logging
 import threading
 
 from redis import Redis
 
 from platypush.bus import Bus
+from platypush.config import Config
 from platypush.message import Message
 
 logger = logging.getLogger(__name__)
 
 
 class RedisBus(Bus):
     """ Overrides the in-process in-memory local bus with a Redis bus """
     _DEFAULT_REDIS_QUEUE = 'platypush/bus'
 
     def __init__(self, on_message=None, redis_queue=_DEFAULT_REDIS_QUEUE,
                  *args, **kwargs):
         super().__init__(on_message=on_message)
+
+        if not args and not kwargs:
+            kwargs = (Config.get('backend.redis') or {}).get('redis_args', {})
+
         self.redis = Redis(*args, **kwargs)
+        self.redis_args = kwargs
         self.redis_queue = redis_queue
         self.on_message = on_message
         self.thread_id = threading.get_ident()
 
     def get(self):
         """ Reads one message from the Redis queue """
         msg = None
```

### Comparing `platypush-0.9.5/platypush/config/__init__.py` & `platypush-0.9.6/platypush/config/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/context/__init__.py` & `platypush-0.9.6/platypush/context/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,14 +89,24 @@
     for token in plugin_name.split('.'):
         cls_name += token.title()
     cls_name += 'Plugin'
 
     plugin_conf = Config.get_plugins()[plugin_name] \
         if plugin_name in Config.get_plugins() else {}
 
+    if 'disabled' in plugin_conf:
+        if plugin_conf['disabled'] is True:
+            return None
+        del plugin_conf['disabled']
+
+    if 'enabled' in plugin_conf:
+        if plugin_conf['enabled'] is False:
+            return None
+        del plugin_conf['enabled']
+
     try:
         plugin_class = getattr(plugin, cls_name)
     except AttributeError as e:
         logger.warning('No such class in {}: {}'.format(plugin_name, cls_name))
         raise RuntimeError(e)
 
     with plugins_init_locks[plugin_name]:
```

### Comparing `platypush-0.9.5/platypush/cron/scheduler.py` & `platypush-0.9.6/platypush/cron/scheduler.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/event/hook.py` & `platypush-0.9.6/platypush/event/hook.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/event/processor/__init__.py` & `platypush-0.9.6/platypush/event/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/__init__.py` & `platypush-0.9.6/platypush/message/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/__init__.py` & `platypush-0.9.6/platypush/message/event/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/adafruit.py` & `platypush-0.9.6/platypush/message/event/adafruit.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/assistant/__init__.py` & `platypush-0.9.6/platypush/message/event/assistant/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -114,9 +114,63 @@
         :param hotword: The detected user hotword
         :type hotword: str
         """
 
         super().__init__(*args, hotword=hotword, **kwargs)
 
 
+class AlertStartedEvent(AssistantEvent):
+    """
+    Event triggered when an alert starts on the assistant
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+class AlertEndEvent(AssistantEvent):
+    """
+    Event triggered when an alert ends on the assistant
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+class AlarmStartedEvent(AlertStartedEvent):
+    """
+    Event triggered when an alarm starts on the assistant
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+class AlarmEndEvent(AlertEndEvent):
+    """
+    Event triggered when an alarm ends on the assistant
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+class TimerStartedEvent(AlertStartedEvent):
+    """
+    Event triggered when a timer starts on the assistant
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+class TimerEndEvent(AlertEndEvent):
+    """
+    Event triggered when a timer ends on the assistant
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
 # vim:sw=4:ts=4:et:
```

### Comparing `platypush-0.9.5/platypush/message/event/button/flic/__init__.py` & `platypush-0.9.6/platypush/message/event/button/flic/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/http/rss.py` & `platypush-0.9.6/platypush/message/event/http/rss.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/joystick.py` & `platypush-0.9.6/platypush/message/event/joystick.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/light.py` & `platypush-0.9.6/platypush/message/event/light.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/midi.py` & `platypush-0.9.6/platypush/message/event/midi.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/music/__init__.py` & `platypush-0.9.6/platypush/message/event/music/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,23 +39,41 @@
     Event fired upon playback paused
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
+class SeekChangeEvent(MusicEvent):
+    """
+    Event fired upon seek change
+    """
+
+    def __init__(self, position, status=None, track=None, *args, **kwargs):
+        super().__init__(position=position, status=status, track=track, *args, **kwargs)
+
+
 class VolumeChangeEvent(MusicEvent):
     """
     Event fired upon volume change
     """
 
     def __init__(self, volume, status=None, track=None, *args, **kwargs):
         super().__init__(volume=volume, status=status, track=track, *args, **kwargs)
 
 
+class MuteChangeEvent(MusicEvent):
+    """
+    Event fired upon mute change
+    """
+
+    def __init__(self, mute, status=None, track=None, *args, **kwargs):
+        super().__init__(mute=mute, status=status, track=track, *args, **kwargs)
+
+
 class PlaybackRepeatModeChangeEvent(MusicEvent):
     """
     Event fired upon repeat mode change
     """
 
     def __init__(self, state, status=None, track=None, *args, **kwargs):
         super().__init__(state=state, status=status, track=track, *args, **kwargs)
```

### Comparing `platypush-0.9.5/platypush/message/event/music/snapcast.py` & `platypush-0.9.6/platypush/message/event/music/snapcast.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/path/__init__.py` & `platypush-0.9.6/platypush/message/event/path/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/pushbullet.py` & `platypush-0.9.6/platypush/message/event/pushbullet.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/scard.py` & `platypush-0.9.6/platypush/message/event/scard.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/sensor/__init__.py` & `platypush-0.9.6/platypush/message/event/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/sensor/ir/__init__.py` & `platypush-0.9.6/platypush/message/event/sensor/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/sensor/leap.py` & `platypush-0.9.6/platypush/message/event/sensor/leap.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/torrent.py` & `platypush-0.9.6/platypush/message/event/torrent.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,44 @@
     Base class for torrent events
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
-class TorrentDownloadStartEvent(TorrentEvent):
+class TorrentDownloadingMetadataEvent(TorrentEvent):
     """
-    Event triggered upon torrent download start
+    Event triggered upon torrent metadata download start
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
-class TorrentSeedingStartEvent(TorrentEvent):
+class TorrentDownloadStartEvent(TorrentEvent):
     """
-    Event triggered upon torrent seeding start
+    Event triggered upon torrent download start
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
-class TorrentDownloadProgressEvent(TorrentEvent):
+class TorrentSeedingStartEvent(TorrentEvent):
     """
-    Event triggered upon torrent download progress
+    Event triggered upon torrent seeding start
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
-class TorrentStateChangeEvent(TorrentEvent):
+class TorrentDownloadProgressEvent(TorrentEvent):
     """
-    Event triggered upon torrent state change
+    Event triggered upon torrent download progress
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class TorrentStateChangeEvent(TorrentEvent):
@@ -70,8 +70,7 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 # vim:sw=4:ts=4:et:
-
```

### Comparing `platypush-0.9.5/platypush/message/event/video/__init__.py` & `platypush-0.9.6/platypush/message/event/video/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from platypush.message.event import Event
+from platypush.message.event.media import MediaEvent
 
 
-class VideoEvent(Event):
+class VideoEvent(MediaEvent):
     """ Base class for video events """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class VideoPlayEvent(VideoEvent):
@@ -51,8 +52,7 @@
         :type video: str
         """
 
         super().__init__(*args, video=video, **kwargs)
 
 
 # vim:sw=4:ts=4:et:
-
```

### Comparing `platypush-0.9.5/platypush/message/event/web/__init__.py` & `platypush-0.9.6/platypush/message/event/web/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/event/wiimote.py` & `platypush-0.9.6/platypush/message/event/wiimote.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/message/request/__init__.py` & `platypush-0.9.6/platypush/message/request/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,25 +204,24 @@
             try:
                 # Run the action
                 args = self._expand_context(**context)
                 response = plugin.run(method=method_name, **args)
 
                 if response and response.is_error():
                     logger.warning(('Response processed with errors from ' +
-                                    'action {}.{}: {}').format(
-                                        plugin, self.action, str(response)))
+                                    'action {}: {}').format(
+                                        self.action, str(response)))
                 else:
-                    logger.info('Processed response from action {}.{}: {}'.
-                                format(plugin, self.action, str(response)))
+                    logger.info('Processed response from action {}: {}'.
+                                format(self.action, str(response)))
             except Exception as e:
                 # Retry mechanism
                 plugin.logger.exception(e)
                 logger.warning(('Uncaught exception while processing response ' +
-                                'from action {}.{}: {}').format(
-                                    plugin, self.action, str(e)))
+                                'from action [{}]: {}').format(self.action, str(e)))
 
                 errors = errors or []
                 if str(e) not in errors:
                     errors.append(str(e))
 
                 response = Response(output=None, errors=errors)
                 if n_tries-1 > 0:
```

### Comparing `platypush-0.9.5/platypush/message/response/__init__.py` & `platypush-0.9.6/platypush/message/response/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/platydock/__init__.py` & `platypush-0.9.6/platypush/platydock/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/__init__.py` & `platypush-0.9.6/platypush/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/adafruit/io.py` & `platypush-0.9.6/platypush/plugins/adafruit/io.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/assistant/google/__init__.py` & `platypush-0.9.6/platypush/plugins/assistant/google/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/assistant/google/pushtotalk.py` & `platypush-0.9.6/platypush/plugins/assistant/google/pushtotalk.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/autoremote.py` & `platypush-0.9.6/platypush/plugins/autoremote.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/calendar/__init__.py` & `platypush-0.9.6/platypush/plugins/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/calendar/ical.py` & `platypush-0.9.6/platypush/plugins/calendar/ical.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/camera/pi.py` & `platypush-0.9.6/platypush/plugins/camera/pi.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/clipboard.py` & `platypush-0.9.6/platypush/plugins/clipboard.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/db/__init__.py` & `platypush-0.9.6/platypush/plugins/db/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/file.py` & `platypush-0.9.6/platypush/plugins/file.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/google/__init__.py` & `platypush-0.9.6/platypush/plugins/google/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/google/calendar.py` & `platypush-0.9.6/platypush/plugins/google/calendar.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/google/credentials.py` & `platypush-0.9.6/platypush/plugins/google/credentials.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/google/mail.py` & `platypush-0.9.6/platypush/plugins/google/mail.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/google/maps.py` & `platypush-0.9.6/platypush/plugins/google/maps.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/google/youtube.py` & `platypush-0.9.6/platypush/plugins/google/youtube.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/gpio/__init__.py` & `platypush-0.9.6/platypush/plugins/gpio/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/gpio/sensor/__init__.py` & `platypush-0.9.6/platypush/plugins/gpio/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/gpio/sensor/accelerometer/__init__.py` & `platypush-0.9.6/platypush/plugins/gpio/sensor/accelerometer/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/gpio/sensor/accelerometer/lib/LIS3DH.py` & `platypush-0.9.6/platypush/plugins/gpio/sensor/accelerometer/lib/LIS3DH.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/gpio/sensor/distance/__init__.py` & `platypush-0.9.6/platypush/plugins/gpio/sensor/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/gpio/sensor/mcp3008/__init__.py` & `platypush-0.9.6/platypush/plugins/gpio/sensor/mcp3008/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/gpio/zeroborg/__init__.py` & `platypush-0.9.6/platypush/plugins/gpio/zeroborg/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/gpio/zeroborg/lib/__init__.py` & `platypush-0.9.6/platypush/plugins/gpio/zeroborg/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/homeseer.py` & `platypush-0.9.6/platypush/plugins/homeseer.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/http/request/__init__.py` & `platypush-0.9.6/platypush/plugins/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/http/request/ota/booking/__init__.py` & `platypush-0.9.6/platypush/plugins/http/request/ota/booking/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/ifttt.py` & `platypush-0.9.6/platypush/plugins/ifttt.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/kafka.py` & `platypush-0.9.6/platypush/plugins/kafka.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/lastfm/__init__.py` & `platypush-0.9.6/platypush/plugins/lastfm/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/light/__init__.py` & `platypush-0.9.6/platypush/plugins/light/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/light/hue/__init__.py` & `platypush-0.9.6/platypush/plugins/light/hue/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import statistics
 import time
 
 from enum import Enum
 from threading import Thread
 from redis import Redis
 from redis.exceptions import TimeoutError as QueueTimeoutError
-from phue import Bridge
 
 from platypush.context import get_backend
 from platypush.plugins import action
 from platypush.plugins.light import LightPlugin
 from platypush.utils import set_thread_name
 
 
@@ -23,14 +22,16 @@
         * **phue** (``pip install phue``)
     """
 
     MAX_BRI = 255
     MAX_SAT = 255
     MAX_HUE = 65535
     ANIMATION_CTRL_QUEUE_NAME = 'platypush/light/hue/AnimationCtrl'
+    _BRIDGE_RECONNECT_SECONDS = 5
+    _MAX_RECONNECT_TRIES = 5
 
     class Animation(Enum):
         COLOR_TRANSITION = 'color_transition'
         BLINK = 'blink'
 
         def __eq__(self, other):
             if isinstance(other, str):
@@ -85,24 +86,36 @@
         after clicking the pairing button on your bridge.
 
         :todo: Support for dynamic retry and better user interaction in case of bridge pairing neeeded.
         """
 
         # Lazy init
         if not self.bridge:
-            self.bridge = Bridge(self.bridge_address)
-            self.logger.info('Bridge connected')
+            from phue import Bridge, PhueRegistrationException
+            success = False
+            n_tries = 0
 
-            self.get_scenes()
+            while not success:
+                try:
+                    n_tries += 1
+                    self.bridge = Bridge(self.bridge_address)
+                    success = True
+                except PhueRegistrationException as e:
+                    self.logger.warning('Bridge registration error: {}'.
+                                        format(str(e)))
+
+                    if n_tries >= self._MAX_RECONNECT_TRIES:
+                        self.logger.error(('Bridge registration failed after ' +
+                                           '{} attempts').format(n_tries))
+                        break
 
-            # uncomment these lines if you're running huectrl for
-            # the first time and you need to pair it to the switch
+                    time.sleep(self._BRIDGE_RECONNECT_SECONDS)
 
-            # self.bridge.connect()
-            # self.bridge.get_api()
+            self.logger.info('Bridge connected')
+            self.get_scenes()
         else:
             self.logger.info('Bridge already connected')
 
 
     @action
     def get_scenes(self):
         """
@@ -237,33 +250,36 @@
             self.stop_animation()
         except Exception as e:
             # Reset bridge connection
             self.bridge = None
             raise e
 
         lights = []; groups = []
-        if 'lights' in kwargs and kwargs['lights']:
+        if 'lights' in kwargs:
             lights = kwargs.pop('lights').split(',').strip() \
                 if isinstance(lights, str) else kwargs.pop('lights')
-        if 'groups' in kwargs and kwargs['groups']:
+        if 'groups' in kwargs:
             groups = kwargs.pop('groups').split(',').strip() \
                 if isinstance(groups, str) else kwargs.pop('groups')
 
         if not lights and not groups:
             lights = self.lights
             groups = self.groups
 
+        if not self.bridge:
+            self.connect()
+
         try:
             if attr == 'scene':
                 self.bridge.run_scene(groups[0], kwargs.pop('name'))
             else:
                 if groups:
-                    self.bridge.set_group(groups, attr, *args)
+                    self.bridge.set_group(groups, attr, *args, **kwargs)
                 if lights:
-                    self.bridge.set_light(lights, attr, *args)
+                    self.bridge.set_light(lights, attr, *args, **kwargs)
         except Exception as e:
             # Reset bridge connection
             self.bridge = None
             raise e
 
 
     @action
@@ -311,37 +327,37 @@
             }
         """
 
         self.connect()
         self.bridge.set_group(group, **kwargs)
 
     @action
-    def on(self, lights=[], groups=[]):
+    def on(self, lights=[], groups=[], **kwargs):
         """
         Turn lights/groups on.
 
         :param lights: Lights to turn on (names or light objects). Default: plugin default lights
         :param groups: Groups to turn on (names or group objects). Default: plugin default groups
         """
 
-        return self._exec('on', True, lights=lights, groups=groups)
+        return self._exec('on', True, lights=lights, groups=groups, **kwargs)
 
     @action
-    def off(self, lights=[], groups=[]):
+    def off(self, lights=[], groups=[], **kwargs):
         """
         Turn lights/groups off.
 
         :param lights: Lights to turn off (names or light objects). Default: plugin default lights
         :param groups: Groups to turn off (names or group objects). Default: plugin default groups
         """
 
-        return self._exec('on', False, lights=lights, groups=groups)
+        return self._exec('on', False, lights=lights, groups=groups, **kwargs)
 
     @action
-    def toggle(self, lights=[], groups=[]):
+    def toggle(self, lights=[], groups=[], **kwargs):
         """
         Toggle lights/groups on/off.
 
         :param lights: Lights to turn off (names or light objects). Default: plugin default lights
         :param groups: Groups to turn off (names or group objects). Default: plugin default groups
         """
 
@@ -376,60 +392,60 @@
 
             lights_off = [
                 light['name'] for light in all_lights
                 if light['name'] in lights and light['state']['on'] is False
             ]
 
         if lights_on or groups_on:
-            self._exec('on', False, lights=lights_on, groups=groups_on)
+            self._exec('on', False, lights=lights_on, groups=groups_on, **kwargs)
 
         if lights_off or groups_off:
-            self._exec('on', True, lights=lights_off, groups=groups_off)
+            self._exec('on', True, lights=lights_off, groups=groups_off, **kwargs)
 
     @action
-    def bri(self, value, lights=[], groups=[]):
+    def bri(self, value, lights=[], groups=[], **kwargs):
         """
         Set lights/groups brightness.
 
         :param lights: Lights to control (names or light objects). Default: plugin default lights
         :param groups: Groups to control (names or group objects). Default: plugin default groups
         :param value: Brightness value (range: 0-255)
         """
 
         return self._exec('bri', int(value) % (self.MAX_BRI+1),
-                      lights=lights, groups=groups)
+                          lights=lights, groups=groups, **kwargs)
 
     @action
-    def sat(self, value, lights=[], groups=[]):
+    def sat(self, value, lights=[], groups=[], **kwargs):
         """
         Set lights/groups saturation.
 
         :param lights: Lights to control (names or light objects). Default: plugin default lights
         :param groups: Groups to control (names or group objects). Default: plugin default groups
         :param value: Saturation value (range: 0-255)
         """
 
         return self._exec('sat', int(value) % (self.MAX_SAT+1),
-                      lights=lights, groups=groups)
+                      lights=lights, groups=groups, **kwargs)
 
     @action
-    def hue(self, value, lights=[], groups=[]):
+    def hue(self, value, lights=[], groups=[], **kwargs):
         """
         Set lights/groups color hue.
 
         :param lights: Lights to control (names or light objects). Default: plugin default lights
         :param groups: Groups to control (names or group objects). Default: plugin default groups
         :param value: Hue value (range: 0-65535)
         """
 
         return self._exec('hue', int(value) % (self.MAX_HUE+1),
-                      lights=lights, groups=groups)
+                      lights=lights, groups=groups, **kwargs)
 
     @action
-    def delta_bri(self, delta, lights=[], groups=[]):
+    def delta_bri(self, delta, lights=[], groups=[], **kwargs):
         """
         Change lights/groups brightness by a delta [-100, 100] compared to the current state.
 
         :param lights: Lights to control (names or light objects). Default: plugin default lights
         :param groups: Groups to control (names or group objects). Default: plugin default groups
         :param delta: Brightness delta value (range: -100, 100)
         """
@@ -459,18 +475,18 @@
         if bri+delta < 0:
             bri = 0
         elif bri+delta > self.MAX_BRI:
             bri = self.MAX_BRI
         else:
             bri += delta
 
-        return self._exec('bri', int(bri), lights=lights, groups=groups)
+        return self._exec('bri', int(bri), lights=lights, groups=groups, **kwargs)
 
     @action
-    def delta_sat(self, delta, lights=[], groups=[]):
+    def delta_sat(self, delta, lights=[], groups=[], **kwargs):
         """
         Change lights/groups saturation by a delta [-100, 100] compared to the current state.
 
         :param lights: Lights to control (names or light objects). Default: plugin default lights
         :param groups: Groups to control (names or group objects). Default: plugin default groups
         :param delta: Saturation delta value (range: -100, 100)
         """
@@ -500,18 +516,18 @@
         if sat+delta < 0:
             sat = 0
         elif sat+delta > self.MAX_SAT:
             sat = self.MAX_SAT
         else:
             sat += delta
 
-        return self._exec('sat', int(sat), lights=lights, groups=groups)
+        return self._exec('sat', int(sat), lights=lights, groups=groups, **kwargs)
 
     @action
-    def delta_hue(self, delta, lights=[], groups=[]):
+    def delta_hue(self, delta, lights=[], groups=[], **kwargs):
         """
         Change lights/groups hue by a delta [-100, 100] compared to the current state.
 
         :param lights: Lights to control (names or light objects). Default: plugin default lights
         :param groups: Groups to control (names or group objects). Default: plugin default groups
         :param delta: Hue delta value (range: -100, 100)
         """
@@ -541,28 +557,28 @@
         if hue+delta < 0:
             hue = 0
         elif hue+delta > self.MAX_HUE:
             hue = self.MAX_HUE
         else:
             hue += delta
 
-        return self._exec('hue', int(hue), lights=lights, groups=groups)
+        return self._exec('hue', int(hue), lights=lights, groups=groups, **kwargs)
 
 
     @action
-    def scene(self, name, lights=[], groups=[]):
+    def scene(self, name, lights=[], groups=[], **kwargs):
         """
         Set a scene by name.
 
         :param lights: Lights to control (names or light objects). Default: plugin default lights
         :param groups: Groups to control (names or group objects). Default: plugin default groups
         :param name: Name of the scene
         """
 
-        return self._exec('scene', name=name, lights=lights, groups=groups)
+        return self._exec('scene', name=name, lights=lights, groups=groups, **kwargs)
 
     @action
     def is_animation_running(self):
         """
         :returns: True if there is an animation running, false otherwise.
         """
 
@@ -571,15 +587,16 @@
     @action
     def stop_animation(self):
         """
         Stop a running animation if any
         """
 
         if self.animation_thread and self.animation_thread.is_alive():
-            self.redis.rpush(self.ANIMATION_CTRL_QUEUE_NAME, 'STOP')
+            redis = self._get_redis()
+            redis.rpush(self.ANIMATION_CTRL_QUEUE_NAME, 'STOP')
 
     @action
     def animate(self, animation, duration=None,
                 hue_range=[0, MAX_HUE], sat_range=[0, MAX_SAT],
                 bri_range=[MAX_BRI-1, MAX_BRI], lights=None, groups=None,
                 hue_step=1000, sat_step=2, bri_step=1, transition_seconds=1.0):
         """
@@ -612,14 +629,21 @@
         :param bri_step: If you selected a color transition, this will specify by how much the brightness will change between iterations. Default: 1
         :type bri_step: int
 
         :param transition_seconds: Time between two transitions or blinks in seconds. Default: 1.0
         :type treansition_seconds: float
         """
 
+        if groups:
+            groups = [g for g in self.bridge.groups if g.name in groups]
+            lights = lights or []
+            for g in groups:
+                lights.extend([l.name for l in g.lights])
+        elif not lights:
+            lights = self.lights
 
         def _initialize_light_attrs(lights):
             if animation == self.Animation.COLOR_TRANSITION:
                 return { l: {
                     'hue': random.randint(hue_range[0], hue_range[1]),
                     'sat': random.randint(sat_range[0], sat_range[1]),
                     'bri': random.randint(bri_range[0], bri_range[1]),
@@ -627,15 +651,14 @@
             elif animation == self.Animation.BLINK:
                 return { l: {
                     'on': True,
                     'bri': self.MAX_BRI,
                     'transitiontime': 0,
                 } for l in lights }
 
-
         def _next_light_attrs(lights):
             if animation == self.Animation.COLOR_TRANSITION:
                 for (light, attrs) in lights.items():
                     for (attr, value) in attrs.items():
                         if attr == 'hue':
                             attr_range = hue_range
                             attr_step = hue_step
@@ -656,15 +679,16 @@
                     'transitiontime': 0,
                 } for (light, attrs) in lights.items() }
 
             return lights
 
         def _should_stop():
             try:
-                self.redis.blpop(self.ANIMATION_CTRL_QUEUE_NAME)
+                redis = self._get_redis(transition_seconds)
+                redis.blpop(self.ANIMATION_CTRL_QUEUE_NAME)
                 return True
             except QueueTimeoutError:
                 return False
 
 
         def _animate_thread(lights):
             set_thread_name('HueAnimate')
@@ -679,24 +703,24 @@
                 if stop_animation or \
                         (duration and time.time() - animation_start_time > duration):
                     break
 
                 try:
                     if animation == self.Animation.COLOR_TRANSITION:
                         for (light, attrs) in lights.items():
-                            self.logger.info('Setting {} to {}'.format(light, attrs))
+                            self.logger.debug('Setting {} to {}'.format(light, attrs))
                             self.bridge.set_light(light, attrs)
                             stop_animation = _should_stop()
                             if stop_animation: break
                     elif animation == self.Animation.BLINK:
                         conf = lights[list(lights.keys())[0]]
-                        self.logger.info('Setting lights to {}'.format(conf))
+                        self.logger.debug('Setting lights to {}'.format(conf))
 
                         if groups:
-                            self.bridge.set_group([g.name for f in groups], conf)
+                            self.bridge.set_group([g.name for g in groups], conf)
                         else:
                             self.bridge.set_light(lights.keys(), conf)
 
                         stop_animation = _should_stop()
                         if stop_animation: break
                 except Exception as e:
                     self.logger.warning(e)
@@ -704,28 +728,22 @@
 
                 lights = _next_light_attrs(lights)
 
             self.logger.info('Stopping animation')
             self.animation_thread = None
             self.redis = None
 
-        redis_args = get_backend('redis').redis_args
-        redis_args['socket_timeout'] = transition_seconds
-        self.redis = Redis(**redis_args)
-
-        if groups:
-            groups = [g for g in self.bridge.groups if g.name in groups]
-            lights = lights or []
-            for g in groups:
-                lights.extend([l.name for l in g.lights])
-        elif not lights:
-            lights = self.lights
-
         self.stop_animation()
         self.animation_thread = Thread(target=_animate_thread,
                                        name='HueAnimate',
                                        args=(lights,))
         self.animation_thread.start()
 
+    def _get_redis(self, socket_timeout=1.0):
+        if not self.redis:
+            redis_args = get_backend('redis').redis_args
+            redis_args['socket_timeout'] = socket_timeout
+            self.redis = Redis(**redis_args)
+        return self.redis
 
-# vim:sw=4:ts=4:et:
 
+# vim:sw=4:ts=4:et:
```

### Comparing `platypush-0.9.5/platypush/plugins/logger.py` & `platypush-0.9.6/platypush/plugins/logger.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/media/chromecast.py` & `platypush-0.9.6/platypush/plugins/media/chromecast.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,28 @@
+import datetime
 import re
 import pychromecast
 
 from pychromecast.controllers.youtube import YouTubeController
 
+from platypush.context import get_plugin, get_bus
 from platypush.plugins import Plugin, action
+from platypush.plugins.media import MediaPlugin
+from platypush.utils import get_mime_type
+from platypush.message.event.media import MediaPlayEvent, MediaPlayRequestEvent, \
+    MediaStopEvent, MediaPauseEvent, NewPlayingMediaEvent
 
 
-class MediaChromecastPlugin(Plugin):
+class MediaChromecastPlugin(MediaPlugin):
     """
     Plugin to interact with Chromecast devices
 
     Supported formats:
 
+        * HTTP media URLs
         * YouTube URLs
         * Plex (through ``media.plex`` plugin, experimental)
 
     Requires:
 
         * **pychromecast** (``pip install pychromecast``)
     """
@@ -28,24 +35,30 @@
         """
         :param chromecast: Default Chromecast to cast to if no name is specified
         :type chromecast: str
         """
 
         super().__init__(*args, **kwargs)
 
+        self._is_local = False
         self.chromecast = chromecast
         self.chromecasts = {}
 
 
     @action
     def get_chromecasts(self):
         """
         Get the list of Chromecast devices
         """
 
+        self.chromecasts.update({
+            cast.device.friendly_name: cast
+            for cast in pychromecast.get_chromecasts()
+        })
+
         return [ {
             'type': cc.cast_type,
             'name': cc.name,
             'manufacturer': cc.device.manufacturer,
             'model_name': cc.model_name,
             'uuid': str(cc.device.uuid),
             'address': cc.host,
@@ -53,56 +66,67 @@
 
             'status': ({
                 'app': {
                     'id': cc.app_id,
                     'name': cc.app_display_name,
                 },
 
+                'media': self.status(cc.name).output,
                 'is_active_input': cc.status.is_active_input,
                 'is_stand_by': cc.status.is_stand_by,
                 'is_idle': cc.is_idle,
                 'namespaces': cc.status.namespaces,
                 'volume': round(100*cc.status.volume_level, 2),
                 'muted': cc.status.volume_muted,
             } if cc.status else {}),
-        } for cc in pychromecast.get_chromecasts() ]
+        } for cc in self.chromecasts.values() ]
+
 
+    def get_chromecast(self, chromecast=None, n_tries=3):
+        if isinstance(chromecast, pychromecast.Chromecast):
+            return chromecast
 
-    def get_chromecast(self, chromecast=None):
         if not chromecast:
             if not self.chromecast:
                 raise RuntimeError('No Chromecast specified nor default Chromecast configured')
             chromecast = self.chromecast
 
 
         if chromecast not in self.chromecasts:
-            self.chromecasts = {
-                cast.device.friendly_name: cast
-                for cast in pychromecast.get_chromecasts()
-            }
+            casts = {}
+            while n_tries > 0:
+                n_tries -= 1
+                casts.update({
+                    cast.device.friendly_name: cast
+                    for cast in pychromecast.get_chromecasts()
+                })
+
+                if chromecast in casts:
+                    self.chromecasts.update(casts)
+                    break
 
             if chromecast not in self.chromecasts:
                 raise RuntimeError('Device {} not found'.format(chromecast))
 
         return self.chromecasts[chromecast]
 
 
     @action
-    def cast_media(self, media, content_type=None, chromecast=None, title=None,
+    def play(self, resource, content_type=None, chromecast=None, title=None,
                    image_url=None, autoplay=True, current_time=0,
                    stream_type=STREAM_TYPE_BUFFERED, subtitles=None,
                    subtitles_lang='en-US', subtitles_mime='text/vtt',
                    subtitle_id=1):
         """
         Cast media to a visible Chromecast
 
-        :param media: Media to cast
-        :type media: str
+        :param resource: Media to cast
+        :type resource: str
 
-        :param content_type: Content type
+        :param content_type: Content type as a MIME type string
         :type content_type: str
 
         :param chromecast: Chromecast to cast to. If none is specified, then the default configured Chromecast will be used.
         :type chromecast: str
 
         :param title: Optional title
         :type title: str
@@ -131,128 +155,209 @@
         :param subtitle_id: ID of the subtitles to be loaded (default: 1)
         :type subtitle_id: int
         """
 
         if not chromecast:
             chromecast = self.chromecast
 
+        get_bus().post(MediaPlayRequestEvent(resource=resource,
+                                             device=chromecast))
+
         cast = self.get_chromecast(chromecast)
         cast.wait()
 
         mc = cast.media_controller
-        yt = self._get_youtube_url(media)
+        yt = self._get_youtube_url(resource)
 
         if yt:
             self.logger.info('Playing YouTube video {} on {}'.format(
                 yt, chromecast))
 
             hndl = YouTubeController()
             cast.register_handler(hndl)
             hndl.update_screen_id()
             return hndl.play_video(yt)
 
+        resource = self._get_resource(resource)
+
+        if resource.startswith('magnet:?'):
+            player_args = { 'chromecast': cast }
+            return get_plugin('media.webtorrent').play(resource,
+                                                       player='chromecast',
+                                                       **player_args)
+
+        if not content_type:
+            content_type = get_mime_type(resource)
+
         if not content_type:
             raise RuntimeError('content_type required to process media {}'.
-                               format(media))
+                               format(resource))
+
+        if not resource.startswith('http://') and \
+                not resource.startswith('https://'):
+            resource = self.start_streaming(resource).output['url']
+            self.logger.info('HTTP media stream started on {}'.format(resource))
 
-        self.logger.info('Playing {} on {}'.format(media, chromecast))
+        self.logger.info('Playing {} on {}'.format(resource, chromecast))
 
-        mc.play_media(media, content_type, title=title, thumb=image_url,
+        mc.play_media(resource, content_type, title=title, thumb=image_url,
                       current_time=current_time, autoplay=autoplay,
                       stream_type=stream_type, subtitles=subtitles,
-                      subtitles_lang=subtitles_lang, subtitles_mime=subtitles_mime,
-                      subtitle_id=subtitle_id)
+                      subtitles_lang=subtitles_lang,
+                      subtitles_mime=subtitles_mime, subtitle_id=subtitle_id)
 
         mc.block_until_active()
+        get_bus().post(MediaPlayEvent(resource=resource,
+                                      device=chromecast))
+
 
 
     @classmethod
     def _get_youtube_url(cls, url):
         m = re.match('https?://www.youtube.com/watch\?v=([^&]+).*', url)
         if m:
             return m.group(1)
 
         m = re.match('youtube:video:(.*)', url)
         if m:
             return m.group(1)
 
         return None
 
-
     @action
-    def play(self, chromecast=None):
-        return self.get_chromecast(chromecast or self.chromecast).media_controller.play()
-
+    def load(self, *args, **kwargs):
+        return self.play(*args, **kwargs)
 
     @action
     def pause(self, chromecast=None):
-        return self.get_chromecast(chromecast or self.chromecast).media_controller.pause()
-
-
-    @action
-    def toggle_pause(self, chromecast=None):
         cast = self.get_chromecast(chromecast or self.chromecast)
         if cast.media_controller.is_paused:
-            return cast.media_controller.play()
-        else:
-            return cast.media_controller.pause()
+            ret = cast.media_controller.play()
+            get_bus().post(MediaPlayEvent(device=chromecast or self.chromecast))
+            return ret
+        elif cast.media_controller.is_playing:
+            ret = cast.media_controller.pause()
+            get_bus().post(MediaPauseEvent(device=chromecast or self.chromecast))
+            return ret
 
 
     @action
     def stop(self, chromecast=None):
-        return self.get_chromecast(chromecast or self.chromecast).media_controller.stop()
+        ret = self.get_chromecast(chromecast or self.chromecast).media_controller.stop()
+        get_bus().post(MediaStopEvent(device=chromecast or self.chromecast))
+        return ret
 
 
     @action
     def rewind(self, chromecast=None):
         return self.get_chromecast(chromecast or self.chromecast).media_controller.rewind()
 
 
     @action
-    def seek(self, location, chromecast=None):
-        return self.get_chromecast(chromecast or self.chromecast).media_controller.seek(location)
+    def set_position(self, position, chromecast=None):
+        return self.get_chromecast(chromecast or self.chromecast).media_controller.seek(position)
 
+    @action
+    def seek(self, position, chromecast=None):
+        return self.forward(chromecast=chromecast, offset=position)
 
     @action
-    def back(self, chromecast=None, delta=30):
+    def back(self, chromecast=None, offset=60):
         mc = self.get_chromecast(chromecast or self.chromecast).media_controller
         if mc.status.current_time:
-            return mc.seek(mc.status.current_time-delta)
+            return mc.seek(mc.status.current_time-offset)
 
 
     @action
-    def forward(self, chromecast=None, delta=30):
+    def forward(self, chromecast=None, offset=60):
         mc = self.get_chromecast(chromecast or self.chromecast).media_controller
         if mc.status.current_time:
-            return mc.seek(mc.status.current_time+delta)
+            return mc.seek(mc.status.current_time+offset)
 
 
     @action
     def is_playing(self, chromecast=None):
         return self.get_chromecast(chromecast or self.chromecast).media_controller.is_playing
 
 
     @action
     def is_paused(self, chromecast=None):
         return self.get_chromecast(chromecast or self.chromecast).media_controller.is_paused
 
 
     @action
-    def enable_subtitle(self, chromecast=None):
-        return self.get_chromecast(chromecast or self.chromecast).media_controller.enable_subtitle()
+    def is_idle(self, chromecast=None):
+        return self.get_chromecast(chromecast or self.chromecast).media_controller.is_idle
 
 
     @action
-    def disable_subtitle(self, chromecast=None):
-        return self.get_chromecast(chromecast or self.chromecast).media_controller.disable_subtitle()
+    def list_subtitles(self, chromecast=None):
+        return self.get_chromecast(chromecast or self.chromecast) \
+            .media_controller.subtitle_tracks
+
+
+    @action
+    def enable_subtitles(self, chromecast=None, track_id=None):
+        mc = self.get_chromecast(chromecast or self.chromecast).media_controller
+        if track_id is not None:
+            return mc.enable_subtitle(track_id)
+        elif mc.subtitle_tracks:
+            return mc.enable_subtitle(mc.subtitle_tracks[0].get('trackId'))
+
+
+    @action
+    def disable_subtitles(self, chromecast=None, track_id=None):
+        mc = self.get_chromecast(chromecast or self.chromecast).media_controller
+        if track_name:
+            return mc.disable_subtitle(track_name)
+        elif mc.current_subtitle_tracks:
+            return mc.disable_subtitle(mc.current_subtitle_tracks[0])
+
+    @action
+    def toggle_subtitles(self, chromecast=None):
+        mc = self.get_chromecast(chromecast or self.chromecast).media_controller
+        all_subs = mc.status.subtitle_tracks
+        cur_subs = mc.status.status.current_subtitle_tracks
+
+        if cur_subs:
+            return self.disable_subtitle(chromecast, cur_subs[0])
+        else:
+            return self.enable_subtitle(chromecast, all_subs[0].get('trackId'))
 
 
     @action
     def status(self, chromecast=None):
-        return self.get_chromecast(chromecast or self.chromecast).media_controller.status
+        status = self.get_chromecast(chromecast or self.chromecast) \
+            .media_controller.status
+        attrs = [a for a in dir(status) if not a.startswith('_')
+                 and not callable(getattr(status, a))]
+        renamed_attrs = {
+            'player_state': 'state',
+            'volume_level': 'volume',
+            'volume_muted': 'muted',
+        }
+
+        ret = {}
+        for attr in attrs:
+            value = getattr(status, attr)
+            if attr == 'volume_level':
+                value *= 100
+            if attr == 'player_state':
+                value = value.lower()
+                if value == 'paused': value = 'pause'
+                if value == 'playing': value = 'play'
+            if isinstance(value, datetime.datetime):
+                value = value.isoformat()
+
+            if attr in renamed_attrs:
+                ret[renamed_attrs[attr]] = value
+            else:
+                ret[attr] = value
+
+        return ret
 
 
     @action
     def disconnect(self, chromecast=None, timeout=None, blocking=True):
         """
         Disconnect a Chromecast and wait for it to terminate
 
@@ -284,15 +389,15 @@
         :type blocking: bool
         """
 
         cast = self.get_chromecast(chromecast)
         cast.join(timeout=timeout, blocking=blocking)
 
     @action
-    def quit_app(self, chromecast=None):
+    def quit(self, chromecast=None):
         """
         Exits the current app on the Chromecast
 
         :param chromecast: Chromecast to cast to. If none is specified, then the default configured Chromecast will be used.
         :type chromecast: str
         """
 
@@ -323,55 +428,54 @@
         :type chromecast: str
         """
 
         cast = self.get_chromecast(chromecast)
         cast.set_volume(volume/100)
 
     @action
-    def volume_up(self, chromecast=None, delta=10):
+    def volup(self, chromecast=None, step=10):
         """
-        Turn up the Chromecast volume by 10% or delta.
+        Turn up the Chromecast volume by 10% or step.
 
         :param chromecast: Chromecast to cast to. If none is specified, then the default configured Chromecast will be used.
         :type chromecast: str
 
-        :param delta: Volume increment between 0 and 100 (default: 100%)
-        :type delta: float
+        :param step: Volume increment between 0 and 100 (default: 100%)
+        :type step: float
         """
 
         cast = self.get_chromecast(chromecast)
-        delta /= 100
-        cast.volume_up(min(delta, 1))
+        step /= 100
+        cast.volume_up(min(step, 1))
 
 
     @action
-    def volume_down(self, chromecast=None, delta=10):
+    def voldown(self, chromecast=None, step=10):
         """
-        Turn down the Chromecast volume by 10% or delta.
+        Turn down the Chromecast volume by 10% or step.
 
         :param chromecast: Chromecast to cast to. If none is specified, then the default configured Chromecast will be used.
         :type chromecast: str
 
-        :param delta: Volume decrement between 0 and 100 (default: 100%)
-        :type delta: float
+        :param step: Volume decrement between 0 and 100 (default: 100%)
+        :type step: float
         """
 
         cast = self.get_chromecast(chromecast)
-        delta /= 100
-        cast.volume_down(max(delta, 0))
+        step /= 100
+        cast.volume_down(max(step, 0))
 
 
     @action
-    def toggle_mute(self, chromecast=None):
+    def mute(self, chromecast=None):
         """
         Toggle the mute status on the Chromecast
 
         :param chromecast: Chromecast to cast to. If none is specified, then the default configured Chromecast will be used.
         :type chromecast: str
         """
 
         cast = self.get_chromecast(chromecast)
         cast.set_volume_muted(not cast.status.volume_muted)
 
 
 # vim:sw=4:ts=4:et:
-
```

### Comparing `platypush-0.9.5/platypush/plugins/media/ctrl.py` & `platypush-0.9.6/platypush/plugins/media/ctrl.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 from platypush.plugins import Plugin, action
 
 class MediaCtrlPlugin(Plugin):
     """
     Wrapper plugin to control audio and video media.
     Examples of supported URL types:
-        - file:///media/movies/Movie.mp4 [requires omxplayer Python support]
-        - youtube:video:poAk9XgK7Cs [requires omxplayer+youtube-dl]
+        - file:///media/movies/Movie.mp4 [requires media plugin enabled]
+        - youtube:video:poAk9XgK7Cs [requires media plugin+youtube-dl]
         - magnet:?torrent_magnet [requires torrentcast]
         - spotify:track:track_id [leverages plugins.music.mpd]
     """
 
     _supported_plugins = {
-        'music.mpd', 'video.omxplayer', 'video.torrentcast'
+        'music.mpd', 'media', 'video.torrentcast'
     }
 
     def __init__(self, torrentcast_port=9090, *args, **kwargs):
         super().__init__()
         self.torrentcast_port = torrentcast_port
         self.url = None
         self.plugin = None
@@ -53,15 +53,15 @@
 
         raise RuntimeError('Unknown URL type: {}'.format(url))
 
 
     def _get_playing_plugin(self):
         if self.plugin:
             status = self.plugin.status()
-            if status['state'] == PlayerState.PLAY or state['state'] == PlayerState.PAUSE:
+            if status['state'] == PlayerState.PLAY.value or state['state'] == PlayerState.PAUSE.value:
                 return self.plugin
 
         for plugin in self._supported_plugins:
             try:
                 player = get_plugin(plugin)
             except:
                 try:
@@ -80,15 +80,15 @@
     def play(self, url):
         (type, resource) = self._get_type_and_resource_by_url(url)
         plugin_name = None
 
         if type == 'mpd':
             plugin_name = 'music.mpd'
         elif type == 'youtube:video' or type == 'file':
-            plugin_name = 'video.omxplayer'
+            plugin_name = 'media'
         elif type == 'torrent':
             plugin_name = 'video.torrentcast'
 
         if not plugin_name:
             raise RuntimeError("Unsupported type '{}'".format(type))
 
         try:
```

### Comparing `platypush-0.9.5/platypush/plugins/media/kodi.py` & `platypush-0.9.6/platypush/plugins/media/kodi.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         :type volume: int
         """
 
         result = self._get_kodi().Application.SetVolume(volume=volume)
         return (result.get('result'), result.get('error'))
 
     @action
-    def toggle_mute(self, *args, **kwargs):
+    def mute(self, *args, **kwargs):
         """
         Mute/unmute the application
         """
 
         muted = self._get_kodi().Application.GetProperties(
             properties=['muted']).get('result', {}).get('muted')
 
@@ -314,27 +314,27 @@
         Get the list of albums in the audio library
         """
 
         result = self._get_kodi().Application.GetAlbums()
         return (result.get('result'), result.get('error'))
 
     @action
-    def toggle_fullscreen(self, *args, **kwargs):
+    def fullscreen(self, *args, **kwargs):
         """
         Set/unset fullscreen mode
         """
 
         fullscreen = self._get_kodi().GUI.GetProperties(
             properties=['fullscreen']).get('result', {}).get('fullscreen')
 
         result = self._get_kodi().GUI.SetFullscreen(fullscreen=(not fullscreen))
         return (result.get('result'), result.get('error'))
 
     @action
-    def toggle_shuffle(self, player_id=None, shuffle=None, *args, **kwargs):
+    def shuffle(self, player_id=None, shuffle=None, *args, **kwargs):
         """
         Set/unset shuffle mode
         """
 
         if not player_id:
             player_id = self._get_player_id()
 
@@ -344,15 +344,15 @@
                 properties=['shuffled']).get('result', {}).get('shuffled')
 
         result = self._get_kodi().Player.SetShuffle(
            playerid=player_id,  shuffle=(not shuffle))
         return (result.get('result'), result.get('error'))
 
     @action
-    def toggle_repeat(self, player_id=None, repeat=None, *args, **kwargs):
+    def repeat(self, player_id=None, repeat=None, *args, **kwargs):
         """
         Set/unset repeat mode
         """
 
         if not player_id:
             player_id = self._get_player_id()
```

### Comparing `platypush-0.9.5/platypush/plugins/media/lib/plexcast.py` & `platypush-0.9.6/platypush/plugins/media/lib/plexcast.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/media/plex.py` & `platypush-0.9.6/platypush/plugins/media/plex.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/midi.py` & `platypush-0.9.6/platypush/plugins/midi.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/mqtt.py` & `platypush-0.9.6/platypush/plugins/mqtt.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/music/__init__.py` & `platypush-0.9.6/platypush/plugins/music/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/music/mpd/__init__.py` & `platypush-0.9.6/platypush/plugins/music/mpd/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import mpd
 import re
+import threading
 import time
 
 from platypush.plugins import action
 from platypush.plugins.music import MusicPlugin
 
 class MusicMpdPlugin(MusicPlugin):
     """
@@ -16,14 +17,16 @@
     etc.).
 
     Requires:
 
         * **python-mpd2** (``pip install python-mpd2``)
     """
 
+    _client_lock = threading.RLock()
+
     def __init__(self, host, port=6600):
         """
         :param host: MPD IP/hostname
         :type host: str
 
         :param port: MPD port (default: 6600)
         :type port: int
@@ -37,28 +40,38 @@
     def _connect(self):
         if not self.client:
             self.client = mpd.MPDClient(use_unicode=True)
             self.client.connect(self.host, self.port)
         return self.client
 
     def _exec(self, method, *args, **kwargs):
+        n_tries = int(kwargs.pop('n_tries')) if 'n_tries' in kwargs else 1
         return_status = kwargs.pop('return_status') \
             if 'return_status' in kwargs else True
 
         try:
             self._connect()
-            response = getattr(self.client, method)(*args, **kwargs)
+            response = None
+            with self._client_lock:
+                response = getattr(self.client, method)(*args, **kwargs)
+
             if return_status:
                 return self.status().output
             return response
         except Exception as e:
             self.logger.warning('Exception while executing MPD method {}: {}'.
                                 format(method, str(e)))
             self.client = None
-            return (None, str(e))
+
+            if n_tries > 0:
+                kwargs['return_status'] = return_status
+                kwargs['n_tries'] = n_tries-1
+                return self._exec(method, *args, **kwargs)
+            else:
+                return (None, str(e))
 
     @action
     def play(self, resource=None):
         """
         Play a resource by path/URI
 
         :param resource: Resource path/URI
@@ -166,30 +179,28 @@
 
         :param delta: Volume up delta (default: +10%)
         :type delta: int
         """
 
         volume = int(self.status().output['volume'])
         new_volume = min(volume+delta, 100)
-        self.setvol(str(new_volume))
-        return self.status()
+        return self.setvol(str(new_volume))
 
     @action
     def voldown(self, delta=10):
         """
         Turn down the volume
 
         :param delta: Volume down delta (default: -10%)
         :type delta: int
         """
 
         volume = int(self.status().output['volume'])
         new_volume = max(volume-delta, 0)
-        self.setvol(str(new_volume))
-        return self.status()
+        return self.setvol(str(new_volume))
 
     @action
     def random(self, value=None):
         """
         Set random mode
 
         :param value: If set, set the random state this value (true/false). Default: None (toggle current state)
@@ -249,15 +260,24 @@
 
         if position is None:
             return self._exec('add', r)
         return self._exec('addid', r, position)
 
     @classmethod
     def _parse_resource(cls, resource):
-        if resource and resource.startswith('spotify:playlist:'):
+        if not resource:
+            return
+
+        m = re.search('^https://open.spotify.com/([^?]+)', resource)
+        if m: resource = 'spotify:{}'.format(m.group(1).replace('/', ':'))
+
+        if resource.startswith('spotify:'):
+            resource = resource.split('?')[0]
+
+        if resource.startswith('spotify:playlist:'):
             # Old Spotify URI format, convert it to new
             m = re.match('^spotify:playlist:(.*)$', resource)
             resource = 'spotify:user:spotify:playlist:' + m.group(1)
         return resource
 
     @action
     def load(self, playlist):
@@ -435,17 +455,16 @@
 
     @action
     def lsinfo(self, uri=None):
         """
         Returns the list of playlists and directories on the server
         """
 
-        output = self._exec('lsinfo', uri, return_status=False) \
+        return self._exec('lsinfo', uri, return_status=False) \
             if uri else self._exec('lsinfo', return_status=False)
-        return output
 
     @action
     def plchanges(self, version):
         """
         Show what has changed on the current playlist since a specified playlist
         version number.
```

### Comparing `platypush-0.9.5/platypush/plugins/music/snapcast.py` & `platypush-0.9.6/platypush/plugins/music/snapcast.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         request = {
             'id': self._get_req_id(),
             'jsonrpc':'2.0',
             'method':'Server.GetStatus'
         }
 
         self._send(sock, request)
-        return self._recv(sock).get('server', {})
+        return (self._recv(sock) or {}).get('server', {})
 
     @action
     def status(self, host=None, port=None, client=None, group=None):
         """
         Get the status either of a Snapcast server, client or group
 
         :param host: Snapcast server to query (default: default configured host)
```

### Comparing `platypush-0.9.5/platypush/plugins/pushbullet.py` & `platypush-0.9.6/platypush/plugins/pushbullet.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/redis.py` & `platypush-0.9.6/platypush/plugins/redis.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/serial/__init__.py` & `platypush-0.9.6/platypush/plugins/serial/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/shell/__init__.py` & `platypush-0.9.6/platypush/plugins/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/sound/__init__.py` & `platypush-0.9.6/platypush/plugins/sound/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 import tempfile
 import time
 
 from enum import Enum
 from threading import Thread, Event, RLock
 
 from .core import Sound, Mix
+
+from platypush.context import get_bus
+from platypush.message.event.sound import SoundPlaybackStartedEvent, \
+    SoundPlaybackPausedEvent, SoundPlaybackStoppedEvent, \
+    SoundRecordingStartedEvent, SoundRecordingPausedEvent, \
+    SoundRecordingStoppedEvent
+
 from platypush.plugins import Plugin, action
 
 
 class PlaybackState(Enum):
     STOPPED='STOPPED',
     PLAYING='PLAYING',
     PAUSED='PAUSED'
@@ -28,14 +35,23 @@
     PAUSED='PAUSED'
 
 
 class SoundPlugin(Plugin):
     """
     Plugin to interact with a sound device.
 
+    Triggers:
+
+        * :class:`platypush.message.event.sound.SoundPlaybackStartedEvent` on playback start
+        * :class:`platypush.message.event.sound.SoundPlaybackStoppedEvent` on playback stop
+        * :class:`platypush.message.event.sound.SoundPlaybackPausedEvent` on playback pause
+        * :class:`platypush.message.event.sound.SoundRecordingStartedEvent` on recording start
+        * :class:`platypush.message.event.sound.SoundRecordingStoppedEvent` on recording stop
+        * :class:`platypush.message.event.sound.SoundRecordingPausedEvent` on recording pause
+
     Requires:
 
         * **sounddevice** (``pip install sounddevice``)
         * **soundfile** (``pip install soundfile``)
         * **numpy** (``pip install numpy``)
     """
 
@@ -380,21 +396,21 @@
                 f.close()
                 f = None
 
             self.stop_playback([stream_index])
 
 
     @action
-    def record(self, file=None, duration=None, device=None, sample_rate=None,
+    def record(self, outfile=None, duration=None, device=None, sample_rate=None,
                blocksize=None, latency=0, channels=1, subtype='PCM_24'):
         """
         Records audio to a sound file (support formats: wav, raw)
 
-        :param file: Sound file (default: the method will create a temporary file with the recording)
-        :type file: str
+        :param outfile: Sound file (default: the method will create a temporary file with the recording)
+        :type outfile: str
 
         :param duration: Recording duration in seconds (default: record until stop event)
         :type duration: float
 
         :param device: Input device (default: default configured device or system default audio input if not configured)
         :type device: int or str
 
@@ -410,89 +426,98 @@
         :param channels: Number of channels (default: 1)
         :type channels: int
 
         :param subtype: Recording subtype - see `soundfile docs <https://pysoundfile.readthedocs.io/en/0.9.0/#soundfile.available_subtypes>`_ for a list of the available subtypes (default: PCM_24)
         :type subtype: str
         """
 
-        import sounddevice as sd
+        def recording_thread(outfile, duration, device, sample_rate, blocksize,
+                             latency, channels, subtype):
+            import sounddevice as sd
 
-        self.recording_paused_changed.clear()
+            self.recording_paused_changed.clear()
 
-        if file:
-            file = os.path.abspath(os.path.expanduser(file))
-        else:
-            file = tempfile.mktemp(prefix='platypush_recording_', suffix='.wav',
-                                   dir='')
-
-        if os.path.isfile(file):
-            self.logger.info('Removing existing audio file {}'.format(file))
-            os.unlink(file)
-
-        if device is None:
-            device = self.input_device
-        if device is None:
-            device = self._get_default_device('input')
+            if outfile:
+                outfile = os.path.abspath(os.path.expanduser(outfile))
+            else:
+                outfile = tempfile.NamedTemporaryFile(
+                    prefix='recording_', suffix='.wav', delete=False,
+                    dir=tempfile.gettempdir()).name
 
-        if sample_rate is None:
-            dev_info = sd.query_devices(device, 'input')
-            sample_rate = int(dev_info['default_samplerate'])
+            if os.path.isfile(outfile):
+                self.logger.info('Removing existing audio file {}'.format(outfile))
+                os.unlink(outfile)
 
-        if blocksize is None:
-            blocksize = self.input_blocksize
+            if device is None:
+                device = self.input_device
+            if device is None:
+                device = self._get_default_device('input')
 
-        q = queue.Queue()
+            if sample_rate is None:
+                dev_info = sd.query_devices(device, 'input')
+                sample_rate = int(dev_info['default_samplerate'])
 
-        def audio_callback(indata, frames, time, status):
-            while self._get_recording_state() == RecordingState.PAUSED:
-                self.recording_paused_changed.wait()
+            if blocksize is None:
+                blocksize = self.input_blocksize
 
-            if status:
-                self.logger.warning('Recording callback status: {}'.format(
-                    str(status)))
+            q = queue.Queue()
 
-            q.put(indata.copy())
+            def audio_callback(indata, frames, time, status):
+                while self._get_recording_state() == RecordingState.PAUSED:
+                    self.recording_paused_changed.wait()
 
+                if status:
+                    self.logger.warning('Recording callback status: {}'.format(
+                        str(status)))
 
-        try:
-            import soundfile as sf
-            import numpy
-
-            with sf.SoundFile(file, mode='x', samplerate=sample_rate,
-                              channels=channels, subtype=subtype) as f:
-                with sd.InputStream(samplerate=sample_rate, device=device,
-                                    channels=channels, callback=audio_callback,
-                                    latency=latency, blocksize=blocksize):
-                    self.start_recording()
-                    self.logger.info('Started recording from device [{}] to [{}]'.
-                                    format(device, file))
-
-                    recording_started_time = time.time()
-
-                    while self._get_recording_state() != RecordingState.STOPPED \
-                            and (duration is None or
-                                 time.time() - recording_started_time < duration):
-                        while self._get_recording_state() == RecordingState.PAUSED:
-                            self.recording_paused_changed.wait()
-
-                        get_args = {
-                            'block': True,
-                            'timeout': max(0, duration - (time.time() -
-                                                          recording_started_time))
-                        } if duration is not None else {}
+                q.put(indata.copy())
 
-                        data = q.get(**get_args)
-                        f.write(data)
 
-                f.flush()
+            try:
+                import soundfile as sf
+                import numpy
 
-        except queue.Empty as e:
-            self.logger.warning('Recording timeout: audio callback failed?')
-        finally:
-            self.stop_recording()
+                with sf.SoundFile(outfile, mode='x', samplerate=sample_rate,
+                                channels=channels, subtype=subtype) as f:
+                    with sd.InputStream(samplerate=sample_rate, device=device,
+                                        channels=channels, callback=audio_callback,
+                                        latency=latency, blocksize=blocksize):
+                        self.start_recording()
+                        get_bus().post(SoundRecordingStartedEvent(filename=outfile))
+                        self.logger.info('Started recording from device [{}] to [{}]'.
+                                        format(device, outfile))
+
+                        recording_started_time = time.time()
+
+                        while self._get_recording_state() != RecordingState.STOPPED \
+                                and (duration is None or
+                                    time.time() - recording_started_time < duration):
+                            while self._get_recording_state() == RecordingState.PAUSED:
+                                self.recording_paused_changed.wait()
+
+                            get_args = {
+                                'block': True,
+                                'timeout': max(0, duration - (time.time() -
+                                                            recording_started_time))
+                            } if duration is not None else {}
+
+                            data = q.get(**get_args)
+                            f.write(data)
+
+                    f.flush()
+
+            except queue.Empty as e:
+                self.logger.warning('Recording timeout: audio callback failed?')
+            finally:
+                self.stop_recording()
+                get_bus().post(SoundRecordingStoppedEvent(filename=outfile))
+
+        Thread(target=recording_thread, args=(
+            outfile, duration, device, sample_rate, blocksize, latency, channels,
+            subtype)).start()
 
 
     @action
     def recordplay(self, duration=None, input_device=None, output_device=None,
                    sample_rate=None, blocksize=None, latency=0, channels=1,
                    dtype=None):
         """
```

### Comparing `platypush-0.9.5/platypush/plugins/sound/core.py` & `platypush-0.9.6/platypush/plugins/sound/core.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/switch/__init__.py` & `platypush-0.9.6/platypush/plugins/switch/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/switch/switchbot/__init__.py` & `platypush-0.9.6/platypush/plugins/switch/switchbot/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/switch/switchbot/__main__.py` & `platypush-0.9.6/platypush/plugins/switch/switchbot/__main__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/switch/tplink.py` & `platypush-0.9.6/platypush/plugins/switch/tplink.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/switch/wemo/__init__.py` & `platypush-0.9.6/platypush/plugins/switch/wemo/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/torrent.py` & `platypush-0.9.6/platypush/plugins/torrent.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/tts/__init__.py` & `platypush-0.9.6/platypush/plugins/tts/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/tts/google.py` & `platypush-0.9.6/platypush/plugins/tts/google.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/variable.py` & `platypush-0.9.6/platypush/plugins/variable.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/video/omxplayer.py` & `platypush-0.9.6/platypush/plugins/media/vlc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,498 +1,406 @@
-import json
 import os
 import re
-import subprocess
-import time
+import threading
 
-import urllib.request
-import urllib.parse
+from platypush.context import get_bus, get_plugin
+from platypush.plugins.media import PlayerState, MediaPlugin
+from platypush.message.event.media import MediaPlayEvent, MediaPlayRequestEvent, \
+    MediaPauseEvent, MediaStopEvent, MediaSeekEvent, MediaVolumeChangedEvent, \
+    MediaMuteChangedEvent, NewPlayingMediaEvent
 
-from platypush.context import get_backend, get_plugin
-from platypush.plugins.media import PlayerState
-from platypush.message.event.video import VideoPlayEvent, VideoPauseEvent, \
-    VideoStopEvent, NewPlayingVideoEvent
+from platypush.plugins import action
 
-from platypush.plugins import Plugin, action
 
-
-class VideoOmxplayerPlugin(Plugin):
+class MediaVlcPlugin(MediaPlugin):
     """
-    Plugin to control video and media playback on your Raspberry Pi or
-    ARM-compatible device using OMXPlayer.
-
-    It can play local files, remote URLs, YouTube URLs and it supports torrents
-    search, download and play.
+    Plugin to control vlc instances
 
     Requires:
 
-        * **omxplayer** installed on your system (see your distro instructions)
-        * **omxplayer-wrapper** (``pip install omxplayer-wrapper``)
-        * **python-libtorrent** (``pip install python-libtorrent``), optional for Torrent support
-        * **youtube-dl** installed on your system (see your distro instructions), optional for YouTube support
+        * **python-vlc** (``pip install python-vlc``)
+        * **vlc** executable on your system
     """
 
-    # Supported video extensions
-    video_extensions = {
-        '.avi', '.flv', '.wmv', '.mov', '.mp4', '.m4v', '.mpg', '.mpeg',
-        '.rm', '.swf', '.vob', '.mkv'
-    }
-
-    def __init__(self, args=[], media_dirs=[], download_dir=None, *argv, **kwargs):
+    def __init__(self, args=None, fullscreen=False, volume=100, *argv, **kwargs):
         """
-        :param args: Arguments that will be passed to the OMXPlayer constructor (e.g. subtitles, volume, start position, window size etc.) see https://github.com/popcornmix/omxplayer#synopsis and http://python-omxplayer-wrapper.readthedocs.io/en/latest/omxplayer/#omxplayer.player.OMXPlayer
-        :type args: list
+        Create the vlc wrapper.
 
-        :param media_dirs: Directories that will be scanned for media files when a search is performed (default: none)
-        :type media_dirs: list
+        :param args: List of extra arguments to pass to the VLC executable (e.g.
+            ``['--sub-language=en', '--snapshot-path=/mnt/snapshots']``)
+        :type args: list[str]
 
-        :param download_dir: Directory where the videos/torrents will be downloaded (default: none)
-        :type download_dir: str
+        :param fullscreen: Set to True if you want media files to be opened in
+            fullscreen by default (can be overridden by `.play()`) (default: False)
+        :type fullscreen: bool
+
+        :param volume: Default media volume (default: 100)
+        :type volume: int
         """
 
         super().__init__(*argv, **kwargs)
 
-        self.args = args
-        self.media_dirs = set(
-            filter(
-                lambda _: os.path.isdir(_),
-                map(
-                    lambda _: os.path.abspath(os.path.expanduser(_)),
-                    media_dirs
-                )
-            )
-        )
-
-        if download_dir:
-            self.download_dir = os.path.abspath(os.path.expanduser(download_dir))
-            if not os.path.isdir(self.download_dir):
-                raise RuntimeError('download_dir [{}] is not a valid directory'
-                                   .format(self.download_dir))
+        self._args = args or []
+        self._instance = None
+        self._player = None
+        self._latest_seek = None
+        self._default_fullscreen = fullscreen
+        self._default_volume = volume
+        self._on_stop_callbacks = []
 
-            self.media_dirs.add(self.download_dir)
 
-        self.player = None
-        self.videos_queue = []
+    @classmethod
+    def _watched_event_types(cls):
+        import vlc
+        return [getattr(vlc.EventType, evt) for evt in [
+            'MediaPlayerLengthChanged', 'MediaPlayerMediaChanged',
+            'MediaDurationChanged', 'MediaPlayerMuted',
+            'MediaPlayerUnmuted', 'MediaPlayerOpening', 'MediaPlayerPaused',
+            'MediaPlayerPlaying', 'MediaPlayerPositionChanged',
+            'MediaPlayerStopped', 'MediaPlayerTimeChanged', 'MediaStateChanged',
+            'MediaPlayerForward', 'MediaPlayerBackward',
+            'MediaPlayerEndReached', 'MediaPlayerTitleChanged',
+            'MediaPlayerAudioVolume',
+        ] if hasattr(vlc.EventType, evt)]
+
+    def _init_vlc(self, resource):
+        import vlc
+        self._reset_state()
+
+        for k,v in self._env.items():
+            os.environ[k] = v
+
+        self._instance = vlc.Instance(*self._args)
+        self._player = self._instance.media_player_new(resource)
+
+        for evt in self._watched_event_types():
+            self._player.event_manager().event_attach(
+                eventtype=evt, callback=self._event_callback())
+
+    def _reset_state(self):
+        self._latest_seek = None
+        if self._player:
+            self._player.release()
+            self._player = None
+
+        if self._instance:
+            self._instance.release()
+            self._instance = None
+
+    def _event_callback(self):
+        def callback(event):
+            from vlc import EventType
+            self.logger.debug('Received vlc event: {}'.format(event))
+            bus = get_bus()
+
+            if event.type == EventType.MediaPlayerPlaying:
+                bus.post(MediaPlayEvent(resource=self._get_current_resource()))
+            elif event.type == EventType.MediaPlayerPaused:
+                bus.post(MediaPauseEvent())
+            elif event.type == EventType.MediaPlayerStopped or \
+                event.type == EventType.MediaPlayerEndReached:
+                self._reset_state()
+                bus.post(MediaStopEvent())
+                for callback in self._on_stop_callbacks:
+                    callback()
+            elif event.type == EventType.MediaPlayerTitleChanged:
+                bus.post(NewPlayingMediaEvent(resource=event.u.new_title))
+            elif event.type == EventType.MediaPlayerMediaChanged:
+                bus.post(NewPlayingMediaEvent(resource=event.u.filename))
+            elif event.type == EventType.MediaPlayerLengthChanged:
+                bus.post(NewPlayingMediaEvent(resource=self._get_current_resource()))
+            elif event.type == EventType.MediaPlayerTimeChanged:
+                pos = float(event.u.new_time/1000)
+                if self._latest_seek is None or \
+                        abs(pos-self._latest_seek) > 5:
+                    bus.post(MediaSeekEvent(position=pos))
+                self._latest_seek = pos
+            elif event.type == EventType.MediaPlayerAudioVolume:
+                bus.post(MediaVolumeChangedEvent(volume=self._player.audio_get_volume()))
+            elif event.type == EventType.MediaPlayerMuted:
+                bus.post(MediaMuteChangedEvent(mute=True))
+            elif event.type == EventType.MediaPlayerUnmuted:
+                bus.post(MediaMuteChangedEvent(mute=False))
+
+        return callback
+
 
     @action
-    def play(self, resource):
+    def play(self, resource, subtitles=None, fullscreen=None, volume=None):
         """
         Play a resource.
 
-        :param resource: Resource to play. Supported types:
+        :param resource: Resource to play - can be a local file or a remote URL
+        :type resource: str
 
-            * Local files (format: ``file://<path>/<file>``)
-            * Remote videos (format: ``https://<url>/<resource>``)
-            * YouTube videos (format: ``https://www.youtube.com/watch?v=<id>``)
-            * Torrents (format: Magnet links, Torrent URLs or local Torrent files)
-        """
+        :param subtitles: Path to optional subtitle file
+        :type subtitles: str
 
-        from dbus.exceptions import DBusException
+        :param fullscreen: Set to explicitly enable/disable fullscreen (default:
+            `fullscreen` configured value or False)
+        :type fullscreen: bool
 
-        if resource.startswith('youtube:') \
-                or resource.startswith('https://www.youtube.com/watch?v='):
-            resource = self._get_youtube_content(resource)
-        elif resource.startswith('magnet:?'):
-            torrents = get_plugin('torrent')
-            response = torrents.download(resource, download_dir=self.download_dir)
-            resources = [f for f in response.output if self._is_video_file(f)]
-            if resources:
-                self.videos_queue = sorted(resources)
-                resource = self.videos_queue.pop(0)
-            else:
-                raise RuntimeError('Unable to download torrent {}'.format(resource))
-
-        self.logger.info('Playing {}'.format(resource))
-
-        if self.player:
-            try:
-                self.player.stop()
-                self.player = None
-            except Exception as e:
-                self.logger.exception(e)
-                self.logger.warning('Unable to stop a previously running instance ' +
-                                'of OMXPlayer, trying to play anyway')
-
-        try:
-            from omxplayer import OMXPlayer
-            self.player = OMXPlayer(resource, args=self.args)
-            self._init_player_handlers()
-        except DBusException as e:
-            self.logger.warning('DBus connection failed: you will probably not ' +
-                            'be able to control the media')
-            self.logger.exception(e)
+        :param volume: Set to explicitly set the playback volume (default:
+            `volume` configured value or 100)
+        :type fullscreen: bool
+        """
 
-        return self.status()
+        get_bus().post(MediaPlayRequestEvent(resource=resource))
+        resource = self._get_resource(resource)
 
-    @action
-    def pause(self):
-        """ Pause the playback """
-        if self.player: self.player.play_pause()
+        if resource.startswith('file://'):
+            resource = resource[len('file://'):]
+        elif resource.startswith('magnet:?'):
+            self._is_playing_torrent = True
+            return get_plugin('media.webtorrent').play(resource)
 
-    @action
-    def stop(self):
-        """ Stop the playback """
-        if self.player:
-            self.player.stop()
-            self.player.quit()
-            self.player = None
-
-        return {'status':'stop'}
+        self._init_vlc(resource)
+        if subtitles:
+            if subtitles.startswith('file://'):
+                subtitles = subtitles[len('file://'):]
+            self._player.video_set_subtitle_file(subtitles)
+
+        self._is_playing_torrent = False
+        self._player.play()
+
+        if fullscreen or self._default_fullscreen:
+            self.set_fullscreen(True)
+
+        if volume is not None or self._default_volume is not None:
+            self.set_volume(volume if volume is not None
+                            else self._default_volume)
 
-    @action
-    def voldown(self):
-        """ Volume down by 10% """
-        if self.player:
-            self.player.set_volume(max(-6000, self.player.volume()-1000))
         return self.status()
 
-    @action
-    def volup(self):
-        """ Volume up by 10% """
-        if self.player:
-            self.player.set_volume(min(0, self.player.volume()+1000))
-        return self.status()
 
     @action
-    def back(self):
-        """ Back by 30 seconds """
-        if self.player:
-            self.player.seek(-30)
-        return self.status()
+    def pause(self):
+        """ Toggle the paused state """
+        if not self._player:
+            return (None, 'No vlc instance is running')
+        if not self._player.can_pause():
+            return (None, 'The specified media type cannot be paused')
 
-    @action
-    def forward(self):
-        """ Forward by 30 seconds """
-        if self.player:
-            self.player.seek(+30)
+        self._player.pause()
         return self.status()
 
     @action
-    def next(self):
-        """ Play the next track/video """
-        if self.player:
-            self.player.stop()
-
-        if self.videos_queue:
-            video = self.videos_queue.pop(0)
-            return self.play(video)
+    def quit(self):
+        """ Quit the player (same as `stop`) """
+        self._stop_torrent()
+        if not self._player:
+            return (None, 'No vlc instance is running')
 
-    @action
-    def hide_subtitles(self):
-        """ Hide the subtitles """
-        if self.player: self.player.hide_subtitles()
-        return self.status()
+        self._player.stop()
+        return { 'state': PlayerState.STOP.value }
 
     @action
-    def hide_video(self):
-        """ Hide the video """
-        if self.player: self.player.hide_video()
-        return self.status()
+    def stop(self):
+        """ Stop the application (same as `quit`) """
+        return self.quit()
 
     @action
-    def is_playing(self):
-        """
-        :returns: True if it's playing, False otherwise
-        """
-
-        if self.player: return self.player.is_playing()
-        else: return False
+    def voldown(self, step=10.0):
+        """ Volume down by (default: 10)% """
+        if not self._player:
+            return (None, 'No vlc instance is running')
+        return self.set_volume(self._player.audio_get_volume()-step)
+
+    @action
+    def volup(self, step=10.0):
+        """ Volume up by (default: 10)% """
+        if not self._player:
+            return (None, 'No vlc instance is running')
+        return self.set_volume(self._player.audio_get_volume()+step)
 
     @action
-    def load(self, resource, pause=False):
+    def set_volume(self, volume):
         """
-        Load a resource/video in the player.
+        Set the volume
 
-        :param pause: If set, load the video in paused mode (default: False)
-        :type pause: bool
+        :param volume: Volume value between 0 and 100
+        :type volume: float
         """
+        if not self._player:
+            return (None, 'No vlc instance is running')
 
-        if self.player: self.player.load(resource, pause)
-        return self.status()
-
-    @action
-    def metadata(self):
-        """ Get the metadata of the current video """
-        if self.player:
-            return self.player.metadata()
-        return self.status()
-
-    @action
-    def mute(self):
-        """ Mute the player """
-        if self.player: self.player.mute()
-        return self.status()
-
-    @action
-    def unmute(self):
-        """ Unmute the player """
-        if self.player: self.player.unmute()
-        return self.status()
+        volume = max(0, min(100, volume))
+        self._player.audio_set_volume(volume)
+        return { 'volume': volume }
 
     @action
-    def seek(self, relative_position):
+    def seek(self, position):
         """
         Seek backward/forward by the specified number of seconds
 
         :param relative_position: Number of seconds relative to the current cursor
         :type relative_position: int
         """
+        if not self._player:
+            return (None, 'No vlc instance is running')
+        if not self._player.is_seekable():
+            return (None, 'The resource is not seekable')
 
-        if self.player: self.player.seek(relative_position)
-        return self.status()
-
-    @action
-    def set_position(self, position):
-        """
-        Seek backward/forward to the specified absolute position
-
-        :param position: Number of seconds from the start
-        :type position: int
-        """
+        media = self._player.get_media()
+        if not media:
+            return (None, 'No media loaded')
 
-        if self.player: self.player.set_seek(position)
-        return self.status()
+        pos = min(media.get_duration()/1000, max(0, position))
+        self._player.set_time(int(pos*1000))
+        return { 'position': pos }
 
     @action
-    def set_volume(self, volume):
-        """
-        Set the volume
+    def back(self, offset=60.0):
+        """ Back by (default: 60) seconds """
+        if not self._player:
+            return (None, 'No vlc instance is running')
 
-        :param volume: Volume value between 0 and 100
-        :type volume: int
-        """
+        media = self._player.get_media()
+        if not media:
+            return (None, 'No media loaded')
 
-        # Transform a [0,100] value to an OMXPlayer volume in [-6000,0]
-        volume = 60.0*volume - 6000
-        if self.player: self.player.set_volume(volume)
-        return self.status()
+        pos = max(0, (self._player.get_time()/1000)-offset)
+        return self.seek(pos)
 
     @action
-    def status(self):
-        """
-        Get the current player state.
+    def forward(self, offset=60.0):
+        """ Forward by (default: 60) seconds """
+        if not self._player:
+            return (None, 'No vlc instance is running')
 
-        :returns: A dictionary containing the current state.
+        media = self._player.get_media()
+        if not media:
+            return (None, 'No media loaded')
 
-        Example::
+        pos = min(media.get_duration()/1000, (self._player.get_time()/1000)+offset)
+        return self.seek(pos)
 
-            output = {
-                "source": "https://www.youtube.com/watch?v=7L9KkZoNZkA",
-                "state": "play",
-                "volume": 80,
-                "elapsed": 123,
-                "duration": 300,
-                "width": 800,
-                "height": 600
-            }
-        """
+    @action
+    def toggle_subtitles(self, visibile=None):
+        """ Toggle the subtitles visibility """
+        if not self._player:
+            return (None, 'No vlc instance is running')
 
-        state = PlayerState.STOP.value
+        if self._player.video_get_spu_count() == 0:
+            return (None, 'The media file has no subtitles set')
 
-        if self.player:
-            state = self.player.playback_status().lower()
-            if state == 'playing': state = PlayerState.PLAY.value
-            elif state == 'stopped': state = PlayerState.STOP.value
-            elif state == 'paused': state = PlayerState.PAUSE.value
-
-            return {
-                'source': self.player.get_source(),
-                'state': state,
-                'volume': self.player.volume(),
-                'elapsed': self.player.position(),
-                'duration': self.player.duration(),
-                'width': self.player.width(),
-                'height': self.player.height(),
-            }
+        if self._player.video_get_spu() is None or \
+                self._player.video_get_spu() == -1:
+            self._player.video_set_spu(0)
         else:
-            return {
-                'state': PlayerState.STOP.value
-            }
+            self._player.video_set_spu(-1)
 
     @action
-    def send_message(self, msg):
-        try:
-            redis = get_backend('redis')
-            if not redis:
-                raise KeyError()
-        except KeyError:
-            self.logger.warning("Backend {} does not implement send_message " +
-                                "and the fallback Redis backend isn't configured")
-            return
-
-        redis.send_message(msg)
+    def toggle_fullscreen(self):
+        """ Toggle the fullscreen mode """
+        if not self._player:
+            return (None, 'No vlc instance is running')
+        self._player.toggle_fullscreen()
 
-    def on_play(self):
-        def _f(player):
-            self.send_message(VideoPlayEvent(video=self.player.get_source()))
-        return _f
-
-    def on_pause(self):
-        def _f(player):
-            self.send_message(VideoPauseEvent(video=self.player.get_source()))
-        return _f
-
-    def on_stop(self):
-        def _f(player):
-            self.send_message(VideoStopEvent())
-        return _f
+    @action
+    def set_fullscreen(self, fullscreen=True):
+        """ Set fullscreen mode """
+        if not self._player:
+            return (None, 'No vlc instance is running')
+        self._player.set_fullscreen(fullscreen)
 
+    @action
+    def set_subtitles(self, filename):
+        """ Sets media subtitles from filename """
+        if not self._player:
+            return (None, 'No vlc instance is running')
+        if filename.startswith('file://'):
+            filename = filename[len('file://'):]
 
-    def _init_player_handlers(self):
-        if not self.player:
-            return
+        self._player.video_set_subtitle_file(filename)
 
-        self.player.playEvent += self.on_play()
-        self.player.pauseEvent += self.on_pause()
-        self.player.stopEvent += self.on_stop()
+    @action
+    def remove_subtitles(self):
+        """ Removes (hides) the subtitles """
+        if not self._player:
+            return (None, 'No vlc instance is running')
+        self._player.video_set_spu(-1)
 
     @action
-    def search(self, query, types=None, queue_results=False, autoplay=False):
+    def is_playing(self):
         """
-        Perform a video search.
-
-        :param query: Query string, video name or partial name
-        :type query: str
-
-        :param types: Video types to search (default: ``["youtube", "file", "torrent"]``)
-        :type types: list
-
-        :param queue_results: Append the results to the current playing queue (default: False)
-        :type queue_results: bool
-
-        :param autoplay: Play the first result of the search (default: False)
-        :type autoplay: bool
+        :returns: True if it's playing, False otherwise
         """
-
-        results = []
-        if types is None:
-            types = { 'youtube', 'file', 'torrent' }
-
-        if 'file' in types:
-            file_results = self.file_search(query).output
-            results.extend(file_results)
-
-        if 'torrent' in types:
-            torrents = get_plugin('torrent')
-            torrent_results = torrents.search(query).output
-            results.extend(torrent_results)
-
-        if 'youtube' in types:
-            yt_results = self.youtube_search(query).output
-            results.extend(yt_results)
-
-        if results:
-            if queue_results:
-                self.videos_queue = [_['url'] for _ in results]
-                if autoplay:
-                    self.play(self.videos_queue.pop(0))
-            elif autoplay:
-                self.play(results[0]['url'])
-
-        return results
-
-    @classmethod
-    def _is_video_file(cls, filename):
-        is_video = False
-        for ext in cls.video_extensions:
-            if filename.lower().endswith(ext):
-                is_video = True
-                break
-
-        return is_video
+        if not self._player:
+            return False
+        return self._player.is_playing()
 
     @action
-    def file_search(self, query):
-        results = []
-        query_tokens = [_.lower() for _ in re.split('\s+', query.strip())]
-
-        for media_dir in self.media_dirs:
-            self.logger.info('Scanning {} for "{}"'.format(media_dir, query))
-            for path, dirs, files in os.walk(media_dir):
-                for f in files:
-                    if not self._is_video_file(f):
-                        continue
-
-                    matches_query = True
-                    for token in query_tokens:
-                        if token not in f.lower():
-                            matches_query = False
-                            break
-
-                    if not matches_query:
-                        continue
-
-                    results.append({
-                        'url': 'file://' + path + os.sep + f,
-                        'title': f,
-                    })
+    def load(self, resource, **args):
+        """
+        Load/queue a resource/video to the player
+        """
+        if not self._player:
+            return self.play(resource, **args)
+        return self._player.set_media(resource)
 
-        return results
+    @action
+    def mute(self):
+        """ Toggle mute state """
+        if not self._player:
+            return (None, 'No vlc instance is running')
+        self._player.audio_toggle_mute()
 
     @action
-    def youtube_search(self, query):
+    def set_position(self, position):
         """
-        Performs a YouTube search either using the YouTube API (faster and
-        recommended, it requires the :mod:`platypush.plugins.google.youtube`
-        plugin to be configured) or parsing the HTML search results (fallback
-        slower method)
+        Seek backward/forward to the specified absolute position (same as ``seek``)
         """
+        return self.seek(position)
 
-        self.logger.info('Searching YouTube for "{}"'.format(query))
-
-        try:
-            return self._youtube_search_api(query=query)
-        except Exception as e:
-            self.logger.warning('Unable to load the YouTube plugin, falling ' +
-                                'back to HTML parse method: {}'.format(str(e)))
+    @action
+    def status(self):
+        """
+        Get the current player state.
 
-            return self._youtube_search_html_parse(query=query)
+        :returns: A dictionary containing the current state.
 
+        Example::
 
-    def _youtube_search_api(self, query):
-        return [
-            {
-                'url': 'https://www.youtube.com/watch?v=' + item['id']['videoId'],
-                'title': item.get('snippet', {}).get('title', '<No Title>'),
+            output = {
+                "filename": "filename or stream URL",
+                "state": "play"  # or "stop" or "pause"
             }
-            for item in get_plugin('google.youtube').search(query=query).output
-            if item.get('id', {}).get('kind') == 'youtube#video'
-        ]
-
-    def _youtube_search_html_parse(self, query):
-        query = urllib.parse.quote(query)
-        url = "https://www.youtube.com/results?search_query=" + query
-        response = urllib.request.urlopen(url)
-        html = response.read().decode('utf-8')
-        results = []
-
-        while html:
-            m = re.search('(<a href="(/watch\?v=.+?)".+?yt-uix-tile-link.+?title="(.+?)".+?>)', html)
-            if m:
-                results.append({
-                    'url': 'https://www.youtube.com' + m.group(2),
-                    'title': m.group(3)
-                })
-
-                html = html.split(m.group(1))[1]
-            else:
-                html = ''
-
-        self.logger.info('{} YouTube video results for the search query "{}"'
-                     .format(len(results), query))
+        """
+        import vlc
+        if not self._player:
+            return { 'state': PlayerState.STOP.value }
 
-        return results
+        vlc_state = self._player.get_state()
+        state = PlayerState.STOP.value
+        filename = self._player.get_media().get_mrl() \
+            if self._player.get_media() else None
 
+        if vlc_state == vlc.State.Playing:
+            state = PlayerState.PLAY.value
+        if vlc_state == vlc.State.Paused:
+            state = PlayerState.PAUSE.value
+
+        time = float(self._player.get_time()/1000) if self._player.get_time() \
+            is not None else None
+
+        media = self._player.get_media()
+        duration = media.get_duration()/1000 if media and media.get_duration() \
+            is not None else None
+
+        return {
+            'filename': filename,
+            'state': state,
+            'time': time,
+            'duration': duration,
+        }
 
-    @classmethod
-    def _get_youtube_content(cls, url):
-        m = re.match('youtube:video:(.*)', url)
-        if m: url = 'https://www.youtube.com/watch?v={}'.format(m.group(1))
+    def on_stop(self, callback):
+        self._on_stop_callbacks.append(callback)
 
-        proc = subprocess.Popen(['youtube-dl','-f','best', '-g', url],
-                                stdout=subprocess.PIPE)
-
-        return proc.stdout.read().decode("utf-8", "strict")[:-1]
+    def _get_current_resource(self):
+        if not self._player or not self._player.get_media():
+            return
+        return self._player.get_media().get_mrl()
 
 
 # vim:sw=4:ts=4:et:
-
```

### Comparing `platypush-0.9.5/platypush/plugins/video/torrentcast.py` & `platypush-0.9.6/platypush/plugins/video/torrentcast.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/weather/forecast.py` & `platypush-0.9.6/platypush/plugins/weather/forecast.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/websocket.py` & `platypush-0.9.6/platypush/plugins/websocket.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/plugins/wiimote.py` & `platypush-0.9.6/platypush/plugins/wiimote.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush/procedure/__init__.py` & `platypush-0.9.6/platypush/procedure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,19 +117,20 @@
     def execute(self, n_tries=1, **context):
         """
         Execute the requests in the procedure
         Params:
             n_tries -- Number of tries in case of failure before raising a RuntimeError
         """
         if self.args:
-            for (k,v) in self.args.items():
+            args = self.args.copy()
+            for (k,v) in args.items():
                 v = Request.expand_value_from_context(v, **context)
-                self.args[k] = v
+                args[k] = v
                 context[k] = v
-            logger.info('Executing procedure {} with arguments {}'.format(self.name, self.args))
+            logger.info('Executing procedure {} with arguments {}'.format(self.name, args))
         else:
             logger.info('Executing procedure {}'.format(self.name))
 
         response = Response()
         token = Config.get('token')
 
         for request in self.requests:
```

### Comparing `platypush-0.9.5/platypush/pusher/__init__.py` & `platypush-0.9.6/platypush/pusher/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/platypush.egg-info/PKG-INFO` & `platypush-0.9.6/platypush.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platypush
-Version: 0.9.5
+Version: 0.9.6
 Summary: Platypush service
 Home-page: https://github.com/BlackLight/platypush
 Author: Fabio Manganiello
 Author-email: info@fabiomanganiello.com
 License: MIT
 Description: Platypush
         =========
@@ -73,36 +73,41 @@
         
 Keywords: pushbullet notifications automation
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >= 3
-Provides-Extra: Support for sound devices
-Provides-Extra: Support for Kodi plugin
-Provides-Extra: Support for MPD/Mopidy music server plugin
-Provides-Extra: Support for torrents download
-Provides-Extra: Support for PDF generation
-Provides-Extra: Support for Pushbullet backend
-Provides-Extra: Support for Apache Kafka backend
-Provides-Extra: Support for Plex plugin
-Provides-Extra: Support for OMXPlayer plugin
-Provides-Extra: Support for smart cards detection
-Provides-Extra: Support for YouTube in the OMXPlayer plugin
+Provides-Extra: Support for RSS feeds
 Provides-Extra: Support for database plugin
-Provides-Extra: Support for Google Assistant
+Provides-Extra: Support for custom hotword detection
+Provides-Extra: Support for torrents download
+Provides-Extra: Support for custom thread and process names
+Provides-Extra: Support for web media subtitles
+Provides-Extra: Support for text2speech plugin
 Provides-Extra: Support for MCP3008 analog-to-digital converter plugin
+Provides-Extra: Support for mopidy backend
+Provides-Extra: Support for Plex plugin
+Provides-Extra: Support for sound devices
 Provides-Extra: Support for GPIO pins access
-Provides-Extra: Support for RSS feeds
-Provides-Extra: Support for Belkin WeMo Switch plugin
-Provides-Extra: Support for Philips Hue plugin
 Provides-Extra: Support for joystick backend
-Provides-Extra: Support for Last.FM scrobbler plugin
-Provides-Extra: Support for custom hotword detection
+Provides-Extra: Support for Philips Hue plugin
+Provides-Extra: Support for external web server
+Provides-Extra: Support for Kodi plugin
 Provides-Extra: Support for HTTP backend
-Provides-Extra: Support for real-time MIDI events
+Provides-Extra: Support for OMXPlayer plugin
+Provides-Extra: Support for PDF generation
+Provides-Extra: Support for MPD/Mopidy music server plugin
+Provides-Extra: Support for most of the HTTP poll backends
+Provides-Extra: Support for mpv player plugin
 Provides-Extra: Support for the Google APIs
+Provides-Extra: Support for Apache Kafka backend
+Provides-Extra: Support for Google Assistant
 Provides-Extra: Support for ICal calendars
-Provides-Extra: Support for HTTP poll backend
+Provides-Extra: Support for smart cards detection
+Provides-Extra: Support for Last.FM scrobbler plugin
+Provides-Extra: Support for Belkin WeMo Switch plugin
+Provides-Extra: Support for Pushbullet backend
 Provides-Extra: Support for Chromecast plugin
-Provides-Extra: Support for most of the HTTP poll backends
-Provides-Extra: Support for text2speech plugin
+Provides-Extra: Support for YouTube in the OMXPlayer plugin
+Provides-Extra: Support for real-time MIDI events
+Provides-Extra: Support for HTTP poll backend
```

### Comparing `platypush-0.9.5/platypush.egg-info/requires.txt` & `platypush-0.9.6/platypush.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 pyyaml
 redis
 requests
-python-prctl
 
 [Support for Apache Kafka backend]
 kafka-python
 
 [Support for Belkin WeMo Switch plugin]
 ouimeaux
 
@@ -63,23 +62,35 @@
 
 [Support for YouTube in the OMXPlayer plugin]
 youtube-dl
 
 [Support for custom hotword detection]
 snowboy
 
+[Support for custom thread and process names]
+python-prctl
+
 [Support for database plugin]
 sqlalchemy
 
+[Support for external web server]
+uwsgi
+
 [Support for joystick backend]
 inputs
 
+[Support for mopidy backend]
+websocket-client
+
 [Support for most of the HTTP poll backends]
 python-dateutil
 
+[Support for mpv player plugin]
+python-mpv
+
 [Support for real-time MIDI events]
 rtmidi
 
 [Support for smart cards detection]
 pyscard
 
 [Support for sound devices]
@@ -91,7 +102,10 @@
 mplayer
 
 [Support for the Google APIs]
 google-api-python-client
 
 [Support for torrents download]
 python-libtorrent
+
+[Support for web media subtitles]
+webvtt-py
```

### Comparing `platypush-0.9.5/setup.py` & `platypush-0.9.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 plugins = pkg_files('platypush/plugins')
 backend = pkg_files('platypush/backend')
 # create_etc_dir()
 
 setup(
     name = "platypush",
-    version = "0.9.5",
+    version = "0.9.6",
     author = "Fabio Manganiello",
     author_email = "info@fabiomanganiello.com",
     description = ("Platypush service"),
     license = "MIT",
     python_requires = '>= 3',
     keywords = "pushbullet notifications automation",
     url = "https://github.com/BlackLight/platypush",
@@ -59,21 +59,22 @@
         "License :: OSI Approved :: MIT License",
         "Development Status :: 3 - Alpha",
     ],
     install_requires = [
         'pyyaml',
         'redis',
         'requests',
-        'python-prctl',
     ],
     extras_require = {
+        'Support for custom thread and process names': ['python-prctl'],
         'Support for Apache Kafka backend': ['kafka-python'],
         'Support for Pushbullet backend': ['requests', 'pushbullet.py'],
         'Support for HTTP backend': ['flask','websockets', 'python-dateutil'],
         'Support for HTTP poll backend': ['frozendict'],
+        'Support for external web server': ['uwsgi'],
         'Support for database plugin': ['sqlalchemy'],
         'Support for RSS feeds': ['feedparser'],
         'Support for PDF generation': ['weasyprint'],
         'Support for Philips Hue plugin': ['phue'],
         'Support for MPD/Mopidy music server plugin': ['python-mpd2'],
         'Support for Belkin WeMo Switch plugin': ['ouimeaux'],
         'Support for text2speech plugin': ['mplayer'],
@@ -91,12 +92,16 @@
         'Support for smart cards detection': ['pyscard'],
         'Support for ICal calendars': ['icalendar', 'python-dateutil'],
         'Support for joystick backend': ['inputs'],
         'Support for Kodi plugin': ['kodi-json'],
         'Support for Plex plugin': ['plexapi'],
         'Support for Chromecast plugin': ['pychromecast'],
         'Support for sound devices': ['sounddevice', 'soundfile', 'numpy'],
+        'Support for web media subtitles': ['webvtt-py'],
+        'Support for mopidy backend': ['websocket-client'],
+        'Support for mpv player plugin': ['python-mpv'],
         # 'Support for Leap Motion backend': ['git+ssh://git@github.com:BlackLight/leap-sdk-python3.git'],
         # 'Support for Flic buttons': ['git+https://@github.com/50ButtonsEach/fliclib-linux-hci.git']
+        # 'Support for media subtitles': ['git+https://github.com/agonzalezro/python-opensubtitles#egg=python-opensubtitles']
     },
 )
```

### Comparing `platypush-0.9.5/tests/test_event_parse.py` & `platypush-0.9.6/tests/test_event_parse.py`

 * *Files identical despite different names*

### Comparing `platypush-0.9.5/tests/test_http.py` & `platypush-0.9.6/tests/test_http.py`

 * *Files identical despite different names*

