# Comparing `tmp/antisafelinks-1.0.2.tar.gz` & `tmp/antisafelinks-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antisafelinks-1.0.2.tar", last modified: Wed Jul 19 17:54:02 2023, max compression
+gzip compressed data, was "antisafelinks-1.1.tar", last modified: Sat Jul 22 16:55:36 2023, max compression
```

## Comparing `antisafelinks-1.0.2.tar` & `antisafelinks-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hawky      (501) staff       (20)        0 2023-07-19 17:54:02.703037 antisafelinks-1.0.2/
--rw-r--r--   0 hawky      (501) staff       (20)    35149 2023-06-15 09:29:18.000000 antisafelinks-1.0.2/LICENSE
--rw-r--r--   0 hawky      (501) staff       (20)     5409 2023-07-19 17:54:02.702926 antisafelinks-1.0.2/PKG-INFO
--rw-r--r--   0 hawky      (501) staff       (20)     4746 2023-07-19 17:09:15.000000 antisafelinks-1.0.2/README.md
--rw-r--r--   0 hawky      (501) staff       (20)      771 2023-07-19 17:53:52.000000 antisafelinks-1.0.2/pyproject.toml
--rw-r--r--   0 hawky      (501) staff       (20)       38 2023-07-19 17:54:02.703069 antisafelinks-1.0.2/setup.cfg
-drwxr-xr-x   0 hawky      (501) staff       (20)        0 2023-07-19 17:54:02.701629 antisafelinks-1.0.2/src/
-drwxr-xr-x   0 hawky      (501) staff       (20)        0 2023-07-19 17:54:02.702206 antisafelinks-1.0.2/src/antisafelinks/
--rw-r--r--   0 hawky      (501) staff       (20)      364 2023-07-19 17:51:34.000000 antisafelinks-1.0.2/src/antisafelinks/__init__.py
--rwxr-xr-x   0 hawky      (501) staff       (20)     9848 2023-07-19 17:51:47.000000 antisafelinks-1.0.2/src/antisafelinks/safelink_decoder.py
-drwxr-xr-x   0 hawky      (501) staff       (20)        0 2023-07-19 17:54:02.702755 antisafelinks-1.0.2/src/antisafelinks.egg-info/
--rw-r--r--   0 hawky      (501) staff       (20)     5409 2023-07-19 17:54:02.000000 antisafelinks-1.0.2/src/antisafelinks.egg-info/PKG-INFO
--rw-r--r--   0 hawky      (501) staff       (20)      308 2023-07-19 17:54:02.000000 antisafelinks-1.0.2/src/antisafelinks.egg-info/SOURCES.txt
--rw-r--r--   0 hawky      (501) staff       (20)        1 2023-07-19 17:54:02.000000 antisafelinks-1.0.2/src/antisafelinks.egg-info/dependency_links.txt
--rw-r--r--   0 hawky      (501) staff       (20)       53 2023-07-19 17:54:02.000000 antisafelinks-1.0.2/src/antisafelinks.egg-info/entry_points.txt
--rw-r--r--   0 hawky      (501) staff       (20)       14 2023-07-19 17:54:02.000000 antisafelinks-1.0.2/src/antisafelinks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:55:36.541409 antisafelinks-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-22 16:55:25.000000 antisafelinks-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-22 16:55:36.541409 antisafelinks-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-22 16:55:25.000000 antisafelinks-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-22 16:55:25.000000 antisafelinks-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:55:36.541409 antisafelinks-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:55:36.541409 antisafelinks-1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:55:36.541409 antisafelinks-1.1/src/antisafelinks/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-22 16:55:25.000000 antisafelinks-1.1/src/antisafelinks/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9178 2023-07-22 16:55:25.000000 antisafelinks-1.1/src/antisafelinks/safelink_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:55:36.541409 antisafelinks-1.1/src/antisafelinks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-22 16:55:36.000000 antisafelinks-1.1/src/antisafelinks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-22 16:55:36.000000 antisafelinks-1.1/src/antisafelinks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:55:36.000000 antisafelinks-1.1/src/antisafelinks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-22 16:55:36.000000 antisafelinks-1.1/src/antisafelinks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 16:55:36.000000 antisafelinks-1.1/src/antisafelinks.egg-info/top_level.txt
```

### Comparing `antisafelinks-1.0.2/LICENSE` & `antisafelinks-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antisafelinks-1.0.2/PKG-INFO` & `antisafelinks-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antisafelinks
-Version: 1.0.2
+Version: 1.1
 Summary: Removes the Microsoft SafeLinks from emails or Maildir folders
 Author-email: Benito Marcote <benito.marcote@icloud.com>
 Project-URL: Homepage, https://github.com/bmarcote/antisafelinks
 Project-URL: Bug Tracker, https://github.com/bmarcote/antisafelinks/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
```

### Comparing `antisafelinks-1.0.2/README.md` & `antisafelinks-1.1/README.md`

 * *Files identical despite different names*

### Comparing `antisafelinks-1.0.2/pyproject.toml` & `antisafelinks-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "antisafelinks"
-version = "1.0.2"
+version = "1.1"
 authors = [{name="Benito Marcote", email="benito.marcote@icloud.com"}]
 description = "Removes the Microsoft SafeLinks from emails or Maildir folders"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `antisafelinks-1.0.2/src/antisafelinks/safelink_decoder.py` & `antisafelinks-1.1/src/antisafelinks/safelink_decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,17 +104,14 @@
             except UnicodeDecodeError as e:
                 print(f"UnicodeDecodeError on email {message['Message-ID']}: {e}")
                 return None
 
     return message
 
 
-def this_is_a_test():
-    print("TEST")
-
 def recover_email_from_file(email_file: str, outfile: str = None, debug=False):
     """Given a file that should contain an RFC 2822-compliant message, it will modify back
     all links, if existing, in the body.
     """
     e = email.message_from_file(open(email_file, 'r'))
 
     if (new_e := recover_email(e, debug=debug)) is None:
@@ -183,17 +180,17 @@
 
 def main():
     """Runs the main AntiSafeLinks program as CLI.
     """
     description = """Recovers the original url links that have been modified by
     the shit Microsoft SafeLink tool.
     """
-    usage = "$(prog)s  [-h]  [-u/--url SafeLink-modified URL] " \
-            " [-e/--email email_file]  [-m/--maildir Maildir folder]"
-    parser = argparse.ArgumentParser(description=description, prog='safelink_decoder.py',
+    usage = "antisafelinks  [-h]  [-u/--url SafeLink-modified URL] " \
+            " [-e/--email email_file]  [-d/--dir folder]  [-m/--maildir Maildir folder]"
+    parser = argparse.ArgumentParser(description=description, prog='antisafelinks',
                                      usage=usage)
     parser.add_argument('-u', '--url', default=None, type=str,
                         help="URL fucked up by Microsoft that needs to be recovered. " \
                              "The output will be printed in STDOUT unless -o/--output is set.")
     parser.add_argument('-e', '--email', default=None, type=str,
                         help="Local email file to be parsed.")
     parser.add_argument('-m', '--maildir', default=None, type=str,
@@ -207,23 +204,15 @@
                         help="If given, it will only scan emails in the 'new' directory. " \
                              "Otherwise it will scan all new/cur/tmp folders.")
     parser.add_argument('--debug', default=False, action="store_true", help="More verbose output.")
 
     args = parser.parse_args()
 
     if (args.url, args.email, args.maildir, args.dir).count(None) != 3:
-        print("One and only one of the following options need to be set:")
-        print(" -e/--email - pointing to an existing file that may or may not contain " \
-              "M$croso$t fucked-up links.")
-        print(" -m/--maildir- pointing to an existing Maildir folder whose emails need to " \
-              "be corrected from M$croso$t fucked up links.")
-        print(" -d/--dir- pointing to an existing folder incluidng Maildir subfolders whose " \
-              "emails need to be corrected from M$croso$t fucked up links.")
-        print(" -u/--url - passing a url that has been fucked up by M$croso$t SafeLink tool.")
-        print("Run me with -h for more help.")
+        print(f"usage: {usage}")
         sys.exit(0)
 
     if args.url is not None:
         print(recover_link(args.url))
     elif args.dir is not None:
         main_dir = Path(args.dir)
         if main_dir.exists():
```

### Comparing `antisafelinks-1.0.2/src/antisafelinks.egg-info/PKG-INFO` & `antisafelinks-1.1/src/antisafelinks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antisafelinks
-Version: 1.0.2
+Version: 1.1
 Summary: Removes the Microsoft SafeLinks from emails or Maildir folders
 Author-email: Benito Marcote <benito.marcote@icloud.com>
 Project-URL: Homepage, https://github.com/bmarcote/antisafelinks
 Project-URL: Bug Tracker, https://github.com/bmarcote/antisafelinks/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
```

