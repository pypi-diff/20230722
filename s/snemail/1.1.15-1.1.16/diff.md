# Comparing `tmp/snemail-1.1.15.tar.gz` & `tmp/snemail-1.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snemail-1.1.15.tar", last modified: Wed Apr 12 04:55:14 2023, max compression
+gzip compressed data, was "snemail-1.1.16.tar", last modified: Sat Jul 22 14:55:43 2023, max compression
```

## Comparing `snemail-1.1.15.tar` & `snemail-1.1.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 04:55:14.858827 snemail-1.1.15/
--rw-rw-rw-   0        0        0     1091 2023-04-10 02:22:39.000000 snemail-1.1.15/LICENSE
--rw-rw-rw-   0        0        0     4002 2023-04-12 04:55:14.857830 snemail-1.1.15/PKG-INFO
--rw-rw-rw-   0        0        0     3594 2023-04-10 02:22:39.000000 snemail-1.1.15/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 04:55:14.858827 snemail-1.1.15/setup.cfg
--rw-rw-rw-   0        0        0     1042 2023-04-12 04:54:47.000000 snemail-1.1.15/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 04:55:14.836802 snemail-1.1.15/snemail/
--rw-rw-rw-   0        0        0       22 2023-04-10 02:22:39.000000 snemail-1.1.15/snemail/__init__.py
--rw-rw-rw-   0        0        0     7662 2023-04-12 04:54:39.000000 snemail-1.1.15/snemail/package.py
-drwxrwxrwx   0        0        0        0 2023-04-12 04:55:14.854866 snemail-1.1.15/snemail.egg-info/
--rw-rw-rw-   0        0        0     4002 2023-04-12 04:55:14.000000 snemail-1.1.15/snemail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-12 04:55:14.000000 snemail-1.1.15/snemail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 04:55:14.000000 snemail-1.1.15/snemail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 04:55:14.000000 snemail-1.1.15/snemail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 04:55:14.856833 snemail-1.1.15/test/
--rw-rw-rw-   0        0        0      573 2023-04-10 03:33:26.000000 snemail-1.1.15/test/test_demp.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:55:43.903536 snemail-1.1.16/
+-rw-rw-rw-   0        0        0     1091 2023-07-22 14:39:52.000000 snemail-1.1.16/LICENSE
+-rw-rw-rw-   0        0        0     4002 2023-07-22 14:55:43.902534 snemail-1.1.16/PKG-INFO
+-rw-rw-rw-   0        0        0     3594 2023-07-22 14:39:52.000000 snemail-1.1.16/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-22 14:55:43.903536 snemail-1.1.16/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2023-07-22 14:39:52.000000 snemail-1.1.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:55:43.888541 snemail-1.1.16/snemail/
+-rw-rw-rw-   0        0        0       22 2023-07-22 14:39:52.000000 snemail-1.1.16/snemail/__init__.py
+-rw-rw-rw-   0        0        0     7992 2023-07-22 14:39:52.000000 snemail-1.1.16/snemail/package.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:55:43.898539 snemail-1.1.16/snemail.egg-info/
+-rw-rw-rw-   0        0        0     4002 2023-07-22 14:55:43.000000 snemail-1.1.16/snemail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-07-22 14:55:43.000000 snemail-1.1.16/snemail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 14:55:43.000000 snemail-1.1.16/snemail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 14:55:43.000000 snemail-1.1.16/snemail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 14:55:43.900536 snemail-1.1.16/test/
+-rw-rw-rw-   0        0        0      616 2023-07-22 14:39:52.000000 snemail-1.1.16/test/test_demp.py
```

### Comparing `snemail-1.1.15/LICENSE` & `snemail-1.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `snemail-1.1.15/PKG-INFO` & `snemail-1.1.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.15
+Version: 1.1.16
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.15/README.md` & `snemail-1.1.16/README.md`

 * *Files identical despite different names*

### Comparing `snemail-1.1.15/setup.py` & `snemail-1.1.16/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="snemail",
-    version="1.1.15",
+    version="1.1.16",
     author="manji",
     author_email="pnsm@qq.com",                         # 作者邮箱
     description="发送邮件库",                            # 模块简介
     long_description=long_description,                  # 模块详细介绍
     long_description_content_type="text/markdown",      # 模块详细介绍格式
     url="https://github.com/majormj/sendmail",
     packages=setuptools.find_packages(),                # 自动找到项目中导入的模块
```

### Comparing `snemail-1.1.15/snemail/package.py` & `snemail-1.1.16/snemail/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,35 +29,41 @@
 
         # 2、准备数据 
         # 1）创建邮件对象 MIMEMultipart（‘mixed’）类型；
         # MIMEMultipart(‘alternative’)；MIMEMultipart(‘related’)类型
     
         self.msg = MIMEMultipart() 
 
-    def mail_login(self,user="",password=""):
+    def mail_login(self,user="",password="",ifssl=True):
         """登录邮箱"""
 
         self.emailCome = user       # 邮件的时间发送人（发邮件的时候调用）
         self.loginStatus = False    # 登录结果状态
         try:
-            # 1、链接邮箱服务器(带 SSL 启用安全机制) # 端口号：465/25
-            # 1.1 判断python版本
-            vamax = sys.version_info.major   #  大版本号例如3.6.8  则表示3
-            vsmin = sys.version_info.minor   #  小版本号例如3.6.8  则表示6
-
-            if vamax == 3 and vsmin < 10:  #  python 版本号大于3
-
-                self.con = smtplib.SMTP_SSL(self.server,self.port) 
-
+            if ifssl:
+                print("ifssl的值",ifssl,"启用SSL验证")
+                # 1、链接邮箱服务器(带 SSL 启用安全机制) # 端口号：465/25
+                # 1.1 判断python版本
+                vamax = sys.version_info.major   #  大版本号例如3.6.8  则表示3
+                vsmin = sys.version_info.minor   #  小版本号例如3.6.8  则表示6
+
+                if vamax == 3 and vsmin < 10:  #  python 版本号大于3
+
+                    self.con = smtplib.SMTP_SSL(self.server,self.port) 
+
+                else:
+                    """ Python 3.10 及以上版本使用"""
+                    import ssl
+                    ctx = ssl.create_default_context()
+                    ctx.set_ciphers('DEFAULT')
+                    self.con = smtplib.SMTP_SSL(self.server,port=self.port, context = ctx)
             else:
-                """ Python 3.10 及以上版本使用"""
-                import ssl
-                ctx = ssl.create_default_context()
-                ctx.set_ciphers('DEFAULT')
-                self.con = smtplib.SMTP_SSL(self.server,port=self.port, context = ctx)
+                print("ifssl的值",ifssl,"不启用验证")
+                self.con = smtplib.SMTP('smtp.office365.com', 587)
+                self.con.starttls()
 
             # 2、登录邮箱 # 链接对象.login(账号、密码)
             self.con.login(user,password) 
             self.loginStatus = True
             return '邮箱登录成功'
         except SMTPAuthenticationError as e:
             return '登录失败，请检查账户密码是否正确，或者尝试授权码登录%s'%repr(e)
```

### Comparing `snemail-1.1.15/snemail.egg-info/PKG-INFO` & `snemail-1.1.16/snemail.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snemail
-Version: 1.1.15
+Version: 1.1.16
 Summary: 发送邮件库
 Home-page: https://github.com/majormj/sendmail
 Author: manji
 Author-email: pnsm@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snemail-1.1.15/test/test_demp.py` & `snemail-1.1.16/test/test_demp.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,7 +18,14 @@
     sn.mail_file([r"C:\Users\manji\Downloads\全量商品列表.xlsx"])
 
     # 登录邮箱
     print(sn.mail_login(user="",password=""))
 
     # 发送邮件
     print(sn.mail_send(emailTo=[]))
+
+
+def uu():
+    """
+    
+    
+    """
```

