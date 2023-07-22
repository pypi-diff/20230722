# Comparing `tmp/cashare-0.0.5.tar.gz` & `tmp/cashare-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashare-0.0.5.tar", last modified: Mon Jun  5 12:03:44 2023, max compression
+gzip compressed data, was "cashare-0.0.6.tar", last modified: Sat Jul 22 02:22:48 2023, max compression
```

## Comparing `cashare-0.0.5.tar` & `cashare-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 12:03:44.864579 cashare-0.0.5/
--rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      164 2023-06-05 12:03:44.863582 cashare-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 12:03:44.854606 cashare-0.0.5/cashare/
--rw-rw-rw-   0        0        0        0 2023-03-25 03:03:24.000000 cashare-0.0.5/cashare/__init__.py
--rw-rw-rw-   0        0        0     3277 2023-06-05 11:57:05.000000 cashare-0.0.5/cashare/day_data.py
--rw-rw-rw-   0        0        0       61 2023-06-04 12:22:16.000000 cashare-0.0.5/cashare/dname.py
--rw-rw-rw-   0        0        0     4343 2023-06-05 11:57:05.000000 cashare-0.0.5/cashare/minute_data.py
--rw-rw-rw-   0        0        0      445 2023-06-05 11:57:05.000000 cashare-0.0.5/cashare/stock_list.py
--rw-rw-rw-   0        0        0      438 2023-06-05 11:57:05.000000 cashare-0.0.5/cashare/stock_now.py
-drwxrwxrwx   0        0        0        0 2023-06-05 12:03:44.862585 cashare-0.0.5/cashare.egg-info/
--rw-rw-rw-   0        0        0      164 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 12:03:44.000000 cashare-0.0.5/cashare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 12:03:44.864579 cashare-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-06-05 12:03:20.000000 cashare-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:22:48.100953 cashare-0.0.6/
+-rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      164 2023-07-22 02:22:48.099956 cashare-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-25 03:03:23.000000 cashare-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 02:22:48.084249 cashare-0.0.6/cashare/
+-rw-rw-rw-   0        0        0        0 2023-03-25 03:03:24.000000 cashare-0.0.6/cashare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:22:48.095000 cashare-0.0.6/cashare/common/
+-rw-rw-rw-   0        0        0        0 2023-06-22 12:34:18.000000 cashare-0.0.6/cashare/common/__init__.py
+-rw-rw-rw-   0        0        0     3283 2023-07-10 13:15:21.000000 cashare-0.0.6/cashare/common/get_com.py
+-rw-rw-rw-   0        0        0     2998 2023-07-21 15:21:20.000000 cashare-0.0.6/cashare/common/get_data.py
+-rw-rw-rw-   0        0        0      393 2023-07-14 13:52:49.000000 cashare-0.0.6/cashare/common/var_date.py
+-rw-rw-rw-   0        0        0     3349 2023-07-21 15:24:56.000000 cashare-0.0.6/cashare/day_data.py
+-rw-rw-rw-   0        0        0       63 2023-07-21 15:34:56.000000 cashare-0.0.6/cashare/dname.py
+-rw-rw-rw-   0        0        0     4410 2023-07-21 15:24:56.000000 cashare-0.0.6/cashare/minute_data.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:22:48.098986 cashare-0.0.6/cashare/stock/
+-rw-rw-rw-   0        0        0        0 2023-06-22 12:23:20.000000 cashare-0.0.6/cashare/stock/__init__.py
+-rw-rw-rw-   0        0        0     1953 2023-07-21 15:39:25.000000 cashare-0.0.6/cashare/stock/c_data.py
+-rw-rw-rw-   0        0        0     2269 2023-07-21 15:24:56.000000 cashare-0.0.6/cashare/stock/c_min.py
+-rw-rw-rw-   0        0        0      650 2023-07-21 15:24:56.000000 cashare-0.0.6/cashare/stock_list.py
+-rw-rw-rw-   0        0        0      615 2023-07-21 15:25:23.000000 cashare-0.0.6/cashare/stock_now.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:22:48.091007 cashare-0.0.6/cashare.egg-info/
+-rw-rw-rw-   0        0        0      164 2023-07-22 02:22:47.000000 cashare-0.0.6/cashare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-07-22 02:22:48.000000 cashare-0.0.6/cashare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 02:22:47.000000 cashare-0.0.6/cashare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-22 02:22:47.000000 cashare-0.0.6/cashare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 02:22:47.000000 cashare-0.0.6/cashare.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 02:22:48.100953 cashare-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-07-22 02:22:35.000000 cashare-0.0.6/setup.py
```

### Comparing `cashare-0.0.5/cashare/day_data.py` & `cashare-0.0.6/cashare/common/get_com.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
             li = hg(sk_code, token=token, start_date=res[i], end_date=res[i+1])
             get_list.append(li)
         else:
             end=datetime.datetime.strptime(res[i+1], '%Y-%m-%d')-dateutil.relativedelta.relativedelta(days=1)
             li=hg(sk_code,token=token,start_date=res[i],end_date=end.strftime("%Y-%m-%d"))
             get_list.append(li)
 
-    # print(" dates : " + str(get_list))
-    # print(get_list)
+    # print(" dates : " + str(get_list.py))
+    # print(get_list.py)
     return get_list
 
 def url_get(url_list):
     import pandas as pd
     df = pd.DataFrame(data=None)
     for item in url_list:
         # print(item)
```

### Comparing `cashare-0.0.5/cashare/minute_data.py` & `cashare-0.0.6/cashare/minute_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import httpx
 from cashare.dname import url1
 import datetime
 import pandas as pd
 import dateutil.relativedelta
 import time
+from cashare.common.get_data import _retry_get
 def m_data(sk_code,type,token,end_date=str(datetime.date.today().strftime('%Y-%m-%d')),start_date='19000101',):
 
 
     if start_date > (datetime.date.today().strftime('%Y-%m-%d')):
         return "start_date大于现在时间"
     elif start_date > end_date:
         return "start_date大于end_date"
@@ -29,15 +30,15 @@
         return dan(start_date=start_date, end_date=end_date,type=type,sk_code=sk_code, token=token, x=95, y=89)
     else:
         return "输入type非法,请输入1min、5min、15min、30min、1hour、4hour"
 
 def dan(start_date,end_date,sk_code,token,x,y,type):
     if ri(start_date, end_date) <= x:
         li = hg(sk_code=sk_code, token=token, type=type, start_date=start_date, end_date=end_date)
-        r = httpx.get(li)
+        r = _retry_get(li,timeout=100)
         return pd.DataFrame(r.json())
     else:
 
         if ri(start_date, end_date) / y > int(ri(start_date, end_date) / y):
             n = (int(ri(start_date, end_date) / y) + 1)
         else:
             n = int(ri(start_date, end_date) / y)
@@ -74,38 +75,39 @@
             li = hg(sk_code, token=token, type=type, start_date=res[i], end_date=res[i+1])
             get_list.append(li)
         else:
             end=datetime.datetime.strptime(res[i+1], '%Y-%m-%d')-dateutil.relativedelta.relativedelta(days=1)
             li=hg(sk_code,token=token,type=type,start_date=res[i],end_date=end.strftime("%Y-%m-%d"))
             get_list.append(li)
 
-    # print(" dates : " + str(get_list))
-    # print(get_list)
+    # print(" dates : " + str(get_list.py))
+    # print(get_list.py)
     return get_list
 
 def url_get(url_list):
     import pandas as pd
     df = pd.DataFrame(data=None)
     for item in url_list:
         # print(item)
-        r = httpx.get(item,timeout=30)
+        r = _retry_get(item,timeout=100)
         # print(r.json())
+        # print(r.text)
         if pd.DataFrame(r.json()).empty:
            pass
         else:
             lsss = pd.DataFrame(r.json()).sort_values(by='date')  # 进行升序排序
             df = df.append(lsss, ignore_index=True)
             time.sleep(0.2)
             # print(df)
     df.drop_duplicates(subset='date', keep='first', inplace =True, ignore_index = True)#去重
-    # df.to_csv("34343.csv")
+
     return df
 
 if __name__ == '__main__':
 
-    df=m_data(sk_code="aapl",token='y0ad8f825bad3234ada0ab7ff56e1925372',type='30min',start_date='2022-03-02',end_date='2023-05-02')
+    df=m_data(sk_code="aapl",token='z9882e4b76023e40fb084c421f588ab864x3',type='30min',start_date='2022-03-02',end_date='2023-05-02')
     print(df)
     pass
```

