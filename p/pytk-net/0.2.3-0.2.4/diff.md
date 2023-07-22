# Comparing `tmp/pytk_net-0.2.3.tar.gz` & `tmp/pytk_net-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytk_net-0.2.3.tar", last modified: Sat Jun 17 07:07:08 2023, max compression
+gzip compressed data, was "dist\pytk_net-0.2.4.tar", last modified: Sat Jul 22 08:18:02 2023, max compression
```

## Comparing `pytk_net-0.2.3.tar` & `pytk_net-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.065563 pytk_net-0.2.3/
--rw-rw-rw-   0        0        0      966 2023-06-17 07:07:08.063576 pytk_net-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-06-14 06:03:47.000000 pytk_net-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.043957 pytk_net-0.2.3/pytk_net/
--rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytk_net-0.2.3/pytk_net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.054763 pytk_net-0.2.3/pytk_net/ext/
--rw-rw-rw-   0        0        0        0 2023-06-15 09:25:02.000000 pytk_net-0.2.3/pytk_net/ext/__init__.py
--rw-rw-rw-   0        0        0      582 2023-06-16 07:33:50.000000 pytk_net-0.2.3/pytk_net/ext/icon.py
--rw-rw-rw-   0        0        0     3203 2023-06-17 07:05:22.000000 pytk_net-0.2.3/pytk_net/ext/navmenu.py
-drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.057936 pytk_net-0.2.3/pytk_net/icons/
--rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.2.3/pytk_net/icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.2.3/pytk_net/icons/bootstrap-icons.woff
-drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.062577 pytk_net-0.2.3/pytk_net/overwrite/
--rw-rw-rw-   0        0        0     2435 2023-06-14 03:32:19.000000 pytk_net-0.2.3/pytk_net/overwrite/DateEntry.py
--rw-rw-rw-   0        0        0        0 2023-06-14 14:24:28.000000 pytk_net-0.2.3/pytk_net/overwrite/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-06-16 08:55:48.000000 pytk_net-0.2.3/pytk_net/utils.py
--rw-rw-rw-   0        0        0      207 2023-06-16 06:24:00.000000 pytk_net-0.2.3/pytk_net/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-17 07:07:08.050772 pytk_net-0.2.3/pytk_net.egg-info/
--rw-rw-rw-   0        0        0      966 2023-06-17 07:07:07.000000 pytk_net-0.2.3/pytk_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-06-17 07:07:07.000000 pytk_net-0.2.3/pytk_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 07:07:07.000000 pytk_net-0.2.3/pytk_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 07:07:07.000000 pytk_net-0.2.3/pytk_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 07:07:08.065563 pytk_net-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-17 07:06:39.000000 pytk_net-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:18:02.066225 pytk_net-0.2.4/
+-rw-rw-rw-   0        0        0     1044 2023-07-22 08:18:02.066225 pytk_net-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-07-22 08:17:04.000000 pytk_net-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 08:18:02.050602 pytk_net-0.2.4/pytk_net/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytk_net-0.2.4/pytk_net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:18:02.066225 pytk_net-0.2.4/pytk_net/ext/
+-rw-rw-rw-   0        0        0        0 2023-06-15 09:25:02.000000 pytk_net-0.2.4/pytk_net/ext/__init__.py
+-rw-rw-rw-   0        0        0     4528 2023-07-22 08:12:22.000000 pytk_net-0.2.4/pytk_net/ext/ext_tabs.py
+-rw-rw-rw-   0        0        0      669 2023-06-19 00:51:44.000000 pytk_net-0.2.4/pytk_net/ext/icon.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:18:02.066225 pytk_net-0.2.4/pytk_net/icons/
+-rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.2.4/pytk_net/icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.2.4/pytk_net/icons/bootstrap-icons.woff
+drwxrwxrwx   0        0        0        0 2023-07-22 08:18:02.066225 pytk_net-0.2.4/pytk_net/overwrite/
+-rw-rw-rw-   0        0        0     2435 2023-06-14 03:32:19.000000 pytk_net-0.2.4/pytk_net/overwrite/DateEntry.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 14:24:28.000000 pytk_net-0.2.4/pytk_net/overwrite/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-06-16 08:55:48.000000 pytk_net-0.2.4/pytk_net/utils.py
+-rw-rw-rw-   0        0        0      200 2023-07-19 12:38:06.000000 pytk_net-0.2.4/pytk_net/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:18:02.050602 pytk_net-0.2.4/pytk_net.egg-info/
+-rw-rw-rw-   0        0        0     1044 2023-07-22 08:18:01.000000 pytk_net-0.2.4/pytk_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-07-22 08:18:01.000000 pytk_net-0.2.4/pytk_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:18:01.000000 pytk_net-0.2.4/pytk_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-22 08:18:01.000000 pytk_net-0.2.4/pytk_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 08:18:02.066225 pytk_net-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-07-22 08:17:17.000000 pytk_net-0.2.4/setup.py
```

### Comparing `pytk_net-0.2.3/PKG-INFO` & `pytk_net-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytk_net
-Version: 0.2.3
+Version: 0.2.4
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
@@ -33,14 +33,18 @@
 
 可以在tkinter上展示图标,图标数量众多大概1800多个,基于开源的bootstrap图标.
 
 ### 日期输入框 DateEntry
 
 基于ttkbootstrap的DateEntry,重写部分代码,更符合国内使用.
 
+### 拓展选项卡组件 ExtTabs
+
+点击右侧选项菜单 切换视图
+
 ## 开源组件
 
 本项目使用的开源项目如下
 
 | 开源名称           |
 |----------------|
 | bootstrap icon |
```

### Comparing `pytk_net-0.2.3/README.md` & `pytk_net-0.2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 
 可以在tkinter上展示图标,图标数量众多大概1800多个,基于开源的bootstrap图标.
 
 ### 日期输入框 DateEntry
 
 基于ttkbootstrap的DateEntry,重写部分代码,更符合国内使用.
 
+### 拓展选项卡组件 ExtTabs
+
+点击右侧选项菜单 切换视图
+
 ## 开源组件
 
 本项目使用的开源项目如下
 
 | 开源名称           |
 |----------------|
 | bootstrap icon |
```

### Comparing `pytk_net-0.2.3/pytk_net/ext/icon.py` & `pytk_net-0.2.4/pytk_net/ext/icon.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,12 +6,15 @@
 class Icon(Label):
     def __init__(self, parent, icon_name, size, color, **kwargs):
         self.color = color
         self.size = size
         self.icon_name = icon_name
         super().__init__(parent, image=load_font_icon(self.icon_name, self.size, self.color), **kwargs)
 
-    def change(self, icon_name, size, color):
-        self.color = color
-        self.size = size
-        self.icon_name = icon_name
+    def change(self, icon_name=None, size=None, color=None):
+        if icon_name:
+            self.icon_name = icon_name
+        if size:
+            self.size = size
+        if color:
+            self.color = color
         self.configure(image=load_font_icon(self.icon_name, self.size, self.color))
```

### Comparing `pytk_net-0.2.3/pytk_net/ext/navmenu.py` & `pytk_net-0.2.4/pytk_net/ext/ext_tabs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,112 @@
-from tkinter import Label, X, LEFT, TOP
-from typing import List
+from tkinter import Label, X, Y, LEFT, RIGHT, TOP, BOTH
+from typing import List, Callable
 
-from ttkbootstrap import Frame, DARK, SECONDARY, WARNING
+from ttkbootstrap import Frame, DARK, SECONDARY
 
 from pytk_net.ext.icon import Icon
 from pytk_net.utils import get_color
 
 
-class NavMenuItem:
-    def __init__(self, icon, text, side=TOP):
+class TabItem:
+    def __init__(self, key, icon, label, frame: Frame, side=TOP, active=False):
+        self.key = key
         self.side = side
         self.icon = icon
-        self.text = text
+        self.label = label
+        self.frame = frame
+        self.active = active
+
+
+class Menu:
+    def __init__(self, tab_item, nav_menu, icon, label):
+        self.tab_item = tab_item
+        self.nav_menu = nav_menu
+        self.icon = icon
+        self.label = label
 
 
 class NavMenu(Frame):
-    def __init__(self, parent, menus: List[NavMenuItem], default_color=DARK, hover_color=SECONDARY,
-                 selected_color=WARNING, icon_txt_color="#FFF", **kwargs):
+    def __init__(self, parent, tab_items: List[TabItem], on_selected: Callable, default_color=DARK,
+                 hover_color=SECONDARY,
+                 selected_color=SECONDARY, icon_txt_color="#FFF", **kwargs):
         self.default_color = default_color
         self.hover_color = hover_color
         self.selected_color = selected_color
         self.icon_txt_color = icon_txt_color
         self.selected_menu = None
+        self.on_selected = on_selected
 
         super(NavMenu, self).__init__(parent, bootstyle=self.default_color, **kwargs)
         self.pack_propagate(False)
-        for menu in menus:
-            self.create_menu(menu)
+        self.nav_items = []
+        for tab_item in tab_items:
+            self.nav_items.append(self.__create_menu(tab_item))
+
+        fm = self.nav_items[0]
+        self.__click(fm.tab_item, fm.nav_menu, fm.icon, fm.label)
 
-    def create_menu(self, menu: NavMenuItem):
+    def __create_menu(self, tab_item: TabItem):
         nav_menu = Frame(self, height=50, bootstyle=self.default_color, padding=(12, 0, 0, 0))
-        icon = Icon(nav_menu, icon_name=menu.icon, size=30, color=self.icon_txt_color, name="icon")
-        label = Label(nav_menu, text=menu.text, font=("", 12), name="label")
+        icon = Icon(nav_menu, icon_name=tab_item.icon, size=30, color=self.icon_txt_color, name="icon")
+        label = Label(nav_menu, text=tab_item.label, font=("", 12), name="label")
 
         nav_menu.pack_propagate(False)
-        nav_menu.pack(fill=X, ipadx=10, ipady=10, side=menu.side)
-        nav_menu.bind("<Enter>", lambda e: self.enter(e, nav_menu, icon, label))
-        nav_menu.bind("<Leave>", lambda e: self.leave(e, nav_menu, icon, label))
-        nav_menu.bind("<Button-1>", lambda e: self.click(e, nav_menu, icon, label))
-        icon.bind("<Button-1>", lambda e: self.click(e, nav_menu, icon, label))
-        label.bind("<Button-1>", lambda e: self.click(e, nav_menu, icon, label))
+        nav_menu.pack(fill=X, ipadx=10, ipady=10, side=tab_item.side)
+        nav_menu.bind("<Enter>", lambda e: self.__enter(tab_item, nav_menu, icon, label))
+        nav_menu.bind("<Leave>", lambda e: self.__leave(tab_item, nav_menu, icon, label))
+        nav_menu.bind("<Button-1>", lambda e: self.__click(tab_item, nav_menu, icon, label))
+        icon.bind("<Button-1>", lambda e: self.__click(tab_item, nav_menu, icon, label))
+        label.bind("<Button-1>", lambda e: self.__click(tab_item, nav_menu, icon, label))
 
         icon.configure(background=get_color(self.default_color))
         icon.pack(side=LEFT, padx=(0, 12))
 
         label.pack(side=LEFT)
         label.configure(background=get_color(self.default_color), fg=self.icon_txt_color)
 
-    def enter(self, _, menu, icon, label):
+        return Menu(tab_item, nav_menu, icon, label)
+
+    def __enter(self, _, menu, icon, label):
         if menu == self.selected_menu:
             return
         menu.configure(bootstyle=self.hover_color)
         icon.configure(background=get_color(self.hover_color))
         label.configure(background=get_color(self.hover_color))
 
-    def leave(self, _, menu, icon, label):
+    def __leave(self, _, menu, icon, label):
         if menu == self.selected_menu:
             return
         menu.configure(bootstyle=self.default_color)
         icon.configure(background=get_color(self.default_color))
         label.configure(background=get_color(self.default_color))
 
-    def click(self, _, menu, icon, label):
+    def __click(self, menu, nav_menu, icon, label):
         if self.selected_menu is not None:
             _icon = self.selected_menu.children.get("icon")
             _label = self.selected_menu.children.get("label")
             tmp = self.selected_menu
-            self.selected_menu = menu
-            self.leave(None, tmp, _icon, _label)
+            self.selected_menu = nav_menu
+            self.__leave(None, tmp, _icon, _label)
         else:
-            self.selected_menu = menu
+            self.selected_menu = nav_menu
 
-        menu.configure(bootstyle=self.selected_color)
+        nav_menu.configure(bootstyle=self.selected_color)
         icon.configure(background=get_color(self.selected_color))
         label.configure(background=get_color(self.selected_color))
+
+        self.on_selected(menu)
+
+
+class ExtTabs(Frame):
+    def __init__(self, master, tabs: List[TabItem], width=300, height=800):
+        super().__init__(master)
+        self.cur_frame = None
+        self.nav = NavMenu(master, tab_items=tabs, width=width, height=height, on_selected=self.on_selected)
+        self.nav.pack(side=LEFT, fill=Y)
+
+    def on_selected(self, menu: TabItem):
+        if self.cur_frame:
+            self.cur_frame.forget()
+        menu.frame.pack_propagate(True)
+        menu.frame.pack(side=RIGHT, fill=BOTH, expand=True)
+        self.cur_frame = menu.frame
```

### Comparing `pytk_net-0.2.3/pytk_net/icons/bootstrap-icons.json` & `pytk_net-0.2.4/pytk_net/icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.3/pytk_net/icons/bootstrap-icons.woff` & `pytk_net-0.2.4/pytk_net/icons/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.3/pytk_net/overwrite/DateEntry.py` & `pytk_net-0.2.4/pytk_net/overwrite/DateEntry.py`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.3/pytk_net/utils.py` & `pytk_net-0.2.4/pytk_net/utils.py`

 * *Files identical despite different names*

### Comparing `pytk_net-0.2.3/pytk_net.egg-info/PKG-INFO` & `pytk_net-0.2.4/pytk_net.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytk-net
-Version: 0.2.3
+Version: 0.2.4
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
@@ -33,14 +33,18 @@
 
 可以在tkinter上展示图标,图标数量众多大概1800多个,基于开源的bootstrap图标.
 
 ### 日期输入框 DateEntry
 
 基于ttkbootstrap的DateEntry,重写部分代码,更符合国内使用.
 
+### 拓展选项卡组件 ExtTabs
+
+点击右侧选项菜单 切换视图
+
 ## 开源组件
 
 本项目使用的开源项目如下
 
 | 开源名称           |
 |----------------|
 | bootstrap icon |
```

