# Comparing `tmp/kobushi_trackviewer-1.1.5-py3-none-any.whl.zip` & `tmp/kobushi_trackviewer-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 42462 bytes, number of entries: 19
+Zip file size: 42490 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      634 b- defN 21-Aug-15 09:07 kobushi/__init__.py
 -rw-r--r--  2.0 unx      649 b- defN 21-Aug-14 12:53 kobushi/__main__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-24 15:41 kobushi/_version.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-22 01:57 kobushi/_version.py
 -rw-r--r--  2.0 unx     3482 b- defN 21-Aug-20 14:15 kobushi/dialog_multifields.py
 -rw-r--r--  2.0 unx    35123 b- defN 23-Jun-24 15:41 kobushi/gui_interface.py
 -rw-r--r--  2.0 unx     2999 b- defN 21-Aug-14 12:53 kobushi/loadheader.py
 -rw-r--r--  2.0 unx      761 b- defN 22-Oct-15 12:32 kobushi/loadmapgrammer.py
 -rw-r--r--  2.0 unx     1665 b- defN 22-Apr-18 12:51 kobushi/map-grammer.lark
--rw-r--r--  2.0 unx     9920 b- defN 22-Oct-15 12:32 kobushi/mapinterpreter.py
--rw-r--r--  2.0 unx    11615 b- defN 22-Mar-10 13:40 kobushi/mapobj.py
+-rw-r--r--  2.0 unx     9929 b- defN 23-Jul-22 02:36 kobushi/mapinterpreter.py
+-rw-r--r--  2.0 unx    11659 b- defN 23-Jul-22 02:37 kobushi/mapobj.py
 -rw-r--r--  2.0 unx    17242 b- defN 23-Jun-24 15:41 kobushi/mapplot.py
 -rw-r--r--  2.0 unx     6306 b- defN 21-Aug-20 14:15 kobushi/othertrack_window.py
 -rw-r--r--  2.0 unx    17540 b- defN 23-Mar-18 15:38 kobushi/trackcoordinate.py
 -rw-r--r--  2.0 unx    35622 b- defN 23-Jun-24 15:41 kobushi/trackgenerator.py
--rw-r--r--  2.0 unx     9724 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2749 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1562 b- defN 23-Jun-25 04:24 kobushi_trackviewer-1.1.5.dist-info/RECORD
-19 files, 157715 bytes uncompressed, 39920 bytes compressed:  74.7%
+-rw-r--r--  2.0 unx     9724 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2749 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1562 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/RECORD
+19 files, 157768 bytes uncompressed, 39948 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: kobushi/trackcoordinate.py
 Comment: 
 
 Filename: kobushi/trackgenerator.py
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.5.dist-info/LICENSE
+Filename: kobushi_trackviewer-1.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.5.dist-info/METADATA
+Filename: kobushi_trackviewer-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.5.dist-info/WHEEL
+Filename: kobushi_trackviewer-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.5.dist-info/top_level.txt
+Filename: kobushi_trackviewer-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.5.dist-info/RECORD
+Filename: kobushi_trackviewer-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kobushi/_version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.5'
+__version__ = '1.1.6'
```

## kobushi/mapinterpreter.py

```diff
@@ -1,9 +1,9 @@
 '''
-    Copyright 2021-2022 konawasabi
+    Copyright 2021-2023 konawasabi
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -39,18 +39,18 @@
         if(env==None):
             self.environment = mapobj.Environment()
             self.isroot=True
         else:
             self.environment = env
             self.isroot=False
     def set_distance(self, value): #距離程設定
-        self.environment.variable['distance'] = float(value)
+        self.environment.predef_vars['distance'] = float(value)
         self.environment.controlpoints.add(float(value))
     def call_predefined_variable(self, argument): #規定変数呼び出し（現実的にはdistanceのみ）
-        return self.environment.variable[argument.lower()]
+        return self.environment.predef_vars[argument.lower()]
     def set_variable(self, *argument): #変数設定
         self.environment.variable[argument[0].lower()]=argument[1]
     def call_variable(self, argument): #変数呼び出し
         return self.environment.variable[argument.lower()]
     def call_function(self, *argument): #数学関数呼び出し
         label = argument[0].lower()
         if (label == 'rand'):
@@ -175,15 +175,15 @@
 
         #print(tree)
         #import pdb
         #pdb.set_trace()
         try: #ツリー処理
             self.transform(tree)
         except Exception as e:
-            raise RuntimeError('IntepretationError: in file '+str(f_path)+', distance='+str(self.environment.variable['distance'])+'\n'+str(e))
+            raise RuntimeError('IntepretationError: in file '+str(f_path)+', distance='+str(self.environment.predef_vars['distance'])+'\n'+str(e))
             #print(self.environment.variable)
             
         
         if(self.isroot): # 最上層のマップファイルのロードが完了したら、データを距離でソート
             self.environment.controlpoints.relocate()
             self.environment.own_track.relocate()
             self.environment.othertrack.relocate()
```

## kobushi/mapobj.py

```diff
@@ -1,9 +1,9 @@
 '''
-    Copyright 2021 konawasabi
+    Copyright 2021-2023 konawasabi
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -22,15 +22,16 @@
     self.variable:   変数を格納するdict
     self.own_track:  自軌道データを格納するオブジェクト
     self.station:    stationデータを格納するオブジェクト
     self.controlpoints: Map要素が指定されている距離程リスト
     '''
     def __init__(self):
         self.rootpath = ''
-        self.variable = {'distance':0.0}
+        self.predef_vars = {'distance':0.0}
+        self.variable = {}
         self.own_track = Owntrack(self)
         self.station = Station(self)
         self.controlpoints = ControlPoints(self)
         self.othertrack = Othertrack(self)
 class Owntrack():
     '''自軌道データクラス
     (1)パーサが読み取った自軌道マップ要素を変換するサブクラス
@@ -127,15 +128,15 @@
         key
             マップ要素の種別
         value
             Noneの場合、'c':直前のコマンドで指定された値と同一を代入
         flag
             '':change, 'i':interpolate, 'bt':begintransition
         '''
-        self.data.append({'distance':self.environment.variable['distance'], 'value':'c' if value == None else value, 'key':key, 'flag':flag})
+        self.data.append({'distance':self.environment.predef_vars['distance'], 'value':'c' if value == None else value, 'key':key, 'flag':flag})
     def relocate(self):
         self.data = sorted(self.data, key=lambda x: x['distance'])
         
 class Station():
     def load(self, *argvs):
         input = loadheader.joinpath(self.environment.rootpath, argvs[0]) #与えられたファイル名とrootpathから絶対パスを作成する。
         f_path, rootpath_tmp, f_encoding = loadheader.loadheader(input,'BveTs Station List ',0.04) #station listファイルかどうか判定する。
@@ -170,15 +171,15 @@
                 encode_retry = 'utf-8'
             try:
                 self.stationkey = read_stationlist(f_path,encode_retry)
             except Exception as e:
                 raise RuntimeError('File encoding error: '+str(f_path))
     def put(self, *argvs):
         #self.position.append({'distance':self.environment.variable['distance'], 'stationkey':argvs[0].lower()})
-        self.position[self.environment.variable['distance']]=argvs[0].lower()
+        self.position[self.environment.predef_vars['distance']]=argvs[0].lower()
     def __init__(self, parent):
         self.position = {}
         self.stationkey = {}
         self.environment = parent
 
 class ControlPoints():
     '''マップ要素が存在する距離程のリストを作る
@@ -266,13 +267,13 @@
         '''
         if type(trackkey) == float:
             trackkey_lc = str(int(trackkey)).lower()
         else:
             trackkey_lc = str(trackkey).lower()
         if trackkey_lc not in self.data.keys():
             self.data[trackkey_lc] = []
-        self.data[trackkey_lc].append({'distance':self.environment.variable['distance'], 'value':'c' if value == None else value, 'key':elementkey, 'flag':flag})
+        self.data[trackkey_lc].append({'distance':self.environment.predef_vars['distance'], 'value':'c' if value == None else value, 'key':elementkey, 'flag':flag})
     def relocate(self):
         self.cp_range = {}
         for trackkey in self.data.keys():
             self.data[trackkey]     = sorted(self.data[trackkey], key=lambda x: x['distance'])
             self.cp_range[trackkey] = {'min':min(self.data[trackkey], key=lambda x: x['distance'])['distance'],'max':max(self.data[trackkey], key=lambda x: x['distance'])['distance']}
```

## Comparing `kobushi_trackviewer-1.1.5.dist-info/LICENSE` & `kobushi_trackviewer-1.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kobushi_trackviewer-1.1.5.dist-info/METADATA` & `kobushi_trackviewer-1.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobushi-trackviewer
-Version: 1.1.5
+Version: 1.1.6
 Summary: Trackviewer for BVE trainsim 5/6
 Home-page: https://github.com/konawasabi/kobushi-trackviewer/
 Author: Konawasabi
 Author-email: webmaster@konawasabi.riceball.jp
 License: Apache License 2.0
 Keywords: BVE trainsim
 Description-Content-Type: text/markdown
```

## Comparing `kobushi_trackviewer-1.1.5.dist-info/RECORD` & `kobushi_trackviewer-1.1.6.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 kobushi/__init__.py,sha256=_OBJRtuhwlJl97iwmsRFAjWTMcS1F7fivZjoumsd8qk,634
 kobushi/__main__.py,sha256=zrMhFiAoyKL6DprEbJWok4KNmlsu-fVIA7xT581287E,649
-kobushi/_version.py,sha256=hTCioFruYR1lv7FF57n5II-8lYry8FuIYb1fA4g2ccc,22
+kobushi/_version.py,sha256=DqimR_gm7By2qcKv1KJXbXiFxmVaELzxn4_BJ8iUCqg,22
 kobushi/dialog_multifields.py,sha256=hWcMMg8KOFql3NC-jQueRrnNUJpQutSI9IOjLh6cleU,3482
 kobushi/gui_interface.py,sha256=SqpZ9EK3vIj3zWDOEw3zRSLYAL0QGn_iH5wZMxRwz94,35123
 kobushi/loadheader.py,sha256=rLutNKL6VAgZXNwyaLmkiz8j3I6VOs93XqqbxFD6Ods,2999
 kobushi/loadmapgrammer.py,sha256=f5OHCL2l483D0IkBLTulsfQZfLcDmyidutt7TDjSHbU,761
 kobushi/map-grammer.lark,sha256=PxlMWCVglsMQMdF80Vfiz6vgGhL-GdLxhWJ58vrT2tw,1665
-kobushi/mapinterpreter.py,sha256=8UuvA5gf5bweLL65GJqUVpF4oSLH8lzlldgJMW22eW4,9920
-kobushi/mapobj.py,sha256=0usquigcUu1BhPf3sHsdOHkFesbVe31LIhhyutbp4aw,11615
+kobushi/mapinterpreter.py,sha256=-HlhhH6IjVVXl3nYu81oq7GCwzuIw6QxuMiNDRBpTU0,9929
+kobushi/mapobj.py,sha256=Gi_xxHAwcK5uIiPXjIr6_om-QvD16_-qFhAuU5q7PFc,11659
 kobushi/mapplot.py,sha256=BLCquNYeJSkMHkfMlm62vwLTfTj5aY26NI-fpEhg4Ck,17242
 kobushi/othertrack_window.py,sha256=662M8YTWkASbnhet6G9ZupYVO8Pi9zT_p8HgZizERPA,6306
 kobushi/trackcoordinate.py,sha256=dwu44v5uvA8yUcJOs50eNLzktOFJJT28pUhccXGJRR8,17540
 kobushi/trackgenerator.py,sha256=9p_elvjclxYnqrxaLwMaFrZkw-exg5ocUijVihy5614,35622
-kobushi_trackviewer-1.1.5.dist-info/LICENSE,sha256=OURbRZ-GYhaD-XMftqfQcIGdw3mEDo71L2K7HGiUIpE,9724
-kobushi_trackviewer-1.1.5.dist-info/METADATA,sha256=fqNeL_3a5UnKOdOsjM35O7tzDqNFXXqmjeaRKqHGOcU,2749
-kobushi_trackviewer-1.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kobushi_trackviewer-1.1.5.dist-info/top_level.txt,sha256=g2m4m7gw1NgwbluSrxfBImA8GHjvuXwFnHgkagrMPB0,8
-kobushi_trackviewer-1.1.5.dist-info/RECORD,,
+kobushi_trackviewer-1.1.6.dist-info/LICENSE,sha256=OURbRZ-GYhaD-XMftqfQcIGdw3mEDo71L2K7HGiUIpE,9724
+kobushi_trackviewer-1.1.6.dist-info/METADATA,sha256=Zo854Np5eJ5igKoq_wDgVfhVLFNJ-R834ZCbzE2Ecz0,2749
+kobushi_trackviewer-1.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kobushi_trackviewer-1.1.6.dist-info/top_level.txt,sha256=g2m4m7gw1NgwbluSrxfBImA8GHjvuXwFnHgkagrMPB0,8
+kobushi_trackviewer-1.1.6.dist-info/RECORD,,
```

