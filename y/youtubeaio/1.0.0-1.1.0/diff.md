# Comparing `tmp/youtubeaio-1.0.0.tar.gz` & `tmp/youtubeaio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubeaio-1.0.0.tar", max compression
+gzip compressed data, was "youtubeaio-1.1.0.tar", max compression
```

## Comparing `youtubeaio-1.0.0.tar` & `youtubeaio-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-07-22 14:57:21.440768 youtubeaio-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     4864 2023-07-22 14:57:21.440768 youtubeaio-1.0.0/README.md
--rw-r--r--   0        0        0     3873 2023-07-22 14:57:39.628586 youtubeaio-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       57 2023-07-22 14:57:21.440768 youtubeaio-1.0.0/src/youtubeaio/__init__.py
--rw-r--r--   0        0        0      831 2023-07-22 14:57:21.440768 youtubeaio-1.0.0/src/youtubeaio/const.py
--rw-r--r--   0        0        0     3149 2023-07-22 14:57:21.440768 youtubeaio-1.0.0/src/youtubeaio/helper.py
--rw-r--r--   0        0        0     3031 2023-07-22 14:57:21.440768 youtubeaio-1.0.0/src/youtubeaio/models.py
--rw-r--r--   0        0        0     1772 2023-07-22 14:57:21.440768 youtubeaio-1.0.0/src/youtubeaio/oauth.py
--rw-r--r--   0        0        0        0 2023-07-22 14:57:21.440768 youtubeaio-1.0.0/src/youtubeaio/py.typed
--rw-r--r--   0        0        0     2040 2023-07-22 14:57:21.440768 youtubeaio-1.0.0/src/youtubeaio/types.py
--rw-r--r--   0        0        0     7122 2023-07-22 14:57:21.444768 youtubeaio-1.0.0/src/youtubeaio/youtube.py
--rw-r--r--   0        0        0     6115 1970-01-01 00:00:00.000000 youtubeaio-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     4864 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/README.md
+-rw-r--r--   0        0        0     3873 2023-07-22 17:20:02.227783 youtubeaio-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/src/youtubeaio/__init__.py
+-rw-r--r--   0        0        0      831 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/src/youtubeaio/const.py
+-rw-r--r--   0        0        0     3149 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/src/youtubeaio/helper.py
+-rw-r--r--   0        0        0     5222 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/src/youtubeaio/models.py
+-rw-r--r--   0        0        0     1772 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/src/youtubeaio/oauth.py
+-rw-r--r--   0        0        0        0 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/src/youtubeaio/py.typed
+-rw-r--r--   0        0        0     2040 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/src/youtubeaio/types.py
+-rw-r--r--   0        0        0     9437 2023-07-22 17:19:40.411560 youtubeaio-1.1.0/src/youtubeaio/youtube.py
+-rw-r--r--   0        0        0     6115 1970-01-01 00:00:00.000000 youtubeaio-1.1.0/PKG-INFO
```

### Comparing `youtubeaio-1.0.0/LICENSE.md` & `youtubeaio-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.0.0/README.md` & `youtubeaio-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.0.0/pyproject.toml` & `youtubeaio-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "youtubeaio"
-version = "1.0.0"
+version = "1.1.0"
 description = "Asynchronous Python client for YouTube V3 API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-youtube"
 repository = "https://github.com/joostlek/python-youtube"
@@ -40,15 +40,15 @@
 mypy = "1.4.1"
 pre-commit = "3.3.3"
 pre-commit-hooks = "4.4.0"
 pylint = "2.17.4"
 pytest = "7.4.0"
 pytest-asyncio = "0.21.1"
 pytest-cov = "4.1.0"
-ruff = "0.0.279"
+ruff = "0.0.280"
 safety = "2.4.0b1"
 yamllint = "1.32.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/joostlek/python-youtube/issues"
 Changelog = "https://github.com/joostlek/python-youtube/releases"
```

### Comparing `youtubeaio-1.0.0/src/youtubeaio/const.py` & `youtubeaio-1.1.0/src/youtubeaio/const.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.0.0/src/youtubeaio/helper.py` & `youtubeaio-1.1.0/src/youtubeaio/helper.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.0.0/src/youtubeaio/models.py` & `youtubeaio-1.1.0/src/youtubeaio/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,19 +29,26 @@
     height: int = Field(...)
 
 
 class YouTubeVideoThumbnails(BaseModel):
     """Model representing video thumbnails."""
 
     default: YouTubeThumbnail = Field(...)
-    medium: YouTubeThumbnail = Field(...)
-    high: YouTubeThumbnail = Field(...)
-    standard: YouTubeThumbnail = Field(...)
+    medium: YouTubeThumbnail | None = Field(None)
+    high: YouTubeThumbnail | None = Field(None)
+    standard: YouTubeThumbnail | None = Field(None)
     maxres: YouTubeThumbnail | None = Field(None)
 
+    def get_highest_quality(self) -> YouTubeThumbnail:
+        """Return the highest quality thumbnail."""
+        for size in (self.maxres, self.standard, self.high, self.medium):
+            if size is not None:
+                return size
+        return self.default
+
 
 class YouTubeVideoSnippet(BaseModel):
     """Model representing video snippet."""
 
     published_at: datetime = Field(..., alias="publishedAt")
     channel_id: str = Field(..., alias="channelId")
     title: str = Field(...)
@@ -64,16 +71,23 @@
     snippet: YouTubeVideoSnippet | None = None
 
 
 class YouTubeChannelThumbnails(BaseModel):
     """Model representing channel thumbnails."""
 
     default: YouTubeThumbnail = Field(...)
-    medium: YouTubeThumbnail = Field(...)
-    high: YouTubeThumbnail = Field(...)
+    medium: YouTubeThumbnail | None = Field(None)
+    high: YouTubeThumbnail | None = Field(None)
+
+    def get_highest_quality(self) -> YouTubeThumbnail:
+        """Return the highest quality thumbnail."""
+        for size in (self.high, self.medium):
+            if size is not None:
+                return size
+        return self.default
 
 
 class YouTubeChannelRelatedPlaylists(BaseModel):
     """Model representing related playlists of a channel."""
 
     likes: str = Field(...)
     uploads: str = Field(...)
@@ -103,7 +117,60 @@
 
     channel_id: str = Field(..., alias="id")
     snippet: YouTubeChannelSnippet | None = None
     content_details: YouTubeChannelContentDetails | None = Field(
         None,
         alias="contentDetails",
     )
+
+    @property
+    def upload_playlist_id(self) -> str:
+        """Return playlist id with uploads from channel."""
+        return str(self.channel_id).replace("UC", "UU", 1)
+
+
+class YouTubeSubscriptionSnippet(BaseModel):
+    """Model representing a YouTube subscription snippet."""
+
+    title: str = Field(...)
+    description: str = Field(...)
+    subscribed_at: datetime = Field(..., alias="publishedAt")
+    channel_info: dict[str, str] = Field(..., alias="resourceId")
+
+    @property
+    def channel_id(self) -> str:
+        """Return channel id."""
+        return self.channel_info["channelId"]
+
+
+class YouTubeSubscription(BaseModel):
+    """Model representing a YouTube subscription."""
+
+    subscription_id: str = Field(..., alias="id")
+    snippet: YouTubeSubscriptionSnippet | None = None
+
+
+class YouTubePlaylistItemSnippet(BaseModel):
+    """Model representing a YouTube playlist item snippet."""
+
+    added_at: datetime = Field(..., alias="publishedAt")
+    title: str = Field(...)
+    description: str = Field(...)
+    thumbnails: YouTubeVideoThumbnails = Field(...)
+    playlist_id: str = Field(..., alias="playlistId")
+
+
+class YouTubePlaylistItemContentDetails(BaseModel):
+    """Model representing a YouTube playlist item content details."""
+
+    video_id: str = Field(..., alias="videoId")
+
+
+class YouTubePlaylistItem(BaseModel):
+    """Model representing a YouTube playlist item."""
+
+    playlist_item_id: str = Field(..., alias="id")
+    snippet: YouTubePlaylistItemSnippet | None = Field(None)
+    content_details: YouTubePlaylistItemContentDetails | None = Field(
+        None,
+        alias="contentDetails",
+    )
```

### Comparing `youtubeaio-1.0.0/src/youtubeaio/oauth.py` & `youtubeaio-1.1.0/src/youtubeaio/oauth.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.0.0/src/youtubeaio/types.py` & `youtubeaio-1.1.0/src/youtubeaio/types.py`

 * *Files identical despite different names*

### Comparing `youtubeaio-1.0.0/src/youtubeaio/youtube.py` & `youtubeaio-1.1.0/src/youtubeaio/youtube.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,24 +2,30 @@
 import asyncio
 from collections.abc import AsyncGenerator, Callable, Coroutine
 from dataclasses import field
 from logging import getLogger
 from typing import Any, TypeVar
 
 import async_timeout
-from aiohttp import ClientResponse, ClientSession
+from aiohttp import ClientError, ClientResponse, ClientSession
 
 from youtubeaio.helper import (
     build_url,
     first,
 )
-from youtubeaio.models import YouTubeVideo
+from youtubeaio.models import (
+    YouTubeChannel,
+    YouTubePlaylistItem,
+    YouTubeSubscription,
+    YouTubeVideo,
+)
 from youtubeaio.types import (
     AuthScope,
     MissingScopeError,
+    UnauthorizedError,
     YouTubeAPIError,
     YouTubeBackendError,
     YouTubeResourceNotFoundError,
 )
 
 __all__ = [
     "YouTube",
@@ -47,14 +53,16 @@
         session: ClientSession | None = None,
         session_timeout: int = 10,
         auto_refresh_auth: bool | None = None,
     ) -> None:
         """Initialize YouTube object."""
         self.session = session
         self.session_timeout = session_timeout
+        self.app_id = app_id
+        self.app_secret = app_secret
         if auto_refresh_auth is None:
             self.auto_refresh_auth = app_id is not None and app_secret is not None
         else:
             self.auto_refresh_auth = auto_refresh_auth
         self._r_lookup: dict[
             str,
             Callable[
@@ -72,16 +80,21 @@
         if response.status == 400:
             msg = (await response.json()).get("message")
             raise YouTubeAPIError(
                 "Bad Request" + ("" if msg is None else f" - {msg!s}"),
             )
         if response.status == 404:
             raise YouTubeResourceNotFoundError
+        if response.status == 401:
+            raise UnauthorizedError
         if 400 <= response.status < 500:
-            raise YouTubeAPIError
+            try:
+                response.raise_for_status()
+            except ClientError as exc:
+                raise YouTubeAPIError from exc
         return response
 
     async def _api_get_request(
         self,
         session: ClientSession,
         url: str,
         data: dict[str, Any] | None = None,
@@ -181,22 +194,90 @@
             "id": video_ids,
         }
         async for item in self._build_generator(
             "GET",
             "videos",
             param,
             YouTubeVideo,
-            split_lists=True,
         ):
             yield item  # type: ignore[misc]
 
     async def get_video(self, video_id: str) -> YouTubeVideo | None:
         """Get a single video."""
         return await first(self.get_videos([video_id]))
 
+    async def _get_channels(
+        self,
+        param: dict[str, Any],
+    ) -> AsyncGenerator[YouTubeChannel, None]:
+        """Get channels."""
+        async for item in self._build_generator(
+            "GET",
+            "channels",
+            param,
+            YouTubeChannel,
+        ):
+            yield item  # type: ignore[misc]
+
+    async def get_user_channels(self) -> AsyncGenerator[YouTubeChannel, None]:
+        """Return channels owned by the authenticated user."""
+        param = {
+            "part": "snippet",
+            "mine": "true",
+        }
+        async for item in self._get_channels(param):
+            yield item
+
+    async def get_channels(
+        self,
+        channel_ids: list[str],
+    ) -> AsyncGenerator[YouTubeChannel, None]:
+        """Return list of channels."""
+        param = {
+            "part": "snippet",
+            "id": channel_ids,
+        }
+        async for item in self._get_channels(param):
+            yield item
+
+    async def get_user_subscriptions(
+        self,
+    ) -> AsyncGenerator[YouTubeSubscription, None]:
+        """Get subscriptions for authenticated user."""
+        param = {
+            "part": "snippet",
+            "mine": "true",
+        }
+        async for item in self._build_generator(
+            "GET",
+            "subscriptions",
+            param,
+            YouTubeSubscription,
+        ):
+            yield item  # type: ignore[misc]
+
+    async def get_playlist_items(
+        self,
+        playlist_id: str,
+        max_results: int = 50,
+    ) -> AsyncGenerator[YouTubePlaylistItem, None]:
+        """Get playlist by id."""
+        param = {
+            "part": "snippet,contentDetails",
+            "playlistId": playlist_id,
+            "maxResults": max_results,
+        }
+        async for item in self._build_generator(
+            "GET",
+            "playlistItems",
+            param,
+            YouTubePlaylistItem,
+        ):
+            yield item  # type: ignore[misc]
+
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
 
     async def __aenter__(self) -> "YouTube":
         """Async enter.
```

### Comparing `youtubeaio-1.0.0/PKG-INFO` & `youtubeaio-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtubeaio
-Version: 1.0.0
+Version: 1.1.0
 Summary: Asynchronous Python client for YouTube V3 API.
 Home-page: https://github.com/joostlek/python-youtube
 License: MIT
 Keywords: youtube,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
```

