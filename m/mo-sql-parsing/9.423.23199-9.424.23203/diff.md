# Comparing `tmp/mo_sql_parsing-9.423.23199-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.424.23203-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38292 bytes, number of entries: 13
+Zip file size: 38347 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2530 b- defN 23-Jul-18 01:32 mo_sql_parsing/__init__.py
 -rw-rw-rw-  2.0 fat    22382 b- defN 23-Jul-18 01:32 mo_sql_parsing/formatting.py
 -rw-rw-rw-  2.0 fat    10695 b- defN 23-Jul-18 01:32 mo_sql_parsing/keywords.py
--rw-rw-rw-  2.0 fat    33903 b- defN 23-Jul-18 01:32 mo_sql_parsing/sql_parser.py
--rw-rw-rw-  2.0 fat     7321 b- defN 23-Mar-26 12:53 mo_sql_parsing/types.py
+-rw-rw-rw-  2.0 fat    34100 b- defN 23-Jul-22 13:56 mo_sql_parsing/sql_parser.py
+-rw-rw-rw-  2.0 fat     7357 b- defN 23-Jul-22 13:56 mo_sql_parsing/types.py
 -rw-rw-rw-  2.0 fat    22995 b- defN 23-Jul-18 01:32 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2920 b- defN 23-Jul-18 01:32 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/RECORD
-13 files, 129274 bytes uncompressed, 36386 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-Jul-22 13:56 mo_sql_parsing-9.424.23203.dist-info/RECORD
+13 files, 129507 bytes uncompressed, 36441 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.423.23199.dist-info/LICENSE
+Filename: mo_sql_parsing-9.424.23203.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.423.23199.dist-info/METADATA
+Filename: mo_sql_parsing-9.424.23203.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.423.23199.dist-info/WHEEL
+Filename: mo_sql_parsing-9.424.23203.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.423.23199.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.424.23203.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.423.23199.dist-info/zip-safe
+Filename: mo_sql_parsing-9.424.23203.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.423.23199.dist-info/RECORD
+Filename: mo_sql_parsing-9.424.23203.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/sql_parser.py

```diff
@@ -289,14 +289,15 @@
             function_name("op")
             + LB
             + Optional(flag("distinct"))
             + Optional(delimited_list(one_param) | Group(query)("params"))
             + Optional((keyword("respect") | keyword("ignore"))("nulls") + keyword("nulls").suppress())
             + Optional(ORDER_BY + delimited_list(Group(sort_column))("orderby"))
             + Optional(assign("limit", expression))
+            + Optional(assign("separator", expression))
             + RB
         ) / to_json_call
 
         dynamic_accessor = LK + expression + RK
         simple_accessor = Literal(".").suppress() + simple_ident / to_literal
         accessor = (
             Literal(":").suppress()
@@ -602,14 +603,15 @@
             )
             + Optional(AS.suppress() + infix_notation(query, [])("query"))
         )("create table")
 
         create_view = (
             keyword("create")
             + Optional(keyword("or") + flag("replace"))
+            + Optional(keyword("algorithm").suppress() + EQ + (keyword("merge") | keyword("temptable") | keyword("undefined"))("algorithm"))
             + temporary
             + VIEW.suppress()
             + Optional((keyword("if not exists") / False)("replace"))
             + identifier("name")
             + AS
             + query("query")
         )("create view")
```

## mo_sql_parsing/types.py

```diff
@@ -226,14 +226,15 @@
         | assign("comment", literal_string)
         | assign("collate", Optional(EQ) + identifier)
         | flag("primary key")
         | column_def_identity("identity")
         | column_def_references
         | assign("check", LB + expr + RB)
         | assign("default", expr)
+        | assign("on update", expr)
     )
 
     column_definition << Group(identifier("name") + (column_type | identifier("type")) + ZeroOrMore(column_options))
 
     set_parser_names()
 
     return column_type, column_definition, column_def_references, column_options
```

## Comparing `mo_sql_parsing-9.423.23199.dist-info/LICENSE` & `mo_sql_parsing-9.424.23203.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.423.23199.dist-info/METADATA` & `mo_sql_parsing-9.424.23203.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.423.23199
+Version: 9.424.23203
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
```

