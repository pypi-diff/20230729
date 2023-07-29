# Comparing `tmp/cloud-pak-operations-cli-0.4.1.tar.gz` & `tmp/cloud-pak-operations-cli-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-pak-operations-cli-0.4.1.tar", last modified: Fri Jul 28 09:36:03 2023, max compression
+gzip compressed data, was "cloud-pak-operations-cli-0.4.2.tar", last modified: Sat Jul 29 14:44:57 2023, max compression
```

## Comparing `cloud-pak-operations-cli-0.4.1.tar` & `cloud-pak-operations-cli-0.4.2.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.515417 cloud-pak-operations-cli-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-28 09:36:03.515417 cloud-pak-operations-cli-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.499417 cloud-pak-operations-cli-0.4.1/cloud_pak_operations_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-28 09:36:03.000000 cloud-pak-operations-cli-0.4.1/cloud_pak_operations_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-28 09:36:03.000000 cloud-pak-operations-cli-0.4.1/cloud_pak_operations_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:36:03.000000 cloud-pak-operations-cli-0.4.1/cloud_pak_operations_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 09:36:03.000000 cloud-pak-operations-cli-0.4.1/cloud_pak_operations_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 09:36:03.000000 cloud-pak-operations-cli-0.4.1/cloud_pak_operations_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-28 09:36:03.000000 cloud-pak-operations-cli-0.4.1/cloud_pak_operations_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.499417 cloud-pak-operations-cli-0.4.1/cpo/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.499417 cloud-pak-operations-cli-0.4.1/cpo/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.499417 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.499417 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/config/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/download_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/get-shell-completion-script-location.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.499417 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/ibm_internal_plugin/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/ibm_internal_plugin/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/store_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/adm/update_dev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.503417 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/get_cluster_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/install_nfs_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/install_odf_storage_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/ls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.503417 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/pull_secret/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/pull_secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/pull_secret/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/pull_secret/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/pull_secret/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/use.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.503417 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.503417 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.503417 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/regenerate_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.503417 cloud-pak-operations-cli-0.4.1/cpo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/config/binaries_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/config/cluster_credentials_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/config/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/cpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.495417 cloud-pak-operations-cli-0.4.1/cpo/deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.503417 cloud-pak-operations-cli-0.4.1/cpo/deps/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.503417 cloud-pak-operations-cli-0.4.1/cpo/deps/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/deps/playbooks/deploy_odf_playbook.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.503417 cloud-pak-operations-cli-0.4.1/cpo/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/abstract_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/openshift_playbook_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/playbook_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/playbook_runners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/playbook_runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/click/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/click/cpd_service_spec_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/click/lazy_loading_multi_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/cluster/cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/dependency_manager_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/terraform_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/data/cluster_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/data/ingress_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    19570 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.507417 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.511417 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/jmespath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.511417 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.511417 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/cluster/generic_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/cluster/generic_cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.511417 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/token_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/user_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.511417 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/data/global_pull_secret_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.511417 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/nfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/nfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/oc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45820 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/openshift_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.511417 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/auths_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/catalog_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/get_pod_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/kind_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/object_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/operator_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/role_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.511417 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/utils/click.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.515417 cloud-pak-operations-cli-0.4.1/cpo/lib/plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/plugin_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/plugin_manager/distribution_entry_point_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/plugin_manager/package_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/lib/plugin_manager/plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.515417 cloud-pak-operations-cli-0.4.1/cpo/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/scripts/get_current_cluster_alias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:36:03.515417 cloud-pak-operations-cli-0.4.1/cpo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/http_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/importlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/cpo/utils/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-28 09:35:53.000000 cloud-pak-operations-cli-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 09:36:03.515417 cloud-pak-operations-cli-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.484635 cloud-pak-operations-cli-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-29 14:44:57.484635 cloud-pak-operations-cli-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.452635 cloud-pak-operations-cli-0.4.2/cloud_pak_operations_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-29 14:44:57.000000 cloud-pak-operations-cli-0.4.2/cloud_pak_operations_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-29 14:44:57.000000 cloud-pak-operations-cli-0.4.2/cloud_pak_operations_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:44:57.000000 cloud-pak-operations-cli-0.4.2/cloud_pak_operations_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-29 14:44:57.000000 cloud-pak-operations-cli-0.4.2/cloud_pak_operations_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-29 14:44:57.000000 cloud-pak-operations-cli-0.4.2/cloud_pak_operations_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-29 14:44:57.000000 cloud-pak-operations-cli-0.4.2/cloud_pak_operations_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.452635 cloud-pak-operations-cli-0.4.2/cpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.452635 cloud-pak-operations-cli-0.4.2/cpo/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.452635 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.452635 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/config/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/download_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/get-shell-completion-script-location.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.456635 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/ibm_internal_plugin/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/ibm_internal_plugin/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/store_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/adm/update_dev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.456635 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/get_cluster_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/install_nfs_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/install_odf_storage_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/ls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.460635 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/pull_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/pull_secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/pull_secret/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/pull_secret/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/pull_secret/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/use.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.460635 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.460635 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.460635 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/regenerate_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.460635 cloud-pak-operations-cli-0.4.2/cpo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/config/binaries_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/config/cluster_credentials_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/config/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/cpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.444635 cloud-pak-operations-cli-0.4.2/cpo/deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.464635 cloud-pak-operations-cli-0.4.2/cpo/deps/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.464635 cloud-pak-operations-cli-0.4.2/cpo/deps/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/deps/playbooks/deploy_odf_playbook.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.464635 cloud-pak-operations-cli-0.4.2/cpo/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.464635 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.464635 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/abstract_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/openshift_playbook_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/playbook_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.464635 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/playbook_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/playbook_runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.468635 cloud-pak-operations-cli-0.4.2/cpo/lib/click/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/click/cpd_service_spec_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/click/lazy_loading_multi_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.468635 cloud-pak-operations-cli-0.4.2/cpo/lib/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/cluster/cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.468635 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/dependency_manager_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.468635 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/terraform_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.468635 cloud-pak-operations-cli-0.4.2/cpo/lib/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.468635 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.472635 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/data/cluster_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/data/ingress_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19570 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.472635 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.472635 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/jmespath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.472635 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.472635 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/cluster/generic_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/cluster/generic_cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.476635 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/token_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/user_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.476635 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/data/global_pull_secret_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.476635 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/nfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/nfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/oc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45820 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/openshift_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.480635 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/auths_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/catalog_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/get_pod_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/kind_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/object_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/operator_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/role_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.480635 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/utils/click.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.480635 cloud-pak-operations-cli-0.4.2/cpo/lib/plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/plugin_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/plugin_manager/distribution_entry_point_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/plugin_manager/package_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/lib/plugin_manager/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.480635 cloud-pak-operations-cli-0.4.2/cpo/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/scripts/get_current_cluster_alias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:57.484635 cloud-pak-operations-cli-0.4.2/cpo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/importlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/cpo/utils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-29 14:44:45.000000 cloud-pak-operations-cli-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-29 14:44:57.488635 cloud-pak-operations-cli-0.4.2/setup.cfg
```

### Comparing `cloud-pak-operations-cli-0.4.1/LICENSE` & `cloud-pak-operations-cli-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cloud_pak_operations_cli.egg-info/SOURCES.txt` & `cloud-pak-operations-cli-0.4.2/cloud_pak_operations_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/config/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/config/set.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/config/set.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/download_dependencies.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/download_dependencies.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/get-shell-completion-script-location.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/get-shell-completion-script-location.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/ibm_internal_plugin/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/ibm_internal_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/ibm_internal_plugin/install.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/ibm_internal_plugin/install.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/ibm_internal_plugin/ls.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/ibm_internal_plugin/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/store_credentials.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/store_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/adm/update_dev.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/adm/update_dev.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/add.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/add.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/current.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/current.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/edit.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/edit.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/get_cluster_access_token.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/get_cluster_access_token.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/install_nfs_storage_class.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/install_nfs_storage_class.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/install_odf_storage_classes.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/install_odf_storage_classes.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/login.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/ls.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/pull_secret/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/pull_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/pull_secret/ls.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/pull_secret/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/pull_secret/rm.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/pull_secret/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/pull_secret/set.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/pull_secret/set.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/rm.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/cluster/use.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/cluster/use.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/login.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/logout.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/logout.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/add.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/add.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/login.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/ls.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/rm.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/oc/cluster/status.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/oc/cluster/status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/commands/ibmcloud/regenerate_api_key.py` & `cloud-pak-operations-cli-0.4.2/cpo/commands/ibmcloud/regenerate_api_key.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/config/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/config/binaries_manager.py` & `cloud-pak-operations-cli-0.4.2/cpo/config/binaries_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/config/cluster_credentials_manager.py` & `cloud-pak-operations-cli-0.4.2/cpo/config/cluster_credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/config/configuration_manager.py` & `cloud-pak-operations-cli-0.4.2/cpo/config/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/cpo.py` & `cloud-pak-operations-cli-0.4.2/cpo/cpo.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/deps/autocomplete/cpo-autocomplete-bash.sh` & `cloud-pak-operations-cli-0.4.2/cpo/deps/autocomplete/cpo-autocomplete-bash.sh`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh` & `cloud-pak-operations-cli-0.4.2/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/deps/playbooks/deploy_odf_playbook.yaml` & `cloud-pak-operations-cli-0.4.2/cpo/deps/playbooks/deploy_odf_playbook.yaml`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/abstract_module.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/abstract_module.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/custom_resource_event_result.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/custom_resource_event_result.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/openshift_playbook_runner.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/openshift_playbook_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/playbook_runner.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/playbook_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/click/cpd_service_spec_param_type.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/click/cpd_service_spec_param_type.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/click/lazy_loading_multi_command.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/click/lazy_loading_multi_command.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/click/utils.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/click/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/cluster/cluster.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/cluster/cluster_factory.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/cluster/cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/dependency_manager.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/dependency_manager_plugin.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/dependency_manager_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/dependency_manager/plugins/terraform_plugin.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/dependency_manager/plugins/terraform_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/data/cluster_status.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/data/cluster_status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/data/ingress_status.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/data/ingress_status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/ibm_cloud_api_manager.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/ibm_cloud_api_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/cluster/ls.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/jmespath.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/jmespath.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/cluster/generic_cluster.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/cluster/generic_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/cluster/generic_cluster_factory.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/cluster/generic_cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/cluster_based_user_credentials.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/cluster_based_user_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/credentials.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/token_credentials.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/token_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/credentials/user_credentials.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/credentials/user_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/data/global_pull_secret_data.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/data/global_pull_secret_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/oc.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/oc.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/openshift_api_manager.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/openshift_api_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/auths_dict.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/auths_dict.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/catalog_source.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/catalog_source.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/credentials.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/custom_resource.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/custom_resource.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/custom_resource_event_result.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/custom_resource_event_result.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/get_pod_entry.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/get_pod_entry.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/kind_metadata.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/kind_metadata.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/object_meta.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/object_meta.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/operator_group.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/operator_group.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/role.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/role.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/role_binding.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/role_binding.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/role_rule.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/role_rule.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/service_account.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/service_account.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/types/subscription.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/types/subscription.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/openshift/utils/click.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/openshift/utils/click.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/plugin_manager/distribution_entry_point_loader.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/plugin_manager/distribution_entry_point_loader.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/plugin_manager/package_data.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/plugin_manager/package_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/lib/plugin_manager/plugin_manager.py` & `cloud-pak-operations-cli-0.4.2/cpo/lib/plugin_manager/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/scripts/get_current_cluster_alias.py` & `cloud-pak-operations-cli-0.4.2/cpo/scripts/get_current_cluster_alias.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/compression.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/compression.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/debugger.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/debugger.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/download.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/download.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/error.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/error.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/file.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/file.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/http_method.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/http_method.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/importlib.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/importlib.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/logging.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/network.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/network.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/operating_system.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/operating_system.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/path.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/path.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/process.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/process.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/ssh.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/cpo/utils/wait.py` & `cloud-pak-operations-cli-0.4.2/cpo/utils/wait.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.4.1/pyproject.toml` & `cloud-pak-operations-cli-0.4.2/pyproject.toml`

 * *Files identical despite different names*

