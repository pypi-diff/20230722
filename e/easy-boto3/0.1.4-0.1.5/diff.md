# Comparing `tmp/easy_boto3-0.1.4.tar.gz` & `tmp/easy_boto3-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_boto3-0.1.4.tar", max compression
+gzip compressed data, was "easy_boto3-0.1.5.tar", max compression
```

## Comparing `easy_boto3-0.1.4.tar` & `easy_boto3-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/LICENSE
--rw-r--r--   0        0        0     7805 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/README.md
--rw-r--r--   0        0        0       21 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/.easy_boto3_internal.yaml
--rw-r--r--   0        0        0      751 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/cloudwatch/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/cloudwatch/cloudwatch_alarm_management.py
--rw-r--r--   0        0        0     1395 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/cloudwatch/create.py
--rw-r--r--   0        0        0     1463 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/cloudwatch/delete.py
--rw-r--r--   0        0        0      878 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/cloudwatch/list.py
--rw-r--r--   0        0        0     1015 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/__init__.py
--rw-r--r--   0        0        0     3436 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/config_parser.py
--rw-r--r--   0        0        0     3061 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/connect.py
--rw-r--r--   0        0        0     1724 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/create.py
--rw-r--r--   0        0        0     2586 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/ec2_connections_management.py
--rw-r--r--   0        0        0     1494 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/ec2_instance_management.py
--rw-r--r--   0        0        0     1741 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/list.py
--rw-r--r--   0        0        0     1487 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/logs.py
--rw-r--r--   0        0        0     3657 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/script.py
--rw-r--r--   0        0        0     2426 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/ssh.py
--rw-r--r--   0        0        0      689 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/start.py
--rw-r--r--   0        0        0      642 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/stop.py
--rw-r--r--   0        0        0        0 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/stop_all.py
--rw-r--r--   0        0        0      892 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/ec2/terminate.py
--rw-r--r--   0        0        0    10078 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/main.py
--rw-r--r--   0        0        0        0 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/profile/__init__.py
--rw-r--r--   0        0        0     1869 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/profile/profile.py
--rw-r--r--   0        0        0      895 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/setup_session.py
--rw-r--r--   0        0        0        0 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/utilities/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/utilities/aws_profile_parser.py
--rw-r--r--   0        0        0     2471 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/utilities/decorators.py
--rw-r--r--   0        0        0     1270 2023-07-19 22:34:06.759482 easy_boto3-0.1.4/easy_boto3/utilities/logger_maker.py
--rw-r--r--   0        0        0     1013 2023-07-19 22:34:06.763482 easy_boto3-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     8956 1970-01-01 00:00:00.000000 easy_boto3-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/LICENSE
+-rw-r--r--   0        0        0     8710 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/README.md
+-rw-r--r--   0        0        0     1030 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/cloudwatch/__init__.py
+-rw-r--r--   0        0        0     1398 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/cloudwatch/create.py
+-rw-r--r--   0        0        0     1463 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/cloudwatch/delete.py
+-rw-r--r--   0        0        0      878 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/cloudwatch/list.py
+-rw-r--r--   0        0        0     1015 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/__init__.py
+-rw-r--r--   0        0        0     3439 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/config_parser.py
+-rw-r--r--   0        0        0     3554 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/connect.py
+-rw-r--r--   0        0        0     1724 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/create.py
+-rw-r--r--   0        0        0     2586 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/ec2_connections_management.py
+-rw-r--r--   0        0        0     1494 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/ec2_instance_management.py
+-rw-r--r--   0        0        0     1741 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/list.py
+-rw-r--r--   0        0        0     1487 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/logs.py
+-rw-r--r--   0        0        0     3657 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/script.py
+-rw-r--r--   0        0        0     2427 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/ssh.py
+-rw-r--r--   0        0        0      689 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/start.py
+-rw-r--r--   0        0        0      642 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/stop.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/stop_all.py
+-rw-r--r--   0        0        0      892 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/terminate.py
+-rw-r--r--   0        0        0    11965 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/main.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/profile/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/profile/active.py
+-rw-r--r--   0        0        0     3311 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/profile/ownership.py
+-rw-r--r--   0        0        0     1477 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/profile/validation.py
+-rw-r--r--   0        0        0      877 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/setup_session.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/utilities/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-22 21:11:16.952674 easy_boto3-0.1.5/easy_boto3/utilities/aws_profile_parser.py
+-rw-r--r--   0        0        0     2471 2023-07-22 21:11:16.952674 easy_boto3-0.1.5/easy_boto3/utilities/decorators.py
+-rw-r--r--   0        0        0     1270 2023-07-22 21:11:16.952674 easy_boto3-0.1.5/easy_boto3/utilities/logger_maker.py
+-rw-r--r--   0        0        0     1013 2023-07-22 21:11:16.952674 easy_boto3-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     9861 1970-01-01 00:00:00.000000 easy_boto3-0.1.5/PKG-INFO
```

### Comparing `easy_boto3-0.1.4/LICENSE` & `easy_boto3-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/README.md` & `easy_boto3-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,42 @@
 `easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file.
 
 ### Contents
 - [`boto3` made easy](#boto3-made-easy)
     - [Contents](#contents)
   - [Installation](#installation)
   - [Using `easy_boto3` CLI](#using-easy_boto3-cli)
-    - [Creating an ec2 instance with cloudwatch alarm](#creating-an-ec2-instance-with-cloudwatch-alarm)
-    - [Show instance cloud\_init logs](#show-instance-cloud_init-logs)
-    - [Show instance syslog logs](#show-instance-syslog-logs)
-    - [Listing ec2 instances](#listing-ec2-instances)
-    - [Stopping an ec2 instance](#stopping-an-ec2-instance)
-    - [Starting a stopped an ec2 instance](#starting-a-stopped-an-ec2-instance)
-    - [Termianting ec2 instances by id](#termianting-ec2-instances-by-id)
+    - [Managing ec2 instances](#managing-ec2-instances)
+      - [Creating an ec2 instance with cloudwatch alarm](#creating-an-ec2-instance-with-cloudwatch-alarm)
+      - [Show instance cloud\_init logs](#show-instance-cloud_init-logs)
+      - [Show instance syslog logs](#show-instance-syslog-logs)
+      - [Listing ec2 instances](#listing-ec2-instances)
+      - [Stopping an ec2 instance](#stopping-an-ec2-instance)
+      - [Starting a stopped an ec2 instance](#starting-a-stopped-an-ec2-instance)
+      - [Termianting ec2 instances by id](#termianting-ec2-instances-by-id)
+    - [Managing AWS profiles](#managing-aws-profiles)
+      - [List all AWS profiles in `~/.aws/credentials`](#list-all-aws-profiles-in-awscredentials)
+      - [List active AWS profile (currently used by `easy_boto3`)](#list-active-aws-profile-currently-used-by-easy_boto3)
+      - [Set active AWS profile (currently used by `easy_boto3`)](#set-active-aws-profile-currently-used-by-easy_boto3)
   - [Using `easy_boto3`'s Python API](#using-easy_boto3s-python-api)
     - [Creating an ec2 instance](#creating-an-ec2-instance)
 
 ## Installation 
 
 You can install `easy_boto3` via `pip` as
 
 ```bash
 pip install easy-boto3
 ```
 
 ## Using `easy_boto3` CLI
 
-### Creating an ec2 instance with cloudwatch alarm
+### Managing ec2 instances
+
+#### Creating an ec2 instance with cloudwatch alarm
 
 `easy_boto3` allows you to translate a standard `boto3` pythonic infrastructure task like instantiating an `ec2` instance with an attached `cloudwatch` cpu usage alarm from complex pythonic implementation like the following 
 
 ```python
 import boto3
 
 # read in aws_access_key_id and aws_secret_access_key based on input profile_name using boto3
@@ -136,27 +143,27 @@
 
 Using `easy_boto3` and this configuration `config.yaml` the same task - instantiating an `ec2` instance - can be accomplished via the command line as follows:
 
 ```bash
 easy_boto3 ec2 create config.yaml
 ```
 
-### Show instance cloud_init logs
+#### Show instance cloud_init logs
 
 ```bash
 easy_boto3 ec2 check_cloud_init_logs <instance_id>
 ```
 
-### Show instance syslog logs
+#### Show instance syslog logs
 
 ```bash
 easy_boto3 ec2 check_syslog <instance_id>
 ```
 
-### Listing ec2 instances 
+#### Listing ec2 instances 
 
 You can use `easy_boto3` to easy see (all/ running / stopped / terminated) instances in your AWS account as follows.
 
 See all instances
 
 ```bash
 easy_boto3 ec2 list_all
@@ -185,35 +192,58 @@
 easy_boto3 ec2 list_stopped
 ```
 
 ```bash
 easy_boto3 ec2 list_terminated
 ```
 
-### Stopping an ec2 instance
+#### Stopping an ec2 instance
 ```bash
 easy_boto3 ec2 stop <instance_id>
 ```
 
-### Starting a stopped an ec2 instance
+#### Starting a stopped an ec2 instance
 ```bash
 easy_boto3 ec2 start <instance_id>
 ```
 
 
-### Termianting ec2 instances by id  
+#### Termianting ec2 instances by id  
 
 You can use `easy_boto3` CLI to terminate an ec2 instance by id as follows
 
 ```bash
 easy_boto3 ec2 terminate <instance_id>
 ```
 
 Note: by default this will delete any cloudwatch alarms associated with the instance.
 
+### Managing AWS profiles
+
+You can use `easy_boto3` CLI to manage AWS profiles as follows
+
+
+#### List all AWS profiles in `~/.aws/credentials`
+
+```bash
+easy_boto3 profile list_all
+```
+
+#### List active AWS profile (currently used by `easy_boto3`)
+
+```bash
+easy_boto3 profile list_active 
+```
+
+#### Set active AWS profile (currently used by `easy_boto3`)
+
+```bash
+easy_boto3 profile set <profile_name>
+```
+
 
 ## Using `easy_boto3`'s Python API
 
 In addition to config driven command line use, `easy_boto3` also offers a simplified python API that makes creating and managing AWS resources with `boto3` easier.
 
 ### Creating an ec2 instance
```

### Comparing `easy_boto3-0.1.4/easy_boto3/cloudwatch/create.py` & `easy_boto3-0.1.5/easy_boto3/cloudwatch/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from easy_boto3.setup_session import setup
 session_auth = setup()
 
 
 @session_auth
 def create_cpu_alarm(instance_id=None,
                      ComparisonOperator='GreaterThanOrEqualToThreshold',
-                     EvaluationPeriods=1,
+                     EvaluationPeriods=10,
                      MetricName='CPUUtilization',
                      Namespace='AWS/EC2',
                      Period=60,
                      Statistic='Average',
-                     Threshold=70,
+                     Threshold=99.9,
                      session=None):
     # create ec2 controller from session
     ec2_client = session.client('ec2')
     cloudwatch_client = session.client('cloudwatch')
 
     # create instance_id stamped alarm name
     AlarmName = '{}-{}'.format('cpu_alarm', instance_id)
```

### Comparing `easy_boto3-0.1.4/easy_boto3/cloudwatch/delete.py` & `easy_boto3-0.1.5/easy_boto3/cloudwatch/delete.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/cloudwatch/list.py` & `easy_boto3-0.1.5/easy_boto3/cloudwatch/list.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/__init__.py` & `easy_boto3-0.1.5/easy_boto3/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/config_parser.py` & `easy_boto3-0.1.5/easy_boto3/ec2/config_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import yaml
 from easy_boto3.ec2.script import read_startup_script, inject_aws_creds, add_ssh_forwarding, add_github_host
-from easy_boto3.profile.profile import check_credentials
+from easy_boto3.profile.validation import check_credentials
 
 
 def parse(base_config):
     # read in base_config
     with open(base_config, 'r') as stream:
         try:
             base_config = yaml.safe_load(stream)
```

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/connect.py` & `easy_boto3-0.1.5/easy_boto3/ec2/ec2_connections_management.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-from easy_boto3.setup_session import setup
-session_auth = setup()
+import os, time
+from easy_boto3 import session_auth
 import paramiko
-import time
-import os
 import logging
 logging.getLogger("paramiko").setLevel(logging.CRITICAL)
 
 
-@session_auth
-def get_public_ip(instance_id, session=None):
-    # create ec2 controller from session
-    ec2_controller = session.client('ec2')
-
-    # get instance public ip
-    response = ec2_controller.describe_instances(InstanceIds=[instance_id])
-    return response['Reservations'][0]['Instances'][0]['PublicIpAddress']
-
-
-@session_auth
-def add_instance_to_known_hosts(instance_ip,
-                                username,
-                                key_name):
+def add_instance_to_known_hosts(instance_ip):
     # connect to instance
     username = 'ubuntu'
-    key_path = '/Users/wattjer/.ssh/shiftsmart_transcript_west_2.pem' 
+    key_path = '/Users/wattjer/.ssh/shiftsmart_transcript_west_2.pem'
     ec2_public_ip = instance_ip
 
     # Create an SSH client
     ssh_client = paramiko.SSHClient()
     ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     # Connect to the EC2 instance
@@ -41,24 +26,23 @@
         try:
             ssh_transport = paramiko.transport.Transport('%s:%s' % (instance_ip, 22))
             inner_options = ssh_transport.get_security_options()
             inner_options.key_types = (key_type,)
 
             ssh_transport.start_client()
             key = ssh_transport.get_remote_server_key()
-            ssh_transport.close()   
+            ssh_transport.close()
 
             name = key.get_name()
             if name not in all_names:
                 all_names.add(name)
                 all_keys.append(key)
         except:
             pass
 
-
     # Add the remote server's public keys to the local known_hosts file    
     home_dir = os.path.expanduser("~")
     known_hosts_path = os.path.join(home_dir, '.ssh', 'known_hosts')
 
     with open(known_hosts_path, 'a') as known_hosts_file:
         for key in all_keys:
             message = f'{instance_ip} {key.get_name()} {key.get_base64()}\n'
@@ -78,23 +62,23 @@
     ssh_client = paramiko.SSHClient()
     ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     # Connect to the EC2 instance
     ssh_client.connect(instance_ip, username=username, key_filename=key_path)
 
 
-# try test_connect every 10 seconds
+# try test_connect every 10 seconds 
 def test_connection(instance_ip):
     max_count = 10
     while True:
         try:
             add_instance_to_known_hosts(instance_ip)
             print('addition to known hosts successful')
             break
         except:
             time.sleep(10)
             print('trying again')
-            
+
         max_count -= 1
         if max_count == 0:
             print('max count reached')
-            break
+            break
```

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/create.py` & `easy_boto3-0.1.5/easy_boto3/ec2/create.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/ec2_connections_management.py` & `easy_boto3-0.1.5/easy_boto3/ec2/connect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,46 @@
-import os, time
-from easy_boto3 import session_auth
+from easy_boto3.profile.ownership import lookup_public_ip
+from easy_boto3.setup_session import setup
+session_auth = setup()
 import paramiko
+import time
+import os
 import logging
 logging.getLogger("paramiko").setLevel(logging.CRITICAL)
 
 
-def add_instance_to_known_hosts(instance_ip):
+@session_auth
+def get_public_ip(instance_id, session=None):
+    # create ec2 controller from session
+    ec2_controller = session.client('ec2')
+
+    # collect response from aws based on instance_id
+    response = ec2_controller.describe_instances(InstanceIds=[instance_id])
+
+    # cut out instance data
+    instance_data = response['Reservations'][0]['Instances'][0]
+
+    # if PublicIpAddress is present as key, return its value
+    if 'PublicIpAddress' in instance_data.keys():
+        return instance_data['PublicIpAddress']         
+    else:
+        # try loading public ip from instance_id_profile_pairs_path via instance_id
+        public_ip = lookup_public_ip(instance_id)
+        if public_ip is not None:
+            return public_ip
+    return None
+
+
+@session_auth
+def add_instance_to_known_hosts(instance_ip,
+                                username,
+                                key_name):
     # connect to instance
     username = 'ubuntu'
-    key_path = '/Users/wattjer/.ssh/shiftsmart_transcript_west_2.pem'
+    key_path = '/Users/wattjer/.ssh/shiftsmart_transcript_west_2.pem' 
     ec2_public_ip = instance_ip
 
     # Create an SSH client
     ssh_client = paramiko.SSHClient()
     ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     # Connect to the EC2 instance
@@ -26,23 +54,24 @@
         try:
             ssh_transport = paramiko.transport.Transport('%s:%s' % (instance_ip, 22))
             inner_options = ssh_transport.get_security_options()
             inner_options.key_types = (key_type,)
 
             ssh_transport.start_client()
             key = ssh_transport.get_remote_server_key()
-            ssh_transport.close()
+            ssh_transport.close()   
 
             name = key.get_name()
             if name not in all_names:
                 all_names.add(name)
                 all_keys.append(key)
         except:
             pass
 
+
     # Add the remote server's public keys to the local known_hosts file    
     home_dir = os.path.expanduser("~")
     known_hosts_path = os.path.join(home_dir, '.ssh', 'known_hosts')
 
     with open(known_hosts_path, 'a') as known_hosts_file:
         for key in all_keys:
             message = f'{instance_ip} {key.get_name()} {key.get_base64()}\n'
@@ -62,23 +91,23 @@
     ssh_client = paramiko.SSHClient()
     ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     # Connect to the EC2 instance
     ssh_client.connect(instance_ip, username=username, key_filename=key_path)
 
 
-# try test_connect every 10 seconds 
+# try test_connect every 10 seconds
 def test_connection(instance_ip):
     max_count = 10
     while True:
         try:
             add_instance_to_known_hosts(instance_ip)
             print('addition to known hosts successful')
             break
         except:
             time.sleep(10)
             print('trying again')
-
+            
         max_count -= 1
         if max_count == 0:
             print('max count reached')
-            break
+            break
```

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/ec2_instance_management.py` & `easy_boto3-0.1.5/easy_boto3/ec2/ec2_instance_management.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/list.py` & `easy_boto3-0.1.5/easy_boto3/ec2/list.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/logs.py` & `easy_boto3-0.1.5/easy_boto3/ec2/logs.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/script.py` & `easy_boto3-0.1.5/easy_boto3/ec2/script.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/ssh.py` & `easy_boto3-0.1.5/easy_boto3/ec2/ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 def delete_host(host,
                 session=None):
     # delete host from ssh config
     config = create_config_object()
     config.remove(host)
     config.save()
 
+
 @session_auth
 def lookup_host_data_by_hostname(instance_ip,
                                  session=None):
 
     # get ssh config 
     config = create_config_object()
```

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/start.py` & `easy_boto3-0.1.5/easy_boto3/ec2/start.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/stop.py` & `easy_boto3-0.1.5/easy_boto3/ec2/stop.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/ec2/terminate.py` & `easy_boto3-0.1.5/easy_boto3/ec2/terminate.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/main.py` & `easy_boto3-0.1.5/easy_boto3/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
-from easy_boto3.profile import profile
+from easy_boto3.profile import ownership, validation, active
 from easy_boto3.ec2.config_parser import parse as ec2_config_parser
-from easy_boto3.ec2.ssh import add_host, delete_host_by_hostname, lookup_host_data_by_hostname
+from easy_boto3.ec2.ssh import add_host, delete_host_by_hostname, lookup_host_data_by_hostname, delete_host
 from easy_boto3.ec2.create import create_instance
 from easy_boto3.ec2.stop import stop_instance
 from easy_boto3.ec2.terminate import terminate_instance
 from easy_boto3.ec2.start import start_instance
 from easy_boto3.ec2.list import list_all, list_running, list_stopped
 from easy_boto3.ec2.logs import check_cloud_init_logs, check_syslog
 from easy_boto3.cloudwatch.create import create_cpu_alarm
@@ -28,20 +28,28 @@
 
         self.create_cpu_alarm = create_cpu_alarm
         self.list_all_alarms = list_alarms
         self.list_instance_alarms = list_instance_alarms
         self.delete_alarm = delete_alarm
 
     def profile(self, sub_operation, **kwargs):
-        if sub_operation == "set":
-            return profile.set(**kwargs)
-        if sub_operation == "check":
-            return profile.check(**kwargs)
+        if sub_operation == "add":
+            return ownership.add_ownership_data(**kwargs)
+        if sub_operation == "delete":
+            return ownership.delete_ownership_data(**kwargs)
+        if sub_operation == "change_state":
+            return ownership.change_ownership_state(**kwargs)
         if sub_operation == "validate":
-            return profile.validate(**kwargs)
+            return validation.validate(**kwargs)
+        if sub_operation == "list_all":
+            return validation.list_all_profiles(**kwargs)
+        if sub_operation == "set":
+            return active.set_active_profile(**kwargs)
+        if sub_operation == "list_active":
+            return active.list_active_profile(**kwargs)
 
     def ec2(self, sub_operation, **kwargs):
         if sub_operation == "create":
             return self.create_instance(**kwargs)
         elif sub_operation == "stop":
             return self.stop_instance(**kwargs)
         elif sub_operation == "start":
@@ -88,59 +96,95 @@
     def process_four_arguments(self):
         if self.args[1] == "ec2":
             if self.args[2] == "create" and ".yaml" in self.args[3]:
                 config = self.args[3]
                 self.create_ec2_instance(config)
             elif self.args[2] == "stop":
                 instance_id = self.args[3]
+
+                # stop instance
                 self.stop_ec2_instance(instance_id)
+
+                # adjust instance state in file
+                self.easy_boto3.profile("change_state", instance_id=instance_id, new_state="stopped")
+
             elif self.args[2] == "terminate":
                 instance_id = self.args[3]
+
+                # terminate instance
                 self.terminate_ec2_instance(instance_id)
+
+                # delete profile entry
+                self.easy_boto3.profile("delete", instance_id=instance_id)
+
             elif self.args[2] == "start":
                 instance_id = self.args[3]
+
+                # start instance
                 self.start_ec2_instance(instance_id)
+
+                # adjust instance state in file
+                self.easy_boto3.profile("change_state", instance_id=instance_id, new_state="running")
+
             elif self.args[2] == "check_cloud_init_logs":
                 instance_id = self.args[3]
                 self.check_cloud_init_logs(instance_id)
             elif self.args[2] == "check_syslog":
                 instance_id = self.args[3]
                 self.check_syslog(instance_id)
         elif self.args[1] == 'alarm':
             if self.args[2] == 'list_instance':
                 instance_id = self.args[3]
                 self.list_alarm_instance(instance_id)
             else:
                 print(f"Invalid sub-operation '{self.args[2]}' for 'alarm'")
+        elif self.args[1] == 'profile':
+            if self.args[2] == 'set':
+                profile_name = self.args[3]
+                self.easy_boto3.profile("set", profile_name=profile_name)
         else:
             print(f"Invalid operation / sub-operation '{self.args}'")
 
     def process_three_arguments(self):
         if self.args[1] == "ec2":
             if 'list' in self.args[2]:
                 self.list_ec2_instances(self.args[2])
             else:
                 print(f"Invalid sub-operation '{self.args[2]}' for 'ec2'")
         elif self.args[1] == 'alarm':
             if self.args[2] == 'list_all':
                 self.list_all_alarms()
             else:
                 print(f"Invalid sub-operation '{self.args[2]}' for 'alarm'")
+        elif self.args[1] == 'profile':
+            if self.args[2] == 'list_active':
+                self.easy_boto3.profile("list_active")
+            elif self.args[2] == 'list_all':
+                self.easy_boto3.profile("list_all")
+            else:
+                print(f"Invalid sub-operation '{self.args[2]}' for 'profile'")
+
 
     def create_ec2_instance(self, config):
         # readin config file
         profile_name, ec2_instance_details, alarm_instance_details, ssh_instance_details = ec2_config_parser(config)
 
         # set aws profile name
-        self.easy_boto3.profile("set", profile_name=profile_name)
+        self.easy_boto3.profile("validate", profile_name=profile_name)
 
         # create ec2 instance
         launch_details = self.easy_boto3.ec2("create", **ec2_instance_details)
         print(f"Instance created - instance_id = {launch_details.id} and public_ip = {launch_details.public_ip}")
 
+        # record instance_id / profile pair in ~/.easy_boto3/instance_profile_pairs.yaml
+        self.easy_boto3.profile("add",
+                                instance_id=launch_details.id, 
+                                public_ip=launch_details.public_ip, 
+                                profile_name=profile_name)
+
         # unpack ssh_details
         ssh_config_settings = ssh_instance_details['Config']
         ssh_options = ssh_instance_details['Options']
 
         # set host if present in config
         host = None
         if 'Host' in list(ssh_config_settings.keys()):
@@ -216,21 +260,22 @@
         stop_details = self.easy_boto3.ec2("stop", instance_id=instance_id)
 
     def start_ec2_instance(self, instance_id):
         start_details = self.easy_boto3.ec2("start", instance_id=instance_id)
 
     def terminate_ec2_instance(self, instance_id):
         # lookup public_ip associated with instance_id
-        instance_ip = get_public_ip(instance_id)
+        # instance_ip = get_public_ip(instance_id)
 
         # delete instance and alarm associated with instance_id
         terminate_details = self.easy_boto3.ec2("terminate", instance_id=instance_id)
 
         # delete entry in ~/.easy_boto3/ssh_config associated with HostName = instance_ip
-        delete_host_by_hostname(instance_ip)
+        # delete_host_by_hostname(instance_ip)
+        delete_host(instance_id)
 
     def list_all_alarms(self):
         alarm_list = self.easy_boto3.cloudwatch("list_all")
         for item in alarm_list:
             print(item)
 
     def ec2_cloud_init_logs(self, instance_ip, config):
```

### Comparing `easy_boto3-0.1.4/easy_boto3/profile/profile.py` & `easy_boto3-0.1.5/easy_boto3/profile/validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,21 @@
 import configparser
-import yaml
-from easy_boto3 import aws_config_path, aws_creds_path, internal_config_path
+from easy_boto3 import aws_config_path, aws_creds_path
 
 
 def validate(profile_name: str = 'default') -> None:
     # load in aws config file using configparser
     aws_config = configparser.ConfigParser()
     aws_config.read(aws_config_path)
 
     # check if profile name is valid
     if profile_name not in aws_config:
         raise ValueError('Profile name not found in aws config')
 
 
-def check_config(profile_name: str = 'default') -> dict:
-    # check if profile name is valid
-    validate(profile_name)
-
-    # load in aws config for read only using configparser
-    aws_config = configparser.ConfigParser()
-    aws_config.read(aws_config_path)
-
-    # retrieve profile secrets from aws_config
-    profile_secrets = aws_config[profile_name]
-
-    # transform into dictionary for return
-    profile_secrets = dict(profile_secrets)
-    return profile_secrets
-
-
 def check_credentials(profile_name: str = 'default') -> dict:
     # check if profile name is valid
     validate(profile_name)
 
     # load in aws config for read only using configparser
     aws_config = configparser.ConfigParser()
     aws_config.read(aws_creds_path)
@@ -41,21 +24,24 @@
     profile_secrets = aws_config[profile_name]
 
     # transform into dictionary for return
     profile_secrets = dict(profile_secrets)
     return profile_secrets
 
 
-def set(profile_name: str = 'default') -> None:
-    # check if profile name is valid
-    validate(profile_name)
+def list_all_profiles() -> list:
+    # load in aws config file using configparser
+    aws_config = configparser.ConfigParser()
+    aws_config.read(aws_config_path)
 
-    # load in easy_boto3 internal config file for read
-    with open(internal_config_path, 'r') as file:
-        internal_config = yaml.safe_load(file)
-
-    # set profile name
-    internal_config['aws_profile'] = profile_name
-
-    # write to easy_boto3 internal config file
-    with open(internal_config_path, 'w') as file:
-        yaml.dump(internal_config, file)
+    # list of all profiles
+    all_profile_sections = list(aws_config.sections())
+    if len(all_profile_sections) == 0:
+        print('No profiles found in aws config')
+    else:
+        # print profiles - one per line
+        print('')
+        print('all profiles found in aws config:')
+        print('--------------------------------')
+        for profile in all_profile_sections:
+            print(profile)
+        print('')
```

### Comparing `easy_boto3-0.1.4/easy_boto3/setup_session.py` & `easy_boto3-0.1.5/easy_boto3/setup_session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from easy_boto3.utilities.decorators import SessionAuthenticator
 from easy_boto3.utilities.aws_profile_parser import get_aws_login_data
-from easy_boto3 import internal_config_path
+from easy_boto3 import active_profile_path
 import yaml
+import json
 
 
 # create session authenticator based on aws credentials
 def setup() -> SessionAuthenticator:
-    # load in internal config file for profile_name
-    with open(internal_config_path, 'r') as f:
-        internal_config = yaml.load(f, Loader=yaml.FullLoader)
+    # read in json file at active_profile_path
+    with open(active_profile_path, 'r') as f:
+        active_profile = json.load(f)
 
     # get profile name
-    profile_name = internal_config['aws_profile']
+    profile_name = active_profile['active_profile']
 
     # load in aws metadata
     aws_metadata = get_aws_login_data(profile_name)
 
     # create session authenticator
     session_auth = SessionAuthenticator(
         aws_access_key_id=aws_metadata['aws_access_key_id'],
```

### Comparing `easy_boto3-0.1.4/easy_boto3/utilities/aws_profile_parser.py` & `easy_boto3-0.1.5/easy_boto3/utilities/aws_profile_parser.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/utilities/decorators.py` & `easy_boto3-0.1.5/easy_boto3/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/easy_boto3/utilities/logger_maker.py` & `easy_boto3-0.1.5/easy_boto3/utilities/logger_maker.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.4/pyproject.toml` & `easy_boto3-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_boto3"
-version = "0.1.4"
+version = "0.1.5"
 description = "`easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file."
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/easy_boto3"
 packages = [{include = "easy_boto3"}]
 include = ["easy_boto3/.easy_boto3_internal.yaml"]
```

### Comparing `easy_boto3-0.1.4/PKG-INFO` & `easy_boto3-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-boto3
-Version: 0.1.4
+Version: 0.1.5
 Summary: `easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file.
 Home-page: https://github.com/jermwatt/easy_boto3
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -30,35 +30,42 @@
 `easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file.
 
 ### Contents
 - [`boto3` made easy](#boto3-made-easy)
     - [Contents](#contents)
   - [Installation](#installation)
   - [Using `easy_boto3` CLI](#using-easy_boto3-cli)
-    - [Creating an ec2 instance with cloudwatch alarm](#creating-an-ec2-instance-with-cloudwatch-alarm)
-    - [Show instance cloud\_init logs](#show-instance-cloud_init-logs)
-    - [Show instance syslog logs](#show-instance-syslog-logs)
-    - [Listing ec2 instances](#listing-ec2-instances)
-    - [Stopping an ec2 instance](#stopping-an-ec2-instance)
-    - [Starting a stopped an ec2 instance](#starting-a-stopped-an-ec2-instance)
-    - [Termianting ec2 instances by id](#termianting-ec2-instances-by-id)
+    - [Managing ec2 instances](#managing-ec2-instances)
+      - [Creating an ec2 instance with cloudwatch alarm](#creating-an-ec2-instance-with-cloudwatch-alarm)
+      - [Show instance cloud\_init logs](#show-instance-cloud_init-logs)
+      - [Show instance syslog logs](#show-instance-syslog-logs)
+      - [Listing ec2 instances](#listing-ec2-instances)
+      - [Stopping an ec2 instance](#stopping-an-ec2-instance)
+      - [Starting a stopped an ec2 instance](#starting-a-stopped-an-ec2-instance)
+      - [Termianting ec2 instances by id](#termianting-ec2-instances-by-id)
+    - [Managing AWS profiles](#managing-aws-profiles)
+      - [List all AWS profiles in `~/.aws/credentials`](#list-all-aws-profiles-in-awscredentials)
+      - [List active AWS profile (currently used by `easy_boto3`)](#list-active-aws-profile-currently-used-by-easy_boto3)
+      - [Set active AWS profile (currently used by `easy_boto3`)](#set-active-aws-profile-currently-used-by-easy_boto3)
   - [Using `easy_boto3`'s Python API](#using-easy_boto3s-python-api)
     - [Creating an ec2 instance](#creating-an-ec2-instance)
 
 ## Installation 
 
 You can install `easy_boto3` via `pip` as
 
 ```bash
 pip install easy-boto3
 ```
 
 ## Using `easy_boto3` CLI
 
-### Creating an ec2 instance with cloudwatch alarm
+### Managing ec2 instances
+
+#### Creating an ec2 instance with cloudwatch alarm
 
 `easy_boto3` allows you to translate a standard `boto3` pythonic infrastructure task like instantiating an `ec2` instance with an attached `cloudwatch` cpu usage alarm from complex pythonic implementation like the following 
 
 ```python
 import boto3
 
 # read in aws_access_key_id and aws_secret_access_key based on input profile_name using boto3
@@ -161,27 +168,27 @@
 
 Using `easy_boto3` and this configuration `config.yaml` the same task - instantiating an `ec2` instance - can be accomplished via the command line as follows:
 
 ```bash
 easy_boto3 ec2 create config.yaml
 ```
 
-### Show instance cloud_init logs
+#### Show instance cloud_init logs
 
 ```bash
 easy_boto3 ec2 check_cloud_init_logs <instance_id>
 ```
 
-### Show instance syslog logs
+#### Show instance syslog logs
 
 ```bash
 easy_boto3 ec2 check_syslog <instance_id>
 ```
 
-### Listing ec2 instances 
+#### Listing ec2 instances 
 
 You can use `easy_boto3` to easy see (all/ running / stopped / terminated) instances in your AWS account as follows.
 
 See all instances
 
 ```bash
 easy_boto3 ec2 list_all
@@ -210,35 +217,58 @@
 easy_boto3 ec2 list_stopped
 ```
 
 ```bash
 easy_boto3 ec2 list_terminated
 ```
 
-### Stopping an ec2 instance
+#### Stopping an ec2 instance
 ```bash
 easy_boto3 ec2 stop <instance_id>
 ```
 
-### Starting a stopped an ec2 instance
+#### Starting a stopped an ec2 instance
 ```bash
 easy_boto3 ec2 start <instance_id>
 ```
 
 
-### Termianting ec2 instances by id  
+#### Termianting ec2 instances by id  
 
 You can use `easy_boto3` CLI to terminate an ec2 instance by id as follows
 
 ```bash
 easy_boto3 ec2 terminate <instance_id>
 ```
 
 Note: by default this will delete any cloudwatch alarms associated with the instance.
 
+### Managing AWS profiles
+
+You can use `easy_boto3` CLI to manage AWS profiles as follows
+
+
+#### List all AWS profiles in `~/.aws/credentials`
+
+```bash
+easy_boto3 profile list_all
+```
+
+#### List active AWS profile (currently used by `easy_boto3`)
+
+```bash
+easy_boto3 profile list_active 
+```
+
+#### Set active AWS profile (currently used by `easy_boto3`)
+
+```bash
+easy_boto3 profile set <profile_name>
+```
+
 
 ## Using `easy_boto3`'s Python API
 
 In addition to config driven command line use, `easy_boto3` also offers a simplified python API that makes creating and managing AWS resources with `boto3` easier.
 
 ### Creating an ec2 instance
```

