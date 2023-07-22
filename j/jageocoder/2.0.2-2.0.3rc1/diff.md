# Comparing `tmp/jageocoder-2.0.2.tar.gz` & `tmp/jageocoder-2.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-2.0.2.tar", max compression
+gzip compressed data, was "jageocoder-2.0.3rc1.tar", max compression
```

## Comparing `jageocoder-2.0.2.tar` & `jageocoder-2.0.3rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      113 2023-04-17 09:16:28.271600 jageocoder-2.0.2/LICENSE
--rw-r--r--   0        0        0     8253 2023-04-29 04:07:32.527460 jageocoder-2.0.2/README.md
--rw-r--r--   0        0        0     1359 2023-07-12 05:31:17.491752 jageocoder-2.0.2/jageocoder/__init__.py
--rw-r--r--   0        0        0     4622 2023-07-12 05:31:17.491752 jageocoder-2.0.2/jageocoder/__main__.py
--rw-r--r--   0        0        0     2574 2023-04-17 09:16:28.279600 jageocoder-2.0.2/jageocoder/address.py
--rw-r--r--   0        0        0     1421 2023-07-12 05:27:45.348493 jageocoder-2.0.2/jageocoder/aliases.json
--rw-r--r--   0        0        0    12147 2023-04-29 04:07:32.535460 jageocoder-2.0.2/jageocoder/aza_master.py
--rw-r--r--   0        0        0     1171 2023-04-29 04:07:32.535460 jageocoder-2.0.2/jageocoder/dataset.py
--rw-r--r--   0        0        0      691 2023-04-17 09:16:28.279600 jageocoder-2.0.2/jageocoder/exceptions.py
--rw-r--r--   0        0        0    18862 2023-04-22 02:31:05.987235 jageocoder-2.0.2/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-04-17 09:16:28.279600 jageocoder-2.0.2/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    10888 2023-07-12 05:31:17.491752 jageocoder-2.0.2/jageocoder/module.py
--rw-r--r--   0        0        0    37186 2023-07-12 05:27:45.348493 jageocoder-2.0.2/jageocoder/node.py
--rw-r--r--   0        0        0     2631 2023-04-29 04:07:32.535460 jageocoder-2.0.2/jageocoder/result.py
--rw-r--r--   0        0        0    15241 2023-07-12 05:27:45.348493 jageocoder-2.0.2/jageocoder/rtree.py
--rw-r--r--   0        0        0     7854 2023-04-17 09:16:28.283600 jageocoder-2.0.2/jageocoder/strlib.py
--rw-r--r--   0        0        0    48985 2023-07-12 05:27:45.348493 jageocoder-2.0.2/jageocoder/tree.py
--rw-r--r--   0        0        0     4995 2023-04-29 04:07:32.535460 jageocoder-2.0.2/jageocoder/trie.py
--rw-r--r--   0        0        0     1225 2023-07-12 05:31:17.491752 jageocoder-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     9684 1970-01-01 00:00:00.000000 jageocoder-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-04-17 09:16:28.271600 jageocoder-2.0.3rc1/LICENSE
+-rw-r--r--   0        0        0     8253 2023-04-29 04:07:32.527460 jageocoder-2.0.3rc1/README.md
+-rw-r--r--   0        0        0     1362 2023-07-22 06:18:13.668357 jageocoder-2.0.3rc1/jageocoder/__init__.py
+-rw-r--r--   0        0        0     6190 2023-07-22 07:23:49.444644 jageocoder-2.0.3rc1/jageocoder/__main__.py
+-rw-r--r--   0        0        0     2574 2023-04-17 09:16:28.279600 jageocoder-2.0.3rc1/jageocoder/address.py
+-rw-r--r--   0        0        0     1421 2023-07-12 05:27:45.348493 jageocoder-2.0.3rc1/jageocoder/aliases.json
+-rw-r--r--   0        0        0    12147 2023-04-29 04:07:32.535460 jageocoder-2.0.3rc1/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2023-04-29 04:07:32.535460 jageocoder-2.0.3rc1/jageocoder/dataset.py
+-rw-r--r--   0        0        0      691 2023-04-17 09:16:28.279600 jageocoder-2.0.3rc1/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    18862 2023-04-22 02:31:05.987235 jageocoder-2.0.3rc1/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-04-17 09:16:28.279600 jageocoder-2.0.3rc1/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    11408 2023-07-22 07:19:14.984430 jageocoder-2.0.3rc1/jageocoder/module.py
+-rw-r--r--   0        0        0    37985 2023-07-22 06:18:13.668357 jageocoder-2.0.3rc1/jageocoder/node.py
+-rw-r--r--   0        0        0     2631 2023-04-29 04:07:32.535460 jageocoder-2.0.3rc1/jageocoder/result.py
+-rw-r--r--   0        0        0    15253 2023-07-22 06:18:13.668357 jageocoder-2.0.3rc1/jageocoder/rtree.py
+-rw-r--r--   0        0        0     7854 2023-04-17 09:16:28.283600 jageocoder-2.0.3rc1/jageocoder/strlib.py
+-rw-r--r--   0        0        0    49426 2023-07-22 07:18:17.917448 jageocoder-2.0.3rc1/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-04-29 04:07:32.535460 jageocoder-2.0.3rc1/jageocoder/trie.py
+-rw-r--r--   0        0        0     1228 2023-07-22 06:18:13.668357 jageocoder-2.0.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     9687 1970-01-01 00:00:00.000000 jageocoder-2.0.3rc1/PKG-INFO
```

### Comparing `jageocoder-2.0.2/README.md` & `jageocoder-2.0.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/__init__.py` & `jageocoder-2.0.3rc1/jageocoder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '2.0.2'  # The package version
+__version__ = '2.0.3rc1'  # The package version
 __dictionary_version__ = '20230405'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
```

### Comparing `jageocoder-2.0.2/jageocoder/__main__.py` & `jageocoder-2.0.3rc1/jageocoder/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,73 @@
 import json
 import logging
+import os
 import sys
 
 import jageocoder
 from jageocoder.exceptions import JageocoderError
 from docopt import docopt
 
 HELP = """
-'jageocoder' is a Python package of Japanese-address geocoder.
+'jageocoder' は日本の住所ジオコーダを実装した Python パッケージです。
 
 Usage:
   {p} -h
   {p} -v
   {p} search [-d] [--area=<area>] [--db-dir=<dir>] [--force-aza-skip|--disable-aza-skip] <address>
   {p} reverse [-d] [--level=<level>] [--db-dir=<dir>] <longitude> <latitude>
   {p} get-db-dir [-d]
   {p} download-dictionary [-d] <url>
   {p} install-dictionary [-d] [-y] [--db-dir=<dir>] <path>
   {p} uninstall-dictionary [-d] [--db-dir=<dir>]
 
 Options:
-  -h --help           Show this help.
-  -v --version        Show version number.
-  -d --debug          Show debug messages.
-  --area=<area>       Specify the target area by jiscode or names.
-  --force-aza-skip    Skip aza-names whenever possible.
-  --disable-aza-skip  Do not skip aza-names.
-  --level=<level>     Max address level to search.
-  --db-dir=<dir>      Specify dictionary directory.
+  -h --help           このヘルプメッセージを表示します.
+  -v --version        バージョン番号を表示します.
+  -d --debug          実行時にデバッグメッセージを表示します.
+  -y --yes            確認メッセージに対して自動的に y と答えます。
+  --area=<area>       検索対象地域の都道府県・市区町村名を指定します。
+  --force-aza-skip    「字」を常にスキップします。
+  --disable-aza-skip  「字」を常にスキップしません。
+  --level=<level>     検索する住所レベルを指定します。
+  --db-dir=<dir>      住所データベースのディレクトリを指定します。
 
 Examples:
 
-- Search address
+- 住所を検索します。
 
   {p} search 多摩市落合1-15
   {p} search --area=14152 中央1-1
   {p} search --area=東京都 落合1-15
+  {p} search --area=町田市,八王子市 中町１－１
 
-- Show dictionary directory
+  環境変数で検索オプションを指定できます（[]内がデフォルト）。
+  - JAGEOCODER_OPT_AZA_SKIP (on,off,[auto])
+    「字」のスキップ処理を指定します。
+  - JAGEOCODER_OPT_BEST_ONLY ([true],false)
+    最適解のみ表示するかどうかを指定します。
+  - JAGEOCODER_OPT_REQUIRE_COORDINATES ([true],false)
+    座標が登録されている住所のみ検索対象とするかどうかを指定します。
+    座標が登録されていない場合、経緯度 ≒ 999.9 と表示されます。
+
+- 住所データベースのディレクトリを表示します。
 
   {p} get-db-dir
 
-- Install dictionary
+- 住所データベースをインストールします。
 
-  (Download from web)
+  (ウェブから最新の全国住居表示レベルデータファイルをダウンロードします)
   {p} download-dictionary https://www.info-proto.com/static/jageocoder/latest/jukyo_all_v20.zip
 
-  (Install from the file)
+  (ダウンロードしたファイルをインストールします)
   {p} install-dictionary jukyo_all_v20.zip
 
-- Uninstall dictionary in '/home/foo/jageocoder_db/'
+- 住所データベースをアンインストールします。
 
-  {p} uninstall-dictionary --db-dir=/home/foo/jageocoder_db
+  {p} uninstall-dictionary
 """.format(p='jageocoder')  # noqa: E501
 
 
 def main():
     args = docopt(HELP)
 
     if args['--version']:
@@ -78,35 +90,44 @@
     console_handler.setFormatter(
         logging.Formatter('%(levelname)s:%(name)s:%(lineno)s:%(message)s')
     )
     logger.addHandler(console_handler)
 
     if args['search']:
         jageocoder.init(db_dir=args['--db-dir'], mode='r')
-        skip_aza = 'auto'
+        search_options = {}
+        target_area = None
         if args.get('--area'):
             target_area = args['--area'].split(',')
-        else:
-            target_area = None
 
         if args['--disable-aza-skip']:
-            skip_aza = 'off'
+            search_options['aza_skip'] = False
         elif args['--force-aza-skip']:
-            skip_aza = 'on'
+            search_options['aza_skip'] = True
+        else:
+            aza_skip = os.environ.get(
+                'JAGEOCODER_OPT_AZA_SKIP', 'auto')
+            search_options['aza_skip'] = aza_skip
+
+        search_options['best_only'] = os.environ.get(
+            'JAGEOCODER_OPT_BEST_ONLY', 'true')
+        search_options['require_coordinates'] = os.environ.get(
+            'JAGEOCODER_OPT_REQUIRE_COORDINATES', 'true')
 
         try:
-            jageocoder.set_search_config(
-                aza_skip=skip_aza, target_area=target_area)
+            jageocoder.set_search_config(target_area=target_area)
         except RuntimeError:
             print((
                 "'{}' is incorrect as a parameter for "
                 "the --area option.").format(args['--area']),
                 file=sys.stderr)
             exit(1)
 
+        jageocoder.set_search_config(**search_options)
+
         try:
             print(json.dumps(
                 jageocoder.search(query=args['<address>']),
                 ensure_ascii=False))
         except RuntimeError as e:
             print(
                 "An error occurred during the search: {}".format(e),
```

### Comparing `jageocoder-2.0.2/jageocoder/address.py` & `jageocoder-2.0.3rc1/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/aliases.json` & `jageocoder-2.0.3rc1/jageocoder/aliases.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/aza_master.py` & `jageocoder-2.0.3rc1/jageocoder/aza_master.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/dataset.py` & `jageocoder-2.0.3rc1/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/exceptions.py` & `jageocoder-2.0.3rc1/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/itaiji.py` & `jageocoder-2.0.3rc1/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/itaiji_dic.json` & `jageocoder-2.0.3rc1/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/module.py` & `jageocoder-2.0.3rc1/jageocoder/module.py`

 * *Files 9% similar despite different names*

```diff
@@ -190,15 +190,16 @@
 
         If omitted, use `get_db_dir()` to decide the directory.
     """
     # Set default value
     if db_dir is None:
         db_dir = get_db_dir(mode='w')
 
-    if skip_confirmation is not True and (db_dir / 'address_node').exists():
+    if skip_confirmation is not True and os.path.exists(
+            os.path.join(db_dir, 'address_node')):
         # Dictionary had been installed.
         r = input("他の辞書がインストール済みです。上書きしますか？(Y/n) ")
         if r.lower()[0] != 'y':
             return
 
     if os.path.exists(path):
         path = path
@@ -321,24 +322,40 @@
         List of dict representation of nodes with
         the longest match to the query string.
     """
     if not is_initialized():
         raise JageocoderError("Not initialized. Call 'init()' first.")
 
     global _tree
-    set_search_config(best_only=True)
+    # set_search_config(best_only=True)
     results = _tree.searchNode(query)
 
-    if len(results) == 0:
-        return {'matched': '', 'candidates': []}
-
-    return {
-        'matched': results[0][1],
-        'candidates': [x[0].as_dict() for x in results],
-    }
+    if _tree.get_config('best_only'):
+        if len(results) == 0:
+            return {'matched': '', 'candidates': []}
+
+        return {
+            'matched': results[0][1],
+            'candidates': [x[0].as_dict() for x in results],
+        }
+
+    result_by_matched = {}
+    for result in results:
+        if result.matched not in result_by_matched:
+            result_by_matched[result.matched] = []
+
+        result_by_matched[result.matched].append(result.node.as_dict())
+
+    return [
+        {"matched": r[0], "candidates": r[1]} for r in sorted(
+            result_by_matched.items(),
+            key=lambda x: len(x[0]),
+            reverse=True
+        )
+    ]
 
 
 def searchNode(query: str) -> List[Result]:
     """
     Searches for address nodes corresponding to an address notation
     and returns the matching substring and a list of nodes.
```

### Comparing `jageocoder-2.0.2/jageocoder/node.py` & `jageocoder-2.0.3rc1/jageocoder/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+import copy
 from functools import lru_cache
 import json
 import logging
 import os
 import re
 from typing import List, Optional, TYPE_CHECKING
 
@@ -295,14 +296,32 @@
                 pos = node.sibling_id
             else:
                 parent = self.table.get_record(pos=node.parent_id)
                 pos = parent.sibling_id
 
         return children
 
+    def add_dummy_coordinates(self) -> AddressNode:
+        """
+        Add dummy coordinate values to the node.
+        """
+        children = self.children
+        new_node = copy.copy(self)
+        for child in children:
+            if child.y <= 90.0:
+                new_node.x, new_node.y = child.x, child.y
+                logger.debug((
+                    "Node {}({}) has no coordinates. "
+                    "Use the coordinates of the child {}({}) instead."
+                ).format(
+                    self.name, self.id, child.name, child.id))
+                break
+
+        return new_node
+
     def search_child_with_criteria(
             self,
             pattern: str,
             min_candidate: Optional[str] = None,
             gt_candidate: Optional[str] = None,
             max_level: Optional[int] = None,
             require_coordinates: bool = False):
@@ -373,17 +392,21 @@
             candidate = self.table.get_record(pos=next_pos)
 
             if gt_candidate is not None and \
                     candidate.name_index >= gt_candidate:
                 break
 
             if re_pattern.match(candidate.name_index) and \
-                    (max_level is None or candidate.level <= max_level) and \
-                    (require_coordinates is False or candidate.y <= 90.0):
-                children.append(candidate)
+                    (max_level is None or candidate.level <= max_level):
+                if require_coordinates is False or candidate.y <= 90.0:
+                    children.append(candidate)
+                else:
+                    candidate = candidate.add_dummy_coordinates()
+                    if candidate.y <= 90.0:
+                        children.append(candidate)
 
             next_pos = candidate.sibling_id
 
         logger.debug("  -> {} found.".format(len(children)))
         return children
 
     def search_recursive(
```

### Comparing `jageocoder-2.0.2/jageocoder/result.py` & `jageocoder-2.0.3rc1/jageocoder/result.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/rtree.py` & `jageocoder-2.0.3rc1/jageocoder/rtree.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
             Created rtree index.
         """
         file_idx = index.Rtree(str(treepath))
         node_table: AddressNodeTable = self._tree.address_nodes
 
         max_id = node_table.count_records()
         id = AddressNode.ROOT_NODE_ID
-        with tqdm(total=max_id, mininterval=0.5) as pbar:
+        with tqdm(total=max_id, mininterval=0.5, ascii=True) as pbar:
             prev_id = 0
             while id < max_id:
                 pbar.update(id - prev_id)
                 prev_id = id
 
                 node = node_table.get_record(pos=id)
                 if node.level > AddressLevel.AZA:
```

### Comparing `jageocoder-2.0.2/jageocoder/strlib.py` & `jageocoder-2.0.3rc1/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/jageocoder/tree.py` & `jageocoder-2.0.3rc1/jageocoder/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,17 @@
         -----
         If the key-value pair is not valid, raise RuntimeError.
         """
         if key == 'target_area':
             if value in (None, []):
                 return
 
+            if re.match(r'\d{2}', value) or re.match(r'\d{5}', value):
+                return
+
             # Check if the value is a name of node in the database.
             std = self.converter.standardize(value)
             candidates = self.trie.common_prefixes(std)
             if std in candidates:
                 trie_node_id = candidates[std]
                 for node_id in self.trie_nodes.get_record(
                         pos=trie_node_id).nodes:
@@ -436,17 +439,17 @@
                 pass
             elif isinstance(value, int):
                 if value == 0:
                     value = False
                 else:
                     value = True
             elif isinstance(value, str):
-                if value.lower() in ('on', 'enable', 'true'):
+                if value.lower() in ('on', 'enable', 'true', 'yes'):
                     value = True
-                elif value.lower() in ('off', 'disable', 'false'):
+                elif value.lower() in ('off', 'disable', 'false', 'no'):
                     value = False
                 elif value.lower() in ('auto', 'none', ''):
                     value = None
                 else:
                     msg = ("The value '{}' for '{}' cannot be recognized "
                            "as bool or None.")
                     raise RuntimeError(msg.format(value, key))
@@ -1199,14 +1202,21 @@
             trie_node = self.trie_nodes.get_record(pos=trie_id)
             offset = self.converter.match_len(index, k)
             key = index[0:offset]
             rest_index = index[offset:]
             for node_id in trie_node.nodes:
                 node = self.get_address_node(id=node_id)
 
+                if node.y > 90.0 and self.get_config('require_coordinates'):
+                    node = node.add_dummy_coordinates()
+                    if node.y > 90.0:
+                        logger.debug("Node {}({}) has no coordinates.".format(
+                            node.name, node.id))
+                        continue
+
                 if min_key == '' and node.level <= AddressLevel.WARD:
                     # To make the process quicker, once a node higher
                     # than the city level is found, addresses shorter
                     # than the node are not searched after this.
                     logger.debug((
                         "A node with ward or higher levels found. "
                         "Set min_key to '{}'").format(k))
```

### Comparing `jageocoder-2.0.2/jageocoder/trie.py` & `jageocoder-2.0.3rc1/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.0.2/pyproject.toml` & `jageocoder-2.0.3rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "2.0.2"
+version = "2.0.3rc1"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
```

### Comparing `jageocoder-2.0.2/PKG-INFO` & `jageocoder-2.0.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 2.0.2
+Version: 2.0.3rc1
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

