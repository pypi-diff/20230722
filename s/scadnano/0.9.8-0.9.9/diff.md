# Comparing `tmp/scadnano-0.9.8.tar.gz` & `tmp/scadnano-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scadnano-0.9.8.tar", last modified: Thu Jul  9 23:55:07 2020, max compression
+gzip compressed data, was "dist\scadnano-0.9.9.tar", last modified: Sat Jul 11 22:13:55 2020, max compression
```

## Comparing `scadnano-0.9.8.tar` & `scadnano-0.9.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2020-07-09 23:55:07.464174 scadnano-0.9.8/
--rw-rw-rw-   0        0        0    11589 2020-07-09 23:55:07.464174 scadnano-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     9470 2020-07-07 15:06:41.000000 scadnano-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2020-07-09 23:55:07.456196 scadnano-0.9.8/scadnano/
--rw-rw-rw-   0        0        0       74 2020-07-03 15:22:00.000000 scadnano-0.9.8/scadnano/__init__.py
--rw-rw-rw-   0        0        0      382 2020-07-09 23:52:12.000000 scadnano-0.9.8/scadnano/_version.py
--rw-rw-rw-   0        0        0      911 2020-07-03 15:22:00.000000 scadnano-0.9.8/scadnano/modifications.py
--rw-rw-rw-   0        0        0    28436 2020-07-05 22:54:42.000000 scadnano-0.9.8/scadnano/origami_rectangle.py
--rw-rw-rw-   0        0        0   233120 2020-07-09 23:52:19.000000 scadnano-0.9.8/scadnano/scadnano.py
-drwxrwxrwx   0        0        0        0 2020-07-09 23:55:07.463178 scadnano-0.9.8/scadnano.egg-info/
--rw-rw-rw-   0        0        0    11589 2020-07-09 23:55:07.000000 scadnano-0.9.8/scadnano.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2020-07-09 23:55:07.000000 scadnano-0.9.8/scadnano.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-09 23:55:07.000000 scadnano-0.9.8/scadnano.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2020-07-09 23:55:07.000000 scadnano-0.9.8/scadnano.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2020-07-09 23:55:07.465171 scadnano-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1842 2020-07-03 15:22:00.000000 scadnano-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-07-11 22:13:55.454939 scadnano-0.9.9/
+-rw-rw-rw-   0        0        0    12483 2020-07-11 22:13:55.455936 scadnano-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10284 2020-07-11 20:39:32.000000 scadnano-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2020-07-11 22:13:55.448954 scadnano-0.9.9/scadnano/
+-rw-rw-rw-   0        0        0       74 2020-07-03 15:22:00.000000 scadnano-0.9.9/scadnano/__init__.py
+-rw-rw-rw-   0        0        0      382 2020-07-11 22:11:57.000000 scadnano-0.9.9/scadnano/_version.py
+-rw-rw-rw-   0        0        0      911 2020-07-03 15:22:00.000000 scadnano-0.9.9/scadnano/modifications.py
+-rw-rw-rw-   0        0        0    28436 2020-07-05 22:54:42.000000 scadnano-0.9.9/scadnano/origami_rectangle.py
+-rw-rw-rw-   0        0        0   235523 2020-07-11 22:12:04.000000 scadnano-0.9.9/scadnano/scadnano.py
+drwxrwxrwx   0        0        0        0 2020-07-11 22:13:55.453941 scadnano-0.9.9/scadnano.egg-info/
+-rw-rw-rw-   0        0        0    12483 2020-07-11 22:13:55.000000 scadnano-0.9.9/scadnano.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2020-07-11 22:13:55.000000 scadnano-0.9.9/scadnano.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-07-11 22:13:55.000000 scadnano-0.9.9/scadnano.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2020-07-11 22:13:55.000000 scadnano-0.9.9/scadnano.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2020-07-11 22:13:55.456933 scadnano-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1842 2020-07-03 15:22:00.000000 scadnano-0.9.9/setup.py
```

### Comparing `scadnano-0.9.8/PKG-INFO` & `scadnano-0.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: scadnano
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python scripting library for generating designs readable by scadnano.
 Home-page: https://github.com/UC-Davis-molecular-computing/scadnano-python-package
 Author: David Doty
 Author-email: doty@ucdavis.edu
 License: MIT
-Download-URL: https://github.com/UC-Davis-molecular-computing/scadnano-python-package/archive/v0.9.8.zip
+Download-URL: https://github.com/UC-Davis-molecular-computing/scadnano-python-package/archive/v0.9.9.zip
 Description: # scadnano-python-package
         
         ![Python package](https://github.com/UC-Davis-molecular-computing/scadnano-python-package/workflows/Python%20package/badge.svg)
         [![Documentation Status](https://readthedocs.org/projects/scadnano-python-package/badge/?version=latest)](https://scadnano-python-package.readthedocs.io/en/latest/?badge=latest)
         
         The scadnano Python module is a library for describing synthetic DNA nanostructures (e.g., DNA origami).
         
         
         If you find scadnano useful in a scientific project, please cite its associated paper:
         
-        > <ins>scadnano: A browser-based, scriptable tool for designing DNA nanostructures</ins>.  
+        > scadnano: A browser-based, scriptable tool for designing DNA nanostructures.  
           David Doty, Benjamin L Lee, and Tristan Stérin.  
           DNA 2020: *Proceedings of the 26th International Conference on DNA Computing and Molecular Programming*  
           [ [paper](https://arxiv.org/abs/2005.11841) | [BibTeX](https://web.cs.ucdavis.edu/~doty/papers/scadnano.bib) ]
         
         
         ## Overview
         
@@ -42,17 +42,25 @@
         
         
         
         
         
         ## Installation
         
-        The scadnano Python package requires Python version 3.7 or later. If you do not have that version (or later) of Python installed, follow [this link](https://www.python.org/downloads/) to install it.
+        The scadnano Python package requires Python version 3.7 or later. If you do not have that version (or later) of Python installed, follow [this link](https://www.python.org/downloads/) to install it. 
         
-        Once Python is installed, there are two ways you can install the scadnano Python package:
+        If you are using Python 3.6 and do not wish to upgrade, with some effort you can install a package that give the required features.
+        The Python 3.7 module that is not present in 3.6 is the 
+        [dataclasses](https://docs.python.org/3/library/dataclasses.html) module.
+        You can install a backported library for it: 
+        [dataclasses backport](https://pypi.org/project/dataclasses/) (this library appears to require at least Python version 3.6)
+        
+        Furthermore, the [typing](https://docs.python.org/3/library/typing.html) module was present in Python 3.5, but scadnano requires at least version Python 3.6.2.
+        
+        Once Python is installed (and the dataclasses backport if you have Python version 3.6), there are two ways you can install the scadnano Python package:
         
         
         1. pip (recommended)
         
             Use [pip](https://pypi.org/project/pip/) to install the package by executing the following at the command line:
             ```console
             pip install scadnano
@@ -63,15 +71,17 @@
             see also 
             https://docs.python.org/3/installing/index.html 
             or 
             https://www.liquidweb.com/kb/install-pip-windows/.
         
         2. download
         
-            As a simple alternative (in case you run into trouble using pip), you can download and place the following files (located in the [scadnano/](https://github.com/UC-Davis-molecular-computing/scadnano-python-package/tree/master/scadnano) subfolder) in your PYTHONPATH (e.g., in the same directory as the scripts you are running). To download them, right-click on "Raw" near the top and select (in Chrome or Firefox) "Save link as...)
+            *Note:* If you are reading this on the PyPI website, the links below won't work. They are relative links intended to be read on the [GitHub README page](https://github.com/UC-Davis-molecular-computing/scadnano-python-package#readme).
+        
+            As a simple alternative (in case you run into trouble using pip), you can download and place the following files (located in the [scadnano/](scadnano) subfolder) in your PYTHONPATH (e.g., in the same directory as the scripts you are running). To download them, right-click on "Raw" near the top and select (in Chrome or Firefox) "Save link as...". 
         
             * *required*: [scadnano.py](scadnano/scadnano.py) 
             * *optional*: [modifications.py](scadnano/modifications.py); This contains some common DNA modifications such as biotin and Cy3. 
             * *optional*: [origami_rectangle.py](scadnano/origami_rectangle.py); This can help create origami rectangles, but it is not necessary to use scadnano.
             * *optional*: [_version.py](scadnano/_version.py) This ensures that the current version number is written into any `.dna` files written by the library; otherwise it may be out of date. (Which should not matter for the most part.)
             
             The scadnano package uses the Python package [xlwt](https://pypi.org/project/xlwt/) to write Excel files, so in order to call the method [`DNADesign.write_idt_plate_excel_file()`](https://scadnano-python-package.readthedocs.io/#scadnano.DNADesign.write_idt_plate_excel_file) to export an Excel file with DNA sequences, xlwt must be installed. To install, type `pip install xlwt` at the command line.
```

### Comparing `scadnano-0.9.8/README.md` & `scadnano-0.9.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Documentation Status](https://readthedocs.org/projects/scadnano-python-package/badge/?version=latest)](https://scadnano-python-package.readthedocs.io/en/latest/?badge=latest)
 
 The scadnano Python module is a library for describing synthetic DNA nanostructures (e.g., DNA origami).
 
 
 If you find scadnano useful in a scientific project, please cite its associated paper:
 
-> <ins>scadnano: A browser-based, scriptable tool for designing DNA nanostructures</ins>.  
+> scadnano: A browser-based, scriptable tool for designing DNA nanostructures.  
   David Doty, Benjamin L Lee, and Tristan Stérin.  
   DNA 2020: *Proceedings of the 26th International Conference on DNA Computing and Molecular Programming*  
   [ [paper](https://arxiv.org/abs/2005.11841) | [BibTeX](https://web.cs.ucdavis.edu/~doty/papers/scadnano.bib) ]
 
 
 ## Overview
 
@@ -33,17 +33,25 @@
 
 
 
 
 
 ## Installation
 
-The scadnano Python package requires Python version 3.7 or later. If you do not have that version (or later) of Python installed, follow [this link](https://www.python.org/downloads/) to install it.
+The scadnano Python package requires Python version 3.7 or later. If you do not have that version (or later) of Python installed, follow [this link](https://www.python.org/downloads/) to install it. 
 
-Once Python is installed, there are two ways you can install the scadnano Python package:
+If you are using Python 3.6 and do not wish to upgrade, with some effort you can install a package that give the required features.
+The Python 3.7 module that is not present in 3.6 is the 
+[dataclasses](https://docs.python.org/3/library/dataclasses.html) module.
+You can install a backported library for it: 
+[dataclasses backport](https://pypi.org/project/dataclasses/) (this library appears to require at least Python version 3.6)
+
+Furthermore, the [typing](https://docs.python.org/3/library/typing.html) module was present in Python 3.5, but scadnano requires at least version Python 3.6.2.
+
+Once Python is installed (and the dataclasses backport if you have Python version 3.6), there are two ways you can install the scadnano Python package:
 
 
 1. pip (recommended)
 
     Use [pip](https://pypi.org/project/pip/) to install the package by executing the following at the command line:
     ```console
     pip install scadnano
@@ -54,15 +62,17 @@
     see also 
     https://docs.python.org/3/installing/index.html 
     or 
     https://www.liquidweb.com/kb/install-pip-windows/.
 
 2. download
 
-    As a simple alternative (in case you run into trouble using pip), you can download and place the following files (located in the [scadnano/](https://github.com/UC-Davis-molecular-computing/scadnano-python-package/tree/master/scadnano) subfolder) in your PYTHONPATH (e.g., in the same directory as the scripts you are running). To download them, right-click on "Raw" near the top and select (in Chrome or Firefox) "Save link as...)
+    *Note:* If you are reading this on the PyPI website, the links below won't work. They are relative links intended to be read on the [GitHub README page](https://github.com/UC-Davis-molecular-computing/scadnano-python-package#readme).
+
+    As a simple alternative (in case you run into trouble using pip), you can download and place the following files (located in the [scadnano/](scadnano) subfolder) in your PYTHONPATH (e.g., in the same directory as the scripts you are running). To download them, right-click on "Raw" near the top and select (in Chrome or Firefox) "Save link as...". 
 
     * *required*: [scadnano.py](scadnano/scadnano.py) 
     * *optional*: [modifications.py](scadnano/modifications.py); This contains some common DNA modifications such as biotin and Cy3. 
     * *optional*: [origami_rectangle.py](scadnano/origami_rectangle.py); This can help create origami rectangles, but it is not necessary to use scadnano.
     * *optional*: [_version.py](scadnano/_version.py) This ensures that the current version number is written into any `.dna` files written by the library; otherwise it may be out of date. (Which should not matter for the most part.)
     
     The scadnano package uses the Python package [xlwt](https://pypi.org/project/xlwt/) to write Excel files, so in order to call the method [`DNADesign.write_idt_plate_excel_file()`](https://scadnano-python-package.readthedocs.io/#scadnano.DNADesign.write_idt_plate_excel_file) to export an Excel file with DNA sequences, xlwt must be installed. To install, type `pip install xlwt` at the command line.
```

### Comparing `scadnano-0.9.8/scadnano/modifications.py` & `scadnano-0.9.9/scadnano/modifications.py`

 * *Files identical despite different names*

### Comparing `scadnano-0.9.8/scadnano/origami_rectangle.py` & `scadnano-0.9.9/scadnano/origami_rectangle.py`

 * *Files identical despite different names*

### Comparing `scadnano-0.9.8/scadnano/scadnano.py` & `scadnano-0.9.9/scadnano/scadnano.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 value than it had originally.
 However, due to Python naming conventions for dataclass fields and property setters,
 it is not straightforward to enforce that the fields cannot be written, 
 so the user must take care not to set them.
 """
 
 # needed to use forward annotations: https://docs.python.org/3/whatsnew/3.7.html#whatsnew37-pep563
-from __future__ import annotations
+# commented out for now to support Python 3.6, which does not support this feature
+# from __future__ import annotations
 
 import dataclasses
 from abc import abstractmethod, ABC
 import json
 import enum
 import itertools
 import re
@@ -59,15 +60,15 @@
 # Don't really understand why, but an explicit import solves the issue described here
 # https://stackoverflow.com/a/39131141
 # solves the build problems: https://github.com/UC-Davis-molecular-computing/scadnano-python-package/actions/runs/125490116
 try:
     from ._version import __version__
 except ImportError:
     # this is so scadnano.py file works without _version.py being present, in case user downloads it
-    __version__ = "0.9.8"
+    __version__ = "0.9.9"
 
 StrandLabel = TypeVar('StrandLabel')
 DomainLabel = TypeVar('DomainLabel')
 
 
 def _pairwise(iterable):
     """s -> (s0,s1), (s1,s2), (s2, s3), ..."""
@@ -138,26 +139,26 @@
 # Colors
 # As with JSON serialization, there are external libraries to handle colors
 # in Python, but I want this to be a simple, single-file library, so we just
 # implement what we need below.
 
 @dataclass
 class Color(_JSONSerializable):
-    r: int = None
+    r: Optional[int] = None
     """
     Red component: 0-255.
     
     Optional if :py:data:`Color.hex` is given."""
 
-    g: int = None
+    g: Optional[int] = None
     """Green component: 0-255.
     
     Optional if :py:data:`Color.hex` is given."""
 
-    b: int = None
+    b: Optional[int] = None
     """Blue component: 0-255.
     
     Optional if :py:data:`Color.hex` is given."""
 
     hex_string: InitVar[str] = None
     """Hex color preceded by # sign, e.g., "#ff0000" is red.
     
@@ -225,15 +226,15 @@
     # """List of colors to cycle through."""
 
     def __init__(self):
         self._current_color_idx = 0
         # random order
         order = [3, 11, 0, 12, 8, 1, 10, 6, 5, 9, 4, 7, 2]
         # order = range(len(self._colors))
-        colors_shuffled: List[Color] = [None] * len(self._colors)
+        colors_shuffled: List[Color] = list(self._colors)
         for i, color in zip(order, self._colors):
             colors_shuffled[i] = color
         self._colors: List[Color] = colors_shuffled
 
     def __iter__(self):
         # need to make ColorCycler an iterator
         return self
@@ -787,30 +788,30 @@
     Use :any:`Modification3Prime`, :any:`Modification5Prime`, or :any:`ModificationInternal`
     to instantiate."""
 
     display_text: str
     """Short text to display in the web interface as an "icon"
     visually representing the modification, e.g., ``'B'`` for biotin or ``'Cy3'`` for Cy3."""
 
-    id: str = None
+    id: str = "WARNING: no id assigned to modification"
     """Short representation as a string; used to write in :any:`Strand` json representation,
     while the full description of the modification is written under a global key in the :any:`DNADesign`."""
 
     idt_text: Optional[str] = None
     """IDT text string specifying this modification (e.g., '/5Biosg/' for 5' biotin). optional"""
 
     def to_json_serializable(self, suppress_indent: bool = True):
         ret = {mod_display_text_key: self.display_text}
         if self.idt_text is not None:
             ret[mod_idt_text_key] = self.idt_text
-            ret[mod_display_connector_key] = False
+            ret[mod_display_connector_key] = False  # type: ignore
         return ret
 
     @staticmethod
-    def from_json(json_map: dict) -> Modification:
+    def from_json(json_map: dict) -> 'Modification':  # remove quotes when Python 3.6 support dropped
         location = json_map[mod_location_key]
         if location == "5'":
             return Modification5Prime.from_json(json_map)
         elif location == "3'":
             return Modification3Prime.from_json(json_map)
         elif location == "internal":
             return ModificationInternal.from_json(json_map)
@@ -824,15 +825,15 @@
 
     def to_json_serializable(self, suppress_indent: bool = True):
         ret = super().to_json_serializable(suppress_indent)
         ret[mod_location_key] = "5'"
         return ret
 
     @staticmethod
-    def from_json(json_map: dict) -> Modification5Prime:
+    def from_json(json_map: dict) -> 'Modification5Prime':  # remove quotes when Python 3.6 support dropped
         display_text = json_map[mod_display_text_key]
         location = json_map[mod_location_key]
         assert location == "5'"
         idt_text = json_map.get(mod_idt_text_key)
         return Modification5Prime(display_text=display_text, idt_text=idt_text)
 
 
@@ -842,15 +843,15 @@
 
     def to_json_serializable(self, suppress_indent: bool = True):
         ret = super().to_json_serializable(suppress_indent)
         ret[mod_location_key] = "3'"
         return ret
 
     @staticmethod
-    def from_json(json_map: dict) -> Modification3Prime:
+    def from_json(json_map: dict) -> 'Modification3Prime':  # remove quotes when Python 3.6 support dropped
         display_text = json_map[mod_display_text_key]
         location = json_map[mod_location_key]
         assert location == "3'"
         idt_text = json_map.get(mod_idt_text_key)
         return Modification3Prime(display_text=display_text, idt_text=idt_text)
 
 
@@ -870,15 +871,15 @@
         ret[mod_location_key] = "internal"
         if self.allowed_bases is not None:
             ret[mod_allowed_bases_key] = NoIndent(
                 list(self.allowed_bases)) if suppress_indent else list(self.allowed_bases)
         return ret
 
     @staticmethod
-    def from_json(json_map: dict) -> ModificationInternal:
+    def from_json(json_map: dict) -> 'ModificationInternal':  # remove quotes when Python 3.6 support dropped
         display_text = json_map[mod_display_text_key]
         location = json_map[mod_location_key]
         assert location == "internal"
         idt_text = json_map.get(mod_idt_text_key)
         allowed_bases_list = json_map.get(mod_allowed_bases_key)
         allowed_bases = frozenset(allowed_bases_list) if allowed_bases_list is not None else None
         return ModificationInternal(display_text=display_text, idt_text=idt_text, allowed_bases=allowed_bases)
@@ -908,15 +909,15 @@
 
     def to_json_serializable(self, suppress_indent: bool = True):
         dct = self.__dict__
         # return NoIndent(dct) if suppress_indent else dct
         return dct
 
     @staticmethod
-    def from_json(json_map: dict) -> Position3D:
+    def from_json(json_map: dict) -> 'Position3D':  # remove quotes when Python 3.6 support dropped
         if position_origin_key in json_map:
             origin = json_map[position_origin_key]
             x = origin[position_x_key]
             y = origin[position_y_key]
             z = origin[position_z_key]
         else:
             x = json_map[position_x_key]
@@ -927,15 +928,15 @@
 
 def in_browser() -> bool:
     """Test if this code is running in the browser.
 
     Checks for existence of package "pyodide" used in pyodide. If present it is assumed the code is
     running in the browser."""
     try:
-        import pyodide
+        import pyodide  # type: ignore
         return True
     except ImportError:
         return False
 
 
 @dataclass
 class Helix(_JSONSerializable):
@@ -953,33 +954,33 @@
 
     Once part of a :any:`DNADesign`, a :any:`Helix` has an index (accessible  via :py:meth:`Helix.idx`
     once the :any:`DNADesign` is created)
     representing its order in the list of all :any:`Helix`'s. This index is how a :any:`Domain` is
     associated to the :any:`Helix` via the integer index :any:`Domain.helix`.
     """
 
-    max_offset: int = None
+    max_offset: int = None  # type: ignore
     """Maximum offset (exclusive) of :any:`Domain` that can be drawn on this :any:`Helix`. 
     If unspecified, it is calculated when the :any:`DNADesign` is instantiated as 
     the largest :any:`Domain.end` offset of any :any:`Domain` in the design.
     """
 
     min_offset: int = 0
     """Minimum offset (inclusive) of :any:`Domain` that can be drawn on this :any:`Helix`. 
     If unspecified, it is set to 0.
     """
 
     major_tick_distance: int = -1
     """If positive, overrides :any:`DNADesign.major_tick_distance`."""
 
-    major_ticks: List[int] = None
+    major_ticks: List[int] = None  # type: ignore
     """If not ``None``, overrides :any:`DNADesign.major_tick_distance` and :any:`Helix.major_tick_distance`
     to specify a list of offsets at which to put major ticks."""
 
-    grid_position: Tuple[int, int] = None
+    grid_position: Tuple[int, int] = None  # type: ignore
     """`(h,v)` position of this helix in the side view grid,
     if :const:`Grid.square`, :const:`Grid.hex` , or :const:`Grid.honeycomb` is used
     in the :any:`DNADesign` containing this helix.
     `h` and `v` are in units of "helices": incrementing `h` moves right one helix in the grid
     and incrementing `v` moves down one helix in the grid. 
     In the case of the hexagonal lattice, 
     The convention is that incrementing `v` moves down and to the right if h is even, 
@@ -992,15 +993,15 @@
     Default is `h` = 0, `v` = index of :any:`Helix` in :py:data:`DNADesign.helices`.
     
     In the case of the honeycomb lattice, we use the same convention as cadnano for encoding hex coordinates,
     see `misc/cadnano-format-specs/v2.txt`.
     That convention is different from simply excluding coordinates from the hex lattice.
     """
 
-    position: Position3D = None
+    position: Position3D = None  # type: ignore
     """Position (x,y,z) of this :any:`Helix` in 3D space.
     
     Must be None if :py:data:`Helix.grid_position` is specified."""
 
     pitch: float = 0
     """Angle in the main view plane; 0 means pointing to the right (min_offset on left, max_offset on right).
     Rotation is clockwise in the main view.
@@ -1015,15 +1016,15 @@
 
     yaw: float = 0
     """Third angle for orientation besides :py:data:`Helix.pitch` and :py:data:`Helix.roll`.
     Not visually displayed in scadnano, but here to support more general 3D applications.
     See https://en.wikipedia.org/wiki/Aircraft_principal_axes
     Units are degrees."""
 
-    idx: int = None
+    idx: int = None  # type: ignore
     """Index of this :any:`Helix`.
     
     Optional if no other :any:`Helix` specifies a value for *idx*.
     Default is the order of the :any:`Helix` is listed in constructor for :any:`DNADesign`."""
 
     # for optimization; list of domains on that Helix
     _domains: List['Domain'] = field(default_factory=list)
@@ -1089,15 +1090,15 @@
         """
         if self.major_ticks is not None:
             return self.major_ticks
         distance = default_major_tick_distance_ if self.major_tick_distance <= 0 else self.major_tick_distance
         return list(range(self.min_offset, self.max_offset + 1, distance))
 
     @staticmethod
-    def from_json(json_map: dict) -> Helix:
+    def from_json(json_map: dict) -> 'Helix':  # remove quotes when Python 3.6 support dropped
         grid_position = None
         if grid_position_key in json_map:
             gp_list = json_map[grid_position_key]
             if len(gp_list) == 3:
                 gp_list = gp_list[:2]
             if len(gp_list) != 2:
                 raise IllegalDNADesignError("list of grid_position coordinates must be length 2, "
@@ -1199,15 +1200,16 @@
     Useful for associating extra information with the :any:`Domain` that will be serialized, for example,
     for DNA sequence design. It must be an object (e.g., a dict or primitive type such as str or int) 
     that is naturally JSON serializable. (Calling ``json.dumps`` on the object should succeed without
     having to specify a custom encoder.)
     """
 
     # not serialized; for efficiency
-    _parent_strand: Strand = field(init=False, repr=False, compare=False, default=None)
+    # remove quotes when Python 3.6 support dropped
+    _parent_strand: 'Strand' = field(init=False, repr=False, compare=False, default=None)
 
     def __post_init__(self):
         self._check_start_end()
 
     def __repr__(self):
         rep = (f'Domain(helix={self.helix}'
                f', forward={self.forward}'
@@ -1217,15 +1219,15 @@
               (f', insertions={self.insertions}' if len(self.insertions) > 0 else '') + \
               ')'
         return rep
 
     def __str__(self):
         return repr(self)
 
-    def strand(self) -> Strand:
+    def strand(self) -> 'Strand':  # remove quotes when Python 3.6 support dropped
         return self._parent_strand
 
     def set_label(self, label: StrandLabel):
         """Sets label of this :any:`Domain`."""
         self.label = label
 
     def _check_start_end(self):
@@ -1420,43 +1422,49 @@
 
     # def _between_3p_and_offset(self, offset_to_test: int, offset_edge: int) -> bool:
     #     return ((self.direction == Direction.left and self.start <= offset_to_test < offset_edge) or
     #             (self.direction == Direction.forward and offset_edge < offset_to_test < self.end))
 
     # The type hint 'Domain' must be in quotes since Domain is not yet defined.
     # This is a "forward reference": https://www.python.org/dev/peps/pep-0484/#forward-references
-    def overlaps(self, other: Domain[DomainLabel]) -> bool:
+    # remove quotes when Python 3.6 support dropped
+    # def overlaps(self, other: Domain[DomainLabel]) -> bool:
+    def overlaps(self, other: 'Domain') -> bool:
         r"""Indicates if this :any:`Domain`'s set of offsets (the set
         :math:`\{x \in \mathbb{N} \mid`
         ``self.start``
         :math:`\leq x \leq`
         ``self.end``
         :math:`\}`)
         has nonempty intersection with those of `other`,
         and they appear on the same helix,
         and they point in opposite directions."""  # noqa (suppress PEP warning)
         return (self.helix == other.helix and
                 self.forward == (not other.forward) and
                 self.compute_overlap(other)[0] >= 0)
 
-    def overlaps_illegally(self, other: Domain[DomainLabel]):
+    # remove quotes when Python 3.6 support dropped
+    # def overlaps_illegally(self, other: Domain[DomainLabel]):
+    def overlaps_illegally(self, other: 'Domain'):
         r"""Indicates if this :any:`Domain`'s set of offsets (the set
         :math:`\{x \in \mathbb{N} \mid`
         ``self.start``
         :math:`\leq x \leq`
         ``self.end``
         :math:`\}`)
         has nonempty intersection with those of `other`,
         and they appear on the same helix,
         and they point in the same direction."""  # noqa (suppress PEP warning)
         return (self.helix == other.helix and
                 self.forward == other.forward and
                 self.compute_overlap(other)[0] >= 0)
 
-    def compute_overlap(self, other: Domain[DomainLabel]) -> Tuple[int, int]:
+    # remove quotes when Python 3.6 support dropped
+    # def compute_overlap(self, other: Domain[DomainLabel]) -> Tuple[int, int]:
+    def compute_overlap(self, other: 'Domain') -> Tuple[int, int]:
         """Return [left,right) offset indicating overlap between this Domain and `other`.
 
         Return ``(-1,-1)`` if they do not overlap (different helices, or non-overlapping regions
         of the same helix)."""
         overlap_start = max(self.start, other.start)
         overlap_end = min(self.end, other.end)
         if overlap_start >= overlap_end:  # overlap is empty
@@ -1531,15 +1539,16 @@
         hairpin = sc.Strand([domain_f, loop, domain_r])
     """
 
     length: int
     """Length (in DNA bases) of this Loopout."""
 
     # not serialized; for efficiency
-    _parent_strand: Strand = field(init=False, repr=False, compare=False, default=None)
+    # remove quotes when Python 3.6 support dropped
+    _parent_strand: 'Strand' = field(init=False, repr=False, compare=False, default=None)
 
     def to_json_serializable(self, suppress_indent: bool = True):
         dct = {loopout_key: self.length}
         return NoIndent(dct)
 
     def __repr__(self):
         return f'Loopout({self.length})'
@@ -1587,15 +1596,15 @@
         self_domain_idx = domains.index(self)
         # index of self's position within the DNA sequence of parent strand
         self_seq_idx_start = sum(prev_domain.dna_length()
                                  for prev_domain in domains[:self_domain_idx])
         return self_seq_idx_start
 
     @staticmethod
-    def from_json(json_map) -> Loopout:
+    def from_json(json_map) -> 'Loopout':  # remove quotes when Python 3.6 support dropped
         # XXX: this should never fail since we detect whether to call this from_json by the presence
         # of a length key in json_map
         length_str = mandatory_field(Loopout, json_map, loopout_key)
         length = int(length_str)
         return Loopout(length=length)
 
 
@@ -1688,52 +1697,55 @@
 
         design.strand(0, 0).to(10).cross(1).to(5).with_modification_5p(mod.biotin_5p).as_scaffold()
 
     :any:`StrandBuilder` should generally not be created directly or manipulated in ways other than the kind
     of method chaining described above, or else errors could result.
     """
 
-    def __init__(self, design: DNADesign, helix: int, offset: int):
+    # remove quotes when Python 3.6 support dropped
+    def __init__(self, design: 'DNADesign', helix: int, offset: int):
         self.design: DNADesign = design
         self.current_helix: int = helix
         self.current_offset: int = offset
         self.loopout_length: Optional[int] = None
         self.strand: Optional[Strand] = None
         self.just_moved_to_helix: bool = True
         self.last_domain: Optional[Domain[DomainLabel]] = None
 
-    def cross(self, helix: int, offset: int = None) -> StrandBuilder:
+    # remove quotes when Python 3.6 support dropped
+    def cross(self, helix: int, offset: int = None) -> 'StrandBuilder':
         """
         Add crossover. Must be followed by call to :py:meth:`StrandBuilder.to` to have any effect.
 
         :param helix: :any:`Helix` to crossover to
         :param offset: new offset on `helix`. If not specified, defaults to current offset.
             (i.e., a "vertical" crossover)
         :return: self
         """
         self.last_domain = None
         self.current_helix = helix
         if offset is not None:
             self.current_offset = offset
         return self
 
-    def loopout(self, helix: int, length: int, offset: int = None) -> StrandBuilder:
+    # remove quotes when Python 3.6 support dropped
+    def loopout(self, helix: int, length: int, offset: int = None) -> 'StrandBuilder':
         """
         Like :py:meth:`StrandBuilder.cross`, but creates a :any:`Loopout` instead of a crossover.
 
         :param helix: :any:`Helix` to crossover to
         :param length: length of :any:`Loopout` to add
         :param offset: new offset on `helix`. If not specified, defaults to current offset.
             (i.e., a "vertical" crossover)
         :return: self
         """
         self.loopout_length = length
         return self.cross(helix, offset)
 
-    def to(self, offset: int) -> StrandBuilder:
+    def to(self, offset: int) -> 'StrandBuilder':  # remove quotes when Python 3.6 support dropped
         """
         Extends this :any:`StrandBuilder` on the current helix to offset `offset`,
         which adds a new :any:`Domain` to the :any:`Strand` being built.
 
         This updates the underlying :any:`DNADesign` with a new :any:`Domain`,
         and if :py:meth:`StrandBuilder.loopout` was last called on this :any:`StrandBuilder`,
         also a new :any:`Loopout`.
@@ -1778,15 +1790,15 @@
             self.strand = Strand(domains=[domain])
             self.design.add_strand(self.strand)
 
         self.current_offset = offset
 
         return self
 
-    def update_to(self, offset: int) -> StrandBuilder:
+    def update_to(self, offset: int) -> 'StrandBuilder':  # remove quotes when Python 3.6 support dropped
         """
         Like :py:meth:`StrandBuilder.to`, but changes the current offset without creating
         a new :any:`Domain`. So unlike :py:meth:`StrandBuilder.to`, several consecutive calls to
         :py:meth:`StrandBuilder.update_to` are equivalent to only making the final call.
 
         If :py:meth:`StrandBuilder.cross` or :py:meth:`StrandBuilder.loopout` was just called,
         then :py:meth:`StrandBuilder.to` and :py:meth:`StrandBuilder.update_to` have the same effect.
@@ -1809,67 +1821,72 @@
         else:
             domain.set_start(offset)
 
         self.current_offset = offset
 
         return self
 
-    def as_scaffold(self) -> StrandBuilder:
+    def as_scaffold(self) -> 'StrandBuilder':  # remove quotes when Python 3.6 support dropped
         """
         Makes Strand being built a scaffold.
 
         :return: self
         """
         self.strand.set_scaffold(True)
         return self
 
-    def with_modification_5p(self, mod: Modification5Prime) -> StrandBuilder:
+    # remove quotes when Python 3.6 support dropped
+    def with_modification_5p(self, mod: Modification5Prime) -> 'StrandBuilder':
         """
         Sets Strand being built to have given 5' modification.
 
         :param mod: 5' modification
         :return: self
         """
         self.strand.set_modification_5p(mod)
         return self
 
-    def with_modification_3p(self, mod: Modification3Prime) -> StrandBuilder:
+    # remove quotes when Python 3.6 support dropped
+    def with_modification_3p(self, mod: Modification3Prime) -> 'StrandBuilder':
         """
         Sets Strand being built to have given 3' modification.
 
         :param mod: 3' modification
         :return: self
         """
         self.strand.set_modification_3p(mod)
         return self
 
+    # remove quotes when Python 3.6 support dropped
     def with_modification_internal(self, idx: int, mod: ModificationInternal,
-                                   warn_on_no_dna: bool) -> StrandBuilder:
+                                   warn_on_no_dna: bool) -> 'StrandBuilder':
         """
         Sets Strand being built to have given internal modification.
 
         :param idx: idx along DNA sequence of internal modification
         :param mod: internal modification
         :param warn_on_no_dna: whether to print warning to screen if DNA has not been assigned
         :return: self
         """
         self.strand.set_modification_internal(idx, mod, warn_on_no_dna)
         return self
 
-    def with_color(self, color: Color) -> StrandBuilder:
+    # remove quotes when Python 3.6 support dropped
+    def with_color(self, color: Color) -> 'StrandBuilder':
         """
         Sets Strand being built to have given color.
 
         :param color: color to set for Strand
         :return: self
         """
         self.strand.set_color(color)
         return self
 
-    def with_sequence(self, sequence: str, assign_complement: bool = True) -> StrandBuilder:
+    # remove quotes when Python 3.6 support dropped
+    def with_sequence(self, sequence: str, assign_complement: bool = True) -> 'StrandBuilder':
         """
         Assigns `sequence` as DNA sequence of the :any:`Strand` being built.
         This should be done after the :any:`Strand`'s structure is done being built, e.g.,
 
         .. code-block:: Python
 
             design.strand(0, 0).to(10).cross(1).to(5).with_sequence('AAAAAAAAAACGCGC')
@@ -1879,15 +1896,16 @@
             bound to this :any:`Strand`. This has the same meaning as the parameter `assign_complement` in
             :py:meth:`DNADesign.assign_dna`.
         :return: self
         """
         self.design.assign_dna(strand=self.strand, sequence=sequence, assign_complement=assign_complement)
         return self
 
-    def with_domain_sequence(self, sequence: str, assign_complement: bool = True) -> StrandBuilder:
+    # remove quotes when Python 3.6 support dropped
+    def with_domain_sequence(self, sequence: str, assign_complement: bool = True) -> 'StrandBuilder':
         """
         Assigns `sequence` as DNA sequence of the most recently created :any:`Domain` in
         the :any:`Strand` being built. This should be called immediately after a :any:`Domain` is created
         via a call to
         :py:meth:`StrandBuilder.to`,
         :py:meth:`StrandBuilder.update_to`,
         or
@@ -1907,29 +1925,31 @@
         :return: self
         """
         last_domain = self.strand.domains[-1]
         self.design.assign_dna(strand=self.strand, sequence=sequence, domain=last_domain,
                                assign_complement=assign_complement)
         return self
 
-    def with_label(self, label: StrandLabel) -> StrandBuilder:
+    # remove quotes when Python 3.6 support dropped
+    def with_label(self, label: StrandLabel) -> 'StrandBuilder':
         """
         Assigns `label` as label of the :any:`Strand` being built.
 
         .. code-block:: Python
 
             design.strand(0, 0).to(10).cross(1).to(5).with_label('scaffold')
 
         :param label: label to assign to the :any:`Strand`
         :return: self
         """
         self.strand.set_label(label)
         return self
 
-    def with_domain_label(self, label: DomainLabel) -> StrandBuilder:
+    # remove quotes when Python 3.6 support dropped
+    def with_domain_label(self, label: DomainLabel) -> 'StrandBuilder':
         """
         Assigns `label` as DNA sequence of the most recently created :any:`Domain` in
         the :any:`Strand` being built. This should be called immediately after a :any:`Domain` is created
         via a call to
         :py:meth:`StrandBuilder.to`,
         :py:meth:`StrandBuilder.update_to`,
         or
@@ -2103,15 +2123,15 @@
 
         if self.use_default_idt:
             self.set_default_idt(True)
 
         self._ensure_modifications_legal()
         self._ensure_domains_nonoverlapping()
 
-    def __eq__(self, other: Strand) -> bool:
+    def __eq__(self, other: 'Strand') -> bool:  # remove quotes when Python 3.6 support dropped
         if not isinstance(other, Strand):
             return False
         return self.domains == other.domains
 
     def __hash__(self):
         return hash(self.domains)
 
@@ -2230,24 +2250,24 @@
         """5' offset of this entire :any:`Strand`, INCLUSIVE."""
         return self.first_domain().offset_5p()
 
     def offset_3p(self) -> int:
         """3' offset of this entire :any:`Strand`, INCLUSIVE."""
         return self.last_domain().offset_3p()
 
-    def overlaps(self, other: Strand) -> bool:
+    def overlaps(self, other: 'Strand') -> bool:  # remove quotes when Python 3.6 support dropped
         """Indicates whether `self` overlaps `other_strand`, meaning that the set of offsets occupied
         by `self` has nonempty intersection with those occupied by `other_strand`."""
         for domain_self in self.bound_domains():
             for domain_other in other.bound_domains():
                 if domain_self.overlaps(domain_other):
                     return True
         return False
 
-    def assign_dna_complement_from(self, other: Strand):
+    def assign_dna_complement_from(self, other: 'Strand'):  # remove quotes when Python 3.6 support dropped
         """Assuming a DNA sequence has been assigned to `other`, assign its Watson-Crick
         complement to the portions of this Strand that are bound to `other`.
 
         Generally this is not called directly; use :py:meth:`DNADesign.assign_dna` to assign
         a DNA sequence to a :any:`Strand`. The method :py:meth:`DNADesign.assign_dna` will calculate
         which other :any:`Strand`'s need
         to be assigned via :py:meth:`Strand.assign_dna_complement_from`.
@@ -2437,15 +2457,15 @@
         If the design was legal before, it will be legal after calling that method.
         """
         self.domains.reverse()
         for domain in self.bound_domains():
             domain.forward = not domain.forward
 
     @staticmethod
-    def from_json(json_map: dict) -> Strand:
+    def from_json(json_map: dict) -> 'Strand':  # remove quotes when Python 3.6 support dropped
         domain_jsons = mandatory_field(Strand, json_map, domains_key, *legacy_domains_keys)
         if len(domain_jsons) == 0:
             raise IllegalDNADesignError(f'{domains_key} list cannot be empty')
 
         domains = []
         for domain_json in domain_jsons:
             if loopout_key in domain_json:
@@ -2755,15 +2775,15 @@
     inter_helix_gap: float = 0.5
     """Gap between helices in nanometers (due to electrostatic repulsion; needed to display to scale)."""
 
     def is_default(self):
         return self == _default_geometry
 
     @staticmethod
-    def from_json(json_map: dict) -> Geometry:
+    def from_json(json_map: dict) -> 'Geometry':  # remove quotes when Python 3.6 support dropped
         geometry = Geometry()
         geometry.rise_per_base_pair = optional_field(_default_geometry.rise_per_base_pair, json_map,
                                                      rise_per_base_pair_key, *legacy_rise_per_base_pair_keys)
         geometry.helix_radius = optional_field(_default_geometry.helix_radius, json_map, helix_radius_key)
         geometry.bases_per_turn = optional_field(_default_geometry.bases_per_turn, json_map,
                                                  bases_per_turn_key)
         geometry.minor_groove_angle = optional_field(_default_geometry.minor_groove_angle, json_map,
@@ -2892,15 +2912,15 @@
 
         if self.strands is None:
             self.strands = []
 
         if self.major_tick_distance < 0 or self.major_tick_distance is None:
             self.major_tick_distance = default_major_tick_distance(self.grid)
 
-        if (self.helices is not None and (helix_template is not None or num_helices is not None)):
+        if self.helices is not None and (helix_template is not None or num_helices is not None):
             raise IllegalDNADesignError('helices is mutually exclusive with helix_template and num_helices; '
                                         'you must specified the first, or the latter two')
 
         if (helix_template is not None and num_helices is None) or (
                 helix_template is None and num_helices is not None):
             raise IllegalDNADesignError('helix type must be specified if and only if num_helices is')
 
@@ -2945,42 +2965,43 @@
         if strand.color is None and self.automatically_assign_color:
             if strand.is_scaffold:
                 strand.color = default_scaffold_color
             else:
                 strand.color = next(self.color_cycler)
 
     @staticmethod
-    def from_scadnano_file(filename: str) -> DNADesign:
+    def from_scadnano_file(filename: str) -> 'DNADesign':  # remove quotes when Python 3.6 support dropped
         """
         Loads a :any:`DNADesign` from the file with the given name.
 
         :param filename: name of the file with the design. Should be a JSON file ending in .dna
         :return: DNADesign described in the file
         """
         with open(filename) as f:
             json_str = f.read()
         return DNADesign.from_scadnano_json_str(json_str)
 
     @staticmethod
-    def from_scadnano_json_str(json_str: str) -> DNADesign:
+    def from_scadnano_json_str(json_str: str) -> 'DNADesign':  # remove quotes when Python 3.6 support dropped
         """
         Loads a :any:`DNADesign` from the given JSON string.
 
         :param json_str: JSON description of the :any:`DNADesign`
         :return: DNADesign described in the JSON string
         """
         json_map = json.loads(json_str)
         try:
             design = DNADesign.from_scadnano_json_map(json_map)
             return design
         except KeyError as e:
             raise IllegalDNADesignError(f'I was expecting a JSON key but did not find it: {e}')
 
     @staticmethod
-    def from_scadnano_json_map(json_map: dict) -> DNADesign:
+    def from_scadnano_json_map(
+            json_map: dict) -> 'DNADesign':  # remove quotes when Python 3.6 support dropped
         """
         Loads a :any:`DNADesign` from the given JSON object (i.e., Python object obtained by calling
         json.loads(json_str) from a string representing contents of a JSON file.
 
         :param json_map: JSON map describing the :any:`DNADesign`
         :return: DNADesign described in the object
         """
@@ -3268,17 +3289,19 @@
         domains = DNADesign._cadnano_v2_import_explore_domains(vstrands, seen, strand_type,
                                                                strand_5_end_base,
                                                                strand_5_end_helix)
         strand = Strand(domains=domains, is_scaffold=(strand_type == 'scaf'), color=strand_color)
 
         return strand
 
+    # remove quotes when Python 3.6 support dropped
     @staticmethod
-    def from_cadnano_v2(directory: str = None, filename: str = None, json_dict: dict = None) -> DNADesign:
-        """ Creates a DNADesign from a cadnano v2 file.
+    def from_cadnano_v2(directory: str = None, filename: str = None, json_dict: dict = None) -> 'DNADesign':
+        """
+        Creates a DNADesign from a cadnano v2 file.
         """
 
         if json_dict is None:
             file_path = os.path.join(directory, filename)
             f = open(file_path, 'r')
             cadnano_v2_design = json.load(f)
             f.close()
@@ -4523,15 +4546,15 @@
         for helix_, forward_, offset_ in [(helix, forward, offset), (helix2, forward2, offset2)]:
             self._prepare_nicks_for_full_crossover(helix_, forward_, offset_)
         self.add_half_crossover(helix=helix, helix2=helix2, offset=offset - 1, offset2=offset2 - 1,
                                 forward=forward, forward2=forward2)
         self.add_half_crossover(helix=helix, helix2=helix2, offset=offset, offset2=offset2,
                                 forward=forward, forward2=forward2)
 
-    def add_crossovers(self, crossovers: List[Crossover]):
+    def add_crossovers(self, crossovers: List['Crossover']):  # remove quotes when Python 3.6 support dropped
         """
         Adds a list of :any:`Crossover`'s in batch.
 
         This helps to avoid problems where adding them one at a time using
         :py:meth:`DNADesign.add_half_crossover`
         or
         :py:meth:`DNADesign.add_full_crossover`
```

### Comparing `scadnano-0.9.8/scadnano.egg-info/PKG-INFO` & `scadnano-0.9.9/scadnano.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: scadnano
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python scripting library for generating designs readable by scadnano.
 Home-page: https://github.com/UC-Davis-molecular-computing/scadnano-python-package
 Author: David Doty
 Author-email: doty@ucdavis.edu
 License: MIT
-Download-URL: https://github.com/UC-Davis-molecular-computing/scadnano-python-package/archive/v0.9.8.zip
+Download-URL: https://github.com/UC-Davis-molecular-computing/scadnano-python-package/archive/v0.9.9.zip
 Description: # scadnano-python-package
         
         ![Python package](https://github.com/UC-Davis-molecular-computing/scadnano-python-package/workflows/Python%20package/badge.svg)
         [![Documentation Status](https://readthedocs.org/projects/scadnano-python-package/badge/?version=latest)](https://scadnano-python-package.readthedocs.io/en/latest/?badge=latest)
         
         The scadnano Python module is a library for describing synthetic DNA nanostructures (e.g., DNA origami).
         
         
         If you find scadnano useful in a scientific project, please cite its associated paper:
         
-        > <ins>scadnano: A browser-based, scriptable tool for designing DNA nanostructures</ins>.  
+        > scadnano: A browser-based, scriptable tool for designing DNA nanostructures.  
           David Doty, Benjamin L Lee, and Tristan Stérin.  
           DNA 2020: *Proceedings of the 26th International Conference on DNA Computing and Molecular Programming*  
           [ [paper](https://arxiv.org/abs/2005.11841) | [BibTeX](https://web.cs.ucdavis.edu/~doty/papers/scadnano.bib) ]
         
         
         ## Overview
         
@@ -42,17 +42,25 @@
         
         
         
         
         
         ## Installation
         
-        The scadnano Python package requires Python version 3.7 or later. If you do not have that version (or later) of Python installed, follow [this link](https://www.python.org/downloads/) to install it.
+        The scadnano Python package requires Python version 3.7 or later. If you do not have that version (or later) of Python installed, follow [this link](https://www.python.org/downloads/) to install it. 
         
-        Once Python is installed, there are two ways you can install the scadnano Python package:
+        If you are using Python 3.6 and do not wish to upgrade, with some effort you can install a package that give the required features.
+        The Python 3.7 module that is not present in 3.6 is the 
+        [dataclasses](https://docs.python.org/3/library/dataclasses.html) module.
+        You can install a backported library for it: 
+        [dataclasses backport](https://pypi.org/project/dataclasses/) (this library appears to require at least Python version 3.6)
+        
+        Furthermore, the [typing](https://docs.python.org/3/library/typing.html) module was present in Python 3.5, but scadnano requires at least version Python 3.6.2.
+        
+        Once Python is installed (and the dataclasses backport if you have Python version 3.6), there are two ways you can install the scadnano Python package:
         
         
         1. pip (recommended)
         
             Use [pip](https://pypi.org/project/pip/) to install the package by executing the following at the command line:
             ```console
             pip install scadnano
@@ -63,15 +71,17 @@
             see also 
             https://docs.python.org/3/installing/index.html 
             or 
             https://www.liquidweb.com/kb/install-pip-windows/.
         
         2. download
         
-            As a simple alternative (in case you run into trouble using pip), you can download and place the following files (located in the [scadnano/](https://github.com/UC-Davis-molecular-computing/scadnano-python-package/tree/master/scadnano) subfolder) in your PYTHONPATH (e.g., in the same directory as the scripts you are running). To download them, right-click on "Raw" near the top and select (in Chrome or Firefox) "Save link as...)
+            *Note:* If you are reading this on the PyPI website, the links below won't work. They are relative links intended to be read on the [GitHub README page](https://github.com/UC-Davis-molecular-computing/scadnano-python-package#readme).
+        
+            As a simple alternative (in case you run into trouble using pip), you can download and place the following files (located in the [scadnano/](scadnano) subfolder) in your PYTHONPATH (e.g., in the same directory as the scripts you are running). To download them, right-click on "Raw" near the top and select (in Chrome or Firefox) "Save link as...". 
         
             * *required*: [scadnano.py](scadnano/scadnano.py) 
             * *optional*: [modifications.py](scadnano/modifications.py); This contains some common DNA modifications such as biotin and Cy3. 
             * *optional*: [origami_rectangle.py](scadnano/origami_rectangle.py); This can help create origami rectangles, but it is not necessary to use scadnano.
             * *optional*: [_version.py](scadnano/_version.py) This ensures that the current version number is written into any `.dna` files written by the library; otherwise it may be out of date. (Which should not matter for the most part.)
             
             The scadnano package uses the Python package [xlwt](https://pypi.org/project/xlwt/) to write Excel files, so in order to call the method [`DNADesign.write_idt_plate_excel_file()`](https://scadnano-python-package.readthedocs.io/#scadnano.DNADesign.write_idt_plate_excel_file) to export an Excel file with DNA sequences, xlwt must be installed. To install, type `pip install xlwt` at the command line.
```

### Comparing `scadnano-0.9.8/setup.py` & `scadnano-0.9.9/setup.py`

 * *Files identical despite different names*

