# Comparing `tmp/dragonk8s-0.0.1.tar.gz` & `tmp/dragonk8s-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonk8s-0.0.1.tar", last modified: Sat Jul  8 01:07:05 2023, max compression
+gzip compressed data, was "dragonk8s-1.0.0.tar", last modified: Sun Jul  9 07:07:49 2023, max compression
```

## Comparing `dragonk8s-0.0.1.tar` & `dragonk8s-1.0.0.tar`

### file list

```diff
@@ -1,289 +1,293 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.697709 dragonk8s-0.0.1/
--rw-r--r--   0 bytedance   (501) staff       (20)      526 2023-07-08 01:07:05.697991 dragonk8s-0.0.1/PKG-INFO
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.476026 dragonk8s-0.0.1/dragonk8s/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:13:15.000000 dragonk8s-0.0.1/dragonk8s/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.480132 dragonk8s-0.0.1/dragonk8s/cmd/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/cmd/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2300 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/cmd/replicaset_controller.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.483730 dragonk8s-0.0.1/dragonk8s/dragon/
--rw-r--r--   0 bytedance   (501) staff       (20)    20327 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.484778 dragonk8s-0.0.1/dragonk8s/dragon/api/
--rw-r--r--   0 bytedance   (501) staff       (20)       87 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/dragon/api/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    25570 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/api_client.py
--rw-r--r--   0 bytedance   (501) staff       (20)    13219 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/dragon/configuration.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3789 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/dragon/exceptions.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.621821 dragonk8s-0.0.1/dragonk8s/dragon/models/
--rw-r--r--   0 bytedance   (501) staff       (20)    19878 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7340 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7160 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_list.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11281 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5424 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6311 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector_match_expressions.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4536 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template.py
--rw-r--r--   0 bytedance   (501) staff       (20)    56389 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5932 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8080 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5669 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7051 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference_match_expressions.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5771 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preferred_during_scheduling_ignored_during_execution.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4948 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6305 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution_node_selector_terms.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9118 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8852 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6036 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_label_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6084 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_namespace_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5914 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_preferred_during_scheduling_ignored_during_execution.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9472 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_required_during_scheduling_ignored_during_execution.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9206 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_anti_affinity.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8504 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_aws_elastic_block_store.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9422 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_disk.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6151 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_file.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9338 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3926 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7400 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3926 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8561 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6613 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_items.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4830 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)    33173 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_containers.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8609 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3990 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi_node_publish_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6588 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4367 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5772 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5101 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_field_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7896 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_items.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6144 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_resource_field_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5807 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_empty_dir.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6430 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5684 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env_from.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4014 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral.py
--rw-r--r--   0 bytedance   (501) staff       (20)    35072 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_containers.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5208 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template.py
--rw-r--r--   0 bytedance   (501) staff       (20)    12563 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6531 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6579 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5787 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_resources.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5952 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7957 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_fc.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8074 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3958 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5003 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flocker.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8566 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_gce_persistent_disk.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6126 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_git_repo.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6411 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_glusterfs.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4531 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_aliases.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5007 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_path.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3934 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_image_pull_secrets.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15402 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3918 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5628 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_label_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4679 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4691 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle1.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5749 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4520 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_exec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8264 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5030 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get_http_headers.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5036 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_tcp_socket.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5717 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_pre_stop.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15919 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15963 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe1.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5173 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_grpc.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4976 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_tcp_socket.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6182 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_nfs.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4372 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_os.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5354 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_persistent_volume_claim.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5162 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_photon_persistent_disk.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8175 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ports.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6203 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_portworx_volume.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5636 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6869 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_config_map.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3894 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_downward_api.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6813 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_secret.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7305 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_service_account_token.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6992 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_sources.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9041 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_quobyte.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11636 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3902 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4117 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_gates.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15963 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_probe.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5403 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5415 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources1.py
--rw-r--r--   0 bytedance   (501) staff       (20)    13690 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3934 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8578 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4788 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)    18343 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context.py
--rw-r--r--   0 bytedance   (501) staff       (20)    18391 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context1.py
--rw-r--r--   0 bytedance   (501) staff       (20)    18069 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6689 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_se_linux_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6024 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_seccomp_profile.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4890 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_sysctls.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9521 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_windows_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4599 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_capabilities.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6669 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_se_linux_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6012 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_seccomp_profile.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9501 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_windows_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15875 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_startup_probe.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8948 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3950 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9007 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_tolerations.py
--rw-r--r--   0 bytedance   (501) staff       (20)    22109 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_topology_spread_constraints.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7066 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5968 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_config_map_key_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5077 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_field_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6112 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_resource_field_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6010 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_secret_key_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5079 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_devices.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9982 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_mounts.py
--rw-r--r--   0 bytedance   (501) staff       (20)    30790 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volumes.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7634 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_vsphere_volume.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9920 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_status.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8637 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_conditions.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4659 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_uncounted_terminated_pods.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7550 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7335 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_list.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6125 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_spec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8587 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7781 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status_conditions.py
--rw-r--r--   0 bytedance   (501) staff       (20)    12500 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/dragon/rest.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.622572 dragonk8s-0.0.1/dragonk8s/lib/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.623145 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.625181 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.628323 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/api/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/api/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5347 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/api/errors.py
--rw-r--r--   0 bytedance   (501) staff       (20)       50 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/api/meta.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.631901 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/apis/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      228 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/apis/meta_internal_version.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3992 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/apis/meta_v1.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9011 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/labels.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.633766 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/runtime/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/runtime/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2082 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/runtime/schema.py
--rw-r--r--   0 bytedance   (501) staff       (20)      210 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/selection.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.635256 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/types/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/types/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      253 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/types/patch.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.636650 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/util/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/util/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.638244 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/util/validation/
--rw-r--r--   0 bytedance   (501) staff       (20)       89 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/util/validation/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3534 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/util/validation/field.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1464 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/util/wait.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.640295 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/watch/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/watch/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4802 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/watch/mux.py
--rw-r--r--   0 bytedance   (501) staff       (20)      436 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/watch/watch.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.641693 dragonk8s-0.0.1/dragonk8s/lib/apimeta/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimeta/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1150 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/apimeta/apigvk.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.642613 dragonk8s-0.0.1/dragonk8s/lib/client/
--rw-r--r--   0 bytedance   (501) staff       (20)    12964 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.646857 dragonk8s-0.0.1/dragonk8s/lib/client/informers/
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/client/informers/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.648166 dragonk8s-0.0.1/dragonk8s/lib/client/informers/dragon/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/client/informers/dragon/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1823 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/informers/dragon/replicaset.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4242 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/lib/client/informers/factory.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1043 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/informers/informer.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.649009 dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.649669 dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/typed/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/typed/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.650268 dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/typed/core/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/typed/core/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.651538 dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/typed/core/v1/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/typed/core/v1/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      761 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/typed/core/v1/event_expansion.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.652549 dragonk8s-0.0.1/dragonk8s/lib/client/lister/
--rw-r--r--   0 bytedance   (501) staff       (20)     2982 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/lister/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.659506 dragonk8s-0.0.1/dragonk8s/lib/client/tools/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/client/tools/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11815 2023-07-08 01:05:12.000000 dragonk8s-0.0.1/dragonk8s/lib/client/tools/cache.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11329 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/tools/delta.py
--rw-r--r--   0 bytedance   (501) staff       (20)    13949 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/tools/events.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5330 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/tools/fifo.py
--rw-r--r--   0 bytedance   (501) staff       (20)    30330 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/tools/informer.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2200 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/lib/client/tools/pager.py
--rw-r--r--   0 bytedance   (501) staff       (20)    19026 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/lib/client/tools/record.py
--rw-r--r--   0 bytedance   (501) staff       (20)      908 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/tools/reference.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.664282 dragonk8s-0.0.1/dragonk8s/lib/client/util/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/client/util/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1182 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/lib/client/util/flow_control.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3604 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/client/util/trans.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8618 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/lib/client/util/workqueue.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.665883 dragonk8s-0.0.1/dragonk8s/lib/models/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/models/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      165 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/models/corev1.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.667322 dragonk8s-0.0.1/dragonk8s/lib/pool/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/pool/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1609 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/pool/thread_manager.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.668744 dragonk8s-0.0.1/dragonk8s/lib/util/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/util/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.670016 dragonk8s-0.0.1/dragonk8s/lib/util/cache/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/util/cache/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1738 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/util/cache/lru.py
--rw-r--r--   0 bytedance   (501) staff       (20)      238 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/util/string.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.671442 dragonk8s-0.0.1/dragonk8s/lib/util/timeutil/
--rw-r--r--   0 bytedance   (501) staff       (20)     1008 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/util/timeutil/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6557 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/lib/util/timeutil/rate.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.672113 dragonk8s-0.0.1/dragonk8s/pkg/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/pkg/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.673326 dragonk8s-0.0.1/dragonk8s/pkg/api/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/pkg/api/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)       78 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/pkg/api/types.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.674783 dragonk8s-0.0.1/dragonk8s/pkg/api/v1/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/pkg/api/v1/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1770 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/pkg/api/v1/pod_util.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.676145 dragonk8s-0.0.1/dragonk8s/pkg/controller/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/pkg/controller/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    19819 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/pkg/controller/controller_utils.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.680919 dragonk8s-0.0.1/dragonk8s/pkg/controller/replicaset/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-0.0.1/dragonk8s/pkg/controller/replicaset/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    21700 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/dragonk8s/pkg/controller/replicaset/replica_set.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5025 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/dragonk8s/pkg/controller/replicaset/replica_set_utils.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.478981 dragonk8s-0.0.1/dragonk8s.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)      526 2023-07-08 01:07:05.000000 dragonk8s-0.0.1/dragonk8s.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)    15651 2023-07-08 01:07:05.000000 dragonk8s-0.0.1/dragonk8s.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-08 01:07:05.000000 dragonk8s-0.0.1/dragonk8s.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       16 2023-07-08 01:07:05.000000 dragonk8s-0.0.1/dragonk8s.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)     1098 2023-07-08 01:07:05.699624 dragonk8s-0.0.1/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)      285 2023-07-08 01:07:03.000000 dragonk8s-0.0.1/setup.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.681628 dragonk8s-0.0.1/tests/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.683579 dragonk8s-0.0.1/tests/dragon/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/dragon/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5822 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/tests/dragon/test_client.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4575 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/tests/dragon/test_infromer.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.684226 dragonk8s-0.0.1/tests/lib/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/lib/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.685444 dragonk8s-0.0.1/tests/lib/client/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/lib/client/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.686328 dragonk8s-0.0.1/tests/lib/client/kubernetes/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/lib/client/kubernetes/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.687093 dragonk8s-0.0.1/tests/lib/client/kubernetes/typed/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/lib/client/kubernetes/typed/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.687757 dragonk8s-0.0.1/tests/lib/client/kubernetes/typed/core/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/lib/client/kubernetes/typed/core/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.688963 dragonk8s-0.0.1/tests/lib/client/kubernetes/typed/core/v1/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/lib/client/kubernetes/typed/core/v1/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5071 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/tests/lib/client/kubernetes/typed/core/v1/test_event_expansion.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.691614 dragonk8s-0.0.1/tests/lib/client/tools/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/lib/client/tools/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      433 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/tests/lib/client/tools/test_cache.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2133 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/tests/lib/client/tools/test_events.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1296 2023-07-08 01:05:11.000000 dragonk8s-0.0.1/tests/lib/client/tools/test_record.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1704 2023-07-06 13:41:18.000000 dragonk8s-0.0.1/tests/lib/client/util_test.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.692820 dragonk8s-0.0.1/tests/lib/until/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/lib/until/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      450 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/tests/lib/until/test_util.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.694462 dragonk8s-0.0.1/tests/pkg/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/pkg/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-08 01:07:05.696988 dragonk8s-0.0.1/tests/pkg/controller/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-0.0.1/tests/pkg/controller/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3840 2023-07-08 01:05:10.000000 dragonk8s-0.0.1/tests/pkg/controller/test_controller_utils.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:49.012318 dragonk8s-1.0.0/
+-rw-r--r--   0 bytedance   (501) staff       (20)      526 2023-07-09 07:07:49.012639 dragonk8s-1.0.0/PKG-INFO
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.676597 dragonk8s-1.0.0/dragonk8s/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 01:14:53.000000 dragonk8s-1.0.0/dragonk8s/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.679063 dragonk8s-1.0.0/dragonk8s/cmd/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/cmd/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2300 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/cmd/replicaset_controller.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.683996 dragonk8s-1.0.0/dragonk8s/dragon/
+-rw-r--r--   0 bytedance   (501) staff       (20)    20327 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.685120 dragonk8s-1.0.0/dragonk8s/dragon/api/
+-rw-r--r--   0 bytedance   (501) staff       (20)       87 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/dragon/api/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    25570 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/api_client.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    13219 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/dragon/configuration.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3789 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/dragon/exceptions.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.894888 dragonk8s-1.0.0/dragonk8s/dragon/models/
+-rw-r--r--   0 bytedance   (501) staff       (20)    19839 2023-07-08 07:31:36.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7340 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7160 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_list.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    11281 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5424 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6311 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector_match_expressions.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4536 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    56389 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5932 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8080 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5669 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7051 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference_match_expressions.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5771 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preferred_during_scheduling_ignored_during_execution.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4948 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6305 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution_node_selector_terms.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9118 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8852 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6036 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_label_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6084 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_namespace_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5914 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_preferred_during_scheduling_ignored_during_execution.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9472 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_required_during_scheduling_ignored_during_execution.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9206 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_anti_affinity.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8504 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_aws_elastic_block_store.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9422 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_disk.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6151 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_file.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9338 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3926 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7400 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3926 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8561 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6613 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_items.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4830 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    33173 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_containers.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8609 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3990 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi_node_publish_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6588 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4367 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5772 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5101 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_field_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7896 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_items.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6144 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_resource_field_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5807 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_empty_dir.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6430 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5684 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env_from.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4014 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    35072 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_containers.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5208 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    12563 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6531 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6579 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5787 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_resources.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5952 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7957 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_fc.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8074 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3958 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5003 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flocker.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8566 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_gce_persistent_disk.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6126 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_git_repo.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6411 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_glusterfs.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4531 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_aliases.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5007 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_path.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3934 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_image_pull_secrets.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15402 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3918 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5628 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_label_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4679 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4691 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5749 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4520 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_exec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8264 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5030 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get_http_headers.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5036 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_tcp_socket.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5717 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_pre_stop.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15919 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15963 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5173 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_grpc.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4976 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_tcp_socket.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6182 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_nfs.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4372 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_os.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5354 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_persistent_volume_claim.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5162 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_photon_persistent_disk.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8175 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ports.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6203 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_portworx_volume.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5636 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6869 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_config_map.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3894 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_downward_api.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6813 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_secret.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7305 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_service_account_token.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6992 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_sources.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9041 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_quobyte.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    11636 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3902 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4117 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_gates.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15963 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_probe.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5403 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5415 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    13690 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3934 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8578 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4788 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    18343 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    18391 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    18069 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6689 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_se_linux_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6024 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_seccomp_profile.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4890 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_sysctls.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9521 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_windows_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4599 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_capabilities.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6669 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_se_linux_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6012 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_seccomp_profile.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9501 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_windows_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15875 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_startup_probe.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8948 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3950 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9007 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_tolerations.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    22109 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_topology_spread_constraints.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7066 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5968 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_config_map_key_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5077 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_field_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6112 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_resource_field_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6010 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_secret_key_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5079 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_devices.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9982 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_mounts.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    30790 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volumes.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7634 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_vsphere_volume.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9920 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_status.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8637 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_conditions.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4659 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_uncounted_terminated_pods.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7550 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7335 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_list.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6125 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_spec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8587 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7781 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status_conditions.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    12500 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/dragon/rest.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.895906 dragonk8s-1.0.0/dragonk8s/lib/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.896461 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.902079 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.909472 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/api/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5347 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/api/errors.py
+-rw-r--r--   0 bytedance   (501) staff       (20)       50 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/api/meta.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.913067 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/apis/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      228 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/apis/meta_internal_version.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3992 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/apis/meta_v1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9011 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/labels.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.914500 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/runtime/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/runtime/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2082 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/runtime/schema.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      210 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/selection.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.916071 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/types/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/types/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      253 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/types/patch.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.918434 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/util/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/util/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.920536 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/util/validation/
+-rw-r--r--   0 bytedance   (501) staff       (20)       89 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/util/validation/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3534 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/util/validation/field.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1464 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/util/wait.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.923907 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/watch/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/watch/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4802 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/watch/mux.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      436 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/watch/watch.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.925485 dragonk8s-1.0.0/dragonk8s/lib/apimeta/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/apimeta/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1607 2023-07-08 07:54:43.000000 dragonk8s-1.0.0/dragonk8s/lib/apimeta/apigvk.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.934410 dragonk8s-1.0.0/dragonk8s/lib/client/
+-rw-r--r--   0 bytedance   (501) staff       (20)    12934 2023-07-08 07:45:28.000000 dragonk8s-1.0.0/dragonk8s/lib/client/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    26010 2023-07-08 07:39:40.000000 dragonk8s-1.0.0/dragonk8s/lib/client/api_client.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    13219 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/configuration.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3789 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/exceptions.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.937852 dragonk8s-1.0.0/dragonk8s/lib/client/informers/
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/informers/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.940981 dragonk8s-1.0.0/dragonk8s/lib/client/informers/dragon/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/informers/dragon/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1823 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/informers/dragon/replicaset.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4242 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/lib/client/informers/factory.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1043 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/informers/informer.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.942258 dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.942821 dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/typed/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/typed/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.943355 dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/typed/core/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/typed/core/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.944625 dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/typed/core/v1/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/typed/core/v1/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      761 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/typed/core/v1/event_expansion.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.945673 dragonk8s-1.0.0/dragonk8s/lib/client/lister/
+-rw-r--r--   0 bytedance   (501) staff       (20)     2982 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/lister/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    12500 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/rest.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.957423 dragonk8s-1.0.0/dragonk8s/lib/client/tools/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/tools/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    11815 2023-07-08 01:05:12.000000 dragonk8s-1.0.0/dragonk8s/lib/client/tools/cache.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    11329 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/tools/delta.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    13949 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/tools/events.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5330 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/tools/fifo.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    30330 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/tools/informer.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2200 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/lib/client/tools/pager.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    19026 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/lib/client/tools/record.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      908 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/tools/reference.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.962135 dragonk8s-1.0.0/dragonk8s/lib/client/util/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/util/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1182 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/lib/client/util/flow_control.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3604 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/client/util/trans.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8618 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/lib/client/util/workqueue.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.964290 dragonk8s-1.0.0/dragonk8s/lib/models/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/models/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      165 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/models/corev1.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.966111 dragonk8s-1.0.0/dragonk8s/lib/pool/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/pool/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1609 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/pool/thread_manager.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.968063 dragonk8s-1.0.0/dragonk8s/lib/util/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/util/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.971486 dragonk8s-1.0.0/dragonk8s/lib/util/cache/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/util/cache/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1738 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/util/cache/lru.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      238 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/util/string.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.974017 dragonk8s-1.0.0/dragonk8s/lib/util/timeutil/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1008 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/util/timeutil/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6557 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/lib/util/timeutil/rate.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.975065 dragonk8s-1.0.0/dragonk8s/pkg/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/pkg/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.976578 dragonk8s-1.0.0/dragonk8s/pkg/api/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/pkg/api/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)       78 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/pkg/api/types.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.978230 dragonk8s-1.0.0/dragonk8s/pkg/api/v1/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/pkg/api/v1/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1770 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/pkg/api/v1/pod_util.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.980164 dragonk8s-1.0.0/dragonk8s/pkg/controller/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/pkg/controller/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    19819 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/pkg/controller/controller_utils.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.984156 dragonk8s-1.0.0/dragonk8s/pkg/controller/replicaset/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.0/dragonk8s/pkg/controller/replicaset/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    21700 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/dragonk8s/pkg/controller/replicaset/replica_set.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5025 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/dragonk8s/pkg/controller/replicaset/replica_set_utils.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.678283 dragonk8s-1.0.0/dragonk8s.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)      526 2023-07-09 07:07:48.000000 dragonk8s-1.0.0/dragonk8s.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)    15788 2023-07-09 07:07:48.000000 dragonk8s-1.0.0/dragonk8s.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-09 07:07:48.000000 dragonk8s-1.0.0/dragonk8s.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       16 2023-07-09 07:07:48.000000 dragonk8s-1.0.0/dragonk8s.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)     1098 2023-07-09 07:07:49.014175 dragonk8s-1.0.0/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)      285 2023-07-09 07:07:44.000000 dragonk8s-1.0.0/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.985878 dragonk8s-1.0.0/tests/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.990092 dragonk8s-1.0.0/tests/dragon/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/dragon/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5940 2023-07-08 07:53:20.000000 dragonk8s-1.0.0/tests/dragon/test_client.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4575 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/tests/dragon/test_infromer.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.991257 dragonk8s-1.0.0/tests/lib/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/lib/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.992603 dragonk8s-1.0.0/tests/lib/client/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/lib/client/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.993831 dragonk8s-1.0.0/tests/lib/client/kubernetes/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/lib/client/kubernetes/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.994372 dragonk8s-1.0.0/tests/lib/client/kubernetes/typed/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/lib/client/kubernetes/typed/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.994984 dragonk8s-1.0.0/tests/lib/client/kubernetes/typed/core/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/lib/client/kubernetes/typed/core/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:48.996524 dragonk8s-1.0.0/tests/lib/client/kubernetes/typed/core/v1/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/lib/client/kubernetes/typed/core/v1/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5071 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/tests/lib/client/kubernetes/typed/core/v1/test_event_expansion.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:49.006302 dragonk8s-1.0.0/tests/lib/client/tools/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/lib/client/tools/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      433 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/tests/lib/client/tools/test_cache.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2133 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/tests/lib/client/tools/test_events.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1296 2023-07-08 01:05:11.000000 dragonk8s-1.0.0/tests/lib/client/tools/test_record.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1704 2023-07-06 13:41:18.000000 dragonk8s-1.0.0/tests/lib/client/util_test.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:49.008592 dragonk8s-1.0.0/tests/lib/until/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/lib/until/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      450 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/tests/lib/until/test_util.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:49.009860 dragonk8s-1.0.0/tests/pkg/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/pkg/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-09 07:07:49.011253 dragonk8s-1.0.0/tests/pkg/controller/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.0/tests/pkg/controller/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3840 2023-07-08 01:05:10.000000 dragonk8s-1.0.0/tests/pkg/controller/test_controller_utils.py
```

### Comparing `dragonk8s-0.0.1/PKG-INFO` & `dragonk8s-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonk8s
-Version: 0.0.1
+Version: 1.0.0
 Summary: A k8s implement of Python3
 Home-page: https://dragonk8s.com
 Author: ma
 Author-email: 591867837@qq.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dragonk8s-0.0.1/dragonk8s/cmd/replicaset_controller.py` & `dragonk8s-1.0.0/dragonk8s/cmd/replicaset_controller.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/__init__.py` & `dragonk8s-1.0.0/dragonk8s/dragon/__init__.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/api_client.py` & `dragonk8s-1.0.0/dragonk8s/dragon/api_client.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/configuration.py` & `dragonk8s-1.0.0/dragonk8s/dragon/configuration.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/exceptions.py` & `dragonk8s-1.0.0/dragonk8s/dragon/exceptions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/__init__.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,9 +142,7 @@
 from dragonk8s.dragon.models.io_dragon_apps_v1_job_status_conditions import IoDragonAppsV1JobStatusConditions
 from dragonk8s.dragon.models.io_dragon_apps_v1_job_status_uncounted_terminated_pods import IoDragonAppsV1JobStatusUncountedTerminatedPods
 from dragonk8s.dragon.models.io_dragon_apps_v1_replica_set import IoDragonAppsV1ReplicaSet
 from dragonk8s.dragon.models.io_dragon_apps_v1_replica_set_list import IoDragonAppsV1ReplicaSetList
 from dragonk8s.dragon.models.io_dragon_apps_v1_replica_set_spec import IoDragonAppsV1ReplicaSetSpec
 from dragonk8s.dragon.models.io_dragon_apps_v1_replica_set_status import IoDragonAppsV1ReplicaSetStatus
 from dragonk8s.dragon.models.io_dragon_apps_v1_replica_set_status_conditions import IoDragonAppsV1ReplicaSetStatusConditions
-
-from kubernetes.client.models import *
```

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_list.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_list.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector_match_expressions.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector_match_expressions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference_match_expressions.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference_match_expressions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preferred_during_scheduling_ignored_during_execution.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preferred_during_scheduling_ignored_during_execution.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution_node_selector_terms.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution_node_selector_terms.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_label_selector.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_label_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_namespace_selector.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_namespace_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_preferred_during_scheduling_ignored_during_execution.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_preferred_during_scheduling_ignored_during_execution.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_required_during_scheduling_ignored_during_execution.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_required_during_scheduling_ignored_during_execution.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_anti_affinity.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_aws_elastic_block_store.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_aws_elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_disk.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_disk.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_file.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_file.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs_secret_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder_secret_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_items.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_items.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_containers.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_containers.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi_node_publish_secret_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi_node_publish_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config_options.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_field_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_field_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_items.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_items.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_resource_field_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_resource_field_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_empty_dir.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_empty_dir.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env_from.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env_from.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_containers.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_containers.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_resources.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_resources.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_selector.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_fc.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_fc.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume_secret_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flocker.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flocker.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_gce_persistent_disk.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_gce_persistent_disk.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_git_repo.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_git_repo.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_glusterfs.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_glusterfs.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_aliases.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_aliases.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_path.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_path.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_image_pull_secrets.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_image_pull_secrets.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi_secret_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_label_selector.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_label_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle1.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_exec.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_exec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get_http_headers.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get_http_headers.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_tcp_socket.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_tcp_socket.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_pre_stop.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_pre_stop.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe1.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_grpc.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_grpc.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_tcp_socket.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_tcp_socket.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_nfs.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_nfs.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_os.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_os.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_persistent_volume_claim.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_photon_persistent_disk.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_photon_persistent_disk.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ports.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ports.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_portworx_volume.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_portworx_volume.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_config_map.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_config_map.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_downward_api.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_downward_api.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_secret.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_secret.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_service_account_token.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_service_account_token.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_sources.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_sources.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_quobyte.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_quobyte.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd_secret_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_gates.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_gates.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_probe.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_probe.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources1.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io_secret_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context1.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_se_linux_options.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_se_linux_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_seccomp_profile.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_seccomp_profile.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_sysctls.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_sysctls.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_windows_options.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_windows_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_capabilities.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_capabilities.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_se_linux_options.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_se_linux_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_seccomp_profile.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_seccomp_profile.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_windows_options.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_windows_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_startup_probe.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_startup_probe.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos_secret_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_tolerations.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_tolerations.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_topology_spread_constraints.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_config_map_key_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_config_map_key_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_field_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_field_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_resource_field_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_resource_field_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_secret_key_ref.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_secret_key_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_devices.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_devices.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_mounts.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_mounts.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volumes.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volumes.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_vsphere_volume.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_vsphere_volume.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_status.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_status.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_conditions.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_conditions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_uncounted_terminated_pods.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_uncounted_terminated_pods.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_list.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_list.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_spec.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_spec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status_conditions.py` & `dragonk8s-1.0.0/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status_conditions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/dragon/rest.py` & `dragonk8s-1.0.0/dragonk8s/dragon/rest.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/api/errors.py` & `dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/api/errors.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/apis/meta_v1.py` & `dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/apis/meta_v1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/labels.py` & `dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/labels.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/runtime/schema.py` & `dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/runtime/schema.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/util/validation/field.py` & `dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/util/validation/field.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/util/wait.py` & `dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/util/wait.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/apimachinery/pkg/watch/mux.py` & `dragonk8s-1.0.0/dragonk8s/lib/apimachinery/pkg/watch/mux.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/__init__.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import six
 from kubernetes.dynamic.client import DynamicClient, ResourceInstance, ApiException, api_exception
-from kubernetes.client.api_client import ApiClient
+from dragonk8s.lib.client.api_client import ApiClient
 from dragonk8s.lib.apimeta import apigvk
 from kubernetes.watch.watch import Watch, SimpleNamespace
-from kubernetes import client
 from dragonk8s.lib.apimachinery.pkg.watch import watch
 from queue import Queue
 
 
 class SimpleBody(object):
 
     def __init__(self, data):
@@ -77,20 +76,21 @@
 
 
 class CommonClient(DynamicClient):
 
     def _get_response_type_list(self, response_type):
         return "{}List".format(response_type)
 
-    def __init__(self, client=None, cache_file=None, discoverer=None):
-        if client is None:
-            client = ApiClient()
+    def __init__(self, cache_file=None, discoverer=None):
+        client = ApiClient()
+
         super().__init__(client, cache_file, discoverer)
         self.response_type_map = {}
         self.init_response_type()
+        apigvk.register_model_package()
 
     def init_response_type(self):
         for gvk in apigvk.ALL:
             self.register_response_type(api_version=gvk.group_version, kind=gvk.kind, response_type=gvk.response_type)
 
     def get_response_type(self, api_version: str, kind: str) -> str:
         key = "{}/{}".format(api_version, kind)
```

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/informers/dragon/replicaset.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/informers/dragon/replicaset.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/informers/factory.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/informers/factory.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/informers/informer.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/informers/informer.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/kubernetes/typed/core/v1/event_expansion.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/kubernetes/typed/core/v1/event_expansion.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/lister/__init__.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/lister/__init__.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/tools/cache.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/tools/cache.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/tools/delta.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/tools/delta.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/tools/events.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/tools/events.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/tools/fifo.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/tools/fifo.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/tools/informer.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/tools/informer.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/tools/pager.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/tools/pager.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/tools/record.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/tools/record.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/tools/reference.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/tools/reference.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/util/flow_control.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/util/flow_control.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/util/trans.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/util/trans.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/client/util/workqueue.py` & `dragonk8s-1.0.0/dragonk8s/lib/client/util/workqueue.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/pool/thread_manager.py` & `dragonk8s-1.0.0/dragonk8s/lib/pool/thread_manager.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/util/cache/lru.py` & `dragonk8s-1.0.0/dragonk8s/lib/util/cache/lru.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/util/timeutil/__init__.py` & `dragonk8s-1.0.0/dragonk8s/lib/util/timeutil/__init__.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/lib/util/timeutil/rate.py` & `dragonk8s-1.0.0/dragonk8s/lib/util/timeutil/rate.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/pkg/api/v1/pod_util.py` & `dragonk8s-1.0.0/dragonk8s/pkg/api/v1/pod_util.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/pkg/controller/controller_utils.py` & `dragonk8s-1.0.0/dragonk8s/pkg/controller/controller_utils.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/pkg/controller/replicaset/replica_set.py` & `dragonk8s-1.0.0/dragonk8s/pkg/controller/replicaset/replica_set.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s/pkg/controller/replicaset/replica_set_utils.py` & `dragonk8s-1.0.0/dragonk8s/pkg/controller/replicaset/replica_set_utils.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/dragonk8s.egg-info/PKG-INFO` & `dragonk8s-1.0.0/dragonk8s.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonk8s
-Version: 0.0.1
+Version: 1.0.0
 Summary: A k8s implement of Python3
 Home-page: https://dragonk8s.com
 Author: ma
 Author-email: 591867837@qq.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dragonk8s-0.0.1/dragonk8s.egg-info/SOURCES.txt` & `dragonk8s-1.0.0/dragonk8s.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,18 @@
 dragonk8s/lib/apimachinery/pkg/util/validation/field.py
 dragonk8s/lib/apimachinery/pkg/watch/__init__.py
 dragonk8s/lib/apimachinery/pkg/watch/mux.py
 dragonk8s/lib/apimachinery/pkg/watch/watch.py
 dragonk8s/lib/apimeta/__init__.py
 dragonk8s/lib/apimeta/apigvk.py
 dragonk8s/lib/client/__init__.py
+dragonk8s/lib/client/api_client.py
+dragonk8s/lib/client/configuration.py
+dragonk8s/lib/client/exceptions.py
+dragonk8s/lib/client/rest.py
 dragonk8s/lib/client/informers/__init__.py
 dragonk8s/lib/client/informers/factory.py
 dragonk8s/lib/client/informers/informer.py
 dragonk8s/lib/client/informers/dragon/__init__.py
 dragonk8s/lib/client/informers/dragon/replicaset.py
 dragonk8s/lib/client/kubernetes/__init__.py
 dragonk8s/lib/client/kubernetes/typed/__init__.py
```

### Comparing `dragonk8s-0.0.1/setup.cfg` & `dragonk8s-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/tests/dragon/test_client.py` & `dragonk8s-1.0.0/tests/dragon/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import unittest
 from kubernetes import config, dynamic
 from kubernetes.client import models, configuration, api_client
 from dragonk8s.dragon.models import *
 from dragonk8s.dragon.models import IoDragonAppsV1ReplicaSetList, IoDragonAppsV1ReplicaSetStatus
 from dragonk8s.lib.client import CommonClient, CommonWatch
 from dragonk8s.dragon.api_client import ApiClient
-from dragonk8s.dragon.configuration import Configuration
+from dragonk8s.lib.client.configuration import Configuration
 from kubernetes.client.models import V1ReplicaSet
 from kubernetes.client.apis import CoreV1Api
 from kubernetes.client.api import CoreApi
 from kubernetes.client.models import V1ObjectMeta
 from kubernetes import watch
 """
 1. 在dragon.models.__init__.py中加上
@@ -21,27 +21,28 @@
 """
 
 
 class DragonClientTest(unittest.TestCase):
 
     def setUp(self):
         cfg = Configuration()
-        config.load_kube_config(config_file="C:\\Users\\Administrator\\.kube\\config", client_configuration=cfg)
+        # config.load_kube_config(config_file="C:\\Users\\Administrator\\.kube\\config", client_configuration=cfg)
+        config.load_kube_config(config_file="/Users/bytedance/mygit/deploy/0_config/my-k8s.conf", client_configuration=cfg)
         Configuration.set_default(cfg)
         self.base_client = ApiClient()
         # client = dynamic.DynamicClient(
         #     self.base_client
         # )
         # config.load_kube_config(config_file="/Users/bytedance/.kube/config")
         # self.base_client = api_client.ApiClient()
         try:
-            client = CommonClient(self.base_client)
-            client2 = dynamic.DynamicClient(self.base_client)
+            client = CommonClient()
+            # client2 = dynamic.DynamicClient(self.base_client)
             self.client = client.resources.get(api_version="apps.dragon.io/v1", kind="ReplicaSet")
-            self.client2 = client2.resources.get(api_version="apps.dragon.io/v1", kind="ReplicaSet")
+            # self.client2 = client2.resources.get(api_version="apps.dragon.io/v1", kind="ReplicaSet")
 
         except EOFError as e:
             print(e)
 
     def test_create(self):
         expressions = IoDragonAppsV1JobSpecSelectorMatchExpressions(
                         key="key",
```

### Comparing `dragonk8s-0.0.1/tests/dragon/test_infromer.py` & `dragonk8s-1.0.0/tests/dragon/test_infromer.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/tests/lib/client/kubernetes/typed/core/v1/test_event_expansion.py` & `dragonk8s-1.0.0/tests/lib/client/kubernetes/typed/core/v1/test_event_expansion.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/tests/lib/client/tools/test_events.py` & `dragonk8s-1.0.0/tests/lib/client/tools/test_events.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/tests/lib/client/tools/test_record.py` & `dragonk8s-1.0.0/tests/lib/client/tools/test_record.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/tests/lib/client/util_test.py` & `dragonk8s-1.0.0/tests/lib/client/util_test.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-0.0.1/tests/pkg/controller/test_controller_utils.py` & `dragonk8s-1.0.0/tests/pkg/controller/test_controller_utils.py`

 * *Files identical despite different names*

