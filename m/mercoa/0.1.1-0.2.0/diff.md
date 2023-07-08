# Comparing `tmp/mercoa-0.1.1.tar.gz` & `tmp/mercoa-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.1.1.tar", max compression
+gzip compressed data, was "mercoa-0.2.0.tar", max compression
```

## Comparing `mercoa-0.1.1.tar` & `mercoa-0.2.0.tar`

### file list

```diff
@@ -1,167 +1,181 @@
--rw-r--r--   0        0        0      410 2023-06-14 06:27:11.377764 mercoa-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6227 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/__init__.py
--rw-r--r--   0        0        0     5449 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      326 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/py.typed
--rw-r--r--   0        0        0     6414 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     2582 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      397 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      148 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      216 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0      469 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      441 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/order_direction.py
--rw-r--r--   0        0        0      855 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      199 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4513 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/client.py
--rw-r--r--   0        0        0      256 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/types/__init__.py
--rw-r--r--   0        0        0     1022 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/types/counterparty_response.py
--rw-r--r--   0        0        0     1446 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/types/find_counterparties_response.py
--rw-r--r--   0        0        0     1491 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    34975 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0     2109 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/__init__.py
--rw-r--r--   0        0        0      487 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/account_type.py
--rw-r--r--   0        0        0      836 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/amount_trigger.py
--rw-r--r--   0        0        0     1075 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_request.py
--rw-r--r--   0        0        0     1003 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_response.py
--rw-r--r--   0        0        0     1059 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_update_request.py
--rw-r--r--   0        0        0      963 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/approver_rule.py
--rw-r--r--   0        0        0     1535 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/business_profile_request.py
--rw-r--r--   0        0        0     1492 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/business_type.py
--rw-r--r--   0        0        0      741 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/ein.py
--rw-r--r--   0        0        0      914 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_add_payees_request.py
--rw-r--r--   0        0        0       80 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_id.py
--rw-r--r--   0        0        0     2432 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_request.py
--rw-r--r--   0        0        0     1814 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_status.py
--rw-r--r--   0        0        0     2084 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_update_request.py
--rw-r--r--   0        0        0      727 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/identifier_list.py
--rw-r--r--   0        0        0     1372 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/individual_profile_response.py
--rw-r--r--   0        0        0     1059 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/invoice_metrics_response.py
--rw-r--r--   0        0        0       80 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/policy_id.py
--rw-r--r--   0        0        0      974 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/profile_response.py
--rw-r--r--   0        0        0      428 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/rule.py
--rw-r--r--   0        0        0      761 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/tax_id.py
--rw-r--r--   0        0        0      594 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/trigger.py
--rw-r--r--   0        0        0      207 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/__init__.py
--rw-r--r--   0        0        0     9662 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/client.py
--rw-r--r--   0        0        0      281 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/types/__init__.py
--rw-r--r--   0        0        0       84 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_id.py
--rw-r--r--   0        0        0     1100 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_request.py
--rw-r--r--   0        0        0     1224 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_response.py
--rw-r--r--   0        0        0      831 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    23201 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0     1228 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/__init__.py
--rw-r--r--   0        0        0      935 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/approval_request.py
--rw-r--r--   0        0        0      843 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/approver.py
--rw-r--r--   0        0        0      631 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/approver_action.py
--rw-r--r--   0        0        0      862 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/approver_response.py
--rw-r--r--   0        0        0       81 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_id.py
--rw-r--r--   0        0        0      934 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_request.py
--rw-r--r--   0        0        0     1128 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_response.py
--rw-r--r--   0        0        0    22179 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/currency_code.py
--rw-r--r--   0        0        0      955 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/document_response.py
--rw-r--r--   0        0        0       81 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_id.py
--rw-r--r--   0        0        0     1302 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1229 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_line_item_response.py
--rw-r--r--   0        0        0      870 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_order_by_field.py
--rw-r--r--   0        0        0     3437 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_request.py
--rw-r--r--   0        0        0     4234 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_response.py
--rw-r--r--   0        0        0     1485 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_status.py
--rw-r--r--   0        0        0      922 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/set_approver.py
--rw-r--r--   0        0        0      213 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4340 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      298 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1068 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/ocr/types/attachments.py
--rw-r--r--   0        0        0     1969 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/ocr/types/email_ocr_request.py
--rw-r--r--   0        0        0      891 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/ocr/types/ocr_mailbox.py
--rw-r--r--   0        0        0     1234 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      983 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0     7449 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1466 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      948 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      656 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1463 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1579 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1145 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      797 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0     1087 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    14367 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/client.py
--rw-r--r--   0        0        0     1638 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/__init__.py
--rw-r--r--   0        0        0       85 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_id.py
--rw-r--r--   0        0        0     1297 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_request.py
--rw-r--r--   0        0        0     1318 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_type.py
--rw-r--r--   0        0        0      819 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_brand.py
--rw-r--r--   0        0        0       78 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_id.py
--rw-r--r--   0        0        0     1120 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_request.py
--rw-r--r--   0        0        0     1217 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_response.py
--rw-r--r--   0        0        0      750 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_type.py
--rw-r--r--   0        0        0       79 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_id.py
--rw-r--r--   0        0        0     1152 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_request.py
--rw-r--r--   0        0        0     1327 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_response.py
--rw-r--r--   0        0        0       80 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_id.py
--rw-r--r--   0        0        0     1568 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1922 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
--rw-r--r--   0        0        0     1639 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py
--rw-r--r--   0        0        0       87 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_id.py
--rw-r--r--   0        0        0     1296 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_request.py
--rw-r--r--   0        0        0     1662 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_response.py
--rw-r--r--   0        0        0     1229 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_type.py
--rw-r--r--   0        0        0      893 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_update_request.py
--rw-r--r--   0        0        0      425 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0     7794 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0      589 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/__init__.py
--rw-r--r--   0        0        0     1984 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1597 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1709 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
--rw-r--r--   0        0        0      143 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/process_invoice/__init__.py
--rw-r--r--   0        0        0     2498 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/process_invoice/client.py
--rw-r--r--   0        0        0      161 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/process_invoice/types/__init__.py
--rw-r--r--   0        0        0      916 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/process_invoice/types/process_invoice_request.py
--rw-r--r--   0        0        0      269 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/__init__.py
--rw-r--r--   0        0        0     8182 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/client.py
--rw-r--r--   0        0        0      381 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/__init__.py
--rw-r--r--   0        0        0       88 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/responsibilities.py
--rw-r--r--   0        0        0      271 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/__init__.py
--rw-r--r--   0        0        0     4315 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/client.py
--rw-r--r--   0        0        0      386 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/__init__.py
--rw-r--r--   0        0        0       85 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_id.py
--rw-r--r--   0        0        0     1125 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_response.py
--rw-r--r--   0        0        0     1564 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_response_expanded.py
--rw-r--r--   0        0        0     1261 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_status.py
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1930 2023-07-08 22:39:19.354413 mercoa-0.2.0/README.md
+-rw-r--r--   0        0        0      368 2023-07-08 22:39:19.354413 mercoa-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4199 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     2384 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/py.typed
+-rw-r--r--   0        0        0     4280 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     3801 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      814 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      237 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
+-rw-r--r--   0        0        0      221 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/errors/auth_header_missing_error.py
+-rw-r--r--   0        0        0      225 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/errors/unauthorized.py
+-rw-r--r--   0        0        0      947 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0       88 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/approval_policy_id.py
+-rw-r--r--   0        0        0      824 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0       81 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/comment_id.py
+-rw-r--r--   0        0        0       80 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/entity_id.py
+-rw-r--r--   0        0        0       84 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/entity_user_id.py
+-rw-r--r--   0        0        0      994 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0       81 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/invoice_id.py
+-rw-r--r--   0        0        0      857 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      441 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/order_direction.py
+-rw-r--r--   0        0        0       87 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/payment_method_id.py
+-rw-r--r--   0        0        0       93 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0      855 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0     2246 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    33504 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0     1593 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/__init__.py
+-rw-r--r--   0        0        0      854 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/__init__.py
+-rw-r--r--   0        0        0    17631 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/client.py
+-rw-r--r--   0        0        0      305 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
+-rw-r--r--   0        0        0      248 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
+-rw-r--r--   0        0        0      854 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/__init__.py
+-rw-r--r--   0        0        0      847 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/amount_trigger.py
+-rw-r--r--   0        0        0     1120 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_request.py
+-rw-r--r--   0        0        0     1056 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_response.py
+-rw-r--r--   0        0        0     1087 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_update_request.py
+-rw-r--r--   0        0        0      965 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approver_rule.py
+-rw-r--r--   0        0        0      651 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/identifier_list.py
+-rw-r--r--   0        0        0      391 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/rule.py
+-rw-r--r--   0        0        0      573 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/trigger.py
+-rw-r--r--   0        0        0      199 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4088 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/client.py
+-rw-r--r--   0        0        0      256 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/counterparty_response.py
+-rw-r--r--   0        0        0     1448 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/find_counterparties_response.py
+-rw-r--r--   0        0        0      145 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    11190 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/client.py
+-rw-r--r--   0        0        0      164 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/types/__init__.py
+-rw-r--r--   0        0        0     1070 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0       65 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    22264 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/payment_method/client.py
+-rw-r--r--   0        0        0      269 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/__init__.py
+-rw-r--r--   0        0        0    12714 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/client.py
+-rw-r--r--   0        0        0      381 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_id.py
+-rw-r--r--   0        0        0     1382 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_request.py
+-rw-r--r--   0        0        0     1547 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_response.py
+-rw-r--r--   0        0        0     1102 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/responsibilities.py
+-rw-r--r--   0        0        0      177 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/__init__.py
+-rw-r--r--   0        0        0    15285 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/client.py
+-rw-r--r--   0        0        0      224 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/__init__.py
+-rw-r--r--   0        0        0     1102 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/entity_user_request.py
+-rw-r--r--   0        0        0     1244 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/entity_user_response.py
+-rw-r--r--   0        0        0     1148 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/account_type.py
+-rw-r--r--   0        0        0     1535 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/business_profile_request.py
+-rw-r--r--   0        0        0     1492 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/business_type.py
+-rw-r--r--   0        0        0      741 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/ein.py
+-rw-r--r--   0        0        0      930 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_add_payees_request.py
+-rw-r--r--   0        0        0     2432 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_request.py
+-rw-r--r--   0        0        0     1830 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_status.py
+-rw-r--r--   0        0        0     2084 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_update_request.py
+-rw-r--r--   0        0        0     1372 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/individual_profile_response.py
+-rw-r--r--   0        0        0      974 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/profile_response.py
+-rw-r--r--   0        0        0      761 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/tax_id.py
+-rw-r--r--   0        0        0      867 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    20763 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      391 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/__init__.py
+-rw-r--r--   0        0        0      131 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/__init__.py
+-rw-r--r--   0        0        0     6536 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/client.py
+-rw-r--r--   0        0        0      142 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/types/__init__.py
+-rw-r--r--   0        0        0     1016 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/types/approval_request.py
+-rw-r--r--   0        0        0      165 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/__init__.py
+-rw-r--r--   0        0        0    15286 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/client.py
+-rw-r--r--   0        0        0      204 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/__init__.py
+-rw-r--r--   0        0        0      933 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/comment_request.py
+-rw-r--r--   0        0        0     1450 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/comment_response.py
+-rw-r--r--   0        0        0      133 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/__init__.py
+-rw-r--r--   0        0        0     3847 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/client.py
+-rw-r--r--   0        0        0      145 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/types/__init__.py
+-rw-r--r--   0        0        0      853 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/types/document_response.py
+-rw-r--r--   0        0        0      877 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/__init__.py
+-rw-r--r--   0        0        0      631 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/approver_action.py
+-rw-r--r--   0        0        0      900 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/assigned_approver.py
+-rw-r--r--   0        0        0      979 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/associated_approval_action.py
+-rw-r--r--   0        0        0     1404 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_approver_response.py
+-rw-r--r--   0        0        0     1325 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1252 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0      870 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_order_by_field.py
+-rw-r--r--   0        0        0     3439 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_request.py
+-rw-r--r--   0        0        0     4299 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_response.py
+-rw-r--r--   0        0        0     1485 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_status.py
+-rw-r--r--   0        0        0      155 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4419 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      189 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1234 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      642 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/types/vendor_network.py
+-rw-r--r--   0        0        0      983 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0    10870 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0     1466 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_provider_response.py
+-rw-r--r--   0        0        0      785 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_response.py
+-rw-r--r--   0        0        0       86 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/organization_id.py
+-rw-r--r--   0        0        0     1463 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/organization_request.py
+-rw-r--r--   0        0        0     1579 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1145 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_request.py
+-rw-r--r--   0        0        0      843 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_response.py
+-rw-r--r--   0        0        0     1597 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0     2083 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/__init__.py
+-rw-r--r--   0        0        0     1215 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_account_request.py
+-rw-r--r--   0        0        0     1478 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_type.py
+-rw-r--r--   0        0        0      819 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_brand.py
+-rw-r--r--   0        0        0     1141 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_request.py
+-rw-r--r--   0        0        0     1480 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_type.py
+-rw-r--r--   0        0        0     1152 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/check_request.py
+-rw-r--r--   0        0        0     1506 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/check_response.py
+-rw-r--r--   0        0        0    22179 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/currency_code.py
+-rw-r--r--   0        0        0     1554 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     2084 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0     1625 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py
+-rw-r--r--   0        0        0     1264 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_request.py
+-rw-r--r--   0        0        0     1298 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_response.py
+-rw-r--r--   0        0        0     1229 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_type.py
+-rw-r--r--   0        0        0      514 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_update_request.py
+-rw-r--r--   0        0        0      369 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0    12318 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0      500 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/__init__.py
+-rw-r--r--   0        0        0     1984 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0     1604 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1732 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0      271 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     6642 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      386 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1132 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1564 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_response_expanded.py
+-rw-r--r--   0        0        0     1261 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.0/PKG-INFO
```

### Comparing `mercoa-0.1.1/src/mercoa/core/datetime_utils.py` & `mercoa-0.2.0/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.2.0/src/mercoa/core/jsonable_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 (e.g. datetimes to strings, Pydantic models to dicts).
 
 Taken from FastAPI, and made a bit simpler
 https://github.com/tiangolo/fastapi/blob/master/fastapi/encoders.py
 """
 
 import dataclasses
+import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
 from pydantic import BaseModel
 from pydantic.json import ENCODERS_BY_TYPE
 
+from .datetime_utils import serialize_datetime
+
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
@@ -56,14 +59,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
+    if isinstance(obj, dt.date):
+        return str(obj)
+    if isinstance(obj, dt.datetime):
+        return serialize_datetime(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.2.0/src/mercoa/resources/bank_lookup/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,78 @@
 # This file was auto-generated by Fern from our API Definition.
 
-import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
+from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
+from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
+from ..commons.errors.unauthorized import Unauthorized
 from .types.bank_lookup_response import BankLookupResponse
 
 
 class BankLookupClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     def find(self, *, routing_number: str) -> BankLookupResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "bankLookup"),
             params={"routingNumber": routing_number},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BankLookupResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncBankLookupClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     async def find(self, *, routing_number: str) -> BankLookupResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "bankLookup"),
                 params={"routingNumber": routing_number},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BankLookupResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/commons/types/address.py` & `mercoa-0.2.0/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.2.0/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.2.0/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/types/document_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from .itin import ITIN
-from .ssn import SSN
+from ......core.datetime_utils import serialize_datetime
 
 
-class IndividualGovernmentID(pydantic.BaseModel):
-    ssn: typing.Optional[SSN]
-    itin: typing.Optional[ITIN]
+class DocumentResponse(pydantic.BaseModel):
+    mime_type: str = pydantic.Field(alias="mimeType")
+    uri: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.2.0/src/mercoa/resources/commons/types/itin.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class ITIN(pydantic.BaseModel):
+class Itin(pydantic.BaseModel):
     full: typing.Optional[str]
     last_four: str = pydantic.Field(alias="lastFour")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.2.0/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.2.0/src/mercoa/resources/commons/types/ssn.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class SSN(pydantic.BaseModel):
+class Ssn(pydantic.BaseModel):
     full: typing.Optional[str]
     last_four: str = pydantic.Field(alias="lastFour")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/counterparty/client.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,99 +3,80 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ...core.api_error import ApiError
-from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import MercoaEnvironment
-from ..entity.types.entity_id import EntityId
-from ..entity.types.entity_response import EntityResponse
+from .....core.api_error import ApiError
+from .....core.remove_none_from_headers import remove_none_from_headers
+from .....environment import MercoaEnvironment
+from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
+from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
+from ....commons.errors.unauthorized import Unauthorized
+from ....commons.types.entity_id import EntityId
 from .types.find_counterparties_response import FindCounterpartiesResponse
 
 
 class CounterpartyClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
-    def get_all(self) -> typing.List[EntityResponse]:
-        _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "counterparties"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
     def find(self, entity_id: EntityId, *, payment_methods: typing.Optional[bool] = None) -> FindCounterpartiesResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/counterparties"),
             params={"paymentMethods": payment_methods},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(FindCounterpartiesResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncCounterpartyClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
-    async def get_all(self) -> typing.List[EntityResponse]:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "counterparties"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
     async def find(
         self, entity_id: EntityId, *, payment_methods: typing.Optional[bool] = None
     ) -> FindCounterpartiesResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/counterparties"),
                 params={"paymentMethods": payment_methods},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(FindCounterpartiesResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/counterparty/types/counterparty_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/counterparty_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from ...entity.types.entity_response import EntityResponse
-from ...payment_method.types.payment_method_response import PaymentMethodResponse
+from ......core.datetime_utils import serialize_datetime
+from .....payment_method.types.payment_method_response import PaymentMethodResponse
+from ....types.entity_response import EntityResponse
 
 
 class CounterpartyResponse(EntityResponse):
     payment_methods: typing.List[PaymentMethodResponse] = pydantic.Field(alias="paymentMethods")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/counterparty/types/find_counterparties_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/find_counterparties_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
+from ......core.datetime_utils import serialize_datetime
 from .counterparty_response import CounterpartyResponse
 
 
 class FindCounterpartiesResponse(pydantic.BaseModel):
     entity_counterparties: typing.List[CounterpartyResponse] = pydantic.Field(
         alias="entityCounterparties", description=("Counterparties that have been paid by this entity\n")
     )
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/client.py` & `mercoa-0.2.0/src/mercoa/resources/entity/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,717 +1,609 @@
 # This file was auto-generated by Fern from our API Definition.
 
-import datetime as dt
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
-from ...core.datetime_utils import serialize_datetime
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
-from ..commons.types.order_direction import OrderDirection
-from ..invoice.types.currency_code import CurrencyCode
-from ..invoice.types.invoice_id import InvoiceId
-from ..invoice.types.invoice_order_by_field import InvoiceOrderByField
-from ..invoice.types.invoice_response import InvoiceResponse
-from ..invoice.types.invoice_status import InvoiceStatus
-from .types.approval_policy_request import ApprovalPolicyRequest
-from .types.approval_policy_response import ApprovalPolicyResponse
-from .types.approval_policy_update_request import ApprovalPolicyUpdateRequest
+from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
+from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
+from ..commons.errors.unauthorized import Unauthorized
+from ..commons.types.entity_id import EntityId
+from .resources.approval_policy.client import ApprovalPolicyClient, AsyncApprovalPolicyClient
+from .resources.counterparty.client import AsyncCounterpartyClient, CounterpartyClient
+from .resources.invoice.client import AsyncInvoiceClient, InvoiceClient
+from .resources.payment_method.client import AsyncPaymentMethodClient, PaymentMethodClient
+from .resources.representative.client import AsyncRepresentativeClient, RepresentativeClient
+from .resources.user.client import AsyncUserClient, UserClient
 from .types.entity_add_payees_request import EntityAddPayeesRequest
-from .types.entity_id import EntityId
 from .types.entity_request import EntityRequest
 from .types.entity_response import EntityResponse
 from .types.entity_status import EntityStatus
 from .types.entity_update_request import EntityUpdateRequest
-from .types.invoice_metrics_response import InvoiceMetricsResponse
-from .types.policy_id import PolicyId
 
 
 class EntityClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
+        self.approval_policy = ApprovalPolicyClient(environment=self._environment, token=self._token)
+        self.counterparty = CounterpartyClient(environment=self._environment, token=self._token)
+        self.invoice = InvoiceClient(environment=self._environment, token=self._token)
+        self.payment_method = PaymentMethodClient(environment=self._environment, token=self._token)
+        self.representative = RepresentativeClient(environment=self._environment, token=self._token)
+        self.user = UserClient(environment=self._environment, token=self._token)
 
-    def get_all(self) -> typing.List[EntityResponse]:
+    def get_all(
+        self, *, is_payee: typing.Optional[bool] = None, is_payor: typing.Optional[bool] = None
+    ) -> typing.List[EntityResponse]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "entities"),
+            params={"isPayee": is_payee, "isPayor": is_payor},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def find(
         self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
     ) -> typing.List[EntityResponse]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
             params={"foreignId": foreign_id, "status": status},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(self, *, request: EntityRequest) -> EntityResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, entity_id: EntityId) -> EntityResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(self, entity_id: EntityId, *, request: EntityUpdateRequest) -> EntityResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, entity_id: EntityId) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_invoices(
-        self,
-        entity_id: EntityId,
-        *,
-        start_date: typing.Optional[dt.datetime] = None,
-        end_date: typing.Optional[dt.datetime] = None,
-        order_by: typing.Optional[InvoiceOrderByField] = None,
-        order_direction: typing.Optional[OrderDirection] = None,
-        limit: typing.Optional[int] = None,
-        starting_after: typing.Optional[InvoiceId] = None,
-        search: typing.Optional[str] = None,
-        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-    ) -> typing.List[InvoiceResponse]:
-        _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
-            params={
-                "startDate": serialize_datetime(start_date) if start_date is not None else None,
-                "endDate": serialize_datetime(end_date) if end_date is not None else None,
-                "orderBy": order_by,
-                "orderDirection": order_direction,
-                "limit": limit,
-                "startingAfter": starting_after,
-                "search": search,
-                "status": status,
-            },
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_invoice_metrics(
-        self,
-        entity_id: EntityId,
-        *,
-        search: typing.Optional[str] = None,
-        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-        due_date_start: typing.Optional[dt.datetime] = None,
-        due_date_end: typing.Optional[dt.datetime] = None,
-        created_date_start: typing.Optional[dt.datetime] = None,
-        created_date_end: typing.Optional[dt.datetime] = None,
-        currency: CurrencyCode,
-    ) -> InvoiceMetricsResponse:
-        _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoice-metrics"),
-            params={
-                "search": search,
-                "status": status,
-                "dueDateStart": serialize_datetime(due_date_start) if due_date_start is not None else None,
-                "dueDateEnd": serialize_datetime(due_date_end) if due_date_end is not None else None,
-                "createdDateStart": serialize_datetime(created_date_start) if created_date_start is not None else None,
-                "createdDateEnd": serialize_datetime(created_date_end) if created_date_end is not None else None,
-                "currency": currency,
-            },
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceMetricsResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def accept_terms_of_service(self, entity_id: EntityId) -> str:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_token(self, entity_id: EntityId) -> str:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def plaid_link_token(self, entity_id: EntityId) -> str:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def add_payees(self, entity_id: EntityId, *, request: EntityAddPayeesRequest) -> None:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/addPayees"),
-            json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def create_approval_policy(self, entity_id: EntityId, *, request: ApprovalPolicyRequest) -> ApprovalPolicyResponse:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policy"),
-            json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApprovalPolicyResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_approval_policy(self, entity_id: EntityId, policy_id: PolicyId) -> ApprovalPolicyResponse:
+    def oatfi_preapproval(self, entity_id: EntityId) -> bool:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policy/{policy_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/oatfiPreapproval"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApprovalPolicyResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(bool, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_approval_policy(
-        self, entity_id: EntityId, policy_id: PolicyId, *, request: ApprovalPolicyUpdateRequest
-    ) -> ApprovalPolicyResponse:
+    def add_payees(self, entity_id: EntityId, *, request: EntityAddPayeesRequest) -> None:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policy/{policy_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/addPayees"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApprovalPolicyResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def delete_approval_policy(self, entity_id: EntityId, policy_id: PolicyId) -> None:
-        _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policy/{policy_id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_all_approval_policies(self, entity_id: EntityId) -> typing.List[ApprovalPolicyResponse]:
-        _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policies"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[ApprovalPolicyResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncEntityClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
+        self.approval_policy = AsyncApprovalPolicyClient(environment=self._environment, token=self._token)
+        self.counterparty = AsyncCounterpartyClient(environment=self._environment, token=self._token)
+        self.invoice = AsyncInvoiceClient(environment=self._environment, token=self._token)
+        self.payment_method = AsyncPaymentMethodClient(environment=self._environment, token=self._token)
+        self.representative = AsyncRepresentativeClient(environment=self._environment, token=self._token)
+        self.user = AsyncUserClient(environment=self._environment, token=self._token)
 
-    async def get_all(self) -> typing.List[EntityResponse]:
+    async def get_all(
+        self, *, is_payee: typing.Optional[bool] = None, is_payor: typing.Optional[bool] = None
+    ) -> typing.List[EntityResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "entities"),
+                params={"isPayee": is_payee, "isPayor": is_payor},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def find(
         self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
     ) -> typing.List[EntityResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
                 params={"foreignId": foreign_id, "status": status},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(self, *, request: EntityRequest) -> EntityResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, entity_id: EntityId) -> EntityResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(self, entity_id: EntityId, *, request: EntityUpdateRequest) -> EntityResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, entity_id: EntityId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_invoices(
-        self,
-        entity_id: EntityId,
-        *,
-        start_date: typing.Optional[dt.datetime] = None,
-        end_date: typing.Optional[dt.datetime] = None,
-        order_by: typing.Optional[InvoiceOrderByField] = None,
-        order_direction: typing.Optional[OrderDirection] = None,
-        limit: typing.Optional[int] = None,
-        starting_after: typing.Optional[InvoiceId] = None,
-        search: typing.Optional[str] = None,
-        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-    ) -> typing.List[InvoiceResponse]:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
-                params={
-                    "startDate": serialize_datetime(start_date) if start_date is not None else None,
-                    "endDate": serialize_datetime(end_date) if end_date is not None else None,
-                    "orderBy": order_by,
-                    "orderDirection": order_direction,
-                    "limit": limit,
-                    "startingAfter": starting_after,
-                    "search": search,
-                    "status": status,
-                },
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_invoice_metrics(
-        self,
-        entity_id: EntityId,
-        *,
-        search: typing.Optional[str] = None,
-        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-        due_date_start: typing.Optional[dt.datetime] = None,
-        due_date_end: typing.Optional[dt.datetime] = None,
-        created_date_start: typing.Optional[dt.datetime] = None,
-        created_date_end: typing.Optional[dt.datetime] = None,
-        currency: CurrencyCode,
-    ) -> InvoiceMetricsResponse:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoice-metrics"),
-                params={
-                    "search": search,
-                    "status": status,
-                    "dueDateStart": serialize_datetime(due_date_start) if due_date_start is not None else None,
-                    "dueDateEnd": serialize_datetime(due_date_end) if due_date_end is not None else None,
-                    "createdDateStart": serialize_datetime(created_date_start)
-                    if created_date_start is not None
-                    else None,
-                    "createdDateEnd": serialize_datetime(created_date_end) if created_date_end is not None else None,
-                    "currency": currency,
-                },
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceMetricsResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def accept_terms_of_service(self, entity_id: EntityId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_token(self, entity_id: EntityId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def plaid_link_token(self, entity_id: EntityId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def add_payees(self, entity_id: EntityId, *, request: EntityAddPayeesRequest) -> None:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/addPayees"),
-                json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def create_approval_policy(
-        self, entity_id: EntityId, *, request: ApprovalPolicyRequest
-    ) -> ApprovalPolicyResponse:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policy"),
-                json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApprovalPolicyResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_approval_policy(self, entity_id: EntityId, policy_id: PolicyId) -> ApprovalPolicyResponse:
+    async def oatfi_preapproval(self, entity_id: EntityId) -> bool:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policy/{policy_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/oatfiPreapproval"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApprovalPolicyResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(bool, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_approval_policy(
-        self, entity_id: EntityId, policy_id: PolicyId, *, request: ApprovalPolicyUpdateRequest
-    ) -> ApprovalPolicyResponse:
+    async def add_payees(self, entity_id: EntityId, *, request: EntityAddPayeesRequest) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policy/{policy_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/addPayees"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApprovalPolicyResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def delete_approval_policy(self, entity_id: EntityId, policy_id: PolicyId) -> None:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policy/{policy_id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_all_approval_policies(self, entity_id: EntityId) -> typing.List[ApprovalPolicyResponse]:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/approval-policies"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[ApprovalPolicyResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/amount_trigger.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/amount_trigger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from ...invoice.types.currency_code import CurrencyCode
+from ......core.datetime_utils import serialize_datetime
+from .....payment_method.types.currency_code import CurrencyCode
 
 
 class AmountTrigger(pydantic.BaseModel):
     amount: float
     currency: CurrencyCode
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_request.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from .policy_id import PolicyId
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.approval_policy_id import ApprovalPolicyId
 from .rule import Rule
 from .trigger import Trigger
 
 
 class ApprovalPolicyRequest(pydantic.BaseModel):
     trigger: Trigger
     rule: Rule
-    upstream_policy_id: PolicyId = pydantic.Field(
+    upstream_policy_id: ApprovalPolicyId = pydantic.Field(
         alias="upstreamPolicyId", description=("Use 'root' if no upstreamPolicyId is intended to be set.\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_add_payees_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,30 +2,26 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .policy_id import PolicyId
-from .rule import Rule
-from .trigger import Trigger
+from ...commons.types.entity_id import EntityId
 
 
-class ApprovalPolicyResponse(pydantic.BaseModel):
-    id: PolicyId
-    trigger: Trigger
-    rule: Rule
-    upstream_policy_id: PolicyId = pydantic.Field(alias="upstreamPolicyId")
+class EntityAddPayeesRequest(pydantic.BaseModel):
+    payees: typing.List[EntityId] = pydantic.Field(
+        description=("List of payee entity IDs to associate with the entity\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_update_request.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/email_provider_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .policy_id import PolicyId
-from .rule import Rule
-from .trigger import Trigger
+from .email_sender_request import EmailSenderRequest
 
 
-class ApprovalPolicyUpdateRequest(pydantic.BaseModel):
-    id: PolicyId
-    trigger: typing.Optional[Trigger]
-    rule: typing.Optional[Rule]
-    upstream_policy_id: typing.Optional[PolicyId] = pydantic.Field(alias="upstreamPolicyId")
+class EmailProviderRequest(pydantic.BaseModel):
+    sender: EmailSenderRequest
+    inbox_domain: str = pydantic.Field(alias="inboxDomain")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/approver_rule.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approver_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
+from ......core.datetime_utils import serialize_datetime
 from .identifier_list import IdentifierList
 
 
 class ApproverRule(pydantic.BaseModel):
     num_approvers: int = pydantic.Field(alias="numApprovers")
     identifier_list: IdentifierList = pydantic.Field(alias="identifierList")
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/business_profile_request.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/business_profile_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...commons.types.address import Address
 from ...commons.types.phone_number import PhoneNumber
 from .business_type import BusinessType
-from .tax_id import TaxID
+from .tax_id import TaxId
 
 
 class BusinessProfileRequest(pydantic.BaseModel):
     email: typing.Optional[str]
     legal_business_name: str = pydantic.Field(alias="legalBusinessName")
     business_type: typing.Optional[BusinessType] = pydantic.Field(alias="businessType")
     phone: typing.Optional[PhoneNumber]
     doing_business_as: typing.Optional[str] = pydantic.Field(alias="doingBusinessAs")
     website: typing.Optional[str]
     description: typing.Optional[str]
     address: typing.Optional[Address]
     owners_provided: typing.Optional[bool] = pydantic.Field(alias="ownersProvided")
-    tax_id: typing.Optional[TaxID] = pydantic.Field(alias="taxId")
+    tax_id: typing.Optional[TaxId] = pydantic.Field(alias="taxId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/business_profile_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/business_type.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/ein.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_add_payees_request.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/comment_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from .entity_id import EntityId
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.entity_user_id import EntityUserId
 
 
-class EntityAddPayeesRequest(pydantic.BaseModel):
-    payees: typing.List[EntityId] = pydantic.Field(
-        description=("List of payee entity IDs to associate with the entity\n")
-    )
+class CommentRequest(pydantic.BaseModel):
+    text: str
+    user_id: typing.Optional[EntityUserId] = pydantic.Field(alias="userId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_request.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...commons.types.entity_id import EntityId
 from .account_type import AccountType
-from .entity_id import EntityId
 from .entity_status import EntityStatus
 from .profile_response import ProfileResponse
 
 
 class EntityResponse(pydantic.BaseModel):
     id: EntityId
     foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_status.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_update_request.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/identifier_list.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/identifier_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import typing
 
 import pydantic
 import typing_extensions
 
-from ...entity_users.types.entity_user_id import EntityUserId
+from .....commons.types.entity_user_id import EntityUserId
 
 
 class IdentifierList_RolesList(pydantic.BaseModel):
     type: typing_extensions.Literal["rolesList"]
     value: typing.List[str]
 
     class Config:
@@ -22,10 +22,8 @@
     type: typing_extensions.Literal["userList"]
     value: typing.List[EntityUserId]
 
     class Config:
         frozen = True
 
 
-IdentifierList = typing_extensions.Annotated[
-    typing.Union[IdentifierList_RolesList, IdentifierList_UserList], pydantic.Field(discriminator="type")
-]
+IdentifierList = typing.Union[IdentifierList_RolesList, IdentifierList_UserList]
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/individual_profile_request.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/individual_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...commons.types.address import Address
 from ...commons.types.birth_date import BirthDate
 from ...commons.types.full_name import FullName
-from ...commons.types.individual_government_id import IndividualGovernmentID
+from ...commons.types.individual_government_id import IndividualGovernmentId
 from ...commons.types.phone_number import PhoneNumber
 
 
 class IndividualProfileRequest(pydantic.BaseModel):
     email: typing.Optional[str]
     name: FullName
     phone: typing.Optional[PhoneNumber]
     address: typing.Optional[Address]
     birth_date: typing.Optional[BirthDate] = pydantic.Field(alias="birthDate")
-    government_id: typing.Optional[IndividualGovernmentID] = pydantic.Field(alias="governmentID")
+    government_id: typing.Optional[IndividualGovernmentId] = pydantic.Field(alias="governmentID")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/individual_profile_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/invoice_metrics_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/types/invoice_metrics_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from ...invoice.types.currency_code import CurrencyCode
+from ......core.datetime_utils import serialize_datetime
+from .....payment_method.types.currency_code import CurrencyCode
 
 
 class InvoiceMetricsResponse(pydantic.BaseModel):
     total_amount: float = pydantic.Field(alias="totalAmount")
     total_count: int = pydantic.Field(alias="totalCount")
     average_amount: float = pydantic.Field(alias="averageAmount")
     currency: CurrencyCode
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/profile_request.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/profile_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/tax_id.py` & `mercoa-0.2.0/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .ein import Ein
+from .itin import Itin
+from .ssn import Ssn
 
 
-class TaxID(pydantic.BaseModel):
-    ein: Ein
+class IndividualGovernmentId(pydantic.BaseModel):
+    ssn: typing.Optional[Ssn]
+    itin: typing.Optional[Itin]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity/types/trigger.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/trigger.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 
 
 class Trigger_Amount(AmountTrigger):
     type: typing_extensions.Literal["amount"]
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
 
 
 class Trigger_All(pydantic.BaseModel):
     type: typing_extensions.Literal["all"]
     value: typing.Any
 
     class Config:
         frozen = True
 
 
-Trigger = typing_extensions.Annotated[typing.Union[Trigger_Amount, Trigger_All], pydantic.Field(discriminator="type")]
+Trigger = typing.Union[Trigger_Amount, Trigger_All]
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_request.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/entity_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
+from ......core.datetime_utils import serialize_datetime
 
 
 class EntityUserRequest(pydantic.BaseModel):
     foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
     email: typing.Optional[str]
     name: typing.Optional[str]
     roles: typing.Optional[typing.List[str]] = pydantic.Field(
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/entity_user_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from .entity_user_id import EntityUserId
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.entity_user_id import EntityUserId
 
 
 class EntityUserResponse(pydantic.BaseModel):
     id: EntityUserId
     foreign_id: typing.Optional[str] = pydantic.Field(
         alias="foreignId", description=("Id from external auth provider or your auth system\n")
     )
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/client.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,480 +1,390 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import datetime as dt
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
+from ...core.datetime_utils import serialize_datetime
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
-from .types.approval_request import ApprovalRequest
-from .types.comment_id import CommentId
-from .types.comment_request import CommentRequest
-from .types.comment_response import CommentResponse
-from .types.document_response import DocumentResponse
-from .types.invoice_id import InvoiceId
+from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
+from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
+from ..commons.errors.unauthorized import Unauthorized
+from ..commons.types.entity_id import EntityId
+from ..commons.types.invoice_id import InvoiceId
+from ..commons.types.order_direction import OrderDirection
+from .resources.approval.client import ApprovalClient, AsyncApprovalClient
+from .resources.comment.client import AsyncCommentClient, CommentClient
+from .resources.document.client import AsyncDocumentClient, DocumentClient
+from .types.invoice_order_by_field import InvoiceOrderByField
 from .types.invoice_request import InvoiceRequest
 from .types.invoice_response import InvoiceResponse
+from .types.invoice_status import InvoiceStatus
 
 
 class InvoiceClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
-
-    def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
-            json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
+        self.approval = ApprovalClient(environment=self._environment, token=self._token)
+        self.comment = CommentClient(environment=self._environment, token=self._token)
+        self.document = DocumentClient(environment=self._environment, token=self._token)
+
+    def find(
+        self,
+        *,
+        entity_ids: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        start_date: typing.Optional[dt.datetime] = None,
+        end_date: typing.Optional[dt.datetime] = None,
+        order_by: typing.Optional[InvoiceOrderByField] = None,
+        order_direction: typing.Optional[OrderDirection] = None,
+        limit: typing.Optional[int] = None,
+        starting_after: typing.Optional[InvoiceId] = None,
+        search: typing.Optional[str] = None,
+        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
+    ) -> typing.List[InvoiceResponse]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
+            params={
+                "entityIds": entity_ids,
+                "startDate": serialize_datetime(start_date) if start_date is not None else None,
+                "endDate": serialize_datetime(end_date) if end_date is not None else None,
+                "orderBy": order_by,
+                "orderDirection": order_direction,
+                "limit": limit,
+                "startingAfter": starting_after,
+                "search": search,
+                "status": status,
+            },
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
+    def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, invoice_id: InvoiceId) -> None:
-        _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
-        _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> CommentResponse:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/approve"),
-            json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> CommentResponse:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/reject"),
-            json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
+    def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[CommentResponse], _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def add_comment(self, invoice_id: InvoiceId, *, request: CommentRequest) -> CommentResponse:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment"),
-            json=jsonable_encoder(request),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def edit_comment(self, invoice_id: InvoiceId, comment_id: CommentId, *, request: CommentRequest) -> CommentResponse:
+    def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete_comment(self, invoice_id: InvoiceId, comment_id: CommentId) -> None:
+    def delete(self, invoice_id: InvoiceId) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_vendor_link(self, invoice_id: InvoiceId) -> str:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def send_vendor_email(self, invoice_id: InvoiceId) -> None:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncInvoiceClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
-
-    async def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
-                json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
+        self.approval = AsyncApprovalClient(environment=self._environment, token=self._token)
+        self.comment = AsyncCommentClient(environment=self._environment, token=self._token)
+        self.document = AsyncDocumentClient(environment=self._environment, token=self._token)
+
+    async def find(
+        self,
+        *,
+        entity_ids: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        start_date: typing.Optional[dt.datetime] = None,
+        end_date: typing.Optional[dt.datetime] = None,
+        order_by: typing.Optional[InvoiceOrderByField] = None,
+        order_direction: typing.Optional[OrderDirection] = None,
+        limit: typing.Optional[int] = None,
+        starting_after: typing.Optional[InvoiceId] = None,
+        search: typing.Optional[str] = None,
+        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
+    ) -> typing.List[InvoiceResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
+                params={
+                    "entityIds": entity_ids,
+                    "startDate": serialize_datetime(start_date) if start_date is not None else None,
+                    "endDate": serialize_datetime(end_date) if end_date is not None else None,
+                    "orderBy": order_by,
+                    "orderDirection": order_direction,
+                    "limit": limit,
+                    "startingAfter": starting_after,
+                    "search": search,
+                    "status": status,
+                },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
+    async def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, invoice_id: InvoiceId) -> None:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> CommentResponse:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/approve"),
-                json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> CommentResponse:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/reject"),
-                json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
+    async def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[CommentResponse], _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def add_comment(self, invoice_id: InvoiceId, *, request: CommentRequest) -> CommentResponse:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment"),
-                json=jsonable_encoder(request),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def edit_comment(
-        self, invoice_id: InvoiceId, comment_id: CommentId, *, request: CommentRequest
-    ) -> CommentResponse:
+    async def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete_comment(self, invoice_id: InvoiceId, comment_id: CommentId) -> None:
+    async def delete(self, invoice_id: InvoiceId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_vendor_link(self, invoice_id: InvoiceId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def send_vendor_email(self, invoice_id: InvoiceId) -> None:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/__init__.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .approval_request import ApprovalRequest
-from .approver import Approver
 from .approver_action import ApproverAction
-from .approver_response import ApproverResponse
-from .comment_id import CommentId
-from .comment_request import CommentRequest
-from .comment_response import CommentResponse
-from .currency_code import CurrencyCode
-from .document_response import DocumentResponse
-from .invoice_id import InvoiceId
+from .assigned_approver import AssignedApprover
+from .associated_approval_action import AssociatedApprovalAction
+from .invoice_approver_response import InvoiceApproverResponse
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_order_by_field import InvoiceOrderByField
 from .invoice_request import InvoiceRequest
 from .invoice_response import InvoiceResponse
 from .invoice_status import InvoiceStatus
-from .set_approver import SetApprover
 
 __all__ = [
-    "ApprovalRequest",
-    "Approver",
     "ApproverAction",
-    "ApproverResponse",
-    "CommentId",
-    "CommentRequest",
-    "CommentResponse",
-    "CurrencyCode",
-    "DocumentResponse",
-    "InvoiceId",
+    "AssignedApprover",
+    "AssociatedApprovalAction",
+    "InvoiceApproverResponse",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
-    "SetApprover",
 ]
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/approval_request.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/associated_approval_action.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...entity_users.types.entity_user_id import EntityUserId
+from ...commons.types.entity_user_id import EntityUserId
+from .approver_action import ApproverAction
 
 
-class ApprovalRequest(pydantic.BaseModel):
-    text: typing.Optional[str]
+class AssociatedApprovalAction(pydantic.BaseModel):
     user_id: EntityUserId = pydantic.Field(alias="userId")
+    action: ApproverAction
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/approver.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/color_scheme_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+import pydantic
+
 from ....core.datetime_utils import serialize_datetime
-from .approver_action import ApproverAction
-from .set_approver import SetApprover
 
 
-class Approver(SetApprover):
-    roles: typing.List[str]
-    action: ApproverAction
+class ColorSchemeResponse(pydantic.BaseModel):
+    primary_color: typing.Optional[str] = pydantic.Field(alias="primaryColor")
+    secondary_color: typing.Optional[str] = pydantic.Field(alias="secondaryColor")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/approver_action.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/approver_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/approver_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...entity_users.types.entity_user_response import EntityUserResponse
-from .approver import Approver
+import pydantic
 
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.approval_policy_id import ApprovalPolicyId
+from .rule import Rule
+from .trigger import Trigger
 
-class ApproverResponse(Approver):
-    user: typing.Optional[EntityUserResponse]
+
+class ApprovalPolicyResponse(pydantic.BaseModel):
+    id: ApprovalPolicyId
+    trigger: Trigger
+    rule: Rule
+    upstream_policy_id: ApprovalPolicyId = pydantic.Field(alias="upstreamPolicyId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_request.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/types/approval_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from ...entity_users.types.entity_user_id import EntityUserId
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.entity_user_id import EntityUserId
 
 
-class CommentRequest(pydantic.BaseModel):
-    text: str
-    user_id: typing.Optional[EntityUserId] = pydantic.Field(alias="userId")
+class ApprovalRequest(pydantic.BaseModel):
+    text: typing.Optional[str] = pydantic.Field(description=("Comment associated with this approval action.\n"))
+    user_id: EntityUserId = pydantic.Field(alias="userId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_response.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/comment_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from ...entity_users.types.entity_user_response import EntityUserResponse
-from .approver import Approver
+from ......core.datetime_utils import serialize_datetime
+from .....entity.resources.user.types.entity_user_response import EntityUserResponse
+from ....types.associated_approval_action import AssociatedApprovalAction
 
 
 class CommentResponse(pydantic.BaseModel):
     id: str
     text: str
     user: typing.Optional[EntityUserResponse]
-    approval: typing.Optional[Approver]
+    associated_approval_action: typing.Optional[AssociatedApprovalAction] = pydantic.Field(
+        alias="associatedApprovalAction",
+        description=(
+            "If an approval action has triggered the generation of this comment, returns the associated approval action and actor\n"
+        ),
+    )
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/currency_code.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/document_response.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_methods_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .payment_rail_response import PaymentRailResponse
 
 
-class DocumentResponse(pydantic.BaseModel):
-    mime_type: str = pydantic.Field(alias="mimeType")
-    uri: str
-    ocr_results: typing.Any = pydantic.Field(alias="ocrResults", description=("Raw output from OCR\n"))
+class PaymentMethodsResponse(pydantic.BaseModel):
+    payer_payments: typing.List[PaymentRailResponse] = pydantic.Field(alias="payerPayments")
+    backup_disbursements: typing.List[PaymentRailResponse] = pydantic.Field(alias="backupDisbursements")
+    vendor_disbursements: typing.List[PaymentRailResponse] = pydantic.Field(alias="vendorDisbursements")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_line_item_request.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_line_item_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .currency_code import CurrencyCode
+from ...payment_method.types.currency_code import CurrencyCode
 
 
 class InvoiceLineItemRequest(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(
         description=(
             "If provided, will overwrite line item on the invoice with this ID. If not provided, will create a new line item.\n"
         )
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_line_item_response.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_line_item_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .currency_code import CurrencyCode
+from ...payment_method.types.currency_code import CurrencyCode
 
 
 class InvoiceLineItemResponse(pydantic.BaseModel):
     id: str
     amount: typing.Optional[float]
     currency: typing.Optional[CurrencyCode]
     description: typing.Optional[str]
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_order_by_field.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_order_by_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_request.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...entity.types.entity_id import EntityId
-from ...entity_users.types.entity_user_id import EntityUserId
-from ...payment_method.types.payment_method_id import PaymentMethodId
-from .currency_code import CurrencyCode
+from ...commons.types.entity_id import EntityId
+from ...commons.types.entity_user_id import EntityUserId
+from ...commons.types.invoice_id import InvoiceId
+from ...payment_method.types.currency_code import CurrencyCode
+from .assigned_approver import AssignedApprover
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_status import InvoiceStatus
-from .set_approver import SetApprover
 
 
 class InvoiceRequest(pydantic.BaseModel):
     status: typing.Optional[InvoiceStatus]
     amount: typing.Optional[float]
     currency: typing.Optional[CurrencyCode]
     invoice_date: typing.Optional[dt.datetime] = pydantic.Field(
@@ -30,20 +30,20 @@
     )
     due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate", description=("Due date of invoice.\n"))
     invoice_number: typing.Optional[str] = pydantic.Field(alias="invoiceNumber")
     note_to_self: typing.Optional[str] = pydantic.Field(alias="noteToSelf")
     service_start_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceStartDate")
     service_end_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceEndDate")
     payer_id: typing.Optional[EntityId] = pydantic.Field(alias="payerId")
-    payment_source_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentSourceId")
-    approvers: typing.Optional[typing.List[SetApprover]] = pydantic.Field(
+    payment_source_id: typing.Optional[InvoiceId] = pydantic.Field(alias="paymentSourceId")
+    approvers: typing.Optional[typing.List[AssignedApprover]] = pydantic.Field(
         description=("Set approvers for this invoice.\n")
     )
     vendor_id: typing.Optional[EntityId] = pydantic.Field(alias="vendorId")
-    payment_destination_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentDestinationId")
+    payment_destination_id: typing.Optional[InvoiceId] = pydantic.Field(alias="paymentDestinationId")
     line_items: typing.Optional[typing.List[InvoiceLineItemRequest]] = pydantic.Field(alias="lineItems")
     metadata: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
         description=(
             "Metadata associated with this invoice. You can specify up to 10 keys, with key names up to 40 characters long and values up to 200 characters long.\n"
         )
     )
     uploaded_image: typing.Optional[str] = pydantic.Field(
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_response.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...entity.types.approval_policy_response import ApprovalPolicyResponse
-from ...entity.types.entity_id import EntityId
+from ...commons.types.entity_id import EntityId
+from ...commons.types.invoice_id import InvoiceId
+from ...entity.resources.approval_policy.types.approval_policy_response import ApprovalPolicyResponse
+from ...entity.resources.user.types.entity_user_response import EntityUserResponse
 from ...entity.types.entity_response import EntityResponse
-from ...entity_users.types.entity_user_response import EntityUserResponse
-from ...payment_method.types.payment_method_id import PaymentMethodId
+from ...payment_method.types.currency_code import CurrencyCode
 from ...payment_method.types.payment_method_response import PaymentMethodResponse
 from ...transaction.types.transaction_response import TransactionResponse
-from .approver import Approver
-from .comment_response import CommentResponse
-from .currency_code import CurrencyCode
-from .invoice_id import InvoiceId
+from ..resources.comment.types.comment_response import CommentResponse
+from .invoice_approver_response import InvoiceApproverResponse
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_status import InvoiceStatus
 
 
 class InvoiceResponse(pydantic.BaseModel):
     id: InvoiceId
     status: InvoiceStatus
@@ -39,25 +38,25 @@
     invoice_number: typing.Optional[str] = pydantic.Field(alias="invoiceNumber")
     note_to_self: typing.Optional[str] = pydantic.Field(alias="noteToSelf")
     service_start_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceStartDate")
     service_end_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceEndDate")
     payer_id: typing.Optional[EntityId] = pydantic.Field(alias="payerId")
     payer: typing.Optional[EntityResponse]
     payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
-    payment_source_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentSourceId")
+    payment_source_id: typing.Optional[InvoiceId] = pydantic.Field(alias="paymentSourceId")
     vendor_id: typing.Optional[EntityId] = pydantic.Field(alias="vendorId")
     vendor: typing.Optional[EntityResponse]
     payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
-    payment_destination_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentDestinationId")
+    payment_destination_id: typing.Optional[InvoiceId] = pydantic.Field(alias="paymentDestinationId")
     payment_destination_confirmed: bool = pydantic.Field(alias="paymentDestinationConfirmed")
     has_documents: bool = pydantic.Field(alias="hasDocuments")
     comments: typing.Optional[typing.List[CommentResponse]]
     transactions: typing.Optional[typing.List[TransactionResponse]]
     line_items: typing.Optional[typing.List[InvoiceLineItemResponse]] = pydantic.Field(alias="lineItems")
-    approvers: typing.List[Approver]
+    approvers: typing.List[InvoiceApproverResponse]
     approval_policy: typing.List[ApprovalPolicyResponse] = pydantic.Field(alias="approvalPolicy")
     metadata: typing.Dict[str, str] = pydantic.Field(description=("Metadata associated with this invoice.\n"))
     created_by: typing.Optional[EntityUserResponse] = pydantic.Field(
         alias="createdBy", description=("Entity user who created this invoice.\n")
     )
     processed_at: typing.Optional[dt.datetime] = pydantic.Field(alias="processedAt")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_status.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_status.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,45 +5,45 @@
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class InvoiceStatus(str, enum.Enum):
     DRAFT = "DRAFT"
     NEW = "NEW"
+    APPROVED = "APPROVED"
+    SCHEDULED = "SCHEDULED"
     PENDING = "PENDING"
     PAID = "PAID"
-    CANCELED = "CANCELED"
-    REFUSED = "REFUSED"
-    APPROVED = "APPROVED"
     ARCHIVED = "ARCHIVED"
-    SCHEDULED = "SCHEDULED"
+    REFUSED = "REFUSED"
+    CANCELED = "CANCELED"
 
     def visit(
         self,
         draft: typing.Callable[[], T_Result],
         new: typing.Callable[[], T_Result],
+        approved: typing.Callable[[], T_Result],
+        scheduled: typing.Callable[[], T_Result],
         pending: typing.Callable[[], T_Result],
         paid: typing.Callable[[], T_Result],
-        canceled: typing.Callable[[], T_Result],
-        refused: typing.Callable[[], T_Result],
-        approved: typing.Callable[[], T_Result],
         archived: typing.Callable[[], T_Result],
-        scheduled: typing.Callable[[], T_Result],
+        refused: typing.Callable[[], T_Result],
+        canceled: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is InvoiceStatus.DRAFT:
             return draft()
         if self is InvoiceStatus.NEW:
             return new()
+        if self is InvoiceStatus.APPROVED:
+            return approved()
+        if self is InvoiceStatus.SCHEDULED:
+            return scheduled()
         if self is InvoiceStatus.PENDING:
             return pending()
         if self is InvoiceStatus.PAID:
             return paid()
-        if self is InvoiceStatus.CANCELED:
-            return canceled()
-        if self is InvoiceStatus.REFUSED:
-            return refused()
-        if self is InvoiceStatus.APPROVED:
-            return approved()
         if self is InvoiceStatus.ARCHIVED:
             return archived()
-        if self is InvoiceStatus.SCHEDULED:
-            return scheduled()
+        if self is InvoiceStatus.REFUSED:
+            return refused()
+        if self is InvoiceStatus.CANCELED:
+            return canceled()
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/invoice/types/set_approver.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/assigned_approver.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...entity_users.types.entity_user_id import EntityUserId
+from ...commons.types.entity_user_id import EntityUserId
 
 
-class SetApprover(pydantic.BaseModel):
+class AssignedApprover(pydantic.BaseModel):
     user_id: EntityUserId = pydantic.Field(alias="userId")
-    date: dt.datetime
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/ocr/client.py` & `mercoa-0.2.0/src/mercoa/resources/ocr/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,97 +7,92 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
-from ..organization.types.organization_id import OrganizationId
-from .types.ocr_response import OCRResponse
+from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
+from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
+from ..commons.errors.unauthorized import Unauthorized
+from ..commons.types.entity_id import EntityId
+from .types.ocr_response import OcrResponse
+from .types.vendor_network import VendorNetwork
 
 
 class OcrClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
-    def ocr(self, *, mime_type: str, image: str) -> OCRResponse:
+    def ocr(
+        self,
+        *,
+        vendor_network: typing.Optional[VendorNetwork] = None,
+        entity_id: typing.Optional[EntityId] = None,
+        mime_type: str,
+        image: str,
+    ) -> OcrResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "ocr"),
+            params={"vendorNetwork": vendor_network, "entityId": entity_id},
             json=jsonable_encoder({"mimeType": mime_type, "image": image}),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(OCRResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def email_inbox(self, *, org: OrganizationId, request: typing.Any) -> None:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "emailOcr"),
-            params={"org": org},
-            json=jsonable_encoder(request),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
+            return pydantic.parse_obj_as(OcrResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncOcrClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
-    async def ocr(self, *, mime_type: str, image: str) -> OCRResponse:
+    async def ocr(
+        self,
+        *,
+        vendor_network: typing.Optional[VendorNetwork] = None,
+        entity_id: typing.Optional[EntityId] = None,
+        mime_type: str,
+        image: str,
+    ) -> OcrResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "ocr"),
+                params={"vendorNetwork": vendor_network, "entityId": entity_id},
                 json=jsonable_encoder({"mimeType": mime_type, "image": image}),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(OCRResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def email_inbox(self, *, org: OrganizationId, request: typing.Any) -> None:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "emailOcr"),
-                params={"org": org},
-                json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
+            return pydantic.parse_obj_as(OcrResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/ocr/types/attachments.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/responsibilities.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
+from ......core.datetime_utils import serialize_datetime
 
 
-class Attachments(pydantic.BaseModel):
-    name: str = pydantic.Field(alias="Name")
-    content_type: str = pydantic.Field(alias="ContentType")
-    content_length: int = pydantic.Field(alias="ContentLength")
-    content_id: str = pydantic.Field(alias="ContentID")
-    download_token: str = pydantic.Field(alias="DownloadToken")
+class Responsibilities(pydantic.BaseModel):
+    job_title: typing.Optional[str] = pydantic.Field(alias="jobTitle")
+    is_controller: typing.Optional[bool] = pydantic.Field(alias="isController")
+    is_owner: typing.Optional[bool] = pydantic.Field(alias="isOwner")
+    ownership_percentage: typing.Optional[float] = pydantic.Field(alias="ownershipPercentage")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/ocr/types/email_ocr_request.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/check_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,35 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .attachments import Attachments
-from .ocr_mailbox import OcrMailbox
+from ...commons.types.payment_method_id import PaymentMethodId
+from .currency_code import CurrencyCode
 
 
-class EmailOcrRequest(pydantic.BaseModel):
-    uuid: typing.List[str] = pydantic.Field(alias="Uuid")
-    message_id: str = pydantic.Field(alias="MessageId")
-    in_reply_to: typing.Optional[str] = pydantic.Field(alias="InReplyTo")
-    from_: OcrMailbox = pydantic.Field(alias="From")
-    to: typing.List[OcrMailbox] = pydantic.Field(alias="To")
-    cc: typing.List[OcrMailbox] = pydantic.Field(alias="Cc")
-    reply_to: typing.Optional[OcrMailbox] = pydantic.Field(alias="ReplyTo")
-    sent_at_date: str = pydantic.Field(alias="SentAtDate")
-    subject: str = pydantic.Field(alias="Subject")
-    attachments: typing.List[Attachments] = pydantic.Field(alias="Attachments")
-    headers: typing.Any = pydantic.Field(alias="Headers")
-    spam_score: float = pydantic.Field(alias="SpamScore")
-    extracted_markdown_message: typing.Optional[str] = pydantic.Field(alias="ExtractedMarkdownMessage")
-    extracted_markdown_signature: typing.Optional[str] = pydantic.Field(alias="ExtractedMarkdownSignature")
-    raw_html_body: typing.Optional[str] = pydantic.Field(alias="RawHtmlBody")
-    raw_text_body: typing.Optional[str] = pydantic.Field(alias="RawTextBody")
+class CheckResponse(pydantic.BaseModel):
+    id: PaymentMethodId
+    pay_to_the_order_of: str = pydantic.Field(alias="payToTheOrderOf")
+    address_line_1: str = pydantic.Field(alias="addressLine1")
+    address_line_2: typing.Optional[str] = pydantic.Field(alias="addressLine2")
+    city: str
+    state_or_province: str = pydantic.Field(alias="stateOrProvince")
+    postal_code: str = pydantic.Field(alias="postalCode")
+    country: str
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/ocr/types/ocr_mailbox.py` & `mercoa-0.2.0/src/mercoa/resources/entity/types/tax_id.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .ein import Ein
 
 
-class OcrMailbox(pydantic.BaseModel):
-    address: str = pydantic.Field(alias="Address")
-    name: typing.Optional[str] = pydantic.Field(alias="Name")
+class TaxId(pydantic.BaseModel):
+    ein: Ein
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.2.0/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ....core.datetime_utils import serialize_datetime
 from ...entity.types.entity_response import EntityResponse
 from ...invoice.types.invoice_response import InvoiceResponse
 from ...payment_method.types.bank_account_response import BankAccountResponse
 from ...payment_method.types.check_response import CheckResponse
 
 
-class OCRResponse(pydantic.BaseModel):
+class OcrResponse(pydantic.BaseModel):
     invoice: InvoiceResponse
     vendor: EntityResponse
     check: typing.Optional[CheckResponse]
     bank_account: typing.Optional[BankAccountResponse] = pydantic.Field(alias="bankAccount")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/__init__.py` & `mercoa-0.2.0/src/mercoa/resources/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/client.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,165 +1,131 @@
 # This file was auto-generated by Fern from our API Definition.
 
-import datetime as dt
-import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
-from ...core.api_error import ApiError
-from ...core.datetime_utils import serialize_datetime
-from ...core.jsonable_encoder import jsonable_encoder
-from ...core.remove_none_from_headers import remove_none_from_headers
-from ...environment import MercoaEnvironment
-from .types.email_log_response import EmailLogResponse
-from .types.organization_request import OrganizationRequest
-from .types.organization_response import OrganizationResponse
+from .....core.api_error import ApiError
+from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_headers import remove_none_from_headers
+from .....environment import MercoaEnvironment
+from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
+from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
+from ....commons.errors.unauthorized import Unauthorized
+from ....commons.types.invoice_id import InvoiceId
+from .types.approval_request import ApprovalRequest
 
 
-class OrganizationClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+class ApprovalClient:
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
-    def get(
-        self,
-        *,
-        payment_methods: typing.Optional[bool] = None,
-        email_provider: typing.Optional[bool] = None,
-        color_scheme: typing.Optional[bool] = None,
-    ) -> OrganizationResponse:
+    def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> None:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
-            params={"paymentMethods": payment_methods, "emailProvider": email_provider, "colorScheme": color_scheme},
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/approve"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(OrganizationResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, *, request: OrganizationRequest) -> OrganizationResponse:
+    def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> None:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/reject"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(OrganizationResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def email_log(
-        self, *, start_date: typing.Optional[dt.datetime] = None, end_date: typing.Optional[dt.datetime] = None
-    ) -> typing.List[EmailLogResponse]:
-        _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "organization/emailLog"),
-            params={
-                "startDate": serialize_datetime(start_date) if start_date is not None else None,
-                "endDate": serialize_datetime(end_date) if end_date is not None else None,
-            },
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EmailLogResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncOrganizationClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+class AsyncApprovalClient:
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
-    async def get(
-        self,
-        *,
-        payment_methods: typing.Optional[bool] = None,
-        email_provider: typing.Optional[bool] = None,
-        color_scheme: typing.Optional[bool] = None,
-    ) -> OrganizationResponse:
+    async def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
-                params={
-                    "paymentMethods": payment_methods,
-                    "emailProvider": email_provider,
-                    "colorScheme": color_scheme,
-                },
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/approve"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(OrganizationResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, *, request: OrganizationRequest) -> OrganizationResponse:
+    async def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/reject"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(OrganizationResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def email_log(
-        self, *, start_date: typing.Optional[dt.datetime] = None, end_date: typing.Optional[dt.datetime] = None
-    ) -> typing.List[EmailLogResponse]:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "organization/emailLog"),
-                params={
-                    "startDate": serialize_datetime(start_date) if start_date is not None else None,
-                    "endDate": serialize_datetime(end_date) if end_date is not None else None,
-                },
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EmailLogResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/__init__.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/color_scheme_request.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/color_scheme_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_update_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.approval_policy_id import ApprovalPolicyId
+from .rule import Rule
+from .trigger import Trigger
 
 
-class ColorSchemeResponse(pydantic.BaseModel):
-    primary_color: typing.Optional[str] = pydantic.Field(alias="primaryColor")
-    secondary_color: typing.Optional[str] = pydantic.Field(alias="secondaryColor")
+class ApprovalPolicyUpdateRequest(pydantic.BaseModel):
+    trigger: typing.Optional[Trigger]
+    rule: typing.Optional[Rule]
+    upstream_policy_id: typing.Optional[ApprovalPolicyId] = pydantic.Field(alias="upstreamPolicyId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/email_provider_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email_sender_request import EmailSenderRequest
+from .email_sender_response import EmailSenderResponse
 
 
-class EmailProviderRequest(pydantic.BaseModel):
-    sender: EmailSenderRequest
+class EmailProviderResponse(pydantic.BaseModel):
+    sender: EmailSenderResponse
     inbox_domain: str = pydantic.Field(alias="inboxDomain")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ....core.datetime_utils import serialize_datetime
-from .email_sender_response import EmailSenderResponse
+from .payment_rail_request import PaymentRailRequest
 
 
-class EmailProviderResponse(pydantic.BaseModel):
-    sender: EmailSenderResponse
-    inbox_domain: str = pydantic.Field(alias="inboxDomain")
+class PaymentRailResponse(PaymentRailRequest):
+    available: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_provider.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class EmailSenderProvider(str, enum.Enum):
     NONE = "none"
     SENDGRID = "sendgrid"
+    SES = "ses"
     RESEND = "resend"
 
     def visit(
         self,
         none: typing.Callable[[], T_Result],
         sendgrid: typing.Callable[[], T_Result],
+        ses: typing.Callable[[], T_Result],
         resend: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is EmailSenderProvider.NONE:
             return none()
         if self is EmailSenderProvider.SENDGRID:
             return sendgrid()
+        if self is EmailSenderProvider.SES:
+            return ses()
         if self is EmailSenderProvider.RESEND:
             return resend()
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/organization_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/organization_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,21 +2,34 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .payment_rail_response import PaymentRailResponse
-
-
-class PaymentMethodsResponse(pydantic.BaseModel):
-    payer_payments: typing.List[PaymentRailResponse] = pydantic.Field(alias="payerPayments")
-    backup_disbursements: typing.List[PaymentRailResponse] = pydantic.Field(alias="backupDisbursements")
-    vendor_disbursements: typing.List[PaymentRailResponse] = pydantic.Field(alias="vendorDisbursements")
+from ...commons.types.payment_method_schema_id import PaymentMethodSchemaId
+from ...payment_method.types.currency_code import CurrencyCode
+from .payment_method_schema_field import PaymentMethodSchemaField
+
+
+class PaymentMethodSchemaResponse(pydantic.BaseModel):
+    id: PaymentMethodSchemaId
+    name: str
+    is_source: bool = pydantic.Field(
+        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
+    )
+    is_destination: bool = pydantic.Field(
+        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
+    )
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(
+        alias="supportedCurrencies", description=("List of currencies that this payment method supports.\n")
+    )
+    fields: typing.List[PaymentMethodSchemaField]
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/client.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,308 +7,223 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
-from ..entity.types.entity_id import EntityId
-from .types.payment_method_id import PaymentMethodId
-from .types.payment_method_request import PaymentMethodRequest
-from .types.payment_method_response import PaymentMethodResponse
-from .types.payment_method_type import PaymentMethodType
-from .types.payment_method_update_request import PaymentMethodUpdateRequest
+from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
+from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
+from ..commons.errors.unauthorized import Unauthorized
+from ..commons.types.payment_method_schema_id import PaymentMethodSchemaId
+from .types.payment_method_schema_request import PaymentMethodSchemaRequest
+from .types.payment_method_schema_response import PaymentMethodSchemaResponse
 
 
-class PaymentMethodClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+class PaymentMethodSchemaClient:
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
-    def get_all(
-        self,
-        entity_id: EntityId,
-        *,
-        type: typing.Union[typing.Optional[PaymentMethodType], typing.List[PaymentMethodType]],
-    ) -> typing.List[PaymentMethodResponse]:
+    def get_all(self) -> typing.List[PaymentMethodSchemaResponse]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/paymentMethods"),
-            params={"type": type},
+            urllib.parse.urljoin(f"{self._environment.value}/", "paymentMethod/schema"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[PaymentMethodResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[PaymentMethodSchemaResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(self, entity_id: EntityId, *, request: PaymentMethodRequest) -> PaymentMethodResponse:
+    def create(self, *, request: PaymentMethodSchemaRequest) -> PaymentMethodSchemaResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "paymentMethod/schema"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(PaymentMethodSchemaResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, entity_id: EntityId, payment_method_id: PaymentMethodId) -> PaymentMethodResponse:
+    def get(self, schema_id: PaymentMethodSchemaId) -> PaymentMethodSchemaResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(
-                f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}"
-            ),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def update(
-        self, entity_id: EntityId, payment_method_id: PaymentMethodId, *, request: PaymentMethodUpdateRequest
-    ) -> PaymentMethodResponse:
-        _response = httpx.request(
-            "PUT",
-            urllib.parse.urljoin(
-                f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}"
-            ),
-            json=jsonable_encoder(request),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"paymentMethod/schema/{schema_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(PaymentMethodSchemaResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, entity_id: EntityId, payment_method_id: PaymentMethodId) -> None:
+    def delete(self, schema_id: PaymentMethodSchemaId) -> None:
         _response = httpx.request(
             "DELETE",
-            urllib.parse.urljoin(
-                f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}"
-            ),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"paymentMethod/schema/{schema_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def initiate_micro_deposits(self, entity_id: EntityId, payment_method_id: PaymentMethodId) -> None:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}/micro-deposits"
-            ),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def complete_micro_deposits(
-        self, entity_id: EntityId, payment_method_id: PaymentMethodId, *, amounts: typing.List[int]
-    ) -> None:
-        _response = httpx.request(
-            "PUT",
-            urllib.parse.urljoin(
-                f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}/micro-deposits"
-            ),
-            json=jsonable_encoder({"amounts": amounts}),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-
-class AsyncPaymentMethodClient:
-    def __init__(
-        self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
-    ):
+class AsyncPaymentMethodSchemaClient:
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
-    async def get_all(
-        self,
-        entity_id: EntityId,
-        *,
-        type: typing.Union[typing.Optional[PaymentMethodType], typing.List[PaymentMethodType]],
-    ) -> typing.List[PaymentMethodResponse]:
+    async def get_all(self) -> typing.List[PaymentMethodSchemaResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/paymentMethods"),
-                params={"type": type},
+                urllib.parse.urljoin(f"{self._environment.value}/", "paymentMethod/schema"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[PaymentMethodResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[PaymentMethodSchemaResponse], _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(self, entity_id: EntityId, *, request: PaymentMethodRequest) -> PaymentMethodResponse:
+    async def create(self, *, request: PaymentMethodSchemaRequest) -> PaymentMethodSchemaResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "paymentMethod/schema"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(PaymentMethodSchemaResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, entity_id: EntityId, payment_method_id: PaymentMethodId) -> PaymentMethodResponse:
+    async def get(self, schema_id: PaymentMethodSchemaId) -> PaymentMethodSchemaResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(
-                    f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}"
-                ),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"paymentMethod/schema/{schema_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(PaymentMethodSchemaResponse, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(
-        self, entity_id: EntityId, payment_method_id: PaymentMethodId, *, request: PaymentMethodUpdateRequest
-    ) -> PaymentMethodResponse:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "PUT",
-                urllib.parse.urljoin(
-                    f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}"
-                ),
-                json=jsonable_encoder(request),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def delete(self, entity_id: EntityId, payment_method_id: PaymentMethodId) -> None:
+    async def delete(self, schema_id: PaymentMethodSchemaId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
-                urllib.parse.urljoin(
-                    f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}"
-                ),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def initiate_micro_deposits(self, entity_id: EntityId, payment_method_id: PaymentMethodId) -> None:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(
-                    f"{self._environment.value}/",
-                    f"entity/{entity_id}/paymentMethod/{payment_method_id}/micro-deposits",
-                ),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-            )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def complete_micro_deposits(
-        self, entity_id: EntityId, payment_method_id: PaymentMethodId, *, amounts: typing.List[int]
-    ) -> None:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "PUT",
-                urllib.parse.urljoin(
-                    f"{self._environment.value}/",
-                    f"entity/{entity_id}/paymentMethod/{payment_method_id}/micro-deposits",
-                ),
-                json=jsonable_encoder({"amounts": amounts}),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"paymentMethod/schema/{schema_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/__init__.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,62 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .bank_account_id import BankAccountId
 from .bank_account_request import BankAccountRequest
 from .bank_account_response import BankAccountResponse
 from .bank_status import BankStatus
 from .bank_type import BankType
 from .card_brand import CardBrand
-from .card_id import CardId
 from .card_request import CardRequest
 from .card_response import CardResponse
 from .card_type import CardType
-from .check_id import CheckId
 from .check_request import CheckRequest
 from .check_response import CheckResponse
-from .custom_id import CustomId
+from .currency_code import CurrencyCode
 from .custom_payment_method_request import CustomPaymentMethodRequest
 from .custom_payment_method_response import CustomPaymentMethodResponse
 from .custom_payment_method_update_request import CustomPaymentMethodUpdateRequest
-from .payment_method_id import PaymentMethodId
-from .payment_method_request import PaymentMethodRequest
-from .payment_method_response import PaymentMethodResponse
+from .payment_method_request import (
+    PaymentMethodRequest,
+    PaymentMethodRequest_BankAccount,
+    PaymentMethodRequest_Card,
+    PaymentMethodRequest_Check,
+    PaymentMethodRequest_Custom,
+)
+from .payment_method_response import (
+    PaymentMethodResponse,
+    PaymentMethodResponse_BankAccount,
+    PaymentMethodResponse_Card,
+    PaymentMethodResponse_Check,
+    PaymentMethodResponse_Custom,
+)
 from .payment_method_type import PaymentMethodType
-from .payment_method_update_request import PaymentMethodUpdateRequest
+from .payment_method_update_request import PaymentMethodUpdateRequest, PaymentMethodUpdateRequest_Custom
 
 __all__ = [
-    "BankAccountId",
     "BankAccountRequest",
     "BankAccountResponse",
     "BankStatus",
     "BankType",
     "CardBrand",
-    "CardId",
     "CardRequest",
     "CardResponse",
     "CardType",
-    "CheckId",
     "CheckRequest",
     "CheckResponse",
-    "CustomId",
+    "CurrencyCode",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
     "CustomPaymentMethodUpdateRequest",
-    "PaymentMethodId",
     "PaymentMethodRequest",
+    "PaymentMethodRequest_BankAccount",
+    "PaymentMethodRequest_Card",
+    "PaymentMethodRequest_Check",
+    "PaymentMethodRequest_Custom",
     "PaymentMethodResponse",
+    "PaymentMethodResponse_BankAccount",
+    "PaymentMethodResponse_Card",
+    "PaymentMethodResponse_Check",
+    "PaymentMethodResponse_Custom",
     "PaymentMethodType",
     "PaymentMethodUpdateRequest",
+    "PaymentMethodUpdateRequest_Custom",
 ]
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_request.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_account_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .bank_account_id import BankAccountId
 from .bank_type import BankType
 
 
 class BankAccountRequest(pydantic.BaseModel):
-    id: typing.Optional[BankAccountId]
     bank_name: str = pydantic.Field(alias="bankName")
     routing_number: str = pydantic.Field(alias="routingNumber")
     account_number: str = pydantic.Field(alias="accountNumber")
     plaid_public_token: typing.Optional[str] = pydantic.Field(
         alias="plaidPublicToken", description=("Public token from Plaid Link\n")
     )
     account_type: BankType = pydantic.Field(alias="accountType")
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_response.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_account_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .bank_account_id import BankAccountId
+from ...commons.types.payment_method_id import PaymentMethodId
 from .bank_status import BankStatus
 from .bank_type import BankType
+from .currency_code import CurrencyCode
 
 
 class BankAccountResponse(pydantic.BaseModel):
-    id: BankAccountId
+    id: PaymentMethodId
     bank_name: str = pydantic.Field(alias="bankName")
     routing_number: str = pydantic.Field(alias="routingNumber")
     account_number: str = pydantic.Field(alias="accountNumber")
     account_type: BankType = pydantic.Field(alias="accountType")
     status: BankStatus
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_status.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_type.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_brand.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_request.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .card_brand import CardBrand
-from .card_id import CardId
 from .card_type import CardType
 
 
 class CardRequest(pydantic.BaseModel):
-    id: typing.Optional[CardId]
-    type: CardType
-    brand: CardBrand
+    card_type: CardType = pydantic.Field(alias="cardType")
+    card_brand: CardBrand = pydantic.Field(alias="cardBrand")
     last_four: str = pydantic.Field(alias="lastFour")
     exp_month: str = pydantic.Field(alias="expMonth")
     exp_year: str = pydantic.Field(alias="expYear")
     token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_response.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/check_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .card_brand import CardBrand
-from .card_id import CardId
-from .card_type import CardType
 
 
-class CardResponse(pydantic.BaseModel):
-    id: CardId
-    type: CardType
-    brand: CardBrand
-    last_four: str = pydantic.Field(alias="lastFour")
-    exp_month: str = pydantic.Field(alias="expMonth")
-    exp_year: str = pydantic.Field(alias="expYear")
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+class CheckRequest(pydantic.BaseModel):
+    pay_to_the_order_of: str = pydantic.Field(alias="payToTheOrderOf")
+    address_line_1: str = pydantic.Field(alias="addressLine1")
+    address_line_2: typing.Optional[str] = pydantic.Field(alias="addressLine2")
+    city: str
+    state_or_province: str = pydantic.Field(alias="stateOrProvince")
+    postal_code: str = pydantic.Field(alias="postalCode")
+    country: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_type.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_request.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,24 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...commons.types.payment_method_schema_id import PaymentMethodSchemaId
 
 
-class CheckRequest(pydantic.BaseModel):
-    pay_to_the_order_of: str = pydantic.Field(alias="payToTheOrderOf")
-    address_line_1: str = pydantic.Field(alias="addressLine1")
-    address_line_2: typing.Optional[str] = pydantic.Field(alias="addressLine2")
-    city: str
-    state_or_province: str = pydantic.Field(alias="stateOrProvince")
-    postal_code: str = pydantic.Field(alias="postalCode")
-    country: str
+class CustomPaymentMethodUpdateRequest(pydantic.BaseModel):
+    foreign_id: typing.Optional[str] = pydantic.Field(
+        alias="foreignId", description=("ID for this payment method in your system\n")
+    )
+    account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
+    account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
+    schema_id: typing.Optional[PaymentMethodSchemaId] = pydantic.Field(
+        alias="schemaId",
+        description=(
+            "Payment method schema used for this payment method. Defines the fields that this payment method contains.\n"
+        ),
+    )
+    data: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
+        description=("Object of key/value pairs that matches the keys in the linked payment method schema.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_response.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from .check_id import CheckId
-
-
-class CheckResponse(pydantic.BaseModel):
-    id: CheckId
-    pay_to_the_order_of: str = pydantic.Field(alias="payToTheOrderOf")
-    address_line_1: str = pydantic.Field(alias="addressLine1")
-    address_line_2: typing.Optional[str] = pydantic.Field(alias="addressLine2")
-    city: str
-    state_or_province: str = pydantic.Field(alias="stateOrProvince")
-    postal_code: str = pydantic.Field(alias="postalCode")
-    country: str
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.address import Address
+from .....commons.types.full_name import FullName
+from .....commons.types.phone_number import PhoneNumber
+from .representative_id import RepresentativeId
+from .responsibilities import Responsibilities
+
+
+class RepresentativeResponse(pydantic.BaseModel):
+    id: RepresentativeId
+    name: FullName
+    phone: PhoneNumber
+    email: str
+    address: Address
+    birth_date_provided: bool = pydantic.Field(alias="birthDateProvided")
+    government_id_provided: bool = pydantic.Field(alias="governmentIDProvided")
+    responsibilities: Responsibilities
+    created_on: dt.datetime = pydantic.Field(alias="createdOn")
+    updated_on: dt.datetime = pydantic.Field(alias="updatedOn")
+    disabled_on: typing.Optional[dt.datetime] = pydantic.Field(alias="disabledOn")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_request.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...payment_method_schema.types.payment_method_schema_id import PaymentMethodSchemaId
+from ...commons.types.payment_method_schema_id import PaymentMethodSchemaId
 
 
 class CustomPaymentMethodRequest(pydantic.BaseModel):
     foreign_id: str = pydantic.Field(alias="foreignId", description=("ID for this payment method in your system\n"))
     account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
     account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
     schema_id: PaymentMethodSchemaId = pydantic.Field(
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_response.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...payment_method_schema.types.payment_method_schema_id import PaymentMethodSchemaId
+from ...commons.types.payment_method_id import PaymentMethodId
+from ...commons.types.payment_method_schema_id import PaymentMethodSchemaId
 from ...payment_method_schema.types.payment_method_schema_response import PaymentMethodSchemaResponse
-from .custom_id import CustomId
+from .currency_code import CurrencyCode
 
 
 class CustomPaymentMethodResponse(pydantic.BaseModel):
-    id: CustomId
+    id: PaymentMethodId
     foreign_id: str = pydantic.Field(alias="foreignId", description=("ID for this payment method in your system\n"))
     account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
     account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
     schema_id: PaymentMethodSchemaId = pydantic.Field(
         alias="schemaId",
         description=(
             "Payment method schema used for this payment method. Defines the fields that this payment method contains.\n"
         ),
     )
     schema_: PaymentMethodSchemaResponse = pydantic.Field(alias="schema")
     data: typing.Dict[str, str] = pydantic.Field(
         description=("Object of key/value pairs that matches the keys in the linked payment method schema.\n")
     )
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...payment_method_schema.types.payment_method_schema_id import PaymentMethodSchemaId
+from .payment_method_schema_field_type import PaymentMethodSchemaFieldType
 
 
-class CustomPaymentMethodUpdateRequest(pydantic.BaseModel):
-    foreign_id: typing.Optional[str] = pydantic.Field(
-        alias="foreignId", description=("ID for this payment method in your system\n")
+class PaymentMethodSchemaField(pydantic.BaseModel):
+    name: str
+    display_name: typing.Optional[str] = pydantic.Field(alias="displayName")
+    type: PaymentMethodSchemaFieldType
+    optional: bool = pydantic.Field(description=("Indicates whether this field is optional\n"))
+    use_as_account_name: typing.Optional[bool] = pydantic.Field(
+        alias="useAsAccountName",
+        description=(
+            "Indicates whether this field should be used as the name of the payment method. Only one field can be used as the name. Will set the accountName field of the payment method to the value of this field.\n"
+        ),
     )
-    account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
-    account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
-    schema_id: typing.Optional[PaymentMethodSchemaId] = pydantic.Field(
-        alias="schemaId",
+    use_as_account_number: typing.Optional[bool] = pydantic.Field(
+        alias="useAsAccountNumber",
         description=(
-            "Payment method schema used for this payment method. Defines the fields that this payment method contains.\n"
+            "Indicates whether this field should be used as the account number of the payment method. Only one field can be used as the account number. Will set the accountNumber field of the payment method to the value of this field.\n"
         ),
     )
-    data: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
-        description=("Object of key/value pairs that matches the keys in the linked payment method schema.\n")
+    options: typing.Optional[typing.List[str]] = pydantic.Field(
+        description=("When type is 'select', provide options that can be selected\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_request.py` & `mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_response_expanded.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .bank_account_request import BankAccountRequest
-from .card_request import CardRequest
-from .check_request import CheckRequest
-from .custom_payment_method_request import CustomPaymentMethodRequest
-from .payment_method_type import PaymentMethodType
+from ...commons.types.invoice_id import InvoiceId
+from ...entity.types.entity_response import EntityResponse
+from ...payment_method.types.payment_method_response import PaymentMethodResponse
+from .transaction_response import TransactionResponse
 
 
-class PaymentMethodRequest(pydantic.BaseModel):
-    type: PaymentMethodType
-    bank_account: typing.Optional[BankAccountRequest] = pydantic.Field(alias="bankAccount")
-    check: typing.Optional[CheckRequest]
-    card: typing.Optional[CardRequest]
-    custom: typing.Optional[CustomPaymentMethodRequest]
+class TransactionResponseExpanded(TransactionResponse):
+    invoice_id: InvoiceId = pydantic.Field(alias="invoiceId")
+    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
+    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
+    payer: typing.Optional[EntityResponse]
+    vendor: typing.Optional[EntityResponse]
+    payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
+    payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_response.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...invoice.types.currency_code import CurrencyCode
-from .bank_account_response import BankAccountResponse
-from .card_response import CardResponse
-from .check_response import CheckResponse
-from .custom_payment_method_response import CustomPaymentMethodResponse
-from .payment_method_id import PaymentMethodId
-from .payment_method_type import PaymentMethodType
+from ...commons.types.payment_method_id import PaymentMethodId
+from .card_brand import CardBrand
+from .card_type import CardType
+from .currency_code import CurrencyCode
 
 
-class PaymentMethodResponse(pydantic.BaseModel):
+class CardResponse(pydantic.BaseModel):
     id: PaymentMethodId
-    type: PaymentMethodType
-    bank_account: typing.Optional[BankAccountResponse] = pydantic.Field(alias="bankAccount")
-    check: typing.Optional[CheckResponse]
-    card: typing.Optional[CardResponse]
-    custom: typing.Optional[CustomPaymentMethodResponse]
+    card_type: CardType = pydantic.Field(alias="cardType")
+    card_brand: CardBrand = pydantic.Field(alias="cardBrand")
+    last_four: str = pydantic.Field(alias="lastFour")
+    exp_month: str = pydantic.Field(alias="expMonth")
+    exp_year: str = pydantic.Field(alias="expYear")
     supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_type.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py` & `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...invoice.types.currency_code import CurrencyCode
+from ...payment_method.types.currency_code import CurrencyCode
 from .payment_method_schema_field import PaymentMethodSchemaField
 
 
 class PaymentMethodSchemaRequest(pydantic.BaseModel):
     name: str
     is_source: bool = pydantic.Field(
         alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/representative/types/representative_request.py` & `mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.address import Address
-from ...commons.types.birth_date import BirthDate
-from ...commons.types.full_name import FullName
-from ...commons.types.individual_government_id import IndividualGovernmentID
-from ...commons.types.phone_number import PhoneNumber
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.address import Address
+from .....commons.types.birth_date import BirthDate
+from .....commons.types.full_name import FullName
+from .....commons.types.individual_government_id import IndividualGovernmentId
+from .....commons.types.phone_number import PhoneNumber
 from .responsibilities import Responsibilities
 
 
 class RepresentativeRequest(pydantic.BaseModel):
     name: FullName
     phone: PhoneNumber
     email: str
     address: Address
     birth_date: BirthDate = pydantic.Field(alias="birthDate")
-    government_id: IndividualGovernmentID = pydantic.Field(alias="governmentID")
+    government_id: IndividualGovernmentId = pydantic.Field(alias="governmentID")
     responsibilities: Responsibilities
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/representative/types/representative_response.py` & `mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,33 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.address import Address
-from ...commons.types.full_name import FullName
-from ...commons.types.phone_number import PhoneNumber
-from .representative_id import RepresentativeId
-from .responsibilities import Responsibilities
-
-
-class RepresentativeResponse(pydantic.BaseModel):
-    id: RepresentativeId
-    name: FullName
-    phone: PhoneNumber
-    email: str
-    address: Address
-    birth_date_provided: bool = pydantic.Field(alias="birthDateProvided")
-    government_id_provided: bool = pydantic.Field(alias="governmentIDProvided")
-    responsibilities: Responsibilities
-    created_on: dt.datetime = pydantic.Field(alias="createdOn")
-    updated_on: dt.datetime = pydantic.Field(alias="updatedOn")
-    disabled_on: typing.Optional[dt.datetime] = pydantic.Field(alias="disabledOn")
+from ...payment_method.types.currency_code import CurrencyCode
+from .transaction_status import TransactionStatus
+
+
+class TransactionResponse(pydantic.BaseModel):
+    id: str
+    status: TransactionStatus
+    amount: float
+    currency: typing.Optional[CurrencyCode]
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/representative/types/responsibilities.py` & `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_approver_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...commons.types.entity_user_id import EntityUserId
+from .approver_action import ApproverAction
 
 
-class Responsibilities(pydantic.BaseModel):
-    job_title: typing.Optional[str] = pydantic.Field(alias="jobTitle")
-    is_controller: typing.Optional[bool] = pydantic.Field(alias="isController")
-    is_owner: typing.Optional[bool] = pydantic.Field(alias="isOwner")
-    ownership_percentage: typing.Optional[float] = pydantic.Field(alias="ownershipPercentage")
+class InvoiceApproverResponse(pydantic.BaseModel):
+    assigned_user_id: typing.Optional[EntityUserId] = pydantic.Field(alias="assignedUserId")
+    action: ApproverAction
+    eligible_roles: typing.List[str] = pydantic.Field(alias="eligibleRoles")
+    eligible_user_ids: typing.List[EntityUserId] = pydantic.Field(alias="eligibleUserIds")
+    date: dt.datetime = pydantic.Field(
+        description=(
+            "Either the date the invoice was created, date the approver was assigned, or date of last action by approver, whichever is latest.\n"
+        )
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_status.py` & `mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

