# Comparing `tmp/dasida-2023.7.3.tar.gz` & `tmp/dasida-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dasida-2023.7.3.tar", last modified: Sun Jul 16 11:09:05 2023, max compression
+gzip compressed data, was "dasida-2023.7.4.tar", last modified: Fri Jul 21 23:27:48 2023, max compression
```

## Comparing `dasida-2023.7.3.tar` & `dasida-2023.7.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.213165 dasida-2023.7.3/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1063 2023-07-16 11:07:17.000000 dasida-2023.7.3/LICENSE
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-16 11:09:05.213165 dasida-2023.7.3/PKG-INFO
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       34 2023-07-16 11:07:17.000000 dasida-2023.7.3/README.md
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.209165 dasida-2023.7.3/dasida/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       58 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/__init__.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.213165 dasida-2023.7.3/dasida/aws/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       99 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1680 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/common.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     8466 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/s3.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     9428 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/secretsmanager.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)    12353 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/sqs.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     4008 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/ssm.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.213165 dasida-2023.7.3/dasida/docker/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       33 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/docker/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1240 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/docker/docker.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     8713 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/scripts.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.209165 dasida-2023.7.3/dasida.egg-info/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      437 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)        1 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       49 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       79 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)        7 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/top_level.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      262 2023-07-16 11:07:17.000000 dasida-2023.7.3/pyproject.toml
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      437 2023-07-16 11:09:05.217165 dasida-2023.7.3/setup.cfg
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-21 23:27:48.415546 dasida-2023.7.4/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1063 2023-07-16 11:07:17.000000 dasida-2023.7.4/LICENSE
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-21 23:27:48.415546 dasida-2023.7.4/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       34 2023-07-16 11:07:17.000000 dasida-2023.7.4/README.md
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-21 23:27:48.415546 dasida-2023.7.4/dasida/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       58 2023-07-16 11:07:17.000000 dasida-2023.7.4/dasida/__init__.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-21 23:27:48.415546 dasida-2023.7.4/dasida/aws/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       99 2023-07-16 11:07:17.000000 dasida-2023.7.4/dasida/aws/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1681 2023-07-21 23:25:20.000000 dasida-2023.7.4/dasida/aws/common.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     8466 2023-07-16 11:07:17.000000 dasida-2023.7.4/dasida/aws/s3.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     9428 2023-07-16 11:07:17.000000 dasida-2023.7.4/dasida/aws/secretsmanager.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)    12353 2023-07-16 11:07:17.000000 dasida-2023.7.4/dasida/aws/sqs.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     4008 2023-07-16 11:07:17.000000 dasida-2023.7.4/dasida/aws/ssm.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-21 23:27:48.415546 dasida-2023.7.4/dasida/docker/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       33 2023-07-16 11:07:17.000000 dasida-2023.7.4/dasida/docker/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1240 2023-07-16 11:07:17.000000 dasida-2023.7.4/dasida/docker/docker.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     9989 2023-07-21 23:22:48.000000 dasida-2023.7.4/dasida/scripts.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-21 23:27:48.415546 dasida-2023.7.4/dasida.egg-info/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-21 23:27:48.000000 dasida-2023.7.4/dasida.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      437 2023-07-21 23:27:48.000000 dasida-2023.7.4/dasida.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        1 2023-07-21 23:27:48.000000 dasida-2023.7.4/dasida.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       49 2023-07-21 23:27:48.000000 dasida-2023.7.4/dasida.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       79 2023-07-21 23:27:48.000000 dasida-2023.7.4/dasida.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        7 2023-07-21 23:27:48.000000 dasida-2023.7.4/dasida.egg-info/top_level.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      262 2023-07-16 11:07:17.000000 dasida-2023.7.4/pyproject.toml
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      437 2023-07-21 23:27:48.419546 dasida-2023.7.4/setup.cfg
```

### Comparing `dasida-2023.7.3/LICENSE` & `dasida-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.3/dasida/aws/common.py` & `dasida-2023.7.4/dasida/aws/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     "aws_secret_access_key": None,
     "aws_session_token": None,
     "region_name": None,
     "botocore_session": None,
     "profile_name": None,
 }
 
+
 ################################################################
 # Helpers
 ################################################################
 # create client for SecretsManager
 def session_maker(
     profile_name=None,
     aws_access_key_id=None,
@@ -44,15 +45,15 @@
                     "aws_access_key_id": aws_access_key_id,
                     "aws_secret_access_key": aws_secret_access_key,
                 }
             )
     if profile_name is not None:
         session_opts = {"profile_name": profile_name}
 
-    # return clinet
+    # return client
     return boto3.session.Session(**session_opts)
 
 
 def validate_response(response, success_codes=[200]):
     meta = response["ResponseMetadata"]
     if meta["HTTPStatusCode"] not in success_codes:
         raise ReferenceError(f"status code {meta['HTTPStatusCode']}, {str(meta)}")
```

### Comparing `dasida-2023.7.3/dasida/aws/s3.py` & `dasida-2023.7.4/dasida/aws/s3.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.3/dasida/aws/secretsmanager.py` & `dasida-2023.7.4/dasida/aws/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.3/dasida/aws/sqs.py` & `dasida-2023.7.4/dasida/aws/sqs.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.3/dasida/aws/ssm.py` & `dasida-2023.7.4/dasida/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.3/dasida/docker/docker.py` & `dasida-2023.7.4/dasida/docker/docker.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.3/dasida/scripts.py` & `dasida-2023.7.4/dasida/scripts.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,17 +32,18 @@
 
 
 @secretsmanager.command()
 @click.argument("secret_name")
 @click.option("--profile", default=None)
 def get(secret_name, profile):
     secrets = aws.secretsmanager.get_secrets(secret_name=secret_name, profile_name=profile)
-    print(f"Secret '{secret_name}':")
-    for k, v in secrets.items():
-        print(f" - {k}: {v}")
+    if secrets:
+        print(f"Secret '{secret_name}':")
+        for k, v in secrets.items():
+            print(f" - {k}: {v}")
 
 
 @secretsmanager.command()
 @click.argument("secret_name")
 @click.option("--profile", default=None)
 def delete(secret_name, profile):
     _ = aws.secretsmanager.delete_secrets(secret_name=secret_name, profile_name=profile)
@@ -73,14 +74,49 @@
     proceed = inquirer.confirm(message="Confirm?", default=False).execute()
     if proceed:
         _ = aws.secretsmanager.create_secrets(secret_name=secret_name, secrets=secrets, profile_name=profile)
     else:
         logger.error("Abort!")
 
 
+@secretsmanager.command()
+@click.argument("secret_name")
+@click.option("--profile", default=None)
+def update(secret_name, profile):
+    secrets = aws.secretsmanager.get_secrets(secret_name=secret_name, profile_name=profile)
+    if not secrets:
+        msg = f"Secret name '{secret_name}' not found!"
+        raise KeyError(msg)
+
+    new_secrets = dict()
+    for k, v in secrets.items():
+        key = inquirer.text(message="Key:", default=k).execute()
+        value = inquirer.text(message="Value:", default=v).execute()
+        if value:
+            new_secrets.update({key: value})
+
+    while True:
+        proceed = inquirer.confirm(message="Add New Key-Value?").execute()
+        if not proceed:
+            break
+        key = inquirer.text(message="Key:").execute()
+        value = inquirer.text(message="Value:").execute()
+        new_secrets.update({key: value})
+
+    print(f"\nUpdate secret '{secret_name}' as follows?:")
+    for k, v in new_secrets.items():
+        print(f" - {k}: {v}")
+
+    proceed = inquirer.confirm(message="Confirm?", default=False).execute()
+    if proceed:
+        _ = aws.secretsmanager.update_secrets(secret_name=secret_name, secrets=new_secrets, profile_name=profile)
+    else:
+        logger.error("Abort!")
+
+
 ################################################################
 # AWS S3
 ################################################################
 @dasida.group()
 def s3():
     pass
```

