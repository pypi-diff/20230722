# Comparing `tmp/dialog-workflow-local-python-package-0.0.21.tar.gz` & `tmp/dialog-workflow-local-python-package-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-python-package-0.0.21.tar", last modified: Thu May 18 18:29:08 2023, max compression
+gzip compressed data, was "dialog-workflow-local-python-package-0.0.7.tar", last modified: Sat Jul 22 13:56:48 2023, max compression
```

## Comparing `dialog-workflow-local-python-package-0.0.21.tar` & `dialog-workflow-local-python-package-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-18 18:29:08.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-18 18:29:08.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:29:08.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 18:29:08.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:56:48.681897 dialog-workflow-local-python-package-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-22 13:56:48.681897 dialog-workflow-local-python-package-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:56:48.681897 dialog-workflow-local-python-package-0.0.7/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    19827 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:56:48.681897 dialog-workflow-local-python-package-0.0.7/dialog_workflow_local_python_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-22 13:56:48.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow_local_python_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-22 13:56:48.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow_local_python_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 13:56:48.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow_local_python_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-22 13:56:48.000000 dialog-workflow-local-python-package-0.0.7/dialog_workflow_local_python_package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 13:56:48.681897 dialog-workflow-local-python-package-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-22 13:56:37.000000 dialog-workflow-local-python-package-0.0.7/setup.py
```

### Comparing `dialog-workflow-local-python-package-0.0.21/dialog_workflow/Act.py` & `dialog-workflow-local-python-package-0.0.7/dialog_workflow/Act.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from dialog_workflow.utils import *
-from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
+from utils import *
 import time
 import msvcrt
 import requests
 from AgeDetection import DetectAge
+from TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
 
 class action(object):
     def __init__(self, incoming_message: str, profile_id: int, language: str, profile_curr_state: int, variables: Variable):
         self.incoming_message = incoming_message
         self.profile_id = profile_id
         self.language = language
         self.variables = variables
@@ -63,17 +63,15 @@
             case action_enum.MULTI_CHOICE_POLL.value:
                 return self.multi_choice_poll()
             case action_enum.PRESENT_CHILD_GROUPS_NAMES_BY_ID.value:
                 return self.present_child_groups_names_by_id()   
             case action_enum.PRESENT_GROUPS_WITH_CERTAIN_TEXT.value:
                 return self.present_groups_with_certain_text()     
             case action_enum.INSERT_MISSING_DATA.value:
-                return self.insert_missing_data()   
-            case action_enum.GET_NEXT_SCRIPT.value:
-                return self.get_next_script()             
+                return self.insert_missing_data()                
                                  
             
     def text_message_action(self):
         """Prints the paramter1 message after formatting: 
         "Hello {First Name}, how are you {feeling|doing}?" --> "Hello Tal, how are you doing? """
         message = self.record.parameter1
         replace_fields_with_values_class = replace_fields_with_values(message, self.language, self.variable)
@@ -274,27 +272,14 @@
                 cursor.execute(f"""USE {schema}""")
                 cursor.execute(f"""UPDATE {table} SET {field_name} = '{self.incoming_message}' WHERE (id= {record_id})""")
                 cursor.execute("""USE dialog_workflow""")
                 connection.commit()
             except: #If one of the arguments isn't valid
                 print("Invalid parameter1")
         return False, None
-    
-    def get_next_script(self):
-        """Action for asking the user which workflo script he would like to run next and change the next state id according to his choice."""
-        cursor.execute("""SELECT start_state_id, name FROM dialog_workflow_script_ml_table WHERE lang_code = %s""", [self.language])
-        avilable_scripts_dict = cursor.fetchall()
-        avilable_scripts = [script["name"] for script in avilable_scripts_dict]
-        outgoing_message = "Please choose your desired script out of the following:~"
-        menu = generic_menu(avilable_scripts, self.got_response, self.incoming_message, choose_one_option=True, outgoing_message=outgoing_message)
-        if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value and not self.got_response :
-            return False, menu
-        else:
-            self.profile_curr_state = avilable_scripts_dict[menu[0]-1]["start_state_id"]
-            return True, None
 
 
 def generic_user_choice_action(record: DialogWorkflowRecord, accumulated_message: str, child_nodes: list, choose_exactly_one_option : bool, got_response: bool, chosen_numbers: str, profile: ProfileContext):
     """Sends the user a question with a couple of answers. This function is generic and can let the user choose either
         exactly one option, or more than one. Each case is handeled differently.
         Returns: 
             1. True if the users' next state should be changed to a child next state, False if there's no need to change it's state
@@ -306,14 +291,15 @@
             accumulated_message = accumulated_message + f'{i+1}) {child["parameter1"]}~'
         outgoing_message = process_message(communication_type= COMMUNICATION_TYPE, action_type= action_enum.TEXT_MESSAGE_ACTION.value, message= accumulated_message) 
         if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
             return False, record.next_state_id, outgoing_message 
         else:
             chosen_numbers = input()
 
+
     # The user has to pick exactly one option
     if choose_exactly_one_option:
         profile_next_state = (child_nodes[int(chosen_numbers)-1])["next_state_id"]
         return True, profile_next_state, None
     # In this case the user can choose more than one option: 
     else:
         chosen_numbers = chosen_numbers.split(',')
```

### Comparing `dialog-workflow-local-python-package-0.0.21/dialog_workflow/Constants.py` & `dialog-workflow-local-python-package-0.0.7/dialog_workflow/Constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from enum import Enum
+from circles_local_database_python.database import database
 from dotenv import load_dotenv
 load_dotenv()
-from circles_local_database_python.database import database
-import mysql.connector
-import os
 
 class action_enum(Enum):
-    GET_NEXT_SCRIPT = 0
     LABEL_ACTION = 1
     TEXT_MESSAGE_ACTION = 2
     QUESTION_ACTION = 3
     JUMP_ACTION = 4
     SEND_REST_API_ACTION = 5    
     ASSIGN_VARIABLE_ACTION = 6
     INCREMENT_VARIABLE_ACTION = 7
@@ -18,27 +15,24 @@
     CONDITION_ACTION = 9
     MENU_ACTION = 10
     AGE_DETECTION = 11
     MULTI_CHOICE_POLL = 12
     PRESENT_CHILD_GROUPS_NAMES_BY_ID = 13
     PRESENT_GROUPS_WITH_CERTAIN_TEXT = 14
     INSERT_MISSING_DATA = 15
-    
 
 class communication_type_enum(Enum):
     CONSOLE = 1
     WEBSOCKET = 2
-
-COMMUNICATION_TYPE = communication_type_enum.CONSOLE.value
-ACTIVE_PROFILE_ID  = 1
+COMMUNICATION_TYPE = 2
 
 VARIABLE_NAMES_DICT = {1 : "Person Id" , 2 : "User Id", 3 : "Profile Id", 4 : "Lang Code", 
                        5 : "Name Prefix", 6 : "First Name", 7 : "Middle Name" , 
                        8 : "Last Name", 9 : "Name Suffix",  10 : "Full Name", 
                        11 : "Country", 12 : "State" , 13 : "County" , 14 : "City", 
                        15 : "Neighborhood", 16 : "Street", 17 : "House", 18 : "Suite/Apartment", 
                        19 : "Zip Code", 20 : "Post Result", 21 : "Age", 22 : "Result"}
 
-
+ACTIVE_PROFILE_ID  = 1
 connection = database().connect_to_database()
 cursor = connection.cursor(dictionary=True, buffered=True)
 cursor.execute("""USE dialog_workflow""")
```

### Comparing `dialog-workflow-local-python-package-0.0.21/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-python-package-0.0.7/dialog_workflow/DialogWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from dialog_workflow.utils import *
-from dialog_workflow.Act import action
-from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable
+from utils import *
+from Act import action
+from TablesAsObjects import DialogWorkflowRecord, Variable
 
 
 def get_preferred_language(profile_id: int):
     cursor.execute("""USE profile""")
     cursor.execute("""SELECT preferred_lang_code FROM profile_view WHERE user_id = %s""", [profile_id])
     language = (cursor.fetchone())["preferred_lang_code"]
     cursor.execute("""USE dialog_workflow""")
```

### Comparing `dialog-workflow-local-python-package-0.0.21/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-python-package-0.0.7/dialog_workflow/TablesAsObjects.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from dialog_workflow.Constants import *
-from dialog_workflow.utils import insert_profile_variable_value, get_curr_state, get_variable_value_by_id
+from Constants import *
+from utils import insert_profile_variable_value, get_curr_state, get_variable_value_by_id
 
 class Variable(object):
     def __init__(self):
         self.name2id_dict = {}
         self.id2name_dict = {}
         self.next_variable_id = 1
         for variable_id in VARIABLE_NAMES_DICT:
@@ -53,14 +53,15 @@
 
     def get_variable_value_by_name(self, variable_name : str) -> str:
         return self.get_variable_value_by_id(self.variables.get_variable_id(variable_name))
 
     def set(self, variable_id : int, variable_value : str):
         self.dict[variable_id] = variable_value
         cursor.execute("""USE logger""")
+        # TODO: We should move this to AuditLog repo/class. There is similar functionality required by Text-Block Microservice
         cursor.execute("""INSERT INTO logger
                         (profile_id, state_id, variable_id, variable_value_new) 
                         VALUES (%s,%s,%s,%s)""", 
                         (self.profile_id, self.curr_state_id, variable_id, variable_value))
         cursor.execute("""USE dialog_workflow""")
         connection.commit()
```

### Comparing `dialog-workflow-local-python-package-0.0.21/dialog_workflow/test.py` & `dialog-workflow-local-python-package-0.0.7/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.21/dialog_workflow/utils.py` & `dialog-workflow-local-python-package-0.0.7/dialog_workflow/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # TODO: Let's talk about Constants and the usage in this file
-from dialog_workflow.Constants import *
+from Constants import *
 import random
 import json
 from circles_local_aws_s3_storage_python.AWSStorage import AwsS3Storage
 
 # TOOD: Please include type to all parameters.
 # TODO: Please include return value.
 # TODO: Please add short documentation per PEP8 standard
@@ -187,23 +187,7 @@
     # def get_child_group_id(self) -> list[int]:
     #     """Gets the id of all the records with the given group name"""
     #     cursor.execute("""USE `group`""")
     #     cursor.execute("""SELECT group_id from group_ml_en_view WHERE title = %s""", [self.parameter1])
     #     group_id_dict = cursor.fetchall()
     #     return [group['group_id'] for group in group_id_dict]        
 
-def generic_menu(options: list[str], got_response: bool, chosen_numbers: str, choose_one_option: bool, outgoing_message: str):
-    """A generic function for displaying a menu for the user.
-        Returns: If not got_response: the menu options as json to send to user.
-                 Otherwise returns the chosen numbers as list in int"""
-    if not got_response:
-        outgoing_message += f"Please choose EXACTLY ONE option between 1-{len(options)}:~" if choose_one_option else f"Please select your desired choices, You may select any of the numbers between 1-{len(options)} with a comma seperator between each choice:~"        
-        for i, option in enumerate(options):
-            outgoing_message = outgoing_message + f'{i+1}) {option}~'
-            outgoing_message_json = process_message(communication_type= COMMUNICATION_TYPE, action_type= action_enum.TEXT_MESSAGE_ACTION.value, message= outgoing_message) 
-        if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
-            return outgoing_message_json 
-    
-    if COMMUNICATION_TYPE == communication_type_enum.CONSOLE.value:  
-        chosen_numbers = input()
-    chosen_numbers = chosen_numbers.split(',')
-    return [int(x)-1 for x in chosen_numbers]
```

### Comparing `dialog-workflow-local-python-package-0.0.21/setup.py` & `dialog-workflow-local-python-package-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local-python-package',  
-     version='0.0.21',
+     version='0.0.7',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

