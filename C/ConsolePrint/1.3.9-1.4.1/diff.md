# Comparing `tmp/consoleprint-1.3.9.tar.gz` & `tmp/consoleprint-1.4.1.tar.gz`

## Comparing `consoleprint-1.3.9.tar` & `consoleprint-1.4.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 consoleprint-1.3.9/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 consoleprint-1.3.9/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 consoleprint-1.3.9/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.9/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 consoleprint-1.3.9/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.9/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.9/LICENSE
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 consoleprint-1.3.9/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 consoleprint-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 consoleprint-1.4.1/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 consoleprint-1.4.1/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 consoleprint-1.4.1/src/ConsolePrint/ansi.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 consoleprint-1.4.1/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.4.1/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 consoleprint-1.4.1/tests/tests.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 consoleprint-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.4.1/LICENSE
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 consoleprint-1.4.1/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 consoleprint-1.4.1/PKG-INFO
```

### Comparing `consoleprint-1.3.9/src/ConsolePrint/animate.py` & `consoleprint-1.4.1/src/ConsolePrint/animate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 import time
 import os
+import re
 
-if __name__ == "__main__":
-    os.system('cls')
-    print('\033[0m', end="\r")
 
+print('\033[0m', end="\r")
 __terminal_width = os.get_terminal_size().columns
 
+
+class DimensionExceptionError(Exception):
+    """Custom error when the terminal width is too small"""
+    def __init__(self, error_message):
+        # self.error_message = error_message
+        super().__init__(error_message)
+
+
+class FormatArgumentError(Exception):
+    """Incorrect ANSI sequence passed"""
+    def __init__(self, error_message):
+        # self.error_message = error_message
+        super().__init__(error_message)
+
+
 def __ansify_color(color:str):  
     match color:
         case 'default': color = '\033[0m'
         case 'grey': color = '\033[30m'
         case 'red': color = '\033[31m'
         case 'green': color = '\033[32m'
         case 'yellow': color = '\033[33m'
@@ -27,20 +41,29 @@
         case 'green_bg': color = '\033[42m'
         case 'yellow_bg': color = '\033[43m'
         case 'blue_bg': color = '\033[44m'
         case 'magenta_bg': color = '\033[45m'
         case 'cyan_bg': color = '\033[46m'
         case 'white_bg': color = '\033[47m'
         case _:
-            if '[' not in color or color[-1] != 'm' or not color[2:3].isdigit():
-                raise Exception("Invalid ANSI escape sequence for argument format")
+            pattern1 = "\\033\[(?:[0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])m"
+            pattern2 = "\\033\[48;5;(?:[0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])m"            
+            if not (re.fullmatch(pattern1, color) or re.fullmatch(pattern2, color)):
+                raise FormatArgumentError("Invalid ANSI escape sequence for argument format")
     return color
 
-def printing(text:str, delay:float=0.05, style:str='letter', stay:bool=True, rev:bool=False, format:str='default'):
+
+def is_width_ok(*text_length):
+    if __terminal_width <= sum([*text_length]):
+        raise DimensionExceptionError("Terminal width is too small to display text output")
+
+
+def printing(text:str, *, delay:float=0.05, style:str='letter', stay:bool=True, rev:bool=False, format:str='default'):
     """Prints text to console letter by letter or word by word"""
+    is_width_ok(len(text))
     format = __ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     match rev:
         case False:
             if style.lower() == 'letter':
                 for _ in range(len(text)):
@@ -62,29 +85,31 @@
                     print(' '.join(text[-1 - _:]), end='\r')
                     time.sleep(delay)
     if stay:
         print()
     print('\033[0m', end='\r')
 
 
-def flashprint(text:str, blinks:int=5, delay:float=0.2, stay:bool=True, format:str='default'):
+def flashprint(text:str, *, blinks:int=5, delay:float=0.2, stay:bool=True, format:str='default'):
     """Gets printed output to blink"""
+    is_width_ok(len(text))
     format = __ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     for _ in range(blinks):
         print(text, end='\r'), time.sleep(delay)
         print(' ' * len(text), end='\r'), time.sleep(delay)
     if stay:
         print(text)
     print('\033[0m', end='\r')
 
 
-def flashtext(phrase:str, text:str, index='end', blinks:int=5, delay:float=0.2, format:str='default'):
+def flashtext(phrase:str, text:str, *, index='end', blinks:int=5, delay:float=0.2, format:str='default'):
     """Hilights key word by flashing it"""
+    is_width_ok(len(text), len(phrase), 1)
     format = __ansify_color(format)
     print(format, end='\r')
     textb = ' ' * len(text)
     if index == 'end':
         phrase1 = phrase
         phrase2 = ''
     else:
@@ -96,61 +121,65 @@
         time.sleep(delay)
         print(phrase1 + textb + phrase2, end='\r')
         time.sleep(delay)
     print(phrase1 + text + phrase2)
     print('\033[0m', end='\r')
 
 
-def animate1(text:str, symbol:str="#", format:str='default'):
+def animate1(text:str, *, symbol:str="#", format:str='default'):
     """Flashing masked text to transition to flasing text"""
+    is_width_ok(len(text))
     if len(symbol) != 1:
-        raise Exception("Symbol input should be a single character")
+        raise ValueError("Symbol input should be a single character")
     format = __ansify_color(format)
     text = text.strip()
     symbol = len(text) * symbol
     flashprint(symbol, blinks=3, stay=False, format=format)
     flashprint(text, blinks=2, stay=True, format=format)
 
 
-def animate2(text:str, symbol:str="#", delay:float=0.05, format:str='default'):
+def animate2(text:str, *, symbol:str="#", delay:float=0.05, format:str='default'):
     """Reveals all characters text by text but first masked then flashes"""
+    is_width_ok(len(text))
     if len(symbol) != 1:
-        raise Exception("Symbol input should be a single character")
+        raise ValueError("Symbol input should be a single character")
     format = __ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     symbol = len(text) * symbol
     for _ in symbol + "\r" + text + "\r":
         print(_, end="", flush=True)
         time.sleep(delay)
     flashprint(text, blinks=2, stay=True, format=format)
     print('\033[0m', end='\r')
 
-def text_box(text:str, symbol:str="#", spread:bool=False, padding:bool=False, wall:bool=True, align:str="center", format:str='default'):
+
+def text_box(text:str, *, symbol:str="#", spread:bool=False, padding:bool=False, wall:bool=True, align:str|int="center", format:str='default'):
     """Prints text in a box of symbols.
 If the align parameter is a number then the box is indented by the number count"""
     if spread:
         text = " ".join(list(text)).upper()
     if len(symbol) != 1:
-        raise Exception("Symbol input should be a single character")
-    format = __ansify_color(format)
-    print(format, end='\r')
+        raise ValueError("Symbol input should be a single character")
+    format = __ansify_color(format)    
     text = text.strip()
     end = 5 if padding else 3
     text_row = 3 if padding else 2
     length = len(text) + 8
     left_border = text_row - 1  if padding else text_row
     right_border = text_row + 1 if padding else text_row
-    
+    is_width_ok(len(text), 8, align if isinstance(align, int) else 0)
     if align == "left": indent = 0
     elif align == "right": indent = __terminal_width - length
     elif align == "center": indent = __terminal_width//2 - length//2
     elif isinstance(align, int) and align <= (__terminal_width - length): indent = align
-    else: raise Exception(f"Error in the align argument: {align=}")  
+    else: 
+        raise ValueError(f"Error in the align argument: {align=}")  
     
+    print(format, end='\r')
     for row in range(1, end + 1):
         for col in range(1, length + 1):
             if col == 1:
                 print('\033[0m' + (" " * indent) + format, end="")
             if row == 1 or row == end or col == 1 or col == length:
                 if wall:
                     print(symbol, end="")
@@ -164,31 +193,34 @@
                     print("{:^{}}".format(text, length-2), end="")
             else:
                 print(" ", end="")  
             if col == length:
                 print('\033[0m')
                 
                 
-def star_square(num:int, symbol:str="#", align:str='center', flush:bool=True, format:str='default'):
+def star_square(num:int, *, symbol:str="#", align:str|int='center', flush:bool=True, format:str='default'):
+    is_width_ok(num)
     if len(symbol) != 1:
         raise Exception("Symbol input should be a single character")
     format = __ansify_color(format)
     print(format, end='\r')
     if num < 5 or num > __terminal_width or not isinstance(num, int):
-        raise Exception(f"Invalid square size. Number must be an integer greater than 4 and less than the terminal width: {__terminal_width}")
+        print('\033[0m\r')
+        raise DimensionExceptionError(f"Invalid square size. Number must be an integer greater than 4 and less than the terminal width: {__terminal_width}")
     elif align == 'center':
         indent = '\033[0m' + (' ' * (__terminal_width//2 - num//2)) + format
     elif align == 'right':
         indent = '\033[0m' + (' ' * (__terminal_width - num)) + format
     elif align == 'left':
         indent = ''  
     elif isinstance(align, int) and __terminal_width - align > num:
         indent = '\033[0m' + (" " * align) + format
     else:
-        raise Exception("Align parameter is invalid")    
+        print('\033[0m\r')
+        raise DimensionExceptionError("Check align parameter and square size with respect to terminal width")    
           
     for row in range(1, num + 1):
         time.sleep(0.04)
         print(indent, end="")
         for col in range(1, num + 1):
             if flush: time.sleep(0.04)                
             if row == 1 or col == 1 or row == num or col == num:
@@ -199,37 +231,37 @@
                 print(symbol, end="", flush=flush)  
             else:
                 print(" ", end="", flush=flush)              
             if col == num:
                 print('\033[0m')
     
 
-def asteriskify(text:str, align:str="center", underscore:bool=True, format:str='default'):
+def asteriskify(text:str, *, align:str="center", underscore:bool=True, format:str='default'):
+    is_width_ok(len(text))
     format = __ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     length = len(text)
     
     if align == 'center':
         indent = '\033[0m' + ' ' * (__terminal_width//2 - length//2) + format
     elif align == 'right':
         indent = '\033[0m' + ' ' * (__terminal_width - length) + format
     elif align == 'left':
         indent = ''
     else:
+        print('\033[0m\r')
         raise Exception("Align argument error") 
     print(indent + text)
     if underscore:
         print(indent + '*' * length)
     print('\033[0m', end='\r')
     
-    
 
-# Code test
-if __name__ == "__main__":
+def terminal_test():
     printing("hello this should print letter by letter ", delay=0.05, style="letter", stay=True, rev=False, format='red_bg')
     printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red')
     flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
     flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
     animate1("This text is animated with #", symbol="#", format='red')
     animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
     text_box("boxed in", symbol="#", padding=False, wall=True, align='center', spread=True, format='\033[48;5;4m')
```

### Comparing `consoleprint-1.3.9/src/ConsolePrint/console2file.py` & `consoleprint-1.4.1/src/ConsolePrint/console2file.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.9/src/ConsolePrint/loading.py` & `consoleprint-1.4.1/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.9/tests/tests.py` & `consoleprint-1.4.1/tests/tests.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.9/LICENSE` & `consoleprint-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.9/README.md` & `consoleprint-1.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,24 @@
 file.startConsoleSave(name="my_output.txt", prompt=False)
 # Saves all output between the start and end functions to filename argument
 from calendar import calendar
 print(calendar(2023))
 file.endConsoleSave()
 ```
 2.  This module permits differnt colourful print animations to be output to file.  The format argument takes an ANSI escape sequences as a string.  You may also modify other arguments as desired.<br>
-<b>Preset string values for the format argument</b>
+To view a full list of all the ANSI escape sequences and confirm if your terminal can display the output, import the package and run the command below:
+```python
+import ConsolePrint
+ConsolePrint.ansi_codes()
+
+#For a preview of what is possible
+Consoleprint.terminal_test()
+```
+
+<b>Preset string values may be used instead of the ANSI escape sequence for the format argument</b>
 <table>
     <tr>
         <td>'default' =        '\033[0m'</td>
         <td>'grey' =           '\033[30m'</td>
         <td>'red' =            '\033[31m'</td>
     </tr>
     <tr>
```

### Comparing `consoleprint-1.3.9/pyproject.toml` & `consoleprint-1.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.3.9"
+version = "1.4.1"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate and beautify print output to console"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `consoleprint-1.3.9/PKG-INFO` & `consoleprint-1.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConsolePrint
-Version: 1.3.9
+Version: 1.4.1
 Summary: A package to animate and beautify print output to console
 Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
 Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
 Author-email: Udemezue Iloabachie <udemezue@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,24 @@
 file.startConsoleSave(name="my_output.txt", prompt=False)
 # Saves all output between the start and end functions to filename argument
 from calendar import calendar
 print(calendar(2023))
 file.endConsoleSave()
 ```
 2.  This module permits differnt colourful print animations to be output to file.  The format argument takes an ANSI escape sequences as a string.  You may also modify other arguments as desired.<br>
-<b>Preset string values for the format argument</b>
+To view a full list of all the ANSI escape sequences and confirm if your terminal can display the output, import the package and run the command below:
+```python
+import ConsolePrint
+ConsolePrint.ansi_codes()
+
+#For a preview of what is possible
+Consoleprint.terminal_test()
+```
+
+<b>Preset string values may be used instead of the ANSI escape sequence for the format argument</b>
 <table>
     <tr>
         <td>'default' =        '\033[0m'</td>
         <td>'grey' =           '\033[30m'</td>
         <td>'red' =            '\033[31m'</td>
     </tr>
     <tr>
```

