# Comparing `tmp/idkwhttph-0.2.9.tar.gz` & `tmp/idkwhttph-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idkwhttph-0.2.9.tar", max compression
+gzip compressed data, was "idkwhttph-0.3.0.tar", max compression
```

## Comparing `idkwhttph-0.2.9.tar` & `idkwhttph-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2601 2023-07-19 13:36:31.940444 idkwhttph-0.2.9/README.rst
--rw-r--r--   0        0        0    15396 2023-07-22 13:51:11.498309 idkwhttph-0.2.9/idkwhttph/__init__.py
--rw-r--r--   0        0        0     5312 2023-07-22 14:56:23.982607 idkwhttph-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     7851 2023-07-22 14:56:29.450021 idkwhttph-0.2.9/setup.py
--rw-r--r--   0        0        0     7996 2023-07-22 14:56:29.450616 idkwhttph-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     2601 2023-07-19 13:36:31.940444 idkwhttph-0.3.0/README.rst
+-rw-r--r--   0        0        0    19022 2023-07-22 15:01:12.430335 idkwhttph-0.3.0/idkwhttph/__init__.py
+-rw-r--r--   0        0        0      859 2023-07-22 15:01:19.974328 idkwhttph-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3398 2023-07-22 15:01:30.096846 idkwhttph-0.3.0/setup.py
+-rw-r--r--   0        0        0     3543 2023-07-22 15:01:30.097604 idkwhttph-0.3.0/PKG-INFO
```

### Comparing `idkwhttph-0.2.9/README.rst` & `idkwhttph-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `idkwhttph-0.2.9/idkwhttph/__init__.py` & `idkwhttph-0.3.0/idkwhttph/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__version__ = "0.2.9"
+__version__ = "0.3.0"
 # Imports
-import bcrypt
+
 from getkey import getkey, keys
 from replit import clear
 from replit import db
 from time import sleep
 import cursor
 import json
 import shutil
@@ -313,34 +313,14 @@
 
 
 # Real password
 list_2 = [""]
 list_3 = list_1
 
 
-
-def hash_password(password: bytes) -> bytes:
-    # Generates a salt
-    salt = bcrypt.gensalt()
-    # Hashes the password with salt and returns the hashed password
-    return bcrypt.hashpw(password, salt)
-
-def verify_password(password: bytes, hashed_password: bytes) -> bool:
-    # Checks if the password matches the hashed password
-    return bcrypt.checkpw(password, hashed_password)
-
-
-
-
-
-
-
-
-
-
 def Sign_In() -> None:
     global list_1, list_2, list_3, username, menu, show_hide, alert, JLI, matches
     username = [""]
     list_1 = [""]
     list_2 = [""]
     list_3 = list_1
     alert = False
@@ -517,97 +497,186 @@
                                     else:
                                         username += string
                         clear()
         except:
             clear()
 
 
-from replit import db
-
-def Log_In() -> bool:
+def Log_In():
     cursor.hide()
-    global username, list_2
+    global list_1, list_2, list_3, username, menu, show_hide, alert, JLI
+    alert = False
+    show_hide = False
     username = [""]
+    list_1 = [""]
     list_2 = [""]
-    selection = 0
+    list_3 = list_1
+    if show_hide:
+        menu = ["Username: ", "PassWord: ", "Hide Password", "Submit!"]
+    if show_hide == False:
+        menu = ["Username: ", "PassWord: ", "Show Password", "Submit!"]
+    opt_2 = ""
+    Hello = False
+    opt = ""
+    selection = 4
     key = ""
-
     while True:
         try:
+            if show_hide:
+                menu = [
+                    "Username: ",
+                    "PassWord: ",
+                    "Hide Password",
+                    "Log In!",
+                    "Don't have an account?",
+                ]
+            if show_hide == False:
+                menu = [
+                    "Username: ",
+                    "PassWord: ",
+                    "Show Password",
+                    "Log In!",
+                    "Don't have an account?",
+                ]
+
+            if key == keys.ENTER:
+                if opt == "PassWord: ":
+                    break
             clear()
-            print("------------------------------------")
-            print("            Log In!")
+            print(f"{S.RESET_ALL}------------------------------------")
+            print("             Log In!")
             print("")
             print("Please use the arrow keys to move Up or Down")
             print("")
+            for i in range(len(menu)):
+                opt = menu[i]
+                if i == selection:
+                    if opt == "PassWord: ":
+                        opt_2 = "".join(list_2)
+                        if Hello:
+                            print(f"> {opt}{opt_2}")
+                        else:
+                            opt_2 = "".join(list_1)
+                            print(f"> {opt}{opt_2}")
 
-            menu = [
-                f"Username: {''.join(username)}",
-                f"Password: {'*' * len(list_2)}",
-                "Submit!",
-                "Don't have an account?",
-            ]
-
-            if key == keys.ENTER:
-                if menu[selection].startswith("Password"):
-                    break
+                    elif opt == "Username: ":
+                        if Hello:
+                            print(f'> {opt}{"".join(username)}')
+                        else:
+                            print(f'> {opt}{"".join(username)}')
+                    else:
+                        print(f"> {opt}")
 
-            for i, opt in enumerate(menu):
-                if i == selection:
-                    print(f"> {opt}")
                 else:
-                    print(f"  {opt}")
+                    if opt == "PassWord: ":
+                        if Hello:
+                            print(f'  {opt}{"".join(list_2)}')
+                        else:
+                            print(f'  {opt}{"".join(list_1)}')
+
+                    elif opt == "Username: ":
+                        if Hello:
+                            print(f'  {opt}{"".join(username)}')
+                        else:
+                            print(f'  {opt}{"".join(username)}')
+                    else:
+                        print(f"  {opt}")
 
             key = getkey()
+            string = key
 
             if key == keys.UP:
                 selection = (selection - 1) % len(menu)
+                if selection == -1:
+                    selection = (selection + len(menu) + 1) % len(menu)
             elif key == keys.DOWN:
                 selection = (selection + 1) % len(menu)
-            elif key == keys.BACKSPACE:
-                if selection == 0 and username:
-                    username.pop()
-                elif selection == 1 and list_2:
-                    list_2.pop()
-            elif key == keys.ENTER:
-                if selection == 2:
-                    # Check for matching username and password
-                    matches = db.prefix('password')
-                    matches = list(matches)
-
-                    for match in matches:
-                        key = match.replace("password", "Name")
-                        if (
-                            "".join(username) == db[key]
-                            and bcrypt.checkpw(
-                                "".join(list_2).encode(), db[match].encode()
-                            )
-                        ):
-                            clear()
-                            print("Logged in!")
-                            enter_to_continue()
-                            clear()
-                            cursor.show()
+                if selection > len(menu):
+                    selection = (selection - len(menu) - 1) % len(menu)
+            if key == keys.UP or key == keys.DOWN:
+                pass
+            else:
+                if selection == 0 or selection == 1:
+                    if key == keys.ENTER:
+                        alert = True
+                    else:
+                        pass
 
-                            return True
+                if alert == True:
+                    alert = False
 
+                elif alert == False:
                     clear()
-                    print("Invalid username or password!")
-                    enter_to_continue()
-                    clear()
-                elif selection == 3:
-                    JLI = True
-                    Sign_In()
-                    break
-            elif selection == 0:
-                if key != keys.ENTER:
-                    username.append(key)
-            elif selection == 1:
-                if key != keys.ENTER:
-                    list_2.append(key)
+                    if key == keys.ENTER and selection == 4:
+                        JLI = True
+                        Sign_In()
+                    else:
+                        if key == keys.ENTER and selection == 3:
+                            if "".join(username) == "" or "".join(list_2) == "":
+                                print("You have not entered a username or password")
+                                enter_to_continue()
+                                clear()
+                                break
 
-            clear()
+                            else:
+                                data = load_json_data()
+                                matches = len(data)
+
+                                for i in range(matches):
+                                    if (
+                                        "".join(username) == data["Name" + str(i)]
+                                        and "".join(list_2) == data["password" + str(i)]
+                                    ):
+                                        clear()
+                                        print("Logged in!")
+                                        enter_to_continue()
+                                        clear()
+                                        cursor.show()
+
+                                        return True
+                                else:
+                                    print("Invalid username or password!")
+                                    enter_to_continue()
+                                    clear()
+                        elif (
+                            key == keys.ENTER
+                            and selection == 2
+                            and menu[2] == "Show Password"
+                        ):
+                            list_3 = list_2
+                            Hello = True
+                            show_hide = True
+                        elif (
+                            key == keys.ENTER
+                            and selection == 2
+                            and menu[2] == "Hide Password"
+                        ):
+                            list_3 = list_1
+                            Hello = False
+                            show_hide = False
+                        if selection == 1:
+                            if key == keys.BACKSPACE:
+                                temp_var = list_1.pop(-1)
+                                temp_var = list_2.pop(-1)
+                            else:
+                                list_1 += "*"
+                                list_2 += string
+                        if selection == 0:
+                            if key == keys.BACKSPACE:
+                                try:
+                                    username.pop(-1)
+                                except:
+                                    clear()
+                            else:
+                                if string not in Restrictions:
+                                    pass
+                                else:
+                                    if string == keys.ENTER:
+                                        pass
+                                    else:
+                                        username += string
+                        clear()
         except:
             clear()
```

