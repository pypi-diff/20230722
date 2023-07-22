# Comparing `tmp/pythonit_toolkit-0.1.88.tar.gz` & `tmp/pythonit-toolkit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonit_toolkit-0.1.88.tar", max compression
+gzip compressed data, was "pythonit-toolkit-0.1.9.tar", last modified: Tue Mar  9 00:29:09 2021, max compression
```

## Comparing `pythonit_toolkit-0.1.88.tar` & `pythonit-toolkit-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/LICENSE
--rw-r--r--   0        0        0      737 2023-07-22 09:49:03.687710 pythonit_toolkit-0.1.88/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/api/__init__.py
--rw-r--r--   0        0        0      854 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/api/builder.py
--rw-r--r--   0        0        0      386 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/api/extensions.py
--rw-r--r--   0        0        0     2472 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/api/graphql_test_client.py
--rw-r--r--   0        0        0     1618 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/api/permissions.py
--rw-r--r--   0        0        0      196 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/api/types.py
--rw-r--r--   0        0        0       70 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/emails/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/emails/backends/__init__.py
--rw-r--r--   0        0        0      535 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/emails/backends/base.py
--rw-r--r--   0        0        0      866 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/emails/backends/local.py
--rw-r--r--   0        0        0     1371 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/emails/backends/ses.py
--rw-r--r--   0        0        0     1258 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/emails/templates.py
--rw-r--r--   0        0        0      893 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/emails/utils.py
--rw-r--r--   0        0        0      127 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/headers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/pastaporto/__init__.py
--rw-r--r--   0        0        0     1065 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/pastaporto/actions.py
--rw-r--r--   0        0        0     1794 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/pastaporto/entities.py
--rw-r--r--   0        0        0      167 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/pastaporto/exceptions.py
--rw-r--r--   0        0        0     1026 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/pastaporto/test.py
--rw-r--r--   0        0        0     1046 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/pastaporto/tokens.py
--rw-r--r--   0        0        0        0 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/sentry/__init__.py
--rw-r--r--   0        0        0      437 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/sentry/sentry.py
--rw-r--r--   0        0        0      129 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/service_client/__init__.py
--rw-r--r--   0        0        0     1680 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/service_client/client.py
--rw-r--r--   0        0        0        0 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/starlette_backend/__init__.py
--rw-r--r--   0        0        0      422 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/starlette_backend/middleware.py
--rw-r--r--   0        0        0     1471 2023-07-22 09:48:50.042806 pythonit_toolkit-0.1.88/pythonit_toolkit/starlette_backend/pastaporto_backend.py
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 pythonit_toolkit-0.1.88/PKG-INFO
+-rw-r--r--   0        0        0      388 2021-03-09 00:29:06.655315 pythonit-toolkit-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-03-06 20:07:31.039711 pythonit-toolkit-0.1.9/pythonit_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2021-03-06 19:39:18.875950 pythonit-toolkit-0.1.9/pythonit_toolkit/pastaporto/__init__.py
+-rw-r--r--   0        0        0     1589 2021-03-06 20:43:15.934618 pythonit-toolkit-0.1.9/pythonit_toolkit/pastaporto/entities.py
+-rw-r--r--   0        0        0      167 2021-03-06 19:42:28.521267 pythonit-toolkit-0.1.9/pythonit_toolkit/pastaporto/exceptions.py
+-rw-r--r--   0        0        0      564 2021-03-06 20:43:06.778554 pythonit-toolkit-0.1.9/pythonit_toolkit/pastaporto/test.py
+-rw-r--r--   0        0        0      857 2021-03-09 00:28:54.331229 pythonit-toolkit-0.1.9/pythonit_toolkit/pastaporto/tokens.py
+-rw-r--r--   0        0        0        0 2021-03-06 20:12:18.829711 pythonit-toolkit-0.1.9/pythonit_toolkit/starlette_backend/__init__.py
+-rw-r--r--   0        0        0      422 2021-03-06 20:36:51.215943 pythonit-toolkit-0.1.9/pythonit_toolkit/starlette_backend/middleware.py
+-rw-r--r--   0        0        0     1187 2021-03-06 20:36:51.231943 pythonit-toolkit-0.1.9/pythonit_toolkit/starlette_backend/pastaporto_backend.py
+-rw-r--r--   0        0        0      655 2021-03-09 00:29:09.304617 pythonit-toolkit-0.1.9/setup.py
+-rw-r--r--   0        0        0      300 2021-03-09 00:29:09.304875 pythonit-toolkit-0.1.9/PKG-INFO
```

### Comparing `pythonit_toolkit-0.1.88/pythonit_toolkit/pastaporto/entities.py` & `pythonit-toolkit-0.1.9/pythonit_toolkit/pastaporto/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,47 +27,38 @@
         self.pastaporto = pastaporto
 
 
 @dataclass
 class PastaportoUserInfo:
     id: int
     email: str
-    is_staff: bool
 
     @classmethod
     def from_data(cls, data: dict[str, Any]):
-        return cls(id=int(data["id"]), email=data["email"], is_staff=data["is_staff"])
+        return cls(id=data["id"], email=data["email"])
 
 
 @dataclass
 class Pastaporto:
     user_info: Optional[PastaportoUserInfo] = None
     credentials: list[Credential] = field(default_factory=list)
 
-    @property
-    def is_authenticated(self):
-        return self.user_info is not None
-
     @classmethod
     def from_token(cls, token: str, secret: str):
         try:
             decoded_token = decode_pastaporto(token, secret)
         except (
             ValueError,
             UnicodeDecodeError,
             jwt.ExpiredSignatureError,
             jwt.DecodeError,
             jwt.InvalidAudienceError,
         ):
             raise InvalidPastaportoError()
 
-        user_info = decoded_token.get("user_info")
+        user_info = decoded_token.get("userInfo")
         return cls(
-            user_info=(
-                PastaportoUserInfo.from_data(user_info)
-                if user_info
-                else None
-            ),
+            user_info=PastaportoUserInfo.from_data(user_info) if user_info else None,
             credentials=[
                 Credential(credential) for credential in decoded_token["credentials"]
             ],
         )
```

### Comparing `pythonit_toolkit-0.1.88/pythonit_toolkit/pastaporto/tokens.py` & `pythonit-toolkit-0.1.9/pythonit_toolkit/pastaporto/tokens.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,38 @@
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timedelta
 from typing import Any
 
 import jwt
 
 
-def decode_pastaporto(token: str, secret: str) -> dict[str, Any]:
-    return jwt.decode(
-        token,
-        str(secret),
-        issuer="users",
-        algorithms=["HS256"],
-        options={"require": ["exp", "iss", "iat"]},
-    )
+def create_identity_token(
+    user_id: int, secret: str, expire_after_minutes: int = 10
+) -> str:
+    now = datetime.utcnow()
+
+    payload = {
+        "sub": user_id,
+        "exp": now + timedelta(minutes=expire_after_minutes),
+        "iat": now,
+    }
+    return jwt.encode(payload, str(secret), algorithm="HS256")
 
 
+def decode_pastaporto(token: str, secret: str) -> dict[str, Any]:
+    return jwt.decode(token, str(secret), algorithms=["HS256"])
+
 def decode_service_to_service_token(
-    token: str, secret: str, *, issuer: str, audience: str
+    token: str,
+    secret: str,
+    *,
+    issuer: str,
+    audience: str
 ):
     return jwt.decode(
         token,
         secret,
+        verify=True,
         audience=audience,
         issuer=issuer,
-        algorithms=["HS256"],
-        options={"require": ["exp", "iss", "aud", "iat"]},
-    )
-
-
-def generate_service_to_service_token(secret: str, issuer: str, audience: str):
-    if not secret:
-        raise ValueError("Secret can not be empty")
-
-    now = datetime.now(tz=timezone.utc)
-
-    return jwt.encode(
-        {
-            "iss": issuer,
-            "aud": audience,
-            "iat": now,
-            "exp": now + timedelta(seconds=60),
-        },
-        str(secret),
-        algorithm="HS256",
+        algorithms=['HS256'],
+        options={"require": ["exp", "iss", "aud"]}
     )
```

### Comparing `pythonit_toolkit-0.1.88/pythonit_toolkit/starlette_backend/pastaporto_backend.py` & `pythonit-toolkit-0.1.9/pythonit_toolkit/starlette_backend/pastaporto_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-from pythonit_toolkit.headers import PASTAPORTO_X_HEADER
 from pythonit_toolkit.pastaporto.entities import Pastaporto, RequestAuth
 from pythonit_toolkit.pastaporto.exceptions import InvalidPastaportoError
-from sentry_sdk import set_user
 from starlette.authentication import AuthenticationBackend, AuthenticationError
 from starlette.responses import JSONResponse
 from starlette.routing import request_response
 
+PASTAPORTO_X_HEADER = "x-pastaporto"
+
 
 def on_auth_error(request: request_response, exc: Exception):
     return JSONResponse({"errors": [{"message": str(exc)}]}, status_code=401)
 
 
 class PastaportoAuthBackend(AuthenticationBackend):
     def __init__(self, secret: str) -> None:
         super().__init__()
         self.pastaporto_secret = secret
 
     async def authenticate(self, request):
         if PASTAPORTO_X_HEADER not in request.headers:
             # TODO: Always fail request without pastaporto?
-            set_user(None)
             return
 
         pastaporto_token = request.headers[PASTAPORTO_X_HEADER]
 
         try:
             pastaporto = Pastaporto.from_token(pastaporto_token, self.pastaporto_secret)
-
-            if pastaporto.is_authenticated:
-                set_user({"id": pastaporto.user_info.id, "ip_address": "{{auto}}"})
-            else:
-                set_user(None)
-
             return RequestAuth(pastaporto), pastaporto.user_info
         except InvalidPastaportoError as e:
-            set_user(None)
             raise AuthenticationError("Invalid pastaporto") from e
```

