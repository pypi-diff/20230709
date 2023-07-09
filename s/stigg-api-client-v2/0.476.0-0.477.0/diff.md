# Comparing `tmp/stigg_api_client_v2-0.476.0.tar.gz` & `tmp/stigg_api_client_v2-0.477.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.476.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.477.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.476.0.tar` & `stigg_api_client_v2-0.477.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1644 2023-07-09 10:54:26.508297 stigg_api_client_v2-0.476.0/README.md
--rw-r--r--   0        0        0      432 2023-07-09 10:55:13.729239 stigg_api_client_v2-0.476.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-09 10:54:26.508297 stigg_api_client_v2-0.476.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-09 10:54:26.508297 stigg_api_client_v2-0.476.0/stigg/client.py
--rw-r--r--   0        0        0    39793 2023-07-09 10:55:11.757200 stigg_api_client_v2-0.476.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-07-09 10:55:11.369193 stigg_api_client_v2-0.476.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    66833 2023-07-09 10:55:11.593197 stigg_api_client_v2-0.476.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-09 10:55:05.605080 stigg_api_client_v2-0.476.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-09 10:55:11.369193 stigg_api_client_v2-0.476.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-09 10:55:10.189169 stigg_api_client_v2-0.476.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-09 10:55:10.205170 stigg_api_client_v2-0.476.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    66418 2023-07-09 10:55:05.821084 stigg_api_client_v2-0.476.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-09 10:55:10.229170 stigg_api_client_v2-0.476.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    23970 2023-07-09 10:55:07.481116 stigg_api_client_v2-0.476.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-09 10:55:10.193169 stigg_api_client_v2-0.476.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-09 10:55:10.201170 stigg_api_client_v2-0.476.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-09 10:55:11.369193 stigg_api_client_v2-0.476.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    54916 2023-07-09 10:55:11.365193 stigg_api_client_v2-0.476.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-09 10:55:10.253171 stigg_api_client_v2-0.476.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-09 10:55:10.261171 stigg_api_client_v2-0.476.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-09 10:55:10.245170 stigg_api_client_v2-0.476.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-09 10:55:10.301172 stigg_api_client_v2-0.476.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-09 10:55:10.277171 stigg_api_client_v2-0.476.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-09 10:55:10.273171 stigg_api_client_v2-0.476.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-09 10:55:10.309172 stigg_api_client_v2-0.476.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-09 10:55:10.265171 stigg_api_client_v2-0.476.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-09 10:55:10.285171 stigg_api_client_v2-0.476.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-09 10:55:10.293172 stigg_api_client_v2-0.476.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-09 10:55:10.153169 stigg_api_client_v2-0.476.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-09 10:55:10.149169 stigg_api_client_v2-0.476.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-09 10:55:10.173169 stigg_api_client_v2-0.476.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126250 2023-07-09 10:55:10.129168 stigg_api_client_v2-0.476.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-09 10:55:10.237170 stigg_api_client_v2-0.476.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-09 10:55:10.141168 stigg_api_client_v2-0.476.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-09 10:55:10.169169 stigg_api_client_v2-0.476.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-09 10:55:10.225170 stigg_api_client_v2-0.476.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-09 10:55:10.221170 stigg_api_client_v2-0.476.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-09 10:55:10.213170 stigg_api_client_v2-0.476.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-09 10:55:11.373193 stigg_api_client_v2-0.476.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-09 10:55:10.161169 stigg_api_client_v2-0.476.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-09 10:55:10.181169 stigg_api_client_v2-0.476.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-09 10:55:10.317172 stigg_api_client_v2-0.476.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.476.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-09 16:10:36.165369 stigg_api_client_v2-0.477.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-09 16:11:26.844503 stigg_api_client_v2-0.477.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-09 16:10:36.165369 stigg_api_client_v2-0.477.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-09 16:10:36.165369 stigg_api_client_v2-0.477.0/stigg/client.py
+-rw-r--r--   0        0        0    39793 2023-07-09 16:11:24.848450 stigg_api_client_v2-0.477.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-07-09 16:11:24.408421 stigg_api_client_v2-0.477.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    66833 2023-07-09 16:11:24.660437 stigg_api_client_v2-0.477.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-09 16:11:18.696077 stigg_api_client_v2-0.477.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-09 16:11:24.408421 stigg_api_client_v2-0.477.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-09 16:11:23.368352 stigg_api_client_v2-0.477.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-09 16:11:23.388353 stigg_api_client_v2-0.477.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    66418 2023-07-09 16:11:18.940091 stigg_api_client_v2-0.477.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-09 16:11:23.416355 stigg_api_client_v2-0.477.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24176 2023-07-09 16:11:20.704194 stigg_api_client_v2-0.477.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-09 16:11:23.372352 stigg_api_client_v2-0.477.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-09 16:11:23.380353 stigg_api_client_v2-0.477.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-09 16:11:24.412421 stigg_api_client_v2-0.477.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    54916 2023-07-09 16:11:24.408421 stigg_api_client_v2-0.477.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-09 16:11:23.440357 stigg_api_client_v2-0.477.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-09 16:11:23.448357 stigg_api_client_v2-0.477.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-09 16:11:23.432356 stigg_api_client_v2-0.477.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-09 16:11:23.492360 stigg_api_client_v2-0.477.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-09 16:11:23.468359 stigg_api_client_v2-0.477.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-09 16:11:23.460358 stigg_api_client_v2-0.477.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-09 16:11:23.504361 stigg_api_client_v2-0.477.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-09 16:11:23.456358 stigg_api_client_v2-0.477.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-09 16:11:23.476359 stigg_api_client_v2-0.477.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-09 16:11:23.488360 stigg_api_client_v2-0.477.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-09 16:11:23.328349 stigg_api_client_v2-0.477.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-09 16:11:23.320349 stigg_api_client_v2-0.477.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-09 16:11:23.352351 stigg_api_client_v2-0.477.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126250 2023-07-09 16:11:23.300348 stigg_api_client_v2-0.477.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-09 16:11:23.424356 stigg_api_client_v2-0.477.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-09 16:11:23.316349 stigg_api_client_v2-0.477.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-09 16:11:23.344350 stigg_api_client_v2-0.477.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-09 16:11:23.408355 stigg_api_client_v2-0.477.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-09 16:11:23.404354 stigg_api_client_v2-0.477.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-09 16:11:23.396354 stigg_api_client_v2-0.477.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-09 16:11:24.416421 stigg_api_client_v2-0.477.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-09 16:11:23.336350 stigg_api_client_v2-0.477.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-09 16:11:23.360352 stigg_api_client_v2-0.477.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-09 16:11:23.512362 stigg_api_client_v2-0.477.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.477.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.476.0/README.md` & `stigg_api_client_v2-0.477.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.476.0/stigg/client.py` & `stigg_api_client_v2-0.477.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.477.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.477.0/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.477.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.477.0/stigg/generated/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.477.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.477.0/stigg/generated/cancel_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/client.py` & `stigg_api_client_v2-0.477.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.477.0/stigg/generated/create_subscription.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.477.0/stigg/generated/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
@@ -360,14 +360,15 @@
     ExperimentStatusError = "ExperimentStatusError"
     FailedToCreateCheckoutSessionError = "FailedToCreateCheckoutSessionError"
     FailedToImportCustomer = "FailedToImportCustomer"
     FeatureNotFound = "FeatureNotFound"
     FetchAllCountriesPricesNotAllowed = "FetchAllCountriesPricesNotAllowed"
     IdentityForbidden = "IdentityForbidden"
     ImportAlreadyInProgress = "ImportAlreadyInProgress"
+    ImportSubscriptionsBulkError = "ImportSubscriptionsBulkError"
     InitStripePaymentMethodError = "InitStripePaymentMethodError"
     IntegrationNotFound = "IntegrationNotFound"
     IntegrityViolation = "IntegrityViolation"
     InvalidAddressError = "InvalidAddressError"
     InvalidArgumentError = "InvalidArgumentError"
     InvalidCancellationDate = "InvalidCancellationDate"
     InvalidEntitlementResetPeriod = "InvalidEntitlementResetPeriod"
@@ -455,14 +456,15 @@
     ENTITLEMENT_REQUESTED = "ENTITLEMENT_REQUESTED"
     ENVIRONMENT_DELETED = "ENVIRONMENT_DELETED"
     FEATURE_CREATED = "FEATURE_CREATED"
     FEATURE_DELETED = "FEATURE_DELETED"
     FEATURE_UPDATED = "FEATURE_UPDATED"
     IMPORT_INTEGRATION_CATALOG_TRIGGERED = "IMPORT_INTEGRATION_CATALOG_TRIGGERED"
     IMPORT_INTEGRATION_CUSTOMERS_TRIGGERED = "IMPORT_INTEGRATION_CUSTOMERS_TRIGGERED"
+    IMPORT_SUBSCRIPTIONS_BULK_TRIGGERED = "IMPORT_SUBSCRIPTIONS_BULK_TRIGGERED"
     MEASUREMENT_REPORTED = "MEASUREMENT_REPORTED"
     PACKAGE_PUBLISHED = "PACKAGE_PUBLISHED"
     PLAN_CREATED = "PLAN_CREATED"
     PLAN_DELETED = "PLAN_DELETED"
     PLAN_UPDATED = "PLAN_UPDATED"
     PRODUCT_CREATED = "PRODUCT_CREATED"
     PRODUCT_DELETED = "PRODUCT_DELETED"
@@ -826,14 +828,15 @@
     PARTIALLY_FAILED = "PARTIALLY_FAILED"
     PENDING = "PENDING"
 
 
 class TaskType(str, Enum):
     IMPORT_INTEGRATION_CATALOG = "IMPORT_INTEGRATION_CATALOG"
     IMPORT_INTEGRATION_CUSTOMERS = "IMPORT_INTEGRATION_CUSTOMERS"
+    IMPORT_SUBSCRIPTIONS_BULK = "IMPORT_SUBSCRIPTIONS_BULK"
     RECALCULATE_ENTITLEMENTS = "RECALCULATE_ENTITLEMENTS"
     RESYNC_INTEGRATION = "RESYNC_INTEGRATION"
     SUBSCRIPTION_MIGRATION = "SUBSCRIPTION_MIGRATION"
 
 
 class TrialPeriodUnits(str, Enum):
     DAY = "DAY"
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.477.0/stigg/generated/estimate_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.477.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.477.0/stigg/generated/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.477.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,14 +32,36 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
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
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -55,36 +77,14 @@
 class PriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
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
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -328,18 +328,14 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class CustomerPortalPromotionalEntitlement(BaseModel):
     display_name: str = Field(alias="displayName")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     usage_limit: Optional[float] = Field(alias="usageLimit")
     period: PromotionalEntitlementPeriod
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -504,14 +500,18 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -842,34 +842,14 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
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
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -884,14 +864,34 @@
 
 class MockPaywallPriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
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
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1311,19 +1311,19 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
 SlimCustomerFragment.update_forward_refs()
@@ -1346,15 +1346,14 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
@@ -1369,14 +1368,15 @@
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
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
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.477.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.477.0/stigg/generated/get_coupons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.477.0/stigg/generated/get_customer_by_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.477.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.477.0/stigg/generated/get_mock_paywall.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.477.0/stigg/generated/get_products.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.477.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.477.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.477.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.477.0/stigg/generated/provision_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.477.0/stigg/generated/provision_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.477.0/stigg/generated/report_usage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.476.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.477.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 10:55
+# Generated by ariadne-codegen on 2023-07-09 16:11
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.476.0/PKG-INFO` & `stigg_api_client_v2-0.477.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.476.0
+Version: 0.477.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

