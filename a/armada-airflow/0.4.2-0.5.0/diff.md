# Comparing `tmp/armada_airflow-0.4.2-py3-none-any.whl.zip` & `tmp/armada_airflow-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 19901 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-14 16:02 armada/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-14 16:08 armada/jobservice/__init__.py
--rw-r--r--  2.0 unx     2891 b- defN 23-Jul-14 16:08 armada/jobservice/jobservice_pb2.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Jul-14 16:08 armada/jobservice/jobservice_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-14 16:02 armada/operators/__init__.py
--rw-r--r--  2.0 unx     5544 b- defN 23-Jul-14 16:02 armada/operators/armada.py
--rw-r--r--  2.0 unx    12637 b- defN 23-Jul-14 16:02 armada/operators/armada_deferrable.py
--rw-r--r--  2.0 unx     3044 b- defN 23-Jul-14 16:02 armada/operators/jobservice.py
--rw-r--r--  2.0 unx     2613 b- defN 23-Jul-14 16:02 armada/operators/jobservice_asyncio.py
--rw-r--r--  2.0 unx    10090 b- defN 23-Jul-14 16:02 armada/operators/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-14 16:15 armada_airflow-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3916 b- defN 23-Jul-14 16:15 armada_airflow-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 16:15 armada_airflow-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-14 16:15 armada_airflow-0.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1290 b- defN 23-Jul-14 16:15 armada_airflow-0.4.2.dist-info/RECORD
-15 files, 57603 bytes uncompressed, 17739 bytes compressed:  69.2%
+Zip file size: 20367 bytes, number of entries: 16
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 22:08 armada/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 22:10 armada/jobservice/__init__.py
+-rw-r--r--  2.0 unx     2891 b- defN 23-Jul-21 22:10 armada/jobservice/jobservice_pb2.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Jul-21 22:10 armada/jobservice/jobservice_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 22:08 armada/operators/__init__.py
+-rw-r--r--  2.0 unx     6081 b- defN 23-Jul-21 22:08 armada/operators/armada.py
+-rw-r--r--  2.0 unx     9671 b- defN 23-Jul-21 22:08 armada/operators/armada_deferrable.py
+-rw-r--r--  2.0 unx     3080 b- defN 23-Jul-21 22:08 armada/operators/grpc.py
+-rw-r--r--  2.0 unx     3044 b- defN 23-Jul-21 22:08 armada/operators/jobservice.py
+-rw-r--r--  2.0 unx     2613 b- defN 23-Jul-21 22:08 armada/operators/jobservice_asyncio.py
+-rw-r--r--  2.0 unx    10090 b- defN 23-Jul-21 22:08 armada/operators/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3916 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1370 b- defN 23-Jul-21 22:18 armada_airflow-0.5.0.dist-info/RECORD
+16 files, 58334 bytes uncompressed, 18081 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -15,32 +15,35 @@
 
 Filename: armada/operators/armada.py
 Comment: 
 
 Filename: armada/operators/armada_deferrable.py
 Comment: 
 
+Filename: armada/operators/grpc.py
+Comment: 
+
 Filename: armada/operators/jobservice.py
 Comment: 
 
 Filename: armada/operators/jobservice_asyncio.py
 Comment: 
 
 Filename: armada/operators/utils.py
 Comment: 
 
-Filename: armada_airflow-0.4.2.dist-info/LICENSE
+Filename: armada_airflow-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: armada_airflow-0.4.2.dist-info/METADATA
+Filename: armada_airflow-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: armada_airflow-0.4.2.dist-info/WHEEL
+Filename: armada_airflow-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: armada_airflow-0.4.2.dist-info/top_level.txt
+Filename: armada_airflow-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: armada_airflow-0.4.2.dist-info/RECORD
+Filename: armada_airflow-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## armada/operators/armada.py

```diff
@@ -22,15 +22,19 @@
 from airflow.models import BaseOperator
 from airflow.exceptions import AirflowException
 from airflow.utils.context import Context
 
 from armada_client.armada.submit_pb2 import JobSubmitRequestItem
 from armada_client.client import ArmadaClient
 
-from armada.operators.jobservice import JobServiceClient
+from armada.operators.grpc import GrpcChannelArgsDict, GrpcChannelArguments
+from armada.operators.jobservice import (
+    JobServiceClient,
+    default_jobservice_channel_options,
+)
 from armada.operators.utils import (
     airflow_error,
     search_for_job_complete,
     annotate_job_request_items,
 )
 from armada.jobservice import jobservice_pb2
 
@@ -45,17 +49,18 @@
 class ArmadaOperator(BaseOperator):
     """
     Implementation of an ArmadaOperator for airflow.
 
     Airflow operators inherit from BaseOperator.
 
     :param name: The name of the airflow task
-    :param armada_client: The Armada Python GRPC client
-                        that is used for interacting with Armada
-    :param job_service_client: The JobServiceClient that is used for polling
+    :param armada_channel_args: GRPC channel arguments to be used when creating
+      a grpc channel to connect to the armada server instance.
+    :param job_service_channel_args: GRPC channel arguments to be used when creating
+      a grpc channel to connect to the job service instance.
     :param armada_queue: The queue name for Armada.
     :param job_request_items: A PodSpec that is used by Armada for submitting a job
     :param lookout_url_template: A URL template to be used to provide users
         a valid link to the related lookout job in this operator's log.
         The format should be:
         "https://lookout.armada.domain/jobs?job_id=<job_id>" where <job_id> will
         be replaced with the actual job ID.
@@ -64,26 +69,29 @@
     """
 
     template_fields: Sequence[str] = ("job_request_items",)
 
     def __init__(
         self,
         name: str,
-        armada_client: ArmadaClient,
-        job_service_client: JobServiceClient,
+        armada_channel_args: GrpcChannelArgsDict,
+        job_service_channel_args: GrpcChannelArgsDict,
         armada_queue: str,
         job_request_items: List[JobSubmitRequestItem],
         lookout_url_template: Optional[str] = None,
         poll_interval: int = 30,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.name = name
-        self.armada_client = armada_client
-        self.job_service = job_service_client
+        self.armada_channel_args = GrpcChannelArguments(**armada_channel_args)
+
+        if "options" not in job_service_channel_args:
+            job_service_channel_args["options"] = default_jobservice_channel_options
+
         self.armada_queue = armada_queue
         self.job_request_items = job_request_items
         self.lookout_url_template = lookout_url_template
         self.poll_interval = poll_interval
 
     def execute(self, context) -> None:
         """
@@ -91,22 +99,25 @@
 
         Runs an Armada job and calls the job_service_client for polling.
 
         :param context: The airflow context.
 
         :return: None
         """
+        job_service_client = JobServiceClient(self.job_service_channel_args.channel())
         # Health Check
-        health = self.job_service.health()
+        health = job_service_client.health()
         if health.status != jobservice_pb2.HealthCheckResponse.SERVING:
             armada_logger.warn("Armada Job Service is not health")
         # This allows us to use a unique id from airflow
         # and have all jobs in a dag correspond to same jobset
         job_set_id = context["run_id"]
-        job = self.armada_client.submit_jobs(
+
+        armada_client = ArmadaClient(channel=self.armada_channel_args.channel())
+        job = armada_client.submit_jobs(
             queue=self.armada_queue,
             job_set_id=job_set_id,
             job_request_items=annotate_job_request_items(
                 context, self.job_request_items
             ),
         )
 
@@ -118,15 +129,15 @@
         armada_logger.info("Running Armada job %s with id %s", self.name, job_id)
 
         lookout_url = self._get_lookout_url(job_id)
         if len(lookout_url) > 0:
             armada_logger.info("Lookout URL: %s", lookout_url)
 
         job_state, job_message = search_for_job_complete(
-            job_service_client=self.job_service,
+            job_service_client=job_service_client,
             armada_queue=self.armada_queue,
             job_set_id=job_set_id,
             airflow_task_name=self.name,
             job_id=job_id,
             poll_interval=self.poll_interval,
         )
         armada_logger.info(
```

## armada/operators/armada_deferrable.py

```diff
@@ -13,30 +13,29 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import logging
-from typing import Optional, Sequence, Tuple, Any, TypedDict, List
-
-import grpc
+from typing import Optional, Sequence, List
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 from airflow.utils.context import Context
 
 from armada_client.armada.submit_pb2 import JobSubmitRequestItem
 from armada_client.client import ArmadaClient
 
 from armada.operators.jobservice import (
     JobServiceClient,
     default_jobservice_channel_options,
 )
+from armada.operators.grpc import GrpcChannelArgsDict, GrpcChannelArguments
 from armada.operators.jobservice_asyncio import JobServiceAsyncIOClient
 from armada.operators.utils import (
     airflow_error,
     search_for_job_complete_async,
     annotate_job_request_items,
 )
 from armada.jobservice import jobservice_pb2
@@ -45,25 +44,14 @@
 
 import jinja2
 
 
 armada_logger = logging.getLogger("airflow.task")
 
 
-class GrpcChannelArgsDict(TypedDict):
-    """
-    Helper class to provide stronger type checking on Grpc channel arugments.
-    """
-
-    target: str
-    credentials: Optional[grpc.ChannelCredentials]
-    options: Optional[Sequence[Tuple[str, Any]]]
-    compression: Optional[grpc.Compression]
-
-
 class ArmadaDeferrableOperator(BaseOperator):
     """
     Implementation of a deferrable armada operator for airflow.
 
     Distinguished from ArmadaOperator by its ability to defer itself after
     submitting its job_request_items.
 
@@ -268,92 +256,7 @@
             armada_queue=self.armada_queue,
             job_set_id=self.job_set_id,
             airflow_task_name=self.airflow_task_name,
             job_id=self.job_id,
             log=self.log,
         )
         yield TriggerEvent({"job_state": job_state, "job_message": job_message})
-
-
-class GrpcChannelArguments(object):
-    """
-    A Serializable GRPC Arguments Object.
-
-    :param target: Target keyword argument used
-        when instantiating a grpc channel.
-    :param credentials: credentials keyword argument used
-        when instantiating a grpc channel.
-    :param options: options keyword argument used
-        when instantiating a grpc channel.
-    :param compression: compression keyword argument used
-        when instantiating a grpc channel.
-    :return: a GrpcChannelArguments instance
-    """
-
-    def __init__(
-        self,
-        target: str,
-        credentials: Optional[grpc.ChannelCredentials] = None,
-        options: Optional[Sequence[Tuple[str, Any]]] = None,
-        compression: Optional[grpc.Compression] = None,
-    ) -> None:
-        self.target = target
-        self.credentials = credentials
-        self.options = options
-        self.compression = compression
-
-    def channel(self) -> grpc.Channel:
-        """
-        Create a grpc.Channel based on arguments supplied to this object.
-
-        :return: Return grpc.insecure_channel if credentials is None. Otherwise
-            returns grpc.secure_channel.
-        """
-
-        if self.credentials is None:
-            return grpc.insecure_channel(
-                target=self.target,
-                options=self.options,
-                compression=self.compression,
-            )
-        return grpc.secure_channel(
-            target=self.target,
-            credentials=self.credentials,
-            options=self.options,
-            compression=self.compression,
-        )
-
-    def aio_channel(self) -> grpc.aio.Channel:
-        """
-        Create a grpc.aio.Channel (asyncio) based on arguments supplied to this object.
-
-        :return: Return grpc.aio.insecure_channel if credentials is None. Otherwise
-            returns grpc.aio.secure_channel.
-        """
-
-        if self.credentials is None:
-            return grpc.aio.insecure_channel(
-                target=self.target,
-                options=self.options,
-                compression=self.compression,
-            )
-        return grpc.aio.secure_channel(
-            target=self.target,
-            credentials=self.credentials,
-            options=self.options,
-            compression=self.compression,
-        )
-
-    def serialize(self) -> dict:
-        """
-        Get a serialized version of this object.
-
-        :return: A dict of keyword arguments used when calling
-            a grpc channel or instantiating this object.
-        """
-
-        return {
-            "target": self.target,
-            "credentials": self.credentials,
-            "options": self.options,
-            "compression": self.compression,
-        }
```

## Comparing `armada_airflow-0.4.2.dist-info/LICENSE` & `armada_airflow-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `armada_airflow-0.4.2.dist-info/METADATA` & `armada_airflow-0.5.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armada-airflow
-Version: 0.4.2
+Version: 0.5.0
 Summary: Armada Airflow Operator
 Author-email: Armada-GROSS <armada@armadaproject.io>
 License: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: armada-client
```

## Comparing `armada_airflow-0.4.2.dist-info/RECORD` & `armada_airflow-0.5.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 armada/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/jobservice_pb2.py,sha256=idcVXwvH0EeYCcyBcloshRhh_JQhCpLn5a2-LPqkxIU,2891
 armada/jobservice/jobservice_pb2_grpc.py,sha256=ApiwP6_oYV8oHFlRC7oFum3I0aeEFQ9RE-7cNuaUmOk,4122
 armada/operators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-armada/operators/armada.py,sha256=kMsanRTjwqhuhAdMqZpkJNWwML60gorOgc6rHxwInNs,5544
-armada/operators/armada_deferrable.py,sha256=VAp0Oh3XtCipPbTcuERuRlzAYmI_evse1HhcqoSy8QM,12637
+armada/operators/armada.py,sha256=b_0OVumrM9wkKP7g27INyoJUIS1itmBbsm_KsY7DNjM,6081
+armada/operators/armada_deferrable.py,sha256=ggadgIswvrd2tA0D3aT86_jSEPvnRxRfDyg_fSppYtI,9671
+armada/operators/grpc.py,sha256=o9X4HhUdjVJIjhsLZNtjLRGubr7bYQRFCkUH7LD2lXw,3080
 armada/operators/jobservice.py,sha256=_Rrrmz6NqbEeATWegdabjMv7y7dEGUzWy5hgKS23-8o,3044
 armada/operators/jobservice_asyncio.py,sha256=DmtzNfSroAheBj-pAOeUZ6lZcx4UItUNt08DFvH3cIA,2613
 armada/operators/utils.py,sha256=ZKgFazRLXNp__htb-ZqLkWW95rm6Z5VNvtNmxCzkyQw,10090
-armada_airflow-0.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-armada_airflow-0.4.2.dist-info/METADATA,sha256=b7l4gnkinGr9OJtVt_ulUim8Zqkx1n3-j0YNLEFBEBM,3916
-armada_airflow-0.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-armada_airflow-0.4.2.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
-armada_airflow-0.4.2.dist-info/RECORD,,
+armada_airflow-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+armada_airflow-0.5.0.dist-info/METADATA,sha256=K_8M-DkTXpo5qbCAz6XO3-NM2UrsGFFzDTlC1Dhwmf8,3916
+armada_airflow-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+armada_airflow-0.5.0.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
+armada_airflow-0.5.0.dist-info/RECORD,,
```

