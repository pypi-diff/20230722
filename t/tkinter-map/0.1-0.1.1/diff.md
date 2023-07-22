# Comparing `tmp/tkinter-map-0.1.tar.gz` & `tmp/tkinter-map-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinter-map-0.1.tar", last modified: Sat Jul 15 18:16:18 2023, max compression
+gzip compressed data, was "tkinter-map-0.1.1.tar", last modified: Sat Jul 22 10:38:14 2023, max compression
```

## Comparing `tkinter-map-0.1.tar` & `tkinter-map-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 18:16:18.645045 tkinter-map-0.1/
--rw-rw-rw-   0        0        0      975 2023-07-15 18:16:18.644049 tkinter-map-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       58 2023-07-15 16:39:19.000000 tkinter-map-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 18:16:18.645045 tkinter-map-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1366 2023-07-15 18:16:09.000000 tkinter-map-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:16:18.567280 tkinter-map-0.1/tkinter_map.egg-info/
--rw-rw-rw-   0        0        0      975 2023-07-15 18:16:18.000000 tkinter-map-0.1/tkinter_map.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-07-15 18:16:18.000000 tkinter-map-0.1/tkinter_map.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 18:16:18.000000 tkinter-map-0.1/tkinter_map.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-15 18:16:18.000000 tkinter-map-0.1/tkinter_map.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 18:16:18.636026 tkinter-map-0.1/tkmap/
--rw-rw-rw-   0        0        0      709 2023-07-15 16:42:20.000000 tkinter-map-0.1/tkmap/__init__.py
--rw-rw-rw-   0        0        0     4271 2023-07-15 06:36:56.000000 tkinter-map-0.1/tkmap/bio.py
--rw-rw-rw-   0        0        0     2909 2023-07-15 16:31:10.000000 tkinter-map-0.1/tkmap/model.py
--rw-rw-rw-   0        0        0    14188 2023-07-15 12:33:17.000000 tkinter-map-0.1/tkmap/widget.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:38:14.719296 tkinter-map-0.1.1/
+-rw-rw-rw-   0        0        0     1077 2023-07-16 08:51:05.000000 tkinter-map-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       69 2023-07-19 20:18:55.000000 tkinter-map-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2477 2023-07-22 10:38:14.718309 tkinter-map-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2023-07-20 17:10:37.000000 tkinter-map-0.1.1/README.md
+-rw-rw-rw-   0        0        0        5 2023-07-16 05:22:19.000000 tkinter-map-0.1.1/VERSION
+-rw-rw-rw-   0        0        0       42 2023-07-22 10:38:14.720292 tkinter-map-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2023-07-15 18:16:09.000000 tkinter-map-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:38:14.592548 tkinter-map-0.1.1/tkinter_map.egg-info/
+-rw-rw-rw-   0        0        0     2477 2023-07-22 10:38:13.000000 tkinter-map-0.1.1/tkinter_map.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-07-22 10:38:13.000000 tkinter-map-0.1.1/tkinter_map.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 10:38:13.000000 tkinter-map-0.1.1/tkinter_map.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-22 10:38:13.000000 tkinter-map-0.1.1/tkinter_map.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 10:38:14.635495 tkinter-map-0.1.1/tkmap/
+drwxrwxrwx   0        0        0        0 2023-07-22 10:38:14.714308 tkinter-map-0.1.1/tkmap/.json/
+-rw-rw-rw-   0        0        0      378 2023-07-19 19:23:52.000000 tkinter-map-0.1.1/tkmap/.json/google-map.json
+-rw-rw-rw-   0        0        0      384 2023-07-19 19:25:10.000000 tkinter-map-0.1.1/tkmap/.json/google-satellite.json
+-rw-rw-rw-   0        0        0      254 2023-07-20 16:52:14.000000 tkinter-map-0.1.1/tkmap/.json/mapbox-satellite-2x.json
+-rw-rw-rw-   0        0        0      208 2023-07-20 16:52:09.000000 tkinter-map-0.1.1/tkmap/.json/mapbox-satellite.json
+-rw-rw-rw-   0        0        0      261 2023-07-19 19:15:15.000000 tkinter-map-0.1.1/tkmap/.json/openstreetmap.json
+-rw-rw-rw-   0        0        0     1029 2023-07-20 17:45:17.000000 tkinter-map-0.1.1/tkmap/__init__.py
+-rw-rw-rw-   0        0        0     6690 2023-07-22 09:44:24.000000 tkinter-map-0.1.1/tkmap/bio.py
+-rw-rw-rw-   0        0        0     2293 2023-07-21 17:13:04.000000 tkinter-map-0.1.1/tkmap/model.py
+-rw-rw-rw-   0        0        0    18662 2023-07-22 10:33:44.000000 tkinter-map-0.1.1/tkmap/widget.py
```

### Comparing `tkinter-map-0.1/setup.py` & `tkinter-map-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tkinter-map-0.1/tkmap/widget.py` & `tkinter-map-0.1.1/tkmap/widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,101 @@
 # -*- coding:utf-8 -*-
+"""
+This module provides the core widget of tkmap package.
+"""
+
 import os
 import time
 import json
 import queue
 import tkinter
 import logging
-import threading
 import functools
-import collections
 
 from tkmap import JSON, load_img_package, bio, model
 from typing import List, Tuple
 from tkinter import ttk
 
 
 class Tile:
+    """
+    `Tile` class to leverage the tcl interpreter to perform fast image
+    operation on canvas.
+
+    Attributes:
+        TILE_CMD_CREATE (str): (class attribute) tcl command pattern to create
+            the image canvas item.
+        TILE_CMD_SHOW (str): (class attribute) tcl command pattern to show the
+            image canvas item.
+        TILE_CMD_HIDE (str): (class attribute) tcl command pattern to hide the
+            image canvas item.
+        TILE_CMD_CLEAR (str): (class attribute) tcl command pattern to delete
+            the image data.
+        tkeval (callable): (class attribute) the tk `eval` command.
+        tkcall (callable): (class attribute) the tk `call` command.
+        w_name (str): master canvas name.
+    """
 
     TILE_CMD_CREATE = \
         "if {[%(w)s find withtag %(t)s] eq {}} { " +\
         "%(w)s lower [%(w)s create image " +\
         "[expr {%(c)s * [image width %(n)s]}] " +\
         "[expr {%(r)s * [image height  %(n)s]}] " +\
         "-anchor nw -image %(n)s -tags {%(t)s tile} -state hidden] }"
     TILE_CMD_SHOW = "%(w)s itemconfig %(t)s -state normal; update"
     TILE_CMD_HIDE = "%(w)s itemconfig %(t)s -state hidden"
-    TILE_CMD_CLEAR = "image delete %(t)s"
+    TILE_CMD_CLEAR = "%(w)s delete %(t)s; image delete %(t)s"
     tkeval = None
     tkcall = None
 
-    def __init__(self, master: tkinter.BaseWidget) -> None:
+    def __init__(self, master: tkinter.Canvas) -> None:
+        """
+        Args:
+            master (tkinter.Canvas): master canvas instance on wich tile is
+                about to be managed.
+        """
+        # initialize tk `eval` and `call` shortcuts they not exist.
         if Tile.tkeval is None or Tile.tkcall is None:
             Tile.tkeval = master.tk.eval
             Tile.tkcall = master.tk.call
         self.w_name = master._w
 
     def create(self, tag: str, data: str) -> None:
+        """
+        Create the image data inside tcl interpreter and generate the
+        associated canvas image-item.
+
+        Args:
+            tag (str): tile tag with format `{zoom}_{row}_{col}`.
+            data (str): image data as string.
+        """
         imgtk = \
             Tile.tkcall("image", "create", "photo", tag, "-data", data)
         _, row, col = tag.split("_")
         args = {"w": self.w_name, "n": imgtk, "r": row, "c": col, "t": tag}
         Tile.tkeval(Tile.TILE_CMD_CREATE % args)
         self._clear = Tile.TILE_CMD_CLEAR % args
         self._hide = Tile.TILE_CMD_HIDE % args
         self._show = Tile.TILE_CMD_SHOW % args
         self._imgtk = imgtk
 
     def show(self) -> None:
+        "Reveal the image item on the canvas."
         logging.info(f" -> {__class__.__name__} {self._imgtk} show")
         Tile.tkeval(self._show)
 
     def hide(self) -> None:
+        "Hide the image item from the canvas."
         logging.info(f" -> {__class__.__name__} {self._imgtk} hidden")
         Tile.tkeval(self._hide)
 
     def clear(self) -> None:
+        """
+        Delete the image item from canvas and image data from tcl interpreter.
+        """
         logging.info(f" -> {__class__.__name__} {self._imgtk} cleared")
         Tile.tkeval(self._clear)
 
 
 # inertia computation @ 100Hz & k = 0.9
 def _drift(obj: tkinter.Canvas, speed_x: float, speed_y: float) -> None:
     t = time.time()
@@ -90,68 +128,76 @@
         obj._drawarea = obj.drawarea
         obj._update()
 
     # _update canvas with queued tiles
     while not obj.DONE.empty():
         try:
             tag, data = obj.DONE.get()
-            tile = Tile(obj)
-            tile.create(tag, data)
-            tile.show()
-            obj.cache[tag] = tile
+            if data:
+                tile = Tile(obj)
+                tile.create(tag, data)
+                tile.show()
+                obj.cache[tag] = tile
             with obj.QUEUED.mutex:
                 if tag in obj.QUEUED.queue:
                     obj.QUEUED.queue.remove(tag)
         except Exception as error:
-            logging.error(f" -> _drawloop error: {error} - tag {tag}")
+            logging.error(
+                f" -> _drawloop error: {error} - tag {tag}",
+                # exc_info=True
+            )
     # clean _after_tasks list
     for callback in obj._after_tasks[:]:
         # if task info unavailable (it raises TclError) then it is running or
         # terminated
         try:
             obj.tk.eval(f"after info {callback}")
         except tkinter.TclError:
             obj._after_tasks.remove(callback)
 
 
 class Tkmap(tkinter.Canvas):
-
-    LOCK = threading.Lock()
-
-    @property
-    def xnw(obj) -> float:
-        return float(obj.tk.eval(f"{obj._w} canvasx 0"))
-
-    @property
-    def ynw(obj) -> float:
-        return float(obj.tk.eval(f"{obj._w} canvasy 0"))
+    """
+    `Tkmap` is a `tkinter.Canvas` object that leverages directly tcl code to
+    provide a smooth user experience.
+
+    Attributes:
+        coords (tkinter.Label): widget to display map coordinates.
+        framerate (int): rate of canvas update.
+        cachesize (int): number of tile stored in Tkmap cache.
+        cache (dict): tile cache.
+        mapmodel (model.MapMode): map model used to generate tile url and
+            compute map coordinates.
+        workers (List[bio.TileWorker]): List of python thread used to perform
+            tile downloads or database queries.
+    """
 
     @property
-    def xse(obj) -> float:
-        return float(
-            obj.tk.eval(f"{obj._w} canvasx [expr [winfo width {obj._w}]]")
-        )
-
-    @property
-    def yse(obj) -> float:
-        return float(
-            obj.tk.eval(f"{obj._w} canvasy [expr [winfo height {obj._w}]]")
-        )
+    def bbox(obj) -> tuple:
+        "Returns east, north, west and south boundaries view on canvas area."
+        return [
+            int(float(e)) for e in obj.tk.eval(
+                f"list [{obj._w} canvasx 0] [{obj._w} canvasy 0]"
+                f" [{obj._w} canvasx [expr [winfo width {obj._w}]]]"
+                f" [{obj._w} canvasy [expr [winfo height {obj._w}]]]"
+            ).split()
+        ]
 
     def __init__(self, master=None, cnf={}, **kw) -> None:
         self.framerate = kw.pop("framerate", 4)
-        self.cachesize = kw.pop("framerate", 500)
+        self.cachesize = kw.pop("cachesize", 500)
 
         tkinter.Canvas.__init__(self, master, cnf, **kw)
         self["xscrollincrement"] = self["yscrollincrement"] = 1
 
-        ttk.Label(
+        self.coords = ttk.Label(
             relief="solid", padding=(5, 1),
             font=("calibri", "8"), textvariable="coords"
-        ).place(y=4, relx=0.5, anchor="n")
+        )
+        self._coords_place = dict(y=-4, rely=1.0, relx=0.5, anchor="s")
 
         load_img_package(self.tk)
 
         self.JOB = queue.LifoQueue()
         self.DONE = queue.LifoQueue()
         self.QUEUED = queue.Queue()
 
@@ -166,83 +212,117 @@
 
         self.borderwidth = 0
         self.drawarea = ()
         self.mapsize = 1, 1
         self.radius = 0
         self.zoom = 0
 
-    def save_location(self) -> None:
+    def place_widget(self, widget: str, cnf={}, **kw) -> None:
+        """
+        Place inner widgets on the canvas instance.
+
+        Args:
+            widget (str): widget attribute name to place.
+            cnf (dict): key-value pairs to place the widget.
+            **kw: keywords arguments to place the widget.
+        """
+        getattr(self, f"_{widget}_place").update(cnf, **kw)
+        getattr(self, widget).place(**self._coords_place)
+
+    def dump_location(self) -> None:
+        "Drops cursor location into filesystem"
         if self.mapmodel is not None:
             self.save_coords(self.winfo_width()/2, self.winfo_height()/2)
             with open(os.path.join(JSON, ".loc"), "w") as out:
                 json.dump({"zoom": self.zoom, "latlon": self.latlon}, out)
 
+    def save_coords(self, x: float = None, y: float = None) -> None:
+        """
+        Save map coordinates from canvas center or specific coordinates
+
+        Args:
+            x (float): horizontal pixel coordinates.
+            y (float): vertical pixel coordinates.
+        """
+        self.latlon = list(
+            self.mapmodel.xy2ll(
+                self.canvasx(x or self.winfo_width()/2),
+                self.canvasy(y or self.winfo_height()/2),
+                self.zoom
+            )
+        )
+
     def load_location(self) -> None:
+        "loads last saved location from filesystem"
         try:
             with open(os.path.join(JSON, ".loc"), "r") as in_:
                 return json.load(in_)
         except Exception:
             return {}
 
     def open(
         self, model: model.MapModel, zoom: int = None,
         location: List[float] = None
     ) -> None:
+        """
+        Open a map.
+
+        Args:
+            model (model.MapModel): map tile provider.
+            zoom (int): zoom level to start at. If not provided, starts to 0
+                or previously saved zoom level.
+            location (List[float]): location to start at. If not provided,
+                starts at longitude 0 and latitude 0 or previously saved
+                location.
+        """
         self.close()
         data = self.load_location()
         self.zoom = zoom or data.get("zoom", 0)
         self.latlon = location or data.get("latlon", [0., 0.])
         self.tk.setvar(
             "coords",
             f"lat {self.latlon[0]:3.5f}° | lon {self.latlon[1]:3.5f}°"
         )
         self.mapmodel = model
         model.init(self)
         self.center()
         self._start()
+        self.place_widget("coords")
 
     def close(self) -> None:
+        "Close the map and clear the canvas."
+        self.coords.place_forget()
         self._stop()
-        self.clear_canvas()
-        self.save_location()
+        self._drawarea = ()
+        self.cache.clear()
+        self.dump_location()
         self.mapmodel = None
 
     def center(self, px: float = None, py: float = None) -> None:
-        px = px or self.winfo_width()/2
-        py = py or self.winfo_height()/2
-        nrow, ncol = self.mapsize
-        width = ncol * self.mapmodel.tile_w
-        height = nrow * self.mapmodel.tile_h
+        """
+        Align canvas center or coordinates to the last saved coordinates.
+
+        Args:
+            px (float): horizontal pixel coordinates.
+            py (float): vertical pixel coordinates.
+        """
+        x1, y1, x2, y2 = [int(e) for e in self["scrollregion"].split()]
+        width, height = x2 - x1, y2 - y1
         x, y = self.mapmodel.ll2xy(*self.latlon, zoom=self.zoom)
         self.xview_moveto(
-            (width * x/width - px or self.winfo_width()/2) / width
+            (width * x/width - (px or self.winfo_width()/2)) / width
         )
         self.yview_moveto(
-            (height * y/height - py or self.winfo_height()/2) / height
+            (height * y/height - (py or self.winfo_height()/2)) / height
         )
 
-    def clear_canvas(self, keep_cache: bool = False) -> None:
-        if not keep_cache:
-            self.cache.clear()
-        else:
-            [tile.hide() for tile in self.cache.values()]
-
     def destroy(self) -> None:
         self.close()
         tkinter.Canvas.destroy(self)
 
-    def save_coords(self, x: float = None, y: float = None) -> None:
-        self.latlon = list(
-            self.mapmodel.xy2ll(
-                self.canvasx(x or self.winfo_width()/2),
-                self.canvasy(y or self.winfo_height()/2),
-                self.zoom
-            )
-        )
-
     def _cancel_tasks(self) -> None:
         for callback in self._after_tasks:
             try:
                 self.tk.eval(f"after cancel {callback}")
             except tkinter.TclError:
                 pass
         self._after_tasks.clear()
@@ -270,32 +350,34 @@
         self.unbind("<Button-1>")
         self.unbind("<B1-Motion>")
         self.unbind("<Motion>")
         self.unbind("<ButtonRelease-1>")
         self.unbind("<MouseWheel>")
         self.unbind("<Configure>")
         self.unbind("<Control-B1-Motion>")
-        with Tkmap.LOCK:
-            while len(self.workers):
-                self.workers.pop(0).kill()
-            self._clear_queues()
+        self._clear_queues()
+        while len(self.workers):
+            worker = self.workers.pop(0)
+            worker.kill()
 
     def _update_drawarea(self) -> None:
         tw, th = self.mapmodel.tilesize
         nr, nc = self.mapsize
         bd = self.borderwidth
+        e, n, w, s = self.bbox
         self.drawarea = (
-            int(max(0, self.xnw//tw-bd)), int(max(0, self.ynw//th-bd)),
-            int(min(nr, self.xse//tw+bd)), int(min(nc, self.yse//th+bd))
+            max(0, e//tw-bd), max(0, n//th-bd),
+            min(nr, w//tw+bd), min(nc, s//th+bd)
         )
 
     def _update(self) -> None:
         c1, r1, c2, r2 = self.drawarea
-        radius = self.radius
+        e, n, w, s = self.bbox
         cmd = self.tk.eval
+        r = self.radius
         _w = self._w
 
         tags_to_show = set(
             functools.reduce(
                 list.__add__,
                 (
                     [f"{self.zoom}_{r}_{c}" for c in range(c1, c2)]
@@ -307,39 +389,39 @@
         cached_tiles = set(self.cache.keys())
         for tag in tags_to_show - cached_tiles:
             if tag not in self.QUEUED.queue:
                 self.QUEUED.put(tag)
                 self.JOB.put([tag, self.mapmodel])
 
         all_tiles = cmd(f"{_w} find overlapping {self['scrollregion']}")
-        tile_to_show = cmd(
-            f"{_w} find overlapping "
-            f"{self.xnw - radius} {self.ynw - radius} "
-            f"{self.xse + radius} {self.yse + radius}"
-        )
+        tile_to_show = \
+            cmd(f"{_w} find overlapping {e - r} {n - r} {w + r} {s + r}")
         tile_to_hide = set(all_tiles.split()) - set(tile_to_show.split())
         standing_by_tiles = tags_to_show & cached_tiles
 
         try:
             cmd(
                 "foreach id {" + " ".join(tile_to_hide) + "} "
                 "{" + _w + " itemconfig $id -state hidden};"
                 "foreach tag {" + " ".join(standing_by_tiles) + "} "
                 "{" + _w + " itemconfig $tag -state normal};"
             )
         except tkinter.TclError as error:
             # due to cache size limitation some images may be deleted
             # during the tcl command execution
-            logging.info(f" -> _update error: {error}")
+            logging.info(
+                f" -> _update error: {error}",
+                # exc_info=True
+            )
 
     def _clear_queues(self) -> None:
-        with self.JOB.mutex:
-            self.JOB.queue.clear()
         with self.DONE.mutex:
             self.DONE.queue.clear()
+        with self.JOB.mutex:
+            self.JOB.queue.clear()
         with self.QUEUED.mutex:
             self.QUEUED.queue.clear()
 
     def on_button_1(self, event: tkinter.Event) -> None:
         self.configure(cursor="fleur")
         self.tk.call(self._w, 'scan', 'mark', event.x, event.y)
         self._tps = [time.time(), event.x, event.y, 0., 0.]
@@ -349,69 +431,98 @@
             self.canvasx(event.x), self.canvasy(event.y), self.zoom
         )
         self.tk.setvar("coords", f"lat {lat:3.5f}° | lon {lon:3.5f}°")
 
     def on_button_1_motion(self, event: tkinter.Event, gain: int = 1) -> None:
         self.tk.call(self._w, 'scan', 'dragto', event.x, event.y, gain)
         self._update_drawarea()
-        # speed computation
+        # speed cursor computation
         t, x, y = time.time(), event.x, event.y
         dt = t - self._tps[0]
         if dt >= 0.01:
             self._tps[-2] = (x - self._tps[1]) / dt
             self._tps[-1] = (y - self._tps[2]) / dt
             self._tps[:3] = [t, x, y]
 
     def on_button_1_release(self, event: tkinter.Event) -> None:
         self.configure(cursor="arrow")
         self.save_coords()
         if self._tps[0]:
             self._tps[0] = None
-            self._tps[1] = time.time()
+            self._tps[1] = time.time()  # needed by _drift definition
             speed_x, speed_y = self._tps[-2:]
             self.after(10, lambda: _drift(self, -speed_x, -speed_y))
 
     def on_mouse_wheel(self, event: tkinter.Event) -> None:
         zoom_max = getattr(self.mapmodel, "zoom_max", 17)
         delta = 1 if event.num == 4 or event.delta == 120 else -1
         zoom = min(max(0, self.zoom + delta), zoom_max)
         if zoom == self.zoom:
             return
 
         self.save_coords(event.x, event.y)
         self.zoom = zoom
-        with Tkmap.LOCK:
-            self._clear_queues()
-            self.clear_canvas(keep_cache=True)
-            self.mapmodel.init(self)
-            self.center(event.x, event.y)
-            self._update_drawarea()
+
+        self._clear_queues()
+        self.cache.hide()
+        self.mapmodel.init(self)
+        self.center(event.x, event.y)
+        self._drawarea = ()
+        self._update_drawarea()
 
 
 class Cache(dict):
 
+    HIDE_ALL = \
+        "foreach tag {%(tags)s} {%(widget)s itemconfig $tag -state hidden};"
+    DELETE_ALL = \
+        'image delete %(tags)s; %(widget)s delete "all";'
+
     def __init__(self, *args, **kwargs) -> None:
-        self.size = kwargs.pop("size", 150)
-        self.store = collections.deque()
+        self.size = kwargs.pop("size", -1)
+        self.store = []
         self.update(dict(*args, **kwargs))
 
     def __setitem__(self, key: str, value: Tile) -> None:
         self.store.append(key)
-        if len(self.store) > self.size:
-            tile = self.pop(self.store[0])
-            tile.clear()
+        if self.size > 0 and len(self.store) > self.size:
+            popped = False
+            i = 0
+            while not popped and i < len(self):
+                tile = self[self.store[i]]
+                if tile.tkeval(
+                    f"{tile.w_name} itemcget {tile._imgtk} -state"
+                ) == 'hidden':
+                    logging.info(
+                        f" -> {__class__.__name__} {tile._imgtk} popped"
+                    )
+                    self.pop(self.store[i]).clear()
+                    popped = True
+                i += 1
         dict.__setitem__(self, key, value)
 
+    def hide(self) -> None:
+        if len(self.store):
+            tile0 = self[self.store[0]]
+            tile0.tkeval(
+                Cache.HIDE_ALL %
+                {"tags": " ".join(self.keys()), "widget": tile0.w_name}
+            )
+
     def clear(self) -> None:
-        self.store.clear()
-        for tile in self.values():
-            tile.clear()
+        if len(self.store):
+            tile0 = self[self.store[0]]
+            tile0.tkeval(
+                Cache.DELETE_ALL %
+                {"tags": " ".join(self.keys()), "widget": tile0.w_name}
+            )
+            self.store.clear()
         dict.clear(self)
 
     def pop(self, key: str) -> Tile:
         self.store.remove(key)
         return dict.pop(self, key)
 
     def popitem(self) -> Tuple[str, Tile]:
         item = dict.popitem(self)
-        self.Store.remove(item[0])
+        self.store.remove(item[0])
         return item
```

