# Comparing `tmp/stigg_api_client_v2-0.475.5.tar.gz` & `tmp/stigg_api_client_v2-0.476.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.475.5.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.476.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.475.5.tar` & `stigg_api_client_v2-0.476.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1644 2023-07-06 13:22:57.896727 stigg_api_client_v2-0.475.5/README.md
--rw-r--r--   0        0        0      432 2023-07-06 13:24:04.741698 stigg_api_client_v2-0.475.5/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-06 13:22:57.900727 stigg_api_client_v2-0.475.5/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-06 13:22:57.900727 stigg_api_client_v2-0.475.5/stigg/client.py
--rw-r--r--   0        0        0    39793 2023-07-06 13:24:02.453669 stigg_api_client_v2-0.475.5/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-07-06 13:24:01.957663 stigg_api_client_v2-0.475.5/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    66833 2023-07-06 13:24:02.241666 stigg_api_client_v2-0.475.5/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-06 13:23:55.133563 stigg_api_client_v2-0.475.5/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-06 13:24:01.957663 stigg_api_client_v2-0.475.5/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-06 13:24:00.693646 stigg_api_client_v2-0.475.5/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-06 13:24:00.713647 stigg_api_client_v2-0.475.5/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    66418 2023-07-06 13:23:55.421567 stigg_api_client_v2-0.475.5/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-06 13:24:00.749647 stigg_api_client_v2-0.475.5/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    23994 2023-07-06 13:23:57.441597 stigg_api_client_v2-0.475.5/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-06 13:24:00.697646 stigg_api_client_v2-0.475.5/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-06 13:24:00.709647 stigg_api_client_v2-0.475.5/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-06 13:24:01.957663 stigg_api_client_v2-0.475.5/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    54916 2023-07-06 13:24:01.953662 stigg_api_client_v2-0.475.5/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-06 13:24:00.777648 stigg_api_client_v2-0.475.5/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-06 13:24:00.785648 stigg_api_client_v2-0.475.5/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-06 13:24:00.765647 stigg_api_client_v2-0.475.5/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-06 13:24:00.837648 stigg_api_client_v2-0.475.5/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-06 13:24:00.805648 stigg_api_client_v2-0.475.5/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-06 13:24:00.801648 stigg_api_client_v2-0.475.5/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-06 13:24:00.849649 stigg_api_client_v2-0.475.5/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-06 13:24:00.793648 stigg_api_client_v2-0.475.5/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-06 13:24:00.821648 stigg_api_client_v2-0.475.5/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-06 13:24:00.833648 stigg_api_client_v2-0.475.5/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-06 13:24:00.649646 stigg_api_client_v2-0.475.5/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-06 13:24:00.641646 stigg_api_client_v2-0.475.5/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-06 13:24:00.673646 stigg_api_client_v2-0.475.5/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126250 2023-07-06 13:24:00.617645 stigg_api_client_v2-0.475.5/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-06 13:24:00.757647 stigg_api_client_v2-0.475.5/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-06 13:24:00.633645 stigg_api_client_v2-0.475.5/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-06 13:24:00.669646 stigg_api_client_v2-0.475.5/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-06 13:24:00.741647 stigg_api_client_v2-0.475.5/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-06 13:24:00.733647 stigg_api_client_v2-0.475.5/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-06 13:24:00.725647 stigg_api_client_v2-0.475.5/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-06 13:24:01.961663 stigg_api_client_v2-0.475.5/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-06 13:24:00.653646 stigg_api_client_v2-0.475.5/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-06 13:24:00.685646 stigg_api_client_v2-0.475.5/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-06 13:24:00.861649 stigg_api_client_v2-0.475.5/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.475.5/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-09 10:54:26.508297 stigg_api_client_v2-0.476.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-09 10:55:13.729239 stigg_api_client_v2-0.476.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-09 10:54:26.508297 stigg_api_client_v2-0.476.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-09 10:54:26.508297 stigg_api_client_v2-0.476.0/stigg/client.py
+-rw-r--r--   0        0        0    39793 2023-07-09 10:55:11.757200 stigg_api_client_v2-0.476.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-07-09 10:55:11.369193 stigg_api_client_v2-0.476.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    66833 2023-07-09 10:55:11.593197 stigg_api_client_v2-0.476.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-09 10:55:05.605080 stigg_api_client_v2-0.476.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-09 10:55:11.369193 stigg_api_client_v2-0.476.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-09 10:55:10.189169 stigg_api_client_v2-0.476.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-09 10:55:10.205170 stigg_api_client_v2-0.476.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    66418 2023-07-09 10:55:05.821084 stigg_api_client_v2-0.476.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-09 10:55:10.229170 stigg_api_client_v2-0.476.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    23970 2023-07-09 10:55:07.481116 stigg_api_client_v2-0.476.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-09 10:55:10.193169 stigg_api_client_v2-0.476.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-09 10:55:10.201170 stigg_api_client_v2-0.476.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-09 10:55:11.369193 stigg_api_client_v2-0.476.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    54916 2023-07-09 10:55:11.365193 stigg_api_client_v2-0.476.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-09 10:55:10.253171 stigg_api_client_v2-0.476.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-09 10:55:10.261171 stigg_api_client_v2-0.476.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-09 10:55:10.245170 stigg_api_client_v2-0.476.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-09 10:55:10.301172 stigg_api_client_v2-0.476.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-09 10:55:10.277171 stigg_api_client_v2-0.476.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-09 10:55:10.273171 stigg_api_client_v2-0.476.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-09 10:55:10.309172 stigg_api_client_v2-0.476.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-09 10:55:10.265171 stigg_api_client_v2-0.476.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-09 10:55:10.285171 stigg_api_client_v2-0.476.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-09 10:55:10.293172 stigg_api_client_v2-0.476.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-09 10:55:10.153169 stigg_api_client_v2-0.476.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-09 10:55:10.149169 stigg_api_client_v2-0.476.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-09 10:55:10.173169 stigg_api_client_v2-0.476.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126250 2023-07-09 10:55:10.129168 stigg_api_client_v2-0.476.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-09 10:55:10.237170 stigg_api_client_v2-0.476.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-09 10:55:10.141168 stigg_api_client_v2-0.476.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-09 10:55:10.169169 stigg_api_client_v2-0.476.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-09 10:55:10.225170 stigg_api_client_v2-0.476.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-09 10:55:10.221170 stigg_api_client_v2-0.476.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-09 10:55:10.213170 stigg_api_client_v2-0.476.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-09 10:55:11.373193 stigg_api_client_v2-0.476.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-09 10:55:10.161169 stigg_api_client_v2-0.476.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-09 10:55:10.181169 stigg_api_client_v2-0.476.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-09 10:55:10.317172 stigg_api_client_v2-0.476.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.476.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.475.5/README.md` & `stigg_api_client_v2-0.476.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.475.5/stigg/client.py` & `stigg_api_client_v2-0.476.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/__init__.py` & `stigg_api_client_v2-0.476.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.476.0/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/async_client.py` & `stigg_api_client_v2-0.476.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/base_client.py` & `stigg_api_client_v2-0.476.0/stigg/generated/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:23
+# Generated by ariadne-codegen on 2023-07-09 10:55
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/base_model.py` & `stigg_api_client_v2-0.476.0/stigg/generated/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.476.0/stigg/generated/cancel_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/client.py` & `stigg_api_client_v2-0.476.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:23
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.476.0/stigg/generated/create_subscription.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/enums.py` & `stigg_api_client_v2-0.476.0/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:23
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
@@ -376,17 +376,15 @@
     InvalidSubscriptionStatus = "InvalidSubscriptionStatus"
     InvalidUpdatePriceUnitAmountError = "InvalidUpdatePriceUnitAmountError"
     MemberInvitationError = "MemberInvitationError"
     MemberNotFound = "MemberNotFound"
     MeterDoesNotBelongToTheEntitlementFeature = (
         "MeterDoesNotBelongToTheEntitlementFeature"
     )
-    MeterMustBeAssociatedToIncrementalFeature = (
-        "MeterMustBeAssociatedToIncrementalFeature"
-    )
+    MeterMustBeAssociatedToMeteredFeature = "MeterMustBeAssociatedToMeteredFeature"
     MeteringNotAvailableForFeatureType = "MeteringNotAvailableForFeatureType"
     MissingEntityIdError = "MissingEntityIdError"
     NoFeatureEntitlementInSubscription = "NoFeatureEntitlementInSubscription"
     NoProductsAvailable = "NoProductsAvailable"
     OperationNotAllowedDuringInProgressExperiment = (
         "OperationNotAllowedDuringInProgressExperiment"
     )
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.476.0/stigg/generated/estimate_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.476.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.476.0/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/fragments.py` & `stigg_api_client_v2-0.476.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -328,32 +328,25 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalSubscriptionPriceFragment(BaseModel):
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    billing_model: Optional[BillingModel] = Field(alias="billingModel")
-    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
-    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
-
-
-class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
-    amount: float
-    currency: Currency
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
 
 
-class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
+class CustomerPortalPromotionalEntitlement(BaseModel):
     display_name: str = Field(alias="displayName")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -406,14 +399,34 @@
 class CustomerPortalSubscriptionAddon(BaseModel):
     addon_id: str = Field(alias="addonId")
     description: Optional[str]
     display_name: str = Field(alias="displayName")
     quantity: int
 
 
+class CustomerPortalSubscriptionPriceFragment(BaseModel):
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    billing_model: Optional[BillingModel] = Field(alias="billingModel")
+    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
+    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
+
+
+class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+
+
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
@@ -491,27 +504,14 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -842,14 +842,34 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -864,34 +884,14 @@
 
 class MockPaywallPriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1346,37 +1346,37 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalSubscriptionPriceFragment.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
+CustomerPortalSubscriptionPriceFragment.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
@@ -1418,19 +1418,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.476.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.476.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.476.0/stigg/generated/get_customer_by_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.476.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.476.0/stigg/generated/get_mock_paywall.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/get_products.py` & `stigg_api_client_v2-0.476.0/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.476.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/input_types.py` & `stigg_api_client_v2-0.476.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.476.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.476.0/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.476.0/stigg/generated/provision_subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.476.0/stigg/generated/report_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.475.5/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.476.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-06 13:24
+# Generated by ariadne-codegen on 2023-07-09 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.475.5/PKG-INFO` & `stigg_api_client_v2-0.476.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.475.5
+Version: 0.476.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

