# Comparing `tmp/nonebot_plugin_session-0.0.5.tar.gz` & `tmp/nonebot_plugin_session-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_session-0.0.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_session-0.0.6.tar", max compression
```

## Comparing `nonebot_plugin_session-0.0.5.tar` & `nonebot_plugin_session-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/LICENSE
--rw-r--r--   0        0        0     4340 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/README.md
--rw-r--r--   0        0        0      601 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/__init__.py
--rw-r--r--   0        0        0       75 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/__init__.py
--rw-r--r--   0        0        0      585 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/console.py
--rw-r--r--   0        0        0     1190 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/kaiheila.py
--rw-r--r--   0        0        0     2719 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3537 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/onebot_v12.py
--rw-r--r--   0        0        0     1565 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/qqguild.py
--rw-r--r--   0        0        0     2616 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/telegram.py
--rw-r--r--   0        0        0      398 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/const.py
--rw-r--r--   0        0        0     2700 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/extractor.py
--rw-r--r--   0        0        0     1525 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
--rw-r--r--   0        0        0     2814 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/model.py
--rw-r--r--   0        0        0     2207 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/saa.py
--rw-r--r--   0        0        0     2053 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/nonebot_plugin_session/session.py
--rw-r--r--   0        0        0     1874 2023-06-21 03:37:33.490563 nonebot_plugin_session-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5391 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4337 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/README.md
+-rw-r--r--   0        0        0      601 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/__init__.py
+-rw-r--r--   0        0        0       75 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/__init__.py
+-rw-r--r--   0        0        0      585 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/console.py
+-rw-r--r--   0        0        0     1190 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/kaiheila.py
+-rw-r--r--   0        0        0     2719 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3537 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     1565 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/qqguild.py
+-rw-r--r--   0        0        0     2616 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/telegram.py
+-rw-r--r--   0        0        0      398 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/const.py
+-rw-r--r--   0        0        0     2700 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/extractor.py
+-rw-r--r--   0        0        0     1525 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
+-rw-r--r--   0        0        0     1264 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/migrations/7d0575ba4608_enum_type.py
+-rw-r--r--   0        0        0     2825 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/model.py
+-rw-r--r--   0        0        0     2228 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/saa.py
+-rw-r--r--   0        0        0     2106 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/session.py
+-rw-r--r--   0        0        0     1874 2023-07-22 14:15:10.077833 nonebot_plugin_session-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5388 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.6/PKG-INFO
```

### Comparing `nonebot_plugin_session-0.0.5/LICENSE` & `nonebot_plugin_session-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/README.md` & `nonebot_plugin_session-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # nonebot-plugin-session
 
 _✨ [Nonebot2](https://github.com/nonebot/nonebot2) 会话信息提取与会话 id 定义插件 ✨_
 
 <p align="center">
   <img src="https://img.shields.io/github/license/noneplugin/nonebot-plugin-session" alt="license">
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="Python">
-  <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
+  <img src="https://img.shields.io/badge/nonebot-2.0.0+-red.svg" alt="NoneBot">
   <a href="https://pypi.org/project/nonebot-plugin-session">
     <img src="https://badgen.net/pypi/v/nonebot-plugin-session" alt="pypi">
   </a>
 </p>
 
 </div>
```

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/__init__.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/console.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/kaiheila.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/onebot_v11.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/onebot_v12.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/qqguild.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/adapters/telegram.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/extractor.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/extractor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/migrations/36de70108aeb_init_db.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/migrations/36de70108aeb_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/model.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from nonebot import require
 
     require("nonebot_plugin_datastore")
 
     from nonebot_plugin_datastore import get_plugin_data
-    from sqlalchemy import Enum, String, UniqueConstraint, select
+    from sqlalchemy import String, UniqueConstraint, select
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Mapped, mapped_column
 
     Model = get_plugin_data().Model
 
     class SessionModel(Model):
         __table_args__ = (
@@ -28,26 +28,26 @@
             ),
         )
 
         id: Mapped[int] = mapped_column(primary_key=True)
         bot_id: Mapped[str] = mapped_column(String(64))
         bot_type: Mapped[str] = mapped_column(String(32))
         platform: Mapped[str] = mapped_column(String(32))
-        level: Mapped[SessionLevel] = mapped_column(Enum(SessionLevel))
+        level: Mapped[str] = mapped_column(String(6))
         id1: Mapped[Optional[str]] = mapped_column(String(64))
         id2: Mapped[Optional[str]] = mapped_column(String(64))
         id3: Mapped[Optional[str]] = mapped_column(String(64))
 
         @property
         def session(self) -> Session:
             return Session(
                 bot_id=self.bot_id,
                 bot_type=self.bot_type,
                 platform=self.platform,
-                level=self.level,
+                level=SessionLevel(self.level),
                 id1=self.id1,
                 id2=self.id2,
                 id3=self.id3,
             )
 
     async def get_or_add_session_model(
         session: Session, db_session: AsyncSession, commit: bool = True
@@ -77,9 +77,9 @@
         )
         db_session.add(session_model)
         if commit:
             await db_session.commit()
             await db_session.refresh(session_model)
         return session_model
 
-except (ImportError, RuntimeError):
+except (ImportError, RuntimeError, ModuleNotFoundError):
     pass
```

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/saa.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/saa.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,9 +49,9 @@
                 return TargetOB12Unknow(detail_type="group", group_id=self.id2)
             elif self.level == SessionLevel.LEVEL3:
                 return TargetOB12Unknow(
                     detail_type="channel", channel_id=self.id2, guild_id=self.id3
                 )
 
     Session.get_saa_target = get_saa_target
-except (ImportError, RuntimeError):
+except (ImportError, RuntimeError, ModuleNotFoundError):
     pass
```

### Comparing `nonebot_plugin_session-0.0.5/nonebot_plugin_session/session.py` & `nonebot_plugin_session-0.0.6/nonebot_plugin_session/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from enum import Enum, IntEnum
+from enum import IntEnum
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from pydantic import BaseModel
+from strenum import StrEnum
 
 if TYPE_CHECKING:
     try:
         from nonebot_plugin_saa import PlatformTarget
     except ImportError:
         pass
 
 
-class SessionLevel(Enum):
-    LEVEL0 = 0
-    LEVEL1 = 1
-    LEVEL2 = 2
-    LEVEL3 = 3
+class SessionLevel(StrEnum):
+    LEVEL0 = "LEVEL0"
+    LEVEL1 = "LEVEL1"
+    LEVEL2 = "LEVEL2"
+    LEVEL3 = "LEVEL3"
 
 
 class SessionIdType(IntEnum):
     TYPE0 = 0
     TYPE1 = 1
     TYPE2 = 2
     TYPE3 = 3
```

### Comparing `nonebot_plugin_session-0.0.5/pyproject.toml` & `nonebot_plugin_session-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_session"
-version = "0.0.5"
+version = "0.0.6"
 description = "Nonebot2 会话信息提取与会话id定义"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-session"
 repository = "https://github.com/noneplugin/nonebot-plugin-session"
```

### Comparing `nonebot_plugin_session-0.0.5/PKG-INFO` & `nonebot_plugin_session-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-session
-Version: 0.0.5
+Version: 0.0.6
 Summary: Nonebot2 会话信息提取与会话id定义
 Home-page: https://github.com/noneplugin/nonebot-plugin-session
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
 # nonebot-plugin-session
 
 _✨ [Nonebot2](https://github.com/nonebot/nonebot2) 会话信息提取与会话 id 定义插件 ✨_
 
 <p align="center">
   <img src="https://img.shields.io/github/license/noneplugin/nonebot-plugin-session" alt="license">
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="Python">
-  <img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
+  <img src="https://img.shields.io/badge/nonebot-2.0.0+-red.svg" alt="NoneBot">
   <a href="https://pypi.org/project/nonebot-plugin-session">
     <img src="https://badgen.net/pypi/v/nonebot-plugin-session" alt="pypi">
   </a>
 </p>
 
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.6 Summary:
 Nonebot2 ä¼è¯ä¿¡æ¯æåä¸ä¼è¯idå®ä¹ Home-page: https://github.com/
 noneplugin/nonebot-plugin-session License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: all
```

