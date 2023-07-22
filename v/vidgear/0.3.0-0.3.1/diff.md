# Comparing `tmp/vidgear-0.3.0.tar.gz` & `tmp/vidgear-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidgear-0.3.0.tar", last modified: Thu Jan 26 04:22:00 2023, max compression
+gzip compressed data, was "vidgear-0.3.1.tar", last modified: Sat Jul 22 18:30:49 2023, max compression
```

## Comparing `vidgear-0.3.0.tar` & `vidgear-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 04:22:00.037013 vidgear-0.3.0/
--rw-rw-rw-   0        0        0    11586 2022-07-15 03:00:40.000000 vidgear-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    48605 2023-01-26 04:22:00.037013 vidgear-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    44666 2023-01-26 04:04:38.000000 vidgear-0.3.0/README.md
--rw-rw-rw-   0        0        0      143 2023-01-26 04:22:00.043008 vidgear-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     6581 2023-01-26 04:04:38.000000 vidgear-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-26 04:21:59.944593 vidgear-0.3.0/vidgear/
--rw-rw-rw-   0        0        0      105 2022-07-15 03:00:42.000000 vidgear-0.3.0/vidgear/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-26 04:22:00.000920 vidgear-0.3.0/vidgear/gears/
--rw-rw-rw-   0        0        0     5780 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-26 04:22:00.032128 vidgear-0.3.0/vidgear/gears/asyncio/
--rw-rw-rw-   0        0        0      257 2022-07-15 03:00:42.000000 vidgear-0.3.0/vidgear/gears/asyncio/__init__.py
--rw-rw-rw-   0        0        0     6131 2022-07-15 03:00:42.000000 vidgear-0.3.0/vidgear/gears/asyncio/__main__.py
--rw-rw-rw-   0        0        0    11557 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/asyncio/helper.py
--rw-rw-rw-   0        0        0    33642 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/asyncio/netgear_async.py
--rw-rw-rw-   0        0        0    22197 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/asyncio/webgear.py
--rw-rw-rw-   0        0        0    26887 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/asyncio/webgear_rtc.py
--rw-rw-rw-   0        0        0    22566 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/camgear.py
--rw-rw-rw-   0        0        0    45279 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/helper.py
--rw-rw-rw-   0        0        0    71953 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/netgear.py
--rw-rw-rw-   0        0        0    13892 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/pigear.py
--rw-rw-rw-   0        0        0    13325 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/screengear.py
--rw-rw-rw-   0        0        0    17380 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/stabilizer.py
--rw-rw-rw-   0        0        0    46187 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/streamgear.py
--rw-rw-rw-   0        0        0     7078 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/videogear.py
--rw-rw-rw-   0        0        0    32841 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/gears/writegear.py
--rw-rw-rw-   0        0        0       21 2023-01-26 04:04:38.000000 vidgear-0.3.0/vidgear/version.py
-drwxrwxrwx   0        0        0        0 2023-01-26 04:21:59.959636 vidgear-0.3.0/vidgear.egg-info/
--rw-rw-rw-   0        0        0    48605 2023-01-26 04:21:59.000000 vidgear-0.3.0/vidgear.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      700 2023-01-26 04:21:59.000000 vidgear-0.3.0/vidgear.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 04:21:59.000000 vidgear-0.3.0/vidgear.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      319 2023-01-26 04:21:59.000000 vidgear-0.3.0/vidgear.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-26 04:21:59.000000 vidgear-0.3.0/vidgear.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 18:30:49.658758 vidgear-0.3.1/
+-rw-rw-rw-   0        0        0    11586 2023-07-22 16:10:07.000000 vidgear-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0    48720 2023-07-22 18:30:49.658758 vidgear-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    44774 2023-07-22 16:10:07.000000 vidgear-0.3.1/README.md
+-rw-rw-rw-   0        0        0      143 2023-07-22 18:30:49.661783 vidgear-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     6575 2023-07-22 18:10:40.000000 vidgear-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:30:49.543555 vidgear-0.3.1/vidgear/
+-rw-rw-rw-   0        0        0      105 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:30:49.619367 vidgear-0.3.1/vidgear/gears/
+-rw-rw-rw-   0        0        0     5780 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:30:49.653980 vidgear-0.3.1/vidgear/gears/asyncio/
+-rw-rw-rw-   0        0        0      257 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     6131 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/asyncio/__main__.py
+-rw-rw-rw-   0        0        0    12919 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/asyncio/helper.py
+-rw-rw-rw-   0        0        0    33642 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/asyncio/netgear_async.py
+-rw-rw-rw-   0        0        0    23272 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/asyncio/webgear.py
+-rw-rw-rw-   0        0        0    27459 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/asyncio/webgear_rtc.py
+-rw-rw-rw-   0        0        0    22566 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/camgear.py
+-rw-rw-rw-   0        0        0    45279 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/helper.py
+-rw-rw-rw-   0        0        0    71953 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/netgear.py
+-rw-rw-rw-   0        0        0    13892 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/pigear.py
+-rw-rw-rw-   0        0        0    16591 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/screengear.py
+-rw-rw-rw-   0        0        0    17380 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/stabilizer.py
+-rw-rw-rw-   0        0        0    46187 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/streamgear.py
+-rw-rw-rw-   0        0        0     7078 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/videogear.py
+-rw-rw-rw-   0        0        0    32841 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/gears/writegear.py
+-rw-rw-rw-   0        0        0       23 2023-07-22 16:10:08.000000 vidgear-0.3.1/vidgear/version.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:30:49.560890 vidgear-0.3.1/vidgear.egg-info/
+-rw-rw-rw-   0        0        0    48720 2023-07-22 18:30:49.000000 vidgear-0.3.1/vidgear.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      700 2023-07-22 18:30:49.000000 vidgear-0.3.1/vidgear.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 18:30:49.000000 vidgear-0.3.1/vidgear.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      306 2023-07-22 18:30:49.000000 vidgear-0.3.1/vidgear.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 18:30:49.000000 vidgear-0.3.1/vidgear.egg-info/top_level.txt
```

### Comparing `vidgear-0.3.0/LICENSE` & `vidgear-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/PKG-INFO` & `vidgear-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: vidgear
-Version: 0.3.0
+Version: 0.3.1
 Summary: High-performance cross-platform Video Processing Python framework powerpacked with unique trailblazing features.
 Home-page: https://abhitronix.github.io/vidgear
 Author: Abhishek Thakur
 Author-email: abhi.una12@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/abhiTronix/vidgear/issues
 Project-URL: Funding, https://ko-fi.com/W7W8WTYO
 Project-URL: Source, https://github.com/abhiTronix/vidgear
 Project-URL: Documentation, https://abhitronix.github.io/vidgear
 Project-URL: Changelog, https://abhitronix.github.io/vidgear/latest/changelog/
-Keywords: OpenCV,multithreading,FFmpeg,picamera,starlette,mss,pyzmq,aiortc,uvicorn,uvloop,yt-dlp,asyncio,dash,hls,Video Processing,Video Stablization,Computer Vision,Video Streaming,raspberrypi,YouTube,Twitch,WebRTC
+Keywords: OpenCV,multithreading,FFmpeg,picamera,starlette,mss,pyzmq,dxcam,aiortc,uvicorn,uvloop,yt-dlp,asyncio,dash,hls,Video Processing,Video Stablization,Computer Vision,Video Streaming,raspberrypi,YouTube,Twitch,WebRTC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
@@ -69,15 +69,15 @@
 
 [![Code Style][black-badge]][black]
 
 </div>
 
 &nbsp;
 
-VidGear is a **High-Performance Video Processing Python Library** that provides an easy-to-use, highly extensible, thoroughly optimised **Multi-Threaded + Asyncio API Framework** on top of many state-of-the-art specialized libraries like _[OpenCV][opencv], [FFmpeg][ffmpeg], [ZeroMQ][zmq], [picamera][picamera], [starlette][starlette], [yt_dlp][yt_dlp], [pyscreenshot][pyscreenshot], [aiortc][aiortc] and [python-mss][mss]_ serving at its backend, and enable us to flexibly exploit their internal parameters and methods, while silently delivering **robust error-handling and real-time performance 🔥**
+VidGear is a **High-Performance Video Processing Python Library** that provides an easy-to-use, highly extensible, thoroughly optimised **Multi-Threaded + Asyncio API Framework** on top of many state-of-the-art specialized libraries like _[OpenCV][opencv], [FFmpeg][ffmpeg], [ZeroMQ][zmq], [picamera][picamera], [starlette][starlette], [yt_dlp][yt_dlp], [pyscreenshot][pyscreenshot], [dxcam][dxcam], [aiortc][aiortc] and [python-mss][mss]_ serving at its backend, and enable us to flexibly exploit their internal parameters and methods, while silently delivering **robust error-handling and real-time performance 🔥**
 
 VidGear primarily focuses on simplicity, and thereby lets programmers and software developers to easily integrate and perform Complex Video Processing Tasks, in just a few lines of code.
 
 &nbsp;
 
 The following **functional block diagram** clearly depicts the generalized functioning of VidGear APIs:
 
@@ -153,15 +153,15 @@
 
 **These Gears can be classified as follows:**
 
 **A. Video-Capture Gears:**
 
 - [**CamGear:**](https://github.com/abhiTronix/vidgear#camgear) Multi-Threaded API targeting various IP-USB-Cameras/Network-Streams/Streaming-Sites-URLs.
 - [**PiGear:**](https://github.com/abhiTronix/vidgear#pigear) Multi-Threaded API targeting various Raspberry-Pi Camera Modules.
-- [**ScreenGear:**](https://github.com/abhiTronix/vidgear#screengear) Multi-Threaded API targeting ultra-fast Screencasting.
+- [**ScreenGear:**](https://github.com/abhiTronix/vidgear#screengear) High-performance API targeting rapid Screencasting Capabilities.
 - [**VideoGear:**](https://github.com/abhiTronix/vidgear#videogear) Common Video-Capture API with internal [Video Stabilizer](https://abhitronix.github.io/vidgear/latest/gears/stabilizer/overview/) wrapper.
 
 **B. Video-Writer Gears:**
 
 - [**WriteGear:**](https://github.com/abhiTronix/vidgear#writegear) Handles Lossless Video-Writer for file/stream/frames Encoding and Compression.
 
 **C. Streaming Gears:**
@@ -359,17 +359,17 @@
 
 &nbsp;
 
 &nbsp;
 
 ## ScreenGear
 
-> _ScreenGear is designed exclusively for ultra-fast Screencasting, which means it can grab frames from your monitor in real-time, either by defining an area on the computer screen or full-screen, at the expense of inconsiderable latency. ScreenGear also seamlessly support frame capturing from multiple monitors as well as supports multiple backends._
+> _ScreenGear is designed exclusively for targeting rapid Screencasting Capabilities, which means it can grab frames from your monitor in real-time, either by defining an area on the computer screen or full-screen, at the expense of inconsiderable latency. ScreenGear also seamlessly support frame capturing from multiple monitors as well as supports multiple backends._
 
-ScreenGear implements a multi-threaded wrapper around [**pyscreenshot**][pyscreenshot] & [**python-mss**][mss] python library API and also supports an easy and flexible direct internal parameter manipulation.
+ScreenGear implements a Lightning-Fast API wrapper around [**dxcam**][dxcam], [**pyscreenshot**][pyscreenshot] & [**python-mss**][mss] python libraries and also supports an easy and flexible direct internal parameters manipulation.
 
 **Below is a snapshot of a ScreenGear API in action:**
 
 <p align="center">
   <img src="https://abhitronix.github.io/vidgear/latest/assets/gifs/screengear.gif" alt="ScreenGear in action!"/>
 </p>
 
@@ -680,36 +680,36 @@
 
 &nbsp;
 
 # Citation
 
 Here is a Bibtex entry you can use to cite this project in a publication:
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6926196.svg)](https://doi.org/10.5281/zenodo.6926196)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7571405.svg)](https://doi.org/10.5281/zenodo.7571405)
 
 ```BibTeX
 @software{vidgear,
   author       = {Abhishek Thakur and
                   Zoe Papakipos and
                   Christian Clauss and
                   Christian Hollinger and
                   Ian Max Andolina and
                   Vincent Boivin and
                   enarche-ahn and
                   freol35241 and
                   Benjamin Lowe and
                   Mickaël Schoentgen and
                   Renaud Bouckenooghe},
-  title        = {abhiTronix/vidgear: VidGear v0.2.6},
-  month        = jul,
-  year         = 2022,
+  title        = {abhiTronix/vidgear: VidGear v0.3.0},
+  month        = jan,
+  year         = 2023,
   publisher    = {Zenodo},
-  version      = {vidgear-0.2.6},
-  doi          = {10.5281/zenodo.6926196},
-  url          = {https://doi.org/10.5281/zenodo.6926196}
+  version      = {vidgear-0.3.0},
+  doi          = {10.5281/zenodo.7571405},
+  url          = {https://doi.org/10.5281/zenodo.7571405}
 }
 ```
 
 &nbsp;
 
 &nbsp;
 
@@ -808,14 +808,15 @@
 [uvloop]: https://github.com/MagicStack/uvloop
 [streamlink]: https://streamlink.github.io/
 [aiortc]: https://aiortc.readthedocs.io/en/latest/
 [pyscreenshot]: https://github.com/ponty/pyscreenshot
 [uvloop-ns]: https://github.com/MagicStack/uvloop/issues/14
 [ffmpeg]: https://www.ffmpeg.org/
 [flake8]: https://flake8.pycqa.org/en/latest/
+[dxcam]: https://github.com/ra1nty/DXcam
 [black]: https://github.com/psf/black
 [pytest]: https://docs.pytest.org/en/latest/
 [opencv-writer]: https://docs.opencv.org/master/dd/d9e/classcv_1_1VideoWriter.html#ad59c61d8881ba2b2da22cff5487465b5
 [opencv-windows]: https://www.learnopencv.com/install-opencv3-on-windows/
 [opencv-linux]: https://www.pyimagesearch.com/2018/05/28/ubuntu-18-04-how-to-install-opencv/
 [opencv-pi]: https://www.pyimagesearch.com/2018/09/26/install-opencv-4-on-your-raspberry-pi/
 [starlette]: https://www.starlette.io/
```

### Comparing `vidgear-0.3.0/README.md` & `vidgear-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 [![Code Style][black-badge]][black]
 
 </div>
 
 &nbsp;
 
-VidGear is a **High-Performance Video Processing Python Library** that provides an easy-to-use, highly extensible, thoroughly optimised **Multi-Threaded + Asyncio API Framework** on top of many state-of-the-art specialized libraries like _[OpenCV][opencv], [FFmpeg][ffmpeg], [ZeroMQ][zmq], [picamera][picamera], [starlette][starlette], [yt_dlp][yt_dlp], [pyscreenshot][pyscreenshot], [aiortc][aiortc] and [python-mss][mss]_ serving at its backend, and enable us to flexibly exploit their internal parameters and methods, while silently delivering **robust error-handling and real-time performance 🔥**
+VidGear is a **High-Performance Video Processing Python Library** that provides an easy-to-use, highly extensible, thoroughly optimised **Multi-Threaded + Asyncio API Framework** on top of many state-of-the-art specialized libraries like _[OpenCV][opencv], [FFmpeg][ffmpeg], [ZeroMQ][zmq], [picamera][picamera], [starlette][starlette], [yt_dlp][yt_dlp], [pyscreenshot][pyscreenshot], [dxcam][dxcam], [aiortc][aiortc] and [python-mss][mss]_ serving at its backend, and enable us to flexibly exploit their internal parameters and methods, while silently delivering **robust error-handling and real-time performance 🔥**
 
 VidGear primarily focuses on simplicity, and thereby lets programmers and software developers to easily integrate and perform Complex Video Processing Tasks, in just a few lines of code.
 
 &nbsp;
 
 The following **functional block diagram** clearly depicts the generalized functioning of VidGear APIs:
 
@@ -119,15 +119,15 @@
 
 **These Gears can be classified as follows:**
 
 **A. Video-Capture Gears:**
 
 - [**CamGear:**](#camgear) Multi-Threaded API targeting various IP-USB-Cameras/Network-Streams/Streaming-Sites-URLs.
 - [**PiGear:**](#pigear) Multi-Threaded API targeting various Raspberry-Pi Camera Modules.
-- [**ScreenGear:**](#screengear) Multi-Threaded API targeting ultra-fast Screencasting.
+- [**ScreenGear:**](#screengear) High-performance API targeting rapid Screencasting Capabilities.
 - [**VideoGear:**](#videogear) Common Video-Capture API with internal [Video Stabilizer](https://abhitronix.github.io/vidgear/latest/gears/stabilizer/overview/) wrapper.
 
 **B. Video-Writer Gears:**
 
 - [**WriteGear:**](#writegear) Handles Lossless Video-Writer for file/stream/frames Encoding and Compression.
 
 **C. Streaming Gears:**
@@ -325,17 +325,17 @@
 
 &nbsp;
 
 &nbsp;
 
 ## ScreenGear
 
-> _ScreenGear is designed exclusively for ultra-fast Screencasting, which means it can grab frames from your monitor in real-time, either by defining an area on the computer screen or full-screen, at the expense of inconsiderable latency. ScreenGear also seamlessly support frame capturing from multiple monitors as well as supports multiple backends._
+> _ScreenGear is designed exclusively for targeting rapid Screencasting Capabilities, which means it can grab frames from your monitor in real-time, either by defining an area on the computer screen or full-screen, at the expense of inconsiderable latency. ScreenGear also seamlessly support frame capturing from multiple monitors as well as supports multiple backends._
 
-ScreenGear implements a multi-threaded wrapper around [**pyscreenshot**][pyscreenshot] & [**python-mss**][mss] python library API and also supports an easy and flexible direct internal parameter manipulation.
+ScreenGear implements a Lightning-Fast API wrapper around [**dxcam**][dxcam], [**pyscreenshot**][pyscreenshot] & [**python-mss**][mss] python libraries and also supports an easy and flexible direct internal parameters manipulation.
 
 **Below is a snapshot of a ScreenGear API in action:**
 
 <p align="center">
   <img src="https://abhitronix.github.io/vidgear/latest/assets/gifs/screengear.gif" alt="ScreenGear in action!"/>
 </p>
 
@@ -646,36 +646,36 @@
 
 &nbsp;
 
 # Citation
 
 Here is a Bibtex entry you can use to cite this project in a publication:
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6926196.svg)](https://doi.org/10.5281/zenodo.6926196)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7571405.svg)](https://doi.org/10.5281/zenodo.7571405)
 
 ```BibTeX
 @software{vidgear,
   author       = {Abhishek Thakur and
                   Zoe Papakipos and
                   Christian Clauss and
                   Christian Hollinger and
                   Ian Max Andolina and
                   Vincent Boivin and
                   enarche-ahn and
                   freol35241 and
                   Benjamin Lowe and
                   Mickaël Schoentgen and
                   Renaud Bouckenooghe},
-  title        = {abhiTronix/vidgear: VidGear v0.2.6},
-  month        = jul,
-  year         = 2022,
+  title        = {abhiTronix/vidgear: VidGear v0.3.0},
+  month        = jan,
+  year         = 2023,
   publisher    = {Zenodo},
-  version      = {vidgear-0.2.6},
-  doi          = {10.5281/zenodo.6926196},
-  url          = {https://doi.org/10.5281/zenodo.6926196}
+  version      = {vidgear-0.3.0},
+  doi          = {10.5281/zenodo.7571405},
+  url          = {https://doi.org/10.5281/zenodo.7571405}
 }
 ```
 
 &nbsp;
 
 &nbsp;
 
@@ -774,14 +774,15 @@
 [uvloop]: https://github.com/MagicStack/uvloop
 [streamlink]: https://streamlink.github.io/
 [aiortc]: https://aiortc.readthedocs.io/en/latest/
 [pyscreenshot]: https://github.com/ponty/pyscreenshot
 [uvloop-ns]: https://github.com/MagicStack/uvloop/issues/14
 [ffmpeg]: https://www.ffmpeg.org/
 [flake8]: https://flake8.pycqa.org/en/latest/
+[dxcam]: https://github.com/ra1nty/DXcam
 [black]: https://github.com/psf/black
 [pytest]: https://docs.pytest.org/en/latest/
 [opencv-writer]: https://docs.opencv.org/master/dd/d9e/classcv_1_1VideoWriter.html#ad59c61d8881ba2b2da22cff5487465b5
 [opencv-windows]: https://www.learnopencv.com/install-opencv3-on-windows/
 [opencv-linux]: https://www.pyimagesearch.com/2018/05/28/ubuntu-18-04-how-to-install-opencv/
 [opencv-pi]: https://www.pyimagesearch.com/2018/09/26/install-opencv-4-on-your-raspberry-pi/
 [starlette]: https://www.starlette.io/
```

### Comparing `vidgear-0.3.0/setup.py` & `vidgear-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,32 +108,32 @@
     extras_require={
         # API specific deps
         "core": [
             "yt_dlp{}".format(latest_version("yt_dlp")),
             "pyzmq==24.0.1",
             "Pillow",
             "simplejpeg{}".format(latest_version("simplejpeg")),
-            "mss{}".format(latest_version("mss")),
+            "mss==7.0.1",  # TODO temporary solution, needs to be addressed
             "pyscreenshot{}".format(latest_version("pyscreenshot")),
         ]
         + (["picamera"] if ("arm" in platform.uname()[4][:3]) else []),
         # API specific + Asyncio deps
         "asyncio": [
             "yt_dlp{}".format(latest_version("yt_dlp")),
             "pyzmq==24.0.1",
             "simplejpeg{}".format(latest_version("simplejpeg")),
-            "mss{}".format(latest_version("mss")),
+            "mss==7.0.1",  # TODO temporary solution, needs to be addressed
             "Pillow",
             "pyscreenshot{}".format(latest_version("pyscreenshot")),
-            "starlette{}".format(latest_version("starlette")),
+            "starlette",
             "jinja2",
             "msgpack{}".format(latest_version("msgpack")),
             "msgpack_numpy{}".format(latest_version("msgpack_numpy")),
             "aiortc{}".format(latest_version("aiortc")),
-            "uvicorn{}".format(latest_version("uvicorn")),
+            "uvicorn",
         ]
         + (["picamera"] if ("arm" in platform.uname()[4][:3]) else [])
         + (
             ["uvloop{}".format(latest_version("uvloop"))]
             if (platform.system() != "Windows")  # windows not supported
             else []
         ),
@@ -142,14 +142,15 @@
         "OpenCV",
         "multithreading",
         "FFmpeg",
         "picamera",
         "starlette",
         "mss",
         "pyzmq",
+        "dxcam",
         "aiortc",
         "uvicorn",
         "uvloop",
         "yt-dlp",
         "asyncio",
         "dash",
         "hls",
```

### Comparing `vidgear-0.3.0/vidgear/gears/__init__.py` & `vidgear-0.3.1/vidgear/gears/__init__.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/asyncio/__main__.py` & `vidgear-0.3.1/vidgear/gears/asyncio/__main__.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/asyncio/helper.py` & `vidgear-0.3.1/vidgear/gears/asyncio/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     return cv2.resize(frame, dimensions, interpolation=interpolation)
 
 
 def generate_webdata(path, c_name="webgear", overwrite_default=False, logging=False):
     """
     ## generate_webdata
 
-    Auto-Generates, and Auto-validates default data for WebGear API.
+    Auto-Generates, and Auto-validates default data for WebGear and WebGear_RTC APIs.
 
     Parameters:
         path (string): path for generating data
         c_name (string): class name that is generating files
         overwrite_default (boolean): overwrite existing data or not?
         logging (bool): enables logging for its operations
 
@@ -181,21 +181,25 @@
     mkdir_safe(favicon_dir, logging=logging)
 
     # check if overwriting is enabled
     if overwrite_default or not validate_webdata(
         template_dir, ["index.html", "404.html", "500.html"]
     ):
         logger.critical(
-            "Overwriting existing WebGear data-files with default data-files from the server!"
+            "Overwriting existing {} data-files with default data-files from the server!".format(
+                c_name.capitalize()
+            )
             if overwrite_default
-            else "Failed to detect critical WebGear data-files: index.html, 404.html & 500.html!"
+            else "Failed to detect critical {} data-files: index.html, 404.html & 500.html!".format(
+                c_name.capitalize()
+            )
         )
         # download default files
         logging and logger.info(
-            "Downloading default data-files from the Gitlab Server: {}.".format(
+            "Downloading default data-files from the Gitlab Server: {}".format(
                 "https://gitlab.com/abhiTronix/vidgear-vitals"
             )
         )
         download_webdata(
             template_dir,
             c_name=c_name,
             files=["index.html", "404.html", "500.html", "base.html"],
@@ -221,69 +225,97 @@
     return path
 
 
 def download_webdata(path, c_name="webgear", files=[], logging=False):
     """
     ## download_webdata
 
-    Downloads given list of files for WebGear API(if not available) from GitHub Server,
+    Downloads given list of files for WebGear and WebGear_RTC APIs(if not available) from GitHub/Gitlab Servers,
     and also Validates them.
 
     Parameters:
         path (string): path for downloading data
         c_name (string): class name that is generating files
         files (list): list of files to be downloaded
         logging (bool): enables logging for its operations
 
     **Returns:** A valid path as string.
     """
     basename = os.path.basename(path)
     if logging:
         logger.debug("Downloading {} data-files at `{}`".format(basename, path))
 
+    # list all registered urls
+    reg_urls = [
+        "https://gitlab.com/abhiTronix/vidgear-vitals/-/raw/main",
+        "https://raw.githubusercontent.com/abhiTronix/vidgear-vitals/main",
+    ]
+
     # create session
     with requests.Session() as http:
-        for file in files:
-            # get filename
-            file_name = os.path.join(path, file)
-            # get URL
-            file_url = "https://gitlab.com/abhiTronix/vidgear-vitals/-/raw/main/{}{}/{}/{}".format(
-                c_name, "/static" if basename != "templates" else "", basename, file
-            )
-            # download and write file to the given path
-            logging and logger.debug(
-                "Downloading {} data-file: {}.".format(basename, file)
-            )
-
-            with open(file_name, "wb") as f:
-                # setup retry strategy
-                retries = Retry(
-                    total=3,
-                    backoff_factor=1,
-                    status_forcelist=[429, 500, 502, 503, 504],
+        for url in reg_urls:
+            try:
+                for file in files:
+                    # get filename
+                    file_name = os.path.join(path, file)
+                    # get URL
+                    file_url = "{}/{}{}/{}/{}".format(
+                        url,
+                        c_name,
+                        "/static" if basename != "templates" else "",
+                        basename,
+                        file,
+                    )
+                    # download and write file to the given path
+                    logging and logger.debug(
+                        "Downloading {} data-file: {}.".format(basename, file)
+                    )
+
+                    with open(file_name, "wb") as f:
+                        # setup retry strategy
+                        retries = Retry(
+                            total=3,
+                            backoff_factor=1,
+                            status_forcelist=[429, 500, 502, 503, 504],
+                        )
+                        # Mount it for https usage
+                        adapter = TimeoutHTTPAdapter(timeout=2.0, max_retries=retries)
+                        http.mount("https://", adapter)
+                        response = http.get(file_url, stream=True)
+                        response.raise_for_status()
+                        total_length = (
+                            response.headers.get("content-length")
+                            if "content-length" in response.headers
+                            else len(response.content)
+                        )
+                        assert not (
+                            total_length is None
+                        ), "[Helper:ERROR] :: Failed to retrieve files, check your Internet connectivity!"
+                        bar = tqdm(total=int(total_length), unit="B", unit_scale=True)
+                        for data in response.iter_content(chunk_size=256):
+                            f.write(data)
+                            if len(data) > 0:
+                                bar.update(len(data))
+                        bar.close()
+            except AssertionError as e:
+                # raise if connection error
+                raise e
+            except Exception as e:
+                # log error
+                logger.exception(str(e))
+                # log event if necessary
+                url != reg_urls[1] and logger.error(
+                    "Download failed for Gitlab Server! Retrying from GitHub Server: {}".format(
+                        url, "https://github.com/abhiTronix/vidgear-vitals"
+                    )
                 )
-                # Mount it for https usage
-                adapter = TimeoutHTTPAdapter(timeout=2.0, max_retries=retries)
-                http.mount("https://", adapter)
-                response = http.get(file_url, stream=True)
-                response.raise_for_status()
-                total_length = (
-                    response.headers.get("content-length")
-                    if "content-length" in response.headers
-                    else len(response.content)
-                )
-                assert not (
-                    total_length is None
-                ), "[Helper:ERROR] :: Failed to retrieve files, check your Internet connectivity!"
-                bar = tqdm(total=int(total_length), unit="B", unit_scale=True)
-                for data in response.iter_content(chunk_size=256):
-                    f.write(data)
-                    if len(data) > 0:
-                        bar.update(len(data))
-                bar.close()
+            else:
+                # break otherwise
+                break
+
     if logging:
         logger.debug("Verifying downloaded data:")
     if validate_webdata(path, files=files, logging=logging):
         if logging:
             logger.info("Successful!")
         return path
     else:
```

### Comparing `vidgear-0.3.0/vidgear/gears/asyncio/netgear_async.py` & `vidgear-0.3.1/vidgear/gears/asyncio/netgear_async.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/asyncio/webgear.py` & `vidgear-0.3.1/vidgear/gears/asyncio/webgear.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         colorspace=None,
         resolution=(640, 480),
         framerate=25,
         logging=False,
         time_delay=0,
         **options
     ):
-
         """
         This constructor method initializes the object state and attributes of the WebGear class.
 
         Parameters:
             enablePiCamera (bool): provide access to PiGear(if True) or CamGear(if False) APIs respectively.
             stabilize (bool): enable access to Stabilizer Class for stabilizing frames.
             camera_num (int): selects the camera module index which will be used as Rpi source.
@@ -127,14 +126,15 @@
         self.__logging = logging
         self.__frame_size_reduction = 25  # use 25% reduction
         # retrieve interpolation for reduction
         self.__interpolation = retrieve_best_interpolation(
             ["INTER_LINEAR_EXACT", "INTER_LINEAR", "INTER_AREA"]
         )
 
+        custom_video_endpoint = ""  # custom video endpoint path
         custom_data_location = ""  # path to save data-files to custom location
         data_path = ""  # path to WebGear data-files
         overwrite_default = False
         self.__enable_inf = False  # continue frames even when video ends.
 
         # reformat dictionary
         options = {str(k).strip(): v for k, v in options.items()}
@@ -208,17 +208,30 @@
                 value = options["frame_size_reduction"]
                 if isinstance(value, (int, float)) and value >= 0 and value <= 90:
                     self.__frame_size_reduction = value
                 else:
                     logger.warning("Skipped invalid `frame_size_reduction` value!")
                 del options["frame_size_reduction"]  # clean
 
+            if "custom_video_endpoint" in options:
+                value = options["custom_video_endpoint"]
+                if value and isinstance(value, str) and value.strip().isalnum():
+                    custom_video_endpoint = value.strip()
+                    logging and logger.critical(
+                        "Using custom video endpoint path: `/{}`".format(
+                            custom_video_endpoint
+                        )
+                    )
+                else:
+                    logger.warning("Skipped invalid `custom_video_endpoint` value!")
+                del options["custom_video_endpoint"]  # clean
+
             if "custom_data_location" in options:
                 value = options["custom_data_location"]
-                if isinstance(value, str):
+                if value and isinstance(value, str):
                     assert os.access(
                         value, os.W_OK
                     ), "[WebGear:ERROR] :: Permission Denied!, cannot write WebGear data-files to '{}' directory!".format(
                         value
                     )
                     assert os.path.isdir(
                         os.path.abspath(value)
@@ -272,29 +285,39 @@
             # define Jinja2 templates handler
             self.__templates = Jinja2Templates(
                 directory="{}/templates".format(data_path)
             )
             # define routing tables
             self.routes = [
                 Route("/", endpoint=self.__homepage),
-                Route("/video", endpoint=self.__video),
+                Route(
+                    "/{}".format(
+                        custom_video_endpoint if custom_video_endpoint else "video"
+                    ),
+                    endpoint=self.__video,
+                ),
                 Mount(
                     "/static",
                     app=StaticFiles(directory="{}/static".format(data_path)),
                     name="static",
                 ),
             ]
         else:
             # log it
             self.__logging and logger.critical(
                 "WebGear Data-Files Auto-Generation WorkFlow has been manually disabled."
             )
             # define routing tables
             self.routes = [
-                Route("/video", endpoint=self.__video),
+                Route(
+                    "/{}".format(
+                        custom_video_endpoint if custom_video_endpoint else "video"
+                    ),
+                    endpoint=self.__video,
+                ),
             ]
             # log exceptions
             self.__logging and logger.warning(
                 "Only `/video` route is available for this instance."
             )
 
         # define custom exception handlers
```

### Comparing `vidgear-0.3.0/vidgear/gears/asyncio/webgear_rtc.py` & `vidgear-0.3.1/vidgear/gears/asyncio/webgear_rtc.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,19 +268,32 @@
                     f_stream,
                     percentage=self.__frame_size_reduction,
                     interpolation=self.__interpolation,
                 )
 
             # construct `av.frame.Frame` from `numpy.nd.array`
             # based on available channels in frames
-            f_format = "bgr24"
             if f_stream.ndim == 3 and f_stream.shape[-1] == 4:
                 f_format = "bgra"
-            if f_stream.ndim == 2:
+            elif f_stream.ndim == 2 or (f_stream.ndim == 3 and f_stream.shape[-1] == 1):
+                # drop third dimension if defined, as only `ndim==2`
+                # grayscale is supported by PyAV
+                f_stream = (
+                    f_stream[:, :, 0]
+                    if f_stream.ndim == 3 and f_stream.shape[-1] == 1
+                    else f_stream
+                )
                 f_format = "gray"
+            elif f_stream.ndim == 3:
+                f_format = "bgr24"
+            else:
+                raise ValueError(
+                    "Input frame of shape: {}, Isn't supported!".format(f_stream.shape)
+                )
+
             frame = VideoFrame.from_ndarray(f_stream, format=f_format)
             frame.pts = pts
             frame.time_base = time_base
 
             # return `av.frame.Frame`
             return frame
 
@@ -337,15 +350,14 @@
         colorspace=None,
         resolution=(640, 480),
         framerate=25,
         logging=False,
         time_delay=0,
         **options
     ):
-
         """
         This constructor method initializes the object state and attributes of the WebGear_RTC class.
 
         Parameters:
             enablePiCamera (bool): provide access to PiGear(if True) or CamGear(if False) APIs respectively.
             stabilize (bool): enable access to Stabilizer Class for stabilizing frames.
             camera_num (int): selects the camera module index which will be used as Rpi source.
```

### Comparing `vidgear-0.3.0/vidgear/gears/camgear.py` & `vidgear-0.3.1/vidgear/gears/camgear.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/helper.py` & `vidgear-0.3.1/vidgear/gears/helper.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/netgear.py` & `vidgear-0.3.1/vidgear/gears/netgear.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/pigear.py` & `vidgear-0.3.1/vidgear/gears/pigear.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/screengear.py` & `vidgear-0.3.1/vidgear/gears/screengear.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ===============================================
 """
 # import the necessary packages
 import cv2
-import queue
+import json
+import platform
 import numpy as np
 import logging as log
 from threading import Thread, Event
 from collections import OrderedDict
 
 # import helper packages
 from .helper import (
@@ -34,219 +35,300 @@
 )
 
 # safe import critical Class modules
 mss = import_dependency_safe("from mss import mss", error="silent")
 if not (mss is None):
     from mss.exception import ScreenShotError
 pysct = import_dependency_safe("pyscreenshot", error="silent")
-if not (pysct is None):
-    from pyscreenshot.err import FailedBackendError
+dxcam = import_dependency_safe("dxcam", error="silent")
 
 # define logger
 logger = log.getLogger("ScreenGear")
 logger.propagate = False
 logger.addHandler(logger_handler())
 logger.setLevel(log.DEBUG)
 
 
 class ScreenGear:
     """
-    ScreenGear is designed exclusively for ultra-fast Screencasting, which means it can grab frames from your monitor in real-time, either by defining an area on the computer screen or full-screen,
-    at the expense of inconsiderable latency. ScreenGear also seamlessly support frame capturing from multiple monitors as well as supports multiple backends.
+    ScreenGear is designed exclusively for targeting rapid Screencasting Capabilities, which means it can
+    grab frames from your monitor in real-time, either by defining an area on the computer screen or full-screen,
+    at the expense of inconsiderable latency. ScreenGear also seamlessly support frame capturing from multiple
+    monitors as well as supports multiple backends.
 
-    ScreenGear API implements a multi-threaded wrapper around pyscreenshot & python-mss python library, and also flexibly supports its internal parameter.
+    ScreenGear API implements a multi-threaded wrapper around dxcam, pyscreenshot, python-mss python library,
+    and also flexibly supports its internal parameter.
     """
 
     def __init__(
-        self, monitor=None, backend="", colorspace=None, logging=False, **options
+        self, monitor=None, backend=None, colorspace=None, logging=False, **options
     ):
         """
         This constructor method initializes the object state and attributes of the ScreenGear class.
 
         Parameters:
             monitor (int): enables `mss` backend and sets the index of the monitor screen.
-            backend (str): enables `pyscreenshot` and select suitable backend for extracting frames.
+            backend (str): select suitable backend for extracting frames.
             colorspace (str): selects the colorspace of the input stream.
             logging (bool): enables/disables logging.
-            options (dict): provides the flexibility to manually set the dimensions of capture screen area.
+            options (dict): provides the flexibility to easily alter backend library parameters. Such as, manually set the dimensions of capture screen area etc.
         """
         # print current version
         logcurr_vidgear_ver(logging=logging)
 
-        # raise error(s) for critical Class imports
-        import_dependency_safe(
-            "from mss import mss" if mss is None else "", pkg_name="mss"
-        )
-        import_dependency_safe("pyscreenshot" if pysct is None else "")
-
         # enable logging if specified:
         self.__logging = logging if isinstance(logging, bool) else False
 
-        # create monitor instance for the user-defined monitor
+        # create instances for the user-defined monitor
         self.__monitor_instance = None
-        self.__backend = ""
-        if monitor is None:
-            self.__capture_object = pysct
-            self.__backend = backend.lower().strip()
-        else:
-            self.__capture_object = mss()
-            if backend.strip():
-                logger.warning(
-                    "Backends are disabled for Monitor Indexing(monitor>=0)!"
-                )
-            try:
-                self.__monitor_instance = self.__capture_object.monitors[monitor]
-            except Exception as e:
-                logger.exception(str(e))
-                self.__monitor_instance = None
+        self.__backend = None
 
-        # assigns special parameter to global variable and clear
-        # Thread Timeout
-        self.__thread_timeout = options.pop("THREAD_TIMEOUT", None)
-        if self.__thread_timeout and isinstance(self.__thread_timeout, (int, float)):
-            # set values
-            self.__thread_timeout = float(self.__thread_timeout)
-        else:
-            # defaults to 5mins timeout
-            self.__thread_timeout = None
+        # validate monitor instance
+        assert (
+            monitor is None or monitor and isinstance(monitor, (int, tuple))
+        ), "[ScreenGear:ERROR] :: Invalid `monitor` value detected!"
 
-        # define deque and assign it to global var
-        self.__queue = queue.Queue(maxsize=96)  # max bufferlen 96 to check overflow
-        # log it
-        if logging:
-            logger.debug("Enabling Threaded Queue Mode by default for ScreenGear!")
-            if self.__thread_timeout:
-                logger.debug(
-                    "Setting Video-Thread Timeout to {}s.".format(self.__thread_timeout)
-                )
+        # initialize backend
+        if backend and monitor is None:
+            self.__backend = backend.lower().strip()
+        else:
+            # enforce `dxcam` for Windows machines if undefined (or monitor is defined)
+            self.__backend = (
+                "dxcam" if platform.system() == "Windows" and dxcam else None
+            )
 
-        # intiate screen dimension handler
+        # initiate screen dimension handler
         screen_dims = {}
         # reformat proper mss dict and assign to screen dimension handler
         screen_dims = {
             k.strip(): v
             for k, v in options.items()
             if k.strip() in ["top", "left", "width", "height"]
         }
         # check whether user-defined dimensions are provided
         if screen_dims and len(screen_dims) == 4:
             key_order = ("top", "left", "width", "height")
             screen_dims = OrderedDict((k, screen_dims[k]) for k in key_order)
-            if logging:
-                logger.debug("Setting Capture-Area dimensions: {}!".format(screen_dims))
+            logging and logger.debug(
+                "Setting Capture-Area dimensions: {}".format(json.dumps(screen_dims))
+            )
         else:
             screen_dims.clear()
 
+        # handle backends
+        if self.__backend == "dxcam":
+            # get target fps in case of DXcam
+            self.__target_fps = options.pop("dxcam_target_fps", 0)
+            if self.__target_fps and isinstance(self.__target_fps, (int, float)):
+                # set values
+                self.__target_fps = int(self.__target_fps)
+                logging and logger.debug(
+                    "Setting Target FPS: {}".format(self.__target_fps)
+                )
+            else:
+                # defaults to 0fps
+                self.__target_fps = 0
+            # check if platform is windows
+            assert (
+                platform.system() == "Windows"
+            ), "`dxcam` backend is only available for Windows Machines."
+            # verify monitor values if tuple
+            assert (
+                monitor is None
+                or isinstance(monitor, int)
+                or (
+                    isinstance(monitor, tuple)
+                    and len(monitor) == 2
+                    and all(isinstance(x, int) for x in monitor)
+                )
+            ), "For dxcam` backend, monitor` tuple value must be format `int` or `(int, int)` only."
+            # raise error(s) for critical Class imports
+            import_dependency_safe("dxcam" if dxcam is None else "")
+            if monitor is None:
+                self.__capture_object = dxcam.create(
+                    region=tuple(screen_dims.values()) if screen_dims else None
+                )
+            else:
+                self.__capture_object = (
+                    dxcam.create(
+                        device_idx=monitor[0],
+                        output_idx=monitor[1],
+                        region=tuple(screen_dims.values()) if screen_dims else None,
+                    )
+                    if isinstance(monitor, tuple)
+                    else dxcam.create(
+                        device_idx=monitor,
+                        region=tuple(screen_dims.values()) if screen_dims else None,
+                    )
+                )
+        else:
+            if monitor is None:
+                # raise error(s) for critical Class imports
+                import_dependency_safe("pyscreenshot" if pysct is None else "")
+                # reset backend if not provided
+                self.__backend = (
+                    "pil"
+                    if self.__backend is None or self.__backend == "mss"
+                    else self.__backend
+                )
+                # check if valid backend
+                assert (
+                    self.__backend in pysct.backends()
+                ), "Unsupported backend {} provided!".format(backend)
+                # create capture object
+                self.__capture_object = pysct
+            else:
+                # monitor value must be integer
+                assert monitor and isinstance(
+                    monitor, int
+                ), "[ScreenGear:ERROR] :: Invalid `monitor` value must be integer with mss backend."
+                # raise error(s) for critical Class imports
+                import_dependency_safe(
+                    "from mss import mss" if mss is None else "", pkg_name="mss"
+                )
+                # create capture object
+                self.__capture_object = mss()
+                self.__backend and logger.warning(
+                    "Backends are disabled for Monitor Indexing(monitor>=0)!"
+                )
+                self.__monitor_instance = self.__capture_object.monitors[monitor]
+
+        # log backend
+        self.__backend and logging and logger.debug(
+            "Setting Backend: {}".format(self.__backend.upper())
+        )
+
+        # assigns special parameter to global variable and clear
         # separately handle colorspace value to int conversion
         if colorspace:
             self.color_space = capPropId(colorspace.strip())
-            if logging and not (self.color_space is None):
-                logger.debug(
-                    "Enabling `{}` colorspace for this video stream!".format(
-                        colorspace.strip()
-                    )
+            logging and not (self.color_space is None) and logger.debug(
+                "Enabling `{}` colorspace for this video stream!".format(
+                    colorspace.strip()
                 )
+            )
         else:
             self.color_space = None
 
-        # intialize mss capture instance
-        self.__mss_capture_instance = ""
+        # initialize mss capture instance
+        self.__mss_capture_instance = None
         try:
-            if self.__monitor_instance is None:
-                if screen_dims:
-                    self.__mss_capture_instance = tuple(screen_dims.values())
+            if self.__backend == "dxcam":
                 # extract global frame from instance
-                self.frame = np.asanyarray(
-                    self.__capture_object.grab(
-                        bbox=self.__mss_capture_instance,
-                        childprocess=False,
-                        backend=self.__backend,
-                    )
-                )
+                self.frame = self.__capture_object.grab()
             else:
-                if screen_dims:
-                    self.__mss_capture_instance = {
-                        "top": self.__monitor_instance["top"] + screen_dims["top"],
-                        "left": self.__monitor_instance["left"] + screen_dims["left"],
-                        "width": screen_dims["width"],
-                        "height": screen_dims["height"],
-                        "mon": monitor,
-                    }
+                if self.__monitor_instance is None:
+                    if screen_dims:
+                        self.__mss_capture_instance = tuple(screen_dims.values())
+                    # extract global frame from instance
+                    self.frame = np.asanyarray(
+                        self.__capture_object.grab(
+                            bbox=self.__mss_capture_instance,
+                            childprocess=False,
+                            backend=self.__backend,
+                        )
+                    )
                 else:
-                    self.__mss_capture_instance = (
-                        self.__monitor_instance  # otherwise create instance from monitor
+                    if screen_dims:
+                        self.__mss_capture_instance = {
+                            "top": self.__monitor_instance["top"] + screen_dims["top"],
+                            "left": self.__monitor_instance["left"]
+                            + screen_dims["left"],
+                            "width": screen_dims["width"],
+                            "height": screen_dims["height"],
+                            "mon": monitor,
+                        }
+                    else:
+                        self.__mss_capture_instance = (
+                            self.__monitor_instance  # otherwise create instance from monitor
+                        )
+                    # extract global frame from instance
+                    self.frame = np.asanyarray(
+                        self.__capture_object.grab(self.__mss_capture_instance)
                     )
-                # extract global frame from instance
-                self.frame = np.asanyarray(
-                    self.__capture_object.grab(self.__mss_capture_instance)
-                )
-            # initialize and append to queue
-            self.__queue.put(self.frame)
+            # convert to bgr frame if applicable
+            self.frame = (
+                self.frame[:, :, ::-1]
+                if self.__backend == "dxcam" or not (pysct is None)
+                else self.frame
+            )
+            # render colorspace if defined
+            if not (self.frame is None) and not (self.color_space is None):
+                self.frame = cv2.cvtColor(self.frame, self.color_space)
         except Exception as e:
             if isinstance(e, ScreenShotError):
                 # otherwise catch and log errors
-                if logging:
-                    logger.exception(self.__capture_object.get_error_details())
+                logging and logger.exception(self.__capture_object.get_error_details())
                 raise ValueError(
                     "[ScreenGear:ERROR] :: ScreenShotError caught, Wrong dimensions passed to python-mss, Kindly Refer Docs!"
                 )
-            elif isinstance(e, KeyError):
-                raise ValueError(
-                    "[ScreenGear:ERROR] :: ScreenShotError caught, Invalid backend: `{}`, Kindly Refer Docs!".format(
-                        backend
-                    )
-                )
             else:
                 raise SystemError(
                     "[ScreenGear:ERROR] :: Unable to grab any instance on this system, Are you running headless?"
                 )
-
         # thread initialization
         self.__thread = None
         # initialize termination flag
         self.__terminate = Event()
 
     def start(self):
         """
         Launches the internal *Threaded Frames Extractor* daemon
 
         **Returns:** A reference to the ScreenGear class object.
         """
         self.__thread = Thread(target=self.__update, name="ScreenGear", args=())
         self.__thread.daemon = True
         self.__thread.start()
+        if self.__backend == "dxcam":
+            self.__capture_object.start(
+                target_fps=self.__target_fps,
+                video_mode=True,
+            )
+            self.__logging and self.__target_fps and logger.debug(
+                "Targeting FPS: {}".format(self.__target_fps)
+            )
         return self
 
     def __update(self):
         """
         A **Threaded Frames Extractor**, that keep iterating frames from `mss` API to a internal monitored deque,
         until the thread is terminated, or frames runs out.
         """
         # initialize frame variable
         frame = None
         # keep looping infinitely until the thread is terminated
         while not self.__terminate.is_set():
             try:
-                if self.__monitor_instance:
-                    frame = np.asanyarray(
-                        self.__capture_object.grab(self.__mss_capture_instance)
-                    )
+                if self.__backend == "dxcam":
+                    # extract global frame from instance
+                    frame = self.__capture_object.get_latest_frame()
                 else:
-                    frame = np.asanyarray(
-                        self.__capture_object.grab(
-                            bbox=self.__mss_capture_instance,
-                            childprocess=False,
-                            backend=self.__backend,
+                    if self.__monitor_instance:
+                        frame = np.asanyarray(
+                            self.__capture_object.grab(self.__mss_capture_instance)
                         )
-                    )
-                    if not self.__backend or self.__backend == "pil":
-                        frame = frame[:, :, ::-1]
+                    else:
+                        frame = np.asanyarray(
+                            self.__capture_object.grab(
+                                bbox=self.__mss_capture_instance,
+                                childprocess=False,
+                                backend=self.__backend,
+                            )
+                        )
+                # check if valid frame
                 assert not (
                     frame is None or np.shape(frame) == ()
-                ), "[ScreenGear:ERROR] :: Failed to retreive any valid frames!"
+                ), "[ScreenGear:ERROR] :: Failed to retrieve valid frame!"
+                # convert to bgr frame if applicable
+                frame = (
+                    frame[:, :, ::-1]
+                    if self.__backend == "dxcam" or not (pysct is None)
+                    else frame
+                )
             except Exception as e:
                 if isinstance(e, ScreenShotError):
                     raise RuntimeError(self.__capture_object.get_error_details())
                 else:
                     logger.exception(str(e))
                 self.__terminate.set()
                 continue
@@ -272,54 +354,40 @@
                         logger.warning("Input colorspace is not a valid colorspace!")
                 if not (color_frame is None):
                     self.frame = color_frame
                 else:
                     self.frame = frame
             else:
                 self.frame = frame
-            # append to queue
-            self.__queue.put(self.frame)
-
-        # signal queue we're done
-        self.__queue.put(None)
 
         # indicate immediate termination
         self.__terminate.set()
 
         # finally release mss resources
         if self.__monitor_instance:
             self.__capture_object.close()
+        if self.__backend == "dxcam":
+            self.__capture_object.stop()
+            del self.__capture_object
 
     def read(self):
         """
         Extracts frames synchronously from monitored deque, while maintaining a fixed-length frame buffer in the memory,
         and blocks the thread if the deque is full.
 
         **Returns:** A n-dimensional numpy array.
         """
-        # check whether or not termination flag is enabled
-        while not self.__terminate.is_set():
-            if self.__queue.empty():
-                break
-            return self.__queue.get(timeout=self.__thread_timeout)
-        # otherwise return NoneType
-        return None
+        # return the frame
+        return self.frame
 
     def stop(self):
         """
         Safely terminates the thread, and release the resources.
         """
         self.__logging and logger.debug("Terminating ScreenGear Processes.")
 
         # indicate that the thread should be terminate
         self.__terminate.set()
 
         # wait until stream resources are released (producer thread might be still grabbing frame)
         if self.__thread is not None:
-            if not (self.__queue is None):
-                while not self.__queue.empty():
-                    try:
-                        self.__queue.get_nowait()
-                    except queue.Empty:
-                        continue
-                    self.__queue.task_done()
             self.__thread.join()
```

### Comparing `vidgear-0.3.0/vidgear/gears/stabilizer.py` & `vidgear-0.3.1/vidgear/gears/stabilizer.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/streamgear.py` & `vidgear-0.3.1/vidgear/gears/streamgear.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/videogear.py` & `vidgear-0.3.1/vidgear/gears/videogear.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear/gears/writegear.py` & `vidgear-0.3.1/vidgear/gears/writegear.py`

 * *Files identical despite different names*

### Comparing `vidgear-0.3.0/vidgear.egg-info/PKG-INFO` & `vidgear-0.3.1/vidgear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: vidgear
-Version: 0.3.0
+Version: 0.3.1
 Summary: High-performance cross-platform Video Processing Python framework powerpacked with unique trailblazing features.
 Home-page: https://abhitronix.github.io/vidgear
 Author: Abhishek Thakur
 Author-email: abhi.una12@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/abhiTronix/vidgear/issues
 Project-URL: Funding, https://ko-fi.com/W7W8WTYO
 Project-URL: Source, https://github.com/abhiTronix/vidgear
 Project-URL: Documentation, https://abhitronix.github.io/vidgear
 Project-URL: Changelog, https://abhitronix.github.io/vidgear/latest/changelog/
-Keywords: OpenCV,multithreading,FFmpeg,picamera,starlette,mss,pyzmq,aiortc,uvicorn,uvloop,yt-dlp,asyncio,dash,hls,Video Processing,Video Stablization,Computer Vision,Video Streaming,raspberrypi,YouTube,Twitch,WebRTC
+Keywords: OpenCV,multithreading,FFmpeg,picamera,starlette,mss,pyzmq,dxcam,aiortc,uvicorn,uvloop,yt-dlp,asyncio,dash,hls,Video Processing,Video Stablization,Computer Vision,Video Streaming,raspberrypi,YouTube,Twitch,WebRTC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
@@ -69,15 +69,15 @@
 
 [![Code Style][black-badge]][black]
 
 </div>
 
 &nbsp;
 
-VidGear is a **High-Performance Video Processing Python Library** that provides an easy-to-use, highly extensible, thoroughly optimised **Multi-Threaded + Asyncio API Framework** on top of many state-of-the-art specialized libraries like _[OpenCV][opencv], [FFmpeg][ffmpeg], [ZeroMQ][zmq], [picamera][picamera], [starlette][starlette], [yt_dlp][yt_dlp], [pyscreenshot][pyscreenshot], [aiortc][aiortc] and [python-mss][mss]_ serving at its backend, and enable us to flexibly exploit their internal parameters and methods, while silently delivering **robust error-handling and real-time performance 🔥**
+VidGear is a **High-Performance Video Processing Python Library** that provides an easy-to-use, highly extensible, thoroughly optimised **Multi-Threaded + Asyncio API Framework** on top of many state-of-the-art specialized libraries like _[OpenCV][opencv], [FFmpeg][ffmpeg], [ZeroMQ][zmq], [picamera][picamera], [starlette][starlette], [yt_dlp][yt_dlp], [pyscreenshot][pyscreenshot], [dxcam][dxcam], [aiortc][aiortc] and [python-mss][mss]_ serving at its backend, and enable us to flexibly exploit their internal parameters and methods, while silently delivering **robust error-handling and real-time performance 🔥**
 
 VidGear primarily focuses on simplicity, and thereby lets programmers and software developers to easily integrate and perform Complex Video Processing Tasks, in just a few lines of code.
 
 &nbsp;
 
 The following **functional block diagram** clearly depicts the generalized functioning of VidGear APIs:
 
@@ -153,15 +153,15 @@
 
 **These Gears can be classified as follows:**
 
 **A. Video-Capture Gears:**
 
 - [**CamGear:**](https://github.com/abhiTronix/vidgear#camgear) Multi-Threaded API targeting various IP-USB-Cameras/Network-Streams/Streaming-Sites-URLs.
 - [**PiGear:**](https://github.com/abhiTronix/vidgear#pigear) Multi-Threaded API targeting various Raspberry-Pi Camera Modules.
-- [**ScreenGear:**](https://github.com/abhiTronix/vidgear#screengear) Multi-Threaded API targeting ultra-fast Screencasting.
+- [**ScreenGear:**](https://github.com/abhiTronix/vidgear#screengear) High-performance API targeting rapid Screencasting Capabilities.
 - [**VideoGear:**](https://github.com/abhiTronix/vidgear#videogear) Common Video-Capture API with internal [Video Stabilizer](https://abhitronix.github.io/vidgear/latest/gears/stabilizer/overview/) wrapper.
 
 **B. Video-Writer Gears:**
 
 - [**WriteGear:**](https://github.com/abhiTronix/vidgear#writegear) Handles Lossless Video-Writer for file/stream/frames Encoding and Compression.
 
 **C. Streaming Gears:**
@@ -359,17 +359,17 @@
 
 &nbsp;
 
 &nbsp;
 
 ## ScreenGear
 
-> _ScreenGear is designed exclusively for ultra-fast Screencasting, which means it can grab frames from your monitor in real-time, either by defining an area on the computer screen or full-screen, at the expense of inconsiderable latency. ScreenGear also seamlessly support frame capturing from multiple monitors as well as supports multiple backends._
+> _ScreenGear is designed exclusively for targeting rapid Screencasting Capabilities, which means it can grab frames from your monitor in real-time, either by defining an area on the computer screen or full-screen, at the expense of inconsiderable latency. ScreenGear also seamlessly support frame capturing from multiple monitors as well as supports multiple backends._
 
-ScreenGear implements a multi-threaded wrapper around [**pyscreenshot**][pyscreenshot] & [**python-mss**][mss] python library API and also supports an easy and flexible direct internal parameter manipulation.
+ScreenGear implements a Lightning-Fast API wrapper around [**dxcam**][dxcam], [**pyscreenshot**][pyscreenshot] & [**python-mss**][mss] python libraries and also supports an easy and flexible direct internal parameters manipulation.
 
 **Below is a snapshot of a ScreenGear API in action:**
 
 <p align="center">
   <img src="https://abhitronix.github.io/vidgear/latest/assets/gifs/screengear.gif" alt="ScreenGear in action!"/>
 </p>
 
@@ -680,36 +680,36 @@
 
 &nbsp;
 
 # Citation
 
 Here is a Bibtex entry you can use to cite this project in a publication:
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6926196.svg)](https://doi.org/10.5281/zenodo.6926196)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7571405.svg)](https://doi.org/10.5281/zenodo.7571405)
 
 ```BibTeX
 @software{vidgear,
   author       = {Abhishek Thakur and
                   Zoe Papakipos and
                   Christian Clauss and
                   Christian Hollinger and
                   Ian Max Andolina and
                   Vincent Boivin and
                   enarche-ahn and
                   freol35241 and
                   Benjamin Lowe and
                   Mickaël Schoentgen and
                   Renaud Bouckenooghe},
-  title        = {abhiTronix/vidgear: VidGear v0.2.6},
-  month        = jul,
-  year         = 2022,
+  title        = {abhiTronix/vidgear: VidGear v0.3.0},
+  month        = jan,
+  year         = 2023,
   publisher    = {Zenodo},
-  version      = {vidgear-0.2.6},
-  doi          = {10.5281/zenodo.6926196},
-  url          = {https://doi.org/10.5281/zenodo.6926196}
+  version      = {vidgear-0.3.0},
+  doi          = {10.5281/zenodo.7571405},
+  url          = {https://doi.org/10.5281/zenodo.7571405}
 }
 ```
 
 &nbsp;
 
 &nbsp;
 
@@ -808,14 +808,15 @@
 [uvloop]: https://github.com/MagicStack/uvloop
 [streamlink]: https://streamlink.github.io/
 [aiortc]: https://aiortc.readthedocs.io/en/latest/
 [pyscreenshot]: https://github.com/ponty/pyscreenshot
 [uvloop-ns]: https://github.com/MagicStack/uvloop/issues/14
 [ffmpeg]: https://www.ffmpeg.org/
 [flake8]: https://flake8.pycqa.org/en/latest/
+[dxcam]: https://github.com/ra1nty/DXcam
 [black]: https://github.com/psf/black
 [pytest]: https://docs.pytest.org/en/latest/
 [opencv-writer]: https://docs.opencv.org/master/dd/d9e/classcv_1_1VideoWriter.html#ad59c61d8881ba2b2da22cff5487465b5
 [opencv-windows]: https://www.learnopencv.com/install-opencv3-on-windows/
 [opencv-linux]: https://www.pyimagesearch.com/2018/05/28/ubuntu-18-04-how-to-install-opencv/
 [opencv-pi]: https://www.pyimagesearch.com/2018/09/26/install-opencv-4-on-your-raspberry-pi/
 [starlette]: https://www.starlette.io/
```

### Comparing `vidgear-0.3.0/vidgear.egg-info/SOURCES.txt` & `vidgear-0.3.1/vidgear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

