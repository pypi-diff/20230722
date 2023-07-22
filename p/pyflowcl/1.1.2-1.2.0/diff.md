# Comparing `tmp/pyflowcl-1.1.2.tar.gz` & `tmp/pyflowcl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflowcl-1.1.2.tar", max compression
+gzip compressed data, was "pyflowcl-1.2.0.tar", max compression
```

## Comparing `pyflowcl-1.1.2.tar` & `pyflowcl-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1072 2020-08-13 01:43:57.938850 pyflowcl-1.1.2/LICENSE
--rw-r--r--   0        0        0     1636 2023-01-10 02:32:49.492403 pyflowcl-1.1.2/README.md
--rw-r--r--   0        0        0     2671 2023-01-10 02:32:49.496403 pyflowcl-1.1.2/pyflowcl/Clients.py
--rw-r--r--   0        0        0     6748 2022-01-18 01:39:07.918862 pyflowcl-1.1.2/pyflowcl/Payment.py
--rw-r--r--   0        0        0     2398 2022-01-17 02:41:57.124741 pyflowcl-1.1.2/pyflowcl/Refund.py
--rw-r--r--   0        0        0      703 2023-01-10 02:32:49.496403 pyflowcl-1.1.2/pyflowcl/__init__.py
--rw-r--r--   0        0        0       88 2023-01-10 02:32:49.496403 pyflowcl-1.1.2/pyflowcl/exceptions.py
--rw-r--r--   0        0        0     8510 2023-01-10 02:32:49.496403 pyflowcl-1.1.2/pyflowcl/flowapi_spec.py
--rw-r--r--   0        0        0    19003 2022-11-24 02:24:18.517297 pyflowcl-1.1.2/pyflowcl/models.py
--rw-r--r--   0        0        0     2083 2023-01-10 02:32:49.496403 pyflowcl-1.1.2/pyflowcl/utils.py
--rw-r--r--   0        0        0   173778 2023-01-10 02:32:49.500403 pyflowcl-1.1.2/pyflowcl/yaml_files/apiFlow.min.yaml
--rw-r--r--   0        0        0   173779 2023-01-10 02:32:49.500403 pyflowcl-1.1.2/pyflowcl/yaml_files/apiFlow.sandbox.min.yaml
--rw-r--r--   0        0        0   190754 2023-01-10 02:32:49.500403 pyflowcl-1.1.2/pyflowcl/yaml_files/apiFlow.yaml
--rw-r--r--   0        0        0     1339 2023-01-10 02:32:49.500403 pyflowcl-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 pyflowcl-1.1.2/setup.py
--rw-r--r--   0        0        0     2999 1970-01-01 00:00:00.000000 pyflowcl-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-22 08:18:28.828508 pyflowcl-1.2.0/LICENSE
+-rw-r--r--   0        0        0      774 2023-07-22 08:18:28.828508 pyflowcl-1.2.0/README.md
+-rw-r--r--   0        0        0     2616 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/Clients.py
+-rw-r--r--   0        0        0     6726 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/Payment.py
+-rw-r--r--   0        0        0     2376 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/Refund.py
+-rw-r--r--   0        0        0      136 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/__init__.py
+-rw-r--r--   0        0        0     2271 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/cli.py
+-rw-r--r--   0        0        0       88 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/exceptions.py
+-rw-r--r--   0        0        0    18975 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/models.py
+-rw-r--r--   0        0        0     3601 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/openapi3.py
+-rw-r--r--   0        0        0     2022 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/utils.py
+-rw-r--r--   0        0        0       22 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/version.py
+-rw-r--r--   0        0        0   172982 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.live.min.yaml
+-rw-r--r--   0        0        0   173070 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.min.yaml
+-rw-r--r--   0        0        0   172983 2023-07-22 08:18:28.832507 pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.sandbox.min.yaml
+-rw-r--r--   0        0        0   189757 2023-07-22 08:18:28.836507 pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.yaml
+-rw-r--r--   0        0        0     2052 2023-07-22 08:18:28.836507 pyflowcl-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 pyflowcl-1.2.0/PKG-INFO
```

### Comparing `pyflowcl-1.1.2/LICENSE` & `pyflowcl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflowcl-1.1.2/pyflowcl/Clients.py` & `pyflowcl-1.2.0/pyflowcl/Clients.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 API_URL = "https://www.flow.cl/api"
 API_KEY = "your_key"
 API_SECRET = "your_secret"
 FLOW_TOKEN = "your_payment_token"
 api = ApiClient(API_URL, API_KEY, API_SECRET)
 ```
 """
-from dataclasses import dataclass
-from typing import Any, Dict
-
-import requests
 import hashlib
 import hmac
 import logging
 import warnings
+from dataclasses import dataclass
+from typing import Any, Dict
+
+import requests
 
 
 @dataclass
 class ApiClient:
     """Clase ApiClient con los objetos para realizar llamadas
 
     Implementa todos los métodos de ``dataclass``.
@@ -39,20 +39,19 @@
     """
 
     api_url: str = "https://www.flow.cl/api"
     api_key: str = ""
     api_secret: str = ""
 
     def __post_init__(self):
-        # warnings.warn(
-        #     "ApiClient será reemplazado por FlowAPI en pyFlowCl-1.2.0",
-        #     DeprecationWarning,
-        #     stacklevel=2,
-        # )
-        pass
+        warnings.warn(
+            "ApiClient está deprecado, porfavor usa FlowAPI",
+            DeprecationWarning,
+            stacklevel=2,
+        )
 
     def make_signature(self, params: Dict[str, Any]) -> str:
         """Crea el Hash de validacion para ser enviado con la informacion
 
         Args:
             params: Parametros para crear la firma
 
@@ -60,17 +59,15 @@
             Hash de validacion
         """
         string = ""
         for k, d in params.items():
             if d is not None:
                 string = string + f"{k}{d}"
         logging.debug(f"String to Hash: {string}")
-        hash_string = hmac.new(
-            self.api_secret.encode(), string.encode(), hashlib.sha256
-        ).hexdigest()
+        hash_string = hmac.new(self.api_secret.encode(), string.encode(), hashlib.sha256).hexdigest()
 
         return hash_string
 
     def get(self, url: str, query_string: Dict[str, Any]) -> Dict[str, Any]:
         """Reimplementa get
 
         Args:
```

### Comparing `pyflowcl-1.1.2/pyflowcl/Payment.py` & `pyflowcl-1.2.0/pyflowcl/Payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import logging
 from dataclasses import asdict
-from typing import Any, Dict, Union, cast
-from pyflowcl.Clients import ApiClient
-from pyflowcl.models import (
+from typing import Any, Dict, cast
+
+from .Clients import ApiClient
+from .models import (
     GenericError,
-    PaymentStatus,
+    PaymentList,
     PaymentRequest,
-    PaymentResponse,
     PaymentRequestEmail,
-    PaymentList,
+    PaymentResponse,
+    PaymentStatus,
 )
-import logging
 
 
 def getStatus(
     apiclient: ApiClient,
     token: str,
 ) -> PaymentStatus:
     """Obtiene el estado de un pago previamente creado, el parametro token
```

### Comparing `pyflowcl-1.1.2/pyflowcl/Refund.py` & `pyflowcl-1.2.0/pyflowcl/Refund.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from dataclasses import asdict
-from typing import Any, Dict, Union, cast
-from pyflowcl.Clients import ApiClient
-from pyflowcl.models import RefundRequest, RefundStatus, GenericError
 import logging
+from dataclasses import asdict
+from typing import Any, Dict, cast
+
+from .Clients import ApiClient
+from .models import GenericError, RefundRequest, RefundStatus
 
 
 def create(apiclient: ApiClient, refund_data: Dict[str, Any]) -> RefundStatus:
     """
     Este servicio permite crear una orden de reembolso. Una vez que el
     receptor del reembolso acepte o rechaze el reembolso, Flow
     notificará vía POST a la página del comercio identificada en
```

### Comparing `pyflowcl-1.1.2/pyflowcl/models.py` & `pyflowcl-1.2.0/pyflowcl/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 pyflowcl.models
 ~~~~~~~~~~~~~~~~
 Modelos de distintos objetos del paquete
 """
-from __future__ import annotations
-
 from dataclasses import dataclass
-from typing import Any, Dict, Optional, List, cast
+from typing import Any, Dict, List, Optional, cast
 
 
 class GenericError(BaseException):
     def __init__(self, data):
         self.code = data.get("code")
         self.message = data.get("message")
         super().__init__(f"{self.code}: {self.message}")
@@ -33,15 +31,15 @@
     payer: Optional[str] = None
     optional: Optional[str] = None
     pending_info: Optional[Dict[Any, Any]] = None
     payment_data: Optional[Dict[Any, Any]] = None
     merchant_id: Optional[str] = None
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> PaymentStatus:
+    def from_dict(d: Dict[str, Any]) -> "PaymentStatus":
         flow_order = d.get("flowOrder")
         commerce_order = d.get("commerceOrder")
         request_date = d.get("requestDate")
         status = d.get("status")
         subject = d.get("subject")
         currency = d.get("currency")
         amount = d.get("amount")
@@ -83,15 +81,15 @@
     subject: str = ""
     timeout: Optional[int] = None
     urlConfirmation: str = ""
     urlReturn: str = ""
     s: str = ""
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> PaymentRequest:
+    def from_dict(d: Dict[str, Any]) -> "PaymentRequest":
         amount = d.get("amount")
         apiKey = d.get("apiKey")
         commerceOrder = d.get("commerceOrder")
         currency = d.get("currency")
         email = d.get("email")
         merchantId = d.get("merchantId")
         optional = d.get("optional")
@@ -138,15 +136,15 @@
     subject: Optional[str] = None
     timeout: Optional[int] = None
     urlConfirmation: str = ""
     urlReturn: str = ""
     s: str = ""
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> PaymentRequestEmail:
+    def from_dict(d: Dict[str, Any]) -> "PaymentRequestEmail":
         amount = d.get("amount")
         apiKey = d.get("apiKey")
         commerceOrder = d.get("commerceOrder")
         currency = d.get("currency")
         email = d.get("email")
         forward_days_after = d.get("forward_days_after")
         forward_times = d.get("forward_times")
@@ -183,15 +181,15 @@
     """Objeto respuesta de una creacion de pago"""
 
     url: Optional[str] = None
     token: Optional[str] = None
     flowOrder: Optional[float] = None
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> PaymentResponse:
+    def from_dict(d: Dict[str, Any]) -> "PaymentResponse":
         url = d.get("url")
         token = d.get("token")
         flowOrder = d.get("flowOrder")
 
         return PaymentResponse(
             url=url,
             token=token,
@@ -204,15 +202,15 @@
     """Lista de pagos"""
 
     total: Optional[float] = None
     hasMore: Optional[bool] = None
     data: Optional[List[Dict[Any, Any]]] = None
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> PaymentList:
+    def from_dict(d: Dict[str, Any]) -> "PaymentList":
         total = d.get("total")
         hasMore = d.get("hasMore")
         data = d.get("data")
 
         return PaymentList(
             total=total,
             hasMore=hasMore,
@@ -230,15 +228,15 @@
     flowTrxId: Optional[float] = None
     receiverEmail: str = "correo@ejemplo.cl"
     refundCommerceOrder: str = ""
     urlCallBack: str = ""
     s: str = ""
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> RefundRequest:
+    def from_dict(d: Dict[str, Any]) -> "RefundRequest":
         amount = d.get("amount")
         apiKey = d.get("apiKey")
         commerceTrxId = d.get("commerceTrxId")
         flowTrxId = d.get("flowTrxId")
         receiverEmail = d.get("receiverEmail")
         refundCommerceOrder = d.get("refundCommerceOrder")
         urlCallBack = d.get("urlCallBack")
@@ -263,15 +261,15 @@
     flowRefundOrder: int = 0
     date: str = ""
     status: str = ""
     amount: float = 0
     fee: float = 0
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> RefundStatus:
+    def from_dict(d: Dict[str, Any]) -> "RefundStatus":
         flowRefundOrder = d.get("flowRefundOrder")
         date = d.get("date")
         status = d.get("status")
         amount = d.get("amount")
         fee = d.get("fee")
 
         return RefundStatus(
@@ -295,15 +293,15 @@
     last4CardDigits: Optional[str] = None
     name: str = ""
     pay_mode: Optional[str] = None
     registerDate: Optional[str] = None
     status: int = 0
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> Customer:
+    def from_dict(d: Dict[str, Any]) -> "Customer":
         created = d.get("created")
         creditCardType = d.get("creditCardType")
         customerId = d.get("customerId")
         email = d.get("email")
         externalId = d.get("externalId")
         last4CardDigits = d.get("last4CardDigits")
         name = d.get("name")
@@ -333,15 +331,15 @@
     customerId: str = ""
     email: str = ""
     externalId: str = ""
     name: str = ""
     s: str = ""
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> CustomerRequest:
+    def from_dict(d: Dict[str, Any]) -> "CustomerRequest":
         apiKey = d.get("apiKey")
         customerId = d.get("customerId")
         email = d.get("email")
         externalId = d.get("externalId")
         name = d.get("name")
         s = d.get("s")
 
@@ -360,15 +358,15 @@
     """Lista de Clientes"""
 
     total: Optional[float] = None
     hasMore: Optional[bool] = None
     data: Optional[List[Dict[Any, Any]]] = None
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> CustomerList:
+    def from_dict(d: Dict[str, Any]) -> "CustomerList":
         total = d.get("total")
         hasMore = d.get("hasMore")
         data = d.get("data")
 
         return CustomerList(
             total=total,
             hasMore=hasMore,
@@ -380,15 +378,15 @@
 class CustomerRegisterResponse:
     """Objeto respuesta"""
 
     url: Optional[str] = None
     token: Optional[str] = None
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> CustomerRegisterResponse:
+    def from_dict(d: Dict[str, Any]) -> "CustomerRegisterResponse":
         url = d.get("url")
         token = d.get("token")
 
         return CustomerRegisterResponse(
             url=url,
             token=token,
         )
@@ -400,15 +398,15 @@
 
     creditCardType: str = ""
     customerId: str = ""
     last4CardDigits: str = ""
     status: int = 0
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> CustomerRegisterStatusResponse:
+    def from_dict(d: Dict[str, Any]) -> "CustomerRegisterStatusResponse":
         creditCardType = d.get("creditCardType")
         customerId = d.get("customerId")
         last4CardDigits = d.get("last4CardDigits")
         status = d.get("status")
 
         return CustomerRegisterStatusResponse(
             creditCardType=creditCardType,
@@ -427,15 +425,15 @@
     commerceOrder: str = ""
     currency: Optional[str] = None
     optionals: Optional[str] = None
     subject: str = ""
     s: str = ""
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> CustomerChargeRequest:
+    def from_dict(d: Dict[str, Any]) -> "CustomerChargeRequest":
         amount = d.get("amount")
         apiKey = d.get("apiKey")
         commerceOrder = d.get("commerceOrder")
         currency = d.get("currency")
         optionals = d.get("optionals")
         subject = d.get("subject")
         s = d.get("s")
@@ -460,26 +458,24 @@
     paymen_result: Optional[PaymentStatus] = None
     status: Optional[int] = None
     token: Optional[str] = None
     type: Optional[float] = None
     url: Optional[str] = None
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> CollectResponse:
+    def from_dict(d: Dict[str, Any]) -> "CollectResponse":
         type = d.get("type")
         commerce_order = d.get("commerceOrder")
         flow_order = d.get("flowOrder")
         url = d.get("url")
         token = d.get("token")
         status = d.get("status")
         paymen_result = None
         if d.get("paymenResult") is not None:
-            paymen_result = PaymentStatus.from_dict(
-                cast(Dict[str, Any], d.get("paymenResult"))
-            )
+            paymen_result = PaymentStatus.from_dict(cast(Dict[str, Any], d.get("paymenResult")))
 
         return CollectResponse(
             type=type,
             commerce_order=commerce_order,
             flow_order=flow_order,
             url=url,
             token=token,
@@ -507,15 +503,15 @@
     subject: Optional[str] = None
     timeout: Optional[int] = None
     urlConfirmation: str = ""
     urlReturn: str = ""
     s: str = ""
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> CollectRequest:
+    def from_dict(d: Dict[str, Any]) -> "CollectRequest":
         amount = d.get("amount")
         apiKey = d.get("apiKey")
         byEmail = d.get("byEmail")
         commerceOrder = d.get("commerceOrder")
         currency = d.get("currency")
         forward_days_after = d.get("forward_days_after")
         forward_times = d.get("forward_times")
@@ -556,15 +552,15 @@
     subject: str
     amount: float
     currency: Optional[str] = None
     payment_method: Optional[float] = None
     optional: Optional[str] = None
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> CollectObject:
+    def from_dict(d: Dict[str, Any]) -> "CollectObject":
         customer_id = d.get("customerId")
         commerce_order = d.get("commerceOrder")
         subject = d.get("subject")
         amount = d.get("amount")
         currency = d.get("currency")
         payment_method = d.get("paymentMethod")
         optional = d.get("optional")
@@ -590,15 +586,15 @@
     timeout: Optional[int] = None
     urlCallBack: str = ""
     urlConfirmation: str = ""
     urlReturn: str = ""
     s: str = ""
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> BatchCollectRequest:
+    def from_dict(d: Dict[str, Any]) -> "BatchCollectRequest":
         apiKey = d.get("apiKey")
         batchRows = d.get("batchRows")
         byEmail = d.get("byEmail")
         forward_days_after = d.get("forward_days_after")
         forward_times = d.get("forward_times")
         timeout = d.get("timeout")
         urlCallBack = d.get("urlCallBack")
@@ -626,15 +622,15 @@
     commerceOrder: Optional[str] = None
     rowNumber: Optional[int] = None
     parameter: Optional[str] = None
     errorCode: Optional[int] = None
     errorMsg: Optional[str] = None
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> BatchCollectRejectedRow:
+    def from_dict(d: Dict[str, Any]) -> "BatchCollectRejectedRow":
         customerId = d.get("customerId")
         commerceOrder = d.get("commerceOrder")
         rowNumber = d.get("rowNumber")
         parameter = d.get("parameter")
         errorCode = d.get("errorCode")
         errorMsg = d.get("errorMsg")
 
@@ -652,15 +648,15 @@
 class BatchCollectResponse:
     token: Optional[str] = None
     receivedRows: Optional[int] = None
     acceptedRows: Optional[int] = None
     rejectedRows: Optional[List[BatchCollectRejectedRow]] = None
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> BatchCollectResponse:
+    def from_dict(d: Dict[str, Any]) -> "BatchCollectResponse":
         token = d.get("token")
         receivedRows = d.get("receivedRows")
         acceptedRows = d.get("acceptedRows")
         rejectedRows = []
         for rejected_row in d.get("rejectedRows") or []:
             rejected_row_item = BatchCollectRejectedRow.from_dict(rejected_row)
```

### Comparing `pyflowcl-1.1.2/pyflowcl/utils.py` & `pyflowcl-1.2.0/pyflowcl/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,47 +4,44 @@
 
 Este modulo contiene
 
 - `genera_firma()` - Funcion para generar hash de validacion
 - `genera_parametros()` - Funcion para generar parametros a enviar
 
 """
-from pyflowcl.exceptions import ParamsException
 import hashlib
 import hmac
 
+from .exceptions import ParamsException
 
-def genera_firma(params: dict = {}, flow_secret: str = None) -> str:
+
+def genera_firma(params: dict = None, flow_secret: str = None) -> str:
     """Crea el Hash de validacion
 
     Args:
         params: Parametros para crear la firma
         flow_secret: secretKey de Flow
 
     Returns:
         Hash de validacion
 
     Raises:
         ParamsException: Si `params` o `flow_key` no están definidos
     """
     if not params or not flow_secret:
-        raise ParamsException(
-            "Se necesita 'params' y 'flow_secret' para usar esta función"
-        )
+        raise ParamsException("Se necesita 'params' y 'flow_secret' para usar esta función")
     string = ""
     for k, d in params.items():
         if d is not None:
             string = f"{string}{k}{d}"
-    hash_string = hmac.new(
-        flow_secret.encode(), string.encode(), hashlib.sha256
-    ).hexdigest()
+    hash_string = hmac.new(flow_secret.encode(), string.encode(), hashlib.sha256).hexdigest()
     return hash_string
 
 
-def genera_parametros(params: dict = {}, flow_secret: str = None) -> dict:
+def genera_parametros(params: dict = None, flow_secret: str = None) -> dict:
     """Normaliza y genera los parametros para las llamadas
 
     Este esta funcion verifica que los parametros se encuentren ordenados
     alfabéticamente, para luego generar el hash de validacion
 
     Args:
         params: Parametros para crear la firma
@@ -53,17 +50,15 @@
     Returns:
         `dict` ordenado alfabeticamente con `apiKey` y `s` incorporados
 
     Raises:
         ParamsException: Si `params` o `flow_secret` no están definidos
     """
     if not params or not flow_secret or "apiKey" not in params:
-        raise ParamsException(
-            "Se necesita 'params' y 'flow_secret' para usar esta función"
-        )
+        raise ParamsException("Se necesita 'params' y 'flow_secret' para usar esta función")
 
     if "apiKey" not in params:
         raise ParamsException("'apiKey' no se encuentra en params")
 
     # Ordenamos por key
     sorted_params = dict(sorted(params.items(), key=lambda item: item[0]))
```

### Comparing `pyflowcl-1.1.2/pyflowcl/yaml_files/apiFlow.min.yaml` & `pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.min.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 openapi: 3.0.0
 servers:
   - url: 'https://www.flow.cl/api'
     description: Production server (uses live data)
+  - url: 'https://sandbox.flow.cl/api'
+    description: Sandbox server (uses test data)
 info:
   description: |
     Referirse a https://mariofix.github.io/pyflowcl/apiFlow.yaml/ para el archivo completo
   version: "3.0.1"
   title: Flow API
   termsOfService: "https://www.flow.cl/terminos.php"
   contact:
@@ -30,21 +32,21 @@
   - name: coupon
     description: "Permite crear cupones de descuento para ser aplicados a suscripciones o clientes"
   - name: invoice
     description: 'Permite obtener los importes que se han generado por medio de las suscripciones.'
   - name: settlement
     description: 'Permite obtener las liquidaciones de pagos efectuadas por Flow'
   - name: merchant
-    description: 'Permite gestionar los comercios asociados'   
+    description: 'Permite gestionar los comercios asociados'
 paths:
   /payment/getStatus:
     get:
       tags:
         - payment
-      summary: Obtiene el estado de una orden de pago. 
+      summary: Obtiene el estado de una orden de pago.
       description: 'Este método se utiliza para obtener el estado de un pago. Se debe utilizar en la página callback del comercio para recibir notificaciones de pagos. Cada vez que el pagador efectúe un pago, **Flow** enviará vía POST una llamada a la página del comercio, pasando como parámetro un **token** que deberá utilizarse en este servicio.'
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
@@ -76,15 +78,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: error interno de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /payment/getStatusByCommerceId:
     get:
       tags:
         - payment
       summary: 'Obtiene el estado de un pago en base al commerceId'
       description: 'Este método permite obtener el estado de un pago en base al **commerceId**'
       parameters:
@@ -121,15 +123,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: error interno de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /payment/getStatusByFlowOrder:
     get:
       tags:
         - payment
       summary: 'Obtiene el estado de un pago en base al número de orden Flow'
       description: 'Este método permite obtener el estado de un pago en base al **flowOrder**'
       parameters:
@@ -167,15 +169,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: error interno de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /payment/getPayments:
     get:
       tags:
         - payment
       summary: 'Obtiene el listado de pagos recibidos en un día'
       description: 'Este método permite obtener la lista paginada de pagos recibidos en un día.Los objetos pagos de la lista tienen la misma estructura de los retornados en los servicios payment/getStatus'
       parameters:
@@ -228,15 +230,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
   /payment/getStatusExtended:
     get:
       tags:
         - payment
-      summary: Obtiene el estado extendido de una orden de pago. 
+      summary: Obtiene el estado extendido de una orden de pago.
       description: 'Este método se utiliza para obtener el estado de un pago. A diferencia del /payment/getStatus este servicio retorna el tipo de pago, los 4 últimos dígitos de la tarjeta (si el pago se hizo con tarjeta) y la información del último intento de pago. Se debe utilizar en la página callback del comercio para recibir notificaciones de pagos. Cada vez que el pagador efectúe un pago, **Flow** enviará vía POST una llamada a la página del comercio, pasando como parámetro un **token** que deberá utilizarse en este servicio.'
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
@@ -318,15 +320,15 @@
               schema:
                 $ref: '#/components/schemas/Error'
 
   /payment/create:
     post:
       tags:
         - payment
-      summary: Genera una orden de pago 
+      summary: Genera una orden de pago
       description: "Este método permite crear una orden de pago a **Flow** y recibe como respuesta la **URL** para redirigir el browser del pagador y el **token** que identifica la transacción. La url de redirección se debe formar concatenando los valores recibidos en la respuesta de la siguiente forma:\n\n **url** + \"?token=\" +**token**\n\n
       Una vez que el pagador efectúe el pago, **Flow** notificará el resultado a la página del comercio que se envió en el parámetro **urlConfirmation**."
       responses:
         '200':
           description: "url y token para redirigir el browser del pagador La url de redirección se debe formar concatenando los valores recibidos en la respuesta de la siguiente forma:\n\n **url** + \"?token=\" +**token**"
           content:
             application/json:
@@ -366,35 +368,35 @@
                   description: Monto de la orden
                   type: number
                 email:
                   description: email del pagador
                   type: string
                   format: email
                 paymentMethod:
-                  description: | 
+                  description: |
                     Identificador del medio de pago. Si se envía el identificador, el pagador será redireccionado directamente al medio de pago que se indique, de lo contrario Flow le presentará una página para seleccionarlo. El medio de pago debe haber sido previamente contratado. Podrá ver los identificadores de sus medios de pago en la sección "Mis Datos" ingresando a Flow con sus credenciales. Para indicar todos los medios de pago utilice el identificador:
                     - 9 Todos los medios
                   type: integer
                 urlConfirmation:
                   description: url callback del comercio donde Flow confirmará el pago
                   type: string
                   format: uri
                 urlReturn:
                   description: url de retorno del comercio donde Flow redirigirá al pagador
                   type: string
                   format: uri
                 optional:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 timeout:
                   description: tiempo en segundos para que una orden expire después de haber sido creada. Si no se envía este parámetro la orden no expirará y estará vigente para pago por tiempo indefinido. Si envía un valor en segundos, la orden expirará x segundos después de haber sido creada y no podrá pagarse.
                   type: integer
-                merchantId: 
+                merchantId:
                   description: Id de comercio asociado. Solo aplica si usted es comercio integrador.
                   type: string
                 payment_currency:
                   description: Moneda en que se espera se pague la orden
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
@@ -420,17 +422,17 @@
                       properties:
                         token:
                           description: hash token que identifica la transacción
                           type: string
               responses:
                 '200':
                   description: Your server returns this code if it accepts the callback
-                        
-                
-  
+
+
+
   /payment/createEmail:
     post:
       tags:
         - payment
       summary: Genera un cobro por email
       description: "Permite generar un cobro por email. **Flow** emite un email al pagador que contiene la información de la Orden de pago y el link de pago correspondiente. Una vez que el pagador efectúe el pago, **Flow** notificará el resultado a la página del comercio que se envió en el parámetro **urlConfirmation**."
       responses:
@@ -488,40 +490,40 @@
                 forward_days_after:
                   description: Número de días posteriores al envío del cobro para enviar una nueva notificación de persistencia si la orden no está pagada.
                   type: number
                 forward_times:
                   description: Número de veces de envío de mail de persistencia.
                   type: number
                 optional:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 timeout:
                   description: tiempo en segundos para que una orden expire después de haber sido creada. Si no se envía este parámetro la orden no expirará y estará vigente para pago por tiempo indefinido. Si envía un valor en segundos, la orden expirará x segundos después de haber sido creada y no podrá pagarse.
                   type: integer
-                merchantId: 
+                merchantId:
                   description: Id de comercio asociado. Solo aplica si usted es comercio integrador.
-                  type: string      
+                  type: string
                 payment_currency:
                   description: Moneda en que se espera se pague la orden
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - commerceOrder
                 - subject
                 - amount
                 - email
                 - urlConfirmation
                 - urlReturn
-                - s   
-                
+                - s
+
   /refund/create:
     post:
       tags:
         - refund
       summary: "Permite crear un reembolso"
       description: "Este servicio permite crear una orden de reembolso. Una vez que el receptor del reembolso acepte o rechaze el reembolso, **Flow** notificará vía POST a la página del comercio identificada en **urlCallback** pasando como parámetro **token**\n\n
       En esta página, el comercio debe invocar el servicio **refund/getStatus** para obtener el estado del reembolso."
@@ -577,15 +579,15 @@
               required:
                 - apiKey
                 - refundCommerceOrder
                 - receiverEmail
                 - amount
                 - urlCallBack
                 - s
-                
+
   /refund/cancel:
     post:
       tags:
         - refund
       summary: "Permite cancelar un reembolso"
       description: "Este servicio permite cancelar una orden de reembolso pendiente"
       responses:
@@ -622,21 +624,21 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - token
                 - s
-                
+
   /refund/getStatus:
     get:
       tags:
         - refund
       summary: "Obtiene el estado de un reemboso."
-      description: "Permite obtener el estado de un reembolso solicitado. Este servicio se debe invocar desde la página del comercio que se señaló en el parámetro **urlCallback** del servicio **refund/create**."  
+      description: "Permite obtener el estado de un reembolso solicitado. Este servicio se debe invocar desde la página del comercio que se señaló en el parámetro **urlCallback** del servicio **refund/create**."
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
             type: string
@@ -667,15 +669,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-          
+
   #<--- Customer
   /customer/create:
     post:
       tags:
         - customer
       summary: "Crear un cliente"
       description: "Permite crear un nuevo cliente. El servicio retorna el objeto cliente creado."
@@ -710,15 +712,15 @@
                 name:
                   description: Nombre del cliente (nombre y apellido)
                   type: string
                 email:
                   description: Email del cliente
                   type: string
                 externalId:
-                  description: Identificador externo del cliente, es decir, el identificador con el que su sistema lo reconoce. 
+                  description: Identificador externo del cliente, es decir, el identificador con el que su sistema lo reconoce.
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - name
@@ -775,15 +777,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - customerId
                 - s
-                
+
   /customer/delete:
     post:
       tags:
         - customer
       summary: "Eliminar un cliente"
       description: "Permite eliminar un cliente. Para eliminar un cliente, este no debe tener suscripciones activas o importes pendientes de pago."
       responses:
@@ -871,15 +873,15 @@
   /customer/list:
     get:
       tags:
         - customer
       summary: "Lista de clientes"
       description: "Permite obtener la lista de clientes paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del cliente\n
-      * status: filtro por estado del cliente" 
+      * status: filtro por estado del cliente"
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
             type: string
@@ -937,15 +939,15 @@
       tags:
         - customer
       summary: "Envía a un cliente a registrar su tarjeta de crédito"
       description: |
         Envía a un cliente a registrar su tarjeta de crédito para poder efectuarle cargos automáticos.
         El servicio responde con la **URL** para redirigir el browser del pagador y el **token** que identifica la transacción. La **url** de redirección se debe formar concatenando los valores recibidos en la respuesta de la siguiente forma:
           > **url** + "?token=" +**token**
-          
+
         Una vez redirigido el browser del cliente, Flow responderá por medio de una llamada POST a la url callback del comercio indicada en el parámetro **url_return** pasando como parámetro **token**. El comercio debe implementar una página y capturar el parámetro token enviado por Flow para luego consumir el servicio "customer/getRegisterStatus" para obtener el resultado del registro.
       responses:
         '200':
           description: "Url y token para redireccionar el browser del cliente a registrar su tarjeta de crédito"
           content:
             application/json:
               schema:
@@ -1032,15 +1034,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /customer/unRegister:
     post:
       tags:
         - customer
       summary: "Elimina el registro de la tarjeta de crédito de un cliente"
       description: "Este servicio permite eliminar el registro de la tarjeta de crédito de un cliente. Al eliminar el registro no se podrá hacer cargos automáticos y Flow enviará un cobro por email."
       responses:
@@ -1077,15 +1079,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - customerId
                 - s
-                
+
   /customer/charge:
     post:
       tags:
         - customer
       summary: "Efectúa un cargo en la tarjeta de crédito un cliente"
       description: "Este servicio permite efectuar un cargo automático en la tarjeta de crédito previamente registrada por el cliente. Si el cliente no tiene registrada una tarjeta el metodo retornará error."
       responses:
@@ -1128,34 +1130,34 @@
                 commerceOrder:
                   description: Identificador de la orden del comercio
                   type: string
                 currency:
                   description: Moneda del cargo (CLP, UF)
                   type: string
                 optionals:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - customerId
                 - amount
                 - subject
                 - commerceOrder
                 - s
-                
+
   /customer/collect:
     post:
       tags:
         - customer
-      summary: "Envía un cobro a un cliente." 
+      summary: "Envía un cobro a un cliente."
       description: "Este servicio envía un cobro a un cliente. Si el cliente tiene registrada una tarjeta de crédito se le hace un cargo automático, si no tiene registrada una tarjeta de credito se genera un cobro. Si se envía el parámetro byEmail = 1, se genera un cobro por email."
       responses:
         '200':
           description: El objeto CollectResponse
           content:
             application/json:
               schema:
@@ -1201,32 +1203,32 @@
                   description: url de retorno del comercio donde Flow redirigirá al pagador
                   type: string
                   format: uri
                 currency:
                   description: Moneda del cargo (CLP, UF)
                   type: string
                 paymentMethod:
-                  description: | 
+                  description: |
                     Identificador del medio de pago. Si se envía el identificador, el pagador será redireccionado directamente al medio de pago que se indique, de lo contrario Flow le presentará una página para seleccionarlo. El medio de pago debe haber sido previamente contratado. Podrá ver los identificadores de sus medios de pago en la sección "Mis Datos" ingresando a Flow con sus credenciales. Para indicar todos los medios de pago utilice el identificador:
                     - 9 Todos los medios
                   type: integer
                 byEmail:
                   description: Si se desea que Flow envíe cobros por email, este parámetro debe enviarse con valor 1
                   type: integer
                 forward_days_after:
                   description: Número de días posteriores al envío del cobro para enviar una nueva notificación de persistencia si la orden no está pagada.
                   type: integer
                 forward_times:
                   description: Número de veces de envío de mail de persistencia.
                   type: integer
                 ignore_auto_charging:
-                  description: Si se envía este parámetro con valor 1 entonces ignora el método de cargo automático aunque el cliente tenga registrada una tarjeta de crédito 
+                  description: Si se envía este parámetro con valor 1 entonces ignora el método de cargo automático aunque el cliente tenga registrada una tarjeta de crédito
                   type: integer
                 optionals:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 timeout:
                   description: tiempo en segundos para que una orden expire después de haber sido creada. Si no se envía este parámetro la orden no expirará y estará vigente para pago por tiempo indefinido. Si envía un valor en segundos, la orden expirará x segundos después de haber sido creada y no podrá pagarse.
                   type: integer
                 s:
@@ -1237,20 +1239,20 @@
                 - customerId
                 - amount
                 - subject
                 - commerceOrder
                 - urlConfirmation
                 - urlReturn
                 - s
-                
+
   /customer/batchCollect:
     post:
       tags:
         - customer
-      summary: "Envía de forma masiva un lote de cobros a  clientes." 
+      summary: "Envía de forma masiva un lote de cobros a  clientes."
       description: Este servicio envía de forma masiva un lote de cobros a clientes. Similar al servicio collect pero masivo y asíncrono. Este servicio responde con un token identificador del lote y el número de filas recibidas.
       responses:
         '200':
           description: El objeto BatchCollectResponse
           content:
             application/json:
               schema:
@@ -1358,15 +1360,15 @@
                       properties:
                         token:
                           description: hash token que identifica el pago
                           type: string
               responses:
                 '200':
                   description: Your server returns this code if it accepts the callback
-  
+
   /customer/getBatchCollectStatus:
     get:
       tags:
         - customer
       summary: "Obtiene el estado de un lote de cobros enviados por el servicio batchCollect"
       description: "Este servicio permite consultar el estado de un lote de cobros enviados por medio del servicio batchCollect."
       parameters:
@@ -1403,21 +1405,21 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /customer/reverseCharge:
     post:
       tags:
         - customer
       summary: "Reversa un cargo efectuado en la tarjeta de crédito de un cliente"
-      description: | 
+      description: |
         Este servicio permite reversar un cargo previamente efectuado a un cliente. Para que el cargo se reverse, este servicio debe ser invocado dentro de las 24 horas siguientes a efectuado el cargo, las 24 horas rigen desde las 14:00 hrs, es decir, si el cargo se efectuó a las 16:00 hrs, este puede reversarse hasta las 14:00 hrs del día siguiente.\n\n
           Puede enviar como parámetros el **commerceOrder** o el **flowOrder**.
       responses:
         '200':
           description: El objeto ReverseChargeResponse
           content:
             application/json:
@@ -1527,15 +1529,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /customer/getChargeAttemps:
     get:
       tags:
         - customer
       summary: "Lista paginada de intentos de cargos fallidos a un cliente"
       description: "Este servicio obtiene la lista paginada de los intentos de cargos fallidos a un cliente."
       parameters:
@@ -1603,15 +1605,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /customer/getSubscriptions:
     get:
       tags:
         - customer
       summary: "Lista paginada de suscripciones de un cliente"
       description: "Este servicio obtiene la lista paginada de las suscripciones de un cliente."
       parameters:
@@ -1666,15 +1668,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-       
+
   /plans/create:
     post:
       tags:
         - plans
       summary: "Crea un Plan de Suscripción"
       description: "Este servicio permite crear un nuevo Plan de Suscripción"
       responses:
@@ -1702,36 +1704,36 @@
             schema:
               type: object
               properties:
                 apiKey:
                   description: apiKey del comercio
                   type: string
                 planId:
-                  description: | 
+                  description: |
                     Identificador del Plan. Un texto identificador del Plan, sin espacios, ejemplo: PlanMensual
                   type: string
                 name:
                   description: Nombre del Plan
                   type: string
                 currency:
                   description: Moneda del Plan, por omisión CLP
                   type: string
                 amount:
                   description: Monto del Plan
                   type: number
                 interval:
-                  description: | 
+                  description: |
                     Especifica la frecuencia de cobros (generación de importe)
                       - 1 diario
                       - 2 semanal
                       - 3 mensual
                       - 4 anual
                   type: number
                 interval_count:
-                  description: | 
+                  description: |
                     Número de intervalos de frecuencia de cobros, por ejemplo:
                       - interval = 2 y interval_count = 2 la frecuancia será quincenal. El valor por omisión es 1.
                   type: number
                 trial_period_days:
                   description: Número de días de Trial. El valor por omisón es 0.
                   type: number
                 days_until_due:
@@ -1757,15 +1759,15 @@
               required:
                 - apiKey
                 - planId
                 - name
                 - amount
                 - interval
                 - s
-        
+
   /plans/get:
     get:
       tags:
         - plans
       summary: "Obtiene los datos de un Plan de Suscripción"
       description: "Este servicio permite obtener los datos de un Plan de Suscripción"
       parameters:
@@ -1849,23 +1851,23 @@
                 currency:
                   description: Moneda del Plan
                   type: string
                 amount:
                   description: Monto del Plan
                   type: number
                 interval:
-                  description: | 
+                  description: |
                     Especifica la frecuencia de cobros (generación de importe)
                       - 1 diario
                       - 2 semanal
                       - 3 mensual
                       - 4 anual
                   type: number
                 interval_count:
-                  description: | 
+                  description: |
                     Número de intervalos de frecuencia de cobros, por ejemplo:
                       - interval = 2 y interval_count = 2 la frecuancia será quincenal. El valor por omisión es 1.
                   type: number
                 trial_period_days:
                   description: Número de días de Trial. El valor por omisón es 0.
                   type: number
                 days_until_due:
@@ -1887,15 +1889,15 @@
                     - 2 al importe (invoice)
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - planId
-  
+
   /plans/delete:
     post:
       tags:
         - plans
       summary: "Elimina un Plan de Suscripción"
       description: "Este servicio permite eliminar un Plan de Suscripción. El eliminar un Plan significa que ya no podrá suscribir nuevos clientes al plan. Pero las suscripciones activas continuarán su ciclo de vida mientras estas no sean cancelas."
       responses:
@@ -1931,15 +1933,15 @@
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - planId
-  
+
   /plans/list:
     get:
       tags:
         - plans
       summary: "Lista paginada de planes de suscripción"
       description: "Permite obtener la lista de planes de suscripción paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del plan\n
@@ -1996,15 +1998,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /subscription/create:
     post:
       tags:
         - subscription
       summary: Crea una nueva suscripción a un Plan
       description: "Este servicio permite crear una nueva suscripción de un cliente a un Plan.\n
       Para crear una nueva suscripción, basta con enviar los  parámetros **planId** y **customerId**, los parámetros opcionales son:\n\n
@@ -2081,15 +2083,15 @@
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - planId
                 - customerId
                 - s
-  
+
   /subscription/get:
     get:
       tags:
         - subscription
       summary: "Obtiene una Suscripción en base al subscriptionId"
       description: "Este servicio permite obtener los datos de una suscripción."
       parameters:
@@ -2126,15 +2128,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /subscription/list:
     get:
       tags:
         - subscription
       summary: Obtiene la lista de suscripciones para un Plan
       description: "Permite obtener la lista de suscripciones paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del plan\n
@@ -2197,22 +2199,22 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-          
+
   /subscription/changeTrial:
     post:
       tags:
         - subscription
       summary: Modifica los días de Trial de una suscripción
-      description: | 
-        Este servicio permite modificar los días de Trial de una suscripción. 
+      description: |
+        Este servicio permite modificar los días de Trial de una suscripción.
         Sólo se puede modificar los días de Trial a una suscripción que aún no se ha iniciado o que todavía está vigente el Trial.
       responses:
         '200':
           description: "El objeto Subscription"
           content:
             application/json:
               schema:
@@ -2248,25 +2250,25 @@
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - trial_period_days
                 - s
-  
+
   /subscription/cancel:
     post:
       tags:
         - subscription
       summary: "Cancela una suscripción"
-      description: | 
+      description: |
         Este servicio permite cancelar una suscripción. Existen formas de cancelar una suscripción:
         - inmediatamente. Es decir, en este instante
         - al terminar el perído vigente.
-      
+
         Si desea cancelar la suscripción inmediatamente, envíe el parámetro **at_period_end** con valor 0, si desea cancelarla al final del período vigente envíe el valor 1.
       responses:
         '200':
           description: "El objeto Subscription"
           content:
             application/json:
               schema:
@@ -2301,15 +2303,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - s
-  
+
   /subscription/addCoupon:
     post:
       tags:
         - subscription
       summary: "Agrega un descuento a la suscripción"
       description: "Este servicio permite agregar un descuento a la suscripción. Si la suscripción ya tenía un descuento, será reemplazado por este."
       responses:
@@ -2337,28 +2339,28 @@
             schema:
               type: object
               properties:
                 apiKey:
                   description: apiKey del comercio
                   type: string
                 subscriptionId:
-                  description: Identificador de la suscripción 
+                  description: Identificador de la suscripción
                   type: string
                 couponId:
                   description: Identificador del cupón de descuento.
                   type: number
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - couponId
                 - s
-                
+
   /subscription/deleteCoupon:
     post:
       tags:
         - subscription
       summary: "Elimina un descuento a la suscripción"
       description: "Este servicio permite eliminar el descuento que tenga la suscripción. El eliminar el descuento de la suscripción, no elimina el descuento que podría tenar asociado el cliente."
       responses:
@@ -2395,15 +2397,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - s
-                
+
   /coupon/create:
     post:
       tags:
         - coupon
       summary: "Crea un cupón de descuento"
       description: "Este servicio permite crear un cupón de descuento"
       responses:
@@ -2431,33 +2433,33 @@
             schema:
               type: object
               properties:
                 apiKey:
                   description: apiKey del comercio
                   type: string
                 name:
-                  description: Nombre del cupón 
+                  description: Nombre del cupón
                   type: string
                 percent_off:
                   description: Porcentaje del cupon. Número entre 0 y 100. Permite 2 decimales con punto decimal. Ejemplo 10.2. No se agrega el signo %
                   type: number
                 currency:
-                  description: Moneda del descuento. Solo agregue la moneda para cupones de monto. 
+                  description: Moneda del descuento. Solo agregue la moneda para cupones de monto.
                   type: string
                 amount:
                   description: Monto del descuento
                   type: number
                 duration:
-                  description: | 
+                  description: |
                     Duración del cupón:
                     - 1 definida
                     - 0 indefinida
                   type: number
                 times:
-                  description: | 
+                  description: |
                     Si la duración del cupón es definida, este campo indica las veces de duración del cupón. Si el cupón se aplica a un cliente veces corresponderá a meses. Si l cupón se aplica a una suscripción, veces corresponderá a los períodos del Plan.
                   type: number
                 max_redemptions:
                   description: Número de veces de aplicación del cupón.
                   type: number
                 expires:
                   description: Fecha de expiración del cupón en formato yyyy-mm-dd
@@ -2465,15 +2467,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - name
                 - s
-                  
+
   /coupon/edit:
     post:
       tags:
         - coupon
       summary: Edita un cupón de descuento
       description: Este servicio permite editar un cupón de descuento. Sólo se puede editar el nombre de un cupón.
       responses:
@@ -2514,15 +2516,15 @@
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - couponId
                 - name
                 - s
-                
+
   /coupon/delete:
     post:
       tags:
         - coupon
       summary: "Elimina un cupón de descuento"
       description: "Este servicio permite eliminar un cupón de descuento. Eliminar un cupón de descuento no elimina los descuentos aplicados a clientes o suscripciones, sólo no permite volver a aplicar este cupón"
       responses:
@@ -2559,15 +2561,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - couponId
                 - s
-                
+
   /coupon/get:
     get:
       tags:
       - coupon
       summary: "Obtiene un cupón de descuento"
       description: "Este servicio permite obtener los datos de un cupón de descuento"
       parameters:
@@ -2604,15 +2606,15 @@
                   $ref: '#/components/schemas/Error'
           '401':
             description: Error de negocio
             content:
               application/json:
                 schema:
                   $ref: '#/components/schemas/Error'
-  
+
   /coupon/list:
     get:
       tags:
       - coupon
       summary: "Lista los cupones de descuento"
       description: "Este servicio permite la lista de cupones de descuento"
       parameters:
@@ -2638,15 +2640,15 @@
           name: filter
           description: Filtro por el nombre del cupón
           required: false
           schema:
             type: string
         - in: query
           name: status
-          description: | 
+          description: |
             Filtro por el estado del cupón:
             - 1 Activo
             - 0 Inactivo
           required: false
           schema:
             type: integer
         - in: query
@@ -2669,16 +2671,16 @@
                 schema:
                   $ref: '#/components/schemas/Error'
           '401':
             description: Error de negocio
             content:
               application/json:
                 schema:
-                  $ref: '#/components/schemas/Error'     
-                
+                  $ref: '#/components/schemas/Error'
+
   /invoice/get:
     get:
       tags:
         - invoice
       summary: "Obtiene los datos de un Invoice (Importe)"
       description: "Este servicio permite obtener los datos de un Importe."
       parameters:
@@ -2715,15 +2717,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-          
+
   /invoice/cancel:
     post:
       tags:
         - invoice
       summary: "Cancela un Importe (Invoice) pendiente de pago"
       description: "Este servicio permite cancelar un Importe (Invoice) pendiente de pago."
       responses:
@@ -2760,15 +2762,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - invoiceId
                 - s
-                
+
   /invoice/outsidePayment:
       post:
         tags:
           - invoice
         summary: "Ingresa un pago por fuera y da por pagado el Importe (Invoice) "
         description: "Este servicio permite dar por pagado un Importe (Invoice) cuando el pago no se realiza por Flow."
         responses:
@@ -2875,15 +2877,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /invoice/retryToCollect:
     post:
       tags:
         - invoice
       summary: "Reintenta el cobro de un invoice vencido"
       description: "Este servicio permite reintentar el cobro de un Invoice vencido."
       responses:
@@ -2968,15 +2970,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-            
+
   /settlement/getById:
     get:
       tags:
         - settlement
       summary: Obtiene la Liquidación efectuada con ese identificador
       description:  'Este método se utiliza para obtener el objeto Settlement correspondiente al identificador. <br>Nota: Si su liquidación es anterior al 01-06-2021 utilizar este servicio, en caso contrario se recomienda utilizar el servicio /settlement/getByIdv2'
       deprecated: true
@@ -3121,15 +3123,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
   /merchant/create:
     post:
       tags:
         - merchant
-      summary: Crea un comercio asociado 
+      summary: Crea un comercio asociado
       description: "Este método permite crear un nuevo comercio asociado en **Flow**"
       responses:
         '200':
           description: "Objeto con información del comercio asocioado en Flow"
           content:
             application/json:
               schema:
@@ -3173,15 +3175,15 @@
                 - name
                 - url
                 - s
   /merchant/edit:
     post:
       tags:
         - merchant
-      summary: Edita un comercio asociado 
+      summary: Edita un comercio asociado
       description: "Este método permite modificar un comercio asociado previamente creado en **Flow**"
       responses:
         '200':
           description: "Objeto con información del comercio asociado en Flow"
           content:
             application/json:
               schema:
@@ -3225,15 +3227,15 @@
                 - name
                 - url
                 - s
   /merchant/delete:
     post:
       tags:
         - merchant
-      summary: Elimina un comercio asociado 
+      summary: Elimina un comercio asociado
       description: "Este método permite eliminar un comercio asociado previamente creado en **Flow**"
       responses:
         '200':
           description: "Objeto con información de la orden generada en Flow"
           content:
             application/json:
               schema:
@@ -3269,15 +3271,15 @@
                 - apiKey
                 - id
                 - s
   /merchant/get:
     get:
       tags:
         - merchant
-      summary: Obtener comercio asociado 
+      summary: Obtener comercio asociado
       description: "Este método permite obtener la información de un comercio asociado previamente creado en **Flow**"
       responses:
         '200':
           description: "Objeto con información del comercio asocioado en Flow"
           content:
             application/json:
               schema:
@@ -3313,15 +3315,15 @@
           required: true
           schema:
             type: string
   /merchant/list:
     get:
       tags:
         - merchant
-      summary: Lista de comercios asociados 
+      summary: Lista de comercios asociados
       description: "Permite obtener la lista de comercios paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del comercio asociado\n
       * status: filtro por estado del comercio asociado"
       responses:
         '200':
           description: "Objeto con información del comercio asocioado en Flow"
           content:
@@ -3395,16 +3397,16 @@
         requestDate:
           type: string
           description: La fecha de creación de la orden
           format: 'yyyy-mm-dd hh:mm:ss'
           example: '2017-07-21 12:32:11'
         status:
           type: integer
-          description: | 
-            El estado de la order 
+          description: |
+            El estado de la order
             - 1 pendiente de pago
             - 2 pagada
             - 3 rechazada
             - 4 anulada
           example: 1
         subject:
           type: string
@@ -3523,16 +3525,16 @@
         requestDate:
           type: string
           description: La fecha de creación de la orden
           format: 'yyyy-mm-dd hh:mm:ss'
           example: '2017-07-21 12:32:11'
         status:
           type: integer
-          description: | 
-            El estado de la order 
+          description: |
+            El estado de la order
             - 1 pendiente de pago
             - 2 pagada
             - 3 rechazada
             - 4 anulada
           example: 1
         subject:
           type: string
@@ -3672,15 +3674,15 @@
           type: string
           description: token de la transacción
           example: "33373581FC32576FAF33C46FC6454B1FFEBD7E1H"
         flowOrder:
           type: number
           description: Número de order de cobro Flow
           example: 8765456
-    
+
     Customer:
       type: object
       properties:
         customerId:
           type: string
           description: Identificador del cliente
           example: cus_onoolldvec
@@ -3714,15 +3716,15 @@
         externalId:
           type: string
           description: El identificador del cliente en su negocio
           example: 14233531-8
         status:
           type: string
           description: |
-            El estado del cliente: 
+            El estado del cliente:
             - 0 Eliminado
             - 1 Activo
           example: '1'
         registerDate:
           type: string
           format: 'yyyy-mm-dd hh:mm:ss'
           description: La fecha en que el cliente registro su tarjeta de crédito.
@@ -3732,25 +3734,25 @@
       properties:
         total:
           type: number
           description: El número total de registros encontrados
           example: 200
         hasMore:
           type: boolean
-          description: | 
+          description: |
             - 1 Si existen más páginas
             - 0 Si es la última página
           example: 1
         data:
           type: array
           items:
             type: object
           description: arreglo de registros de la página
           example: '[{item list 1}{item list 2}{item list n..}'
-          
+
     RegisterResult:
       type: object
       properties:
         status:
           type: string
           description: El estado del registro
             - 1 registrado
@@ -3764,34 +3766,34 @@
           type: string
           description: Marca de la tarjeta de crédito
           example: Visa
         last4CardDigits:
           type: string
           description: Últimos 4 dígitos de la tarjeta de crédito
           example: '0366'
-          
+
     RefundStatus:
       type: object
       properties:
-        token: 
+        token:
           type: string
           description: Token del reembolso
           example: C93B4FAD6D63ED9A3F25D21E5D6DD0105FA8CAAQ
         flowRefundOrder:
           type: string
           description: Número de orden de reembolso
           example: '122767'
         date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha de solicitud de reembolso
           example: '2017-07-21 12:33:15'
         status:
           type: string
-          description: | 
+          description: |
             Estado del reembolso, los estado pueden ser:
             - created Solicitud creada
             - accepted Reembolso aceptado
             - rejected Reembolso rechazado
             - refunded Reembolso reembolsado
             - canceled Reembolso cancelado
           example: created
@@ -3799,19 +3801,19 @@
           type: number
           description: Monto del reembolso
           example: '12000.00'
         fee:
           type: number
           description: Costo del servicio de reembolso
           example: '240.00'
-          
+
     CollectResponse:
       type: object
       properties:
-        type: 
+        type:
           type: number
           description: |
             Tipo de cobro:
             - 1 Cobro automático
             - 2 Cobro normal (link de pago)
             - 3 Cobro por email
           example: '1'
@@ -3836,16 +3838,16 @@
           type: integer
           description: |
             Estado de emisión del cobro, es decir si se emitió el cobro, no indica si hubo pago:
             - 0 Cobro no emitido (uncollected)
             - 1 Cobro emitido (collected)
         paymenResult:
           $ref: '#/components/schemas/PaymentStatus'
-          
-    
+
+
     CollectObject:
       type: object
       description: Objeto de cobro para un lote de cobros
       properties:
         customerId:
           type: string
           description: Identificador del cliente en Flow
@@ -3875,15 +3877,15 @@
           description: Valores opcionales en formato JSON
           example: {"factura":"123456", "clave": "Valor"}
       required:
         - customerId
         - commerceOrder
         - subject
         - amount
-        
+
     BatchCollectResponse:
       type: object
       properties:
         token:
           type: string
           description: hash token identificador del lote recibido
           example: "33373581FC32576FAF33C46FC6454B1FFEBD7E1H"
@@ -3896,16 +3898,16 @@
           description: Número de filas de collects aceptadas
           example: '111'
         rejectedRows:
           type: array
           description: Arreglo de filas de collects rechazadas
           items:
             $ref: '#/components/schemas/BatchCollectRejectedRow'
-          
-          
+
+
     BatchCollectRejectedRow:
       type: object
       properties:
         customerId:
           type: string
           description: Identificador del cliente en Flow
           example: cus_onoolldvec
@@ -3937,15 +3939,15 @@
             - 109 The minimum amount is $value CLP
             - 110 Optional values are not in JSON format
           example: 104
         errorMsg:
           type: string
           description: descripción del error
           example: commerceOrder already sent
-          
+
     BatchCollectStatusResponse:
       type: object
       properties:
         token:
           type: string
           description: hash token identificador del lote recibido
           example: "33373581FC32576FAF33C46FC6454B1FFEBD7E1H"
@@ -3967,23 +3969,23 @@
             - processing (lote en procesamiento)
             - processed (lote procesado)
         collectRows:
           type: array
           description: arreglo de resultados de los cargos (collect) generados
           items:
             $ref: '#/components/schemas/CollectStatus'
-          
+
     CollectStatus:
       type: object
       properties:
         commerceOrder:
           type: string
           description: El número de la orden del comercio
           example: 'zc23456'
-        type: 
+        type:
           type: integer
           description: |
             Tipo de cobro:
             - 1 Cobro automático
             - 2 Cobro normal (link de pago)
             - 3 Cobro por email
           example: '1'
@@ -4012,30 +4014,30 @@
           type: integer
           description: Código de error de la fila
           example: 105
         errorMsg:
           type: string
           description: Mensaje de error de la fila
           example: 12300 has been previously paid
-       
+
     ReverseChargeResponse:
       type: object
       properties:
         status:
           type: string
           description: |
             Estado de la reversa:
             - 0 Reversa no efectuada
             - 1 Reversa efectuada
           example: '1'
         message:
           type: string
           description: Mensaje resultado de la reversa
           example: Reverse charge was successful
-          
+
     Plan:
       type: object
       properties:
         planId:
           type: string
           description: Identificador del plan
           example: myPlan01
@@ -4096,27 +4098,27 @@
           type: number
           description: |
             Si hay conversión de moneda, en qué momento hará la conversión:
             - 1 al pago
             - 2 al importe (invoice)
         status:
           type: number
-          description: | 
+          description: |
             El estado del plan:
             - 1 activo
             - 0 eliminado
           example: 1
         public:
           type: number
           description: |
             Si el Plan es de visibilidad pública, es decir, expuestos a otras aplicaciones:
             - 0 privado
             - 1 público
           example: 1
-             
+
     Subscription:
       type: object
       properties:
         subscriptionId:
           type: string
           description: Identificador de la suscripción
           example: "sus_azcyjj9ycd"
@@ -4174,15 +4176,15 @@
         trial_end:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha de término del trial.
           example: '2018-06-26 00:00:00'
         cancel_at_period_end:
           type: number
-          description: | 
+          description: |
             Si la suscripción será cancelada automáticamente al finalizar el período actual:
             - 0 No
             - 1 Si
           example: 0
         cancel_at:
           type: string
           description: Fecha de cancelación de la suscripción
@@ -4193,37 +4195,37 @@
           example: 12
         days_until_due:
           type: number
           description: Número de días pasados, después de generar un importe, para considerar el importe vencido.
           example: 3
         status:
           type: number
-          description: | 
+          description: |
             Estado de la suscripción:
             - 0 Inactivo (no iniciada)
             - 1 Activa
             - 2 En período de trial
             - 4 Cancelada
           example: 1
         morose:
           type: number
-          description: | 
+          description: |
             Si la subscripción está morosa:
             - 0 si todos los invoices está pagados.
             - 1 si uno o más invoices están vencidos.
             - 2 si uno o más invoices están pendiente de pago, pero no vencidos.
           example: 0
         discount:
           $ref: '#/components/schemas/Discount'
         invoices:
           type: array
           description: Lista de los importe efectuados a la suscripción.
           items:
             $ref: '#/components/schemas/Invoice'
-            
+
     Coupon:
       properties:
         id:
           type: number
           description: "El identificador del cupón"
           example: 166
         name:
@@ -4267,16 +4269,16 @@
           type: number
           description: "El estado del cupón, Activo = 1, Inactivo = 0"
           example: 1
         redemtions:
           type: number
           description: "El número de veces que se ha aplicado este cupón"
           example: 21
-          
-    
+
+
     Invoice:
       properties:
         id:
           type: number
           description: Identificador del importe
           example: 1034
         subscriptionId:
@@ -4316,15 +4318,15 @@
           example: '2018-07-26 00:00:00'
         attemp_count:
           type: integer
           description: Número de intentos de cobro del importe
           example: 0
         attemped:
           type: integer
-          description: | 
+          description: |
             Si este importe se cobrará:
             - 1 Se cobrará
             - 0 No se cobrará
           example: 1
         next_attemp_date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
@@ -4333,15 +4335,15 @@
         due_date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha en que este importe será considerado moroso
           example: '2018-06-30 00:00:00'
         status:
           type: integer
-          description: | 
+          description: |
             Estado del importe:
             - 0 impago
             - 1 pagado
             - 2 anulado
           example: 0
         error:
           type: integer
@@ -4373,29 +4375,29 @@
           description: Link de pago. Cuando el invoice no esta pagado
           example: https://www.flow.cl/app/web/pay.php?token=7C18C35358FEF0E33C056C719E94956D4FC9BBEL
         chargeAttemps:
           type: array
           description: Intentos de cargo fallidos
           items:
             $ref: '#/components/schemas/ChargeAttemps'
-            
+
     OutsidePayment:
       description: Objeto que muestra los datos de un pago por fuera
       type: object
       nullable: true
       properties:
         date:
           type: string
           description: Fecha del pago por fuera
           example: 2021-03-08 00:00:00
         comment:
           type: string
           description: descripción del pago por fuera
           example: Pago por caja
-          
+
     InvoiceItem:
       type: object
       properties:
         id:
           type: number
           description: Identificador del InvoiceItem
           example: 567
@@ -4416,38 +4418,38 @@
           type: string
           description: Moneda del item
           example: 'CLP'
         amount:
           type: number
           description: Monto del item
           example: 20000
-          
+
     Error:
       type: object
       properties:
         code:
           type: number
           description: Código de error
           example: 401
         message:
           type: string
           description: Mensaje de error
           example: 'Bad Request'
-          
+
     Discount:
       type: object
       description: Descuento aplicado a una Suscripción
       properties:
         id:
           type: number
           description: Identificador del descuento
           example: 181
         type:
           type: string
-          description: | 
+          description: |
             Tipo de descuento puede ser de 2 tipos
             - Subscription discount
             - Customer discount
           example: Subscription discount
         created:
           type: string
           description: Fecha de creación del descuento
@@ -4469,16 +4471,16 @@
           description: |
             Estado del descuento
             - 1 Activo
             - 0 Inactivo
           example: 1
         coupon:
           $ref: '#/components/schemas/Coupon'
-          
-    
+
+
     Settlement:
       type: object
       properties:
         id:
           type: number
           description: Identificador de la liquidación
           example: 1001
@@ -4556,16 +4558,16 @@
           items:
             $ref: '#/components/schemas/GeneralDetail'
         refundBilledDetail:
           type: array
           description: Detalle de reembolsos facturados
           items:
             $ref: '#/components/schemas/RefundDetail'
-            
-    
+
+
     SettlementSummary:
       type: object
       description: Resumen de liquidación. Si los valores se muestran con signo negativo significa que se deducen ya sea de la transferencia bancaria o de la facturación.
       properties:
         item:
           type: string
           description: Concepto del detalle
@@ -4574,15 +4576,15 @@
           type: number
           description: Monto del detalle
           example: -1000
         taxes:
           type: number
           description: Monto del impuesto si es que aplica
           example: -190
-          
+
     TransferDetail:
       type: object
       description: Detalle de transferencia bancaria
       properties:
         date:
           type: string
           format: 'yyyy-mm-dd'
@@ -4590,15 +4592,15 @@
           example: '2018-06-15'
         name:
           type: string
           description: Nombre asociado a la cuenta bancaria
           example: 'Francisco Castillo'
         bank:
           type: string
-          description: Nombre del banco 
+          description: Nombre del banco
           example: 'Banco de Chile - Edwards'
         account:
           type: string
           description: Número de la cuenta bancaria
           example: '001456700900'
         type:
           type: string
@@ -4616,22 +4618,22 @@
           type: number
           description: Monto de la transferencia bancaria
           example: 120000
         status:
           type: string
           description: Estado de la transferencia
           example: Transferida
-          
+
     PaymentDetail:
       type: object
       description: Detalle de pagos de una liquidación
       properties:
         id:
           type: number
-          description: Identificador Flow de la transacción 
+          description: Identificador Flow de la transacción
           example: 3879654
         date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha del pago
           example: '2018-06-12 16:13:39'
         subject:
@@ -4650,15 +4652,15 @@
           type: number
           description: Tasa de comision aplicada
           example: 3.35
         fee:
           type: number
           description: Monto de comisión aplicado
           example: 1960
-          
+
     GeneralDetail:
       type: object
       description: Detalle de Retención o Devolución
       properties:
         id:
           type: number
           description: Identificador
@@ -4672,15 +4674,15 @@
           type: string
           description: Concepto
           example: 'Dif IVA retenido/facturado fact 1345'
         amount:
           type: number
           description: Monto de la retención o devolución
           example: 100
-          
+
     RefundDetail:
       type: object
       description: Detalle de Reembolsos en liquidación
       properties:
         id:
           type: number
           description: Identificador del reembolso
@@ -4758,15 +4760,15 @@
             summary:
               type: object
               properties:
                 transferred:
                   type: array
                   description: Resumen de transferencia de fondos.
                   items:
-                    $ref: '#/components/schemas/SettlementSummary'    
+                    $ref: '#/components/schemas/SettlementSummary'
                 commission:
                   type: array
                   description: Resumen de comisiones
                   items:
                     $ref: '#/components/schemas/SettlementComissionSummary'
                 payment:
                   type: array
@@ -4920,15 +4922,15 @@
           example: 100
         commission:
           type: number
           description: Comisión
           example: 83.8
         taxes:
           type: number
-          description: Impuesto 
+          description: Impuesto
           example: 15.9
         balance:
           type: number
           description: Saldo
           example: 1900.3
     SettlementPaymentDetail:
       type: object
@@ -5003,15 +5005,15 @@
         taxes:
           type: number
           description: Monto del impuesto si es que aplica
           example: 190
         balance:
           type: number
           description: Monto neto
-          example: 83.80      
+          example: 83.80
     ChargeAttemps:
       type: object
       description: Intentos fallidos de cargos automáticos
       properties:
         id:
           type: number
           description: Identificador del intento
@@ -5050,15 +5052,15 @@
           type: string
           description: La descripción del error producido en el intento de cargo
           example: "This commerceOrder 1883 has been previously paid"
     Merchant:
       type: object
       description: Objeto de comercio asociado
       properties:
-        id: 
+        id:
           type: string
           description: Id de comercio asociado
           example: NEG-A
         name:
           type: string
           description: Nombre de comercio asociado
           example: Negocio A
@@ -5079,15 +5081,15 @@
           nullable: true
           description: Fecha de aprobación/rechazo
           example: "02-04-2020 11:52"
     MerchantDeleteResponse:
       type: object
       description: Objeto de comercio asociado
       properties:
-        status: 
+        status:
           type: string
-          description: Estado de la operacion 
+          description: Estado de la operacion
           example: ok
         message:
           type: string
           description: Mensaje asociado a la operacion
-          example: Merchant X deleted
+          example: Merchant X deleted
```

### Comparing `pyflowcl-1.1.2/pyflowcl/yaml_files/apiFlow.sandbox.min.yaml` & `pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.live.min.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 openapi: 3.0.0
 servers:
-  - url: 'https://sandbox.flow.cl/api'
-    description: Sandbox server (uses test data)
+  - url: 'https://www.flow.cl/api'
+    description: Production server (uses live data)
 info:
   description: |
     Referirse a https://mariofix.github.io/pyflowcl/apiFlow.yaml/ para el archivo completo
   version: "3.0.1"
   title: Flow API
   termsOfService: "https://www.flow.cl/terminos.php"
   contact:
@@ -30,21 +30,21 @@
   - name: coupon
     description: "Permite crear cupones de descuento para ser aplicados a suscripciones o clientes"
   - name: invoice
     description: 'Permite obtener los importes que se han generado por medio de las suscripciones.'
   - name: settlement
     description: 'Permite obtener las liquidaciones de pagos efectuadas por Flow'
   - name: merchant
-    description: 'Permite gestionar los comercios asociados'   
+    description: 'Permite gestionar los comercios asociados'
 paths:
   /payment/getStatus:
     get:
       tags:
         - payment
-      summary: Obtiene el estado de una orden de pago. 
+      summary: Obtiene el estado de una orden de pago.
       description: 'Este método se utiliza para obtener el estado de un pago. Se debe utilizar en la página callback del comercio para recibir notificaciones de pagos. Cada vez que el pagador efectúe un pago, **Flow** enviará vía POST una llamada a la página del comercio, pasando como parámetro un **token** que deberá utilizarse en este servicio.'
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
@@ -76,15 +76,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: error interno de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /payment/getStatusByCommerceId:
     get:
       tags:
         - payment
       summary: 'Obtiene el estado de un pago en base al commerceId'
       description: 'Este método permite obtener el estado de un pago en base al **commerceId**'
       parameters:
@@ -121,15 +121,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: error interno de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /payment/getStatusByFlowOrder:
     get:
       tags:
         - payment
       summary: 'Obtiene el estado de un pago en base al número de orden Flow'
       description: 'Este método permite obtener el estado de un pago en base al **flowOrder**'
       parameters:
@@ -167,15 +167,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: error interno de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /payment/getPayments:
     get:
       tags:
         - payment
       summary: 'Obtiene el listado de pagos recibidos en un día'
       description: 'Este método permite obtener la lista paginada de pagos recibidos en un día.Los objetos pagos de la lista tienen la misma estructura de los retornados en los servicios payment/getStatus'
       parameters:
@@ -228,15 +228,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
   /payment/getStatusExtended:
     get:
       tags:
         - payment
-      summary: Obtiene el estado extendido de una orden de pago. 
+      summary: Obtiene el estado extendido de una orden de pago.
       description: 'Este método se utiliza para obtener el estado de un pago. A diferencia del /payment/getStatus este servicio retorna el tipo de pago, los 4 últimos dígitos de la tarjeta (si el pago se hizo con tarjeta) y la información del último intento de pago. Se debe utilizar en la página callback del comercio para recibir notificaciones de pagos. Cada vez que el pagador efectúe un pago, **Flow** enviará vía POST una llamada a la página del comercio, pasando como parámetro un **token** que deberá utilizarse en este servicio.'
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
@@ -318,15 +318,15 @@
               schema:
                 $ref: '#/components/schemas/Error'
 
   /payment/create:
     post:
       tags:
         - payment
-      summary: Genera una orden de pago 
+      summary: Genera una orden de pago
       description: "Este método permite crear una orden de pago a **Flow** y recibe como respuesta la **URL** para redirigir el browser del pagador y el **token** que identifica la transacción. La url de redirección se debe formar concatenando los valores recibidos en la respuesta de la siguiente forma:\n\n **url** + \"?token=\" +**token**\n\n
       Una vez que el pagador efectúe el pago, **Flow** notificará el resultado a la página del comercio que se envió en el parámetro **urlConfirmation**."
       responses:
         '200':
           description: "url y token para redirigir el browser del pagador La url de redirección se debe formar concatenando los valores recibidos en la respuesta de la siguiente forma:\n\n **url** + \"?token=\" +**token**"
           content:
             application/json:
@@ -366,35 +366,35 @@
                   description: Monto de la orden
                   type: number
                 email:
                   description: email del pagador
                   type: string
                   format: email
                 paymentMethod:
-                  description: | 
+                  description: |
                     Identificador del medio de pago. Si se envía el identificador, el pagador será redireccionado directamente al medio de pago que se indique, de lo contrario Flow le presentará una página para seleccionarlo. El medio de pago debe haber sido previamente contratado. Podrá ver los identificadores de sus medios de pago en la sección "Mis Datos" ingresando a Flow con sus credenciales. Para indicar todos los medios de pago utilice el identificador:
                     - 9 Todos los medios
                   type: integer
                 urlConfirmation:
                   description: url callback del comercio donde Flow confirmará el pago
                   type: string
                   format: uri
                 urlReturn:
                   description: url de retorno del comercio donde Flow redirigirá al pagador
                   type: string
                   format: uri
                 optional:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 timeout:
                   description: tiempo en segundos para que una orden expire después de haber sido creada. Si no se envía este parámetro la orden no expirará y estará vigente para pago por tiempo indefinido. Si envía un valor en segundos, la orden expirará x segundos después de haber sido creada y no podrá pagarse.
                   type: integer
-                merchantId: 
+                merchantId:
                   description: Id de comercio asociado. Solo aplica si usted es comercio integrador.
                   type: string
                 payment_currency:
                   description: Moneda en que se espera se pague la orden
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
@@ -420,17 +420,17 @@
                       properties:
                         token:
                           description: hash token que identifica la transacción
                           type: string
               responses:
                 '200':
                   description: Your server returns this code if it accepts the callback
-                        
-                
-  
+
+
+
   /payment/createEmail:
     post:
       tags:
         - payment
       summary: Genera un cobro por email
       description: "Permite generar un cobro por email. **Flow** emite un email al pagador que contiene la información de la Orden de pago y el link de pago correspondiente. Una vez que el pagador efectúe el pago, **Flow** notificará el resultado a la página del comercio que se envió en el parámetro **urlConfirmation**."
       responses:
@@ -488,40 +488,40 @@
                 forward_days_after:
                   description: Número de días posteriores al envío del cobro para enviar una nueva notificación de persistencia si la orden no está pagada.
                   type: number
                 forward_times:
                   description: Número de veces de envío de mail de persistencia.
                   type: number
                 optional:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 timeout:
                   description: tiempo en segundos para que una orden expire después de haber sido creada. Si no se envía este parámetro la orden no expirará y estará vigente para pago por tiempo indefinido. Si envía un valor en segundos, la orden expirará x segundos después de haber sido creada y no podrá pagarse.
                   type: integer
-                merchantId: 
+                merchantId:
                   description: Id de comercio asociado. Solo aplica si usted es comercio integrador.
-                  type: string      
+                  type: string
                 payment_currency:
                   description: Moneda en que se espera se pague la orden
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - commerceOrder
                 - subject
                 - amount
                 - email
                 - urlConfirmation
                 - urlReturn
-                - s   
-                
+                - s
+
   /refund/create:
     post:
       tags:
         - refund
       summary: "Permite crear un reembolso"
       description: "Este servicio permite crear una orden de reembolso. Una vez que el receptor del reembolso acepte o rechaze el reembolso, **Flow** notificará vía POST a la página del comercio identificada en **urlCallback** pasando como parámetro **token**\n\n
       En esta página, el comercio debe invocar el servicio **refund/getStatus** para obtener el estado del reembolso."
@@ -577,15 +577,15 @@
               required:
                 - apiKey
                 - refundCommerceOrder
                 - receiverEmail
                 - amount
                 - urlCallBack
                 - s
-                
+
   /refund/cancel:
     post:
       tags:
         - refund
       summary: "Permite cancelar un reembolso"
       description: "Este servicio permite cancelar una orden de reembolso pendiente"
       responses:
@@ -622,21 +622,21 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - token
                 - s
-                
+
   /refund/getStatus:
     get:
       tags:
         - refund
       summary: "Obtiene el estado de un reemboso."
-      description: "Permite obtener el estado de un reembolso solicitado. Este servicio se debe invocar desde la página del comercio que se señaló en el parámetro **urlCallback** del servicio **refund/create**."  
+      description: "Permite obtener el estado de un reembolso solicitado. Este servicio se debe invocar desde la página del comercio que se señaló en el parámetro **urlCallback** del servicio **refund/create**."
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
             type: string
@@ -667,15 +667,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-          
+
   #<--- Customer
   /customer/create:
     post:
       tags:
         - customer
       summary: "Crear un cliente"
       description: "Permite crear un nuevo cliente. El servicio retorna el objeto cliente creado."
@@ -710,15 +710,15 @@
                 name:
                   description: Nombre del cliente (nombre y apellido)
                   type: string
                 email:
                   description: Email del cliente
                   type: string
                 externalId:
-                  description: Identificador externo del cliente, es decir, el identificador con el que su sistema lo reconoce. 
+                  description: Identificador externo del cliente, es decir, el identificador con el que su sistema lo reconoce.
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - name
@@ -775,15 +775,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - customerId
                 - s
-                
+
   /customer/delete:
     post:
       tags:
         - customer
       summary: "Eliminar un cliente"
       description: "Permite eliminar un cliente. Para eliminar un cliente, este no debe tener suscripciones activas o importes pendientes de pago."
       responses:
@@ -871,15 +871,15 @@
   /customer/list:
     get:
       tags:
         - customer
       summary: "Lista de clientes"
       description: "Permite obtener la lista de clientes paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del cliente\n
-      * status: filtro por estado del cliente" 
+      * status: filtro por estado del cliente"
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
             type: string
@@ -937,15 +937,15 @@
       tags:
         - customer
       summary: "Envía a un cliente a registrar su tarjeta de crédito"
       description: |
         Envía a un cliente a registrar su tarjeta de crédito para poder efectuarle cargos automáticos.
         El servicio responde con la **URL** para redirigir el browser del pagador y el **token** que identifica la transacción. La **url** de redirección se debe formar concatenando los valores recibidos en la respuesta de la siguiente forma:
           > **url** + "?token=" +**token**
-          
+
         Una vez redirigido el browser del cliente, Flow responderá por medio de una llamada POST a la url callback del comercio indicada en el parámetro **url_return** pasando como parámetro **token**. El comercio debe implementar una página y capturar el parámetro token enviado por Flow para luego consumir el servicio "customer/getRegisterStatus" para obtener el resultado del registro.
       responses:
         '200':
           description: "Url y token para redireccionar el browser del cliente a registrar su tarjeta de crédito"
           content:
             application/json:
               schema:
@@ -1032,15 +1032,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /customer/unRegister:
     post:
       tags:
         - customer
       summary: "Elimina el registro de la tarjeta de crédito de un cliente"
       description: "Este servicio permite eliminar el registro de la tarjeta de crédito de un cliente. Al eliminar el registro no se podrá hacer cargos automáticos y Flow enviará un cobro por email."
       responses:
@@ -1077,15 +1077,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - customerId
                 - s
-                
+
   /customer/charge:
     post:
       tags:
         - customer
       summary: "Efectúa un cargo en la tarjeta de crédito un cliente"
       description: "Este servicio permite efectuar un cargo automático en la tarjeta de crédito previamente registrada por el cliente. Si el cliente no tiene registrada una tarjeta el metodo retornará error."
       responses:
@@ -1128,34 +1128,34 @@
                 commerceOrder:
                   description: Identificador de la orden del comercio
                   type: string
                 currency:
                   description: Moneda del cargo (CLP, UF)
                   type: string
                 optionals:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - customerId
                 - amount
                 - subject
                 - commerceOrder
                 - s
-                
+
   /customer/collect:
     post:
       tags:
         - customer
-      summary: "Envía un cobro a un cliente." 
+      summary: "Envía un cobro a un cliente."
       description: "Este servicio envía un cobro a un cliente. Si el cliente tiene registrada una tarjeta de crédito se le hace un cargo automático, si no tiene registrada una tarjeta de credito se genera un cobro. Si se envía el parámetro byEmail = 1, se genera un cobro por email."
       responses:
         '200':
           description: El objeto CollectResponse
           content:
             application/json:
               schema:
@@ -1201,32 +1201,32 @@
                   description: url de retorno del comercio donde Flow redirigirá al pagador
                   type: string
                   format: uri
                 currency:
                   description: Moneda del cargo (CLP, UF)
                   type: string
                 paymentMethod:
-                  description: | 
+                  description: |
                     Identificador del medio de pago. Si se envía el identificador, el pagador será redireccionado directamente al medio de pago que se indique, de lo contrario Flow le presentará una página para seleccionarlo. El medio de pago debe haber sido previamente contratado. Podrá ver los identificadores de sus medios de pago en la sección "Mis Datos" ingresando a Flow con sus credenciales. Para indicar todos los medios de pago utilice el identificador:
                     - 9 Todos los medios
                   type: integer
                 byEmail:
                   description: Si se desea que Flow envíe cobros por email, este parámetro debe enviarse con valor 1
                   type: integer
                 forward_days_after:
                   description: Número de días posteriores al envío del cobro para enviar una nueva notificación de persistencia si la orden no está pagada.
                   type: integer
                 forward_times:
                   description: Número de veces de envío de mail de persistencia.
                   type: integer
                 ignore_auto_charging:
-                  description: Si se envía este parámetro con valor 1 entonces ignora el método de cargo automático aunque el cliente tenga registrada una tarjeta de crédito 
+                  description: Si se envía este parámetro con valor 1 entonces ignora el método de cargo automático aunque el cliente tenga registrada una tarjeta de crédito
                   type: integer
                 optionals:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 timeout:
                   description: tiempo en segundos para que una orden expire después de haber sido creada. Si no se envía este parámetro la orden no expirará y estará vigente para pago por tiempo indefinido. Si envía un valor en segundos, la orden expirará x segundos después de haber sido creada y no podrá pagarse.
                   type: integer
                 s:
@@ -1237,20 +1237,20 @@
                 - customerId
                 - amount
                 - subject
                 - commerceOrder
                 - urlConfirmation
                 - urlReturn
                 - s
-                
+
   /customer/batchCollect:
     post:
       tags:
         - customer
-      summary: "Envía de forma masiva un lote de cobros a  clientes." 
+      summary: "Envía de forma masiva un lote de cobros a  clientes."
       description: Este servicio envía de forma masiva un lote de cobros a clientes. Similar al servicio collect pero masivo y asíncrono. Este servicio responde con un token identificador del lote y el número de filas recibidas.
       responses:
         '200':
           description: El objeto BatchCollectResponse
           content:
             application/json:
               schema:
@@ -1358,15 +1358,15 @@
                       properties:
                         token:
                           description: hash token que identifica el pago
                           type: string
               responses:
                 '200':
                   description: Your server returns this code if it accepts the callback
-  
+
   /customer/getBatchCollectStatus:
     get:
       tags:
         - customer
       summary: "Obtiene el estado de un lote de cobros enviados por el servicio batchCollect"
       description: "Este servicio permite consultar el estado de un lote de cobros enviados por medio del servicio batchCollect."
       parameters:
@@ -1403,21 +1403,21 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /customer/reverseCharge:
     post:
       tags:
         - customer
       summary: "Reversa un cargo efectuado en la tarjeta de crédito de un cliente"
-      description: | 
+      description: |
         Este servicio permite reversar un cargo previamente efectuado a un cliente. Para que el cargo se reverse, este servicio debe ser invocado dentro de las 24 horas siguientes a efectuado el cargo, las 24 horas rigen desde las 14:00 hrs, es decir, si el cargo se efectuó a las 16:00 hrs, este puede reversarse hasta las 14:00 hrs del día siguiente.\n\n
           Puede enviar como parámetros el **commerceOrder** o el **flowOrder**.
       responses:
         '200':
           description: El objeto ReverseChargeResponse
           content:
             application/json:
@@ -1527,15 +1527,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /customer/getChargeAttemps:
     get:
       tags:
         - customer
       summary: "Lista paginada de intentos de cargos fallidos a un cliente"
       description: "Este servicio obtiene la lista paginada de los intentos de cargos fallidos a un cliente."
       parameters:
@@ -1603,15 +1603,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /customer/getSubscriptions:
     get:
       tags:
         - customer
       summary: "Lista paginada de suscripciones de un cliente"
       description: "Este servicio obtiene la lista paginada de las suscripciones de un cliente."
       parameters:
@@ -1666,15 +1666,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-       
+
   /plans/create:
     post:
       tags:
         - plans
       summary: "Crea un Plan de Suscripción"
       description: "Este servicio permite crear un nuevo Plan de Suscripción"
       responses:
@@ -1702,36 +1702,36 @@
             schema:
               type: object
               properties:
                 apiKey:
                   description: apiKey del comercio
                   type: string
                 planId:
-                  description: | 
+                  description: |
                     Identificador del Plan. Un texto identificador del Plan, sin espacios, ejemplo: PlanMensual
                   type: string
                 name:
                   description: Nombre del Plan
                   type: string
                 currency:
                   description: Moneda del Plan, por omisión CLP
                   type: string
                 amount:
                   description: Monto del Plan
                   type: number
                 interval:
-                  description: | 
+                  description: |
                     Especifica la frecuencia de cobros (generación de importe)
                       - 1 diario
                       - 2 semanal
                       - 3 mensual
                       - 4 anual
                   type: number
                 interval_count:
-                  description: | 
+                  description: |
                     Número de intervalos de frecuencia de cobros, por ejemplo:
                       - interval = 2 y interval_count = 2 la frecuancia será quincenal. El valor por omisión es 1.
                   type: number
                 trial_period_days:
                   description: Número de días de Trial. El valor por omisón es 0.
                   type: number
                 days_until_due:
@@ -1757,15 +1757,15 @@
               required:
                 - apiKey
                 - planId
                 - name
                 - amount
                 - interval
                 - s
-        
+
   /plans/get:
     get:
       tags:
         - plans
       summary: "Obtiene los datos de un Plan de Suscripción"
       description: "Este servicio permite obtener los datos de un Plan de Suscripción"
       parameters:
@@ -1849,23 +1849,23 @@
                 currency:
                   description: Moneda del Plan
                   type: string
                 amount:
                   description: Monto del Plan
                   type: number
                 interval:
-                  description: | 
+                  description: |
                     Especifica la frecuencia de cobros (generación de importe)
                       - 1 diario
                       - 2 semanal
                       - 3 mensual
                       - 4 anual
                   type: number
                 interval_count:
-                  description: | 
+                  description: |
                     Número de intervalos de frecuencia de cobros, por ejemplo:
                       - interval = 2 y interval_count = 2 la frecuancia será quincenal. El valor por omisión es 1.
                   type: number
                 trial_period_days:
                   description: Número de días de Trial. El valor por omisón es 0.
                   type: number
                 days_until_due:
@@ -1887,15 +1887,15 @@
                     - 2 al importe (invoice)
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - planId
-  
+
   /plans/delete:
     post:
       tags:
         - plans
       summary: "Elimina un Plan de Suscripción"
       description: "Este servicio permite eliminar un Plan de Suscripción. El eliminar un Plan significa que ya no podrá suscribir nuevos clientes al plan. Pero las suscripciones activas continuarán su ciclo de vida mientras estas no sean cancelas."
       responses:
@@ -1931,15 +1931,15 @@
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - planId
-  
+
   /plans/list:
     get:
       tags:
         - plans
       summary: "Lista paginada de planes de suscripción"
       description: "Permite obtener la lista de planes de suscripción paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del plan\n
@@ -1996,15 +1996,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /subscription/create:
     post:
       tags:
         - subscription
       summary: Crea una nueva suscripción a un Plan
       description: "Este servicio permite crear una nueva suscripción de un cliente a un Plan.\n
       Para crear una nueva suscripción, basta con enviar los  parámetros **planId** y **customerId**, los parámetros opcionales son:\n\n
@@ -2081,15 +2081,15 @@
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - planId
                 - customerId
                 - s
-  
+
   /subscription/get:
     get:
       tags:
         - subscription
       summary: "Obtiene una Suscripción en base al subscriptionId"
       description: "Este servicio permite obtener los datos de una suscripción."
       parameters:
@@ -2126,15 +2126,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /subscription/list:
     get:
       tags:
         - subscription
       summary: Obtiene la lista de suscripciones para un Plan
       description: "Permite obtener la lista de suscripciones paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del plan\n
@@ -2197,22 +2197,22 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-          
+
   /subscription/changeTrial:
     post:
       tags:
         - subscription
       summary: Modifica los días de Trial de una suscripción
-      description: | 
-        Este servicio permite modificar los días de Trial de una suscripción. 
+      description: |
+        Este servicio permite modificar los días de Trial de una suscripción.
         Sólo se puede modificar los días de Trial a una suscripción que aún no se ha iniciado o que todavía está vigente el Trial.
       responses:
         '200':
           description: "El objeto Subscription"
           content:
             application/json:
               schema:
@@ -2248,25 +2248,25 @@
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - trial_period_days
                 - s
-  
+
   /subscription/cancel:
     post:
       tags:
         - subscription
       summary: "Cancela una suscripción"
-      description: | 
+      description: |
         Este servicio permite cancelar una suscripción. Existen formas de cancelar una suscripción:
         - inmediatamente. Es decir, en este instante
         - al terminar el perído vigente.
-      
+
         Si desea cancelar la suscripción inmediatamente, envíe el parámetro **at_period_end** con valor 0, si desea cancelarla al final del período vigente envíe el valor 1.
       responses:
         '200':
           description: "El objeto Subscription"
           content:
             application/json:
               schema:
@@ -2301,15 +2301,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - s
-  
+
   /subscription/addCoupon:
     post:
       tags:
         - subscription
       summary: "Agrega un descuento a la suscripción"
       description: "Este servicio permite agregar un descuento a la suscripción. Si la suscripción ya tenía un descuento, será reemplazado por este."
       responses:
@@ -2337,28 +2337,28 @@
             schema:
               type: object
               properties:
                 apiKey:
                   description: apiKey del comercio
                   type: string
                 subscriptionId:
-                  description: Identificador de la suscripción 
+                  description: Identificador de la suscripción
                   type: string
                 couponId:
                   description: Identificador del cupón de descuento.
                   type: number
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - couponId
                 - s
-                
+
   /subscription/deleteCoupon:
     post:
       tags:
         - subscription
       summary: "Elimina un descuento a la suscripción"
       description: "Este servicio permite eliminar el descuento que tenga la suscripción. El eliminar el descuento de la suscripción, no elimina el descuento que podría tenar asociado el cliente."
       responses:
@@ -2395,15 +2395,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - s
-                
+
   /coupon/create:
     post:
       tags:
         - coupon
       summary: "Crea un cupón de descuento"
       description: "Este servicio permite crear un cupón de descuento"
       responses:
@@ -2431,33 +2431,33 @@
             schema:
               type: object
               properties:
                 apiKey:
                   description: apiKey del comercio
                   type: string
                 name:
-                  description: Nombre del cupón 
+                  description: Nombre del cupón
                   type: string
                 percent_off:
                   description: Porcentaje del cupon. Número entre 0 y 100. Permite 2 decimales con punto decimal. Ejemplo 10.2. No se agrega el signo %
                   type: number
                 currency:
-                  description: Moneda del descuento. Solo agregue la moneda para cupones de monto. 
+                  description: Moneda del descuento. Solo agregue la moneda para cupones de monto.
                   type: string
                 amount:
                   description: Monto del descuento
                   type: number
                 duration:
-                  description: | 
+                  description: |
                     Duración del cupón:
                     - 1 definida
                     - 0 indefinida
                   type: number
                 times:
-                  description: | 
+                  description: |
                     Si la duración del cupón es definida, este campo indica las veces de duración del cupón. Si el cupón se aplica a un cliente veces corresponderá a meses. Si l cupón se aplica a una suscripción, veces corresponderá a los períodos del Plan.
                   type: number
                 max_redemptions:
                   description: Número de veces de aplicación del cupón.
                   type: number
                 expires:
                   description: Fecha de expiración del cupón en formato yyyy-mm-dd
@@ -2465,15 +2465,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - name
                 - s
-                  
+
   /coupon/edit:
     post:
       tags:
         - coupon
       summary: Edita un cupón de descuento
       description: Este servicio permite editar un cupón de descuento. Sólo se puede editar el nombre de un cupón.
       responses:
@@ -2514,15 +2514,15 @@
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - couponId
                 - name
                 - s
-                
+
   /coupon/delete:
     post:
       tags:
         - coupon
       summary: "Elimina un cupón de descuento"
       description: "Este servicio permite eliminar un cupón de descuento. Eliminar un cupón de descuento no elimina los descuentos aplicados a clientes o suscripciones, sólo no permite volver a aplicar este cupón"
       responses:
@@ -2559,15 +2559,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - couponId
                 - s
-                
+
   /coupon/get:
     get:
       tags:
       - coupon
       summary: "Obtiene un cupón de descuento"
       description: "Este servicio permite obtener los datos de un cupón de descuento"
       parameters:
@@ -2604,15 +2604,15 @@
                   $ref: '#/components/schemas/Error'
           '401':
             description: Error de negocio
             content:
               application/json:
                 schema:
                   $ref: '#/components/schemas/Error'
-  
+
   /coupon/list:
     get:
       tags:
       - coupon
       summary: "Lista los cupones de descuento"
       description: "Este servicio permite la lista de cupones de descuento"
       parameters:
@@ -2638,15 +2638,15 @@
           name: filter
           description: Filtro por el nombre del cupón
           required: false
           schema:
             type: string
         - in: query
           name: status
-          description: | 
+          description: |
             Filtro por el estado del cupón:
             - 1 Activo
             - 0 Inactivo
           required: false
           schema:
             type: integer
         - in: query
@@ -2669,16 +2669,16 @@
                 schema:
                   $ref: '#/components/schemas/Error'
           '401':
             description: Error de negocio
             content:
               application/json:
                 schema:
-                  $ref: '#/components/schemas/Error'     
-                
+                  $ref: '#/components/schemas/Error'
+
   /invoice/get:
     get:
       tags:
         - invoice
       summary: "Obtiene los datos de un Invoice (Importe)"
       description: "Este servicio permite obtener los datos de un Importe."
       parameters:
@@ -2715,15 +2715,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-          
+
   /invoice/cancel:
     post:
       tags:
         - invoice
       summary: "Cancela un Importe (Invoice) pendiente de pago"
       description: "Este servicio permite cancelar un Importe (Invoice) pendiente de pago."
       responses:
@@ -2760,15 +2760,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - invoiceId
                 - s
-                
+
   /invoice/outsidePayment:
       post:
         tags:
           - invoice
         summary: "Ingresa un pago por fuera y da por pagado el Importe (Invoice) "
         description: "Este servicio permite dar por pagado un Importe (Invoice) cuando el pago no se realiza por Flow."
         responses:
@@ -2875,15 +2875,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /invoice/retryToCollect:
     post:
       tags:
         - invoice
       summary: "Reintenta el cobro de un invoice vencido"
       description: "Este servicio permite reintentar el cobro de un Invoice vencido."
       responses:
@@ -2968,15 +2968,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-            
+
   /settlement/getById:
     get:
       tags:
         - settlement
       summary: Obtiene la Liquidación efectuada con ese identificador
       description:  'Este método se utiliza para obtener el objeto Settlement correspondiente al identificador. <br>Nota: Si su liquidación es anterior al 01-06-2021 utilizar este servicio, en caso contrario se recomienda utilizar el servicio /settlement/getByIdv2'
       deprecated: true
@@ -3121,15 +3121,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
   /merchant/create:
     post:
       tags:
         - merchant
-      summary: Crea un comercio asociado 
+      summary: Crea un comercio asociado
       description: "Este método permite crear un nuevo comercio asociado en **Flow**"
       responses:
         '200':
           description: "Objeto con información del comercio asocioado en Flow"
           content:
             application/json:
               schema:
@@ -3173,15 +3173,15 @@
                 - name
                 - url
                 - s
   /merchant/edit:
     post:
       tags:
         - merchant
-      summary: Edita un comercio asociado 
+      summary: Edita un comercio asociado
       description: "Este método permite modificar un comercio asociado previamente creado en **Flow**"
       responses:
         '200':
           description: "Objeto con información del comercio asociado en Flow"
           content:
             application/json:
               schema:
@@ -3225,15 +3225,15 @@
                 - name
                 - url
                 - s
   /merchant/delete:
     post:
       tags:
         - merchant
-      summary: Elimina un comercio asociado 
+      summary: Elimina un comercio asociado
       description: "Este método permite eliminar un comercio asociado previamente creado en **Flow**"
       responses:
         '200':
           description: "Objeto con información de la orden generada en Flow"
           content:
             application/json:
               schema:
@@ -3269,15 +3269,15 @@
                 - apiKey
                 - id
                 - s
   /merchant/get:
     get:
       tags:
         - merchant
-      summary: Obtener comercio asociado 
+      summary: Obtener comercio asociado
       description: "Este método permite obtener la información de un comercio asociado previamente creado en **Flow**"
       responses:
         '200':
           description: "Objeto con información del comercio asocioado en Flow"
           content:
             application/json:
               schema:
@@ -3313,15 +3313,15 @@
           required: true
           schema:
             type: string
   /merchant/list:
     get:
       tags:
         - merchant
-      summary: Lista de comercios asociados 
+      summary: Lista de comercios asociados
       description: "Permite obtener la lista de comercios paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del comercio asociado\n
       * status: filtro por estado del comercio asociado"
       responses:
         '200':
           description: "Objeto con información del comercio asocioado en Flow"
           content:
@@ -3395,16 +3395,16 @@
         requestDate:
           type: string
           description: La fecha de creación de la orden
           format: 'yyyy-mm-dd hh:mm:ss'
           example: '2017-07-21 12:32:11'
         status:
           type: integer
-          description: | 
-            El estado de la order 
+          description: |
+            El estado de la order
             - 1 pendiente de pago
             - 2 pagada
             - 3 rechazada
             - 4 anulada
           example: 1
         subject:
           type: string
@@ -3523,16 +3523,16 @@
         requestDate:
           type: string
           description: La fecha de creación de la orden
           format: 'yyyy-mm-dd hh:mm:ss'
           example: '2017-07-21 12:32:11'
         status:
           type: integer
-          description: | 
-            El estado de la order 
+          description: |
+            El estado de la order
             - 1 pendiente de pago
             - 2 pagada
             - 3 rechazada
             - 4 anulada
           example: 1
         subject:
           type: string
@@ -3672,15 +3672,15 @@
           type: string
           description: token de la transacción
           example: "33373581FC32576FAF33C46FC6454B1FFEBD7E1H"
         flowOrder:
           type: number
           description: Número de order de cobro Flow
           example: 8765456
-    
+
     Customer:
       type: object
       properties:
         customerId:
           type: string
           description: Identificador del cliente
           example: cus_onoolldvec
@@ -3714,15 +3714,15 @@
         externalId:
           type: string
           description: El identificador del cliente en su negocio
           example: 14233531-8
         status:
           type: string
           description: |
-            El estado del cliente: 
+            El estado del cliente:
             - 0 Eliminado
             - 1 Activo
           example: '1'
         registerDate:
           type: string
           format: 'yyyy-mm-dd hh:mm:ss'
           description: La fecha en que el cliente registro su tarjeta de crédito.
@@ -3732,25 +3732,25 @@
       properties:
         total:
           type: number
           description: El número total de registros encontrados
           example: 200
         hasMore:
           type: boolean
-          description: | 
+          description: |
             - 1 Si existen más páginas
             - 0 Si es la última página
           example: 1
         data:
           type: array
           items:
             type: object
           description: arreglo de registros de la página
           example: '[{item list 1}{item list 2}{item list n..}'
-          
+
     RegisterResult:
       type: object
       properties:
         status:
           type: string
           description: El estado del registro
             - 1 registrado
@@ -3764,34 +3764,34 @@
           type: string
           description: Marca de la tarjeta de crédito
           example: Visa
         last4CardDigits:
           type: string
           description: Últimos 4 dígitos de la tarjeta de crédito
           example: '0366'
-          
+
     RefundStatus:
       type: object
       properties:
-        token: 
+        token:
           type: string
           description: Token del reembolso
           example: C93B4FAD6D63ED9A3F25D21E5D6DD0105FA8CAAQ
         flowRefundOrder:
           type: string
           description: Número de orden de reembolso
           example: '122767'
         date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha de solicitud de reembolso
           example: '2017-07-21 12:33:15'
         status:
           type: string
-          description: | 
+          description: |
             Estado del reembolso, los estado pueden ser:
             - created Solicitud creada
             - accepted Reembolso aceptado
             - rejected Reembolso rechazado
             - refunded Reembolso reembolsado
             - canceled Reembolso cancelado
           example: created
@@ -3799,19 +3799,19 @@
           type: number
           description: Monto del reembolso
           example: '12000.00'
         fee:
           type: number
           description: Costo del servicio de reembolso
           example: '240.00'
-          
+
     CollectResponse:
       type: object
       properties:
-        type: 
+        type:
           type: number
           description: |
             Tipo de cobro:
             - 1 Cobro automático
             - 2 Cobro normal (link de pago)
             - 3 Cobro por email
           example: '1'
@@ -3836,16 +3836,16 @@
           type: integer
           description: |
             Estado de emisión del cobro, es decir si se emitió el cobro, no indica si hubo pago:
             - 0 Cobro no emitido (uncollected)
             - 1 Cobro emitido (collected)
         paymenResult:
           $ref: '#/components/schemas/PaymentStatus'
-          
-    
+
+
     CollectObject:
       type: object
       description: Objeto de cobro para un lote de cobros
       properties:
         customerId:
           type: string
           description: Identificador del cliente en Flow
@@ -3875,15 +3875,15 @@
           description: Valores opcionales en formato JSON
           example: {"factura":"123456", "clave": "Valor"}
       required:
         - customerId
         - commerceOrder
         - subject
         - amount
-        
+
     BatchCollectResponse:
       type: object
       properties:
         token:
           type: string
           description: hash token identificador del lote recibido
           example: "33373581FC32576FAF33C46FC6454B1FFEBD7E1H"
@@ -3896,16 +3896,16 @@
           description: Número de filas de collects aceptadas
           example: '111'
         rejectedRows:
           type: array
           description: Arreglo de filas de collects rechazadas
           items:
             $ref: '#/components/schemas/BatchCollectRejectedRow'
-          
-          
+
+
     BatchCollectRejectedRow:
       type: object
       properties:
         customerId:
           type: string
           description: Identificador del cliente en Flow
           example: cus_onoolldvec
@@ -3937,15 +3937,15 @@
             - 109 The minimum amount is $value CLP
             - 110 Optional values are not in JSON format
           example: 104
         errorMsg:
           type: string
           description: descripción del error
           example: commerceOrder already sent
-          
+
     BatchCollectStatusResponse:
       type: object
       properties:
         token:
           type: string
           description: hash token identificador del lote recibido
           example: "33373581FC32576FAF33C46FC6454B1FFEBD7E1H"
@@ -3967,23 +3967,23 @@
             - processing (lote en procesamiento)
             - processed (lote procesado)
         collectRows:
           type: array
           description: arreglo de resultados de los cargos (collect) generados
           items:
             $ref: '#/components/schemas/CollectStatus'
-          
+
     CollectStatus:
       type: object
       properties:
         commerceOrder:
           type: string
           description: El número de la orden del comercio
           example: 'zc23456'
-        type: 
+        type:
           type: integer
           description: |
             Tipo de cobro:
             - 1 Cobro automático
             - 2 Cobro normal (link de pago)
             - 3 Cobro por email
           example: '1'
@@ -4012,30 +4012,30 @@
           type: integer
           description: Código de error de la fila
           example: 105
         errorMsg:
           type: string
           description: Mensaje de error de la fila
           example: 12300 has been previously paid
-       
+
     ReverseChargeResponse:
       type: object
       properties:
         status:
           type: string
           description: |
             Estado de la reversa:
             - 0 Reversa no efectuada
             - 1 Reversa efectuada
           example: '1'
         message:
           type: string
           description: Mensaje resultado de la reversa
           example: Reverse charge was successful
-          
+
     Plan:
       type: object
       properties:
         planId:
           type: string
           description: Identificador del plan
           example: myPlan01
@@ -4096,27 +4096,27 @@
           type: number
           description: |
             Si hay conversión de moneda, en qué momento hará la conversión:
             - 1 al pago
             - 2 al importe (invoice)
         status:
           type: number
-          description: | 
+          description: |
             El estado del plan:
             - 1 activo
             - 0 eliminado
           example: 1
         public:
           type: number
           description: |
             Si el Plan es de visibilidad pública, es decir, expuestos a otras aplicaciones:
             - 0 privado
             - 1 público
           example: 1
-             
+
     Subscription:
       type: object
       properties:
         subscriptionId:
           type: string
           description: Identificador de la suscripción
           example: "sus_azcyjj9ycd"
@@ -4174,15 +4174,15 @@
         trial_end:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha de término del trial.
           example: '2018-06-26 00:00:00'
         cancel_at_period_end:
           type: number
-          description: | 
+          description: |
             Si la suscripción será cancelada automáticamente al finalizar el período actual:
             - 0 No
             - 1 Si
           example: 0
         cancel_at:
           type: string
           description: Fecha de cancelación de la suscripción
@@ -4193,37 +4193,37 @@
           example: 12
         days_until_due:
           type: number
           description: Número de días pasados, después de generar un importe, para considerar el importe vencido.
           example: 3
         status:
           type: number
-          description: | 
+          description: |
             Estado de la suscripción:
             - 0 Inactivo (no iniciada)
             - 1 Activa
             - 2 En período de trial
             - 4 Cancelada
           example: 1
         morose:
           type: number
-          description: | 
+          description: |
             Si la subscripción está morosa:
             - 0 si todos los invoices está pagados.
             - 1 si uno o más invoices están vencidos.
             - 2 si uno o más invoices están pendiente de pago, pero no vencidos.
           example: 0
         discount:
           $ref: '#/components/schemas/Discount'
         invoices:
           type: array
           description: Lista de los importe efectuados a la suscripción.
           items:
             $ref: '#/components/schemas/Invoice'
-            
+
     Coupon:
       properties:
         id:
           type: number
           description: "El identificador del cupón"
           example: 166
         name:
@@ -4267,16 +4267,16 @@
           type: number
           description: "El estado del cupón, Activo = 1, Inactivo = 0"
           example: 1
         redemtions:
           type: number
           description: "El número de veces que se ha aplicado este cupón"
           example: 21
-          
-    
+
+
     Invoice:
       properties:
         id:
           type: number
           description: Identificador del importe
           example: 1034
         subscriptionId:
@@ -4316,15 +4316,15 @@
           example: '2018-07-26 00:00:00'
         attemp_count:
           type: integer
           description: Número de intentos de cobro del importe
           example: 0
         attemped:
           type: integer
-          description: | 
+          description: |
             Si este importe se cobrará:
             - 1 Se cobrará
             - 0 No se cobrará
           example: 1
         next_attemp_date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
@@ -4333,15 +4333,15 @@
         due_date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha en que este importe será considerado moroso
           example: '2018-06-30 00:00:00'
         status:
           type: integer
-          description: | 
+          description: |
             Estado del importe:
             - 0 impago
             - 1 pagado
             - 2 anulado
           example: 0
         error:
           type: integer
@@ -4373,29 +4373,29 @@
           description: Link de pago. Cuando el invoice no esta pagado
           example: https://www.flow.cl/app/web/pay.php?token=7C18C35358FEF0E33C056C719E94956D4FC9BBEL
         chargeAttemps:
           type: array
           description: Intentos de cargo fallidos
           items:
             $ref: '#/components/schemas/ChargeAttemps'
-            
+
     OutsidePayment:
       description: Objeto que muestra los datos de un pago por fuera
       type: object
       nullable: true
       properties:
         date:
           type: string
           description: Fecha del pago por fuera
           example: 2021-03-08 00:00:00
         comment:
           type: string
           description: descripción del pago por fuera
           example: Pago por caja
-          
+
     InvoiceItem:
       type: object
       properties:
         id:
           type: number
           description: Identificador del InvoiceItem
           example: 567
@@ -4416,38 +4416,38 @@
           type: string
           description: Moneda del item
           example: 'CLP'
         amount:
           type: number
           description: Monto del item
           example: 20000
-          
+
     Error:
       type: object
       properties:
         code:
           type: number
           description: Código de error
           example: 401
         message:
           type: string
           description: Mensaje de error
           example: 'Bad Request'
-          
+
     Discount:
       type: object
       description: Descuento aplicado a una Suscripción
       properties:
         id:
           type: number
           description: Identificador del descuento
           example: 181
         type:
           type: string
-          description: | 
+          description: |
             Tipo de descuento puede ser de 2 tipos
             - Subscription discount
             - Customer discount
           example: Subscription discount
         created:
           type: string
           description: Fecha de creación del descuento
@@ -4469,16 +4469,16 @@
           description: |
             Estado del descuento
             - 1 Activo
             - 0 Inactivo
           example: 1
         coupon:
           $ref: '#/components/schemas/Coupon'
-          
-    
+
+
     Settlement:
       type: object
       properties:
         id:
           type: number
           description: Identificador de la liquidación
           example: 1001
@@ -4556,16 +4556,16 @@
           items:
             $ref: '#/components/schemas/GeneralDetail'
         refundBilledDetail:
           type: array
           description: Detalle de reembolsos facturados
           items:
             $ref: '#/components/schemas/RefundDetail'
-            
-    
+
+
     SettlementSummary:
       type: object
       description: Resumen de liquidación. Si los valores se muestran con signo negativo significa que se deducen ya sea de la transferencia bancaria o de la facturación.
       properties:
         item:
           type: string
           description: Concepto del detalle
@@ -4574,15 +4574,15 @@
           type: number
           description: Monto del detalle
           example: -1000
         taxes:
           type: number
           description: Monto del impuesto si es que aplica
           example: -190
-          
+
     TransferDetail:
       type: object
       description: Detalle de transferencia bancaria
       properties:
         date:
           type: string
           format: 'yyyy-mm-dd'
@@ -4590,15 +4590,15 @@
           example: '2018-06-15'
         name:
           type: string
           description: Nombre asociado a la cuenta bancaria
           example: 'Francisco Castillo'
         bank:
           type: string
-          description: Nombre del banco 
+          description: Nombre del banco
           example: 'Banco de Chile - Edwards'
         account:
           type: string
           description: Número de la cuenta bancaria
           example: '001456700900'
         type:
           type: string
@@ -4616,22 +4616,22 @@
           type: number
           description: Monto de la transferencia bancaria
           example: 120000
         status:
           type: string
           description: Estado de la transferencia
           example: Transferida
-          
+
     PaymentDetail:
       type: object
       description: Detalle de pagos de una liquidación
       properties:
         id:
           type: number
-          description: Identificador Flow de la transacción 
+          description: Identificador Flow de la transacción
           example: 3879654
         date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha del pago
           example: '2018-06-12 16:13:39'
         subject:
@@ -4650,15 +4650,15 @@
           type: number
           description: Tasa de comision aplicada
           example: 3.35
         fee:
           type: number
           description: Monto de comisión aplicado
           example: 1960
-          
+
     GeneralDetail:
       type: object
       description: Detalle de Retención o Devolución
       properties:
         id:
           type: number
           description: Identificador
@@ -4672,15 +4672,15 @@
           type: string
           description: Concepto
           example: 'Dif IVA retenido/facturado fact 1345'
         amount:
           type: number
           description: Monto de la retención o devolución
           example: 100
-          
+
     RefundDetail:
       type: object
       description: Detalle de Reembolsos en liquidación
       properties:
         id:
           type: number
           description: Identificador del reembolso
@@ -4758,15 +4758,15 @@
             summary:
               type: object
               properties:
                 transferred:
                   type: array
                   description: Resumen de transferencia de fondos.
                   items:
-                    $ref: '#/components/schemas/SettlementSummary'    
+                    $ref: '#/components/schemas/SettlementSummary'
                 commission:
                   type: array
                   description: Resumen de comisiones
                   items:
                     $ref: '#/components/schemas/SettlementComissionSummary'
                 payment:
                   type: array
@@ -4920,15 +4920,15 @@
           example: 100
         commission:
           type: number
           description: Comisión
           example: 83.8
         taxes:
           type: number
-          description: Impuesto 
+          description: Impuesto
           example: 15.9
         balance:
           type: number
           description: Saldo
           example: 1900.3
     SettlementPaymentDetail:
       type: object
@@ -5003,15 +5003,15 @@
         taxes:
           type: number
           description: Monto del impuesto si es que aplica
           example: 190
         balance:
           type: number
           description: Monto neto
-          example: 83.80      
+          example: 83.80
     ChargeAttemps:
       type: object
       description: Intentos fallidos de cargos automáticos
       properties:
         id:
           type: number
           description: Identificador del intento
@@ -5050,15 +5050,15 @@
           type: string
           description: La descripción del error producido en el intento de cargo
           example: "This commerceOrder 1883 has been previously paid"
     Merchant:
       type: object
       description: Objeto de comercio asociado
       properties:
-        id: 
+        id:
           type: string
           description: Id de comercio asociado
           example: NEG-A
         name:
           type: string
           description: Nombre de comercio asociado
           example: Negocio A
@@ -5079,15 +5079,15 @@
           nullable: true
           description: Fecha de aprobación/rechazo
           example: "02-04-2020 11:52"
     MerchantDeleteResponse:
       type: object
       description: Objeto de comercio asociado
       properties:
-        status: 
+        status:
           type: string
-          description: Estado de la operacion 
+          description: Estado de la operacion
           example: ok
         message:
           type: string
           description: Mensaje asociado a la operacion
-          example: Merchant X deleted
+          example: Merchant X deleted
```

### Comparing `pyflowcl-1.1.2/pyflowcl/yaml_files/apiFlow.yaml` & `pyflowcl-1.2.0/pyflowcl/yaml_files/apiFlow.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,49 +6,49 @@
     description: Sandbox server (uses test data)
 info:
   description: |
     # Introducción
 
     Bienvenido a la documentacion de referencia del **API REST** de Flow!
     [REST](http://en.wikipedia.org/wiki/REST_API) es un protocolo de servicio web que se presta para un desarrollo rápido mediante el uso de la tecnología HTTP y JSON.
-    
+
     La API REST de Flow proporciona un amplio conjunto de operaciones y recursos para:
 
     - Payments (Pagos)
 
     - Customer (Clientes, cobros, cargos automáticos)
 
     - Refunds (Reembolsos)
 
     - Subscriptions (Suscripciones, cobros recurrentes)
-    
+
     - Coupons (Cupones de descuento para subscripciones)
-    
+
     - Settlement (Liquidaciones de pagos, reembolsos y comisiones,)
-    
+
     - Merchants (Gestión de comercios asociados)
-    
+
     ## Versionamiento
     La API se encuentra en constante crecimiento, añadiendo nuevos servicios y/o mejorando funcionalidades existentes para que nuestros clientes puedan sacar el mayor provecho posible a sus integraciones. Por lo mismo, cada vez que se hacen cambios en la API se considera que son <b>compatibles con la versiones anteriores</B>.
-    
+
     Ahora bien, FLOW considera los siguientes cambios como compatibles con versiones anteriores:
-    
+
     - Añadir nuevos servicios
     - Añadir nuevos parámetros opcionales a servicios existentes
     - Añadir nuevas propiedades a respuestas de servicios existentes
     - Modificar el orden de las propiedades en respuestas existentes
-    
+
     Debido a lo anterior es que instamos a nuestros clientes a que consideren estos aspectos en sus integraciones, para evitar inconvenientes con nuevas versiones.
-    
+
     Para más información en relación a los cambios pueden revisar el <a href='api_changelog.txt' download target='_blank'>API changelog</a> y suscribirse a nuestra <a href='https://groups.google.com/d/forum/api-list-flow-cl' download target='_blank'>lista de correos</a> para enterarse de anuncios de la API.
-    
+
     ## Acceso al API
 
     SI tienes una cuenta en Flow, puedes acceder al API REST mediante los siguientes endpoints:
-    
+
     <table>
       <thead>
         <tr>
           <th>Site</th>
           <th>Base URL for Rest Endpoints</th>
         </tr>
       </thead>
@@ -59,19 +59,19 @@
         </tr>
          <tr>
           <td>Sandbox</td>
           <td>https://sandbox.flow.cl/api</td>
         </tr>
       </tbody>
     </table>
-    
+
     El endpoint de Producción proporciona acceso directo para generar transacciones reales. El endpoint Sandbox permite probar su integración sin afectar los datos reales.
-    
+
     ## Autenticación y Seguridad
-    
+
     El API soporta como método de autenticación el **APIKey** y como seguridad, los datos que usted envíe siempre deberían estar firmado con su **SecretKey**. De esta forma, Flow verifica que los datos enviados le pertenecen y que no fueron adulterados durante la transmisión de red.
     Además, los datos viajan encriptados con un canal seguro mediante **SSL.**
 
     Tanto su ApiKey como su SecretKey se obtienen desde su cuenta de Flow:
     <table>
       <thead>
         <tr>
@@ -92,40 +92,40 @@
     </table>
 
     ## ¿Cómo firmar con su SecretKey?
     Se deben firmar todos los parámetros menos el parámetro **s** que es donde va la firma.
     Primero se deben ordenar los parámetros de forma alfabética ascendente en base al nombre del parámetro.
 
     Una vez ordenados, se deben concatenar en un string los parámetros de la siguiente forma:
-    
+
     Nombre_del_parametro  **valor**  nombre_del_parametro  **valor**.
-    
+
     **Ejemplo:**
-   
+
     Si sus parámetros son:
     - "apiKey" = "XXXX-XXXX-XXXX"
     - "currency" = "CLP"
     - "amount" = 5000
-    
+
     El string ordenado para firmar deberia ser:
-    
+
     **"amount5000apiKeyXXXX-XXXX-XXXXcurrencyCLP"**
-    
-    
-    
+
+
+
     El string concatenado se debe firmar con la función **hmac** utilizando el algoritmo **sha256** y su **secretKey** como llave.
-    
-    
+
+
     ### Ejemplo PHP
     Ordenando los parámetros:
     ```php
-    $params = array( 
+    $params = array(
       "apiKey" => "1F90971E-8276-4715-97FF-2BLG5030EE3B,
       "token" = "AJ089FF5467367"
-    ); 
+    );
     $keys = array_keys($params);
     sort($keys);
     ```
     Concatenando:
     ```php
     $toSign = "";
     foreach($keys as $key) {
@@ -133,35 +133,35 @@
     };
     ```
     Firmando:
     ```php
     $signature = hash_hmac('sha256', $toSign , $secretKey);
     ```
     ### Ejemplos de firmado:
-    
+
     **PHP:**
     ```php
     $sign = hash_hmac('sha256', $string_to_sign, $secretKey);
     ```
-    
+
     **Java:**
     ```java
     String sign = hmacSHA256(secretKey, string_to_sign);
     ```
 
     **Ruby:**
     ```ruby
     OpenSSL::HMAC.hexdigest(OpenSSL::Digest.new('sha256'),secret_key,string_to_sign);
     ```
 
      **Javascript:**
     ```javascript
     var sign = CryptoJS.HmacSHA256(stringToSign, secretKey);
     ```
-    
+
     ## Consumiendo servicios método GET
     Una vez obtenida la firma de los parámetros, agregue al resto de los parámetros el parámetro **s** con el valor del hash obtenido en el proceso de firma.
     ### Ejemplo PHP:
     ```php
     $url = 'https://www.flow.cl/api';
     // Agrega a la url el servicio a consumir
     $url = $url . '/payment/getStatus';
@@ -173,28 +173,28 @@
         $ch = curl_init();
         curl_setopt($ch, CURLOPT_URL, $url);
         curl_setopt($ch, CURLOPT_RETURNTRANSFER, TRUE);
         $response = curl_exec($ch);
         if($response === false) {
           $error = curl_error($ch);
           throw new Exception($error, 1);
-        } 
+        }
         $info = curl_getinfo($ch);
         if(!in_array($info['http_code'], array('200', '400', '401')) {
           throw new Exception('Unexpected error occurred. HTTP_CODE: '.$info['http_code'] , $info['http_code']);
         }
         echo $response;
         } catch (Exception $e) {
           echo 'Error: ' . $e->getCode() . ' - ' . $e->getMessage();
         }
     ```
 
     ## Consumiendo servicios método POST
     Una vez obtenida la firma de los parámetros, agregue al resto de los parámetros el parámetro **s** con el valor del hash obtenido en el proceso de firma.
-    
+
     ### Ejemplo PHP:
     ```php
     $url = 'https://www.flow.cl/api';
     // Agrega a la url el servicio a consumir
     $url = $url . '/payment/create';
     //Agrega la firma a los parámetros
     $params["s"] = $signature;
@@ -204,30 +204,30 @@
       curl_setopt($ch, CURLOPT_RETURNTRANSFER, TRUE);
       curl_setopt($ch, CURLOPT_POST, TRUE);
       curl_setopt($ch, CURLOPT_POSTFIELDS, $params);
       $response = curl_exec($ch);
       if($response === false) {
         $error = curl_error($ch);
         throw new Exception($error, 1);
-      } 
+      }
       $info = curl_getinfo($ch);
       if(!in_array($info['http_code'], array('200', '400', '401')) {
         throw new Exception('Unexpected error occurred. HTTP_CODE: '.$info['http_code'] , $info['http_code']);
       }
       echo $response;
     } catch (Exception $e) {
       echo 'Error: ' . $e->getCode() . ' - ' . $e->getMessage();
     }
     ```
 
     ## Notificaciones de Flow a su comercio
     Para todas las transaciones asíncronas **Flow** envía a su comercio notificaciones a sus páginas de callback, por medio de request via **POST**, content-type: **application/x-www-form-urlencoded**, enviando como parámetro un **token**, con este token el comercio debe invocar el servicio correspondiente que responde con los datos. Por ejemplo:
     Para crear un pago, en el servicio **payment/create** el comercio envía como uno de los parámetros **urlConfirmation**, que corresponde a la url donde **Flow** notificará el estado del pago. En esta página, el comercio recibirá el **token** y deberá invocar el servicio **payment/getStatus** para obtener el resultado del pago.
     ### Transacciones asíncronas:
-    
+
     <table>
       <thead>
         <tr>
           <th>Servicio</th>
           <th>Url callback</th>
           <th>Método para obtener el resultado</th>
         </tr>
@@ -268,15 +268,15 @@
           <td>payment/getStatus</td>
         </tr>
       </tbody>
     </table>
 
     ## Códigos de error de intentos de pago
     Al utilizar los servicios extendidos **payment/getStatusExtended** y **payment/getStatusByFlowOrderExtended** se puede obtener la información de error en el último intento de pago. Los códigos existentes son:
-    
+
     <table>
       <thead>
         <tr>
           <th>Código</th>
           <th>Descripción</th>
         </tr>
       </thead>
@@ -327,18 +327,18 @@
         </tr>
         <tr>
           <td>999</td>
           <td>Error desconocido</td>
         </tr>
       </tbody>
     </table>
-    
+
     ## Paginación
     Todos los servicios cuyo resultado son listas **Flow** entrega los resultados paginados. La cantidad de registros por página y la navegación por las distintas páginas se controlan con los siguientes parámetros:
-    
+
     <table>
       <thead>
         <tr>
           <th>Parámetro</th>
           <th>Descripción</th>
         </tr>
       </thead>
@@ -349,26 +349,26 @@
         </tr>
         <tr>
           <td>limit</td>
           <td>número de registros por página. Si se omite el valor por omisón es 10. El valor máximo es de 100 registros por página.</td>
         </tr>
       </tbody>
     </table>
-    
+
     Todos los servicios de paginación retornan un objeto JSON con los siguientes datos:
     ```
     {
       "total": número de registros totales,
       "hasMore": 1 Si hay más páginas, 0 si no hay,
       "data": [{}] arreglo con los registros
     }
     ```
-    
+
     Para recorrer las páginas, si como resultado **hasMore** es 1, entonces suma el valor del parámetro **limit** al parámetro **start** y vuelve a invocar el servicio hasta que **hasMore** retorne 0
-    
+
     ## Clientes API
     Disponemos de los siguientes clientes API Rest que facilitan la integración con Flow:
     <table>
       <thead>
         <tr>
           <th>Lenguage</th>
           <th>URL de descarga</th>
@@ -377,28 +377,28 @@
       <tbody>
         <tr>
           <td>PHP</td>
           <td><a href='https://github.com/flowcl/PHP-API-CLIENT' target='_blank'>https://github.com/flowcl/PHP-API-CLIENT</a></td>
         </tr>
       </tbody>
     </table>
-    
+
     ## Postman
     Disponemos de Collections de Postman para probar el consumo de los distintos servicios del API. Estas colecciones están agrupadas por funcionalidades y vienen con el algoritmo de firmado pre-programado.
-    
+
     **¿Que es Postman?** Postman es una herramienta que permite crear peticiones sobre APIs de una forma muy sencilla y poder, de esta manera, probar las APIs
-    
+
     Puede descargar Postman aquí: <a href='https://www.getpostman.com/downloads/' target='_blank'>Postman download</a>
-    
+
     Para utilizarlos, deberá crear **Environment** con las siguientes variables de ambiente:
     - apiKey: apiKey obtenida de su cuenta Flow
     - secretKey: secretKey obtenida de su cuenta Flow
     - Hosting: **sandbox.flow.cl** para ambiente sandbox o **www.flow.cl** para ambiente productivo.
-    
-    
+
+
     Puede descargar los archivos Collections para Postman aquí:
     <table>
       <thead>
         <tr>
           <th>Collection</th>
           <th>URL de descarga</th>
         </tr>
@@ -438,22 +438,22 @@
         </tr>
         <tr>
           <td>Flow Merchant</td>
           <td><a href='Flow Merchant.postman_collection.json' download target='_blank'>Flow Merchant.postman_collection.json</a></td>
         </tr>
       </tbody>
     </table>
-    
+
     ## Realizar pruebas en nuestro ambiente Sandbox
     Puede realizar pruebas en nuestro ambiente Sandbox para los distintos medios de pagos.
-    
+
     Para realizar pruebas de pago con Webpay o registrar una tarjeta de crédito para cargo automático utilice los siguientes datos:
-    
+
     ### Tarjeta de crédito
-    
+
     <table>
       <thead>
         <tr>
           <th>Dato</th>
           <th>Valor</th>
         </tr>
       </thead>
@@ -472,17 +472,17 @@
         </tr>
         <tr>
           <td>CVV</td>
           <td>123</td>
         </tr>
       </tbody>
     </table>
-    
+
     ### En la simulación del banco usar:
-    
+
     <table>
       <thead>
         <tr>
           <th>Dato</th>
           <th>Valor</th>
         </tr>
       </thead>
@@ -493,23 +493,23 @@
         </tr>
         <tr>
           <td>Clave</td>
           <td>123</td>
         </tr>
       </tbody>
     </table>
-    
+
     ### Para los medios de pago:
     - Servipag
     - Multicaja
     - Mach
     - Cryptocompra
-    
+
     Se presentan simuladores de pago, donde sólo debe hacer clic en el botón aceptar.
-    
+
   version: "3.0.1"
   title: Flow API
   termsOfService: "https://www.flow.cl/terminos.php"
   contact:
     email: soporte@flow.cl
   license:
     name: Apache 2.0
@@ -531,21 +531,21 @@
   - name: coupon
     description: "Permite crear cupones de descuento para ser aplicados a suscripciones o clientes"
   - name: invoice
     description: 'Permite obtener los importes que se han generado por medio de las suscripciones.'
   - name: settlement
     description: 'Permite obtener las liquidaciones de pagos efectuadas por Flow'
   - name: merchant
-    description: 'Permite gestionar los comercios asociados'   
+    description: 'Permite gestionar los comercios asociados'
 paths:
   /payment/getStatus:
     get:
       tags:
         - payment
-      summary: Obtiene el estado de una orden de pago. 
+      summary: Obtiene el estado de una orden de pago.
       description: 'Este método se utiliza para obtener el estado de un pago. Se debe utilizar en la página callback del comercio para recibir notificaciones de pagos. Cada vez que el pagador efectúe un pago, **Flow** enviará vía POST una llamada a la página del comercio, pasando como parámetro un **token** que deberá utilizarse en este servicio.'
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
@@ -577,15 +577,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: error interno de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /payment/getStatusByCommerceId:
     get:
       tags:
         - payment
       summary: 'Obtiene el estado de un pago en base al commerceId'
       description: 'Este método permite obtener el estado de un pago en base al **commerceId**'
       parameters:
@@ -622,15 +622,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: error interno de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /payment/getStatusByFlowOrder:
     get:
       tags:
         - payment
       summary: 'Obtiene el estado de un pago en base al número de orden Flow'
       description: 'Este método permite obtener el estado de un pago en base al **flowOrder**'
       parameters:
@@ -668,15 +668,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: error interno de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /payment/getPayments:
     get:
       tags:
         - payment
       summary: 'Obtiene el listado de pagos recibidos en un día'
       description: 'Este método permite obtener la lista paginada de pagos recibidos en un día.Los objetos pagos de la lista tienen la misma estructura de los retornados en los servicios payment/getStatus'
       parameters:
@@ -729,15 +729,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
   /payment/getStatusExtended:
     get:
       tags:
         - payment
-      summary: Obtiene el estado extendido de una orden de pago. 
+      summary: Obtiene el estado extendido de una orden de pago.
       description: 'Este método se utiliza para obtener el estado de un pago. A diferencia del /payment/getStatus este servicio retorna el tipo de pago, los 4 últimos dígitos de la tarjeta (si el pago se hizo con tarjeta) y la información del último intento de pago. Se debe utilizar en la página callback del comercio para recibir notificaciones de pagos. Cada vez que el pagador efectúe un pago, **Flow** enviará vía POST una llamada a la página del comercio, pasando como parámetro un **token** que deberá utilizarse en este servicio.'
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
@@ -819,15 +819,15 @@
               schema:
                 $ref: '#/components/schemas/Error'
 
   /payment/create:
     post:
       tags:
         - payment
-      summary: Genera una orden de pago 
+      summary: Genera una orden de pago
       description: "Este método permite crear una orden de pago a **Flow** y recibe como respuesta la **URL** para redirigir el browser del pagador y el **token** que identifica la transacción. La url de redirección se debe formar concatenando los valores recibidos en la respuesta de la siguiente forma:\n\n **url** + \"?token=\" +**token**\n\n
       Una vez que el pagador efectúe el pago, **Flow** notificará el resultado a la página del comercio que se envió en el parámetro **urlConfirmation**."
       responses:
         '200':
           description: "url y token para redirigir el browser del pagador La url de redirección se debe formar concatenando los valores recibidos en la respuesta de la siguiente forma:\n\n **url** + \"?token=\" +**token**"
           content:
             application/json:
@@ -867,35 +867,35 @@
                   description: Monto de la orden
                   type: number
                 email:
                   description: email del pagador
                   type: string
                   format: email
                 paymentMethod:
-                  description: | 
+                  description: |
                     Identificador del medio de pago. Si se envía el identificador, el pagador será redireccionado directamente al medio de pago que se indique, de lo contrario Flow le presentará una página para seleccionarlo. El medio de pago debe haber sido previamente contratado. Podrá ver los identificadores de sus medios de pago en la sección "Mis Datos" ingresando a Flow con sus credenciales. Para indicar todos los medios de pago utilice el identificador:
                     - 9 Todos los medios
                   type: integer
                 urlConfirmation:
                   description: url callback del comercio donde Flow confirmará el pago
                   type: string
                   format: uri
                 urlReturn:
                   description: url de retorno del comercio donde Flow redirigirá al pagador
                   type: string
                   format: uri
                 optional:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 timeout:
                   description: tiempo en segundos para que una orden expire después de haber sido creada. Si no se envía este parámetro la orden no expirará y estará vigente para pago por tiempo indefinido. Si envía un valor en segundos, la orden expirará x segundos después de haber sido creada y no podrá pagarse.
                   type: integer
-                merchantId: 
+                merchantId:
                   description: Id de comercio asociado. Solo aplica si usted es comercio integrador.
                   type: string
                 payment_currency:
                   description: Moneda en que se espera se pague la orden
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
@@ -921,17 +921,17 @@
                       properties:
                         token:
                           description: hash token que identifica la transacción
                           type: string
               responses:
                 '200':
                   description: Your server returns this code if it accepts the callback
-                        
-                
-  
+
+
+
   /payment/createEmail:
     post:
       tags:
         - payment
       summary: Genera un cobro por email
       description: "Permite generar un cobro por email. **Flow** emite un email al pagador que contiene la información de la Orden de pago y el link de pago correspondiente. Una vez que el pagador efectúe el pago, **Flow** notificará el resultado a la página del comercio que se envió en el parámetro **urlConfirmation**."
       responses:
@@ -989,40 +989,40 @@
                 forward_days_after:
                   description: Número de días posteriores al envío del cobro para enviar una nueva notificación de persistencia si la orden no está pagada.
                   type: number
                 forward_times:
                   description: Número de veces de envío de mail de persistencia.
                   type: number
                 optional:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 timeout:
                   description: tiempo en segundos para que una orden expire después de haber sido creada. Si no se envía este parámetro la orden no expirará y estará vigente para pago por tiempo indefinido. Si envía un valor en segundos, la orden expirará x segundos después de haber sido creada y no podrá pagarse.
                   type: integer
-                merchantId: 
+                merchantId:
                   description: Id de comercio asociado. Solo aplica si usted es comercio integrador.
-                  type: string		  
+                  type: string
                 payment_currency:
                   description: Moneda en que se espera se pague la orden
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - commerceOrder
                 - subject
                 - amount
                 - email
                 - urlConfirmation
                 - urlReturn
-                - s   
-                
+                - s
+
   /refund/create:
     post:
       tags:
         - refund
       summary: "Permite crear un reembolso"
       description: "Este servicio permite crear una orden de reembolso. Una vez que el receptor del reembolso acepte o rechaze el reembolso, **Flow** notificará vía POST a la página del comercio identificada en **urlCallback** pasando como parámetro **token**\n\n
       En esta página, el comercio debe invocar el servicio **refund/getStatus** para obtener el estado del reembolso."
@@ -1078,15 +1078,15 @@
               required:
                 - apiKey
                 - refundCommerceOrder
                 - receiverEmail
                 - amount
                 - urlCallBack
                 - s
-                
+
   /refund/cancel:
     post:
       tags:
         - refund
       summary: "Permite cancelar un reembolso"
       description: "Este servicio permite cancelar una orden de reembolso pendiente"
       responses:
@@ -1123,21 +1123,21 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - token
                 - s
-                
+
   /refund/getStatus:
     get:
       tags:
         - refund
       summary: "Obtiene el estado de un reemboso."
-      description: "Permite obtener el estado de un reembolso solicitado. Este servicio se debe invocar desde la página del comercio que se señaló en el parámetro **urlCallback** del servicio **refund/create**."  
+      description: "Permite obtener el estado de un reembolso solicitado. Este servicio se debe invocar desde la página del comercio que se señaló en el parámetro **urlCallback** del servicio **refund/create**."
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
             type: string
@@ -1168,15 +1168,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-          
+
   #<--- Customer
   /customer/create:
     post:
       tags:
         - customer
       summary: "Crear un cliente"
       description: "Permite crear un nuevo cliente. El servicio retorna el objeto cliente creado."
@@ -1211,15 +1211,15 @@
                 name:
                   description: Nombre del cliente (nombre y apellido)
                   type: string
                 email:
                   description: Email del cliente
                   type: string
                 externalId:
-                  description: Identificador externo del cliente, es decir, el identificador con el que su sistema lo reconoce. 
+                  description: Identificador externo del cliente, es decir, el identificador con el que su sistema lo reconoce.
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - name
@@ -1276,15 +1276,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - customerId
                 - s
-                
+
   /customer/delete:
     post:
       tags:
         - customer
       summary: "Eliminar un cliente"
       description: "Permite eliminar un cliente. Para eliminar un cliente, este no debe tener suscripciones activas o importes pendientes de pago."
       responses:
@@ -1372,15 +1372,15 @@
   /customer/list:
     get:
       tags:
         - customer
       summary: "Lista de clientes"
       description: "Permite obtener la lista de clientes paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del cliente\n
-      * status: filtro por estado del cliente" 
+      * status: filtro por estado del cliente"
       parameters:
         - in: query
           name: apiKey
           description: apiKey del comercio
           required: true
           schema:
             type: string
@@ -1438,15 +1438,15 @@
       tags:
         - customer
       summary: "Envía a un cliente a registrar su tarjeta de crédito"
       description: |
         Envía a un cliente a registrar su tarjeta de crédito para poder efectuarle cargos automáticos.
         El servicio responde con la **URL** para redirigir el browser del pagador y el **token** que identifica la transacción. La **url** de redirección se debe formar concatenando los valores recibidos en la respuesta de la siguiente forma:
           > **url** + "?token=" +**token**
-          
+
         Una vez redirigido el browser del cliente, Flow responderá por medio de una llamada POST a la url callback del comercio indicada en el parámetro **url_return** pasando como parámetro **token**. El comercio debe implementar una página y capturar el parámetro token enviado por Flow para luego consumir el servicio "customer/getRegisterStatus" para obtener el resultado del registro.
       responses:
         '200':
           description: "Url y token para redireccionar el browser del cliente a registrar su tarjeta de crédito"
           content:
             application/json:
               schema:
@@ -1533,15 +1533,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /customer/unRegister:
     post:
       tags:
         - customer
       summary: "Elimina el registro de la tarjeta de crédito de un cliente"
       description: "Este servicio permite eliminar el registro de la tarjeta de crédito de un cliente. Al eliminar el registro no se podrá hacer cargos automáticos y Flow enviará un cobro por email."
       responses:
@@ -1578,15 +1578,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - customerId
                 - s
-                
+
   /customer/charge:
     post:
       tags:
         - customer
       summary: "Efectúa un cargo en la tarjeta de crédito un cliente"
       description: "Este servicio permite efectuar un cargo automático en la tarjeta de crédito previamente registrada por el cliente. Si el cliente no tiene registrada una tarjeta el metodo retornará error."
       responses:
@@ -1629,34 +1629,34 @@
                 commerceOrder:
                   description: Identificador de la orden del comercio
                   type: string
                 currency:
                   description: Moneda del cargo (CLP, UF)
                   type: string
                 optionals:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - customerId
                 - amount
                 - subject
                 - commerceOrder
                 - s
-                
+
   /customer/collect:
     post:
       tags:
         - customer
-      summary: "Envía un cobro a un cliente." 
+      summary: "Envía un cobro a un cliente."
       description: "Este servicio envía un cobro a un cliente. Si el cliente tiene registrada una tarjeta de crédito se le hace un cargo automático, si no tiene registrada una tarjeta de credito se genera un cobro. Si se envía el parámetro byEmail = 1, se genera un cobro por email."
       responses:
         '200':
           description: El objeto CollectResponse
           content:
             application/json:
               schema:
@@ -1702,32 +1702,32 @@
                   description: url de retorno del comercio donde Flow redirigirá al pagador
                   type: string
                   format: uri
                 currency:
                   description: Moneda del cargo (CLP, UF)
                   type: string
                 paymentMethod:
-                  description: | 
+                  description: |
                     Identificador del medio de pago. Si se envía el identificador, el pagador será redireccionado directamente al medio de pago que se indique, de lo contrario Flow le presentará una página para seleccionarlo. El medio de pago debe haber sido previamente contratado. Podrá ver los identificadores de sus medios de pago en la sección "Mis Datos" ingresando a Flow con sus credenciales. Para indicar todos los medios de pago utilice el identificador:
                     - 9 Todos los medios
                   type: integer
                 byEmail:
                   description: Si se desea que Flow envíe cobros por email, este parámetro debe enviarse con valor 1
                   type: integer
                 forward_days_after:
                   description: Número de días posteriores al envío del cobro para enviar una nueva notificación de persistencia si la orden no está pagada.
                   type: integer
                 forward_times:
                   description: Número de veces de envío de mail de persistencia.
                   type: integer
                 ignore_auto_charging:
-                  description: Si se envía este parámetro con valor 1 entonces ignora el método de cargo automático aunque el cliente tenga registrada una tarjeta de crédito 
+                  description: Si se envía este parámetro con valor 1 entonces ignora el método de cargo automático aunque el cliente tenga registrada una tarjeta de crédito
                   type: integer
                 optionals:
-                  description: | 
+                  description: |
                     Datos opcionales en formato JSON clave = valor, ejemplo:
                       {"rut":"9999999-9","nombre":"cliente 1"}
                   type: string
                 timeout:
                   description: tiempo en segundos para que una orden expire después de haber sido creada. Si no se envía este parámetro la orden no expirará y estará vigente para pago por tiempo indefinido. Si envía un valor en segundos, la orden expirará x segundos después de haber sido creada y no podrá pagarse.
                   type: integer
                 s:
@@ -1738,20 +1738,20 @@
                 - customerId
                 - amount
                 - subject
                 - commerceOrder
                 - urlConfirmation
                 - urlReturn
                 - s
-                
+
   /customer/batchCollect:
     post:
       tags:
         - customer
-      summary: "Envía de forma masiva un lote de cobros a  clientes." 
+      summary: "Envía de forma masiva un lote de cobros a  clientes."
       description: Este servicio envía de forma masiva un lote de cobros a clientes. Similar al servicio collect pero masivo y asíncrono. Este servicio responde con un token identificador del lote y el número de filas recibidas.
       responses:
         '200':
           description: El objeto BatchCollectResponse
           content:
             application/json:
               schema:
@@ -1859,15 +1859,15 @@
                       properties:
                         token:
                           description: hash token que identifica el pago
                           type: string
               responses:
                 '200':
                   description: Your server returns this code if it accepts the callback
-  
+
   /customer/getBatchCollectStatus:
     get:
       tags:
         - customer
       summary: "Obtiene el estado de un lote de cobros enviados por el servicio batchCollect"
       description: "Este servicio permite consultar el estado de un lote de cobros enviados por medio del servicio batchCollect."
       parameters:
@@ -1904,21 +1904,21 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /customer/reverseCharge:
     post:
       tags:
         - customer
       summary: "Reversa un cargo efectuado en la tarjeta de crédito de un cliente"
-      description: | 
+      description: |
         Este servicio permite reversar un cargo previamente efectuado a un cliente. Para que el cargo se reverse, este servicio debe ser invocado dentro de las 24 horas siguientes a efectuado el cargo, las 24 horas rigen desde las 14:00 hrs, es decir, si el cargo se efectuó a las 16:00 hrs, este puede reversarse hasta las 14:00 hrs del día siguiente.\n\n
           Puede enviar como parámetros el **commerceOrder** o el **flowOrder**.
       responses:
         '200':
           description: El objeto ReverseChargeResponse
           content:
             application/json:
@@ -2028,15 +2028,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /customer/getChargeAttemps:
     get:
       tags:
         - customer
       summary: "Lista paginada de intentos de cargos fallidos a un cliente"
       description: "Este servicio obtiene la lista paginada de los intentos de cargos fallidos a un cliente."
       parameters:
@@ -2104,15 +2104,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /customer/getSubscriptions:
     get:
       tags:
         - customer
       summary: "Lista paginada de suscripciones de un cliente"
       description: "Este servicio obtiene la lista paginada de las suscripciones de un cliente."
       parameters:
@@ -2167,15 +2167,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-       
+
   /plans/create:
     post:
       tags:
         - plans
       summary: "Crea un Plan de Suscripción"
       description: "Este servicio permite crear un nuevo Plan de Suscripción"
       responses:
@@ -2203,36 +2203,36 @@
             schema:
               type: object
               properties:
                 apiKey:
                   description: apiKey del comercio
                   type: string
                 planId:
-                  description: | 
+                  description: |
                     Identificador del Plan. Un texto identificador del Plan, sin espacios, ejemplo: PlanMensual
                   type: string
                 name:
                   description: Nombre del Plan
                   type: string
                 currency:
                   description: Moneda del Plan, por omisión CLP
                   type: string
                 amount:
                   description: Monto del Plan
                   type: number
                 interval:
-                  description: | 
+                  description: |
                     Especifica la frecuencia de cobros (generación de importe)
                       - 1 diario
                       - 2 semanal
                       - 3 mensual
                       - 4 anual
                   type: number
                 interval_count:
-                  description: | 
+                  description: |
                     Número de intervalos de frecuencia de cobros, por ejemplo:
                       - interval = 2 y interval_count = 2 la frecuancia será quincenal. El valor por omisión es 1.
                   type: number
                 trial_period_days:
                   description: Número de días de Trial. El valor por omisón es 0.
                   type: number
                 days_until_due:
@@ -2258,15 +2258,15 @@
               required:
                 - apiKey
                 - planId
                 - name
                 - amount
                 - interval
                 - s
-        
+
   /plans/get:
     get:
       tags:
         - plans
       summary: "Obtiene los datos de un Plan de Suscripción"
       description: "Este servicio permite obtener los datos de un Plan de Suscripción"
       parameters:
@@ -2350,23 +2350,23 @@
                 currency:
                   description: Moneda del Plan
                   type: string
                 amount:
                   description: Monto del Plan
                   type: number
                 interval:
-                  description: | 
+                  description: |
                     Especifica la frecuencia de cobros (generación de importe)
                       - 1 diario
                       - 2 semanal
                       - 3 mensual
                       - 4 anual
                   type: number
                 interval_count:
-                  description: | 
+                  description: |
                     Número de intervalos de frecuencia de cobros, por ejemplo:
                       - interval = 2 y interval_count = 2 la frecuancia será quincenal. El valor por omisión es 1.
                   type: number
                 trial_period_days:
                   description: Número de días de Trial. El valor por omisón es 0.
                   type: number
                 days_until_due:
@@ -2388,15 +2388,15 @@
                     - 2 al importe (invoice)
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - planId
-  
+
   /plans/delete:
     post:
       tags:
         - plans
       summary: "Elimina un Plan de Suscripción"
       description: "Este servicio permite eliminar un Plan de Suscripción. El eliminar un Plan significa que ya no podrá suscribir nuevos clientes al plan. Pero las suscripciones activas continuarán su ciclo de vida mientras estas no sean cancelas."
       responses:
@@ -2432,15 +2432,15 @@
                   type: string
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - planId
-  
+
   /plans/list:
     get:
       tags:
         - plans
       summary: "Lista paginada de planes de suscripción"
       description: "Permite obtener la lista de planes de suscripción paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del plan\n
@@ -2497,15 +2497,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /subscription/create:
     post:
       tags:
         - subscription
       summary: Crea una nueva suscripción a un Plan
       description: "Este servicio permite crear una nueva suscripción de un cliente a un Plan.\n
       Para crear una nueva suscripción, basta con enviar los  parámetros **planId** y **customerId**, los parámetros opcionales son:\n\n
@@ -2582,15 +2582,15 @@
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - planId
                 - customerId
                 - s
-  
+
   /subscription/get:
     get:
       tags:
         - subscription
       summary: "Obtiene una Suscripción en base al subscriptionId"
       description: "Este servicio permite obtener los datos de una suscripción."
       parameters:
@@ -2627,15 +2627,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-  
+
   /subscription/list:
     get:
       tags:
         - subscription
       summary: Obtiene la lista de suscripciones para un Plan
       description: "Permite obtener la lista de suscripciones paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del plan\n
@@ -2698,22 +2698,22 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-          
+
   /subscription/changeTrial:
     post:
       tags:
         - subscription
       summary: Modifica los días de Trial de una suscripción
-      description: | 
-        Este servicio permite modificar los días de Trial de una suscripción. 
+      description: |
+        Este servicio permite modificar los días de Trial de una suscripción.
         Sólo se puede modificar los días de Trial a una suscripción que aún no se ha iniciado o que todavía está vigente el Trial.
       responses:
         '200':
           description: "El objeto Subscription"
           content:
             application/json:
               schema:
@@ -2749,25 +2749,25 @@
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - trial_period_days
                 - s
-  
+
   /subscription/cancel:
     post:
       tags:
         - subscription
       summary: "Cancela una suscripción"
-      description: | 
+      description: |
         Este servicio permite cancelar una suscripción. Existen formas de cancelar una suscripción:
         - inmediatamente. Es decir, en este instante
         - al terminar el perído vigente.
-      
+
         Si desea cancelar la suscripción inmediatamente, envíe el parámetro **at_period_end** con valor 0, si desea cancelarla al final del período vigente envíe el valor 1.
       responses:
         '200':
           description: "El objeto Subscription"
           content:
             application/json:
               schema:
@@ -2802,15 +2802,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - s
-  
+
   /subscription/addCoupon:
     post:
       tags:
         - subscription
       summary: "Agrega un descuento a la suscripción"
       description: "Este servicio permite agregar un descuento a la suscripción. Si la suscripción ya tenía un descuento, será reemplazado por este."
       responses:
@@ -2838,28 +2838,28 @@
             schema:
               type: object
               properties:
                 apiKey:
                   description: apiKey del comercio
                   type: string
                 subscriptionId:
-                  description: Identificador de la suscripción 
+                  description: Identificador de la suscripción
                   type: string
                 couponId:
                   description: Identificador del cupón de descuento.
                   type: number
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - couponId
                 - s
-                
+
   /subscription/deleteCoupon:
     post:
       tags:
         - subscription
       summary: "Elimina un descuento a la suscripción"
       description: "Este servicio permite eliminar el descuento que tenga la suscripción. El eliminar el descuento de la suscripción, no elimina el descuento que podría tenar asociado el cliente."
       responses:
@@ -2896,15 +2896,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey
                   type: string
               required:
                 - apiKey
                 - subscriptionId
                 - s
-                
+
   /coupon/create:
     post:
       tags:
         - coupon
       summary: "Crea un cupón de descuento"
       description: "Este servicio permite crear un cupón de descuento"
       responses:
@@ -2932,33 +2932,33 @@
             schema:
               type: object
               properties:
                 apiKey:
                   description: apiKey del comercio
                   type: string
                 name:
-                  description: Nombre del cupón 
+                  description: Nombre del cupón
                   type: string
                 percent_off:
                   description: Porcentaje del cupon. Número entre 0 y 100. Permite 2 decimales con punto decimal. Ejemplo 10.2. No se agrega el signo %
                   type: number
                 currency:
-                  description: Moneda del descuento. Solo agregue la moneda para cupones de monto. 
+                  description: Moneda del descuento. Solo agregue la moneda para cupones de monto.
                   type: string
                 amount:
                   description: Monto del descuento
                   type: number
                 duration:
-                  description: | 
+                  description: |
                     Duración del cupón:
                     - 1 definida
                     - 0 indefinida
                   type: number
                 times:
-                  description: | 
+                  description: |
                     Si la duración del cupón es definida, este campo indica las veces de duración del cupón. Si el cupón se aplica a un cliente veces corresponderá a meses. Si l cupón se aplica a una suscripción, veces corresponderá a los períodos del Plan.
                   type: number
                 max_redemptions:
                   description: Número de veces de aplicación del cupón.
                   type: number
                 expires:
                   description: Fecha de expiración del cupón en formato yyyy-mm-dd
@@ -2966,15 +2966,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - name
                 - s
-                  
+
   /coupon/edit:
     post:
       tags:
         - coupon
       summary: Edita un cupón de descuento
       description: Este servicio permite editar un cupón de descuento. Sólo se puede editar el nombre de un cupón.
       responses:
@@ -3015,15 +3015,15 @@
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - couponId
                 - name
                 - s
-                
+
   /coupon/delete:
     post:
       tags:
         - coupon
       summary: "Elimina un cupón de descuento"
       description: "Este servicio permite eliminar un cupón de descuento. Eliminar un cupón de descuento no elimina los descuentos aplicados a clientes o suscripciones, sólo no permite volver a aplicar este cupón"
       responses:
@@ -3060,15 +3060,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - couponId
                 - s
-                
+
   /coupon/get:
     get:
       tags:
       - coupon
       summary: "Obtiene un cupón de descuento"
       description: "Este servicio permite obtener los datos de un cupón de descuento"
       parameters:
@@ -3105,15 +3105,15 @@
                   $ref: '#/components/schemas/Error'
           '401':
             description: Error de negocio
             content:
               application/json:
                 schema:
                   $ref: '#/components/schemas/Error'
-  
+
   /coupon/list:
     get:
       tags:
       - coupon
       summary: "Lista los cupones de descuento"
       description: "Este servicio permite la lista de cupones de descuento"
       parameters:
@@ -3139,15 +3139,15 @@
           name: filter
           description: Filtro por el nombre del cupón
           required: false
           schema:
             type: string
         - in: query
           name: status
-          description: | 
+          description: |
             Filtro por el estado del cupón:
             - 1 Activo
             - 0 Inactivo
           required: false
           schema:
             type: integer
         - in: query
@@ -3170,16 +3170,16 @@
                 schema:
                   $ref: '#/components/schemas/Error'
           '401':
             description: Error de negocio
             content:
               application/json:
                 schema:
-                  $ref: '#/components/schemas/Error'     
-                
+                  $ref: '#/components/schemas/Error'
+
   /invoice/get:
     get:
       tags:
         - invoice
       summary: "Obtiene los datos de un Invoice (Importe)"
       description: "Este servicio permite obtener los datos de un Importe."
       parameters:
@@ -3216,15 +3216,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-          
+
   /invoice/cancel:
     post:
       tags:
         - invoice
       summary: "Cancela un Importe (Invoice) pendiente de pago"
       description: "Este servicio permite cancelar un Importe (Invoice) pendiente de pago."
       responses:
@@ -3261,15 +3261,15 @@
                 s:
                   description: la firma de los parámetros efectuada con su secretKey.
                   type: string
               required:
                 - apiKey
                 - invoiceId
                 - s
-                
+
   /invoice/outsidePayment:
       post:
         tags:
           - invoice
         summary: "Ingresa un pago por fuera y da por pagado el Importe (Invoice) "
         description: "Este servicio permite dar por pagado un Importe (Invoice) cuando el pago no se realiza por Flow."
         responses:
@@ -3376,15 +3376,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-                
+
   /invoice/retryToCollect:
     post:
       tags:
         - invoice
       summary: "Reintenta el cobro de un invoice vencido"
       description: "Este servicio permite reintentar el cobro de un Invoice vencido."
       responses:
@@ -3469,15 +3469,15 @@
                 $ref: '#/components/schemas/Error'
         '401':
           description: Error de negocio
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
-            
+
   /settlement/getById:
     get:
       tags:
         - settlement
       summary: Obtiene la Liquidación efectuada con ese identificador
       description:  'Este método se utiliza para obtener el objeto Settlement correspondiente al identificador. <br>Nota: Si su liquidación es anterior al 01-06-2021 utilizar este servicio, en caso contrario se recomienda utilizar el servicio /settlement/getByIdv2'
       deprecated: true
@@ -3622,15 +3622,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/Error'
   /merchant/create:
     post:
       tags:
         - merchant
-      summary: Crea un comercio asociado 
+      summary: Crea un comercio asociado
       description: "Este método permite crear un nuevo comercio asociado en **Flow**"
       responses:
         '200':
           description: "Objeto con información del comercio asocioado en Flow"
           content:
             application/json:
               schema:
@@ -3674,15 +3674,15 @@
                 - name
                 - url
                 - s
   /merchant/edit:
     post:
       tags:
         - merchant
-      summary: Edita un comercio asociado 
+      summary: Edita un comercio asociado
       description: "Este método permite modificar un comercio asociado previamente creado en **Flow**"
       responses:
         '200':
           description: "Objeto con información del comercio asociado en Flow"
           content:
             application/json:
               schema:
@@ -3726,15 +3726,15 @@
                 - name
                 - url
                 - s
   /merchant/delete:
     post:
       tags:
         - merchant
-      summary: Elimina un comercio asociado 
+      summary: Elimina un comercio asociado
       description: "Este método permite eliminar un comercio asociado previamente creado en **Flow**"
       responses:
         '200':
           description: "Objeto con información de la orden generada en Flow"
           content:
             application/json:
               schema:
@@ -3770,15 +3770,15 @@
                 - apiKey
                 - id
                 - s
   /merchant/get:
     get:
       tags:
         - merchant
-      summary: Obtener comercio asociado 
+      summary: Obtener comercio asociado
       description: "Este método permite obtener la información de un comercio asociado previamente creado en **Flow**"
       responses:
         '200':
           description: "Objeto con información del comercio asocioado en Flow"
           content:
             application/json:
               schema:
@@ -3814,15 +3814,15 @@
           required: true
           schema:
             type: string
   /merchant/list:
     get:
       tags:
         - merchant
-      summary: Lista de comercios asociados 
+      summary: Lista de comercios asociados
       description: "Permite obtener la lista de comercios paginada de acuerdo a los parámetros de paginación. Además, se puede definir los siguientes filtros:\n\n
       * filter: filtro por nombre del comercio asociado\n
       * status: filtro por estado del comercio asociado"
       responses:
         '200':
           description: "Objeto con información del comercio asocioado en Flow"
           content:
@@ -3896,16 +3896,16 @@
         requestDate:
           type: string
           description: La fecha de creación de la orden
           format: 'yyyy-mm-dd hh:mm:ss'
           example: '2017-07-21 12:32:11'
         status:
           type: integer
-          description: | 
-            El estado de la order 
+          description: |
+            El estado de la order
             - 1 pendiente de pago
             - 2 pagada
             - 3 rechazada
             - 4 anulada
           example: 1
         subject:
           type: string
@@ -4018,16 +4018,16 @@
         requestDate:
           type: string
           description: La fecha de creación de la orden
           format: 'yyyy-mm-dd hh:mm:ss'
           example: '2017-07-21 12:32:11'
         status:
           type: integer
-          description: | 
-            El estado de la order 
+          description: |
+            El estado de la order
             - 1 pendiente de pago
             - 2 pagada
             - 3 rechazada
             - 4 anulada
           example: 1
         subject:
           type: string
@@ -4167,15 +4167,15 @@
           type: string
           description: token de la transacción
           example: "33373581FC32576FAF33C46FC6454B1FFEBD7E1H"
         flowOrder:
           type: number
           description: Número de order de cobro Flow
           example: 8765456
-    
+
     Customer:
       type: object
       properties:
         customerId:
           type: string
           description: Identificador del cliente
           example: cus_onoolldvec
@@ -4209,15 +4209,15 @@
         externalId:
           type: string
           description: El identificador del cliente en su negocio
           example: 14233531-8
         status:
           type: string
           description: |
-            El estado del cliente: 
+            El estado del cliente:
             - 0 Eliminado
             - 1 Activo
           example: '1'
         registerDate:
           type: string
           format: 'yyyy-mm-dd hh:mm:ss'
           description: La fecha en que el cliente registro su tarjeta de crédito.
@@ -4227,25 +4227,25 @@
       properties:
         total:
           type: number
           description: El número total de registros encontrados
           example: 200
         hasMore:
           type: boolean
-          description: | 
+          description: |
             - 1 Si existen más páginas
             - 0 Si es la última página
           example: 1
         data:
           type: array
           items:
             type: object
           description: arreglo de registros de la página
           example: '[{item list 1}{item list 2}{item list n..}'
-          
+
     RegisterResult:
       type: object
       properties:
         status:
           type: string
           description: El estado del registro
             - 1 registrado
@@ -4259,34 +4259,34 @@
           type: string
           description: Marca de la tarjeta de crédito
           example: Visa
         last4CardDigits:
           type: string
           description: Últimos 4 dígitos de la tarjeta de crédito
           example: '0366'
-          
+
     RefundStatus:
       type: object
       properties:
-        token: 
+        token:
           type: string
           description: Token del reembolso
           example: C93B4FAD6D63ED9A3F25D21E5D6DD0105FA8CAAQ
         flowRefundOrder:
           type: string
           description: Número de orden de reembolso
           example: '122767'
         date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha de solicitud de reembolso
           example: '2017-07-21 12:33:15'
         status:
           type: string
-          description: | 
+          description: |
             Estado del reembolso, los estado pueden ser:
             - created Solicitud creada
             - accepted Reembolso aceptado
             - rejected Reembolso rechazado
             - refunded Reembolso reembolsado
             - canceled Reembolso cancelado
           example: created
@@ -4294,19 +4294,19 @@
           type: number
           description: Monto del reembolso
           example: '12000.00'
         fee:
           type: number
           description: Costo del servicio de reembolso
           example: '240.00'
-          
+
     CollectResponse:
       type: object
       properties:
-        type: 
+        type:
           type: number
           description: |
             Tipo de cobro:
             - 1 Cobro automático
             - 2 Cobro normal (link de pago)
             - 3 Cobro por email
           example: '1'
@@ -4331,16 +4331,16 @@
           type: integer
           description: |
             Estado de emisión del cobro, es decir si se emitió el cobro, no indica si hubo pago:
             - 0 Cobro no emitido (uncollected)
             - 1 Cobro emitido (collected)
         paymenResult:
           $ref: '#/components/schemas/PaymentStatus'
-          
-    
+
+
     CollectObject:
       type: object
       description: Objeto de cobro para un lote de cobros
       properties:
         customerId:
           type: string
           description: Identificador del cliente en Flow
@@ -4370,15 +4370,15 @@
           description: Valores opcionales en formato JSON
           example: {"factura":"123456", "clave": "Valor"}
       required:
         - customerId
         - commerceOrder
         - subject
         - amount
-        
+
     BatchCollectResponse:
       type: object
       properties:
         token:
           type: string
           description: hash token identificador del lote recibido
           example: "33373581FC32576FAF33C46FC6454B1FFEBD7E1H"
@@ -4391,16 +4391,16 @@
           description: Número de filas de collects aceptadas
           example: '111'
         rejectedRows:
           type: array
           description: Arreglo de filas de collects rechazadas
           items:
             $ref: '#/components/schemas/BatchCollectRejectedRow'
-          
-          
+
+
     BatchCollectRejectedRow:
       type: object
       properties:
         customerId:
           type: string
           description: Identificador del cliente en Flow
           example: cus_onoolldvec
@@ -4432,15 +4432,15 @@
             - 109 The minimum amount is $value CLP
             - 110 Optional values are not in JSON format
           example: 104
         errorMsg:
           type: string
           description: descripción del error
           example: commerceOrder already sent
-          
+
     BatchCollectStatusResponse:
       type: object
       properties:
         token:
           type: string
           description: hash token identificador del lote recibido
           example: "33373581FC32576FAF33C46FC6454B1FFEBD7E1H"
@@ -4462,23 +4462,23 @@
             - processing (lote en procesamiento)
             - processed (lote procesado)
         collectRows:
           type: array
           description: arreglo de resultados de los cargos (collect) generados
           items:
             $ref: '#/components/schemas/CollectStatus'
-          
+
     CollectStatus:
       type: object
       properties:
         commerceOrder:
           type: string
           description: El número de la orden del comercio
           example: 'zc23456'
-        type: 
+        type:
           type: integer
           description: |
             Tipo de cobro:
             - 1 Cobro automático
             - 2 Cobro normal (link de pago)
             - 3 Cobro por email
           example: '1'
@@ -4507,30 +4507,30 @@
           type: integer
           description: Código de error de la fila
           example: 105
         errorMsg:
           type: string
           description: Mensaje de error de la fila
           example: 12300 has been previously paid
-       
+
     ReverseChargeResponse:
       type: object
       properties:
         status:
           type: string
           description: |
             Estado de la reversa:
             - 0 Reversa no efectuada
             - 1 Reversa efectuada
           example: '1'
         message:
           type: string
           description: Mensaje resultado de la reversa
           example: Reverse charge was successful
-          
+
     Plan:
       type: object
       properties:
         planId:
           type: string
           description: Identificador del plan
           example: myPlan01
@@ -4591,27 +4591,27 @@
           type: number
           description: |
             Si hay conversión de moneda, en qué momento hará la conversión:
             - 1 al pago
             - 2 al importe (invoice)
         status:
           type: number
-          description: | 
+          description: |
             El estado del plan:
             - 1 activo
             - 0 eliminado
           example: 1
         public:
           type: number
           description: |
             Si el Plan es de visibilidad pública, es decir, expuestos a otras aplicaciones:
             - 0 privado
             - 1 público
           example: 1
-             
+
     Subscription:
       type: object
       properties:
         subscriptionId:
           type: string
           description: Identificador de la suscripción
           example: "sus_azcyjj9ycd"
@@ -4669,15 +4669,15 @@
         trial_end:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha de término del trial.
           example: '2018-06-26 00:00:00'
         cancel_at_period_end:
           type: number
-          description: | 
+          description: |
             Si la suscripción será cancelada automáticamente al finalizar el período actual:
             - 0 No
             - 1 Si
           example: 0
         cancel_at:
           type: string
           description: Fecha de cancelación de la suscripción
@@ -4688,37 +4688,37 @@
           example: 12
         days_until_due:
           type: number
           description: Número de días pasados, después de generar un importe, para considerar el importe vencido.
           example: 3
         status:
           type: number
-          description: | 
+          description: |
             Estado de la suscripción:
             - 0 Inactivo (no iniciada)
             - 1 Activa
             - 2 En período de trial
             - 4 Cancelada
           example: 1
         morose:
           type: number
-          description: | 
+          description: |
             Si la subscripción está morosa:
             - 0 si todos los invoices está pagados.
             - 1 si uno o más invoices están vencidos.
             - 2 si uno o más invoices están pendiente de pago, pero no vencidos.
           example: 0
         discount:
           $ref: '#/components/schemas/Discount'
         invoices:
           type: array
           description: Lista de los importe efectuados a la suscripción.
           items:
             $ref: '#/components/schemas/Invoice'
-            
+
     Coupon:
       properties:
         id:
           type: number
           description: "El identificador del cupón"
           example: 166
         name:
@@ -4762,16 +4762,16 @@
           type: number
           description: "El estado del cupón, Activo = 1, Inactivo = 0"
           example: 1
         redemtions:
           type: number
           description: "El número de veces que se ha aplicado este cupón"
           example: 21
-          
-    
+
+
     Invoice:
       properties:
         id:
           type: number
           description: Identificador del importe
           example: 1034
         subscriptionId:
@@ -4811,15 +4811,15 @@
           example: '2018-07-26 00:00:00'
         attemp_count:
           type: integer
           description: Número de intentos de cobro del importe
           example: 0
         attemped:
           type: integer
-          description: | 
+          description: |
             Si este importe se cobrará:
             - 1 Se cobrará
             - 0 No se cobrará
           example: 1
         next_attemp_date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
@@ -4828,15 +4828,15 @@
         due_date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha en que este importe será considerado moroso
           example: '2018-06-30 00:00:00'
         status:
           type: integer
-          description: | 
+          description: |
             Estado del importe:
             - 0 impago
             - 1 pagado
             - 2 anulado
           example: 0
         error:
           type: integer
@@ -4868,29 +4868,29 @@
           description: Link de pago. Cuando el invoice no esta pagado
           example: https://www.flow.cl/app/web/pay.php?token=7C18C35358FEF0E33C056C719E94956D4FC9BBEL
         chargeAttemps:
           type: array
           description: Intentos de cargo fallidos
           items:
             $ref: '#/components/schemas/ChargeAttemps'
-            
+
     OutsidePayment:
       description: Objeto que muestra los datos de un pago por fuera
       type: object
       nullable: true
       properties:
         date:
           type: string
           description: Fecha del pago por fuera
           example: 2021-03-08 00:00:00
         comment:
           type: string
           description: descripción del pago por fuera
           example: Pago por caja
-          
+
     InvoiceItem:
       type: object
       properties:
         id:
           type: number
           description: Identificador del InvoiceItem
           example: 567
@@ -4911,38 +4911,38 @@
           type: string
           description: Moneda del item
           example: 'CLP'
         amount:
           type: number
           description: Monto del item
           example: 20000
-          
+
     Error:
       type: object
       properties:
         code:
           type: number
           description: Código de error
           example: 401
         message:
           type: string
           description: Mensaje de error
           example: 'Bad Request'
-          
+
     Discount:
       type: object
       description: Descuento aplicado a una Suscripción
       properties:
         id:
           type: number
           description: Identificador del descuento
           example: 181
         type:
           type: string
-          description: | 
+          description: |
             Tipo de descuento puede ser de 2 tipos
             - Subscription discount
             - Customer discount
           example: Subscription discount
         created:
           type: string
           description: Fecha de creación del descuento
@@ -4964,16 +4964,16 @@
           description: |
             Estado del descuento
             - 1 Activo
             - 0 Inactivo
           example: 1
         coupon:
           $ref: '#/components/schemas/Coupon'
-          
-    
+
+
     Settlement:
       type: object
       properties:
         id:
           type: number
           description: Identificador de la liquidación
           example: 1001
@@ -5051,16 +5051,16 @@
           items:
             $ref: '#/components/schemas/GeneralDetail'
         refundBilledDetail:
           type: array
           description: Detalle de reembolsos facturados
           items:
             $ref: '#/components/schemas/RefundDetail'
-            
-    
+
+
     SettlementSummary:
       type: object
       description: Resumen de liquidación. Si los valores se muestran con signo negativo significa que se deducen ya sea de la transferencia bancaria o de la facturación.
       properties:
         item:
           type: string
           description: Concepto del detalle
@@ -5069,15 +5069,15 @@
           type: number
           description: Monto del detalle
           example: -1000
         taxes:
           type: number
           description: Monto del impuesto si es que aplica
           example: -190
-          
+
     TransferDetail:
       type: object
       description: Detalle de transferencia bancaria
       properties:
         date:
           type: string
           format: 'yyyy-mm-dd'
@@ -5085,15 +5085,15 @@
           example: '2018-06-15'
         name:
           type: string
           description: Nombre asociado a la cuenta bancaria
           example: 'Francisco Castillo'
         bank:
           type: string
-          description: Nombre del banco 
+          description: Nombre del banco
           example: 'Banco de Chile - Edwards'
         account:
           type: string
           description: Número de la cuenta bancaria
           example: '001456700900'
         type:
           type: string
@@ -5111,22 +5111,22 @@
           type: number
           description: Monto de la transferencia bancaria
           example: 120000
         status:
           type: string
           description: Estado de la transferencia
           example: Transferida
-          
+
     PaymentDetail:
       type: object
       description: Detalle de pagos de una liquidación
       properties:
         id:
           type: number
-          description: Identificador Flow de la transacción 
+          description: Identificador Flow de la transacción
           example: 3879654
         date:
           type: string
           format: 'yyyy-mm-dd hh:mm.ss'
           description: Fecha del pago
           example: '2018-06-12 16:13:39'
         subject:
@@ -5145,15 +5145,15 @@
           type: number
           description: Tasa de comision aplicada
           example: 3.35
         fee:
           type: number
           description: Monto de comisión aplicado
           example: 1960
-          
+
     GeneralDetail:
       type: object
       description: Detalle de Retención o Devolución
       properties:
         id:
           type: number
           description: Identificador
@@ -5167,15 +5167,15 @@
           type: string
           description: Concepto
           example: 'Dif IVA retenido/facturado fact 1345'
         amount:
           type: number
           description: Monto de la retención o devolución
           example: 100
-          
+
     RefundDetail:
       type: object
       description: Detalle de Reembolsos en liquidación
       properties:
         id:
           type: number
           description: Identificador del reembolso
@@ -5253,15 +5253,15 @@
             summary:
               type: object
               properties:
                 transferred:
                   type: array
                   description: Resumen de transferencia de fondos.
                   items:
-                    $ref: '#/components/schemas/SettlementSummary'    
+                    $ref: '#/components/schemas/SettlementSummary'
                 commission:
                   type: array
                   description: Resumen de comisiones
                   items:
                     $ref: '#/components/schemas/SettlementComissionSummary'
                 payment:
                   type: array
@@ -5415,15 +5415,15 @@
           example: 100
         commission:
           type: number
           description: Comisión
           example: 83.8
         taxes:
           type: number
-          description: Impuesto 
+          description: Impuesto
           example: 15.9
         balance:
           type: number
           description: Saldo
           example: 1900.3
     SettlementPaymentDetail:
       type: object
@@ -5498,15 +5498,15 @@
         taxes:
           type: number
           description: Monto del impuesto si es que aplica
           example: 190
         balance:
           type: number
           description: Monto neto
-          example: 83.80      
+          example: 83.80
     ChargeAttemps:
       type: object
       description: Intentos fallidos de cargos automáticos
       properties:
         id:
           type: number
           description: Identificador del intento
@@ -5545,15 +5545,15 @@
           type: string
           description: La descripción del error producido en el intento de cargo
           example: "This commerceOrder 1883 has been previously paid"
     Merchant:
       type: object
       description: Objeto de comercio asociado
       properties:
-        id: 
+        id:
           type: string
           description: Id de comercio asociado
           example: NEG-A
         name:
           type: string
           description: Nombre de comercio asociado
           example: Negocio A
@@ -5574,15 +5574,15 @@
           nullable: true
           description: Fecha de aprobación/rechazo
           example: "02-04-2020 11:52"
     MerchantDeleteResponse:
       type: object
       description: Objeto de comercio asociado
       properties:
-        status: 
+        status:
           type: string
-          description: Estado de la operacion 
+          description: Estado de la operacion
           example: ok
         message:
           type: string
           description: Mensaje asociado a la operacion
-          example: Merchant X deleted
+          example: Merchant X deleted
```

### Comparing `pyflowcl-1.1.2/PKG-INFO` & `pyflowcl-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,48 @@
 Metadata-Version: 2.1
 Name: pyflowcl
-Version: 1.1.2
+Version: 1.2.0
 Summary: Cliente para comunicacion con flowAPI-3 de flow.cl
-Home-page: https://github.com/mariofix/pyflowcl
+Home-page: https://www.flow.cl/docs/api.html
 License: MIT
+Keywords: plataforma de pagos,pagos,pagar,cobrar,ecommerce,tarjetas,credito,debito,redcompra,webpay,visa,mastercard,transbank
 Author: Mario Hernandez
 Author-email: yo@mariofix.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.5,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: openapi3 (>=1.7.0,<2.0.0)
-Requires-Dist: python-fsutil (>=0.7.0,<0.8.0)
-Requires-Dist: python-slugify (>=7.0.0,<8.0.0)
-Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: certifi
+Requires-Dist: openapi3 (==1.8.1)
+Requires-Dist: python-fsutil (==0.10.0)
+Requires-Dist: python-slugify (==8.0.1)
+Requires-Dist: pyyaml (==6.0.1)
+Requires-Dist: requests (==2.31.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://mariofix.github.io/pyflowcl/
 Project-URL: Repository, https://github.com/mariofix/pyflowcl
 Description-Content-Type: text/markdown
 
 PyFlowCL
 ============
-Cliente API para operaciones con el servicio de pagos Flow.cl  [FlowAPI-3.0.1](https://www.flow.cl/docs/api.html)  
-Frunciona como wrapper sobre cliente [OpenAPI3] (https://github.com/Dorthu/openapi3)  
+Cliente API para operaciones con el servicio de pagos Flow.cl  [FlowAPI-3.0.1](https://www.flow.cl/docs/api.html)
+Frunciona como wrapper sobre cliente [OpenAPI3] (https://github.com/Dorthu/openapi3)
 
-[![pyflowcl-tests](https://github.com/mariofix/pyflowcl/actions/workflows/pyflowcl.yml/badge.svg?branch=dev)](https://github.com/mariofix/pyflowcl/actions/workflows/pyflowcl.yml)
-[![PyPI version](https://badge.fury.io/py/pyflowcl.svg)](https://badge.fury.io/py/pyflowcl)
+[![pyflowcl-tests](https://github.com/mariofix/pyflowcl/actions/workflows/pyflowcl.yml/badge.svg?branch=dev)](https://github.com/mariofix/pyflowcl/actions/workflows/pyflowcl.yml) [![PyPI version](https://badge.fury.io/py/pyflowcl.svg)](https://badge.fury.io/py/pyflowcl)
 ---
 
-## Instalación
-Este proyecto está desarrollado para Python 3.7 y superior.  
-Este proyecto es administrado por Poetry.  
-
-
-```bash
-# con Poetry
-$ poetry add pyflowcl
-# con PIP
-$ pip install pyflowcl
-```
-
-
-## Uso
-APIKey y SecretKey pueden ser configurados de dos maneras
-
-### Usando el constructor
-```python
-from pyflowcl import FlowAPI
 
-flow = FlowAPI(flow_key="key", flow_secret="secret")
-```
-
-### Usando variables de entorno
-
-```bash
-export PYFLOWCL_KEY="key"
-export PYFLOWCL_SECRET="SECRET"
-python cliente_flow.py
-```
-
-
-### Cliente Antiguo
-
-```python
-from pyflowcl import Payment
-from pyflowcl.Clients import ApiClient
-
-API_URL = "https://www.flow.cl/api"
-API_KEY = "your_key"
-API_SECRET = "your_secret"
-FLOW_TOKEN = "your_payment_token"
-api = ApiClient(API_URL, API_KEY, API_SECRET)
-
-call = Payment.getStatus(api, FLOW_TOKEN)
-print(call)
-```
 
 ---
 
 ## Licencia
->Puedes revisar el texto completo de la licencia [aqui](https://github.com/mariofix/pyflowcl/blob/stable-v3/LICENSE)
+>Puedes revisar el [texto completo de la licencia](https://github.com/mariofix/pyflowcl/blob/main/LICENSE)
 
-Este proyecto está licenciado bajo los términos de la licencia **MIT**.  
+Este proyecto está licenciado bajo los términos de la licencia **MIT**.
 FlowAPI está licenciado bajo los términos de la licencia **Apache 2.0**.
+
```

