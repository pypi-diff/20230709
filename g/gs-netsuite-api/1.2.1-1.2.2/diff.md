# Comparing `tmp/gs-netsuite-api-1.2.1.tar.gz` & `tmp/gs-netsuite-api-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs-netsuite-api-1.2.1.tar", last modified: Sun Jul  2 18:47:24 2023, max compression
+gzip compressed data, was "gs-netsuite-api-1.2.2.tar", last modified: Sun Jul  9 07:26:42 2023, max compression
```

## Comparing `gs-netsuite-api-1.2.1.tar` & `gs-netsuite-api-1.2.2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.956724 gs-netsuite-api-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1910 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-02 17:00:02.000000 gs-netsuite-api-1.2.1/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.940724 gs-netsuite-api-1.2.1/.idea/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/.idea/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/.idea/GitlabLint.xml
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/.idea/misc.xml
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/.idea/vcs.xml
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/.local-antora-playbook.yml
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/.ruff
--rw-r--r--   0 root         (0) root         (0)      186 2023-07-02 18:47:24.956724 gs-netsuite-api-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/README.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.940724 gs-netsuite-api-1.2.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/docs/antora.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/docs/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.940724 gs-netsuite-api-1.2.1/docs/modules/ROOT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/docs/modules/ROOT/examples/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/docs/modules/ROOT/nav.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.940724 gs-netsuite-api-1.2.1/docs/modules/ROOT/pages/
--rw-rw-rw-   0 root         (0) root         (0)     3361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/docs/modules/ROOT/pages/api.adoc
--rw-rw-rw-   0 root         (0) root         (0)     2353 2023-07-02 15:12:18.000000 gs-netsuite-api-1.2.1/docs/modules/ROOT/pages/convertion.adoc
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/docs/modules/ROOT/pages/index.adoc
--rw-rw-rw-   0 root         (0) root         (0)     2206 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/docs/modules/ROOT/pages/types.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.940724 gs-netsuite-api-1.2.1/example/
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-07-02 17:04:11.000000 gs-netsuite-api-1.2.1/example/sample_customer_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.1/example/sample_item_fulfillment_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.1/example/sample_item_receipt_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.1/example/sample_product_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1819 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.1/example/sample_purchase_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.1/example/sample_sale_api.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-02 17:04:11.000000 gs-netsuite-api-1.2.1/example/sample_vendor_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 14:42:03.000000 gs-netsuite-api-1.2.1/netsuite-api.iml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/output/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/output/wsdl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.940724 gs-netsuite-api-1.2.1/output/wsdl/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   133803 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/wsdl/v2022_2_0/netsuite.wsdl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/output/xsd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/output/xsd/activities/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.940724 gs-netsuite-api-1.2.1/output/xsd/activities/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    38231 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/activities/v2022_2_0/scheduling.xsd
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/activities/v2022_2_0/schedulingTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/output/xsd/documents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.944724 gs-netsuite-api-1.2.1/output/xsd/documents/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)     8963 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/documents/v2022_2_0/fileCabinet.xsd
--rw-rw-rw-   0 root         (0) root         (0)     4282 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/output/xsd/general/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.944724 gs-netsuite-api-1.2.1/output/xsd/general/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    14530 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/general/v2022_2_0/communication.xsd
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/general/v2022_2_0/communicationTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/output/xsd/lists/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.948724 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   424972 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/accounting.xsd
--rw-rw-rw-   0 root         (0) root         (0)    40848 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/accountingTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    11949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/employeeTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    31010 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/employees.xsd
--rw-rw-rw-   0 root         (0) root         (0)    27949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/marketing.xsd
--rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/marketingTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     7100 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/relationshipTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)   102099 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/relationships.xsd
--rw-rw-rw-   0 root         (0) root         (0)    16989 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/supplyChain.xsd
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    29653 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/support.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2906 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/supportTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/website.xsd
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/websiteTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/output/xsd/platform/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.948724 gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   744517 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/common.xsd
--rw-rw-rw-   0 root         (0) root         (0)    59244 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/commonTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    47859 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/core.xsd
--rw-rw-rw-   0 root         (0) root         (0)    37883 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/coreTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    72361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/faultTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     3764 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/faults.xsd
--rw-rw-rw-   0 root         (0) root         (0)    28339 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/messages.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.932724 gs-netsuite-api-1.2.1/output/xsd/setup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.948724 gs-netsuite-api-1.2.1/output/xsd/setup/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   102180 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/setup/v2022_2_0/customization.xsd
--rw-rw-rw-   0 root         (0) root         (0)     4880 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/setup/v2022_2_0/customizationTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.936724 gs-netsuite-api-1.2.1/output/xsd/transactions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.952724 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    13345 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/bank.xsd
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/bankTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/customerTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    75538 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/customers.xsd
--rw-rw-rw-   0 root         (0) root         (0)    10022 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/demandPlanning.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2094 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/employeeTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    43650 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/employees.xsd
--rw-rw-rw-   0 root         (0) root         (0)     5844 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/financial.xsd
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/financialTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    23444 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/general.xsd
--rw-rw-rw-   0 root         (0) root         (0)    49374 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/inventory.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     1983 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    64002 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/purchases.xsd
--rw-rw-rw-   0 root         (0) root         (0)    32740 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/saleTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)   141383 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/sales.xsd
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-06-22 14:42:03.000000 gs-netsuite-api-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 18:47:24.956724 gs-netsuite-api-1.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.936724 gs-netsuite-api-1.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.956724 gs-netsuite-api-1.2.1/src/gs_netsuite_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-07-02 18:47:24.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    27778 2023-07-02 18:38:33.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api/api.py.adoc
--rw-rw-rw-   0 root         (0) root         (0)     4680 2023-07-02 18:38:33.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)     3856 2023-07-02 15:24:56.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api/ns_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:47:24.956724 gs-netsuite-api-1.2.1/src/gs_netsuite_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2023-07-02 18:47:24.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3295 2023-07-02 18:47:24.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:47:24.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-02 18:47:24.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-02 18:47:24.000000 gs-netsuite-api-1.2.1/src/gs_netsuite_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3864 2023-07-02 15:28:33.000000 gs-netsuite-api-1.2.1/wsdldownloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.627856 gs-netsuite-api-1.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-02 19:22:44.000000 gs-netsuite-api-1.2.2/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/.idea/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/.idea/GitlabLint.xml
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/.idea/vcs.xml
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/.local-antora-playbook.yml
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/.ruff
+-rw-r--r--   0 root         (0) root         (0)      186 2023-07-09 07:26:42.627856 gs-netsuite-api-1.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/README.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/docs/antora.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.611856 gs-netsuite-api-1.2.2/docs/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/docs/modules/ROOT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.611856 gs-netsuite-api-1.2.2/docs/modules/ROOT/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/docs/modules/ROOT/nav.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/docs/modules/ROOT/pages/
+-rw-rw-rw-   0 root         (0) root         (0)     3361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/docs/modules/ROOT/pages/api.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2353 2023-07-02 15:12:18.000000 gs-netsuite-api-1.2.2/docs/modules/ROOT/pages/convertion.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/docs/modules/ROOT/pages/index.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2206 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/docs/modules/ROOT/pages/types.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/example/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-07-02 17:04:11.000000 gs-netsuite-api-1.2.2/example/sample_customer_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.2/example/sample_item_fulfillment_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.2/example/sample_item_receipt_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.2/example/sample_product_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.2/example/sample_purchase_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.2/example/sample_sale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-02 17:04:11.000000 gs-netsuite-api-1.2.2/example/sample_vendor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 14:42:03.000000 gs-netsuite-api-1.2.2/netsuite-api.iml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.611856 gs-netsuite-api-1.2.2/output/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.611856 gs-netsuite-api-1.2.2/output/wsdl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/output/wsdl/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   133803 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/wsdl/v2022_2_0/netsuite.wsdl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/output/xsd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/output/xsd/activities/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.619856 gs-netsuite-api-1.2.2/output/xsd/activities/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    38231 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/activities/v2022_2_0/scheduling.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/activities/v2022_2_0/schedulingTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/output/xsd/documents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.619856 gs-netsuite-api-1.2.2/output/xsd/documents/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)     8963 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/documents/v2022_2_0/fileCabinet.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     4282 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/output/xsd/general/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.619856 gs-netsuite-api-1.2.2/output/xsd/general/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    14530 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/general/v2022_2_0/communication.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/general/v2022_2_0/communicationTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/output/xsd/lists/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.619856 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   424972 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/accounting.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    40848 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/accountingTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/employeeTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    31010 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/employees.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    27949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/marketing.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/marketingTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     7100 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/relationshipTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)   102099 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/relationships.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    16989 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/supplyChain.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    29653 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/support.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2906 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/supportTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/website.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/websiteTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/output/xsd/platform/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.623856 gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   744517 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/common.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    59244 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/commonTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    47859 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/core.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    37883 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/coreTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    72361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/faultTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     3764 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/faults.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    28339 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/messages.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/output/xsd/setup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.623856 gs-netsuite-api-1.2.2/output/xsd/setup/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   102180 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/setup/v2022_2_0/customization.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     4880 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/setup/v2022_2_0/customizationTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/output/xsd/transactions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.623856 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    13345 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/bank.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/bankTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/customerTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    75538 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/customers.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    10022 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/demandPlanning.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/employeeTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    43650 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/employees.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     5844 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/financial.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/financialTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    23444 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/general.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    49374 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/inventory.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    64002 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/purchases.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    32740 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/saleTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)   141383 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/sales.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-02 19:22:44.000000 gs-netsuite-api-1.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 07:26:42.627856 gs-netsuite-api-1.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.615856 gs-netsuite-api-1.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.623856 gs-netsuite-api-1.2.2/src/gs_netsuite_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-09 07:26:42.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    27737 2023-07-02 21:28:21.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api/api.py.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     4680 2023-07-02 18:38:33.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3856 2023-07-02 15:24:56.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api/ns_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 07:26:42.627856 gs-netsuite-api-1.2.2/src/gs_netsuite_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-07-09 07:26:42.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3295 2023-07-09 07:26:42.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 07:26:42.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-09 07:26:42.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-09 07:26:42.000000 gs-netsuite-api-1.2.2/src/gs_netsuite_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3864 2023-07-02 15:28:33.000000 gs-netsuite-api-1.2.2/wsdldownloader.py
```

### Comparing `gs-netsuite-api-1.2.1/.gitignore` & `gs-netsuite-api-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/.pre-commit-config.yaml` & `gs-netsuite-api-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/README.adoc` & `gs-netsuite-api-1.2.2/README.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/docs/modules/ROOT/pages/api.adoc` & `gs-netsuite-api-1.2.2/docs/modules/ROOT/pages/api.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/docs/modules/ROOT/pages/convertion.adoc` & `gs-netsuite-api-1.2.2/docs/modules/ROOT/pages/convertion.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/docs/modules/ROOT/pages/index.adoc` & `gs-netsuite-api-1.2.2/docs/modules/ROOT/pages/index.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/docs/modules/ROOT/pages/types.adoc` & `gs-netsuite-api-1.2.2/docs/modules/ROOT/pages/types.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/example/sample_customer_api.py` & `gs-netsuite-api-1.2.2/example/sample_customer_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/example/sample_item_fulfillment_api.py` & `gs-netsuite-api-1.2.2/example/sample_item_fulfillment_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/example/sample_item_receipt_api.py` & `gs-netsuite-api-1.2.2/example/sample_item_receipt_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/example/sample_product_api.py` & `gs-netsuite-api-1.2.2/example/sample_product_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/example/sample_purchase_api.py` & `gs-netsuite-api-1.2.2/example/sample_purchase_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/example/sample_sale_api.py` & `gs-netsuite-api-1.2.2/example/sample_sale_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/example/sample_vendor_api.py` & `gs-netsuite-api-1.2.2/example/sample_vendor_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/mkdocs.yml` & `gs-netsuite-api-1.2.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/wsdl/v2022_2_0/netsuite.wsdl` & `gs-netsuite-api-1.2.2/output/wsdl/v2022_2_0/netsuite.wsdl`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/activities/v2022_2_0/scheduling.xsd` & `gs-netsuite-api-1.2.2/output/xsd/activities/v2022_2_0/scheduling.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/activities/v2022_2_0/schedulingTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/activities/v2022_2_0/schedulingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/documents/v2022_2_0/fileCabinet.xsd` & `gs-netsuite-api-1.2.2/output/xsd/documents/v2022_2_0/fileCabinet.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/general/v2022_2_0/communication.xsd` & `gs-netsuite-api-1.2.2/output/xsd/general/v2022_2_0/communication.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/general/v2022_2_0/communicationTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/general/v2022_2_0/communicationTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/accounting.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/accounting.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/accountingTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/accountingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/employeeTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/employeeTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/employees.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/employees.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/marketing.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/marketing.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/marketingTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/marketingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/relationshipTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/relationshipTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/relationships.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/relationships.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/supplyChain.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/supplyChain.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/support.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/support.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/supportTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/supportTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/lists/v2022_2_0/website.xsd` & `gs-netsuite-api-1.2.2/output/xsd/lists/v2022_2_0/website.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/common.xsd` & `gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/common.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/commonTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/commonTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/core.xsd` & `gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/core.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/coreTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/coreTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/faultTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/faultTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/faults.xsd` & `gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/faults.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/platform/v2022_2_0/messages.xsd` & `gs-netsuite-api-1.2.2/output/xsd/platform/v2022_2_0/messages.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/setup/v2022_2_0/customization.xsd` & `gs-netsuite-api-1.2.2/output/xsd/setup/v2022_2_0/customization.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/setup/v2022_2_0/customizationTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/setup/v2022_2_0/customizationTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/bank.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/bank.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/customerTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/customerTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/customers.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/customers.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/demandPlanning.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/demandPlanning.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/employeeTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/employeeTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/employees.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/employees.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/financial.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/financial.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/financialTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/financialTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/general.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/general.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/inventory.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/inventory.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/purchases.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/purchases.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/saleTypes.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/saleTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/output/xsd/transactions/v2022_2_0/sales.xsd` & `gs-netsuite-api-1.2.2/output/xsd/transactions/v2022_2_0/sales.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/pyproject.toml` & `gs-netsuite-api-1.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -28,7 +28,12 @@
 
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 line-length = 120
+
+[tool.isort]
+profile = "black"
+skip_gitignore = true
+skip = "__init__.py"
```

### Comparing `gs-netsuite-api-1.2.1/src/gs_netsuite_api/api.py` & `gs-netsuite-api-1.2.2/src/gs_netsuite_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,29 @@
 import asyncio
 import datetime
 import logging
 from typing import Any, Callable, Coroutine, Generic, List, TypeVar
 
 from netsuite import NetSuiteSoapApi
 
-from .data_types import (InventoryAdjustment, InventoryAdjustmentLine,
-                         ItemMove, ItemPicking, ProductAvailability,
-                         ProductData, PurchaseOrderData, PurchaseOrderLineData,
-                         RecordRef, RelationShip, SaleOrderData,
-                         SaleOrderLineData)
-from .ns_utils import (NetSuiteCredential, SearchParams, assertSuccess,
-                       search_with_pref)
+from .data_types import (
+    InventoryAdjustment,
+    InventoryAdjustmentLine,
+    ItemMove,
+    ItemPicking,
+    ProductAvailability,
+    ProductData,
+    PurchaseOrderData,
+    PurchaseOrderLineData,
+    RecordRef,
+    RelationShip,
+    SaleOrderData,
+    SaleOrderLineData,
+)
+from .ns_utils import NetSuiteCredential, SearchParams, assertSuccess, search_with_pref
 
 _logger = logging.getLogger(__name__)
 RT = TypeVar("RT", bound=RecordRef)
 R = TypeVar("R", bound=Any)
 
 
 class GsNetSuiteApi(abc.ABC, Generic[RT]):
@@ -561,15 +569,15 @@
                     amount_tax_included=sub_el.grossAmt,
                     order_qty=sub_el.quantity,
                     billed_qty=sub_el.quantityBilled,
                     backordered_qty=sub_el.quantityBackOrdered,
                     committed_qty=sub_el.quantityCommitted,
                     on_hand_qty=sub_el.quantityOnHand,
                     closed=sub_el.isClosed,
-                    custom_fields=sub_el.customFieldList.customField,
+                    custom_fields=sub_el.customFieldList and sub_el.customFieldList.customField or {},
                 )
             )
         return sale
 
 
 class _BaseItemStockAPI(_TransactionAPI[ItemPicking]):
     def _convert_to_data(self, record) -> ItemPicking:
```

### Comparing `gs-netsuite-api-1.2.1/src/gs_netsuite_api/data_types.py` & `gs-netsuite-api-1.2.2/src/gs_netsuite_api/data_types.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/src/gs_netsuite_api/ns_utils.py` & `gs-netsuite-api-1.2.2/src/gs_netsuite_api/ns_utils.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/src/gs_netsuite_api.egg-info/SOURCES.txt` & `gs-netsuite-api-1.2.2/src/gs_netsuite_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.2.1/wsdldownloader.py` & `gs-netsuite-api-1.2.2/wsdldownloader.py`

 * *Files identical despite different names*

