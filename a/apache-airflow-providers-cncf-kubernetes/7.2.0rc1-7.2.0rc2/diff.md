# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-7.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-7.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.2.0rc1.tar", last modified: Wed Jul  5 07:29:50 2023, max compression
+gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.2.0rc2.tar", last modified: Thu Jul  6 04:50:31 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1.tar` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.958422 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-07-05 07:29:49.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4637 2023-07-05 07:29:50.959046 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2963 2023-07-05 07:29:49.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.816293 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.817531 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.818692 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.865239 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-05 07:19:39.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.871145 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.877032 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4483 2023-07-05 07:29:49.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.882992 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23125 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.898742 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    40772 2023-07-05 07:19:39.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0 root         (0) root         (0)     6484 2023-06-28 06:26:40.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.910348 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.919973 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    11941 2023-06-30 08:49:17.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.931804 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0 root         (0) root         (0)    24797 2023-07-01 06:49:42.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:50.955701 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4637 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1893 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:50.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-07-05 07:29:50.960978 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-05 07:29:49.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:31.044342 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-07-06 04:50:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-07-06 04:50:31.044953 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-07-06 04:50:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.896052 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.897373 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.898543 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.955705 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-05 18:48:19.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.961583 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.968046 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-07-06 04:50:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.974522 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23125 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.991405 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    40772 2023-07-05 07:19:39.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0 root         (0) root         (0)     6484 2023-06-28 06:26:40.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:30.997085 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:31.005609 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    11941 2023-06-30 08:49:17.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:31.017562 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0 root         (0) root         (0)    24797 2023-07-01 06:49:42.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:31.041692 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:30.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-06 04:50:31.046894 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-06 04:50:29.000000 apache-airflow-providers-cncf-kubernetes-7.2.0rc2/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/LICENSE` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.2.0rc1
+Version: 7.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.2.0rc1``
+Release: ``7.2.0rc2``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/README.rst` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.2.0rc1``
+Release: ``7.2.0rc2``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.2.0rc1
+Version: 7.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.2.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.2.0rc1``
+Release: ``7.2.0rc2``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -57,10 +57,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.cncf.kubernetes.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.cncf.kubernetes
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.2.0rc1/setup.py` & `apache-airflow-providers-cncf-kubernetes-7.2.0rc2/setup.py`

 * *Files identical despite different names*

