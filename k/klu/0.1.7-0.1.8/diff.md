# Comparing `tmp/klu-0.1.7.tar.gz` & `tmp/klu-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klu-0.1.7.tar", max compression
+gzip compressed data, was "klu-0.1.8.tar", max compression
```

## Comparing `klu-0.1.7.tar` & `klu-0.1.8.tar`

### file list

```diff
@@ -1,54 +1,59 @@
--rw-r--r--   0        0        0     1070 2023-06-03 17:41:15.902941 klu-0.1.7/LICENSE
--rw-r--r--   0        0        0     2840 2023-06-03 17:41:15.902941 klu-0.1.7/README.md
--rw-r--r--   0        0        0      150 2023-06-03 17:41:15.902941 klu-0.1.7/klu/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/__init__.py
--rw-r--r--   0        0        0    11322 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/client.py
--rw-r--r--   0        0        0      280 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/constants.py
--rw-r--r--   0        0        0      547 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/errors.py
--rw-r--r--   0        0        0     1980 2023-06-03 17:41:15.902941 klu-0.1.7/klu/action/models.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/__init__.py
--rw-r--r--   0        0        0     2998 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/client.py
--rw-r--r--   0        0        0      199 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/config.py
--rw-r--r--   0        0        0      118 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/constants.py
--rw-r--r--   0        0        0     1406 2023-06-03 17:41:15.902941 klu-0.1.7/klu/api/sse_client.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/__init__.py
--rw-r--r--   0        0        0     7753 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/client.py
--rw-r--r--   0        0        0      259 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/constants.py
--rw-r--r--   0        0        0      318 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/errors.py
--rw-r--r--   0        0        0     1464 2023-06-03 17:41:15.902941 klu-0.1.7/klu/application/models.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/client/__init__.py
--rw-r--r--   0        0        0      794 2023-06-03 17:41:15.902941 klu-0.1.7/klu/client/klu.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/common/__init__.py
--rw-r--r--   0        0        0     3086 2023-06-03 17:41:15.902941 klu-0.1.7/klu/common/client.py
--rw-r--r--   0        0        0     2975 2023-06-03 17:41:15.902941 klu-0.1.7/klu/common/errors.py
--rw-r--r--   0        0        0     2209 2023-06-03 17:41:15.902941 klu-0.1.7/klu/common/models.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/__init__.py
--rw-r--r--   0        0        0     2291 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/client.py
--rw-r--r--   0        0        0       25 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/constants.py
--rw-r--r--   0        0        0      274 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/errors.py
--rw-r--r--   0        0        0     3199 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data/models.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/__init__.py
--rw-r--r--   0        0        0     8672 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/client.py
--rw-r--r--   0        0        0      287 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/constants.py
--rw-r--r--   0        0        0      309 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/errors.py
--rw-r--r--   0        0        0     3415 2023-06-03 17:41:15.902941 klu-0.1.7/klu/data_index/models.py
--rw-r--r--   0        0        0       19 2023-06-03 17:41:15.902941 klu-0.1.7/klu/klu.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/__init__.py
--rw-r--r--   0        0        0     3505 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/client.py
--rw-r--r--   0        0        0       28 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/constants.py
--rw-r--r--   0        0        0      447 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/errors.py
--rw-r--r--   0        0        0     1397 2023-06-03 17:41:15.902941 klu-0.1.7/klu/model/models.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/session/__init__.py
--rw-r--r--   0        0        0     1488 2023-06-03 17:41:15.902941 klu-0.1.7/klu/session/client.py
--rw-r--r--   0        0        0       32 2023-06-03 17:41:15.902941 klu-0.1.7/klu/session/constants.py
--rw-r--r--   0        0        0     1264 2023-06-03 17:41:15.902941 klu-0.1.7/klu/session/models.py
--rw-r--r--   0        0        0      111 2023-06-03 17:41:15.902941 klu-0.1.7/klu/utils/dict_helpers.py
--rw-r--r--   0        0        0      752 2023-06-03 17:41:15.902941 klu-0.1.7/klu/utils/file_upload.py
--rw-r--r--   0        0        0     2407 2023-06-03 17:41:15.902941 klu-0.1.7/klu/utils/paginator.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/__init__.py
--rw-r--r--   0        0        0     8052 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/client.py
--rw-r--r--   0        0        0      321 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/constants.py
--rw-r--r--   0        0        0      244 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/errors.py
--rw-r--r--   0        0        0      943 2023-06-03 17:41:15.902941 klu-0.1.7/klu/workspace/models.py
--rw-r--r--   0        0        0     1952 2023-06-03 17:41:15.906941 klu-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3698 1970-01-01 00:00:00.000000 klu-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-08 22:55:36.156770 klu-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2840 2023-07-08 22:55:36.156770 klu-0.1.8/README.md
+-rw-r--r--   0        0        0      150 2023-07-08 22:55:36.156770 klu-0.1.8/klu/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.156770 klu-0.1.8/klu/action/__init__.py
+-rw-r--r--   0        0        0    11398 2023-07-08 22:55:36.156770 klu-0.1.8/klu/action/client.py
+-rw-r--r--   0        0        0      280 2023-07-08 22:55:36.156770 klu-0.1.8/klu/action/constants.py
+-rw-r--r--   0        0        0      537 2023-07-08 22:55:36.156770 klu-0.1.8/klu/action/errors.py
+-rw-r--r--   0        0        0     1936 2023-07-08 22:55:36.160770 klu-0.1.8/klu/action/models.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/__init__.py
+-rw-r--r--   0        0        0     2998 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/client.py
+-rw-r--r--   0        0        0      199 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/config.py
+-rw-r--r--   0        0        0      118 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/constants.py
+-rw-r--r--   0        0        0     1406 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/sse_client.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/__init__.py
+-rw-r--r--   0        0        0     7753 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/client.py
+-rw-r--r--   0        0        0      259 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/constants.py
+-rw-r--r--   0        0        0      318 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/errors.py
+-rw-r--r--   0        0        0     1421 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/models.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/client/__init__.py
+-rw-r--r--   0        0        0      898 2023-07-08 22:55:36.160770 klu-0.1.8/klu/client/klu.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/common/__init__.py
+-rw-r--r--   0        0        0     3086 2023-07-08 22:55:36.160770 klu-0.1.8/klu/common/client.py
+-rw-r--r--   0        0        0     2975 2023-07-08 22:55:36.160770 klu-0.1.8/klu/common/errors.py
+-rw-r--r--   0        0        0     2403 2023-07-08 22:55:36.160770 klu-0.1.8/klu/common/models.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/__init__.py
+-rw-r--r--   0        0        0     2534 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/client.py
+-rw-r--r--   0        0        0       25 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/constants.py
+-rw-r--r--   0        0        0      274 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/errors.py
+-rw-r--r--   0        0        0     3381 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/models.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/__init__.py
+-rw-r--r--   0        0        0     8671 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/client.py
+-rw-r--r--   0        0        0      287 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/constants.py
+-rw-r--r--   0        0        0      309 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/errors.py
+-rw-r--r--   0        0        0     3405 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/models.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/__init__.py
+-rw-r--r--   0        0        0     6137 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/client.py
+-rw-r--r--   0        0        0      104 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/constants.py
+-rw-r--r--   0        0        0      573 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/errors.py
+-rw-r--r--   0        0        0     1083 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/models.py
+-rw-r--r--   0        0        0       19 2023-07-08 22:55:36.160770 klu-0.1.8/klu/klu.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/__init__.py
+-rw-r--r--   0        0        0     3505 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/client.py
+-rw-r--r--   0        0        0       28 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/constants.py
+-rw-r--r--   0        0        0      447 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/errors.py
+-rw-r--r--   0        0        0     1387 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/models.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/session/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-08 22:55:36.160770 klu-0.1.8/klu/session/client.py
+-rw-r--r--   0        0        0       32 2023-07-08 22:55:36.160770 klu-0.1.8/klu/session/constants.py
+-rw-r--r--   0        0        0     1255 2023-07-08 22:55:36.160770 klu-0.1.8/klu/session/models.py
+-rw-r--r--   0        0        0      111 2023-07-08 22:55:36.160770 klu-0.1.8/klu/utils/dict_helpers.py
+-rw-r--r--   0        0        0      752 2023-07-08 22:55:36.160770 klu-0.1.8/klu/utils/file_upload.py
+-rw-r--r--   0        0        0     2407 2023-07-08 22:55:36.160770 klu-0.1.8/klu/utils/paginator.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/__init__.py
+-rw-r--r--   0        0        0     8052 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/client.py
+-rw-r--r--   0        0        0      321 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/constants.py
+-rw-r--r--   0        0        0      244 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/errors.py
+-rw-r--r--   0        0        0      943 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/models.py
+-rw-r--r--   0        0        0     1952 2023-07-08 22:55:36.160770 klu-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3698 1970-01-01 00:00:00.000000 klu-0.1.8/PKG-INFO
```

### Comparing `klu-0.1.7/LICENSE` & `klu-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/README.md` & `klu-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/action/client.py` & `klu-0.1.8/klu/action/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from klu.action.models import Action, PromptResponse
 from klu.common.client import KluClientBase
 from klu.common.errors import (
     InvalidUpdateParamsError,
     UnknownKluAPIError,
     UnknownKluError,
 )
+from klu.common.models import PromptInput
 from klu.data.models import Data
 from klu.utils.dict_helpers import dict_no_empty
 from klu.utils.paginator import Paginator
 from klu.workspace.errors import WorkspaceOrUserNotFoundError
 
 
 class ActionsClient(KluClientBase):
@@ -130,26 +131,26 @@
             Deleted Action object.
         """
         return await super().delete(guid)
 
     async def run_action_prompt(
         self,
         action_guid: str,
-        prompt: str,
+        input: PromptInput,
         filter: Optional[str] = None,
         streaming: Optional[bool] = False,
         async_mode: Optional[bool] = False,
         session_guid: Optional[str] = None,
     ) -> PromptResponse:
         """
         Run a prompt with an agent, optionally using streaming.
 
         Args:
             action_guid (str): The GUID of the agent to run the prompt with.
-            prompt (str): The prompt to run with the agent.
+            input (PromptInput): The prompt to run with the agent.
             filter (Optional[str]): The filter to use when running the prompt.
             session_guid (Optional[str]): The GUID of the session to run the prompt with.
             streaming (Optional[bool]): Flag that defines whether to use streaming or not.
             async_mode (Optional[bool]): Boolean that identifies whether the async mode should be used. Defaults to False.
 
         Returns:
             An object result of running the prompt with the message and a feedback_url for providing feedback.
@@ -157,15 +158,15 @@
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
 
             try:
                 response = await client.post(
                     ACTION_ENDPOINT,
                     {
-                        "prompt": prompt,
+                        "input": input,
                         "filter": filter,
                         "action": action_guid,
                         "streaming": streaming,
                         "async_mode": async_mode,
                         "sessionGuid": session_guid,
                     },
                 )
@@ -212,23 +213,23 @@
                         "prompt": prompt,
                         "toolIds": tool_ids,
                         "modelId": model_id,
                         "indexIds": index_ids,
                         "modelConfig": model_config,
                     },
                 )
-                return PromptResponse(**response)
+                return PromptResponse._create_instance(**response)
             except ClientResponseError as e:
                 if e.status == 404:
                     raise WorkspaceOrUserNotFoundError()
                 if e.status == 400:
                     raise InvalidActionPromptData(e.message)
 
                 raise UnknownKluAPIError(e.status, e.message)
-            except Exception:
+            except Exception as e:
                 raise UnknownKluError()
 
     async def get_action_data(self, guid: str) -> List[Data]:
         """
         Retrieves data information for an action.
 
         Args:
```

### Comparing `klu-0.1.7/klu/action/errors.py` & `klu-0.1.8/klu/action/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 class ActionNotFoundError(Exception):
-    application_id: str
+    action_id: str
 
     def __init__(self, action_id: str):
-        self.application_id = action_id
+        self.action_id = action_id
         self.message = f"Action with id {action_id} was not found."
         super().__init__(self.message)
 
 
 class InvalidActionPromptData(Exception):
     def __init__(self, response_message: str):
         self.message = (
```

### Comparing `klu-0.1.7/klu/action/models.py` & `klu-0.1.8/klu/application/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,52 @@
 """
-This module provides data models for the Action.
+This module provides data models for the Application.
 """
 from dataclasses import asdict, dataclass
 from datetime import datetime
 from typing import Optional
 
-from klu.common.models import BaseDataClass, BaseEngineModel
+from klu.common.models import BaseEngineModel
 
 
 @dataclass
-class Action(BaseEngineModel):
+class Application(BaseEngineModel):
     """
-    This class represents the Action data model returned from the Klu engine
+    This class represents the Application data model returned from the Klu engine
     """
 
+    id: int
     guid: str
     name: str
-    prompt: str
-    app_id: int
-    model_id: int
-    action_type: str
+    app_type: str
+    enabled: bool
+
+    workspace_id: int
+    created_by_id: str
+
     description: Optional[str]
-    model_config: Optional[dict]
-    experiment_id: Optional[int] = None
-    updated_at: Optional[datetime] = None
-    created_at: Optional[datetime] = None
+    deleted: Optional[bool] = None
+    updated_at: Optional[str] = None
+    created_at: Optional[str] = None
 
     @classmethod
-    def _from_engine_format(cls, data: dict) -> "Action":
+    def _from_engine_format(cls, data: dict) -> "Application":
         return cls._create_instance(
             **{
-                "app_id": data.pop("appId", None),
-                "model_id": data.pop("modelId", None),
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
-                "action_type": data.pop("agent_type", None),
-                "experiment_id": data.pop("experimentId", None),
+                "workspace_id": data.pop("workspaceId", None),
+                "created_by_id": data.pop("createdById", None),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
         base_dict = asdict(self)
 
         return {
-            "appId": base_dict.pop("app_id", None),
-            "modelId": base_dict.pop("model_id", None),
             "updatedAt": base_dict.pop("updated_at", None),
             "createdAt": base_dict.pop("created_at", None),
-            "agent_type": base_dict.pop("action_type", None),
-            "experimentId": base_dict.pop("experiment_id", None),
+            "workspaceId": base_dict.pop("workspace_id", None),
+            "createdById": base_dict.pop("created_by_id", None),
             **base_dict,
         }
-
-
-@dataclass
-class PromptResponse(BaseDataClass):
-    """
-    This class represents the Response data model returned from the Klu engine in response to action prompting.
-    """
-
-    msg: str
-    streaming: bool
-    result_url: Optional[str] = None
-    feedback_url: Optional[str] = None
-    streaming_url: Optional[str] = None
```

### Comparing `klu-0.1.7/klu/api/client.py` & `klu-0.1.8/klu/api/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/api/sse_client.py` & `klu-0.1.8/klu/api/sse_client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/application/client.py` & `klu-0.1.8/klu/application/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/application/models.py` & `klu-0.1.8/klu/model/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 """
-This module provides data models for the Application.
+This module provides data models for the Model.
 """
+
 from dataclasses import asdict, dataclass
 from datetime import datetime
 from typing import Optional
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
-class Application(BaseEngineModel):
+class Model(BaseEngineModel):
     """
-    This class represents the Application data model returned from the Klu engine
+    This class represents the Model data returned from the Klu engine
     """
 
     id: int
+    llm: str
     guid: str
-    name: str
-    app_type: str
-    enabled: bool
-
-    workspace_id: int
+    model_name: str
     created_by_id: str
-
-    description: Optional[str]
-    model_config: Optional[dict]
-    deleted: Optional[bool] = None
-    updated_at: Optional[datetime] = None
-    created_at: Optional[datetime] = None
+    workspace_model_provider_id: int
+    updated_at: Optional[str] = None
+    created_at: Optional[str] = None
 
     @classmethod
-    def _from_engine_format(cls, data: dict) -> "Application":
+    def _from_engine_format(cls, data: dict) -> "Model":
         return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
-                "workspace_id": data.pop("workspaceId", None),
                 "created_by_id": data.pop("createdById", None),
+                "workspace_model_provider_id": data.pop(
+                    "workspaceModelProviderId", None
+                ),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self)
+        base_dict = asdict(
+            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
+        )
+
+        base_dict.pop("updated_at", None)
+        base_dict.pop("created_at", None)
+        base_dict.pop("created_by_id", None)
+        base_dict.pop("workspace_model_provider_id", None)
 
-        return {
-            "updatedAt": base_dict.pop("updated_at", None),
-            "createdAt": base_dict.pop("created_at", None),
-            "workspaceId": base_dict.pop("workspace_id", None),
-            "createdById": base_dict.pop("created_by_id", None),
-            **base_dict,
-        }
+        return base_dict
```

### Comparing `klu-0.1.7/klu/client/klu.py` & `klu-0.1.8/klu/client/klu.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from klu.action.client import ActionsClient
 from klu.api.sse_client import SSEClient
 from klu.application.client import ApplicationsClient
 from klu.data.client import DataClient
 from klu.data_index.client import DataIndexClient
+from klu.experiment.client import ExperimentClient
 from klu.model.client import ModelsClient
 from klu.session.client import SessionClient
 from klu.workspace.client import WorkspaceClient
 
 
 class KluClient:
     def __init__(self, api_key: str):
@@ -14,8 +15,9 @@
 
         self.data = DataClient(api_key)
         self.models = ModelsClient(api_key)
         self.actions = ActionsClient(api_key)
         self.sessions = SessionClient(api_key)
         self.workspace = WorkspaceClient(api_key)
         self.data_index = DataIndexClient(api_key)
+        self.experiments = ExperimentClient(api_key)
         self.applications = ApplicationsClient(api_key)
```

### Comparing `klu-0.1.7/klu/common/client.py` & `klu-0.1.8/klu/common/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/common/errors.py` & `klu-0.1.8/klu/common/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/common/models.py` & `klu-0.1.8/klu/common/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABCMeta, abstractmethod
 from enum import Enum
-from typing import Optional
+from typing import Any, Dict, Optional, Union
 
 
 class BasicEnum(Enum):
     """
     Basic class for enums across the projects. Adds basic functions to list names and values.
     Overrides comparison function to allow comparing against string values.
     """
@@ -74,7 +74,14 @@
     @abstractmethod
     def _from_engine_format(cls, data: dict) -> "BaseEngineModel":
         pass
 
     @abstractmethod
     def _to_engine_format(self) -> dict:
         pass
+
+
+"""
+This type defines input that can be sent to a prompt.
+It can either be a string or a Dict with properties you defined in Klu
+"""
+PromptInput = Union[str, Dict[str, Any]]
```

### Comparing `klu-0.1.7/klu/data/client.py` & `klu-0.1.8/klu/data/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # mypy: disable-error-code="override"
 from typing import Optional
 
 from klu.common.client import KluClientBase
 from klu.data.constants import DATA_ENDPOINT
-from klu.data.models import Data
+from klu.data.models import Data, DataSourceType
 
 
 class DataClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, DATA_ENDPOINT, Data)
 
     async def create(
         self,
         input: str,
         output: str,
         rating: int,
         action_guid: str,
+        full_prompt_sent: Optional[str] = None,
         issue: Optional[str] = None,
         correction: Optional[str] = None,
         meta_data: Optional[dict] = None,
         session_guid: Optional[str] = None,
     ) -> Data:
         """
         Creates new data instance for an action_id provided.
@@ -33,23 +34,28 @@
             session_guid (str): Guid of a session data belongs to
             meta_data (dict): Data meta_data
             correction (str): Data correction
 
         Returns:
             Created Data object
         """
+        meta_data = meta_data or {}
         return await super().create(
             issue=issue,
             input=input,
             output=output,
             rating=rating,
-            meta_data=meta_data,
+            action=action_guid,
+            session=session_guid,
             correction=correction,
-            action_guid=action_guid,
-            session_guid=session_guid,
+            full_prompt_sent=full_prompt_sent,
+            meta_data={
+                **meta_data,
+                "source": meta_data.pop("source", DataSourceType.SDK),
+            },
         )
 
     async def get(self, guid: str) -> Data:
         """
         Retrieves data information based on the data ID.
 
         Args:
```

### Comparing `klu-0.1.7/klu/data/models.py` & `klu-0.1.8/klu/data/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 This module provides data models for the Data.
 """
 
 from abc import ABC
 from dataclasses import asdict, dataclass
-from datetime import datetime
 from typing import Optional
 
-from klu.common.models import BaseEngineModel
+from klu.common.models import BaseEngineModel, BasicStringEnum
 
 
 @dataclass
 class DataWithId(BaseEngineModel, ABC):
     """
     This class represents the base data with Id after it has been persisted into the Klu Database
     """
@@ -38,16 +37,17 @@
     issue: Optional[int] = None
     input: Optional[str] = None
     action: Optional[int] = None
     output: Optional[str] = None
     rating: Optional[int] = None
     metadata: Optional[dict] = None
     correction: Optional[str] = None
-    updated_at: Optional[datetime] = None
-    created_at: Optional[datetime] = None
+    updated_at: Optional[str] = None
+    created_at: Optional[str] = None
+    full_prompt_sent: Optional[dict] = None
 
     @classmethod
     def _from_engine_format(cls, data: dict) -> "DataBaseClass":
         return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
@@ -115,7 +115,15 @@
             self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
         )
 
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
 
         return base_dict
+
+
+class DataSourceType(BasicStringEnum):
+    """The enum used to represent the source of the Data"""
+
+    SDK = "SDK"
+    API = "API"
+    BACK_FILL = "backfill"
```

### Comparing `klu-0.1.7/klu/data_index/client.py` & `klu-0.1.8/klu/data_index/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         file_url = await self.upload_index_file(file_data) if file_data else None
         data_index = {
             "name": name,
             "splitter": splitter,
             "description": description,
         }
         if file_url:
-            data_index["file_url"] = file_url
+            data_index["fileUrl"] = file_url
 
         return await super().create(**data_index)
 
     # type: ignore
     async def get(self, guid: str) -> DataIndex:
         """
         Retrieves data_index information based on the id.
```

### Comparing `klu-0.1.7/klu/data_index/models.py` & `klu-0.1.8/klu/data_index/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     file_url: str
     index_url: str
     loader_id: int
     workspace_id: int
     created_by_id: str
 
     description: Optional[str]
-    updated_at: Optional[datetime] = None
-    created_at: Optional[datetime] = None
+    updated_at: Optional[str] = None
+    created_at: Optional[str] = None
 
     @classmethod
     def _from_engine_format(cls, data: dict) -> "DataIndex":
         return cls._create_instance(
             **{
                 "type_id": data.pop("typeId", None),
                 "task_id": data.pop("taskId", None),
```

### Comparing `klu-0.1.7/klu/model/client.py` & `klu-0.1.8/klu/model/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/model/models.py` & `klu-0.1.8/klu/experiment/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 """
-This module provides data models for the Model.
+This module provides data models for the Experiment.
 """
 
 from dataclasses import asdict, dataclass
-from datetime import datetime
 from typing import Optional
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
-class Model(BaseEngineModel):
+class Experiment(BaseEngineModel):
     """
-    This class represents the Model data returned from the Klu engine
+    This class represents the Experiment data returned from the Klu engine
     """
 
-    id: int
-    llm: str
     guid: str
-    model_name: str
-    created_by_id: str
-    workspace_model_provider_id: int
-    updated_at: Optional[datetime] = None
-    created_at: Optional[datetime] = None
+    name: str
+    status: str
+    app_guid: str
+    action_primary_guid: str
+    action_secondary_guid: str
+    created_at: Optional[str] = None
+    updated_at: Optional[str] = None
 
     @classmethod
-    def _from_engine_format(cls, data: dict) -> "Model":
+    def _from_engine_format(cls, data: dict) -> "Experiment":
         return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
-                "created_by_id": data.pop("createdById", None),
-                "workspace_model_provider_id": data.pop(
-                    "workspaceModelProviderId", None
-                ),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
         base_dict = asdict(
             self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
         )
 
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
-        base_dict.pop("created_by_id", None)
-        base_dict.pop("workspace_model_provider_id", None)
 
         return base_dict
```

### Comparing `klu-0.1.7/klu/session/client.py` & `klu-0.1.8/klu/session/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
         Args:
             action_guid (str): Guid of the action object this session is attached to.
 
         Returns:
             A newly created Session object.
         """
-        return await super().create(action_guid=action_guid)
+        return await super().create(action=action_guid)
 
     async def get(self, guid: str) -> Session:
         """
         Retrieves session information based on the unique Session guid, created during the Session creation.
 
         Args:
             guid (str): GUID of a session to fetch. The one that was used during the session creation
```

### Comparing `klu-0.1.7/klu/session/models.py` & `klu-0.1.8/klu/session/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 This module provides data models for the Session.
 """
 
 from dataclasses import asdict, dataclass
-from datetime import datetime
 from typing import Optional
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
 class Session(BaseEngineModel):
@@ -15,16 +14,17 @@
     This class represents the Session data returned from the Klu engine
     """
 
     id: int
     guid: str
     action_id: int
     created_by_id: str
-    created_at: Optional[datetime] = None
-    updated_at: Optional[datetime] = None
+    name: Optional[str] = None
+    created_at: Optional[str] = None
+    updated_at: Optional[str] = None
 
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Session":
         return cls._create_instance(
             **{
                 "action_id": data.pop("actionId", None),
                 "updated_at": data.pop("updatedAt", None),
```

### Comparing `klu-0.1.7/klu/utils/file_upload.py` & `klu-0.1.8/klu/utils/file_upload.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/utils/paginator.py` & `klu-0.1.8/klu/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/workspace/client.py` & `klu-0.1.8/klu/workspace/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/klu/workspace/models.py` & `klu-0.1.8/klu/workspace/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.7/pyproject.toml` & `klu-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "klu"
-version = "0.1.7"
+version = "0.1.8"
 homepage = "https://github.com/ssabev/klu"
 description = "SDK for building AI Enabled apps."
 authors = ["Stefan Sabev <stefan@klu.ai>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `klu-0.1.7/PKG-INFO` & `klu-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klu
-Version: 0.1.7
+Version: 0.1.8
 Summary: SDK for building AI Enabled apps.
 Home-page: https://github.com/ssabev/klu
 License: MIT
 Author: Stefan Sabev
 Author-email: stefan@klu.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

