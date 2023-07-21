# Comparing `tmp/karray-0.2.1.tar.gz` & `tmp/karray-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karray-0.2.1.tar", last modified: Tue Feb 21 10:32:59 2023, max compression
+gzip compressed data, was "karray-0.3.0.tar", last modified: Fri Jul 21 22:16:25 2023, max compression
```

## Comparing `karray-0.2.1.tar` & `karray-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cgaete   (738813943) domänen-benutzer (738800513)        0 2023-02-21 10:32:59.823840 karray-0.2.1/
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)     1069 2022-11-11 20:12:05.000000 karray-0.2.1/LICENSE
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      948 2023-02-21 10:32:59.823840 karray-0.2.1/PKG-INFO
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      108 2022-12-07 14:15:40.000000 karray-0.2.1/README.md
-drwxr-xr-x   0 cgaete   (738813943) domänen-benutzer (738800513)        0 2023-02-21 10:32:59.823840 karray-0.2.1/karray/
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      356 2023-02-21 10:27:49.000000 karray-0.2.1/karray/__init__.py
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)    53945 2023-02-21 10:15:49.000000 karray-0.2.1/karray/arrays.py
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      355 2023-02-16 20:46:04.000000 karray-0.2.1/karray/setting.py
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)     2166 2023-02-16 20:46:04.000000 karray-0.2.1/karray/utils.py
-drwxr-xr-x   0 cgaete   (738813943) domänen-benutzer (738800513)        0 2023-02-21 10:32:59.823840 karray-0.2.1/karray.egg-info/
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      948 2023-02-21 10:32:59.000000 karray-0.2.1/karray.egg-info/PKG-INFO
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      275 2023-02-21 10:32:59.000000 karray-0.2.1/karray.egg-info/SOURCES.txt
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)        1 2023-02-21 10:32:59.000000 karray-0.2.1/karray.egg-info/dependency_links.txt
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)       21 2023-02-21 10:32:59.000000 karray-0.2.1/karray.egg-info/requires.txt
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)        7 2023-02-21 10:32:59.000000 karray-0.2.1/karray.egg-info/top_level.txt
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)       38 2023-02-21 10:32:59.823840 karray-0.2.1/setup.cfg
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)     1559 2023-02-21 10:28:04.000000 karray-0.2.1/setup.py
-drwxr-xr-x   0 cgaete   (738813943) domänen-benutzer (738800513)        0 2023-02-21 10:32:59.823840 karray-0.2.1/test/
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)     3295 2023-02-08 22:23:05.000000 karray-0.2.1/test/test.py
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)     7220 2023-02-16 20:46:04.000000 karray-0.2.1/test/testlong.py
+drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 22:16:25.135443 karray-0.3.0/
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1069 2023-05-23 09:09:19.000000 karray-0.3.0/LICENSE
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      898 2023-07-21 22:16:25.135443 karray-0.3.0/PKG-INFO
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      108 2023-05-23 09:09:19.000000 karray-0.3.0/README.md
+drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 22:16:25.135443 karray-0.3.0/karray/
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      114 2023-07-21 22:14:16.000000 karray-0.3.0/karray/__init__.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    78230 2023-07-21 21:52:21.000000 karray-0.3.0/karray/arrays.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    32055 2023-07-21 21:48:54.000000 karray-0.3.0/karray/long.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      411 2023-07-21 21:48:54.000000 karray-0.3.0/karray/setting.py
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     5408 2023-07-21 21:48:54.000000 karray-0.3.0/karray/utils.py
+drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 22:16:25.135443 karray-0.3.0/karray.egg-info/
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      898 2023-07-21 22:16:25.000000 karray-0.3.0/karray.egg-info/PKG-INFO
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)      273 2023-07-21 22:16:25.000000 karray-0.3.0/karray.egg-info/SOURCES.txt
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        1 2023-07-21 22:16:25.000000 karray-0.3.0/karray.egg-info/dependency_links.txt
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        6 2023-07-21 22:16:25.000000 karray-0.3.0/karray.egg-info/requires.txt
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)        7 2023-07-21 22:16:25.000000 karray-0.3.0/karray.egg-info/top_level.txt
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)       38 2023-07-21 22:16:25.135443 karray-0.3.0/setup.cfg
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)     1472 2023-07-21 22:06:19.000000 karray-0.3.0/setup.py
+drwxrwxr-x   0 cgaete    (1000) cgaete    (1000)        0 2023-07-21 22:16:25.135443 karray-0.3.0/test/
+-rw-rw-r--   0 cgaete    (1000) cgaete    (1000)    10901 2023-07-21 21:48:54.000000 karray-0.3.0/test/test.py
```

### Comparing `karray-0.2.1/LICENSE` & `karray-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `karray-0.2.1/PKG-INFO` & `karray-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: karray
-Version: 0.2.1
+Version: 0.3.0
 Summary: Lightweight labelled multidimensional arrays with NumPy arrays under the hood.
 Author: Carlos Gaete-Morales
 Author-email: cdgaete@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karray-0.2.1/karray/arrays.py` & `karray-0.3.0/karray/arrays.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,369 +1,88 @@
-
 import numpy as np
-import pandas as pd
+try:
+    import pandas as pd
+    pandas_enabled = True
+except:
+    pandas_enabled = False
 import csv
 import json
+from functools import reduce
 from html import escape
-from typing import List, Dict, Tuple, Union
-from collections import Counter
-from .utils import _format_bytes, css, union_multi_coords
-from .setting import settings
-
-class Long:
-    def __init__(self, index:Dict[str, Union[np.ndarray, List[str], List[int], pd.DatetimeIndex]], value:Union[np.ndarray,List[float],List[int]]) -> None:
-
-        # Assertion with value
-        assert isinstance(value, (np.ndarray, list, float))
-        if isinstance(value, np.ndarray):
-            if issubclass(value.dtype.type, np.integer):
-                value = value.astype(float)
-            assert issubclass(value.dtype.type, float)
-            if value.ndim == 0:
-                value = value.reshape((value.size,))
-        elif isinstance(value, float):
-            value = np.array([value], dtype=float)
-        else:
-            value = np.array(value, dtype=float)
-        assert value.ndim == 1
-        # Assertion with index
-        assert isinstance(index, dict)
-        assert all([isinstance(index[dim], (np.ndarray,list,pd.DatetimeIndex)) for dim in index])
-        dims = list(index)
-        for dim in dims:
-            index[dim] = _test_type_and_update(index[dim])
-
-        assert all([index[dim].ndim == 1 for dim in index])
-        assert all([index[dim].size == value.size for dim in index])
-        assert 'value' not in index, "'value' can not be a dimension name as it is reserved"
-        assert all([isinstance(dim, str) for dim in index])
-
-        self._value = value
-        self._index = index
-        self._dims = list(self._index)
-
-        self.rows_display = settings.rows_display
-        self.decimals_display = settings.decimals_display
-        self.oneshot_display = settings.oneshot_display
-        self.long_nbytes = _format_bytes(sum([self._index[dim].nbytes for dim in self._index] + [self._value.nbytes]))
-
-    def __repr__(self) -> str:
-        return f'''Long
-    Object size: {self.long_nbytes}
-    Dimensions: {self.dims}
-    Rows: {self._value.size}'''
-
-    def _repr_html_(self) -> str:
-        dims = self.dims
-        items = self._value.size
-
-        if items > self.rows_display:
-            short = False
-            if self.oneshot_display:
-                rows = self.rows_display
-            else:
-                rows = int(self.rows_display/2)
-        else:
-            short = True
-            rows = items
-
-        columns = dims + ['value']
-        html = [f"{css}"]
-        html += ['<h3>[Long]</h3>',
-                '<table>',
-                f'<tr><th>Long object size</th><td>{self.long_nbytes}</td></tr>',
-                "<!-- DENSE -->",
-                f'<tr><th>Dimensions</th><td>{dims}</td></tr>',
-                '<!-- SHAPE -->',
-                f'<tr><th>Rows</th><td>{items}</td></tr>',
-                '</table>']
-        html += ["<!-- COORDS -->"]
-        html += [f"<details>"]
-        html += [f'<table><summary><div class="tooltip"> Show data <small>[default: 16 rows, 2 decimals]</small>']
-        html += [f'<!-- A --><span class="tooltiptext tooltip-top">To change default values:<br> obj.rows_display = Int val<br>obj.decimals_display = Int val<br>obj.oneshot_display = False<!-- Z -->']
-        html += ['</span></div></summary><tr><th>']
-        html += [f"<th>{j}" for j in columns]
-   
-        for i in range(rows):
-            html.append(f"<tr><th><b>{i}</b>")
-            for j,v in self.items():
-                val = v[i]
-                html.append("<td>")
-                html.append(escape(f"{val:.{self.decimals_display}f}" if issubclass(v.dtype.type, float) else f"{val}"))
-
-        if not self.oneshot_display:
-            if not short:
-                html.append("<tr><th>")
-                for _ in range(len(dims)+1):
-                    html.append("<td>...")
-                for i in range(items-rows,items,1):
-                    html.append(f"<tr><th><b>{i}</b>")
-                    for j,v in self.items():
-                        val = v[i]
-                        html.append("<td>")
-                        html.append(escape(f"{val:.{self.decimals_display}f}" if issubclass(v.dtype.type, float) else f"{val}"))
-        html.append("</table></details>")
-        return "".join(html)
-
-    @property
-    def index(self):
-        assert set(self.dims) == set(self._index.keys()), "dims names must match with index names" 
-        return {dim:self._index[dim] for dim in self.dims}
+from typing import List, Dict, Tuple, Union, Callable
 
-    @property
-    def value(self):
-        return self._value.copy()
-
-    @property
-    def dims(self):
-        return self._dims[:]
-
-    @property
-    def size(self):
-        return self.value.size
-
-    @property
-    def ndim(self):
-        return len(self.index)
-
-    def insert(self, **kwargs):
-        assert all([dim not in self.dims for dim in kwargs])
-        assert all([isinstance(kwargs[dim], (str, int, dict)) for dim in kwargs])
-        for dim in kwargs:
-            if isinstance(kwargs[dim], dict):
-                value = kwargs[dim]
-                assert len(value) == 1
-                existing_dim = next(iter(value))
-                assert isinstance(existing_dim, str)
-                assert existing_dim in self.dims
-                assert isinstance(value[existing_dim], (dict, list))
-                if isinstance(value[existing_dim], dict):
-                    old_dim_items = list(value[existing_dim])
-                    old_dim_items_set = set(old_dim_items)
-                elif isinstance(value[existing_dim], list):
-                    kwargs[dim][existing_dim][0] = _test_type_and_update(value[existing_dim][0])
-                    old_dim_items = kwargs[dim][existing_dim][0]
-                    old_dim_items_set = set(old_dim_items)
-                    kwargs[dim][existing_dim][1] = _test_type_and_update(kwargs[dim][existing_dim][1])
-                assert set(np.unique(self.index[existing_dim])).issubset(old_dim_items_set)
-                assert len(old_dim_items) == len(old_dim_items_set) # mapping has unique keys
-
-        index = {}
-        for new_dim in kwargs:
-            value = kwargs[new_dim]
-            if isinstance(value, str):
-                idxarray = np.empty(self.size, dtype=np.object_)
-                idxarray[:] = value
-            elif isinstance(value, int):
-                idxarray = np.empty(self.size, dtype=np.integer)
-                idxarray[:] = value
-            elif isinstance(value, dict):
-                existing_dim = next(iter(value))
-                if isinstance(value[existing_dim], dict):
-                    mapping_dict = value[existing_dim]
-                    existing_dim_items = self.index[existing_dim]
-                    k = np.array(list(mapping_dict)) # This must be unique
-                    v = np.array(list(mapping_dict.values())) # This not necessary unique
-                elif isinstance(value[existing_dim], list):
-                    assert isinstance(value[existing_dim][0],np.ndarray)
-                    assert isinstance(value[existing_dim][1],np.ndarray)
-                    k = value[existing_dim][0]
-                    v = value[existing_dim][1]
-                    existing_dim_items = self.index[existing_dim]
-                else:
-                    raise Exception(f"type {type(value[existing_dim])} not implemented.")
-
-                idxarray = np.array(v)[np.argsort(k)[np.searchsorted(k, existing_dim_items, sorter=np.argsort(k))]]
-            index[new_dim] = idxarray
-
-        for dim in self.index:
-            index[dim] = self.index[dim]
-
-        return Long(index=index, value=self.value)
-    
-    def rename(self, **kwargs):
-        assert all([odim in self.dims for odim in kwargs])
-        assert all([ndim not in self.dims for ndim in kwargs.values()])
-        index = {}
-        for dim in self.dims:
-            if dim in kwargs:
-                index[kwargs[dim]] = self._index[dim]
-            else:
-                index[dim] = self._index[dim]
-        return Long(index=index, value=self._value)
-
-    def drop(self, dims:Union[str,List[str]]):
-        assert isinstance(dims, (str, list))
-        index = {}
-        if isinstance(dims, str):
-            assert dims in self.dims
-            dims = [dims]
-        elif isinstance(dims, list):
-            assert all([dim in self.dims for dim in dims])
-        for dim in self.dims:
-            if dim not in dims:
-                index[dim] = self._index[dim]
-        item_tuples = list(zip(*index.values()))
-        if len(set(item_tuples)) == len(item_tuples):
-            flag = True
-        else:
-            flag=False
-            counts = Counter(item_tuples)
-            most_common = counts.most_common(1)[0][0]
-            first = item_tuples.index(most_common,0)
-            second  = item_tuples.index(most_common,first+1)
-            display_str = f"e.g.:\n  {tuple(index)} value\n{first} {item_tuples[first]} {self._value[first]}\n{second} {item_tuples[second]} {self._value[second]}"
-        assert flag, f"Index items per row must be unique. By removing {dims} leads the existence of repeated indexes \n{display_str}\nIntead, you can use obj.reduce('{dims[0]}')\nWith an aggfunc: sum() by default"
-        return Long(index=index, value=self._value)
-        
-    def items(self):
-        dc = dict(**self.index)
-        dc.update(dict(value=self._value))
-        for k,v in dc.items():
-            yield (k,v)
-
-    def __getitem__(self, item):
-        assert isinstance(item, (str, int, list, np.ndarray, slice, tuple))
-        if isinstance(item, int):
-            return Long(index={dim:self._index[dim][item] for dim in self.dims}, value=self._value[item])
-        elif isinstance(item, list):
-            item = np.array(item, dtype=np.integer)
-            return Long(index={dim:self._index[dim][item] for dim in self.dims}, value=self._value[item])
-        elif isinstance(item, np.ndarray):
-            assert issubclass(item.dtype.type, np.integer) or issubclass(item.dtype.type, np.bool_)
-            return Long(index={dim:self._index[dim][item] for dim in self.dims}, value=self._value[item])
-        elif isinstance(item, slice):
-            return Long(index={dim:self._index[dim][item] for dim in self.dims}, value=self._value[item])
-        elif isinstance(item, str):
-            assert item in self.dims
-            return self._index[item]
-        elif isinstance(item, tuple):
-            assert len(item) == 2
-            if isinstance(item[0], str):
-                dim = item[0]
-                condition = item[1]
-                assert dim in self.dims
-                assert isinstance(condition, (list, np.ndarray, slice))
-                index_items_on_dim = self._index[dim]
-                # Go over the elements of the numpy array
-                if isinstance(condition, (list,np.ndarray)):
-                    mask = np.isin(index_items_on_dim, condition)
-                    return Long(index={dim_:self._index[dim_][mask] for dim_ in self.dims}, value=self._value[mask])
-                # only works if elements of the numpy array are integers
-                elif isinstance(condition, slice):
-                    assert issubclass(index_items_on_dim.dtype.type, np.integer)
-                    start = condition.start or int(np.min(index_items_on_dim))
-                    step = condition.step or 1
-                    stop = condition.stop or int(np.max(index_items_on_dim) + step)
-                    arange_condition = np.arange(start,stop,step)
-                    mask = np.isin(index_items_on_dim, arange_condition)
-                    return Long(index={dim_:self._index[dim_][mask] for dim_ in self.dims}, value=self._value[mask])
-            # Reorder dims
-            elif isinstance(item[0], list):
-                reorder = item[0]
-                assert set(self.dims) == set(reorder)
-                assert isinstance(item[1], slice)
-                condition = item[1]
-                start = condition.start or 0
-                stop = condition.stop or self._value.size
-                step = condition.step or 1
-                arange_condition = np.arange(start,stop,step)
-                return Long(index={dim_:self._index[dim_][arange_condition] for dim_ in reorder}, value=self._value[arange_condition])
-            # TODO: Implement slice over datetime
-
-    def __eq__(self, __o: object):
-        if isinstance(__o, Long):
-            dims_equal = tuple(self.dims) == tuple(__o.dims)
-            if not dims_equal:
-                return False
-            value_equal = np.array_equal(self._value,__o._value)
-            if not value_equal:
-                return False
-            return all(np.array_equal(self._index[dim],__o._index[dim]) for dim in self.dims)
-        else:
-            if np.isnan(__o):
-                return np.isnan(self._value)
-            elif np.isinf(__o):
-                return np.isinf(self._value)
-            elif isinstance(__o, (int,float)):
-                return self._value == __o
-            elif isinstance(__o, np.generic):
-                raise Exception("np.ndarray not supported yet")
-            else:
-                raise Exception(f"{type(__o)} not supported yet")
-
-    def __ne__(self, __o: object):
-        if isinstance(__o, Long):
-            dims_equal = tuple(self.dims) == tuple(__o.dims)
-            if not dims_equal:
-                return True
-            value_equal = np.array_equal(self._value,__o._value)
-            if not value_equal:
-                return True
-            return not all(np.array_equal(self._index[dim],__o._index[dim]) for dim in self.dims)
-        else:
-            if np.isnan(__o):
-                return ~np.isnan(self._value)
-            elif np.isinf(__o):
-                return ~np.isinf(self._value)
-            elif isinstance(__o, (int,float)):
-                return self._value != __o
-            elif isinstance(__o, np.generic):
-                raise Exception("np.ndarray not supported yet")
-            else:
-                raise Exception(f"{type(__o)} not supported yet")
+from .long import Long
+from .utils import _format_bytes, css, union_multi_coords, _test_type_and_update
+from .setting import settings
 
 
 class Array:
     """
     A class for labelled multidimensional arrays.
     """
-    def __init__(self, data:Union[Tuple[dict,Union[np.ndarray,List[float]]],Long,None]=None, coords:Union[Dict[str,Union[np.ndarray,List[str],List[int],List[np.datetime64],pd.DatetimeIndex]],None]=None):
+    def __init__(self, data:Union[Tuple[dict,Union[np.ndarray,List[float],List[int],List[bool]]],Long,np.ndarray,None]=None, coords:Union[Dict[str,Union[np.ndarray,List[str],List[int],List[float],List[np.datetime64]]],None]=None):
         '''
-        Initialize a karray.
+        Initialize a karray. data can be:
+        tuple: index,value: index (dict[keys:str|int, values:list|np.ndarray[int|str|datetime64]): keys are dim names, values are 1d array of dim coordinates or list. value (np.ndarray|list): 1d array of float.
+        long: (Long) is a Long instance
+        dense: (ndarray) n-dimensional array
         
         Args:
-            data: must be a tuple of index,value or a Long object.
+            data: must be a tuple of index,value, a np.ndarray or a Long object.
             coords (dict[key:str, values:list|np.ndarray[str|int|datetime64]): dictionary with all possible coordinates.
 
-            data could be:
-            - tuple index,value: index (dict[keys:str|int, values:list|np.ndarray[int|str|datetime64]): keys are dim names, values are 1d array of dim coordinates or list.
-                                 value (np.ndarray|list): 1d array of float.
-            - long (Long) is a Long instance
-            - dense (ndarray) n-dimensional array
-
-            A rule for the order of the array dimensions> coords keys sets dims order, otherwise index sets the order of dims. Both are subject to order list if not None.
+        Attributes:
+            dims (List[str]): A list of the dimensions in the Array object.
+            coords (Dict[str, np.ndarray]): A dictionary of coordinate arrays corresponding to each dimension in the data.
+            shape (List[int]): The shape of the Array object.
+            size (int): The number of elements in the Array object.
+            capacity (int): The maximun number of elements when consider all possible combinations of the dimensions' coordinates.
+            ndim (int): The number of dimensions in the Array object.
 
         Example:
-            >>> import karray as ka
-            >>> import numpy as np
-            First example
-            >>> index = {'x':[2,5], 'y':[1,4]}
-            >>> value = [3.0,6.0]
-            >>> ar = ka.Array(data = (index, value), coords = {'x':[2,5,7], 'y':[1,4,8]}
-            Second example
-            >>> long = Long(index=index, value=value)
-            >>> ar = ka.Array(data = long, coords = {'x':[2,5,7], 'y':[1,4,8]}
-            Third example
-            >>> long_format_2darray = np.array([[2,1,3.0],[5,4,6.0]]) # First two columns are dimensions, last column is value.
-            >>> long = ka.numpy_to_long(array=long_format_2darray, dims=['x','y'])
-            >>> ar = ka.Array(data = long, coords = {'x':[2,5,7], 'y':[1,4,8]})
+
+            .. code-block:: python
+
+                >>> import karray as ka
+                >>> import numpy as np
+
+                >>> index = {'x':[2,5], 'y':[1,4]}
+                >>> value = [3.0,6.0]
+                >>> ar = ka.Array(data=(index, value), coords={'x':[2,5,7], 'y':[1,4,8]}
+
+                >>> long = Long(index=index, value=value)
+                >>> ar = ka.Array(data=long, coords={'x':[2,5,7], 'y':[1,4,8]}
+
+                >>> long_format_2darray = np.array([[2,1,3.0],[5,4,6.0]]) # First two columns are dimensions, last column is value.
+                >>> long = ka.numpy_to_long(array=long_format_2darray, dims=['x','y'])
+                >>> ar = ka.Array(data = long, coords = {'x':[2,5,7], 'y':[1,4,8]})
 
         '''
         self.__dict__["_repo"] = {}
         self.long = None
         self.coords = None
         self.dense = None
         self.keep_zeros = settings.keep_zeros
         self.sort_coords = settings.sort_coords
         self.fill_missing = settings.fill_missing
         self.attr_constructor(**self.check_input(data, coords))
         return None
 
     def check_input(self, data, coords:dict):
+        """
+        Checks the input and returns corrected values
+            
+        Args:
+            data (Long, tuple, np.ndarray, type(None)): input data to be checked
+            coords: coordinates of the data in an array
+
+        Returns: Dictionary containing corrected values:
+            dense, long, index, value, coords
+
+        """
         assert isinstance(data, (Long, tuple, np.ndarray, type(None)))
         if isinstance(data, Long):
             long:Union[Long,None] = data
             index:Union[dict,None] = None
             value:Union[np.ndarray,None] = None
             dense:Union[np.ndarray,None] = None
         elif isinstance(data, tuple):
@@ -382,15 +101,15 @@
             index:Union[dict,None] = None
             value:Union[np.ndarray,None] = None
             dense:Union[np.ndarray,None] = None
             assert coords is not None
         # TODO: Add here the assertions indicated below.
         if coords is not None:
             assert isinstance(coords, dict)
-            assert all([isinstance(coords[dim], (np.ndarray,list)) for dim in coords])
+            assert all([isinstance(coords[dim], (np.ndarray, list)) for dim in coords])
             cdims = list(coords)
             for dim in cdims:
                 assert isinstance(dim, str)
                 coords[dim] = _test_type_and_update(coords[dim])
                 assert coords[dim].ndim == 1
                 assert coords[dim].size == np.unique(coords[dim]).size, f"coords elements of dim '{dim}' must be unique. {coords[dim].size=}, {np.unique(coords[dim]).size=}"
             if long is not None:
@@ -401,18 +120,34 @@
                 assert all([set(np.unique(index[dim])).issubset(coords[dim]) for dim in coords])
             elif dense is not None:
                 assert dense.ndim == len(coords)
                 assert dense.shape == tuple(self._shape(coords))
                 assert dense.size == self._capacity(coords)
         if isinstance(data, tuple):
             assert isinstance(index, dict)
-            assert all([isinstance(index[dim], (np.ndarray,list, pd.DatetimeIndex)) for dim in index])
+            if pandas_enabled:
+                assert all([isinstance(index[dim], (np.ndarray, list, pd.DatetimeIndex)) for dim in index])
+            else:
+                assert all([isinstance(index[dim], (np.ndarray, list)) for dim in index])
         return dict(dense=dense, long=long, index=index, value=value, coords=coords)
 
     def attr_constructor(self, dense, long, index, value, coords):
+        """
+        Construct a new object from one or more input parameters.
+
+            Parameters:
+            dense (np.ndarray or None, optional): A dense array representing the data
+            long (Long or None, optional): A Long object representing the data.
+            index (dict or None, optional): A dictionary representing the index of the data 
+            value (np.ndarray or None, optional): An array representing the values of the data. 
+            coords (dict or None, optional): A dictionary representing the coordinates of the data.
+
+            Returns: None
+        """
+
         # Check input has several assertions, compare and modify accordingly
         # TODO: Noticed that coords dims could be str or int, while index in Long class can only be str. We must fix everywhere that coords keys -> dimension can only be str!
         if long is not None:
             if coords is not None: # TODO: Assertion: set(coords.keys()) == set(long.dims). Assertion long.index arrays are subset of coords values
                 if len(coords) == 0:
                     assert long.ndim == 0
                     self.coords = self._reorder_coords(coords, settings.order, self.sort_coords)
@@ -446,14 +181,16 @@
                 if self.sort_coords:
                     self.coords = self._reorder_coords(coords, settings.order, self.sort_coords)
                     long = self._dense_to_long(dense, coords)
                     self.dense = self._dense(long, self.coords)
                     self.long = self._reorder_long(long, list(self.coords), self.keep_zeros)
                 else:
                     self.coords = coords
+                    if issubclass(dense.dtype.type, np.int64):
+                        dense = dense.astype(float)
                     self.dense = dense
             else:
                 self.coords = self._reorder_coords(coords, settings.order, self.sort_coords)
                 long = self._dense_to_long(dense, coords)
                 self.dense = self._dense(long, self.coords)
                 self.long = self._reorder_long(long, list(self.coords), self.keep_zeros)
         else:
@@ -469,54 +206,104 @@
                     long = Long(index={dim: np.array([], dtype=dtypes[dim]) for dim in self.coords}, value= np.array([], dtype=float))
                     self.long = long
             else:
                 raise Exception("If 'value' is not None, then 'index' must be provided. Currently 'index' is None")
         return None
 
     def __repr__(self):
+        """
+        Returns a string representation of the object that can be used to recreate the object.
+
+        Returns:
+             String representation of the object that can be used to recreate the object in the format Karray.Array(data, coords)
+        
+        """
         return f"Karray.Array(data, coords)"
 
     def _repr_html_(self):
         html = ['<details><table><summary><div class="tooltip"> Show unique coords</div></summary>']
         html.append("<tr><th>Dimension<th>Length<th>Type<th>Items")
         for dim in self.coords:
             html.append(f"<tr><th><b>{dim}</b><td>")
             html.append(escape(f"{len(self.coords[dim])}"))
-            html.append(f"<td>{self.coords[dim].dtype}<td>")
-            html.append(f'<details><summary><div class="tooltip">show details</div></summary>')
+            html.append("<td>")
+            html.append(escape(f"{self.coords[dim].dtype}"))
+            html.append("<td>")
+            html.append('<details>')
+            html.append('<summary><div class="tooltip">show details</div></summary>')
             html.append(escape(f"{self.coords[dim]}"))
+            html.append("</details>")
         html.append("</table></details>")
         dense_size = f"<tr><th>Dense object size</th><td>{_format_bytes(self.dense.nbytes)}</td></tr>"
         script = ''.join(html)
         shape = f"<tr><th>Shape</th><td>{self.shape}</td></tr>"
         
         return self.long._repr_html_().replace('[Long]','[k]array') \
                                       .replace('<!-- DENSE -->', dense_size) \
                                       .replace('<!-- COORDS -->',script) \
                                       .replace('<!-- SHAPE -->',shape) \
                                       .replace('<!-- A -->','<!-- ') \
                                       .replace('<!-- Z -->',' -->')
 
     def _reorder_coords(self, coords, order_preference, sort_coords):
+        """
+        reorders the dimensions of the coordinates according to a given order preference and sorts them if requested
+        
+        Args:
+            coords: a dictionary with the coordinates of the array. The keys are the names of the dimensions, and the values are the coordinate arrays.
+            order_preference: a list with the preferred order of the dimensions. The first dimensions in the list have higher priority than the last ones.
+            sort_coords: a boolean indicating whether to sort the coordinate arrays or not.
+        
+        Returns:
+            Dictionary with the reordered and optionally sorted coordinates of the array
+
+        """
         order = self._order_with_preference(list(coords), order_preference)
         if sort_coords:
             coords_ = {dim:np.sort(coords[dim]) for dim in order}
         else:
             coords_ = {dim:coords[dim] for dim in order}
         return coords_
 
     def _reorder_long(self, long, order, keep_zeros):
+        """
+        Reorders long objects
+
+        Args:
+            long: Long object to be reordered
+            order: a list of dimensions specifying order of the dimensions
+             keep_zeros: boolean indicating whether zerovalues should be kept
+
+        """
         long = long[order,:]
         # print(f"{keep_zeros=}")
         return long if keep_zeros else long[long != 0.0]
 
     def __setattr__(self, name, value):
+        """
+        sets the name attribute for a value
+
+        Args:
+            name (str): name of the attribute to be set
+            value (Any): value to be assigned to the attribute
+
+        """
         self._repo[name] = value
 
     def __getattr__(self, name):
+        """
+        Retrieve the attribute value for the given name
+
+        Args:
+            name: name of the attribute
+
+        Returns:
+            xx
+
+        """
         if name.startswith('_'):
             raise AttributeError(name) # ipython requirement for repr_html
         elif name == 'long':
             if name in self._repo:
                 if self._repo[name] is None:
                     assert self.dense is not None
                     self._repo[name] = self._dense_to_long(self.dense, self.coords)
@@ -539,86 +326,268 @@
                 assert self.long is not None
                 self._repo[name] = self._dense(self.long, self.coords)
                 return self._repo[name]
         else:
             return self._repo[name]
 
     def _shape(self, coords):
+        """
+        shape of the Karray object
+   
+        Args:
+            coords (dict): dictionary of coordinates
+
+        Returns:
+            list: A list of integers representing the shape of the Karray objec
+
+        """
         return [coords[dim].size for dim in coords]
 
     @property
     def shape(self):
+        """
+        Returns the shape of the array as a tuple
+
+        Returns:
+            Tuple of integers representing the shape of each dimension of the array
+
+        """
         return self._shape(self.coords)
 
     def _capacity(self, coords):
+        """
+        maximum number of values a karray object can hold
+
+        Args:
+            coords (dict): dictionary that shows dimension names to arrays of coordinates.
+
+        Returns:
+            int: max number of elements the Karray object can hold
+            
+        """
         return int(np.prod(self._shape(coords)))
 
     @property
     def capacity(self):
+        """
+        Returns the maximum number of elements that can be stored in the array.
+
+        Returns:
+            int: The maximum number of elements that can be stored in the array.
+
+        """
         return self._capacity(self.coords)
 
     @property
     def dims(self):
+        """
+        list of the dimensions
+            
+        Returns:
+            list of dimensions of the karray object.
+
+        """
         return list(self.coords)
 
     @property
     def dindex(self):
+        """
+        returns the dense index of the array.
+
+        Returns:
+            index: A dictionary that represents the dense index of the array.
+
+        """
         arrays = np.unravel_index(np.arange(self._capacity(self.coords)), self._shape(self.coords))
         index = {dim:self.coords[dim][idx] for dim, idx in zip(self.coords, arrays)}
         return index
+    
+    @staticmethod
+    def _filler_and_dtype(long, fill_missing):
+        if issubclass(long.value.dtype.type, float):
+            dtype = long.value.dtype
+            if np.isnan(fill_missing) or np.isinf(fill_missing):
+                filler = fill_missing
+            elif isinstance(fill_missing, float):
+                filler = fill_missing
+            elif isinstance(fill_missing, (int, bool)):
+                filler = float(fill_missing)
+            else:
+                raise TypeError("fill_missing must be a float, int or bool")
+        elif issubclass(long.value.dtype.type, (np.int16, np.int32, np.int64)):
+            dtype = long.value.dtype
+            if np.isnan(fill_missing) or np.isinf(fill_missing):
+                filler = fill_missing
+                dtype = float
+                # TODO: logging int converted to float
+            elif isinstance(fill_missing, float):
+                filler = fill_missing
+                dtype = float
+                # TODO: logging int converted to float
+            elif isinstance(fill_missing, int):
+                filler = fill_missing
+            elif isinstance(fill_missing, bool):
+                if fill_missing == True:
+                    filler = 1
+                else:
+                    filler = 0
+            else:
+                raise TypeError("fill_missing must be a float, int or bool")
+        elif issubclass(long.value.dtype.type, np.bool_):
+            dtype = long.value.dtype
+            if np.isnan(fill_missing) or np.isinf(fill_missing):
+                filler = fill_missing
+                dtype = float
+                # TODO: logging bool converted to float
+            elif isinstance(fill_missing, float):
+                if fill_missing == 0.0:
+                    filler = False
+                elif fill_missing == 1.0:
+                    filler = True
+                else:
+                    filler = fill_missing
+                    dtype = float
+                    # TODO: logging bool converted to float
+            elif isinstance(fill_missing, int):
+                if fill_missing == 0:
+                    filler = False
+                elif fill_missing == 1:
+                    filler = True
+                else:
+                    filler = float(fill_missing)
+                    dtype = float
+                    # TODO: logging bool converted to float
+            elif isinstance(fill_missing, bool):
+                filler = fill_missing
+            else:
+                raise TypeError("fill_missing must be a float, int or bool")
+        else:
+            raise TypeError("fill_missing must be a float, int or bool")
+        return filler, dtype
 
     def _dense(self, long, coords):
+        """
+        returns a dense array, that helps improve storage and latency times
+                    
+        Args:
+            long (Long): long array with coordinates and values
+            coords (list): coordinates of the n-dimensional array
+
+        Returns:
+            nd_dense (ndarray): A long array formatted to a dense array.
+
+        """
         if len(coords) == 0:
             return long.value
         long_stack = np.vstack([np.argsort(coords[dim])[np.searchsorted(coords[dim], long._index[dim], sorter=np.argsort(coords[dim]))] for dim in coords])
         shape = self._shape(coords)
         indexes = np.ravel_multi_index(long_stack, shape)
         capacity = self._capacity(coords)
-        flatten_dense = np.zeros((capacity,), dtype=float)
-        flatten_dense[:] = self.fill_missing
-        flatten_dense[indexes] = long.value
+        filler, dtype = self._filler_and_dtype(long, self.fill_missing)
+        flatten_dense = np.empty((capacity,), dtype=dtype)
+        flatten_dense[:] = filler
+        flatten_dense[indexes] = long.value.astype(dtype)
         nd_dense = flatten_dense.view().reshape(shape)
         return nd_dense
 
     def _dense_to_long(self, dense, coords):
+        """
+        converts a dense array to a long array
+                    
+        Args:
+            dense (ndarray): Dense array to convert to a long array
+            coords (dict): coordinates that describe the shape of the dense array
+
+        Returns:
+            long object with the same data as provided in the dense array.
+
+        """
+        if issubclass(dense.dtype.type, np.int64):
+            dense = dense.astype(float)
         if len(coords) == 0 and dense.ndim == 1:
             return Long(index={}, value=dense)
         arrays = np.unravel_index(np.arange(self._capacity(coords)), self._shape(coords))
         index = {dim:coords[dim][idx] for dim, idx in zip(coords, arrays)}
         long = Long(index=index, value=dense.reshape(dense.size))
         return self._reorder_long(long, list(coords), self.keep_zeros)
 
     @staticmethod
     def _reorder(self_long, self_coords, reorder=None):
+        """
+        Reorders the dimensions of a Long object and returns a dictionary with the reordered data and coordinates
+
+        Args:
+            self_long (Long): The Long object to be reordered.
+            self_coords: A dictionary with the coordinates of the original Long object.
+            reorder (boolean): if a reorder should be provided
+
+        Returns:
+            A dictionary with the reordered data (Long object and coordinates).
+
+        """
         assert reorder is not None, "order must be provided"
         assert set(reorder) == set(self_long.dims), "order must be equal to self.dims, the order can be different, though"
         if tuple(self_long.dims) == tuple(reorder):
             return dict(data=self_long, coords=self_coords)
         coords = {k:self_coords[k] for k in reorder}
         long = self_long[reorder,:]
         return dict(data=long, coords=coords)
 
     def reorder(self, reorder=None):
+        """
+        Returns a new Array with dimensions ordered according to the provided `reorder` list
+
+        Args:
+            reorder (List[str]): A list with the new order of the dimensions.
+
+        Returns:
+            Array: A new Array object with the same data as the original, but with dimensions ordered according to the provided `reorder` list.
+
+        """
         return Array(**self._reorder(self.long, self.coords, reorder))
 
     @staticmethod
     def _order_with_preference(dims:list, preferred_order:list=None):
+        """
+        Returns a new list of dimensions that is ordered based on the preferred order. If preferred_order is None, the method simply returns the original dims list.
+                    
+        Args:
+            dims (list): A list of dimensions that needs to be ordered
+            preferred_order (list): A preferred order of dimensions
+
+        Returns:
+            ordered (list): A new list of dimensions that is ordered based on the preferred order
+        
+        """
         if preferred_order is None:
             return dims
         else:
             ordered = []
             disordered = dims[:]
             for dim in preferred_order:
                 if dim in disordered:
                     ordered.append(dim)
                     disordered.remove(dim)
             ordered.extend(disordered)
             return ordered
 
     def _union_dims(self, other, preferred_order: list = None):
+        """
+        Returns the union of the dimensions of two Array objects
+        If the two arrays have the same dimensions, the dimensions are returned in the same order.
+        If one of the arrays has no dimensions, the dimensions of the other array are returned.
+        
+        Args:
+            other (Array): The second array
+            preferred_order (list): A list of dimension names in the desired order.
+
+        Returns:
+            list of dimension names.
+
+        """
         if set(self.dims) == set(other.dims):
             return self._order_with_preference(self.dims, preferred_order)
         elif len(self.dims) == 0 or len(other.dims) == 0:
             for obj in [self,other]:
                 if len(obj.dims) > 0:
                     dims = obj.dims
             return self._order_with_preference(dims, preferred_order)
@@ -644,14 +613,29 @@
                 for dim in ordered_common:
                     if dim in semi_ordered:
                         semi_ordered.remove(dim)
                 ordered =  ordered_common + semi_ordered
                 return ordered
 
     def _union_coords(self, other, uniondims):
+        """
+        Returns a dictionary containing the union of the coordinate values.
+      
+        Args:
+            other: Array object to be compared
+            uniondims: list of dimension names for which the union of the coordinate values will be provided
+
+        Returns:
+
+            tuple with three values:
+            boolean value checking if all coords from self have been used
+            boolean value checking if all coords from other have been used
+            dictionary of coords
+
+        """
         coords = {}
         self_coords_bool = []
         other_coords_bool = []
         for dim in uniondims:
             if dim in self.coords:
                 if dim in other.coords:
                     if self.coords[dim].size == other.coords[dim].size:
@@ -696,150 +680,628 @@
             else:
                 raise Exception(f"Dimension {dim} not found in either arrays")
         self_coords_bool_ = all(self_coords_bool)
         other_coords_bool_ = all(other_coords_bool)
         return (self_coords_bool_, other_coords_bool_, coords)
 
     def _get_inv_dense(self, uniondims, unioncoords, coords_bool):
+        """
+        Returns a dense array with the dimensions transposed and with data filled in from the provided unioncoords
+       
+        Args:
+            uniondims (list): List of dimension names for which the union of the coordinate values is provided
+            unioncoords (dict): Dictionary containing the union of the coordinate values
+            coords_bool (bool): Boolean indicating whether the coordinate values have already been unionized
+        
+        Returns:
+            A dense array with dimensions transposed and data filled in from the provided unioncoords
+        
+        """
         self_dims = [d for d in uniondims if d in self.dims]
         if coords_bool:
             if tuple(self.dims) == tuple(self_dims):
                 self_inv_dense = self.dense.T
                 return self_inv_dense
         self_coords = {d:unioncoords[d] for d in self_dims}
         self_inv_dense = self._dense(self.long, self_coords).T
         return self_inv_dense
 
     def _pre_operation_with_array(self, other):
+        """
+        calculates the union dimensions between the two arrays, and then gets the inverse dense representation of both arrays based on these union dimensions
+         
+        Args:
+            other (array): used to calculate the inverse dense representation
+
+        Returns:
+            self_inv_dense (array): transposed dense array of self
+            other_inv_dense (array): transposed dense array of other
+            unioncoords (dict): dictionary containing the union of the coordinate values for the union dimensions
+        
+        """
+
         uniondims = self._union_dims(other, preferred_order=settings.order)
         self_coords_bool, other_coords_bool, unioncoords = self._union_coords(other, uniondims)
         self_inv_dense = self._get_inv_dense(uniondims, unioncoords, self_coords_bool)
         other_inv_dense = other._get_inv_dense(uniondims, unioncoords, other_coords_bool)
         return self_inv_dense, other_inv_dense, unioncoords
 
     def _pre_operation_with_number(self):
+        """
+        returns the transpose of the instance's `dense` attribute.
+
+        Returns:
+            numpy.ndarray: The transpose of the instance's `dense` attribute
+
+        """
         return self.dense.T
 
     def _post_operation(self, resulting_dense, coords):
+        """
+        returns an Array object from a handed in dense array
+          
+        Args:
+            resulting_dense (array): dense array
+            coords: coords for the dimensions of the object
+
+        Returns:
+            New Array resulting from the handed in objects
+
+        """
         if len(coords) == 0:
             return Array(data=({},resulting_dense), coords=coords)
         return Array(data=resulting_dense.T, coords=coords)
 
     def __add__(self, other):
+        """
+        Return the sum of this array with `other`
+
+        Args:
+            other: array object.
+
+        Returns:
+            A new array object representing the sum of this array and other
+        """
         if isinstance(other, (int, float)):
             self_dense = self._pre_operation_with_number()
             resulting_dense = self_dense + other
             return self._post_operation(resulting_dense, self.coords)
         elif isinstance(other, Array):
             self_dense, other_dense, coords = self._pre_operation_with_array(other)
             resulting_dense = self_dense + other_dense
             return self._post_operation(resulting_dense, coords)
 
     def __mul__(self, other):
+        """
+        multiplies two arrays.
+                    
+        Args:
+            other (Array): object to be multiplied
+
+        Returns:
+            a new object showing the product of the objects
+        
+        """
         if isinstance(other, (int, float)):
             self_dense = self._pre_operation_with_number()
             resulting_dense = self_dense * other
             return self._post_operation(resulting_dense, self.coords)
         elif isinstance(other, Array):
             self_dense, other_dense, coords = self._pre_operation_with_array(other)
             resulting_dense = self_dense * other_dense
             return self._post_operation(resulting_dense, coords)
 
     def __sub__(self, other):
+        """
+        substracts two arrays.
+                    
+        Args:
+            other (Array): object to be substracted.
+
+        Returns:
+            a new object showing the difference of the objects.
+
+        """
         if isinstance(other, (int, float)):
             self_dense = self._pre_operation_with_number()
             resulting_dense = self_dense - other
             return self._post_operation(resulting_dense, self.coords)
         elif isinstance(other, Array):
             self_dense, other_dense, coords = self._pre_operation_with_array(other)
             resulting_dense = self_dense - other_dense
             return self._post_operation(resulting_dense, coords)
 
     def __truediv__(self, other):
+        """
+        divides two arrays
+                    
+        Args:
+            other (Array): divisor
+
+        Returns:
+            a new object showing the quotient of the objects
+
+        """
         if isinstance(other, (int, float)):
             self_dense = self._pre_operation_with_number()
             resulting_dense = self_dense / other
             return self._post_operation(resulting_dense, self.coords)
         elif isinstance(other, Array):
             self_dense, other_dense, coords = self._pre_operation_with_array(other)
             resulting_dense = self_dense/other_dense
             return self._post_operation(resulting_dense, coords)
 
     def __radd__(self, other):
+        """
+            divides two arrays with reversed operands.
+       
+            Args:
+                other (Array): divisor
+
+            Returns:
+                a new object showing the quotient of the objects
+
+            """
         if isinstance(other, (int, float)):
             self_dense = self._pre_operation_with_number()
             resulting_dense = other + self_dense
             return self._post_operation(resulting_dense, self.coords)
 
     def __rmul__(self, other):
+        """
+        multiplies two arrays with reversed operands.
+         
+        Args:
+            other (Array): object to be multiplied.
+
+        Returns:
+            a new object showing the product of the objects
+
+        """
         if isinstance(other, (int, float)):
             self_dense = self._pre_operation_with_number()
             resulting_dense = other * self_dense
             return self._post_operation(resulting_dense, self.coords)
 
     def __rsub__(self, other):
+        """
+        substracts two arrays with reversed operands.
+                    
+        Args:
+            other (Array): object to be substracted.
+
+        Returns:
+            a new object showing the difference of the objects.
+
+        """
         if isinstance(other, (int, float)):
             self_dense = self._pre_operation_with_number()
             resulting_dense = other - self_dense
             return self._post_operation(resulting_dense, self.coords)
 
     def __rtruediv__(self, other):
+        """
+        divides two arrays with reversed operands.
+                    
+        Args:
+            other (Array): divisor
+
+        Returns:
+            a new object showing the quotient of the objects
+
+        """
         if isinstance(other, (int, float)):
             self_dense = self._pre_operation_with_number()
             resulting_dense = other / self_dense
             return self._post_operation(resulting_dense, self.coords)
 
     def __neg__(self):
+        """
+        transforms the array into negative values.
+                    
+        Returns:
+            a new object showing a dense array with negative values
+
+        """
         self_dense = self._pre_operation_with_number()
         resulting_dense = -self_dense
         return self._post_operation(resulting_dense, self.coords)
 
     def __pos__(self):
+        """
+        transforms the array into positive values.
+                    
+        Returns:
+            a new object showing a dense array with positive values
+
+        """
         self_dense = self._pre_operation_with_number()
         resulting_dense = +self_dense
         return self._post_operation(resulting_dense, self.coords)
+    
+    def __eq__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (Array): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+            
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = self_dense == other
+            return self._post_operation(resulting_dense, self.coords)
+        elif isinstance(other, Array):
+            self_dense, other_dense, coords = self._pre_operation_with_array(other)
+            resulting_dense = self_dense == other_dense
+            return self._post_operation(resulting_dense, coords)     
+        
+    def __ne__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (Array): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = self_dense != other
+            return self._post_operation(resulting_dense, self.coords)
+        elif isinstance(other, Array):
+            self_dense, other_dense, coords = self._pre_operation_with_array(other)
+            resulting_dense = self_dense != other_dense
+            return self._post_operation(resulting_dense, coords)
+        
+    def __lt__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (Array): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = self_dense < other
+            return self._post_operation(resulting_dense, self.coords)
+        elif isinstance(other, Array):
+            self_dense, other_dense, coords = self._pre_operation_with_array(other)
+            resulting_dense = self_dense < other_dense
+            return self._post_operation(resulting_dense, coords)
+        
+    def __rlt__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (int, float): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = other < self_dense
+            return self._post_operation(resulting_dense, self.coords)
+        
+    def __le__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (Array): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = self_dense <= other
+            return self._post_operation(resulting_dense, self.coords)
+        elif isinstance(other, Array):
+            self_dense, other_dense, coords = self._pre_operation_with_array(other)
+            resulting_dense = self_dense <= other_dense
+            return self._post_operation(resulting_dense, coords)
+        
+    def __rle__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (int,float): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects  
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = other <= self_dense
+            return self._post_operation(resulting_dense, self.coords)
+        
+    def __gt__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (Array): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = self_dense > other
+            return self._post_operation(resulting_dense, self.coords)
+        elif isinstance(other, Array):
+            self_dense, other_dense, coords = self._pre_operation_with_array(other)
+            resulting_dense = self_dense > other_dense
+            return self._post_operation(resulting_dense, coords)
+    def __rgt__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (int,float): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = other > self_dense
+            return self._post_operation(resulting_dense, self.coords)
+        
+    def __ge__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (Array): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = self_dense >= other
+            return self._post_operation(resulting_dense, self.coords)
+        elif isinstance(other, Array):
+            self_dense, other_dense, coords = self._pre_operation_with_array(other)
+            resulting_dense = self_dense >= other_dense
+            return self._post_operation(resulting_dense, coords)
+        
+    def __rge__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (int,float): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = other >= self_dense
+            return self._post_operation(resulting_dense, self.coords)
+        
+    def __and__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (Array): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, bool):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = self_dense & other
+            return self._post_operation(resulting_dense, self.coords)
+        elif isinstance(other, Array):
+            self_dense, other_dense, coords = self._pre_operation_with_array(other)
+            resulting_dense = self_dense & other_dense
+            return self._post_operation(resulting_dense, coords)
+        
+    def __rand__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (bool): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """ 
+        if isinstance(other, bool):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = other & self_dense
+            return self._post_operation(resulting_dense, self.coords)
+        
+    def __or__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (Array): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+
+        """
+        if isinstance(other, (int, float)):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = self_dense | other
+            return self._post_operation(resulting_dense, self.coords)
+        elif isinstance(other, Array):
+            self_dense, other_dense, coords = self._pre_operation_with_array(other)
+            resulting_dense = self_dense | other_dense
+            return self._post_operation(resulting_dense, coords)
+        
+    def __ror__(self, other):
+        """
+        compares two arrays.
+                    
+        Args:
+            other (bool): object to be compared.
+
+        Returns:
+            a new object showing the comparison of the objects
+        """
+        if isinstance(other, bool):
+            self_dense = self._pre_operation_with_number()
+            resulting_dense = other | self_dense
+            return self._post_operation(resulting_dense, self.coords)
+        
+    def __invert__(self):
+        """
+        Inverts the values of the Array object. Using the ~ operator.
+        """
+        self_dense = self._pre_operation_with_number()
+        return self._post_operation(resulting_dense= ~self_dense, coords=self.coords)
+        
+    def __bool__(self):
+        """
+        Raises an error as Array object can not be evaluated as a boolean
+        """
+        raise ValueError("The truth value of an array with more than one element is ambiguous. Use Array.any() or Array.all()")
+
+    def any(self):
+        """
+        compares two arrays.
+                    
+        Returns:
+            a new object showing the comparison of the objects
+        """
+        return self.dense.any()
+    
+    def all(self):
+        """
+        compares two arrays.
+                    
+        Returns:
+            a new object showing the comparison of the objects
+        """
+        return self.dense.all()
 
     def items(self):
+        """
+        iterates over the attributes of the Array object.
+
+        Returns:
+            returns an iterator that yields the index and value attributes of the Array object as key-value pairs.
+        
+        """
         dc = dict(**self.dindex)
         dc.update(dict(value=self.dense.reshape(-1)))
         for k,v in dc.items():
             yield (k,v)
 
     def to_pandas(self):
+        """
+        transforms the Array object into a pandas dataframe.
+
+        Returns:
+            returns an pandas dataframe object
+
+        """
+        if pandas_enabled:
+            pass
+        else:
+            raise Exception("pandas not installed. Install with `pip install pandas`")
         return pd.DataFrame(dict(self.items()))
 
     def to_polars(self):
+        """
+        transforms the Array object into a polars dataframe object.
+
+        Returns: 
+            returns an polars dataframe object.
+
+        """
         import polars as pl
         return pl.from_dict(dict(self.items()))
 
-    def to_dataframe(self, with_:str=None):
+    def to_dataframe(self, with_:str='pandas'):
+        """
+        transforms the Array object into a dataframe object
+
+        Returns: 
+            returns an dataframe object
+
+        """
         assert with_ in ['pandas','polars']
         if with_ == "pandas":
             return self.to_pandas()
         elif with_ == "polars":
             return self.to_polars()
 
     def to_arrow(self):
+        """
+        adds an arrow to the axes.
+
+        Returns: 
+            a pandas table
+
+        """
         import pyarrow as pa
-        table = pa.Table.from_pandas(pd.DataFrame({k:v for k,v in self.long.items()}))
+        table = pa.Table.from_pandas(self.long.to_pandas())
         existing_meta = table.schema.metadata
         custom_meta_key = 'karray'
         custom_metadata = {'coords':{dim:self.coords[dim].tolist() for dim in self.coords}}
         custom_meta_json = json.dumps(custom_metadata)
         existing_meta = table.schema.metadata
         combined_meta = {custom_meta_key.encode() : custom_meta_json.encode(),**existing_meta}
         return table.replace_schema_metadata(combined_meta)
 
     def to_feather(self, path):
+        """
+        writes a dataframe to the binary Feather format.
+
+        """
         import pyarrow.feather as ft
         table = self.to_arrow()
         ft.write_feather(table, path)
         return None
 
     def shrink(self, **kwargs):
+        """
+        shrinks the array according to the provided values
+
+        Returns:
+            New Array of Long and the newly assigned coords
+
+        Raises:
+            Assertion Error
+
+        Example:
+
+            .. code-block:: python
+
+        """
         #TODO: Assertion that all elements of a list must be same type. Options are: str or int
         assert all([kw in self.coords for kw in kwargs]), "Selected dimension must be in coords"
         assert all([isinstance(kwargs[dim], (list, np.ndarray)) for dim in kwargs]), "Keeping elements must be contained in lists or np.ndarray"
         assert all([set(kwargs[kw]).issubset(self.coords[kw]) for kw in kwargs]), "All keeping elements must be included of coords"
         assert all([len(set(kwargs[kw])) == len(kwargs[kw]) for kw in kwargs]), "Keeping elements in list must be unique"
         # removing elements from coords dictionary
         new_coords = {}
@@ -851,47 +1313,160 @@
         long = self.long
         for dim in self.dims:
             if dim in kwargs:
                 long = long[dim, kwargs[dim]]
         return Array(data=long, coords=new_coords)
 
     def add_elem(self, **kwargs):
+        """
+        adds an element to the array
+        Example:
+
+            .. code-block:: python
+        Returns:
+            New updated Array object of Long and the coords
+        Raises:
+            Assertion Error
+        """
         for dim in kwargs:
             assert dim in self.dims, f'dim: {dim} must exist in self.dims: {self.dims}'
-        assert all([isinstance(kwargs[dim], (list, np.ndarray,pd.DatetimeIndex)) for dim in kwargs]), "Keeping elements must be contained in lists or np.ndarray"
+        if pandas_enabled:
+            assert all([isinstance(kwargs[dim], (list, np.ndarray,pd.DatetimeIndex)) for dim in kwargs]), "Keeping elements must be contained in lists, np.ndarray or pd.DatetimeIndex"
+        else:
+            assert all([isinstance(kwargs[dim], (list, np.ndarray)) for dim in kwargs]), "Keeping elements must be contained in lists or np.ndarray"
         #TODO: assertion new elements of a dimension coords must have the same type of existing elements
         coords = {}
         for dim in self.coords:
             if dim in kwargs:
-                coords[dim] = np.unique(np.hstack(self.coords[dim], _test_type_and_update(kwargs[dim])))
+                coords[dim] = np.unique(np.hstack((self.coords[dim], _test_type_and_update(kwargs[dim]))))
             else:
                 coords[dim] = self.coords[dim]
         return Array(data=self.long, coords=coords)
 
-    def reduce(self, dim:str, aggfunc=np.add.reduce):
-        '''
-        aggfunc in [np.add.reduce,np.multiply.reduce,np.average]. defult np.add.reduce
-        aggfunc(np.ndarray,axis)
-        axis is index of dim from self.dims.index(dim)
-        '''
+    def reduce(self, dim:str, aggfunc:Union[str,Callable]=np.add.reduce):
+        """
+        Reduce the corresponding dimension by applying a numpy ufunc. The input of the ufunc must be ndarray and axis: aggfunc(np.ndarray,axis) where axis is index of dim from self.dims.index(dim).
+    
+        Args:
+            dim [str] = Dimension to reduce
+            aggfunc [str, Callable] = Strings can be 'sum', 'mean' or 'prod'. Callable should be numpy ufunc such as np.add.reduce, np.multiply.reduce, np.average. The input of the ufunc must be ndarray and axis
+
+        Returns:
+            Updated dict of transposed dense index values and coords
+
+        Example:
+
+            .. code-block:: python
+            
+        """
+        # aggfunc in [np.add.reduce,np.multiply.reduce,np.average]. defult np.add.reduce
+        # aggfunc(np.ndarray,axis)
+        # axis is index of dim from self.dims.index(dim)
+
         assert dim in self.dims, f"dim {dim} not in self.dims: {self.dims}"
+        if isinstance(aggfunc, str):
+            assert aggfunc in ['sum','mean','prod'], "String options for aggfunc can be 'sum', 'mean' or 'prod'"
+            if aggfunc == 'sum':
+                aggfunc = np.add.reduce
+            elif aggfunc == 'mean':
+                aggfunc = np.average
+            elif aggfunc == 'prod':
+                aggfunc = np.multiply.reduce
+        elif isinstance(aggfunc, Callable):
+            pass
         dense = aggfunc(self.dense, axis=self.dims.index(dim))
         dims = [d for d in self.dims if d != dim]
         coords = {k:v for k,v in self.coords.items() if k in dims}
         return self._post_operation(dense.T, coords)
 
+    def _shift_one_dim(self, dim:str, count:int, fill_value:Union[float,None]=None):
+        """
+        shift data in a given dimension by a number of positions along a given axis.
+
+        Args:
+            dim: name of dimension to shift.
+            count: integer offset indicating the number of places by which elements are shifted.
+            fill_value: fill the gaps left due to the shift. Default: None. If none, then self.fill_missing is used.
+        """
+        if fill_value is None:
+            fill_value = self.fill_missing
+
+        ax = self.dims.index(dim)
+        dense = np.roll(self.dense, shift=count, axis=ax)
+        if count > 0:
+            dense.swapaxes(0, ax)[:count] = fill_value
+        elif count < 0:
+            dense.swapaxes(0, ax)[count:] = fill_value
+        return self._post_operation(dense.T, self.coords)
+    
+    def shift(self, fill_value:Union[float,None]=None, **kwargs):
+        if fill_value is None:
+            fill_value = self.fill_missing
+
+        assert len(kwargs) > 0
+        assert all([dim in self.dims for dim in kwargs])
+        assert all([isinstance(kwargs[dim], int) for dim in kwargs])
+
+        obj = self
+
+        for dim in kwargs:
+            obj = obj._shift_one_dim(dim=dim, count=kwargs[dim], fill_value=fill_value)
+
+        return obj
+    
+    def _roll_one_dim(self, dim:str, count:int):
+        """
+        Rolls data in a given dimension by a number of positions along a given axis. For periodic data.
+
+        Args:
+            dim: name of dimension to roll.
+            count: integer offset indicating the number of places by which elements are shifted.
+        """
+        assert dim in self.dims, f"{dim} not in dims: {self.dims}"
+        assert isinstance(count, int), f"{count} must be int"
+
+        ax = self.dims.index(dim)
+        dense = np.roll(self.dense, shift=count, axis=ax)
+        return self._post_operation(dense.T, self.coords)
+    
+    def roll(self, **kwargs):
+        
+        assert len(kwargs) > 0
+        assert all([dim in self.dims for dim in kwargs])
+        assert all([isinstance(kwargs[dim], int) for dim in kwargs])
+
+        obj = self
+
+        for dim in kwargs:
+            obj = obj._roll_one_dim(dim=dim, count=kwargs[dim])
+
+        return obj
+
     def insert(self, **kwargs):
+        """
+        inserts elements into an array object; transforms kwargs into an np.array
+        Example:
+
+            .. code-block:: python
+        Returns:
+            New Array object of long values and coords values
+        Raises:
+            Assertion Error
+        """
         coords = {}
         for new_dim in kwargs:
             assert new_dim not in self.dims
             value = kwargs[new_dim]
-            if isinstance(value, str):
+            if isinstance(value, (np.dtype, type)): # Here a dtype
+                figures = np.array([], dtype=value)
+                coords[new_dim] = _test_type_and_update(figures)
+            elif isinstance(value, str):
                 coords[new_dim] = np.array([value], dtype=np.object_)
             elif isinstance(value, int):
-                coords[new_dim] = np.array([value], dtype=np.integer)
+                coords[new_dim] = np.array([value], dtype=np.int64)
             elif isinstance(value, dict):
                 assert len(value) == 1
                 existing_dim = next(iter(value))
                 assert isinstance(existing_dim, str)
                 assert existing_dim in self.dims
                 assert isinstance(value[existing_dim], (dict,list))
                 if isinstance(value[existing_dim], dict):
@@ -903,166 +1478,338 @@
                     assert len(value[existing_dim]) == 2
                     old_dim_items_set = set(value[existing_dim][0])
                     assert set(self.coords[existing_dim])== old_dim_items_set, f"All items in the mapping dict associated with '{new_dim}' and '{existing_dim}' must be included in .coords['{existing_dim}']"
                     assert len(value[existing_dim][0]) == len(old_dim_items_set), f"There are duplicate items in the mapping dict associated with '{new_dim}' and '{existing_dim}'" # mapping has unique keys
                     if isinstance(value[existing_dim][0], list):
                         kwargs[new_dim][existing_dim][0] = _test_type_and_update(value[existing_dim][0])
                     assert isinstance(kwargs[new_dim][existing_dim][0], np.ndarray)
-                    coords[new_dim] = np.unique(_test_type_and_update(value[existing_dim][1]))
+                    new_dim_items = value[existing_dim][1]
+                    new_dim_items_set = set(new_dim_items)
+                    if len(new_dim_items) == len(new_dim_items_set):
+                        coords[new_dim] = _test_type_and_update(value[existing_dim][1])
+                    else:
+                        coords[new_dim] = np.unique(_test_type_and_update(value[existing_dim][1]))
+            elif isinstance(value, list):
+                assert value, "List cannot be empty"
+                assert all([dim in self.dims for dim in value]), "All items in the list must be in dims"
+                selected_coords = {dim:self.coords[dim] for dim in value}
+                arrays = np.unravel_index(np.arange(self._capacity(selected_coords)), self._shape(selected_coords))
+                index = {dim:self.coords[dim][idx] for dim, idx in zip(selected_coords, arrays)}
+                coords[new_dim] = _join_str(list(index.values()), sep=":")
+                kwargs[new_dim] = {tuple(value):[selected_coords, coords[new_dim]]}
+            else:
+                raise AssertionError(f"Unexpected type: {type(value)}")
         for dim in self.coords:
             coords[dim] = self.coords[dim]
         long = self.long.insert(**kwargs)
         return Array(data=long, coords=coords)
 
     def add_dim(self, **kwargs):
+        """
+        adds a dimension to the array
+        Example:
+
+            .. code-block:: python
+        Returns:
+            an array object with an additional dimension
+        """
         return self.insert(**kwargs)
         
     def rename(self, **kwargs):
+        """
+        adds a dimension to the array
+        Example:
+
+            .. code-block:: python
+        Returns:
+            an array object with an additional dimension
+        Raises:
+            Assertion Error
+        """
         for olddim, newdim in kwargs.items():
             assert olddim in self.dims, f"Dimension {olddim} must be in dims {self.dims}"
             assert newdim not in self.dims, f"Dimension {newdim} must not be in dims {self.dims}"
         coords = {}
         for dim, elems in self.coords.items():
             if dim in kwargs:
                 coords[kwargs[dim]] = elems
             else:
                 coords[dim] = elems
         return Array(data=self.dense, coords=coords)
 
     def drop(self, dims:Union[str, List[str]]):
+        """
+        drops an element from the array object
+        Args:
+            dims: string or list of string that will be dropped
+        Example:
+
+            .. code-block:: python
+
+        Returns:
+            a new array object with less dimensions
+        """
         long = self.long.drop(dims=dims)
         coords = {dim:self.coords[dim] for dim in long.dims}
         return Array(data=long, coords=coords)
     
     def dropna(self):
+        """
+        drops all na-values
+        Args:
+            dims: string or list of string that will be dropped
+        Example:
+
+            .. code-block:: python
+
+        Returns:
+            a new array object without na-values
+        """
         long = self.long
         long = long[long != np.nan]
         return Array(data=long, coords=self.coords)
 
     def dropinf(self, pos:bool=False, neg:bool=False):
+        """
+        drops all infinite values
+        Args:
+            pos (boolean): true if all positive infinite values should be dropped
+            neg (boolean): true if all negative infinite values should be dropped
+        Example:
+
+            .. code-block:: python
+
+        Returns:
+            a new array object without infinite values
+        Raises:
+            AssertionError if both boolean values are false
+        """
         assert any([pos,neg]), "pos and neg cannot be both False"
         long = self.long
         if pos:
             long = long[long != np.inf]
         if neg:
             long = long[long != -np.inf]
         return Array(data=long, coords=self.coords)
 
     def round(self, decimals:int):
+        """note MB: this method might be redundant as the standard round function should cover this"""
+        """
+        rounds values to the decimal numbers provided
+        Args:
+            pos (boolean): true if all positive infinite values should be dropped
+            neg (boolean): true if all negative infinite values should be dropped
+        Example:
+
+            .. code-block:: python
+
+        Returns:
+            a new array object with values rounded to a specific decimal number
+        """
         dense = self.dense.round(decimals=decimals)
         coords = self.coords
         return Array(data=dense, coords=coords)
 
     def elems_to_datetime(self, new_dim:str, actual_dim:str, reference_date:str, freq:str, sort_coords:bool=True):
+        """
+        converts array elements into the datetime-format and returns an array with the corresponding datetime coordinates
+        Args:
+            new_dim (str): new dimension to be created
+            actual_dim (str): existing dimension to be converted to datetime
+            reference_date (str): reference date to use as a starting point for the datetime conversion
+            freq (str): frequency of the datetime coordinates
+            sort_coords (boolean): Whether to sort the new coordinates in ascending order (default: True)
+
+        Example:
+
+            .. code-block:: python
+
+        Returns:
+            An array object with a new dimension `new_dim` and converted to datetime and 
+            with the corresponding datetime coordinates as values
+        """
+        if pandas_enabled:
+            pass
+        else:
+            raise Exception("pandas not installed. Install with `pip install pandas`")
         assert actual_dim in self.dims
         start_date = pd.to_datetime(reference_date)
         t = pd.date_range(start=start_date, periods=self.coords[actual_dim].size, freq=freq)
         if sort_coords:
             new_array = self.insert(**{new_dim:{actual_dim:[np.sort(self.coords[actual_dim]),t]}})
         else:
             new_array = self.insert(**{new_dim:{actual_dim:[self.coords[actual_dim],t]}})
         return new_array
 
     def elems_to_int(self, new_dim:str, actual_dim:str):
+        """
+        Convert the elements of a dimension in the array to integers and return an array with an additional dimension of the corresponding coords
+        Args:
+            new_dim (str): name of the new dimension to be created
+            actual_dim (str): name of the existing dimension to be converted to integers
+        Returns:
+            An array object with a new dimension `new_dim`, converted to integers and 
+            with the corresponding integers coordinates as values
+        """
+        if pandas_enabled:
+            pass
+        else:
+            raise Exception("pandas not installed. Install with `pip install pandas`")
         serie = pd.Series(data=self.coords[actual_dim])
         serie = serie.str.extract(r"(\d+)", expand=False).astype("int")
         new_array = self.insert(**{new_dim:{actual_dim:[self.coords[actual_dim], serie.values]}})
         return new_array
+    
+    def empty(self):
+        return Array(data=({dim:[] for dim in self.dims}, np.array([], dtype=self.dense.dtype)), coords=self.coords)
+    
+    def choice(self, dim:str, seed:int=1):
+        
+        rng = np.random.default_rng(seed=seed)
+        assert dim in self.dims, f"dim {dim} not in self.dims: {self.dims}"
+        axis = self.dims.index(dim)
+        probabilities = self.dense
+        mask = choice_ND(p=probabilities, axis=axis, rng=rng)
+        assert mask.shape == probabilities.shape
+        return Array(data=mask, coords=self.coords)
+
+    def expand(self, **kwargs):
+        """
+        expands the dimensions of the array object 
+        Args:
+            kwargs (dict): dictionary of new dimensions
+        Returns:
+            a new array object
 
-def _test_type_and_update(item:Union[List[str],List[int],List[np.datetime64],np.ndarray,pd.DatetimeIndex]):
-    if len(item) == 0: #
-        return np.array([], dtype=None) # Maybe change to np.object_
-    else:
-        if isinstance(item, np.ndarray):
-            if issubclass(type(item[0]), str):
-                if issubclass(item.dtype.type, np.object_):
-                    variable_out = item.copy()
-                elif issubclass(item.dtype.type, str):
-                    variable_out = item.astype('object')
-                else:
-                    raise Exception(f"item: {item}, type: {type(item[0])} not implemented")
-            elif issubclass(item.dtype.type, np.object_):
-                if issubclass(type(item[0]), int):
-                    variable_out = item.astype('int')
-                else:
-                    raise Exception(f"item: {item}, type: {type(item[0])} not implemented")
-            elif issubclass(item.dtype.type, np.integer):
-                variable_out = item.copy()
-            elif issubclass(item.dtype.type, np.datetime64):
-                variable_out = item.copy()
-            elif issubclass(item.dtype.type, float):
-                assert float(item[0]).is_integer(), f"item accepts float values when they are integers only. Value: {item} , type: {type(item[0])}"
-                variable_out = item.astype('int')
-            else:
-                raise Exception(f"item: {item}, type: {type(item[0])} not implemented")
-        elif isinstance(item, list):
-            value_type = type(item[0])
-            if issubclass(value_type, str):
-                selected_type = 'object'
-            elif issubclass(value_type, int):
-                selected_type = 'int'
-            elif issubclass(value_type, np.datetime64):
-                selected_type = 'datetime64[ns]'
-            elif issubclass(value_type, float):
-                assert float(item[0]).is_integer(), f"item accept float values when they are integers only. Value: {item[0]} , type: {type(item[0])}"
-                selected_type = 'int'
-            else:
-                raise Exception(f"item: {item}, type: {type(item[0])} not implemented")
-            variable_out = np.array(item, dtype=selected_type)
-        elif isinstance(item,pd.DatetimeIndex):
-            variable_out = item.values
+        """
+        return self.empty().insert(**{dim:kwargs[dim].dtype for dim in kwargs}).add_elem(**kwargs) + self
+    
+    def ufunc(self, dim:str, func:Callable, **kwargs):
+        axis = self.dims.index(dim)
+        result = func(a=self.dense, axis=axis, **kwargs)
+        return Array(data=result, coords=self.coords)
+    
+    @property
+    def df(self):
+        if settings.df_with == "pandas":
+            return self.to_pandas()
+        elif settings.df_with == "polars":
+            return self.to_polars()
         else:
-            raise Exception(f"item: {item}, type: {type(item)} not implemented")
-        return variable_out
+            raise Exception(f"ka.settings.df_with must be either 'pandas' or 'polars'")
+
+
 
 def concat(arrays:List[Array]):
+    """
+    Concatenates a list of `Array` objects along their shared dimensions.
+    Args:
+        arrays (List[Array]): list of Array objects to concatenate
+    Returns: 
+        A new `Array` object containing the concatenated data and coordinates
+    Raises:
+        AssertionError
+    """
     dims = arrays[0].dims[:]
     assert all([isinstance(arr, Array) for arr in arrays]), "All list items must be karray.array"
     assert all([set(arr.dims) == set(dims) for arr in arrays]), "All array must have the same dimensions"
     index = {dim:[] for dim in dims}
     value = []
     [index[dim].append(arr.long.index[dim]) for arr in arrays for dim in arr.dims]
     index = {dim:np.hstack(index[dim]) for dim in dims}
     [value.append(arr.long.value) for arr in arrays]
     value = np.hstack(value)
     list_of_coords = [arr.coords for arr in arrays]
     coords = union_multi_coords(*list_of_coords)
     return Array(data=(index,value), coords=coords)
 
 def numpy_to_long(array:np.ndarray, dims:list) -> Long:
+    """
+    Converts a NumPy array to a Long object
+    Args:
+        array (np.ndarray): NumPy array of coordinates and values
+        dims (list): list of dimensions
+    Returns:
+        New Long object constructed from the input array.
+    """
     assert isinstance(array, np.ndarray)
     assert isinstance(dims, list)
     assert array.ndim == 2, "Array must be a 2 dimensions array"
     assert len(dims) + 1 == len(array.T), f"Numpy array must contain {len(dims) + 1} columns"
     value = array.T[len(dims)]
     _index = {dim:arr for dim, arr in zip(dims, array.T[0:len(dims)])}
     _value = value if issubclass(value.dtype.type, float) else value.astype(float)
     return Long(_index, _value)
 
 def _pandas_to_array(df, coords:Union[dict,None]=None):
+    """
+    Converts an np.array to a dictionary
+    Args:
+        df (numpy array): NumPy array of coordinates and values
+        coords (dict): dict of coordinates
+    Returns:
+        New dict constructed from the input values
+    """
     assert "value" in df.columns, "Column named 'value' must exist"
     value = df["value"].values
     df = df.drop(labels="value", axis=1)
-    index = df.to_dict(orient='list')
+    index = {}
+    for col in df.columns:
+        index[col] = df[col].values
     return dict(data=(index,value), coords=coords)
 
 def from_pandas(df, coords:Union[dict,None]=None):
+    """
+    Converts an np.array to an Array
+    Args:
+        df (numpy array): NumPy array of coordinates and values
+        coords (dict): dict of coordinates
+    Returns:
+        New Array constructed from the input values
+    """
     return Array(**_pandas_to_array(df, coords=coords))
 
 def _polars_to_array(df, coords:Union[dict,None]=None):
+    """
+    Converts a polars dataframe to a dict
+    Args:
+        df (numpy array): NumPy array of coordinates and values
+        coords (dict): dict of coordinates
+    Returns:
+        New dict constructed from the input values
+    """
     assert "value" in df.columns, "Column named 'value' must exist"
     value = df["value"].to_numpy()
     df = df.drop(columns="value")
     index = df.to_dict(as_series=False)
     return dict(data=(index,value), coords=coords)
 
 def from_polars(df, coords:Union[dict,None]=None):
+    """
+    Converts a polars dataframe to a dict
+    Args:
+        df (numpy array): NumPy array of coordinates and values
+        coords (dict): dict of coordinates
+    Returns:
+        New array constructed from the input values
+    """
     return Array(**_polars_to_array(df, coords=coords))
 
 def _from_feather(path, use_threads=True, with_:str=None):
+    """
+    converts a feather file into an array
+    Args:
+        path: path of the file to be read
+        use_threads (boolean): If True, uses multiple threads to read the feather file
+        with_(str): package to use for the conversion (pandas or polars)
+    Returns:
+        An `Array` object constructed from the feather file.
+    Raises:
+        AssertionError
+    """
     assert with_ in ["pandas","polars"]
     import pyarrow.feather as ft
     restored_table = ft.read_table(path, use_threads=use_threads)
     column_names = restored_table.column_names
     assert "value" in column_names, "Column named 'value' must exist"
     custom_meta_key = 'karray'
     if custom_meta_key.encode() in restored_table.schema.metadata:
@@ -1079,31 +1826,56 @@
         if with_ == "pandas":
             return _pandas_to_array(df=restored_table.to_pandas(), coords=None)
         elif with_ == "polars":
             import polars as pl
             return _polars_to_array(df=pl.from_arrow(restored_table), coords=None)
 
 def from_feather(path, use_threads=True, with_:str="polars"):
+    """
+    converts a feather file into an array
+    Args:
+        path: path of the file to be read
+        use_threads (boolean): If True, uses multiple threads to read the feather file
+        with_(str): package to use for the conversion (pandas or polars)
+    Returns:
+        An `Array` object constructed from the feather file.
+    """
     return Array(**_from_feather(path=path, use_threads=use_threads, with_=with_))
 
 def _from_csv(path, coords:Union[dict,None]=None, delimiter:str=',', with_:str="numpy"):
+    """
+    converts a csv file into an array
+    Args:
+        path (str): path to the CSV file
+        coords (dict): dictionary containing the coordinate names as keys and their values as
+        values
+        delimiter (str): delimiter used in the CSV file. Defaults to ','
+        with_ (str): library to use for loading the CSV file. Can be one of 'numpy', 'pandas', or
+        'polars'. Defaults to 'numpy'.
+    Returns:
+        dictionary containing the data and coordinates of the array
+    Raises:
+        AssertionError
+    """
     assert with_ in ["numpy","pandas","polars"]
     if with_ == "numpy":
         with open(path,'r') as csvfile:
             reader = csv.reader(csvfile, delimiter=delimiter)
             for row in reader:
                 file_load_headers = row
                 break
         assert file_load_headers[-1] == "value", f"{file_load_headers[-1]}"
         if coords is None:
             dims = file_load_headers[:-1] # remove last column ('value')
         else:
             dims = list(coords)
         
         raw_csv =  np.loadtxt(path, delimiter=delimiter, skiprows=1, dtype=np.object_)
+        if raw_csv.ndim == 1:
+            raw_csv = raw_csv.reshape(1,-1)
 
         index = {}
         i = 0
         for dim in dims:
             arr = raw_csv[:,i]
             arr_ = np.array(list(arr))
             if not issubclass(arr_.dtype.type, str):
@@ -1113,16 +1885,80 @@
         if dims:
             value = raw_csv[:,i].astype(float)
         else:
             assert raw_csv.ndim == 0
             value = raw_csv.astype(float)
         return dict(data=(index,value), coords=coords)
     elif with_ == "pandas":
+        if pandas_enabled:
+            pass
+        else:
+            raise Exception("pandas not installed. Install with `pip install pandas`")
         df = pd.read_csv(path)
         return _pandas_to_array(df=df, coords=coords)
     elif with_ == "polars":
         import polars as pl
         df = pl.read_csv(path)
         return _polars_to_array(df=df, coords=coords)
 
 def from_csv(path, coords:Union[dict,None]=None, delimiter:str=',', with_:str="numpy"):
+    """
+    converts a csv file into an array
+    Args:
+        path (str): path to the CSV file
+        coords (dict): dictionary containing the coordinate names as keys and their values as
+        values
+        delimiter (str): delimiter used in the CSV file. Defaults to ','
+        with_ (str): library to use for loading the CSV file. Can be one of 'numpy', 'pandas', or
+        'polars'. Defaults to 'numpy'.
+    Returns:
+        Array object containing the data and coordinates of the array
+    Raises:
+        AssertionError
+    """
     return Array(**_from_csv(path, coords=coords, delimiter=delimiter, with_=with_))
+
+def _join_str(arr:List[np.ndarray], sep:str) -> np.ndarray:
+    rows = arr[0].shape[0]
+    columns = len(arr)
+    separator_str = np.repeat([sep], rows)
+
+    arrays = []
+    for i in range(columns):
+        arrays.append(arr[i].astype(str))
+        if i != columns-1:
+            arrays.append(separator_str)
+    return reduce(lambda x,y: np.char.add(x,y), arrays)
+
+def choice_ND(p: np.ndarray, axis:int, rng:np.random.Generator) -> np.ndarray:
+    '''   '''
+
+    def _masking(p, axis):
+        shape = [nr for i, nr in enumerate(p.shape) if i != axis]
+        rand = rng.random(tuple(shape))
+        r = np.expand_dims(rand, axis=axis)
+        cum = p.cumsum(axis=axis)
+        assert np.allclose(cum.max(axis=axis), 1.0), "Probabilities do not sum to 1"
+        mask = (cum > r)
+        return mask
+
+    def _unravel(mask, axis):
+        args = mask.argmax(axis=axis, keepdims=True)
+        idx = np.unravel_index(np.arange(args.size), args.shape)
+        args_ravel = args.ravel()
+        new_idx = [arr if i != axis else args_ravel for i, arr in enumerate(idx)]
+        return new_idx
+
+    def _nd_bool(idxs, shape, size):
+        indexes = np.ravel_multi_index(idxs, shape)
+        flatten_dense = np.empty((size,), dtype=bool)
+        flatten_dense[:] = False
+        flatten_dense[indexes] = True
+        nd_dense = flatten_dense.view().reshape(shape)
+        return nd_dense
+    
+    shape = p.shape
+    size = p.size
+    mask = _masking(p, axis)
+    idxs = _unravel(mask, axis)
+    del mask
+    return _nd_bool(idxs,shape, size)
```

### Comparing `karray-0.2.1/karray.egg-info/PKG-INFO` & `karray-0.3.0/karray.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: karray
-Version: 0.2.1
+Version: 0.3.0
 Summary: Lightweight labelled multidimensional arrays with NumPy arrays under the hood.
 Author: Carlos Gaete-Morales
 Author-email: cdgaete@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karray-0.2.1/setup.py` & `karray-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,35 +15,32 @@
         pkg = dirpath.replace(os.path.sep, ".")
         if os.path.altsep:
             pkg = pkg.replace(os.path.altsep, ".")
         packages.append(pkg)
 
 setup(
     name="karray",
-    version="0.2.1",
+    version="0.3.0",
     packages=packages,
     author="Carlos Gaete-Morales",
     author_email="cdgaete@gmail.com",
     install_requires=[
-        "numpy",
-        "pandas",
-        "pyarrow",
+        "numpy"
     ],
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Lightweight labelled multidimensional arrays with NumPy arrays under the hood.",
     classifiers=[
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
     ],
 )
```

